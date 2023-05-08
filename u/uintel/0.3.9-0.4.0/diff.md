# Comparing `tmp/uintel-0.3.9.tar.gz` & `tmp/uintel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uintel-0.3.9.tar", last modified: Wed Feb 15 21:55:52 2023, max compression
+gzip compressed data, was "uintel-0.4.0.tar", last modified: Mon May  8 03:36:13 2023, max compression
```

## Comparing `uintel-0.3.9.tar` & `uintel-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.340139 uintel-0.3.9/
--rw-rw-rw-   0        0        0     1096 2023-01-18 03:00:37.000000 uintel-0.3.9/LICENSE
--rw-rw-rw-   0        0        0     4118 2023-02-15 21:55:52.333917 uintel-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3336 2023-02-10 03:40:36.000000 uintel-0.3.9/README.md
--rw-rw-rw-   0        0        0       97 2023-01-18 03:00:38.000000 uintel-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-15 21:55:52.341108 uintel-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1591 2023-02-15 21:55:25.000000 uintel-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.127353 uintel-0.3.9/src/
-drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.251396 uintel-0.3.9/src/uintel/
--rw-rw-rw-   0        0        0     3122 2023-02-15 03:54:11.000000 uintel-0.3.9/src/uintel/__init__.py
--rw-rw-rw-   0        0        0     8130 2023-01-26 03:30:11.000000 uintel-0.3.9/src/uintel/aws.py
--rw-rw-rw-   0        0        0     4751 2023-02-15 04:36:27.000000 uintel-0.3.9/src/uintel/colours.py
--rw-rw-rw-   0        0        0    10867 2023-02-15 21:52:53.000000 uintel-0.3.9/src/uintel/esri.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.315724 uintel-0.3.9/src/uintel/fonts/
--rw-rw-rw-   0        0        0    94884 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/fonts/Myriad Pro (TrueType).ttf
--rw-rw-rw-   0        0        0   208636 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/fonts/Rubik (TrueType).ttf
--rw-rw-rw-   0        0        0   202424 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/fonts/Rubik Italic (TrueType).ttf
--rw-rw-rw-   0        0        0    20653 2023-02-12 21:37:30.000000 uintel-0.3.9/src/uintel/geometry.py
--rw-rw-rw-   0        0        0    23622 2023-02-15 00:53:18.000000 uintel-0.3.9/src/uintel/install.py
--rw-rw-rw-   0        0        0     2353 2023-01-30 21:31:25.000000 uintel-0.3.9/src/uintel/ogc.py
--rw-rw-rw-   0        0        0     3869 2023-02-10 05:41:23.000000 uintel-0.3.9/src/uintel/query.py
--rw-rw-rw-   0        0        0     8139 2023-01-23 22:19:34.000000 uintel-0.3.9/src/uintel/server.py
--rw-rw-rw-   0        0        0    14891 2023-01-23 21:02:38.000000 uintel-0.3.9/src/uintel/slack.py
--rw-rw-rw-   0        0        0     3222 2023-01-23 21:00:27.000000 uintel-0.3.9/src/uintel/sql.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.323234 uintel-0.3.9/src/uintel/styles/
--rw-rw-rw-   0        0        0     1096 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/styles/ui.mplstyle
-drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.291282 uintel-0.3.9/src/uintel.egg-info/
--rw-rw-rw-   0        0        0     4118 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/top_level.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:36:13.632856 uintel-0.4.0/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.0/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:36:13.632856 uintel-0.4.0/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.0/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.0/pyproject.toml
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-08 03:36:13.632856 uintel-0.4.0/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-05-08 03:36:03.000000 uintel-0.4.0/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:36:13.624856 uintel-0.4.0/src/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:36:13.628856 uintel-0.4.0/src/uintel/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.0/src/uintel/aws.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/colours.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.0/src/uintel/esri.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:36:13.632856 uintel-0.4.0/src/uintel/fonts/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/fonts/Myriad Pro (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/fonts/Rubik (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/fonts/Rubik Italic (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)    20290 2023-05-05 02:33:43.000000 uintel-0.4.0/src/uintel/geometry.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/install.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/ogc.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/query.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.0/src/uintel/server.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.0/src/uintel/slack.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6388 2023-05-08 03:33:42.000000 uintel-0.4.0/src/uintel/sql.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:36:13.632856 uintel-0.4.0/src/uintel/styles/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.0/src/uintel/styles/ui.mplstyle
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:36:13.628856 uintel-0.4.0/src/uintel.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:36:13.000000 uintel-0.4.0/src/uintel.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-05-08 03:36:13.000000 uintel-0.4.0/src/uintel.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-08 03:36:13.000000 uintel-0.4.0/src/uintel.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-05-08 03:36:13.000000 uintel-0.4.0/src/uintel.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-05-08 03:36:13.000000 uintel-0.4.0/src/uintel.egg-info/top_level.txt
```

### Comparing `uintel-0.3.9/LICENSE` & `uintel-0.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Urban Intelligence
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Urban Intelligence
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `uintel-0.3.9/PKG-INFO` & `uintel-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-Metadata-Version: 2.1
-Name: uintel
-Version: 0.3.9
-Summary: Urban Intelligence's unified Python data analysis toolkit
-Home-page: https://uintel.github.io/pyui/
-Author: Sam Archie
-Author-email: sam.archie@urbanintelligence.co.nz
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
-
-<div align="center">
-  <img src="https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"><br>
-</div>
-
------------------
-
-# uintel: unified Python data analysis toolkit
-[![PyPI Latest Release](https://img.shields.io/pypi/v/uintel.svg)](https://pypi.org/project/uintel/)
-[![License](https://img.shields.io/pypi/l/uintel.svg)](https://github.com/uintel/pyui/blob/main/LICENSE)
-
-## What is it?
-
-**uintel** is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts. 
-
-
-## Main Features
-
-  - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
-  - Creating colour palettes relating to Urban Intelligence's main products
-  - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
-  - Bulk querying (public and private) ESRI servers to download geometric data with attributes
-  - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
-  - Quickly send messages or files to a Slack channel or person
-  - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
-  - Quickly convert a GeoDataFrame to a simplified topojson file
-  - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
-  - Determine the fastest transportation route between a set of origins and destinations
-
-## Where to get it
-The source code is currently hosted on GitHub at: [https://github.com/uintel/pyui](https://github.com/uintel/pyui)
-
-Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/uintel) by running:
-
-```sh
-pip install uintel
-```
-
-> If `pip install uintel` fails due to required packages that are known to be tricky, such as GDAL, the binary distributions can be downloaded from: [https://www.lfd.uci.edu/~gohlke/pythonlibs](https://www.lfd.uci.edu/~gohlke/pythonlibs). 
-
-> For more convenience on Windows, `pip install pipwin` and `pipwin install gdal` is an approach that downloads the right binary wheel from Christoph Gohlke.
-
-> For Linux distributions, check the available version of GDAL by running `ogrinfo --version` and then perform `pip install gdal==available_version`. Typically on our analyst computers, the available version is 3.0.4.
-
-## Configuration
-Each time ```uintel``` is imported,
-
-```py
-import uintel as ui
-```
-
-all necessary installations shall begin that have not been completed before. This will include creating a configuration file, installing fonts and modifying matplotlib - if it has not been done so before.
-
-If you have adjusted your computer and the UI defaults have altered, you can revert them by running:
-
-```py
-ui.reset_fonts()
-ui.reset_styles()
-ui.reset_config()
-```
-
-## Documentation
-Documentation is available at [https://uintel.github.io/pyui/](https://uintel.github.io/pyui/)
+Metadata-Version: 2.1
+Name: uintel
+Version: 0.4.0
+Summary: Urban Intelligence's unified Python data analysis toolkit
+Home-page: https://uintel.github.io/pyui/
+Author: Sam Archie
+Author-email: sam.archie@urbanintelligence.co.nz
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
+Description-Content-Type: text/markdown
+Provides-Extra: full
+License-File: LICENSE
+
+<div align="center">
+  <img src="https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"><br>
+</div>
+
+-----------------
+
+# uintel: unified Python data analysis toolkit
+[![PyPI Latest Release](https://img.shields.io/pypi/v/uintel.svg)](https://pypi.org/project/uintel/)
+[![License](https://img.shields.io/pypi/l/uintel.svg)](https://github.com/uintel/pyui/blob/main/LICENSE)
+
+## What is it?
+
+**uintel** is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts. 
+
+
+## Main Features
+
+  - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
+  - Creating colour palettes relating to Urban Intelligence's main products
+  - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
+  - Bulk querying (public and private) ESRI servers to download geometric data with attributes
+  - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
+  - Quickly send messages or files to a Slack channel or person
+  - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
+  - Quickly convert a GeoDataFrame to a simplified topojson file
+  - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
+  - Determine the fastest transportation route between a set of origins and destinations
+
+## Where to get it
+The source code is currently hosted on GitHub at: [https://github.com/uintel/pyui](https://github.com/uintel/pyui)
+
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/uintel) by running:
+
+```sh
+pip install uintel
+```
+
+> If `pip install uintel` fails due to required packages that are known to be tricky, such as GDAL, the binary distributions can be downloaded from: [https://www.lfd.uci.edu/~gohlke/pythonlibs](https://www.lfd.uci.edu/~gohlke/pythonlibs). 
+
+> For more convenience on Windows, `pip install pipwin` and `pipwin install gdal` is an approach that downloads the right binary wheel from Christoph Gohlke.
+
+> For Linux distributions, check the available version of GDAL by running `ogrinfo --version` and then perform `pip install gdal==available_version`. Typically on our analyst computers, the available version is 3.0.4.
+
+## Configuration
+Each time ```uintel``` is imported,
+
+```py
+import uintel as ui
+```
+
+all necessary installations shall begin that have not been completed before. This will include creating a configuration file, installing fonts and modifying matplotlib - if it has not been done so before.
+
+If you have adjusted your computer and the UI defaults have altered, you can revert them by running:
+
+```py
+ui.reset_fonts()
+ui.reset_styles()
+ui.reset_config()
+```
+
+## Documentation
+Documentation is available at [https://uintel.github.io/pyui/](https://uintel.github.io/pyui/)
```

### Comparing `uintel-0.3.9/README.md` & `uintel-0.4.0/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-<div align="center">
-  <img src="docs/images/blue_logo.svg"><br>
-</div>
-
------------------
-
-# uintel: unified Python data analysis toolkit
-[![PyPI Latest Release](https://img.shields.io/pypi/v/uintel.svg)](https://pypi.org/project/uintel/)
-[![License](https://img.shields.io/pypi/l/uintel.svg)](https://github.com/uintel/pyui/blob/main/LICENSE)
-
-## What is it?
-
-**uintel** is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts. 
-
-
-## Main Features
-
-  - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
-  - Creating colour palettes relating to Urban Intelligence's main products
-  - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
-  - Bulk querying (public and private) ESRI servers to download geometric data with attributes
-  - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
-  - Quickly send messages or files to a Slack channel or person
-  - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
-  - Quickly convert a GeoDataFrame to a simplified topojson file
-  - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
-  - Determine the fastest transportation route between a set of origins and destinations
-
-## Where to get it
-The source code is currently hosted on GitHub at: [https://github.com/uintel/pyui](https://github.com/uintel/pyui)
-
-Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/uintel) by running:
-
-```sh
-pip install uintel
-```
-
-> If `pip install uintel` fails due to required packages that are known to be tricky, such as GDAL, the binary distributions can be downloaded from: [https://www.lfd.uci.edu/~gohlke/pythonlibs](https://www.lfd.uci.edu/~gohlke/pythonlibs). 
-
-> For more convenience on Windows, `pip install pipwin` and `pipwin install gdal` is an approach that downloads the right binary wheel from Christoph Gohlke.
-
-> For Linux distributions, check the available version of GDAL by running `ogrinfo --version` and then perform `pip install gdal==available_version`. Typically on our analyst computers, the available version is 3.0.4.
-
-## Configuration
-Each time ```uintel``` is imported,
-
-```py
-import uintel as ui
-```
-
-all necessary installations shall begin that have not been completed before. This will include creating a configuration file, installing fonts and modifying matplotlib - if it has not been done so before.
-
-If you have adjusted your computer and the UI defaults have altered, you can revert them by running:
-
-```py
-ui.reset_fonts()
-ui.reset_styles()
-ui.reset_config()
-```
-
-## Documentation
-Documentation is available at [https://uintel.github.io/pyui/](https://uintel.github.io/pyui/)
+<div align="center">
+  <img src="docs/images/blue_logo.svg"><br>
+</div>
+
+-----------------
+
+# uintel: unified Python data analysis toolkit
+[![PyPI Latest Release](https://img.shields.io/pypi/v/uintel.svg)](https://pypi.org/project/uintel/)
+[![License](https://img.shields.io/pypi/l/uintel.svg)](https://github.com/uintel/pyui/blob/main/LICENSE)
+
+## What is it?
+
+**uintel** is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts. 
+
+
+## Main Features
+
+  - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
+  - Creating colour palettes relating to Urban Intelligence's main products
+  - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
+  - Bulk querying (public and private) ESRI servers to download geometric data with attributes
+  - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
+  - Quickly send messages or files to a Slack channel or person
+  - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
+  - Quickly convert a GeoDataFrame to a simplified topojson file
+  - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
+  - Determine the fastest transportation route between a set of origins and destinations
+
+## Where to get it
+The source code is currently hosted on GitHub at: [https://github.com/uintel/pyui](https://github.com/uintel/pyui)
+
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/uintel) by running:
+
+```sh
+pip install uintel
+```
+
+> If `pip install uintel` fails due to required packages that are known to be tricky, such as GDAL, the binary distributions can be downloaded from: [https://www.lfd.uci.edu/~gohlke/pythonlibs](https://www.lfd.uci.edu/~gohlke/pythonlibs). 
+
+> For more convenience on Windows, `pip install pipwin` and `pipwin install gdal` is an approach that downloads the right binary wheel from Christoph Gohlke.
+
+> For Linux distributions, check the available version of GDAL by running `ogrinfo --version` and then perform `pip install gdal==available_version`. Typically on our analyst computers, the available version is 3.0.4.
+
+## Configuration
+Each time ```uintel``` is imported,
+
+```py
+import uintel as ui
+```
+
+all necessary installations shall begin that have not been completed before. This will include creating a configuration file, installing fonts and modifying matplotlib - if it has not been done so before.
+
+If you have adjusted your computer and the UI defaults have altered, you can revert them by running:
+
+```py
+ui.reset_fonts()
+ui.reset_styles()
+ui.reset_config()
+```
+
+## Documentation
+Documentation is available at [https://uintel.github.io/pyui/](https://uintel.github.io/pyui/)
```

### Comparing `uintel-0.3.9/src/uintel/__init__.py` & `uintel-0.4.0/src/uintel/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""Urban Intelligence's collection of Python code for everyday use.
-
-uintel is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts.
-
-Main Features
-    - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
-    - Creating colour palettes relating to Urban Intelligence's main products
-    - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
-    - Bulk querying (public and private) ESRI servers to download geometric data with attributes
-    - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
-    - Quickly send messages or files to a Slack channel or person
-    - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
-    - Quickly convert a GeoDataFrame to a simplified topojson file
-    - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
-"""
-
-from . import install as _install
-
-def reset_fonts() -> None:
-    """Force re-install all fonts.
-
-    Reinstalls all Urban Intelligence fonts back to defaults.
-
-    Args: 
-        None
-    
-    Returns:
-        None
-    
-    Raises:
-        None
-    """
-    _install._install_fonts(force=True, verbose=True)
-
-
-def reset_styles() -> None:
-    """Force re-install all matplotlib styles.
-    
-    Reinstalls all Urban Intelligence matplotlib styles (*.mplstyle files in /fonts) back to defaults.
-
-    Args: 
-        None
-    
-    Returns:
-        None
-    
-    Raises:
-        None
-
-    """
-    _install._install_styles(force=True, verbose=True)
-
-
-def reset_config() -> None:
-    """Force re-make the configuration file, in case at least one saved bit of information needs updating.
-    
-    Remakes the configuration file, regardless if it exists or is is up to date.
-
-    Args: 
-        None
-    
-    Returns:
-        None
-    
-    Raises:
-        None
-    """
-    _install._create_config_file()
-
-
-def save_config(config: dict) -> None:
-    """Save the configuration file.
-    
-    Saves the configuration to disk, regardless if it exists or is up to date.
-
-    Args: 
-        config: A dictionary of the Urban Intelligence configurations
-    
-    Returns:
-        None
-    
-    Raises:
-        None
-    """
-    _install._save_config(config)
-
-
-_install._update_config_file()
-_install._install_styles(force=False, verbose=True)
-_install._install_fonts(force=False, verbose=True)
-
-from . import aws, colours, esri, geometry, server, slack, sql, ogc
+"""Urban Intelligence's collection of Python code for everyday use.
+
+uintel is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts.
+
+Main Features
+    - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
+    - Creating colour palettes relating to Urban Intelligence's main products
+    - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
+    - Bulk querying (public and private) ESRI servers to download geometric data with attributes
+    - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
+    - Quickly send messages or files to a Slack channel or person
+    - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
+    - Quickly convert a GeoDataFrame to a simplified topojson file
+    - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
+"""
+
+from . import install as _install
+
+def reset_fonts() -> None:
+    """Force re-install all fonts.
+
+    Reinstalls all Urban Intelligence fonts back to defaults.
+
+    Args: 
+        None
+    
+    Returns:
+        None
+    
+    Raises:
+        None
+    """
+    _install._install_fonts(force=True, verbose=True)
+
+
+def reset_styles() -> None:
+    """Force re-install all matplotlib styles.
+    
+    Reinstalls all Urban Intelligence matplotlib styles (*.mplstyle files in /fonts) back to defaults.
+
+    Args: 
+        None
+    
+    Returns:
+        None
+    
+    Raises:
+        None
+
+    """
+    _install._install_styles(force=True, verbose=True)
+
+
+def reset_config() -> None:
+    """Force re-make the configuration file, in case at least one saved bit of information needs updating.
+    
+    Remakes the configuration file, regardless if it exists or is is up to date.
+
+    Args: 
+        None
+    
+    Returns:
+        None
+    
+    Raises:
+        None
+    """
+    _install._create_config_file()
+
+
+def save_config(config: dict) -> None:
+    """Save the configuration file.
+    
+    Saves the configuration to disk, regardless if it exists or is up to date.
+
+    Args: 
+        config: A dictionary of the Urban Intelligence configurations
+    
+    Returns:
+        None
+    
+    Raises:
+        None
+    """
+    _install._save_config(config)
+
+
+_install._update_config_file()
+_install._install_styles(force=False, verbose=True)
+_install._install_fonts(force=False, verbose=True)
+
+from . import aws, colours, esri, geometry, server, slack, sql, ogc
 __all__ = ["aws", "colours","esri", "geometry", "server", "slack", "sql", "ogc"]
```

### Comparing `uintel-0.3.9/src/uintel/aws.py` & `uintel-0.4.0/src/uintel/aws.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-"""
-Connecting and utilising Amazon Web Services (AWS).
-
-This module allows easy uploading to and downloading from S3 buckets. More importantly as data caching is enabled for some dashboards, versioning is taken care of by removing previous versions and updating the versions.json file on S3. 
-
-"""
-
-__all__ = ["upload_file_to_S3", "download_file_from_S3", "update_S3_versions", "remove_previous_versions", "get_S3_client"]
-
-import boto3, json, os, tqdm, threading, tempfile, botocore.exceptions
-from typing import Optional
-
-
-def create_aws_client(service: str, region: str = "ap-southeast-2") -> boto3.client:
-    """Create an AWS client.
-
-    Return an AWS client connected to one service by using the credentials file at ~/.aws/credentials.
-
-    Args:
-        service: Which AWS service to connect to. E.g. 's3'.
-        region: The AWS region to connect to.
-    
-    Returns:
-        A boto3.client connected to the requested AWS service and region.
-    
-    """
-    try:
-        return boto3.client(service, region_name=region)
-    except botocore.exceptions.NoCredentialsError as error:
-        print("""\033[91mFor first-timers, be sure to generate a credentials file as ~/.aws/credentials with the following information:
-        [default]
-        aws_access_key_id = ********
-        aws_secret_access_key = ***********\n    
-        If that does not fix this, then please investigate the following error\033[0m""")
-        raise error
-    except Exception as error:
-        raise error
-
-
-def upload_file_to_S3(local_filepath: str, remote_filepath: str, s3_client: boto3.client = None, bucket: str = "urbanintelligencedevdata", extra_args: dict = None) -> None:
-    """Upload a file to an AWS S3 bucket.
-
-    Upload a file at local_filepath to the remote_filepath in a given AWS S3 bucket. 
-    
-    Args:
-        local_filepath: Filepath that is to be uploaded.
-        remote_filepath: Filepath to put the file in the AWS S3 bucket. The remote_filepath should be in the format: '/data/project_name/version/filename' like 'data/mrapple/1.4.5/growth_statistics.csv'.
-        s3_client: A boto3.client that is connected to the S3 service.
-        bucket: The AWS S3 bucket to upload the file to.
-        extra_args: A dictionary of additional arguments to upload the file with. To make the file not cache for end-users, use: extra_args={'Metadata': {'CacheControl': 'no-store'}}.
-
-    Returns:
-        None.
-    """
-    if not s3_client:
-        s3_client = create_aws_client('s3')
-    s3_client.upload_file(local_filepath, bucket, remote_filepath, ExtraArgs=extra_args, Callback=_ProgressBar(local_filepath))
-
-
-def download_file_from_S3(remote_filepath: str, local_filepath: str, s3_client: boto3.client = None, bucket: str = "urbanintelligencedevdata") -> None:
-    """Download a file from an AWS S3 bucket.
-
-    Download a file at remote_filepath to the local_filepath from a given AWS S3 bucket. 
-
-    Args:
-        remote_filepath: Filepath in the AWS S3 bucket to download. The remote_filepath should be in the format: '/data/project_name/version/filename' like 'data/mrapple/1.4.5/growth_statistics.csv'.
-        local_filepath: Filepath where the downloaded file should be saved.
-        s3_client: A boto3.client that is connected to the S3 service.
-        bucket: The AWS S3 bucket to upload the file to.
-    
-    Returns:
-        None.
-    """
-    if not s3_client:
-        s3_client = create_aws_client('s3')
-    s3_client.download_file(bucket, remote_filepath, local_filepath)
-
-
-def update_S3_versions(project_name: str, dev_version: Optional[str] = None, test_version: Optional[str] = None, prod_version: Optional[str] = None) -> None:
-    """Update the data/version.json file with new versioning.
-
-    Edit the data/versions.json file on the S3 bucket to the new versions provided for each domain (dev/test/prod) on a given project_name. If ther project_name is not in versions.json, it is added.
-
-    Args:
-        project_name: Project name in versions.json to update/add.
-        dev_version: Version to update the development dashboard to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'. If dev_version=None, the current will remain unchanged.
-        test_version: Version to update the testing dashboard to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'. If test_version=None, the current will remain unchanged.
-        prod_version: Version to update the production dashboard to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'. If prod_version=None, the current will remain unchanged.
-
-    Returns:
-        None.
-    """
-
-    # Create a temporary directory to download version.json in
-    tempdir = tempfile.TemporaryDirectory()
-    tempfile_name = os.path.join(tempdir.name, "versions.json")
-
-    # Download the current versions.json file
-    s3_client = create_aws_client('s3')
-    download_file_from_S3("data/versions.json", tempfile_name, s3_client)
-
-    # Read the file and make the necessary changes as requested
-    with open(tempfile_name, "r") as file:
-        versions = json.load(file)
-
-    if dev_version:
-        versions[project_name]["dev"] = dev_version
-    if test_version:
-        versions[project_name]["test"] = test_version
-    if prod_version:
-        versions[project_name]["production"] = prod_version
-
-    with open(tempfile_name, "w") as file:
-        json.dump(versions, file, indent=4)
-
-    # Upload the modified versions.json to the bucket with no caching allowed
-    upload_file_to_S3(tempfile_name, "data/versions.json", s3_client, extra_args={'Metadata': {'CacheControl': 'no-store'}})
-    s3_client.close()
-    
-    tempdir.cleanup()
-
-
-def remove_previous_versions(project_name: str, current_version: str, bucket: str = "urbanintelligencedevdata") -> None:
-    """Delete all versions (excluding the current) from a project.
-
-    Delete ALL files and folders (except the current_version) for a given project_name from the given AWS S3 bucket.
-
-    Args:
-        project_name: Project name in versions.json to update/add.
-        current_version: Current version of the project to keep to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'.
-        bucket: The AWS S3 bucket to remove the previous versions from.
-
-    Returns:
-        None.
-    """
-
-    # Get all the subfolders and objects within this project folder
-    s3_client =  create_aws_client('s3')
-    result = s3_client.list_objects(Bucket=bucket, Prefix=f"data/{project_name}/", Delimiter='/')
-    version_folders = [version_folder.get('Prefix') for version_folder in result.get('CommonPrefixes')]
-    s3_client.close()
-
-    # Obviosuly, we should not delete the folder with the new data in it!
-    version_folders.remove(f"data/{project_name}/{current_version}/")
-
-    # The client can tag objections for deletion, but can't go ahead with it. Hence, use the Bucket Resource.
-    bucket_client = boto3.resource('s3').Bucket(bucket) ### boto3.resource is not be supported soon. Better find a way around this before it happens
-    for version_folder in version_folders:
-        bucket_client.objects.filter(Prefix=version_folder).delete()
-    
-
-class _ProgressBar(object):
-    """Display the progress of an uploading file.
-
-    Using a tqdm progress bar, indicate the progress of an uploading file. This is to be used in the Callback function as the ProgressBar class will be updated on each call.
-
-    Attributes:
-        None.
-    """
-    
-    def __init__(self, filename: str):
-        """Initialises ProgressBar to be zero."""
-        self._size = float(os.path.getsize(filename))
-        self._seen_so_far = 0
-        self._lock = threading.Lock()
-        self.pbar = tqdm.tqdm(desc=f"Uploading {filename}", total=100, leave=False, dynamic_ncols=True)
-
-    def __call__(self, bytes_uploaded: float):
-        """Update the progress bar with the bytes_uploaded and refresh the percentage bar."""
-        with self._lock:
-            self._seen_so_far += bytes_uploaded
-            self.pbar.n = round((self._seen_so_far / self._size) * 100, 2)
+"""
+Connecting and utilising Amazon Web Services (AWS).
+
+This module allows easy uploading to and downloading from S3 buckets. More importantly as data caching is enabled for some dashboards, versioning is taken care of by removing previous versions and updating the versions.json file on S3. 
+
+"""
+
+__all__ = ["upload_file_to_S3", "download_file_from_S3", "update_S3_versions", "remove_previous_versions", "get_S3_client"]
+
+import boto3, json, os, tqdm, threading, tempfile, botocore.exceptions
+from typing import Optional
+
+
+def create_aws_client(service: str, region: str = "ap-southeast-2", **kwargs) -> boto3.client:
+    """Create an AWS client.
+
+    Return an AWS client connected to one service by using the credentials file at ~/.aws/credentials.
+
+    Args:
+        service: Which AWS service to connect to. E.g. 's3'.
+        region: The AWS region to connect to.
+    
+    Returns:
+        A boto3.client connected to the requested AWS service and region.
+    
+    """
+    try:
+        return boto3.client(service, region_name=region, **kwargs)
+    except botocore.exceptions.NoCredentialsError as error:
+        print("""\033[91mFor first-timers, be sure to generate a credentials file as ~/.aws/credentials with the following information:
+        [default]
+        aws_access_key_id = ********
+        aws_secret_access_key = ***********\n    
+        If that does not fix this, then please investigate the following error\033[0m""")
+        raise error
+    except Exception as error:
+        raise error
+
+
+def upload_file_to_S3(local_filepath: str, remote_filepath: str, s3_client: boto3.client = None, bucket: str = "urbanintelligencedevdata", extra_args: dict = None) -> None:
+    """Upload a file to an AWS S3 bucket.
+
+    Upload a file at local_filepath to the remote_filepath in a given AWS S3 bucket. 
+    
+    Args:
+        local_filepath: Filepath that is to be uploaded.
+        remote_filepath: Filepath to put the file in the AWS S3 bucket. The remote_filepath should be in the format: '/data/project_name/version/filename' like 'data/mrapple/1.4.5/growth_statistics.csv'.
+        s3_client: A boto3.client that is connected to the S3 service.
+        bucket: The AWS S3 bucket to upload the file to.
+        extra_args: A dictionary of additional arguments to upload the file with. To make the file not cache for end-users, use: extra_args={'Metadata': {'CacheControl': 'no-store'}}.
+
+    Returns:
+        None.
+    """
+    if not s3_client:
+        s3_client = create_aws_client('s3')
+    s3_client.upload_file(local_filepath, bucket, remote_filepath, ExtraArgs=extra_args, Callback=_ProgressBar(local_filepath))
+
+
+def download_file_from_S3(remote_filepath: str, local_filepath: str, s3_client: boto3.client = None, bucket: str = "urbanintelligencedevdata") -> None:
+    """Download a file from an AWS S3 bucket.
+
+    Download a file at remote_filepath to the local_filepath from a given AWS S3 bucket. 
+
+    Args:
+        remote_filepath: Filepath in the AWS S3 bucket to download. The remote_filepath should be in the format: '/data/project_name/version/filename' like 'data/mrapple/1.4.5/growth_statistics.csv'.
+        local_filepath: Filepath where the downloaded file should be saved.
+        s3_client: A boto3.client that is connected to the S3 service.
+        bucket: The AWS S3 bucket to upload the file to.
+    
+    Returns:
+        None.
+    """
+    if not s3_client:
+        s3_client = create_aws_client('s3')
+    s3_client.download_file(bucket, remote_filepath, local_filepath)
+
+
+def update_S3_versions(project_name: str, dev_version: Optional[str] = None, test_version: Optional[str] = None, prod_version: Optional[str] = None) -> None:
+    """Update the data/version.json file with new versioning.
+
+    Edit the data/versions.json file on the S3 bucket to the new versions provided for each domain (dev/test/prod) on a given project_name. If ther project_name is not in versions.json, it is added.
+
+    Args:
+        project_name: Project name in versions.json to update/add.
+        dev_version: Version to update the development dashboard to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'. If dev_version=None, the current will remain unchanged.
+        test_version: Version to update the testing dashboard to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'. If test_version=None, the current will remain unchanged.
+        prod_version: Version to update the production dashboard to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'. If prod_version=None, the current will remain unchanged.
+
+    Returns:
+        None.
+    """
+
+    # Create a temporary directory to download version.json in
+    tempdir = tempfile.TemporaryDirectory()
+    tempfile_name = os.path.join(tempdir.name, "versions.json")
+
+    # Download the current versions.json file
+    s3_client = create_aws_client('s3')
+    download_file_from_S3("data/versions.json", tempfile_name, s3_client)
+
+    # Read the file and make the necessary changes as requested
+    with open(tempfile_name, "r") as file:
+        versions = json.load(file)
+
+    if dev_version:
+        versions[project_name]["dev"] = dev_version
+    if test_version:
+        versions[project_name]["test"] = test_version
+    if prod_version:
+        versions[project_name]["production"] = prod_version
+
+    with open(tempfile_name, "w") as file:
+        json.dump(versions, file, indent=4)
+
+    # Upload the modified versions.json to the bucket with no caching allowed
+    upload_file_to_S3(tempfile_name, "data/versions.json", s3_client, extra_args={'Metadata': {'CacheControl': 'no-store'}})
+    s3_client.close()
+    
+    tempdir.cleanup()
+
+
+def remove_previous_versions(project_name: str, current_version: str, bucket: str = "urbanintelligencedevdata") -> None:
+    """Delete all versions (excluding the current) from a project.
+
+    Delete ALL files and folders (except the current_version) for a given project_name from the given AWS S3 bucket.
+
+    Args:
+        project_name: Project name in versions.json to update/add.
+        current_version: Current version of the project to keep to. E.g. '1.9.2', '2023_12_18', 'v1.2.8'.
+        bucket: The AWS S3 bucket to remove the previous versions from.
+
+    Returns:
+        None.
+    """
+
+    # Get all the subfolders and objects within this project folder
+    s3_client =  create_aws_client('s3')
+    result = s3_client.list_objects(Bucket=bucket, Prefix=f"data/{project_name}/", Delimiter='/')
+    version_folders = [version_folder.get('Prefix') for version_folder in result.get('CommonPrefixes')]
+    s3_client.close()
+
+    # Obviosuly, we should not delete the folder with the new data in it!
+    version_folders.remove(f"data/{project_name}/{current_version}/")
+
+    # The client can tag objections for deletion, but can't go ahead with it. Hence, use the Bucket Resource.
+    bucket_client = boto3.resource('s3').Bucket(bucket) ### boto3.resource is not be supported soon. Better find a way around this before it happens
+    for version_folder in version_folders:
+        bucket_client.objects.filter(Prefix=version_folder).delete()
+    
+
+class _ProgressBar(object):
+    """Display the progress of an uploading file.
+
+    Using a tqdm progress bar, indicate the progress of an uploading file. This is to be used in the Callback function as the ProgressBar class will be updated on each call.
+
+    Attributes:
+        None.
+    """
+    
+    def __init__(self, filename: str):
+        """Initialises ProgressBar to be zero."""
+        self._size = float(os.path.getsize(filename))
+        self._seen_so_far = 0
+        self._lock = threading.Lock()
+        self.pbar = tqdm.tqdm(desc=f"Uploading {filename}", total=100, leave=False, dynamic_ncols=True)
+
+    def __call__(self, bytes_uploaded: float):
+        """Update the progress bar with the bytes_uploaded and refresh the percentage bar."""
+        with self._lock:
+            self._seen_so_far += bytes_uploaded
+            self.pbar.n = round((self._seen_so_far / self._size) * 100, 2)
             self.pbar.refresh()
```

### Comparing `uintel-0.3.9/src/uintel/colours.py` & `uintel-0.4.0/src/uintel/colours.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""Generate colours to the Urban Intelligence style guide.
-
-This module aims to assist in creating figures to a single style across the organisation. The colour palletes are engrained in this module and the core function is to modify the pallete to fit the need of the users figure.
-"""
-
-__all__ = ["generate_colour_palette", "get_colour"]
-
-import colour as _colour_module
-from typing import Union
-
-__ALLOWABLE_FORMATS = ['hex', 'rgb', 'hsl']
-
-__COLOUR_PALETTES = {
-    "planning": {
-        "monochromatic": ["#5aa33b", "#48942e", "#358520", "#207611", "#006700"],
-        "divergent": ["#5aa33b", "#76b05a", "#8fbd77", "#a8ca95", "#c0d7b3", "#d9e4d2", "#f1f1f1", "#f1d4d4", "#f0b8b8", "#ec9c9d", "#e67f83", "#de6069", "#d43d51"], 
-    },
-    "access": {
-        "monochromatic": ["#246783", "#21779a", "#1b86b2", "#1396cb", "#09a7e5", "#00b7ff"],
-        "divergent": ["#246783", "#307d91", "#44929d", "#5ca8a8", "#78beb1", "#97d3bb", "#93daa7", "#9fdd8c", "#b7de6a", "#d8dc44", "#ffd416"], 
-    },
-    "risk": {
-        "monochromatic": ["#0b2948", "#344a69", "#596d8d", "#7f93b1", "#a7bad8", "#d1e3ff"],
-        "divergent": ["#0b2948", "#3b4b67", "#657187", "#9198a8", "#bfc2ca", "#eeeeee", "#fad3c1", "#ffb896", "#ff9d6b", "#fe813f", "#f86302"], 
-    }
-}
-
-__UI_COLOURS = {
-    # Add new UI colours here!
-    "dark blue": "#0b2948",
-    "secondary blue": "#04497c",
-    "orange": "#f86302",
-    "red": "#e70e02",
-    "pink": "#ff8fa3",
-    "light blue": "#00b7ff",
-    "dark green": "#006700",
-    "light green": "#",
-    "white": "#ffffff",
-    "black": "#000000",
-}
-
-AVAILABLE_COLOURS = list(__UI_COLOURS.keys())
-
-def generate_colour_palette(palette: str = "risk", scheme: str = "divergent", n: int = 5, format: str = "hex") -> list:
-    """Generate a specific colour palette resembling a Urban Intelligence product.
-
-    Return a list of colours that relate to an Urban Intelligence colour palette (planning, access or risk) for a given colour scheme (monochromatic or divergent). Colours are always returned in the order of positive to worst (in respect of what the palette is defining as a good and poor colour).
-
-    Args:
-        palette: The Urban Intelligence product to mimic the palette off.
-        scheme: The colour scheme required ('divergent' or 'monochromatic').
-        n: The number of unique colours required.
-    
-    Returns:
-        A list of n colours relating to the requested palette and scheme.
-    """
-
-    if palette not in __COLOUR_PALETTES.keys():
-        raise ValueError(f"The given pallete: {palette} is not acceptable. Please choose from: {list(__COLOUR_PALETTES.keys())}")
-    if scheme not in __COLOUR_PALETTES[palette].keys():
-        raise ValueError(f"The given scheme: {scheme} is not acceptable. Please choose from: {list(__COLOUR_PALETTES[palette].keys())}")
-    assert n > 0 and type(n) == int, "The requested number of colours ('n') must be a positive integer."
-
-    default_colours = __COLOUR_PALETTES[palette][scheme]
-    if len(default_colours) == 0:
-        raise NotImplementedError(f"Unfortunately, there is no colour scheme for the {palette} palette using a {scheme} scheme. Apologies for the inconvenience.")
-    elif len(default_colours) == n:
-        # A perfect match!
-        return [_colour_module.Color(colour).__getattribute__(f"get_{format}")() for colour in default_colours]
-    elif n == 1:
-        # If requested only one colour, return the first one
-        return [_colour_module.Color(default_colours[0]).__getattribute__(f"get_{format}")()]
-    else:
-        # Create a range of colours with n steps between the two ends
-        return [color.__getattribute__(f"get_{format}")() for color in _colour_module.Color(default_colours[0]).range_to(_colour_module.Color(default_colours[-1]), steps=n)]
-
-
-def get_colour(name: str = "dark blue", format: str = "hex") -> Union[str, tuple]:
-    """Get one specific colour, by name.
-
-    Return a colour that relates to an Urban Intelligence product, by name. See uintel.colours.AVAILABLE_COLOURS for a list of available colour names.
-
-    Args:
-        name: The name of the colour to return.
-        format: The format the colour should be returned as
-    
-    Returns:
-        The value of the requested colour in the requested format.
-    """
-    if name not in __UI_COLOURS:
-        raise ValueError(f"The given name: {name} is not acceptable. Please choose from: {list(__UI_COLOURS.keys())}")
-    if format not in __ALLOWABLE_FORMATS:
-        raise ValueError(f"The given format: {format} is not acceptable. Please choose from: {__ALLOWABLE_FORMATS}")
-    return _colour_module.Color(__UI_COLOURS[name]).__getattribute__(f"get_{format}")()
+"""Generate colours to the Urban Intelligence style guide.
+
+This module aims to assist in creating figures to a single style across the organisation. The colour palletes are engrained in this module and the core function is to modify the pallete to fit the need of the users figure.
+"""
+
+__all__ = ["generate_colour_palette", "get_colour"]
+
+import colour as _colour_module
+from typing import Union
+
+__ALLOWABLE_FORMATS = ['hex', 'rgb', 'hsl']
+
+__COLOUR_PALETTES = {
+    "planning": {
+        "monochromatic": ["#5aa33b", "#48942e", "#358520", "#207611", "#006700"],
+        "divergent": ["#5aa33b", "#76b05a", "#8fbd77", "#a8ca95", "#c0d7b3", "#d9e4d2", "#f1f1f1", "#f1d4d4", "#f0b8b8", "#ec9c9d", "#e67f83", "#de6069", "#d43d51"], 
+    },
+    "access": {
+        "monochromatic": ["#246783", "#21779a", "#1b86b2", "#1396cb", "#09a7e5", "#00b7ff"],
+        "divergent": ["#246783", "#307d91", "#44929d", "#5ca8a8", "#78beb1", "#97d3bb", "#93daa7", "#9fdd8c", "#b7de6a", "#d8dc44", "#ffd416"], 
+    },
+    "risk": {
+        "monochromatic": ["#0b2948", "#344a69", "#596d8d", "#7f93b1", "#a7bad8", "#d1e3ff"],
+        "divergent": ["#0b2948", "#3b4b67", "#657187", "#9198a8", "#bfc2ca", "#eeeeee", "#fad3c1", "#ffb896", "#ff9d6b", "#fe813f", "#f86302"], 
+    }
+}
+
+__UI_COLOURS = {
+    # Add new UI colours here!
+    "dark blue": "#0b2948",
+    "secondary blue": "#04497c",
+    "orange": "#f86302",
+    "red": "#e70e02",
+    "pink": "#ff8fa3",
+    "light blue": "#00b7ff",
+    "dark green": "#006700",
+    "light green": "#",
+    "white": "#ffffff",
+    "black": "#000000",
+}
+
+AVAILABLE_COLOURS = list(__UI_COLOURS.keys())
+
+def generate_colour_palette(palette: str = "risk", scheme: str = "divergent", n: int = 5, format: str = "hex") -> list:
+    """Generate a specific colour palette resembling a Urban Intelligence product.
+
+    Return a list of colours that relate to an Urban Intelligence colour palette (planning, access or risk) for a given colour scheme (monochromatic or divergent). Colours are always returned in the order of positive to worst (in respect of what the palette is defining as a good and poor colour).
+
+    Args:
+        palette: The Urban Intelligence product to mimic the palette off.
+        scheme: The colour scheme required ('divergent' or 'monochromatic').
+        n: The number of unique colours required.
+    
+    Returns:
+        A list of n colours relating to the requested palette and scheme.
+    """
+
+    if palette not in __COLOUR_PALETTES.keys():
+        raise ValueError(f"The given pallete: {palette} is not acceptable. Please choose from: {list(__COLOUR_PALETTES.keys())}")
+    if scheme not in __COLOUR_PALETTES[palette].keys():
+        raise ValueError(f"The given scheme: {scheme} is not acceptable. Please choose from: {list(__COLOUR_PALETTES[palette].keys())}")
+    assert n > 0 and type(n) == int, "The requested number of colours ('n') must be a positive integer."
+
+    default_colours = __COLOUR_PALETTES[palette][scheme]
+    if len(default_colours) == 0:
+        raise NotImplementedError(f"Unfortunately, there is no colour scheme for the {palette} palette using a {scheme} scheme. Apologies for the inconvenience.")
+    elif len(default_colours) == n:
+        # A perfect match!
+        return [_colour_module.Color(colour).__getattribute__(f"get_{format}")() for colour in default_colours]
+    elif n == 1:
+        # If requested only one colour, return the first one
+        return [_colour_module.Color(default_colours[0]).__getattribute__(f"get_{format}")()]
+    else:
+        # Create a range of colours with n steps between the two ends
+        return [color.__getattribute__(f"get_{format}")() for color in _colour_module.Color(default_colours[0]).range_to(_colour_module.Color(default_colours[-1]), steps=n)]
+
+
+def get_colour(name: str = "dark blue", format: str = "hex") -> Union[str, tuple]:
+    """Get one specific colour, by name.
+
+    Return a colour that relates to an Urban Intelligence product, by name. See uintel.colours.AVAILABLE_COLOURS for a list of available colour names.
+
+    Args:
+        name: The name of the colour to return.
+        format: The format the colour should be returned as
+    
+    Returns:
+        The value of the requested colour in the requested format.
+    """
+    if name not in __UI_COLOURS:
+        raise ValueError(f"The given name: {name} is not acceptable. Please choose from: {list(__UI_COLOURS.keys())}")
+    if format not in __ALLOWABLE_FORMATS:
+        raise ValueError(f"The given format: {format} is not acceptable. Please choose from: {__ALLOWABLE_FORMATS}")
+    return _colour_module.Color(__UI_COLOURS[name]).__getattribute__(f"get_{format}")()
```

### Comparing `uintel-0.3.9/src/uintel/esri.py` & `uintel-0.4.0/src/uintel/esri.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,199 +1,196 @@
-"""Connect to and download ESRI services.
-
-Bulk querying and downloading of geometric data hosted on an ESRI FeatureService, MapService or ImageServer. When the Service is private, authentication is attempted using saved credentials in the project file.
-"""
-
-__all__ = ["get_data", "generate_token"]
-
-import geopandas as gpd, requests, esridump, esridump.errors, yaml
-import typing, subprocess, logging, os
-
-logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
-logger = logging.getLogger(__name__)
-
-
-def get_data(url: str, layer: int = None, projection: int = 2193, verbose: bool = False, assume_data_type: str = "Feature Layer", boundary: gpd.GeoDataFrame = None) -> gpd.GeoDataFrame:
-    """Query an ESRI service and return data.
-    
-    The main function to call to return an ESRI REST MapServer, FeatureService or ImageServer. The url is verified to ensure a layer number is within the url, and gathers any query parameters that were added in the url. An automatic attempt is made to see if the Service contains vector or raster geometry, and thhe appropiate downloading methodology is chosen.
-    
-    Args:
-        url: String of the ESRI Service. E.g. https://services7.arcgis.com/NNoivt2IKUC8czGf/arcgis/rest/services/NZTA_One_Road/FeatureServer.
-        layer: If the layer number is not provided at the end of the url, this parameter should be the layer number you wish to get.
-        projection: Integer of the CRS that the data should be returned in.
-        verbose: Display progress of the downloading procedure and assumptions made if verbose=True. Otherwise, logging is kept to errors or above.
-        assume_data_type: If the automatic attempt of determining the type of the Service fails, the assume_data_type is used instead. Hence, assume_data_type should either be: "Feature Service" or "Raster Layer".
-        bbox: A tuple of values in the given projection to limit the returned results of the query
-
-    Returns:
-        For vector Services, a geopandas.GeoDataFrame (for vector data) is returned.
-    
-    Raises:
-        NotImplementedError: Raised if the Service is a MapServer or ImageServer.
-    """
-    
-    # Verify the given endpoint is okay
-    url, query_parameters = _check_url(url, layer, boundary)
-    # Check the type of data of the endpoint so we know which method to download as
-    response = requests.get(url + '?f=json')
-    if response.ok:
-        results = response.json()
-        data_type = results.get("type", None)
-        if not data_type and 'pixelType' in results:
-            data_type = "Raster Layer"
-        elif not data_type:
-            data_type = assume_data_type
-    else:
-        data_type = assume_data_type
-
-    if data_type == "Feature Layer":
-        # Grab the features using the esridumps package and return as a GeoDataFrame
-        return _download_vector_endpoint(url, query_parameters, projection, verbose)
-
-    elif data_type == "Raster Layer":
-        # Return the server as an numpy array?
-        return _download_raster_endpoint(url, query_parameters, projection)
-
-
-def _check_url(url: str, layer: int = None, boundary: gpd.GeoDataFrame = None) -> typing.Tuple[str, dict]:
-    """Ensure the url is valid.
-
-    Check to see if the given url was valid by ensuring it is correctly formatted with the layer number if it is a MapServer or FeatureSever.
-
-    Args: 
-        url: String of the ESRI Service. E.g. https://services7.arcgis.com/NNoivt2IKUC8czGf/arcgis/rest/services/NZTA_One_Road/FeatureServer.
-        layer: If the layer number is not provided at the end of the url, this parameter should be the layer number you wish to get.
-    
-    Returns:
-        The verified url and a dictionary of query parameters. If not query parameters are were in the original url, then the defaul query parameters are returned.
-    """
-
-    # Check to see if there are query parmeters already in the given end_point_url
-    if 'query?' in url:
-        # Drop the url part
-        query_parameters_str = url[url.index('query?'):].replace("query?", "")
-        # Build a dictionary of key:values for each parameter
-        query_parameters = {}
-        for query_combo in query_parameters_str.split("&"):
-            query_parameters[query_combo.split("=")[0]] = query_combo.split("=")[1]
-        if "%3D" in query_parameters.get("where", ""):
-            query_parameters["where"] = query_parameters["where"].replace("%3D", "=")
-        if "f" in query_parameters:
-            del query_parameters["f"]
-        # Set the url as everything before the query parameters
-        url = url[:url.index('query?')]
-    else:
-        # Set as default query parameters
-        query_parameters = {'where': '1=1', 'outFields': '*'}
-        if boundary:
-            minx, miny, maxx, maxy = boundary.bounds.values[0]
-            query_parameters["geometry"] = f"geometryType=esriGeometryEnvelope&geometry={minx},{miny},{maxx},{maxy}"
-            query_parameters["geometryType"] = "esriGeometryEnvelope"
-            query_parameters["inSR"] = boundary.crs.to_wkt()
-            query_parameters["spatialRel"] = "esriSpatialRelIntersects"
-    
-    if not url.endswith('/'):
-        # Map Server URL needs a slash at the end
-        url += '/' 
-    
-    if url.endswith("FeatureServer/") or url.endswith("MapServer/"):
-        if layer:
-            url += f"{layer}/"
-        else:
-            raise RuntimeError(f"No layer number was inputted to the function, and it was not found within the url: {url}. Please ensure a layer number is inputted.")
-        
-    return url, query_parameters
-
-
-def _download_vector_endpoint(url: str, query_parameters: dict, projection: int, verbose: bool) -> gpd.GeoDataFrame:
-    """
-    Return an ESRI REST FeatureService Layer (which contains vector geometries) as a GeoDataFrame. The most efficient way of downloading the Layer, given the host's configurations, is chosen based on https://github.com/openaddresses/pyesridump#methodology.
-    """
-
-    if not verbose:
-        # Shut the logger from spitting out shit by force setting to ERROR level
-        logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.ERROR, datefmt='%Y-%m-%d %H:%M:%S', force=True)
- 
-    try:
-        # Try downloading the data and see if we get stopped
-        endpoint_data = gpd.GeoDataFrame.from_features(list(esridump.EsriDumper(url=url, outSR=projection, request_geometry=True, extra_query_args=query_parameters, pause_seconds=0, timeout=120)))
-        if len(endpoint_data) > 0:
-            endpoint_data.set_crs(projection, inplace=True)
-        else:
-            endpoint_data = gpd.GeoDataFrame(crs=projection)  
-
-    except esridump.errors.EsriDownloadError as error:
-        if "Token Required" in str(error):
-            # Then we have an endpoint that requires authentication. The best way to generate a token is using the Arcpy package that is only available in the arcgispro virtual environment
-            arcgis_venv_path = r'C:\Program Files\ArcGIS\Pro\bin\Python\envs\arcgispro-py3\python.exe'
-            if not os.path.exists(arcgis_venv_path):
-                raise RuntimeError("Unfortunately, a token is required and you do not have ArcGIS Pro installed on this device. We are unable to generate a token, so please move onto a device that has ArcGIS installed.")
-
-            # Get the login details from a saved file
-            credentials_savepath = os.path.join(os.getcwd(), "config", "esri.yaml")
-            if os.path.exists(credentials_savepath):
-                credentials = yaml.load(credentials_savepath)
-            else:
-                print("No credentials could be found for this project.")
-                credentials = {
-                    "username": input("What is your Esri login username? "),
-                    "password": input("What is your Esri login password? ")
-                }
-                os.makedirs(credentials_savepath, exist_ok=True)
-                yaml.dump(credentials, open(credentials_savepath, "w"))
-            
-            # Generate a token in this script which outputs the token in the stdout
-            res = subprocess.run([arcgis_venv_path, __file__, "token", credentials["username"], credentials["password"]], capture_output=True)
-            if res.returncode == 0:
-                query_parameters.update({"token": res.stdout.decode()})
-                try:
-                    endpoint_data =  gpd.GeoDataFrame.from_features(list(esridump.EsriDumper(url=url, outSR=projection, request_geometry=True, extra_query_args=query_parameters, pause_seconds=0, timeout=120))).set_crs(projection, inplace=True)
-                except esridump.errors.EsriDownloadError as error2:
-                    # Token failed to fix the error.
-                    raise esridump.errors.EsriDownloadError(f"The generated token did not fix the EsriDownloadError, albeit it said a token was required. Please address the new error: \n{error2.reason}")
-            
-            else:
-                # Token failed to be made. This should never happen but leave a catch clause in here. 
-                raise esridump.errors.EsriDownloadError(f"{url} requires authentication. However, the automatically generated token led to a further issue when trying to be created: \n{res.reason}")
-        else:
-            raise error
-    
-    except Exception as error:
-        # Catch all other errors
-        raise error
-
-    if not verbose:
-        # Return logger to INFO level
-        logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S', force=True)
-    
-    return endpoint_data
-
-
-def _download_raster_endpoint(url: str, query_parameters: dict, projection: int) -> None:
-    """
-    Return an ESRI REST MapService Layer (which contains raster information).
-    """
-    # url = "https://gisimagery.ecan.govt.nz/arcgis/rest/services/Elevation/Latest_DEM/ImageServer"
-    raise NotImplementedError("Sorry, rasters aren't ready yet!")
-
-
-def generate_token(username: str, password: str) -> str:
-    """Generate a token.
-    
-    Generate a token using Esri login details. This must be run in an virtual environment (typically 'arcgispro') where the arcgis package is available.
-    
-    Args:
-        username: The username to connect to ESRI
-        password: The password to connect to ESRI
-
-    Returns:
-        A valid ESRI token  
-    """
-    import arcgis.gis
-    return arcgis.gis.GIS("https://www.arcgis.com/", username, password)._con.token
-
-
-if __name__ == "__main__":
-    import sys
-    if sys.argv[2] == "token":
+"""Connect to and download ESRI services.
+
+Bulk querying and downloading of geometric data hosted on an ESRI FeatureService, MapService or ImageServer. When the Service is private, authentication is attempted using saved credentials in the project file.
+"""
+
+__all__ = ["get_data", "generate_token"]
+
+import geopandas as gpd, requests, esridump, esridump.errors, yaml
+import typing, subprocess, logging, os
+
+logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
+logger = logging.getLogger(__name__)
+
+
+def get_data(url: str, layer: int = None, projection: int = 2193, verbose: bool = False, assume_data_type: str = "Feature Layer", boundary: gpd.GeoDataFrame = None) -> gpd.GeoDataFrame:
+    """Query an ESRI service and return data.
+    
+    The main function to call to return an ESRI REST MapServer, FeatureService or ImageServer. The url is verified to ensure a layer number is within the url, and gathers any query parameters that were added in the url. An automatic attempt is made to see if the Service contains vector or raster geometry, and thhe appropiate downloading methodology is chosen.
+    
+    Args:
+        url: String of the ESRI Service. E.g. https://services7.arcgis.com/NNoivt2IKUC8czGf/arcgis/rest/services/NZTA_One_Road/FeatureServer.
+        layer: If the layer number is not provided at the end of the url, this parameter should be the layer number you wish to get.
+        projection: Integer of the CRS that the data should be returned in.
+        verbose: Display progress of the downloading procedure and assumptions made if verbose=True. Otherwise, logging is kept to errors or above.
+        assume_data_type: If the automatic attempt of determining the type of the Service fails, the assume_data_type is used instead. Hence, assume_data_type should either be: "Feature Service" or "Raster Layer".
+        bbox: A tuple of values in the given projection to limit the returned results of the query
+
+    Returns:
+        For vector Services, a geopandas.GeoDataFrame (for vector data) is returned.
+    
+    Raises:
+        NotImplementedError: Raised if the Service is a MapServer or ImageServer.
+    """
+    
+    # Verify the given endpoint is okay
+    url, query_parameters = _check_url(url, layer, boundary)
+    # Check the type of data of the endpoint so we know which method to download as
+    response = requests.get(url + '?f=json')
+    if response.ok:
+        results = response.json()
+        data_type = results.get("type", None)
+        if not data_type and 'pixelType' in results:
+            data_type = "Raster Layer"
+        elif not data_type:
+            data_type = assume_data_type
+    else:
+        data_type = assume_data_type
+
+    if data_type == "Feature Layer":
+        # Grab the features using the esridumps package and return as a GeoDataFrame
+        return _download_vector_endpoint(url, query_parameters, projection, verbose)
+
+    elif data_type == "Raster Layer":
+        # Return the server as an numpy array?
+        return _download_raster_endpoint(url, query_parameters, projection)
+
+
+def _check_url(url: str, layer: int = None, boundary: gpd.GeoDataFrame = None) -> typing.Tuple[str, dict]:
+    """Ensure the url is valid.
+
+    Check to see if the given url was valid by ensuring it is correctly formatted with the layer number if it is a MapServer or FeatureSever.
+
+    Args: 
+        url: String of the ESRI Service. E.g. https://services7.arcgis.com/NNoivt2IKUC8czGf/arcgis/rest/services/NZTA_One_Road/FeatureServer.
+        layer: If the layer number is not provided at the end of the url, this parameter should be the layer number you wish to get.
+    
+    Returns:
+        The verified url and a dictionary of query parameters. If not query parameters are were in the original url, then the defaul query parameters are returned.
+    """
+
+    # Check to see if there are query parmeters already in the given end_point_url
+    if 'query?' in url:
+        # Drop the url part
+        query_parameters_str = url[url.index('query?'):].replace("query?", "")
+        # Build a dictionary of key:values for each parameter
+        query_parameters = {}
+        for query_combo in query_parameters_str.split("&"):
+            query_parameters[query_combo.split("=")[0]] = query_combo.split("=")[1]
+        if "%3D" in query_parameters.get("where", ""):
+            query_parameters["where"] = query_parameters["where"].replace("%3D", "=")
+        if "f" in query_parameters:
+            del query_parameters["f"]
+        # Set the url as everything before the query parameters
+        url = url[:url.index('query?')]
+    else:
+        # Set as default query parameters
+        query_parameters = {'where': '1=1', 'outFields': '*'}
+        if type(boundary) == gpd.GeoDataFrame:
+            minx, miny, maxx, maxy = boundary.bounds.values[0]
+            query_parameters["geometry"] = f"geometryType=esriGeometryEnvelope&geometry={minx},{miny},{maxx},{maxy}"
+            query_parameters["geometryType"] = "esriGeometryEnvelope"
+            query_parameters["inSR"] = {"wkt": boundary.crs.to_wkt()}
+            query_parameters["spatialRel"] = "esriSpatialRelIntersects"
+    
+    if not url.endswith('/'):
+        # Map Server URL needs a slash at the end
+        url += '/' 
+    
+    if url.endswith("FeatureServer/") or url.endswith("MapServer/"):
+        if layer:
+            url += f"{layer}/"
+        else:
+            raise RuntimeError(f"No layer number was inputted to the function, and it was not found within the url: {url}. Please ensure a layer number is inputted.")
+        
+    return url, query_parameters
+
+
+def _download_vector_endpoint(url: str, query_parameters: dict, projection: int, verbose: bool) -> gpd.GeoDataFrame:
+    """
+    Return an ESRI REST FeatureService Layer (which contains vector geometries) as a GeoDataFrame. The most efficient way of downloading the Layer, given the host's configurations, is chosen based on https://github.com/openaddresses/pyesridump#methodology.
+    """
+
+    if not verbose:
+        # Shut the logger from spitting out shit by force setting to ERROR level
+        logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.ERROR, datefmt='%Y-%m-%d %H:%M:%S', force=True)
+ 
+    try:
+        # Try downloading the data and see if we get stopped
+        endpoint_data = gpd.GeoDataFrame.from_features(list(esridump.EsriDumper(url=url, outSR=projection, request_geometry=True, extra_query_args=query_parameters, pause_seconds=0, timeout=120)))
+        if len(endpoint_data) > 0:
+            endpoint_data.set_crs(projection, inplace=True)
+    except esridump.errors.EsriDownloadError as error:
+        if "Token Required" in str(error):
+            # Then we have an endpoint that requires authentication. The best way to generate a token is using the Arcpy package that is only available in the arcgispro virtual environment
+            arcgis_venv_path = r'C:\Program Files\ArcGIS\Pro\bin\Python\envs\arcgispro-py3\python.exe'
+            if not os.path.exists(arcgis_venv_path):
+                raise RuntimeError("Unfortunately, a token is required and you do not have ArcGIS Pro installed on this device. We are unable to generate a token, so please move onto a device that has ArcGIS installed.")
+
+            # Get the login details from a saved file
+            credentials_savepath = os.path.join(os.getcwd(), "config", "esri.yaml")
+            if os.path.exists(credentials_savepath):
+                credentials = yaml.load(credentials_savepath)
+            else:
+                print("No credentials could be found for this project.")
+                credentials = {
+                    "username": input("What is your Esri login username? "),
+                    "password": input("What is your Esri login password? ")
+                }
+                os.makedirs(credentials_savepath, exist_ok=True)
+                yaml.dump(credentials, open(credentials_savepath, "w"))
+            
+            # Generate a token in this script which outputs the token in the stdout
+            res = subprocess.run([arcgis_venv_path, __file__, "token", credentials["username"], credentials["password"]], capture_output=True)
+            if res.returncode == 0:
+                query_parameters.update({"token": res.stdout.decode()})
+                try:
+                    endpoint_data =  gpd.GeoDataFrame.from_features(list(esridump.EsriDumper(url=url, outSR=projection, request_geometry=True, extra_query_args=query_parameters, pause_seconds=0, timeout=120))).set_crs(projection, inplace=True)
+                except esridump.errors.EsriDownloadError as error2:
+                    # Token failed to fix the error.
+                    raise esridump.errors.EsriDownloadError(f"The generated token did not fix the EsriDownloadError, albeit it said a token was required. Please address the new error: \n{error2.reason}")
+            
+            else:
+                # Token failed to be made. This should never happen but leave a catch clause in here. 
+                raise esridump.errors.EsriDownloadError(f"{url} requires authentication. However, the automatically generated token led to a further issue when trying to be created: \n{res.reason}")
+        else:
+            raise error
+    
+    except Exception as error:
+        # Catch all other errors
+        raise error
+
+    if not verbose:
+        # Return logger to INFO level
+        logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S', force=True)
+    
+    return endpoint_data
+
+
+def _download_raster_endpoint(url: str, query_parameters: dict, projection: int) -> None:
+    """
+    Return an ESRI REST MapService Layer (which contains raster information).
+    """
+    # url = "https://gisimagery.ecan.govt.nz/arcgis/rest/services/Elevation/Latest_DEM/ImageServer"
+    raise NotImplementedError("Sorry, rasters aren't ready yet!")
+
+
+def generate_token(username: str, password: str) -> str:
+    """Generate a token.
+    
+    Generate a token using Esri login details. This must be run in an virtual environment (typically 'arcgispro') where the arcgis package is available.
+    
+    Args:
+        username: The username to connect to ESRI
+        password: The password to connect to ESRI
+
+    Returns:
+        A valid ESRI token  
+    """
+    import arcgis.gis
+    return arcgis.gis.GIS("https://www.arcgis.com/", username, password)._con.token
+
+
+if __name__ == "__main__":
+    import sys
+    if sys.argv[2] == "token":
         sys.stdout.write(generate_token(sys.argv[3], sys.argv[4]))
```

### Comparing `uintel-0.3.9/src/uintel/fonts/Myriad Pro (TrueType).ttf` & `uintel-0.4.0/src/uintel/fonts/Myriad Pro (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.3.9/src/uintel/fonts/Rubik (TrueType).ttf` & `uintel-0.4.0/src/uintel/fonts/Rubik (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.3.9/src/uintel/fonts/Rubik Italic (TrueType).ttf` & `uintel-0.4.0/src/uintel/fonts/Rubik Italic (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.3.9/src/uintel/geometry.py` & `uintel-0.4.0/src/uintel/geometry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,345 +1,346 @@
-"""
-Tools related to geometric items:
-
-- Quickly convert a GeoDataFrame to a simplified topojson file
-- Calculate statistics of raster files over a polygon geometry ("zonal statistics")
-"""
-
-__all__ = ["save_geodataframe_as_topojson", "calculate_zonal_statistics"]
-
-import tempfile, warnings, geopandas as gpd, numpy as np, pandas as pd, os, topojson as tp, tqdm
-from typing import Optional
-
-def save_geodataframe_as_topojson(gdf: gpd.GeoDataFrame, save_path: str, simplify_factor: Optional[float] = None) -> None:
-    """Save a geopandas.GeoDataFrame as a .topojson file.
-
-    Convert a [multi-geometry type or single-geometry type] geodataframe to a topojson file, optimised for the web by simplyfing geometries in EPSG:4326. 
-    
-    Args:
-        gdf: The GeoDataFrame to convert to a topojson.
-        save_path: The filepath to save the topojson to.
-        simplify_factor: Apply toposimplify to remove unnecessary points from polylines and polygons after the topology is constructed. Sensible values for coordinates stored in degrees are in the range of 0.0001 to 10. If None, then no toposimplify is performed.
-    
-    Returns:
-        None.
-    """
-    
-    # Make a temporary directory to save shapefile and topojsons to
-    temp_dir = tempfile.TemporaryDirectory()
-    warnings.filterwarnings("ignore")
-    
-    # Drop duplicates and prepare the dataset
-    gdf.drop_duplicates(inplace=True)
-    gdf.reset_index(drop=True, inplace=True)
-    if not gdf.crs:
-        raise RuntimeError("The geodataframe does not have an associated CRS. Please add one and try again.")
-    gdf.to_crs("EPSG:4326", inplace=True)
-    
-    # Split the GeoDataFrame into the 3 main geometry types
-    points = gdf[gdf.geom_type.isin(["Point", "MultiPoint"])]
-    polylines = gdf[gdf.geom_type.isin(["Polyline", "LineString"])]
-    polygons = gdf[gdf.geom_type.isin(["Polygon", "MulitPolygon"])]
-    
-    # Make a geojson dictionary to add all the features to
-    final_shp = gpd.GeoDataFrame()
-
-    for (geom_type, shapefile) in [("point", points), ("polyline", polylines), ("polygon", polygons)]:
-        if len(shapefile) > 0:           
-            # Make sure all geometry is good! You can't use pass to topojson if there is invalid geometry!
-            valid_geometry = shapefile.is_valid
-            if not valid_geometry.all():
-                if geom_type == "polyline":
-                    # An error occurs "too few points in geometry component" and this is as the line is clipped and there is no length to it! We can't buffer it and there isn't a nice way to fix it unfortunately. Revisit: ST_MakeValid in SQL could be a go?. Hence, only retain the good geometry
-                    warnings.warn(f"{len(valid_geometry)-valid_geometry.sum()} LineString geometries could not be saved to the topojson file as they are invalid. The cause of this may be due to a very small line length. These geometries have been skipped in the meantime.")
-                    shapefile = shapefile[valid_geometry]
-                else:
-                    # Usually a polygon asset doesn't have any errors when buffer is used!
-                    shapefile.loc[~valid_geometry, "geometry"] = shapefile.loc[~valid_geometry, "geometry"].buffer(0)
-
-            # Simplify the geometry
-            if not simplify_factor or type(simplify_factor) not in (float, int) or geom_type == "point":
-                shapefile = tp.Topology(shapefile, prequantize=False).to_gdf(crs="EPSG:4326")
-            else:
-                shapefile = tp.Topology(shapefile, prequantize=False, toposimplify=simplify_factor, prevent_oversimplify=True).to_gdf(crs="EPSG:4326")
-                        
-            # A stupid error occurs in opening topojsons in the website where there are NaN values! They occur in the id column which has been dropped, but just in case, replace them with none values.
-            if "id" in shapefile.columns:
-                shapefile.drop(columns="id", inplace=True)
-            
-            # Change the dtypes of the columns
-            for column_name in shapefile.columns.tolist():
-                if column_name == "asset_id":
-                    # Reduce dtypes
-                    if shapefile["asset_id"].max() < 127:
-                        shapefile["asset_id"] = shapefile["asset_id"].astype('uint8')
-                    elif shapefile["asset_id"].max() < 32767:
-                        shapefile["asset_id"] = shapefile["asset_id"].astype('uint16')
-                    else:
-                        shapefile["asset_id"] = shapefile["asset_id"].astype('uint32')
-                elif column_name == "geometry":
-                    continue
-                else:
-                    # Assume every other column is categorical
-                    shapefile[column_name] = shapefile[column_name].astype('object')
-            
-            # Replace any bad geometries after the simplification procedure, with the original unsimplified geometry. Perhaps we could use a different (like a backup) simplification factor that is less, but seeing as its only a few geometries then we may as well use the original geometry. 
-            geometry_is_valid = np.logical_and(shapefile.is_valid, ~shapefile.is_empty)
-            gdf_geometry_is_valid = np.logical_and(gdf.is_valid, ~gdf.is_empty)
-            if geometry_is_valid.sum() != len(geometry_is_valid):
-                # Then there is at least one geometry that is invalid after simplification.
-                shapefile = pd.concat([shapefile[geometry_is_valid], gdf[~gdf_geometry_is_valid]]).sort_index()
-            # Add to the overall shapefile
-            final_shp = pd.concat([final_shp, shapefile], ignore_index=False).sort_index()
-
-    # Remove all the temporary files made
-    temp_dir.cleanup()
-    if not os.path.exists(os.path.dirname(save_path)):
-        os.makedirs(os.path.dirname(save_path))
-    # Convert the overall shapefile to a Topology object and save it
-    tp.Topology(final_shp, prequantize=False).to_json(save_path)
-
-
-def _boundingBoxToOffsets(vector_bbox, raster_geotransform):
-    col1 = int((vector_bbox[0] - raster_geotransform[0]) / raster_geotransform[1])
-    col2 = int((vector_bbox[1] - raster_geotransform[0]) / raster_geotransform[1]) + 1
-    row1 = int((vector_bbox[3] - raster_geotransform[3]) / raster_geotransform[5])
-    row2 = int((vector_bbox[2] - raster_geotransform[3]) / raster_geotransform[5]) + 1
-    return [row1, row2, col1, col2]
-
-
-def _geotFromOffsets(row_offset, col_offset, raster_geotransform):
-    return [raster_geotransform[0] + (col_offset * raster_geotransform[1]), raster_geotransform[1], 0.0, raster_geotransform[3] + (row_offset * raster_geotransform[5]), 0.0, raster_geotransform[5]]
-
-
-def _check_inputted_datasets(raster_path, vector_path):
-    """
-    Run compatibility checks to ensure:
-        - Files exist
-        - Vector file only contains Polygons
-        - Geographic projections match
-    """
-    try:
-        import rasterio as rio
-    except ModuleNotFoundError:
-        raise ModuleNotFoundError("RasterIO could not be located. Please install rasterio seperately into this Python environment, or run 'pip install uintel[full]'")
-
-    # Do some checks to make sure the vector file input is okay
-    if type(vector_path) == gpd.GeoDataFrame:
-        if not os.path.exists("shp-tmp"):
-            os.makedirs("shp-tmp")
-        vector_path.to_file("shp-tmp/vector_file.shp")
-        vector_path = os.path.join(os.getcwd(), "shp-tmp", "vector_file.shp")
-    elif type(vector_path) != str:
-        raise TypeError(f"The vector file must be either a string of the filepath to the shape OR a GeoDataFrame. A {type(vector_path)} is not acceptable.")
-
-    try:
-        vector_file = gpd.read_file(vector_path)
-    except Exception as e:
-        raise e
-
-    geom_types = vector_file.geom_type.unique()
-    if len(geom_types) != 1:
-        raise TypeError(f"The vector file: {vector_path} can only contain Polygon geometries, but it contains {geom_types}. Please correct this before running again.")
-    if geom_types[0] != 'Polygon':
-        raise TypeError(f"The vector file: {vector_path} can only contain Polygon geometries, but it contains {geom_types}. Please correct this before running again.")
-    vector_epsg = vector_file.crs.to_epsg()
-    del vector_file
-
-    # Do some checks to make sure the raster file input is okay
-    if type(raster_path) != str:
-        raise TypeError(f"The raster file must be a string of the filepath to the raster. A {type(vector_path)} is not acceptable.")
-    try:
-        raster_epsg = rio.open(raster_path).crs.to_epsg()
-        if rio.open(raster_path).crs.to_epsg() == None:
-            raster_epsg = 2193
-    except Exception as e:
-        raise e
-
-
-    # Check to see if the projections match
-    if vector_epsg != raster_epsg:
-        if type(raster_epsg) in (int, float):
-            warnings.warn(f"The two inputted datasets are in different projections (raster: {raster_epsg}; vector: {vector_epsg}). An attempt will be made to reproject the vector layer into the projection of the raster. This will change the vector file saved at {vector_path} to EPSG:{raster_epsg}.")
-            try:
-                _ = gpd.read_file(vector_path).to_crs(raster_epsg).to_file(vector_path)
-            except:
-                raise TypeError(f"The automatic attempt at changing projections failed. Please correct this before running again.")
-        else:
-            raise TypeError(f"The two inputted datasets are in different projections (raster: {raster_epsg}; vector: {vector_epsg}). Please correct this before running again.")
-
-    return raster_epsg
-
-
-def _get_raster_array(raster_dataset, offsets, raster_x_size, raster_y_size, raster_band, raster_nodata):
-    """
-    Checks to see if the vector offset geometry lies within the raster dataset, and if so, returns the values from the raster_dataset. If only a proportion of the geometries overlap, then the other pixel values are given the raster_nodata value.
-    """
-
-    # Grab the "normal" parameters to pass to ReadAsArray  
-    y_top, y_bottom, x_left, x_right = offsets         
-    width, height = x_right-x_left, y_bottom-y_top
-   
-    if width == 0 or height == 0:
-        # The  the requested raster has a zero dimension which is invalid
-        return None
-    if x_left > raster_x_size or y_top > raster_y_size:
-        # Then the starting point (top left of the polygon) is outside of the bottom right raster extent
-        return None
-    elif x_right < 0 or y_bottom < 0:
-        # Then the finishing point (bottom right of the polygon) is outside of the top left raster extent
-        return None
-    elif x_left >= 0 and x_right <= raster_x_size and y_top >= 0 and y_bottom <= raster_y_size and width >= 0 and height >= 0:
-        # Then the whole vector geometry is within the raster
-        return raster_dataset.GetRasterBand(raster_band).ReadAsArray(x_left, y_top, width, height)    
-    elif (x_left < 0 or y_top < 0) and x_right > 0 and y_bottom > 0:
-        # Then the starting point (top left of the polygon) is outside of the raster extent
-        # Only some of the vector geometry is within the raster extent so create a full no-data array and overwrite values that exist
-        raster = np.full((height, width), raster_nodata)
-        
-        x_offset, y_offset = 0, 0
-        # Adjust the height and widths to be in the bounds of the raster
-        if x_left < 0:
-            x_offset = -x_left # Move everything left to make x_left = 0
-            width -= x_offset  # sum negative number will reduce the width 
-            x_left = 0
-        if y_top < 0:
-            y_offset = -y_top # Move everything down to make y_top =0 
-            height -= y_offset  # sum negative number will reduce the width
-            y_top = 0
-        if x_right > raster_x_size:
-            width -= (x_right - raster_x_size) # subtract how much over the boundary
-            x_right = raster_x_size
-        if y_bottom > raster_y_size:
-            height -= (y_bottom - raster_y_size) # subtract how much over the boundary
-            y_bottom = raster_y_size
-        raster[y_offset:y_offset+height, x_offset:x_offset+width] = raster_dataset.GetRasterBand(raster_band).ReadAsArray(x_left, y_top, width, height)
-        return raster
-    elif x_left >= 0 and x_left < raster_x_size and y_top >= 0 and y_top < raster_y_size and (x_right > raster_x_size or y_bottom > raster_y_size):
-        # Only some of the vector geometry is within the raster extent so create a full no-data array and overwrite values that exist
-        raster = np.full((height, width), raster_nodata)
-        new_xsize, new_ysize = min(raster_x_size-x_left, width), min(raster_y_size-y_top, height)
-        raster[0:new_ysize, 0:new_xsize] = raster_dataset.GetRasterBand(raster_band).ReadAsArray(x_left, y_top, new_xsize, new_ysize)
-        return raster
-    else:
-        warnings.warn(f"Uncaught case in zonal statistics get_raster_array! Details below:\n bounds = {offsets} with raster extends of {raster_x_size} x {raster_y_size}.")
-
-
-def calculate_zonal_statistics(raster_path: str, vector_path: str, raster_band: int = 1, allow_touching_pixels: bool = True, show_progress: bool = True) -> dict:
-    """Calculate statistics of a raster over a vector geometry.
-
-    Collect stats (min, max, mean, median, std, sum, 10th percentile, 90th percentile and count) on pixel values (raster) which lie within polygons (vector). If allow_touching_pixels is set to True, then any pixel that touches the exterior of the vector geometry is included in the statistics calculation. The returned dictionary has the vector FID as the key, where the values is a dictionary mapping the statistic's name to value.
-    
-    Examples:
-        >>> zonal_statistics = calculate_zonal_statistics("raster.tiff", "vector.shp")
-        >>> zonal_statistics[67] # To get the statistics of the raster over the vector shape with an FID of 67
-        {"min": 0, "max": 10.6, "mean": 2.5, "median": 2.8, "std": 0.6, "sum": 180.8, "count": 72, "90th_percentile": 28,"10th_percentile": 0.2}      
-
-    Args:
-        raster_path: Filepath of where the raster is stored.
-        vector_path: Filepath of where the vector geometry (typically a shapefile) is stored.
-        raster_band: Band of the raster to analyse.
-        allow_touching_pixels: If True, any pixel that touches the exterior of the vector geometry is included in the statistics calculation. Otherwise, the statistics is using pixels within the vector geometry.
-        show_progress: If True, show the progress of calculating the statistics for each vector feature.
-    
-    Returns:
-        A dictionary of nested dictionaries, where the keys are the FID of the vector geometry and the dictionary contains the statistics of the raster over the FID geometry.
-    """
-    try:
-        import osgeo.ogr, osgeo.osr, osgeo.gdal
-    except ModuleNotFoundError:
-        raise ModuleNotFoundError("GDAL could not be located. Please install GDAL seperately into this Python environment, or run 'pip install uintel[full]'")
-    try:
-        import rasterio as rio
-    except ModuleNotFoundError:
-        raise ModuleNotFoundError("RasterIO could not be located. Please install rasterio seperately into this Python environment, or run 'pip install uintel[full]'")
-
-    
-    epsg = _check_inputted_datasets(raster_path, vector_path)
-
-    # Get GDAL driver
-    mem_driver = osgeo.ogr.GetDriverByName("Memory")
-    mem_driver_gdal = osgeo.gdal.GetDriverByName("MEM")
-
-    # Open datasets
-    vector_dataset = osgeo.ogr.Open(vector_path)
-    vector_layer = vector_dataset.GetLayer()
-    raster_dataset = osgeo.gdal.Open(raster_path)
-
-    # Get information about the raster dataset
-    raster_geotransform = raster_dataset.GetGeoTransform()
-    raster_nodata = raster_dataset.GetRasterBand(raster_band).GetNoDataValue()
-    raster_x_size = raster_dataset.RasterXSize
-    raster_y_size = raster_dataset.RasterYSize
-    dest_srs = osgeo.osr.SpatialReference()
-    _ = dest_srs.ImportFromEPSG(epsg)
-
-    # Set up a progress bar if the user wants one
-    if show_progress:
-        progress_bar = tqdm.tqdm(desc="Calculating zonal statistics", total=len(gpd.read_file(vector_path)), leave=False, dynamic_ncols=True)
-
-    # Iterate through each polygon in the shapefile (vector feature)
-    zonal_statistics = {}
-    vector_feature = vector_layer.GetNextFeature()
-    while vector_feature:
-        if vector_feature.GetGeometryRef() is not None:
-            # Create a new driver
-            if os.path.exists("temp"):
-                _ = mem_driver.DeleteDataSource("temp")
-            temporary_dataset = mem_driver.CreateDataSource("temp")
-            
-            # Create a new layer of just the one feature
-            temporary_layer = temporary_dataset.CreateLayer('polygons', dest_srs, osgeo.ogr.wkbPolygon)
-            _ = temporary_layer.CreateFeature(vector_feature.Clone())
-            
-            # Determine the offsets
-            offsets = _boundingBoxToOffsets(vector_feature.GetGeometryRef().GetEnvelope(), raster_geotransform)
-            
-            # Transform from the offsets
-            new_geotransform = _geotFromOffsets(offsets[0], offsets[2], raster_geotransform)
-            
-            # Create a blank transformed dataset
-            transformed_dataset = mem_driver_gdal.Create("", offsets[3] - offsets[2], offsets[1] - offsets[0], 1, osgeo.gdal.GDT_Byte)
-            _ = transformed_dataset.SetGeoTransform(new_geotransform)
-            
-            # Rasterise the transformed dataset to the temporary layer where the array is 1 = touches, 0 = does not touch
-            _= osgeo.gdal.RasterizeLayer(transformed_dataset, [1], temporary_layer, burn_values=[1], options=[f'ALL_TOUCHED={str(allow_touching_pixels).upper()}'])
-            transformed_array = transformed_dataset.ReadAsArray()
-            
-            # Grab the values of the raster that intersect the vector geometry
-            raster_array = _get_raster_array(raster_dataset, offsets, raster_x_size, raster_y_size, raster_band, raster_nodata)
-            
-            id = vector_feature.GetFID()
-            if raster_array is not None and len(raster_array) > 0:
-                # Mask the raster to only cover the vector geometry (transformed array)
-                raster_values_over_vector_feature = raster_array[~np.logical_or(raster_array==raster_nodata, np.logical_not(transformed_array))]
-                if raster_values_over_vector_feature is not None and len(raster_values_over_vector_feature) > 0:
-                    # Then there are some values over the vector feature!!
-                    zonal_statistics[id] = {
-                        "min": raster_values_over_vector_feature.min(),
-                        "max": raster_values_over_vector_feature.max(),
-                        "mean": raster_values_over_vector_feature.mean(),
-                        "median": np.median(raster_values_over_vector_feature),
-                        "std": raster_values_over_vector_feature.std(),
-                        "sum": raster_values_over_vector_feature.sum(),
-                        "count": len(raster_values_over_vector_feature),
-                        "90th_percentile": np.percentile(raster_values_over_vector_feature, 90),
-                        "10th_percentile": np.percentile(raster_values_over_vector_feature, 10)
-                        }      
-                else:
-                    # There are no raster cells overlapping the vector feature
-                    zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": None, "90th_percentile": None, "10th_percentile": None}     
-            else:
-                # There is no raster?
-                zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": None, "90th_percentile": None, "10th_percentile": None}
-            
-            # Clear some memory
-            temporary_dataset = None
-            temporary_layer = None
-            transformed_dataset = None
-            # Repeat with the next polygon geometry
-            vector_feature = vector_layer.GetNextFeature()
-        
-        if show_progress: 
-            _ = progress_bar.update(1)
-
-    return zonal_statistics  
+"""
+Tools related to geometric items:
+
+- Quickly convert a GeoDataFrame to a simplified topojson file
+- Calculate statistics of raster files over a polygon geometry ("zonal statistics")
+"""
+
+__all__ = ["save_geodataframe_as_topojson", "calculate_zonal_statistics"]
+
+import tempfile, warnings, geopandas as gpd, numpy as np, pandas as pd, os, topojson as tp, tqdm
+from typing import Optional
+
+def save_geodataframe_as_topojson(gdf: gpd.GeoDataFrame, save_path: str, simplify_factor: Optional[float] = None) -> None:
+    """Save a geopandas.GeoDataFrame as a .topojson file.
+
+    Convert a [multi-geometry type or single-geometry type] geodataframe to a topojson file, optimised for the web by simplyfing geometries in EPSG:4326. 
+    
+    Args:
+        gdf: The GeoDataFrame to convert to a topojson.
+        save_path: The filepath to save the topojson to.
+        simplify_factor: Apply toposimplify to remove unnecessary points from polylines and polygons after the topology is constructed. Sensible values for coordinates stored in degrees are in the range of 0.0001 to 10. If None, then no toposimplify is performed.
+    
+    Returns:
+        None.
+    """
+    
+    # Make a temporary directory to save shapefile and topojsons to
+    temp_dir = tempfile.TemporaryDirectory()
+    warnings.filterwarnings("ignore")
+    
+    # Drop duplicates and prepare the dataset
+    gdf = gdf.explode(ignore_index=True)
+    gdf.drop_duplicates(inplace=True)
+    gdf.reset_index(drop=True, inplace=True)
+    if not gdf.crs:
+        raise RuntimeError("The geodataframe does not have an associated CRS. Please add one and try again.")
+    gdf.to_crs("EPSG:4326", inplace=True)
+    
+    # Split the GeoDataFrame into the 3 main geometry types
+    points = gdf[gdf.geom_type == "Point"]
+    polylines = gdf[gdf.geom_type == "Polyline"]
+    polygons = gdf[gdf.geom_type == "Polygon"]
+    
+    # Make a geojson dictionary to add all the features to
+    final_shp = gpd.GeoDataFrame()
+
+    for (geom_type, shapefile) in [("point", points), ("polyline", polylines), ("polygon", polygons)]:
+        if len(shapefile) > 0:           
+            # Make sure all geometry is good! You can't use pass to topojson if there is invalid geometry!
+            valid_geometry = shapefile.is_valid
+            if not valid_geometry.all():
+                if geom_type == "polyline":
+                    # An error occurs "too few points in geometry component" and this is as the line is clipped and there is no length to it! We can't buffer it and there isn't a nice way to fix it unfortunately. Revisit: ST_MakeValid in SQL could be a go?. Hence, only retain the good geometry
+                    warnings.warn(f"{len(valid_geometry)-valid_geometry.sum()} LineString geometries could not be saved to the topojson file as they are invalid. The cause of this may be due to a very small line length. These geometries have been skipped in the meantime.")
+                    shapefile = shapefile[valid_geometry]
+                else:
+                    # Usually a polygon asset doesn't have any errors when buffer is used!
+                    shapefile.loc[~valid_geometry, "geometry"] = shapefile.loc[~valid_geometry, "geometry"].buffer(0)
+
+            # Simplify the geometry
+            if not simplify_factor or type(simplify_factor) not in (float, int) or geom_type == "point":
+                shapefile = tp.Topology(shapefile, prequantize=False).to_gdf(crs="EPSG:4326")
+            else:
+                shapefile = tp.Topology(shapefile, prequantize=False, toposimplify=simplify_factor, prevent_oversimplify=True).to_gdf(crs="EPSG:4326")
+                        
+            # A stupid error occurs in opening topojsons in the website where there are NaN values! They occur in the id column which has been dropped, but just in case, replace them with none values.
+            if "id" in shapefile.columns:
+                shapefile.drop(columns="id", inplace=True)
+            
+            # Change the dtypes of the columns
+            for column_name in shapefile.columns.tolist():
+                if column_name == "asset_id":
+                    # Reduce dtypes
+                    if shapefile["asset_id"].max() < 127:
+                        shapefile["asset_id"] = shapefile["asset_id"].astype('uint8')
+                    elif shapefile["asset_id"].max() < 32767:
+                        shapefile["asset_id"] = shapefile["asset_id"].astype('uint16')
+                    else:
+                        shapefile["asset_id"] = shapefile["asset_id"].astype('uint32')
+                elif column_name == "geometry":
+                    continue
+                else:
+                    # Assume every other column is categorical
+                    shapefile[column_name] = shapefile[column_name].astype('object')
+            
+            # Replace any bad geometries after the simplification procedure, with the original unsimplified geometry. Perhaps we could use a different (like a backup) simplification factor that is less, but seeing as its only a few geometries then we may as well use the original geometry. 
+            geometry_is_valid = np.logical_and(shapefile.is_valid, ~shapefile.is_empty)
+            gdf_geometry_is_valid = np.logical_and(gdf.is_valid, ~gdf.is_empty)
+            if geometry_is_valid.sum() != len(geometry_is_valid):
+                # Then there is at least one geometry that is invalid after simplification.
+                shapefile = pd.concat([shapefile[geometry_is_valid], gdf[~gdf_geometry_is_valid]]).sort_index()
+            # Add to the overall shapefile
+            final_shp = pd.concat([final_shp, shapefile], ignore_index=False).sort_index()
+
+    # Remove all the temporary files made
+    temp_dir.cleanup()
+    if not os.path.exists(os.path.dirname(save_path)):
+        os.makedirs(os.path.dirname(save_path))
+    # Convert the overall shapefile to a Topology object and save it
+    tp.Topology(final_shp, prequantize=False).to_json(save_path)
+
+
+def _boundingBoxToOffsets(vector_bbox, raster_geotransform):
+    col1 = int((vector_bbox[0] - raster_geotransform[0]) / raster_geotransform[1])
+    col2 = int((vector_bbox[1] - raster_geotransform[0]) / raster_geotransform[1]) + 1
+    row1 = int((vector_bbox[3] - raster_geotransform[3]) / raster_geotransform[5])
+    row2 = int((vector_bbox[2] - raster_geotransform[3]) / raster_geotransform[5]) + 1
+    return [row1, row2, col1, col2]
+
+
+def _geotFromOffsets(row_offset, col_offset, raster_geotransform):
+    return [raster_geotransform[0] + (col_offset * raster_geotransform[1]), raster_geotransform[1], 0.0, raster_geotransform[3] + (row_offset * raster_geotransform[5]), 0.0, raster_geotransform[5]]
+
+
+def _check_inputted_datasets(raster_path, vector_path):
+    """
+    Run compatibility checks to ensure:
+        - Files exist
+        - Vector file only contains Polygons
+        - Geographic projections match
+    """
+    try:
+        import rasterio as rio
+    except ModuleNotFoundError:
+        raise ModuleNotFoundError("RasterIO could not be located. Please install rasterio seperately into this Python environment, or run 'pip install uintel[full]'")
+
+    # Do some checks to make sure the vector file input is okay
+    if type(vector_path) == gpd.GeoDataFrame:
+        if not os.path.exists("shp-tmp"):
+            os.makedirs("shp-tmp")
+        vector_path.to_file("shp-tmp/vector_file.shp")
+        vector_path = os.path.join(os.getcwd(), "shp-tmp", "vector_file.shp")
+    elif type(vector_path) != str:
+        raise TypeError(f"The vector file must be either a string of the filepath to the shape OR a GeoDataFrame. A {type(vector_path)} is not acceptable.")
+
+    try:
+        vector_file = gpd.read_file(vector_path)
+    except Exception as e:
+        raise e
+
+    geom_types = vector_file.geom_type.unique()
+    if len(geom_types) != 1:
+        raise TypeError(f"The vector file: {vector_path} can only contain Polygon geometries, but it contains {geom_types}. Please correct this before running again.")
+    if geom_types[0] != 'Polygon':
+        raise TypeError(f"The vector file: {vector_path} can only contain Polygon geometries, but it contains {geom_types}. Please correct this before running again.")
+    vector_epsg = vector_file.crs.to_epsg()
+    del vector_file
+
+    # Do some checks to make sure the raster file input is okay
+    if type(raster_path) != str:
+        raise TypeError(f"The raster file must be a string of the filepath to the raster. A {type(vector_path)} is not acceptable.")
+    try:
+        raster_epsg = rio.open(raster_path).crs.to_epsg()
+        if rio.open(raster_path).crs.to_epsg() == None:
+            raster_epsg = 2193
+    except Exception as e:
+        raise e
+
+
+    # Check to see if the projections match
+    if vector_epsg != raster_epsg:
+        if type(raster_epsg) in (int, float):
+            warnings.warn(f"The two inputted datasets are in different projections (raster: {raster_epsg}; vector: {vector_epsg}). An attempt will be made to reproject the vector layer into the projection of the raster. This will change the vector file saved at {vector_path} to EPSG:{raster_epsg}.")
+            try:
+                _ = gpd.read_file(vector_path).to_crs(raster_epsg).to_file(vector_path)
+            except:
+                raise TypeError(f"The automatic attempt at changing projections failed. Please correct this before running again.")
+        else:
+            raise TypeError(f"The two inputted datasets are in different projections (raster: {raster_epsg}; vector: {vector_epsg}). Please correct this before running again.")
+
+    return raster_epsg
+
+
+def _get_raster_array(raster_dataset, offsets, raster_x_size, raster_y_size, raster_band, raster_nodata):
+    """
+    Checks to see if the vector offset geometry lies within the raster dataset, and if so, returns the values from the raster_dataset. If only a proportion of the geometries overlap, then the other pixel values are given the raster_nodata value.
+    """
+
+    # Grab the "normal" parameters to pass to ReadAsArray  
+    y_top, y_bottom, x_left, x_right = offsets         
+    width, height = x_right-x_left, y_bottom-y_top
+   
+    if width == 0 or height == 0:
+        # The  the requested raster has a zero dimension which is invalid
+        return None
+    if x_left > raster_x_size or y_top > raster_y_size:
+        # Then the starting point (top left of the polygon) is outside of the bottom right raster extent
+        return None
+    elif x_right < 0 or y_bottom < 0:
+        # Then the finishing point (bottom right of the polygon) is outside of the top left raster extent
+        return None
+    elif x_left >= 0 and x_right <= raster_x_size and y_top >= 0 and y_bottom <= raster_y_size and width >= 0 and height >= 0:
+        # Then the whole vector geometry is within the raster
+        return raster_dataset.GetRasterBand(raster_band).ReadAsArray(x_left, y_top, width, height)    
+    elif (x_left < 0 or y_top < 0) and x_right > 0 and y_bottom > 0:
+        # Then the starting point (top left of the polygon) is outside of the raster extent
+        # Only some of the vector geometry is within the raster extent so create a full no-data array and overwrite values that exist
+        raster = np.full((height, width), raster_nodata)
+        
+        x_offset, y_offset = 0, 0
+        # Adjust the height and widths to be in the bounds of the raster
+        if x_left < 0:
+            x_offset = -x_left # Move everything left to make x_left = 0
+            width -= x_offset  # sum negative number will reduce the width 
+            x_left = 0
+        if y_top < 0:
+            y_offset = -y_top # Move everything down to make y_top =0 
+            height -= y_offset  # sum negative number will reduce the width
+            y_top = 0
+        if x_right > raster_x_size:
+            width -= (x_right - raster_x_size) # subtract how much over the boundary
+            x_right = raster_x_size
+        if y_bottom > raster_y_size:
+            height -= (y_bottom - raster_y_size) # subtract how much over the boundary
+            y_bottom = raster_y_size
+        raster[y_offset:y_offset+height, x_offset:x_offset+width] = raster_dataset.GetRasterBand(raster_band).ReadAsArray(x_left, y_top, width, height)
+        return raster
+    elif x_left >= 0 and x_left < raster_x_size and y_top >= 0 and y_top < raster_y_size and (x_right > raster_x_size or y_bottom > raster_y_size):
+        # Only some of the vector geometry is within the raster extent so create a full no-data array and overwrite values that exist
+        raster = np.full((height, width), raster_nodata)
+        new_xsize, new_ysize = min(raster_x_size-x_left, width), min(raster_y_size-y_top, height)
+        raster[0:new_ysize, 0:new_xsize] = raster_dataset.GetRasterBand(raster_band).ReadAsArray(x_left, y_top, new_xsize, new_ysize)
+        return raster
+    else:
+        warnings.warn(f"Uncaught case in zonal statistics get_raster_array! Details below:\n bounds = {offsets} with raster extends of {raster_x_size} x {raster_y_size}.")
+
+
+def calculate_zonal_statistics(raster_path: str, vector_path: str, raster_band: int = 1, allow_touching_pixels: bool = True, show_progress: bool = True) -> dict:
+    """Calculate statistics of a raster over a vector geometry.
+
+    Collect stats (min, max, mean, median, std, sum, 10th percentile, 90th percentile and count) on pixel values (raster) which lie within polygons (vector). If allow_touching_pixels is set to True, then any pixel that touches the exterior of the vector geometry is included in the statistics calculation. The returned dictionary has the vector FID as the key, where the values is a dictionary mapping the statistic's name to value.
+    
+    Examples:
+        >>> zonal_statistics = calculate_zonal_statistics("raster.tiff", "vector.shp")
+        >>> zonal_statistics[67] # To get the statistics of the raster over the vector shape with an FID of 67
+        {"min": 0, "max": 10.6, "mean": 2.5, "median": 2.8, "std": 0.6, "sum": 180.8, "count": 72, "90th_percentile": 28,"10th_percentile": 0.2}      
+
+    Args:
+        raster_path: Filepath of where the raster is stored.
+        vector_path: Filepath of where the vector geometry (typically a shapefile) is stored.
+        raster_band: Band of the raster to analyse.
+        allow_touching_pixels: If True, any pixel that touches the exterior of the vector geometry is included in the statistics calculation. Otherwise, the statistics is using pixels within the vector geometry.
+        show_progress: If True, show the progress of calculating the statistics for each vector feature.
+    
+    Returns:
+        A dictionary of nested dictionaries, where the keys are the FID of the vector geometry and the dictionary contains the statistics of the raster over the FID geometry.
+    """
+    try:
+        import osgeo.ogr, osgeo.osr, osgeo.gdal
+    except ModuleNotFoundError:
+        raise ModuleNotFoundError("GDAL could not be located. Please install GDAL seperately into this Python environment, or run 'pip install uintel[full]'")
+    try:
+        import rasterio as rio
+    except ModuleNotFoundError:
+        raise ModuleNotFoundError("RasterIO could not be located. Please install rasterio seperately into this Python environment, or run 'pip install uintel[full]'")
+
+    
+    epsg = _check_inputted_datasets(raster_path, vector_path)
+
+    # Get GDAL driver
+    mem_driver = osgeo.ogr.GetDriverByName("Memory")
+    mem_driver_gdal = osgeo.gdal.GetDriverByName("MEM")
+
+    # Open datasets
+    vector_dataset = osgeo.ogr.Open(vector_path)
+    vector_layer = vector_dataset.GetLayer()
+    raster_dataset = osgeo.gdal.Open(raster_path)
+
+    # Get information about the raster dataset
+    raster_geotransform = raster_dataset.GetGeoTransform()
+    raster_nodata = raster_dataset.GetRasterBand(raster_band).GetNoDataValue()
+    raster_x_size = raster_dataset.RasterXSize
+    raster_y_size = raster_dataset.RasterYSize
+    dest_srs = osgeo.osr.SpatialReference()
+    _ = dest_srs.ImportFromEPSG(epsg)
+
+    # Set up a progress bar if the user wants one
+    if show_progress:
+        progress_bar = tqdm.tqdm(desc="Calculating zonal statistics", total=len(gpd.read_file(vector_path)), leave=False, dynamic_ncols=True)
+
+    # Iterate through each polygon in the shapefile (vector feature)
+    zonal_statistics = {}
+    vector_feature = vector_layer.GetNextFeature()
+    while vector_feature:
+        if vector_feature.GetGeometryRef() is not None:
+            # Create a new driver
+            if os.path.exists("temp"):
+                _ = mem_driver.DeleteDataSource("temp")
+            temporary_dataset = mem_driver.CreateDataSource("temp")
+            
+            # Create a new layer of just the one feature
+            temporary_layer = temporary_dataset.CreateLayer('polygons', dest_srs, osgeo.ogr.wkbPolygon)
+            _ = temporary_layer.CreateFeature(vector_feature.Clone())
+            
+            # Determine the offsets
+            offsets = _boundingBoxToOffsets(vector_feature.GetGeometryRef().GetEnvelope(), raster_geotransform)
+            
+            # Transform from the offsets
+            new_geotransform = _geotFromOffsets(offsets[0], offsets[2], raster_geotransform)
+            
+            # Create a blank transformed dataset
+            transformed_dataset = mem_driver_gdal.Create("", offsets[3] - offsets[2], offsets[1] - offsets[0], 1, osgeo.gdal.GDT_Byte)
+            _ = transformed_dataset.SetGeoTransform(new_geotransform)
+            
+            # Rasterise the transformed dataset to the temporary layer where the array is 1 = touches, 0 = does not touch
+            _= osgeo.gdal.RasterizeLayer(transformed_dataset, [1], temporary_layer, burn_values=[1], options=[f'ALL_TOUCHED={str(allow_touching_pixels).upper()}'])
+            transformed_array = transformed_dataset.ReadAsArray()
+            
+            # Grab the values of the raster that intersect the vector geometry
+            raster_array = _get_raster_array(raster_dataset, offsets, raster_x_size, raster_y_size, raster_band, raster_nodata)
+            
+            id = vector_feature.GetFID()
+            if raster_array is not None and len(raster_array) > 0:
+                # Mask the raster to only cover the vector geometry (transformed array)
+                raster_values_over_vector_feature = raster_array[~np.logical_or(raster_array==raster_nodata, np.logical_not(transformed_array))]
+                if raster_values_over_vector_feature is not None and len(raster_values_over_vector_feature) > 0:
+                    # Then there are some values over the vector feature!!
+                    zonal_statistics[id] = {
+                        "min": raster_values_over_vector_feature.min(),
+                        "max": raster_values_over_vector_feature.max(),
+                        "mean": raster_values_over_vector_feature.mean(),
+                        "median": np.median(raster_values_over_vector_feature),
+                        "std": raster_values_over_vector_feature.std(),
+                        "sum": raster_values_over_vector_feature.sum(),
+                        "count": len(raster_values_over_vector_feature),
+                        "90th_percentile": np.percentile(raster_values_over_vector_feature, 90),
+                        "10th_percentile": np.percentile(raster_values_over_vector_feature, 10)
+                        }      
+                else:
+                    # There are no raster cells overlapping the vector feature
+                    zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": None, "90th_percentile": None, "10th_percentile": None}     
+            else:
+                # There is no raster?
+                zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": None, "90th_percentile": None, "10th_percentile": None}
+            
+            # Clear some memory
+            temporary_dataset = None
+            temporary_layer = None
+            transformed_dataset = None
+            # Repeat with the next polygon geometry
+            vector_feature = vector_layer.GetNextFeature()
+        
+        if show_progress: 
+            _ = progress_bar.update(1)
+
+    return zonal_statistics
```

### Comparing `uintel-0.3.9/src/uintel/install.py` & `uintel-0.4.0/src/uintel/install.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,438 +1,438 @@
-"""
-Functions to install and configure UI onto this machine.
-"""
-
-import ctypes, glob, os, shutil, subprocess, sys, ctypes.wintypes, json, threading
-import matplotlib as mpl, matplotlib.font_manager as mpl_fonts, matplotlib.pyplot as plt
-
-if sys.platform == "win32":
-    try:
-        import winreg
-    except ImportError:
-        import _winreg as winreg
-
-_CONFIG_PATH = os.path.expanduser("~/.ui/config")
-
-class _printColours:
-   PURPLE = '\033[95m'
-   CYAN = '\033[96m'
-   DARKCYAN = '\033[36m'
-   BLUE = '\033[94m'
-   GREEN = '\033[92m'
-   YELLOW = '\033[93m'
-   RED = '\033[91m'
-   BOLD = '\033[1m'
-   UNDERLINE = '\033[4m'
-   END = '\033[0m'
-
-
-def _get_config() -> dict:
-    """
-    Return the configuration file
-    """
-    with threading.Lock():
-        with open(_CONFIG_PATH, "r") as fp:
-            config = json.load(fp)
-    return config
-
-
-def _save_config(config: dict) -> None:
-    """
-    Save the configuration file
-    """
-    os.makedirs(os.path.dirname(_CONFIG_PATH), exist_ok=True)
-    with threading.Lock():
-        with open(_CONFIG_PATH, "w") as fp:
-            json.dump(config, fp, indent=4)
-
-
-def _update_config_file(verbose=True) -> bool:
-    """
-    Update the existing configuartion file to the latest version. As new versions of uintel as released, the configuration file may change structure and hence need to be altered or completely re-built. This function aims to fill in gaps, or completely re-build it to get it to the latest version.
-    """
-
-    if not os.path.exists(_CONFIG_PATH):
-        if verbose:
-            print(f"{_printColours.RED}The configuration file is missing... Starting to rebuild{_printColours.END}")
-        _create_config_file()
-        return 
-    
-    config = _get_config()
-    
-    if type(config) != dict:
-        if verbose:
-            print(f"{_printColours.RED}The configuration file is corrupted... Starting to rebuild{_printColours.END}")
-        _create_config_file()
-
-    if "name" not in config:
-        config["name"] = input("Whoops, it seems I don't know who you are! What is your name? ")
-        print(f"Thanks, {config['name']}. It's a pleasure to have you here.")
-
-    if "servers" not in config:
-        config["servers"] = _get_server_details()
-    else:
-        if type(config["servers"]) != dict:
-            config["servers"] = _get_server_details()
-        else:
-            # Check to see if all servers have the right amount of information
-            for nickname, details in config["servers"].items():
-                if type(nickname) != str or type(details) != dict:
-                    config["servers"] = _get_server_details()
-                    break
-                else:
-                    if not details.get("address"):
-                        details["address"] = input(f"I seem to be missing the address for the {nickname} server. What is the address? (e.g. 173.42.60.98) ")
-                    if not details.get("username"):
-                        details["username"] = input(f"I seem to be missing the username for the {nickname} server. What is your username? ")
-                    if "ssh_key" not in details:
-                        details["ssh_key"] = input(f"I seem to be missing if you have a SSH key the {nickname} server. Do you use a SSH key to connect? (yes/no) ").lower == "yes"
-                    else:
-                        # Check it is a bool
-                        if type(details["ssh_key"]) != bool:
-                            details["ssh_key"] = input(f"I seem to be missing if you have a SSH key the {nickname} server. Do you use a SSH key to connect? (yes/no) ").lower == "yes"
-                    
-                    if details["ssh_key"]:
-                        details["password"] = None
-                    else:
-                        if not details.get("password"):
-                            details["password"] = input(f"Since you have indicated you do not use a SSH key for {nickname}, what is your password? ")
-
-    if "slack" not in config:
-        config["slack"] = _get_slack_details()
-    else:
-        if type(config["slack"]) != dict:
-            config["slack"] = _get_slack_details()
-        else:
-            for domain, token in config["slack"]:
-                if type(domain) != str or type(token) != str:
-                    config["slack"] = _get_slack_details()
-                    break
-    
-    if "sql" not in config:
-        config["sql"] = _get_sql_details()
-    else:
-        if type(config["sql"]) != dict:
-            config["sql"] = _get_sql_details()
-        else:
-            # Check to see if all servers have the right amount of information
-            for host, details in config["sql"].items():
-                if type(host) != str or type(details) != dict:
-                    config["servers"] = _get_server_details()
-                    break
-                else:
-                    if not details.get("port"):
-                        details["port"] = input(f"I seem to be missing the port for the {nickname} SQL database. What is the port? (e.g. 5002) ")
-                    if not details.get("username"):
-                        details["username"] = input(f"I seem to be missing the username for the {nickname} SQL database. What is the username? (e.g. postgres) ")
-                    if not details.get("password"):
-                        details["password"] = input(f"I seem to be missing the password for the {nickname} SQL database. What is the password? ")
-    
-    _save_config(config)
-
-
-def _create_config_file() -> None:
-    """
-    Create a configuration file that contains key information about the user and key Urban Intelligence information, that is commonly used throughout multiple programs.
-    """
-
-    print(f"{_printColours.UNDERLINE}{_printColours.BOLD}{_printColours.BLUE}Kia ora and welcome to Urban Intelligence.{_printColours.END}\n")
-    print(f"{_printColours.BLUE}To streamline this package and reduce asking these details continuously, we wish to ask you some questions about yourself to store in a credentials file.\nThis file will be located at {_CONFIG_PATH} should you ever wish to view it or alter information.{_printColours.END}\n")
-
-    config = {}
-    config["name"] = input("To begin, what is your name? ").title()
-    
-    print(f"{_printColours.BLUE}It's a pleasure to have you here, {config['name']}.\nIf at any stage you do not know the answer to any of the questions or if they are not applicable, then please leave the prompt empty and hit enter.{_printColours.END}")
-    
-    config["servers"] = _get_server_details()
-    config["slack"] = _get_slack_details()
-    config["sql"] = _get_sql_details()
-
-    _create_aws_credentials()
-
-    _save_config(config)    
-
-    print(f"\n{_printColours.BLUE}Awesome, thanks for answering those questions {config['name']}! I'll now continue with the rest of the installation :) {_printColours.END}")
-
-
-def _get_server_details() -> dict:
-    """
-    Return a dictionary of server details that the users wishes to add to the configuration file.
-    """
-
-    print(f"\n{_printColours.BLUE}These next set of questions deal with connecting to our servers.{_printColours.END}")
-    server_details = {}
-    all_servers_added = input(f"Would you like to save a server for easy file transferring to within Python code? (yes/no) ") == "no"
-    while not all_servers_added:
-        server_nickname = input("What is the name of the nickname of the server you wish to connect to? (e.g. piwakawaka; test; dev; products) ")
-        server_details[server_nickname] = {
-            "address": input(f"What is the address for {server_nickname}? (e.g. 173.42.60.98) "),
-            "username": input(f"What is your username for {server_nickname}? "),
-            "ssh_key": input(f"Do you use a SSH key to connect to {server_nickname}? (yes/no) ").lower() == "yes"
-            }
-        if not server_details[server_nickname]["ssh_key"]:
-            server_details[server_nickname]["password"] = input(f"Since you have indicated you do not use a SSH key for {server_nickname}, what is your password? ")
-        else:
-            server_details[server_nickname]["password"] = None
-        all_servers_added = input(f"Excellent, I have saved the details for {server_nickname}. Is there another server you wish to add? (yes/no) ") == "no"
-    
-    return server_details
-
-
-def _get_slack_details() -> dict:
-    """
-    Return a dictionary of Slack details that the users wishes to add to the configuration file.
-    """
-
-    print(f"\n{_printColours.BLUE}This next section will address the use of Slack.\n{_printColours.UNDERLINE}{_printColours.BOLD}This will require you to navigate to a pinned post in the #pyui slack channel containing the answers to the question, and paste them here. If you are not a member of that channel, then please contact Sam directly.{_printColours.END}")
-
-    slack_details = {}
-    all_slacks_added = input(f"Would you like to save a Slack domain for easy message posting and file uploading within Python code? (yes/no) ") == "no"
-    
-    while not all_slacks_added:
-        slack_domain = input("What is the Slack domain you wish to add? (e.g. UI; UC) ")
-        slack_details[slack_domain] = input(f"What is the token to access the {slack_domain} slack channel? ")
-        all_slacks_added = input(f"Excellent, I have saved the details for {slack_domain}. Is there another domain you wish to add? (yes/no) ") == "no"
-    
-    return slack_details
-
-
-def _get_sql_details() -> dict:
-    """
-    Return a dictionary of Slack details that the users wishes to add to the configuration file.
-    """
-
-    print(f"\n{_printColours.BLUE}This next section will address the use of SQL databases.{_printColours.END}")
-    sql_details = {}
-    all_sql_dbs_added = input(f"Would you like to save a SQL database for easy data management within Python code? (yes/no) ") == "no"
-    
-    while not all_sql_dbs_added:
-        host = input("What is the SQL host you wish to add? (e.g. encivmu-tml62) ")
-        sql_details[host] = {
-            "port": int(input("What port is the SQL database on? (e.g. 5002) ")),
-            "username": input("What is the username to connect to SQL? (e.g. postgres) "),
-            "password": input("What is the password to connect to SQL? ")
-        }
-        all_sql_dbs_added = input(f"Excellent, I have saved the details for {host}. Is there another SQL database you wish to add? (yes/no) ") == "no"
-    
-    return sql_details
-
-
-def _create_aws_credentials() -> None:
-    """
-    If it has not been done and the user has an account, create a file at ~/.aws/credentials containing the users credentials so that they can quickly connect to AWS services.
-    """
-    
-    if not os.path.exists(os.path.expanduser("~/.aws/credentials")):
-        print(f"{_printColours.BLUE}This next section will address the use of Amazon Web Services (AWS).{_printColours.END}")
-        if "yes" in input(f"{_printColours.BLUE}To send files to AWS for the UI dashboards, you will require an AWS account. I noticed you have not saved your credentials to this computer.\nDo you have an AWS account you wish to connect? (yes/no){_printColours.END} ").lower():
-            print(f"{_printColours.BLUE}Excellent. There are two key bits of information I require to do this - an access key id and a secret access key.\n\n{_printColours.BOLD}Instructions: To create a new secret access key for an IAM user, open the IAM console in AWS. Click Users in the Details pane, click the appropriate IAM user, and then click Create Access Key on the Security Credentials tab. The two bits of information should now be showing.{_printColours.END}")
-            aws_credentials = f"[default]\naws_access_key_id = {input('What is the access key? ')}\naws_secret_access_key = {input('What is the secret access key? ')}"
-            if not os.path.exists(os.path.expanduser("~/.aws")):
-                os.makedirs(os.path.expanduser("~/.aws"))
-            with open(os.path.expanduser("~/.aws/credentials"), "w") as file:
-                _ = file.write(aws_credentials)
-
-
-def _install_styles(force: bool, verbose: bool) -> None:
-    """
-    Copy all unregistered UI style sheets (saved in 'styles' folder) to the matplotlib configuration folder. To revert stylesheets back to default (in case they were manually edited), use force=True.
-    """
-    try:
-        style_dir = os.path.dirname(__file__) + '/styles'
-        mpl_style_dir = os.path.join(mpl.get_configdir(), "stylelib")
-        os.makedirs(mpl_style_dir, exist_ok=True)
-        stylesheets = glob.glob(style_dir + "/*.mplstyle")     
-        if len(stylesheets) == 0:
-            print(f"{_printColours.YELLOW}No matplotlib stylesheets detected in this version. If you were expecting some to install, please contact the maintainer of this package, Sam.{_printColours.END}")
-            return
-        else:
-            altered_files = 0
-            for stylefile in stylesheets:
-                if os.path.basename(stylefile).split(".")[0] not in plt.style.library or force:
-                    # Move each style sheet to the right place, which replaces any manual changes to UI stylelibs
-                    _ = shutil.copy(stylefile, os.path.join(mpl_style_dir, os.path.basename(stylefile)))
-                    altered_files += 1
-
-        # Update the current instance of matplotlib with the stylesheets
-        stylesheets = plt.style.core.read_style_directory(style_dir)
-        _ = plt.style.core.update_nested_dict(plt.style.library, stylesheets)
-        plt.style.core.available[:] = sorted(plt.style.library.keys())
-        
-        if altered_files > 0 and verbose:
-            print(f"{_printColours.GREEN}Successfully updated {altered_files} matplotlib stylesheets!{_printColours.END}")
-        elif verbose:
-            print(f"{_printColours.GREEN}All matplotlib stylesheets were already up to date!{_printColours.END}")
-    except Exception as error:
-        print(f"{_printColours.RED}The Urban Intelligence matplotlib stylesheets have not been successfully installed. Please contact the maintainer of this package, Sam, with the following error message:\n{error}{_printColours.END}")
-
-
-def _install_fonts(force: bool, verbose=True) -> None:
-    """
-    Copy and install all unregistered fonts (saved in 'fonts' folder) to this machine. To revert fonts back to default (in case they were manually edited), use force=True.
-    """
-
-    fonts = {os.path.basename(filepath): filepath for filepath in glob.glob(os.path.dirname(__file__) + "/fonts/*.ttf")}
-    if len(fonts) == 0:
-        print(f"{_printColours.YELLOW}No fonts detected in this version. If you were expecting some to install, please contact the maintainer of this package, Sam.{_printColours.END}")
-        return
-    
-    if force:
-        # Delete all installed fonts so they can be reinstalled
-        _delete_installed_fonts(fonts)
-    else:   
-        # Otherwise, we should skip fonts that are already installed 
-        fonts = _get_uninstalled_fonts(fonts)
-
-    if len(fonts) > 0:
-        if sys.platform == "win32":
-            _install_windows_fonts(fonts, verbose)
-            _refresh_matplotlib_fonts()
-        elif sys.platform == "linux":
-            _install_linux_fonts(fonts, verbose)
-            _refresh_matplotlib_fonts()
-        else:
-            print(f"{_printColours.RED}Unfortunately, the automatic downloading and installing Urban Intelligence's fonts has only been set up to be used for Windows or Linux distributions (because Sam doesn't have a Mac to test this code on). If the Rubik font is not installed on your device, please do so manually. Apolgies for the inconvience.{_printColours.END}")
-    else:
-        print(f"{_printColours.GREEN}All fonts were already up to date!{_printColours.END}")
-
-
-def _get_uninstalled_fonts(fonts: dict) -> None:
-    """
-    Takes a dictionary of font_name:font_path (e.g. 'Rubik.ttf':'/fonts/rubik.ttf') and returns only the keys of fonts that are not installed on this machine.
-    """
-    uninstalled_fonts = {}
-
-    if sys.platform == "win32":
-        for font_name, font_path in fonts.items():
-            font_in_regedit = False
-            with winreg.OpenKey(winreg.HKEY_CURRENT_USER, r'Software\Microsoft\Windows NT\CurrentVersion\Fonts', 0, winreg.KEY_READ) as key:
-                # Loop over each Value (font names) in the Key (registry path to the fonts) and see if it our wanted fonts are contained
-                for i in range(winreg.QueryInfoKey(key)[1]):
-                    font_name_installed, _, _ = winreg.EnumValue(key, i)
-                    if font_name.split(".")[0] == font_name_installed:
-                        font_in_regedit = True
-                        break
-           
-            if not font_in_regedit:
-                # The font is not properly installed for at least one reason.
-                uninstalled_fonts[font_name] = font_path
-
-    elif sys.platform == "linux":
-        
-        font_path = os.path.expanduser("~/.local/share/fonts/")
-        if os.path.exists(font_path):
-            installed_fonts = os.listdir(font_path)
-            for font_name, font_path in fonts.items():
-                if font_name not in installed_fonts:
-                    uninstalled_fonts[font_name] = font_path
-        else:
-            uninstalled_fonts = fonts.copy()
-
-    else:
-        print(f"{_printColours.RED}Unfortunately, the automatic downloading and installing Urban Intelligence's fonts has only been set up to be used for Windows or Linux distributions (because Sam doesn't have a Mac to test this code on). If the Rubik font is not installed on your device, please do so manually. Apolgies for the inconvience.{_printColours.END}")
-
-    return uninstalled_fonts
-
-
-def _delete_installed_fonts(fonts: dict) -> None:
-    """
-    Delete all installed fonts
-    """
-    
-    if sys.platform == "win32":
-        # Delete registry keys
-        with winreg.OpenKey(winreg.HKEY_CURRENT_USER, r'Software\Microsoft\Windows NT\CurrentVersion\Fonts', 0, winreg.KEY_ALL_ACCESS) as key:
-            for font_name in fonts:
-                try:
-                    _ = winreg.DeleteValue(key, font_name.split(".")[0])
-                except:
-                    pass
-        
-        # Delete the actual files
-        font_save_path = os.path.expandvars('%LOCALAPPDATA%/Microsoft/Windows/Fonts')
-        for font_name in fonts:
-            if os.path.exists(os.path.join(font_save_path, font_name)):
-                _ = os.remove(os.path.join(font_save_path, font_name))
-
-    
-    elif sys.platform == "linux":
-        # Delete the actual files
-        font_save_path = os.path.expanduser("~/.local/share/fonts/")
-        for font_name in fonts:
-            if os.path.exists(os.path.join(font_save_path, font_name)):
-                _ = os.remove(os.path.join(font_save_path, font_name))
-
-    else:
-        print(f"{_printColours.RED}Unfortunately, the automatic downloading and installing Urban Intelligence's fonts has only been set up to be used for Windows or Linux distributions (because Sam doesn't have a Mac to test this code on). If the Rubik font is not installed on your device, please do so manually. Apolgies for the inconvience.{_printColours.END}")
-
-    return
-
-
-def _install_windows_fonts(fonts: dict, verbose=True) -> None:
-    """
-    Install the fonts into the computers fonts folder (or users local fonts folder if permissions are denied) and register them on RegistryEditor.
-    Based on code by https://stackoverflow.com/a/68714427    
-    """
-
-    user32 = ctypes.WinDLL('user32', use_last_error=True)
-    gdi32 = ctypes.WinDLL('gdi32', use_last_error=True)
-
-    if not hasattr(ctypes.wintypes, 'LPDWORD'):
-        ctypes.wintypes.LPDWORD = ctypes.POINTER(ctypes.wintypes.DWORD)
-
-    user32.SendMessageTimeoutW.restype = ctypes.wintypes.LPVOID
-    user32.SendMessageTimeoutW.argtypes = (ctypes.wintypes.HWND, ctypes.wintypes.UINT, ctypes.wintypes.LPVOID, ctypes.wintypes.LPVOID, ctypes.wintypes.UINT, ctypes.wintypes.UINT, ctypes.wintypes.LPVOID)
-    gdi32.AddFontResourceW.argtypes = (ctypes.wintypes.LPCWSTR,)
-    gdi32.GetFontResourceInfoW.argtypes = (ctypes.wintypes.LPCWSTR, ctypes.wintypes.LPDWORD, ctypes.wintypes.LPVOID, ctypes.wintypes.DWORD)
-    
-    for font_name, font_path in fonts.items():
-        try:
-            # Copy the font to the user's Font folder
-            dest_folder = os.path.expandvars('%LOCALAPPDATA%/Microsoft/Windows/Fonts')
-            os.makedirs(dest_folder, exist_ok=True)
-            dst_path = os.path.join(dest_folder, font_name)
-            _ = shutil.copy(font_path, dst_path)
-                            
-            # Notify running programs that there is a new font
-            _ = user32.SendMessageTimeoutW(0xFFFF, 0x001D, 0, 0, 0x0002, 1000, None)
-            
-            # Store the fontname/filename in the registry so it can be found 
-            with winreg.OpenKey(winreg.HKEY_CURRENT_USER, r'Software\Microsoft\Windows NT\CurrentVersion\Fonts', 0, winreg.KEY_SET_VALUE) as key:
-                _ = winreg.SetValueEx(key, font_name.split(".")[0], 0, winreg.REG_SZ, dst_path)
-
-            if verbose:
-                print(f"{_printColours.GREEN}Successfully installed {font_name}!{_printColours.END}")
-        except Exception as error:
-            print(f"{_printColours.RED}The font {font_name} could not be installed. Please download and install the font manually, or contact the maintainer of this package, Sam, about the following error message:\n{error}{_printColours.END}")
-    
-
-def _install_linux_fonts(fonts: dict, verbose=True) -> None:
-    """
-    Install the fonts into the computers fonts folder (or users local fonts folder if permissions are denied) and then refresh the font cache.
-    """
-
-    for font_name, font_path in fonts.items():
-        try:
-            # Copy the font to the user's Font folder
-            dest_folder = os.path.expanduser("~/.local/share/fonts/")
-            os.makedirs(dest_folder, exist_ok=True)
-            dest_path = os.path.join(dest_folder, font_name)
-            _ = shutil.copy(font_path, dest_path)
-                            
-        except Exception as error:
-            print(f"{_printColours.RED}The font '{font_name}' could not be installed. Please log the following error message as an issue on the GiHub repository https://github.com/uintel/pyui/issues\n{error}{_printColours.END}")
-    
-    # Rebuild the font cache with fc-cache -f -v
-    process = subprocess.run(["fc-cache", "-f"])    
-    if process.returncode == 0 and verbose:
-        print(f"{_printColours.GREEN}Successfuly installed {len(fonts)} fonts!{_printColours.END}")
-    elif process.returncode != 0:
-        print(f"{_printColours.RED}One or more of the fonts '{list(fonts.keys())}' could not be installed. Please download and install the font manually, or contact the maintainer of this package, Sam, about the following error message:\nError {process.returncode}: {process.stderr.decode()}{_printColours.END}")
-    
-
-def _refresh_matplotlib_fonts():
-    """
-    Refresh the cache of available fonts to use in matplotlib
-    """
-    mpl_fonts.json_dump(mpl_fonts.FontManager(), os.path.join(mpl.get_cachedir(), f"fontlist-v{mpl_fonts.FontManager.__version__}.json"))
-
+"""
+Functions to install and configure UI onto this machine.
+"""
+
+import ctypes, glob, os, shutil, subprocess, sys, ctypes.wintypes, json, threading
+import matplotlib as mpl, matplotlib.font_manager as mpl_fonts, matplotlib.pyplot as plt
+
+if sys.platform == "win32":
+    try:
+        import winreg
+    except ImportError:
+        import _winreg as winreg
+
+_CONFIG_PATH = os.path.expanduser("~/.ui/config")
+
+class _printColours:
+   PURPLE = '\033[95m'
+   CYAN = '\033[96m'
+   DARKCYAN = '\033[36m'
+   BLUE = '\033[94m'
+   GREEN = '\033[92m'
+   YELLOW = '\033[93m'
+   RED = '\033[91m'
+   BOLD = '\033[1m'
+   UNDERLINE = '\033[4m'
+   END = '\033[0m'
+
+
+def _get_config() -> dict:
+    """
+    Return the configuration file
+    """
+    with threading.Lock():
+        with open(_CONFIG_PATH, "r") as fp:
+            config = json.load(fp)
+    return config
+
+
+def _save_config(config: dict) -> None:
+    """
+    Save the configuration file
+    """
+    os.makedirs(os.path.dirname(_CONFIG_PATH), exist_ok=True)
+    with threading.Lock():
+        with open(_CONFIG_PATH, "w") as fp:
+            json.dump(config, fp, indent=4)
+
+
+def _update_config_file(verbose=True) -> bool:
+    """
+    Update the existing configuartion file to the latest version. As new versions of uintel as released, the configuration file may change structure and hence need to be altered or completely re-built. This function aims to fill in gaps, or completely re-build it to get it to the latest version.
+    """
+
+    if not os.path.exists(_CONFIG_PATH):
+        if verbose:
+            print(f"{_printColours.RED}The configuration file is missing... Starting to rebuild{_printColours.END}")
+        _create_config_file()
+        return 
+    
+    config = _get_config()
+    
+    if type(config) != dict:
+        if verbose:
+            print(f"{_printColours.RED}The configuration file is corrupted... Starting to rebuild{_printColours.END}")
+        _create_config_file()
+
+    if "name" not in config:
+        config["name"] = input("Whoops, it seems I don't know who you are! What is your name? ")
+        print(f"Thanks, {config['name']}. It's a pleasure to have you here.")
+
+    if "servers" not in config:
+        config["servers"] = _get_server_details()
+    else:
+        if type(config["servers"]) != dict:
+            config["servers"] = _get_server_details()
+        else:
+            # Check to see if all servers have the right amount of information
+            for nickname, details in config["servers"].items():
+                if type(nickname) != str or type(details) != dict:
+                    config["servers"] = _get_server_details()
+                    break
+                else:
+                    if not details.get("address"):
+                        details["address"] = input(f"I seem to be missing the address for the {nickname} server. What is the address? (e.g. 173.42.60.98) ")
+                    if not details.get("username"):
+                        details["username"] = input(f"I seem to be missing the username for the {nickname} server. What is your username? ")
+                    if "ssh_key" not in details:
+                        details["ssh_key"] = input(f"I seem to be missing if you have a SSH key the {nickname} server. Do you use a SSH key to connect? (yes/no) ").lower == "yes"
+                    else:
+                        # Check it is a bool
+                        if type(details["ssh_key"]) != bool:
+                            details["ssh_key"] = input(f"I seem to be missing if you have a SSH key the {nickname} server. Do you use a SSH key to connect? (yes/no) ").lower == "yes"
+                    
+                    if details["ssh_key"]:
+                        details["password"] = None
+                    else:
+                        if not details.get("password"):
+                            details["password"] = input(f"Since you have indicated you do not use a SSH key for {nickname}, what is your password? ")
+
+    if "slack" not in config:
+        config["slack"] = _get_slack_details()
+    else:
+        if type(config["slack"]) != dict:
+            config["slack"] = _get_slack_details()
+        else:
+            for domain, token in config["slack"]:
+                if type(domain) != str or type(token) != str:
+                    config["slack"] = _get_slack_details()
+                    break
+    
+    if "sql" not in config:
+        config["sql"] = _get_sql_details()
+    else:
+        if type(config["sql"]) != dict:
+            config["sql"] = _get_sql_details()
+        else:
+            # Check to see if all servers have the right amount of information
+            for host, details in config["sql"].items():
+                if type(host) != str or type(details) != dict:
+                    config["servers"] = _get_server_details()
+                    break
+                else:
+                    if not details.get("port"):
+                        details["port"] = input(f"I seem to be missing the port for the {nickname} SQL database. What is the port? (e.g. 5002) ")
+                    if not details.get("username"):
+                        details["username"] = input(f"I seem to be missing the username for the {nickname} SQL database. What is the username? (e.g. postgres) ")
+                    if not details.get("password"):
+                        details["password"] = input(f"I seem to be missing the password for the {nickname} SQL database. What is the password? ")
+    
+    _save_config(config)
+
+
+def _create_config_file() -> None:
+    """
+    Create a configuration file that contains key information about the user and key Urban Intelligence information, that is commonly used throughout multiple programs.
+    """
+
+    print(f"{_printColours.UNDERLINE}{_printColours.BOLD}{_printColours.BLUE}Kia ora and welcome to Urban Intelligence.{_printColours.END}\n")
+    print(f"{_printColours.BLUE}To streamline this package and reduce asking these details continuously, we wish to ask you some questions about yourself to store in a credentials file.\nThis file will be located at {_CONFIG_PATH} should you ever wish to view it or alter information.{_printColours.END}\n")
+
+    config = {}
+    config["name"] = input("To begin, what is your name? ").title()
+    
+    print(f"{_printColours.BLUE}It's a pleasure to have you here, {config['name']}.\nIf at any stage you do not know the answer to any of the questions or if they are not applicable, then please leave the prompt empty and hit enter.{_printColours.END}")
+    
+    config["servers"] = _get_server_details()
+    config["slack"] = _get_slack_details()
+    config["sql"] = _get_sql_details()
+
+    _create_aws_credentials()
+
+    _save_config(config)    
+
+    print(f"\n{_printColours.BLUE}Awesome, thanks for answering those questions {config['name']}! I'll now continue with the rest of the installation :) {_printColours.END}")
+
+
+def _get_server_details() -> dict:
+    """
+    Return a dictionary of server details that the users wishes to add to the configuration file.
+    """
+
+    print(f"\n{_printColours.BLUE}These next set of questions deal with connecting to our servers.{_printColours.END}")
+    server_details = {}
+    all_servers_added = input(f"Would you like to save a server for easy file transferring to within Python code? (yes/no) ") == "no"
+    while not all_servers_added:
+        server_nickname = input("What is the name of the nickname of the server you wish to connect to? (e.g. piwakawaka; test; dev; products) ")
+        server_details[server_nickname] = {
+            "address": input(f"What is the address for {server_nickname}? (e.g. 173.42.60.98) "),
+            "username": input(f"What is your username for {server_nickname}? "),
+            "ssh_key": input(f"Do you use a SSH key to connect to {server_nickname}? (yes/no) ").lower() == "yes"
+            }
+        if not server_details[server_nickname]["ssh_key"]:
+            server_details[server_nickname]["password"] = input(f"Since you have indicated you do not use a SSH key for {server_nickname}, what is your password? ")
+        else:
+            server_details[server_nickname]["password"] = None
+        all_servers_added = input(f"Excellent, I have saved the details for {server_nickname}. Is there another server you wish to add? (yes/no) ") == "no"
+    
+    return server_details
+
+
+def _get_slack_details() -> dict:
+    """
+    Return a dictionary of Slack details that the users wishes to add to the configuration file.
+    """
+
+    print(f"\n{_printColours.BLUE}This next section will address the use of Slack.\n{_printColours.UNDERLINE}{_printColours.BOLD}This will require you to navigate to a pinned post in the #pyui slack channel containing the answers to the question, and paste them here. If you are not a member of that channel, then please contact Sam directly.{_printColours.END}")
+
+    slack_details = {}
+    all_slacks_added = input(f"Would you like to save a Slack domain for easy message posting and file uploading within Python code? (yes/no) ") == "no"
+    
+    while not all_slacks_added:
+        slack_domain = input("What is the Slack domain you wish to add? (e.g. UI; UC) ")
+        slack_details[slack_domain] = input(f"What is the token to access the {slack_domain} slack channel? ")
+        all_slacks_added = input(f"Excellent, I have saved the details for {slack_domain}. Is there another domain you wish to add? (yes/no) ") == "no"
+    
+    return slack_details
+
+
+def _get_sql_details() -> dict:
+    """
+    Return a dictionary of Slack details that the users wishes to add to the configuration file.
+    """
+
+    print(f"\n{_printColours.BLUE}This next section will address the use of SQL databases.{_printColours.END}")
+    sql_details = {}
+    all_sql_dbs_added = input(f"Would you like to save a SQL database for easy data management within Python code? (yes/no) ") == "no"
+    
+    while not all_sql_dbs_added:
+        host = input("What is the SQL host you wish to add? (e.g. encivmu-tml62) ")
+        sql_details[host] = {
+            "port": int(input("What port is the SQL database on? (e.g. 5002) ")),
+            "username": input("What is the username to connect to SQL? (e.g. postgres) "),
+            "password": input("What is the password to connect to SQL? ")
+        }
+        all_sql_dbs_added = input(f"Excellent, I have saved the details for {host}. Is there another SQL database you wish to add? (yes/no) ") == "no"
+    
+    return sql_details
+
+
+def _create_aws_credentials() -> None:
+    """
+    If it has not been done and the user has an account, create a file at ~/.aws/credentials containing the users credentials so that they can quickly connect to AWS services.
+    """
+    
+    if not os.path.exists(os.path.expanduser("~/.aws/credentials")):
+        print(f"{_printColours.BLUE}This next section will address the use of Amazon Web Services (AWS).{_printColours.END}")
+        if "yes" in input(f"{_printColours.BLUE}To send files to AWS for the UI dashboards, you will require an AWS account. I noticed you have not saved your credentials to this computer.\nDo you have an AWS account you wish to connect? (yes/no){_printColours.END} ").lower():
+            print(f"{_printColours.BLUE}Excellent. There are two key bits of information I require to do this - an access key id and a secret access key.\n\n{_printColours.BOLD}Instructions: To create a new secret access key for an IAM user, open the IAM console in AWS. Click Users in the Details pane, click the appropriate IAM user, and then click Create Access Key on the Security Credentials tab. The two bits of information should now be showing.{_printColours.END}")
+            aws_credentials = f"[default]\naws_access_key_id = {input('What is the access key? ')}\naws_secret_access_key = {input('What is the secret access key? ')}"
+            if not os.path.exists(os.path.expanduser("~/.aws")):
+                os.makedirs(os.path.expanduser("~/.aws"))
+            with open(os.path.expanduser("~/.aws/credentials"), "w") as file:
+                _ = file.write(aws_credentials)
+
+
+def _install_styles(force: bool, verbose: bool) -> None:
+    """
+    Copy all unregistered UI style sheets (saved in 'styles' folder) to the matplotlib configuration folder. To revert stylesheets back to default (in case they were manually edited), use force=True.
+    """
+    try:
+        style_dir = os.path.dirname(__file__) + '/styles'
+        mpl_style_dir = os.path.join(mpl.get_configdir(), "stylelib")
+        os.makedirs(mpl_style_dir, exist_ok=True)
+        stylesheets = glob.glob(style_dir + "/*.mplstyle")     
+        if len(stylesheets) == 0:
+            print(f"{_printColours.YELLOW}No matplotlib stylesheets detected in this version. If you were expecting some to install, please contact the maintainer of this package, Sam.{_printColours.END}")
+            return
+        else:
+            altered_files = 0
+            for stylefile in stylesheets:
+                if os.path.basename(stylefile).split(".")[0] not in plt.style.library or force:
+                    # Move each style sheet to the right place, which replaces any manual changes to UI stylelibs
+                    _ = shutil.copy(stylefile, os.path.join(mpl_style_dir, os.path.basename(stylefile)))
+                    altered_files += 1
+
+        # Update the current instance of matplotlib with the stylesheets
+        stylesheets = plt.style.core.read_style_directory(style_dir)
+        _ = plt.style.core.update_nested_dict(plt.style.library, stylesheets)
+        plt.style.core.available[:] = sorted(plt.style.library.keys())
+        
+        if altered_files > 0 and verbose:
+            print(f"{_printColours.GREEN}Successfully updated {altered_files} matplotlib stylesheets!{_printColours.END}")
+        elif verbose:
+            print(f"{_printColours.GREEN}All matplotlib stylesheets were already up to date!{_printColours.END}")
+    except Exception as error:
+        print(f"{_printColours.RED}The Urban Intelligence matplotlib stylesheets have not been successfully installed. Please contact the maintainer of this package, Sam, with the following error message:\n{error}{_printColours.END}")
+
+
+def _install_fonts(force: bool, verbose=True) -> None:
+    """
+    Copy and install all unregistered fonts (saved in 'fonts' folder) to this machine. To revert fonts back to default (in case they were manually edited), use force=True.
+    """
+
+    fonts = {os.path.basename(filepath): filepath for filepath in glob.glob(os.path.dirname(__file__) + "/fonts/*.ttf")}
+    if len(fonts) == 0:
+        print(f"{_printColours.YELLOW}No fonts detected in this version. If you were expecting some to install, please contact the maintainer of this package, Sam.{_printColours.END}")
+        return
+    
+    if force:
+        # Delete all installed fonts so they can be reinstalled
+        _delete_installed_fonts(fonts)
+    else:   
+        # Otherwise, we should skip fonts that are already installed 
+        fonts = _get_uninstalled_fonts(fonts)
+
+    if len(fonts) > 0:
+        if sys.platform == "win32":
+            _install_windows_fonts(fonts, verbose)
+            _refresh_matplotlib_fonts()
+        elif sys.platform == "linux":
+            _install_linux_fonts(fonts, verbose)
+            _refresh_matplotlib_fonts()
+        else:
+            print(f"{_printColours.RED}Unfortunately, the automatic downloading and installing Urban Intelligence's fonts has only been set up to be used for Windows or Linux distributions (because Sam doesn't have a Mac to test this code on). If the Rubik font is not installed on your device, please do so manually. Apolgies for the inconvience.{_printColours.END}")
+    else:
+        print(f"{_printColours.GREEN}All fonts were already up to date!{_printColours.END}")
+
+
+def _get_uninstalled_fonts(fonts: dict) -> None:
+    """
+    Takes a dictionary of font_name:font_path (e.g. 'Rubik.ttf':'/fonts/rubik.ttf') and returns only the keys of fonts that are not installed on this machine.
+    """
+    uninstalled_fonts = {}
+
+    if sys.platform == "win32":
+        for font_name, font_path in fonts.items():
+            font_in_regedit = False
+            with winreg.OpenKey(winreg.HKEY_CURRENT_USER, r'Software\Microsoft\Windows NT\CurrentVersion\Fonts', 0, winreg.KEY_READ) as key:
+                # Loop over each Value (font names) in the Key (registry path to the fonts) and see if it our wanted fonts are contained
+                for i in range(winreg.QueryInfoKey(key)[1]):
+                    font_name_installed, _, _ = winreg.EnumValue(key, i)
+                    if font_name.split(".")[0] == font_name_installed:
+                        font_in_regedit = True
+                        break
+           
+            if not font_in_regedit:
+                # The font is not properly installed for at least one reason.
+                uninstalled_fonts[font_name] = font_path
+
+    elif sys.platform == "linux":
+        
+        font_path = os.path.expanduser("~/.local/share/fonts/")
+        if os.path.exists(font_path):
+            installed_fonts = os.listdir(font_path)
+            for font_name, font_path in fonts.items():
+                if font_name not in installed_fonts:
+                    uninstalled_fonts[font_name] = font_path
+        else:
+            uninstalled_fonts = fonts.copy()
+
+    else:
+        print(f"{_printColours.RED}Unfortunately, the automatic downloading and installing Urban Intelligence's fonts has only been set up to be used for Windows or Linux distributions (because Sam doesn't have a Mac to test this code on). If the Rubik font is not installed on your device, please do so manually. Apolgies for the inconvience.{_printColours.END}")
+
+    return uninstalled_fonts
+
+
+def _delete_installed_fonts(fonts: dict) -> None:
+    """
+    Delete all installed fonts
+    """
+    
+    if sys.platform == "win32":
+        # Delete registry keys
+        with winreg.OpenKey(winreg.HKEY_CURRENT_USER, r'Software\Microsoft\Windows NT\CurrentVersion\Fonts', 0, winreg.KEY_ALL_ACCESS) as key:
+            for font_name in fonts:
+                try:
+                    _ = winreg.DeleteValue(key, font_name.split(".")[0])
+                except:
+                    pass
+        
+        # Delete the actual files
+        font_save_path = os.path.expandvars('%LOCALAPPDATA%/Microsoft/Windows/Fonts')
+        for font_name in fonts:
+            if os.path.exists(os.path.join(font_save_path, font_name)):
+                _ = os.remove(os.path.join(font_save_path, font_name))
+
+    
+    elif sys.platform == "linux":
+        # Delete the actual files
+        font_save_path = os.path.expanduser("~/.local/share/fonts/")
+        for font_name in fonts:
+            if os.path.exists(os.path.join(font_save_path, font_name)):
+                _ = os.remove(os.path.join(font_save_path, font_name))
+
+    else:
+        print(f"{_printColours.RED}Unfortunately, the automatic downloading and installing Urban Intelligence's fonts has only been set up to be used for Windows or Linux distributions (because Sam doesn't have a Mac to test this code on). If the Rubik font is not installed on your device, please do so manually. Apolgies for the inconvience.{_printColours.END}")
+
+    return
+
+
+def _install_windows_fonts(fonts: dict, verbose=True) -> None:
+    """
+    Install the fonts into the computers fonts folder (or users local fonts folder if permissions are denied) and register them on RegistryEditor.
+    Based on code by https://stackoverflow.com/a/68714427    
+    """
+
+    user32 = ctypes.WinDLL('user32', use_last_error=True)
+    gdi32 = ctypes.WinDLL('gdi32', use_last_error=True)
+
+    if not hasattr(ctypes.wintypes, 'LPDWORD'):
+        ctypes.wintypes.LPDWORD = ctypes.POINTER(ctypes.wintypes.DWORD)
+
+    user32.SendMessageTimeoutW.restype = ctypes.wintypes.LPVOID
+    user32.SendMessageTimeoutW.argtypes = (ctypes.wintypes.HWND, ctypes.wintypes.UINT, ctypes.wintypes.LPVOID, ctypes.wintypes.LPVOID, ctypes.wintypes.UINT, ctypes.wintypes.UINT, ctypes.wintypes.LPVOID)
+    gdi32.AddFontResourceW.argtypes = (ctypes.wintypes.LPCWSTR,)
+    gdi32.GetFontResourceInfoW.argtypes = (ctypes.wintypes.LPCWSTR, ctypes.wintypes.LPDWORD, ctypes.wintypes.LPVOID, ctypes.wintypes.DWORD)
+    
+    for font_name, font_path in fonts.items():
+        try:
+            # Copy the font to the user's Font folder
+            dest_folder = os.path.expandvars('%LOCALAPPDATA%/Microsoft/Windows/Fonts')
+            os.makedirs(dest_folder, exist_ok=True)
+            dst_path = os.path.join(dest_folder, font_name)
+            _ = shutil.copy(font_path, dst_path)
+                            
+            # Notify running programs that there is a new font
+            _ = user32.SendMessageTimeoutW(0xFFFF, 0x001D, 0, 0, 0x0002, 1000, None)
+            
+            # Store the fontname/filename in the registry so it can be found 
+            with winreg.OpenKey(winreg.HKEY_CURRENT_USER, r'Software\Microsoft\Windows NT\CurrentVersion\Fonts', 0, winreg.KEY_SET_VALUE) as key:
+                _ = winreg.SetValueEx(key, font_name.split(".")[0], 0, winreg.REG_SZ, dst_path)
+
+            if verbose:
+                print(f"{_printColours.GREEN}Successfully installed {font_name}!{_printColours.END}")
+        except Exception as error:
+            print(f"{_printColours.RED}The font {font_name} could not be installed. Please download and install the font manually, or contact the maintainer of this package, Sam, about the following error message:\n{error}{_printColours.END}")
+    
+
+def _install_linux_fonts(fonts: dict, verbose=True) -> None:
+    """
+    Install the fonts into the computers fonts folder (or users local fonts folder if permissions are denied) and then refresh the font cache.
+    """
+
+    for font_name, font_path in fonts.items():
+        try:
+            # Copy the font to the user's Font folder
+            dest_folder = os.path.expanduser("~/.local/share/fonts/")
+            os.makedirs(dest_folder, exist_ok=True)
+            dest_path = os.path.join(dest_folder, font_name)
+            _ = shutil.copy(font_path, dest_path)
+                            
+        except Exception as error:
+            print(f"{_printColours.RED}The font '{font_name}' could not be installed. Please log the following error message as an issue on the GiHub repository https://github.com/uintel/pyui/issues\n{error}{_printColours.END}")
+    
+    # Rebuild the font cache with fc-cache -f -v
+    process = subprocess.run(["fc-cache", "-f"])    
+    if process.returncode == 0 and verbose:
+        print(f"{_printColours.GREEN}Successfuly installed {len(fonts)} fonts!{_printColours.END}")
+    elif process.returncode != 0:
+        print(f"{_printColours.RED}One or more of the fonts '{list(fonts.keys())}' could not be installed. Please download and install the font manually, or contact the maintainer of this package, Sam, about the following error message:\nError {process.returncode}: {process.stderr.decode()}{_printColours.END}")
+    
+
+def _refresh_matplotlib_fonts():
+    """
+    Refresh the cache of available fonts to use in matplotlib
+    """
+    mpl_fonts.json_dump(mpl_fonts.FontManager(), os.path.join(mpl.get_cachedir(), f"fontlist-v{mpl_fonts.FontManager.__version__}.json"))
+
```

### Comparing `uintel-0.3.9/src/uintel/ogc.py` & `uintel-0.4.0/src/uintel/ogc.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""Connect to and download Open Geospatial Consortium (OCG) services.
-
-Bulk querying and downloading of geometric data hosted on an OCG GeoServer, such as Web Feature Services (WFS) and Web Map Services (WMS).
-"""
-
-__all__ = ["get_wfs_data"]
-
-import owslib.wfs, requests, geopandas as gpd
-
-
-def get_wfs_data(url: str, layer_name: str = None, projection: int = 2193) -> gpd.GeoDataFrame:
-    """Query a Web Feature Service (WFS) and return all data from a layer.
-    
-    Returns a geopandas.GeoDataFrame of all atrribute and geometric data from a layer in a WFS service.
-        
-    Args:
-        url: String of the OGC Service, with any query parameters followed afterwards. E.g. https://data.wairoadc.govt.nz/geoserver/ows?typeName=geonode:ncs_cemetary_plots.
-        layer_name: Name of the layer to download, if it is not already embedded in the url as the 'typeName' query parameter. E.g. 'geonode:ncs_cemetery_plots'.
-        projection: Integer of the CRS that the data should be returned in.
-
-    Returns:
-        A geopandas.GeoDataFrame containing all geometric data in the requested projection, with any attribute data.
-    
-    Raises:
-        ValueError: Raised if the given layer name is not a part of the WFS 
-        RuntimeError: Raised if there was no given layer to download
-    """
-    wfs = owslib.wfs.WebFeatureService(url, version="1.0.0") # other versions are 1.1.0 and 2.0.0 but not all services will allow these versions so take a cautious approach
-
-    if "typeName=" not in url:
-        if layer_name and layer_name not in wfs.contents:
-            raise ValueError(f"The requested layer '{layer_name}' is not available from {url}.\nPlease choose from the following available layers:\n{list(wfs.contents)}")
-        elif not layer_name:
-            raise RuntimeError("No layer name has been specified. Please embed it as the 'typeName' query parameter in the url, or pass it in through the 'layer_name' parameter to this function call.")
-
-    params = {
-        "service": "WFS",
-        "version": wfs.version,
-        "request": "GetFeature",
-        "typeName": layer_name,
-        "srsName": f"EPSG:{projection}",
-        "outputFormat": "json",
-    }
-
-    wfs_request_url = requests.Request('GET', url, params=params).prepare().url
+"""Connect to and download Open Geospatial Consortium (OCG) services.
+
+Bulk querying and downloading of geometric data hosted on an OCG GeoServer, such as Web Feature Services (WFS) and Web Map Services (WMS).
+"""
+
+__all__ = ["get_wfs_data"]
+
+import owslib.wfs, requests, geopandas as gpd
+
+
+def get_wfs_data(url: str, layer_name: str = None, projection: int = 2193) -> gpd.GeoDataFrame:
+    """Query a Web Feature Service (WFS) and return all data from a layer.
+    
+    Returns a geopandas.GeoDataFrame of all atrribute and geometric data from a layer in a WFS service.
+        
+    Args:
+        url: String of the OGC Service, with any query parameters followed afterwards. E.g. https://data.wairoadc.govt.nz/geoserver/ows?typeName=geonode:ncs_cemetary_plots.
+        layer_name: Name of the layer to download, if it is not already embedded in the url as the 'typeName' query parameter. E.g. 'geonode:ncs_cemetery_plots'.
+        projection: Integer of the CRS that the data should be returned in.
+
+    Returns:
+        A geopandas.GeoDataFrame containing all geometric data in the requested projection, with any attribute data.
+    
+    Raises:
+        ValueError: Raised if the given layer name is not a part of the WFS 
+        RuntimeError: Raised if there was no given layer to download
+    """
+    wfs = owslib.wfs.WebFeatureService(url, version="1.0.0") # other versions are 1.1.0 and 2.0.0 but not all services will allow these versions so take a cautious approach
+
+    if "typeName=" not in url:
+        if layer_name and layer_name not in wfs.contents:
+            raise ValueError(f"The requested layer '{layer_name}' is not available from {url}.\nPlease choose from the following available layers:\n{list(wfs.contents)}")
+        elif not layer_name:
+            raise RuntimeError("No layer name has been specified. Please embed it as the 'typeName' query parameter in the url, or pass it in through the 'layer_name' parameter to this function call.")
+
+    params = {
+        "service": "WFS",
+        "version": wfs.version,
+        "request": "GetFeature",
+        "typeName": layer_name,
+        "srsName": f"EPSG:{projection}",
+        "outputFormat": "json",
+    }
+
+    wfs_request_url = requests.Request('GET', url, params=params).prepare().url
     return gpd.read_file(wfs_request_url)
```

### Comparing `uintel-0.3.9/src/uintel/query.py` & `uintel-0.4.0/src/uintel/query.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""Determine the fastest route from a set of origins to a set of destinations, by any transportation method.
-
-Bulk querying of coordinates to determine the fastest transportation route (by distance or duration) from an origin to the closest destination.
-"""
-
-__all__ = ["get_wfs_data"]
-
-_available_transport_modes = ["driving", "walking", "cycling", "public transport"]
-
-import subprocess, socket, os
-
-def init_osrm(name, transport_mode="driving", continent="australia-oceania", region="new-zealand", subregion=None, update_roads=False):
-    """Creates a docker container with the osrm/osrm-backend image.
-    
-    Create (or refresh) a docker container with the given name, that is set up to be a high-performance open-source routing engine (OSRM). OpenStreetMap (OSM) data is stored in '~/.osm'.
-        
-    Args:
-        name: The name to give the docker container.
-        transport_mode: The type of transportation to be simulating. Options include: 'driving', 'walking' and 'cycling'.
-        continent: The name of the continent to be analysing, e.g. "north-america". See https://download.geofabrik.de/ for a list of available continents.
-        region: The name of the region to be analysing, e.g. "canada". See https://download.geofabrik.de/{continent}.html for a list of available regions.
-        subregion: The name of the subregion to be analysing, e.g. "ontario". Some regions, such as "new-zealand", will not have subregions. See https://download.geofabrik.de/{continent}/{region}.html for a list of available subregions. 
-        update_roads: The path to the csv of which will update roads in the OSM network.
-    
-    Returns:
-        An integer which is the port the docker container is running on 
-    """
-
-    # Determine where to save all the data files
-    osm_directory = os.path.expanduser("~/.osm")
-
-    # Determine free port
-    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    sock.bind(('', 0))
-    port = sock.getsockname()[1]
-    sock.close()
-
-    lua = {'driving':'car','walking':'foot','cycling':'bicycle'}.get(transport_mode, "car")
-
-    # Stop and remove any existing dockers with this name
-    subprocess.run(f'docker stop osrm-{name}'.split(), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-    subprocess.run(f'docker rm osrm-{name}'.split(), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-
-    # Download the data
-    pbf_filepath = f'https://download.geofabrik.de/{continent}/{region}{f"/{subregion}" if subregion else ""}-latest.osm.pbf'
-    download_process = subprocess.run(f'wget -N {pbf_filepath} -P {osm_directory}'.split(), bufsize=0, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
-
-    if not '304 Not Modified' in str(download_process.stderr) or (update_roads != False):
-        # Extract and initialise the data
-        shell_commands = [
-            f'docker run -t -v {osm_directory}:/data osrm/osrm-backend osrm-extract -p /opt/{lua}.lua /data/{subregion if subregion else region}-latest.osm.pbf',
-            f'docker run -t -v {osm_directory}:/data osrm/osrm-backend osrm-partition /data/{subregion if subregion else region}-latest.osrm',
-            f'docker run -t -v {osm_directory}:/data osrm/osrm-backend osrm-customize /data/{subregion if subregion else region}-latest.osrm{f" --segment-speed-file {update_roads}" if update_roads else ""}',
-        ]
-        for com in shell_commands:
-            subprocess.run(com.split(), stdout=open(os.devnull, 'wb'), stderr=subprocess.STDOUT)
-
-    run_docker = f'docker run -d --name osrm-{name} -t -i -p {port}:5000 -v {osm_directory}:/data osrm/osrm-backend osrm-routed --algorithm mld --max-table-size 100000 /data/{subregion if subregion else region}-latest.osrm'
-    subprocess.run(run_docker.split(), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-    return port
-
+"""Determine the fastest route from a set of origins to a set of destinations, by any transportation method.
+
+Bulk querying of coordinates to determine the fastest transportation route (by distance or duration) from an origin to the closest destination.
+"""
+
+__all__ = ["get_wfs_data"]
+
+_available_transport_modes = ["driving", "walking", "cycling", "public transport"]
+
+import subprocess, socket, os
+
+def init_osrm(name, transport_mode="driving", continent="australia-oceania", region="new-zealand", subregion=None, update_roads=False):
+    """Creates a docker container with the osrm/osrm-backend image.
+    
+    Create (or refresh) a docker container with the given name, that is set up to be a high-performance open-source routing engine (OSRM). OpenStreetMap (OSM) data is stored in '~/.osm'.
+        
+    Args:
+        name: The name to give the docker container.
+        transport_mode: The type of transportation to be simulating. Options include: 'driving', 'walking' and 'cycling'.
+        continent: The name of the continent to be analysing, e.g. "north-america". See https://download.geofabrik.de/ for a list of available continents.
+        region: The name of the region to be analysing, e.g. "canada". See https://download.geofabrik.de/{continent}.html for a list of available regions.
+        subregion: The name of the subregion to be analysing, e.g. "ontario". Some regions, such as "new-zealand", will not have subregions. See https://download.geofabrik.de/{continent}/{region}.html for a list of available subregions. 
+        update_roads: The path to the csv of which will update roads in the OSM network.
+    
+    Returns:
+        An integer which is the port the docker container is running on 
+    """
+
+    # Determine where to save all the data files
+    osm_directory = os.path.expanduser("~/.osm")
+
+    # Determine free port
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    sock.bind(('', 0))
+    port = sock.getsockname()[1]
+    sock.close()
+
+    lua = {'driving':'car','walking':'foot','cycling':'bicycle'}.get(transport_mode, "car")
+
+    # Stop and remove any existing dockers with this name
+    subprocess.run(f'docker stop osrm-{name}'.split(), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+    subprocess.run(f'docker rm osrm-{name}'.split(), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+
+    # Download the data
+    pbf_filepath = f'https://download.geofabrik.de/{continent}/{region}{f"/{subregion}" if subregion else ""}-latest.osm.pbf'
+    download_process = subprocess.run(f'wget -N {pbf_filepath} -P {osm_directory}'.split(), bufsize=0, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
+
+    if not '304 Not Modified' in str(download_process.stderr) or (update_roads != False):
+        # Extract and initialise the data
+        shell_commands = [
+            f'docker run -t -v {osm_directory}:/data osrm/osrm-backend osrm-extract -p /opt/{lua}.lua /data/{subregion if subregion else region}-latest.osm.pbf',
+            f'docker run -t -v {osm_directory}:/data osrm/osrm-backend osrm-partition /data/{subregion if subregion else region}-latest.osrm',
+            f'docker run -t -v {osm_directory}:/data osrm/osrm-backend osrm-customize /data/{subregion if subregion else region}-latest.osrm{f" --segment-speed-file {update_roads}" if update_roads else ""}',
+        ]
+        for com in shell_commands:
+            subprocess.run(com.split(), stdout=open(os.devnull, 'wb'), stderr=subprocess.STDOUT)
+
+    run_docker = f'docker run -d --name osrm-{name} -t -i -p {port}:5000 -v {osm_directory}:/data osrm/osrm-backend osrm-routed --algorithm mld --max-table-size 100000 /data/{subregion if subregion else region}-latest.osrm'
+    subprocess.run(run_docker.split(), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+    return port
+
```

### Comparing `uintel-0.3.9/src/uintel/server.py` & `uintel-0.4.0/src/uintel/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,175 +1,174 @@
-"""Connect to Linux servers.
-
-Connect to Linux servers to execute terminal commands, as well as uploading files and/or whole directories to the server.
-"""
-
-__all__ = ["Server"]
-
-import paramiko, os, tqdm, warnings, zipfile, tempfile, glob, logging
-from typing import Union
-from .install import _get_config, _save_config
-
-class Server(object):
-    """
-    A Class of a SSH and SFTP client that can execute commands on any Linux server and send files.
-    """
-    def __init__(self, nickname: str) -> None:
-        """Initilise the class.
-
-        Create a SSH and SFTP client with a server. The server nickname must be saved in your UI configuration file, otherwise you will be asked to authenticate yourself.
-
-        Args:
-            nickname: The nickname of the server that is saved in the UI configuration file.
-        """
-        client = paramiko.SSHClient()
-        try:
-            config = _get_config()
-            servers = config["servers"]
-            credentials = servers[nickname]
-        except KeyError:
-            warnings.warn(f"Unfortunately, {nickname} is not in your saved servers.")
-
-            credentials = {
-                "address": input(f"What is the address for {nickname}? (e.g. 173.42.60.98) "),
-                "username": input(f"What is your username for {nickname}? "),
-                "ssh_key": input(f"Do you use a SSH key to connect to {nickname}? (yes/no) ").lower() == "yes"
-                }
-            if not credentials["ssh_key"]:
-                credentials["password"] = input(f"Since you have indicated you do not use a SSH key for {nickname}, what is your password? ")
-            else:
-                credentials["password"] = None
-            
-            # Save this new connection to the UI configuration file
-            config["servers"][nickname] = credentials
-            _save_config(config)
-
-        log_level = logging.root.level
-        logging.basicConfig(level=logging.ERROR, force=True)
-        try:
-            if credentials["ssh_key"]:
-                # Set it to automatically add the host to known hosts
-                client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-                client.connect(hostname=credentials["address"], username=credentials["username"])
-            else:
-                client.connect(hostname=credentials["address"], username=credentials["username"], password=credentials["password"])
-        except paramiko.SSHException as error:
-            raise paramiko.SSHException(f"Unfortunately, your credentials could not be verified. Connection to {credentials['address']} ({nickname}) failed.\n{error}")
-        
-        self.client = client
-        self.sftp_client = client.open_sftp()
-    
-        logging.basicConfig(level=log_level, force=True)
-
-
-    def close(self) -> None:
-        """Close the connection.
-        
-        Close the SSH and SFTP connections with the server.
-        """
-        self.client.close()
-        self.sftp_client.close()
-
-
-    def execute_command(self, command: str, capture_output: bool = False) -> Union[None, tuple]:
-        """Execute a command.
-
-        Args:
-            command: The command to execute in the server's terminal.
-            capture_output: if True, return the output from the command (stdin, stdout, stderr).
-        
-        Returns:
-            The stdin, stdout and stderr if capture_output=True.
-        """
-        # Execute the command
-        stdin, stdout, stderr = self.client.exec_command(command)
-        
-        error = ''
-        for line in stderr.readlines():
-            error += line
-        if error:
-            warnings.warn(f"The command: {command} could not be executed due to: \n{error}")
-    
-        if capture_output:
-            return stdin, stdout, stderr
-
-
-    def upload_file(self, local_path: str, remote_path: str, show_progress: bool = True, perm: int = 775, group: str = "www-data") -> None:
-        """Upload a file.
-
-        Upload a local file to the given remote filepath on the server.
-
-        Args:
-            local_path: Filepath to be uploaded.
-            remote_path: Filepath on the server to upload to.
-            show_progress: If True, show a progress bar as the file uploads.
-            perm: The integer of the permissions to update the file with, e.g. 775.
-            group: The group to assign the file to.
-        """
-        def print_progress(transferred, toBeTransferred):
-            transferred = round(transferred/1e6, 2) # in MB now
-            toBeTransferred = round(toBeTransferred/1e6, 2) # in MB now
-            if toBeTransferred > 0:
-                # Prevent a divide by zero error
-                print(f"Progress: {100*transferred/toBeTransferred:.2f}%\t Transferred: {transferred:.2f} / {toBeTransferred:.2f} MB", end="\n" if transferred/toBeTransferred == 1 else "\r")
-        
-        # Check the directory specified exists
-        if not os.path.exists(local_path):
-            raise FileNotFoundError(f"The file {local_path} does not exists.")
-
-        # Make sure a directory exists and the old file is deleted
-        self.execute_command(f"mkdir {os.path.dirname(remote_path)}")
-        self.execute_command(f"rm -f {remote_path}")
-
-        _ = self.sftp_client.put(local_path, remote_path, callback=print_progress if show_progress else None, confirm=True)
-        
-        if perm:
-            self.execute_command(f'chmod {perm} {remote_path}')
-        if group:
-            self.execute_command(f'chgrp {group} {remote_path}')
-
-
-    def upload_directory(self, local_directory: str, remote_directory: str, show_progress: bool = True, perm: int = 775, group: str = "www-data") -> None:
-        """Upload an entire folder to the server.
-
-        Zip a directory (or a portion using glob notation) and upload it to the remote filepath on the server and uncompress it.
-
-        Args:
-            local_directory: The path to the folder to upload. This can also be a glob pattern (e.g. "data/**/*.csv") where a filter is applied. 
-            remote_directory: The path on the server to upload to.
-            show_progress: If True, show a progress bar as the file uploads.
-            perm: The integer of the permissions to update the file with, e.g. 775.
-            group: The group to assign the file to.
-        """    
-
-        if "*" not in local_directory:
-            # Convert normal path to glob notation to get everything underneath
-            base_directory = local_directory
-            local_directory = os.path.join(local_directory, "*")
-        else:
-            base_directory = local_directory[:local_directory.index("*")]
-
-        all_files = [fp for fp in glob.glob(local_directory, recursive=True) if os.path.isfile(fp)]
-        
-        if len(all_files) == 0:
-            raise RuntimeError(f"No files matching: {local_directory} were found.")
-        
-        # Make the zip file
-        temp_dir = tempfile.TemporaryDirectory()
-        local_path = os.path.join(temp_dir.name, "zipped_dir.zip")
-        with zipfile.ZipFile(local_path, "w", compression=zipfile.ZIP_DEFLATED) as zip:
-            for filepath in tqdm.tqdm(all_files, "Creating ZIP file", total=len(all_files), leave=False, dynamic_ncols=True):
-                zip.write(filepath, arcname=os.path.relpath(filepath, base_directory))
-
-        # Upload the zip file
-        remote_path = f"{remote_directory if remote_directory.endswith('/') else remote_directory + '/'}zipped_dir.zip"
-        self.upload_file(local_path, remote_path, show_progress, perm, group)
-        # Unzip and overwrite on the server
-        self.execute_command(f"unzip -q -o {remote_path} -d {remote_directory}")
-        # Delete the zip files on the server and local path
-        self.execute_command(f"rm {remote_path}")
-        temp_dir.cleanup()
-        
-        if perm:
-            self.execute_command(f'chmod -R {perm} {remote_directory}')
-        if group:
-            self.execute_command(f'chgrp -R {group} {remote_directory}')
+"""Connect to Linux servers.
+
+Connect to Linux servers to execute terminal commands, as well as uploading files and/or whole directories to the server.
+"""
+
+__all__ = ["Server"]
+
+import paramiko, os, tqdm, warnings, zipfile, tempfile, glob, logging
+from typing import Union
+from .install import _get_config, _save_config
+
+class Server(object):
+    """
+    A Class of a SSH and SFTP client that can execute commands on any Linux server and send files.
+    """
+    def __init__(self, nickname: str) -> None:
+        """Initilise the class.
+
+        Create a SSH and SFTP client with a server. The server nickname must be saved in your UI configuration file, otherwise you will be asked to authenticate yourself.
+
+        Args:
+            nickname: The nickname of the server that is saved in the UI configuration file.
+        """
+        client = paramiko.SSHClient()
+        try:
+            config = _get_config()
+            credentials = config["servers"][nickname]
+        except KeyError:
+            warnings.warn(f"Unfortunately, {nickname} is not in your saved servers.")
+
+            credentials = {
+                "address": input(f"What is the address for {nickname}? (e.g. 173.42.60.98) "),
+                "username": input(f"What is your username for {nickname}? "),
+                "ssh_key": input(f"Do you use a SSH key to connect to {nickname}? (yes/no) ").lower() == "yes"
+                }
+            if not credentials["ssh_key"]:
+                credentials["password"] = input(f"Since you have indicated you do not use a SSH key for {nickname}, what is your password? ")
+            else:
+                credentials["password"] = None
+            
+            # Save this new connection to the UI configuration file
+            config["servers"][nickname] = credentials
+            _save_config(config)
+
+        log_level = logging.root.level
+        logging.basicConfig(level=logging.ERROR, force=True)
+        try:
+            if credentials["ssh_key"]:
+                # Set it to automatically add the host to known hosts
+                client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+                client.connect(hostname=credentials["address"], username=credentials["username"])
+            else:
+                client.connect(hostname=credentials["address"], username=credentials["username"], password=credentials["password"])
+        except paramiko.SSHException as error:
+            raise paramiko.SSHException(f"Unfortunately, your credentials could not be verified. Connection to {credentials['address']} ({nickname}) failed.\n{error}")
+        
+        self.client = client
+        self.sftp_client = client.open_sftp()
+    
+        logging.basicConfig(level=log_level, force=True)
+
+
+    def close(self) -> None:
+        """Close the connection.
+        
+        Close the SSH and SFTP connections with the server.
+        """
+        self.client.close()
+        self.sftp_client.close()
+
+
+    def execute_command(self, command: str, capture_output: bool = False) -> Union[None, tuple]:
+        """Execute a command.
+
+        Args:
+            command: The command to execute in the server's terminal.
+            capture_output: if True, return the output from the command (stdin, stdout, stderr).
+        
+        Returns:
+            The stdin, stdout and stderr if capture_output=True.
+        """
+        # Execute the command
+        stdin, stdout, stderr = self.client.exec_command(command)
+        
+        error = ''
+        for line in stderr.readlines():
+            error += line
+        if error:
+            warnings.warn(f"The command: {command} could not be executed due to: \n{error}")
+    
+        if capture_output:
+            return stdin, stdout, stderr
+
+
+    def upload_file(self, local_path: str, remote_path: str, show_progress: bool = True, perm: int = 775, group: str = "www-data") -> None:
+        """Upload a file.
+
+        Upload a local file to the given remote filepath on the server.
+
+        Args:
+            local_path: Filepath to be uploaded.
+            remote_path: Filepath on the server to upload to.
+            show_progress: If True, show a progress bar as the file uploads.
+            perm: The integer of the permissions to update the file with, e.g. 775.
+            group: The group to assign the file to.
+        """
+        def print_progress(transferred, toBeTransferred):
+            transferred = round(transferred/1e6, 2) # in MB now
+            toBeTransferred = round(toBeTransferred/1e6, 2) # in MB now
+            if toBeTransferred > 0:
+                # Prevent a divide by zero error
+                print(f"Progress: {100*transferred/toBeTransferred:.2f}%\t Transferred: {transferred:.2f} / {toBeTransferred:.2f} MB", end="\n" if transferred/toBeTransferred == 1 else "\r")
+        
+        # Check the directory specified exists
+        if not os.path.exists(local_path):
+            raise FileNotFoundError(f"The file {local_path} does not exists.")
+
+        # Make sure a directory exists and the old file is deleted
+        self.execute_command(f"mkdir {os.path.dirname(remote_path)}")
+        self.execute_command(f"rm -f {remote_path}")
+
+        _ = self.sftp_client.put(local_path, remote_path, callback=print_progress if show_progress else None, confirm=True)
+        
+        if perm:
+            self.execute_command(f'chmod {perm} {remote_path}')
+        if group:
+            self.execute_command(f'chgrp {group} {remote_path}')
+
+
+    def upload_directory(self, local_directory: str, remote_directory: str, show_progress: bool = True, perm: int = 775, group: str = "www-data") -> None:
+        """Upload an entire folder to the server.
+
+        Zip a directory (or a portion using glob notation) and upload it to the remote filepath on the server and uncompress it.
+
+        Args:
+            local_directory: The path to the folder to upload. This can also be a glob pattern (e.g. "data/**/*.csv") where a filter is applied. 
+            remote_directory: The path on the server to upload to.
+            show_progress: If True, show a progress bar as the file uploads.
+            perm: The integer of the permissions to update the file with, e.g. 775.
+            group: The group to assign the file to.
+        """    
+
+        if "*" not in local_directory:
+            # Convert normal path to glob notation to get everything underneath
+            base_directory = local_directory
+            local_directory = os.path.join(local_directory, "*")
+        else:
+            base_directory = local_directory[:local_directory.index("*")]
+
+        all_files = [fp for fp in glob.glob(local_directory, recursive=True) if os.path.isfile(fp)]
+        
+        if len(all_files) == 0:
+            raise RuntimeError(f"No files matching: {local_directory} were found.")
+        
+        # Make the zip file
+        temp_dir = tempfile.TemporaryDirectory()
+        local_path = os.path.join(temp_dir.name, "zipped_dir.zip")
+        with zipfile.ZipFile(local_path, "w", compression=zipfile.ZIP_DEFLATED) as zip:
+            for filepath in tqdm.tqdm(all_files, "Creating ZIP file", total=len(all_files), leave=False, dynamic_ncols=True):
+                zip.write(filepath, arcname=os.path.relpath(filepath, base_directory))
+
+        # Upload the zip file
+        remote_path = f"{remote_directory if remote_directory.endswith('/') else remote_directory + '/'}zipped_dir.zip"
+        self.upload_file(local_path, remote_path, show_progress, perm, group)
+        # Unzip and overwrite on the server
+        self.execute_command(f"unzip -q -o {remote_path} -d {remote_directory}")
+        # Delete the zip files on the server and local path
+        self.execute_command(f"rm {remote_path}")
+        temp_dir.cleanup()
+        
+        if perm:
+            self.execute_command(f'chmod -R {perm} {remote_directory}')
+        if group:
+            self.execute_command(f'chgrp -R {group} {remote_directory}')
```

### Comparing `uintel-0.3.9/src/uintel/slack.py` & `uintel-0.4.0/src/uintel/slack.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,294 +1,271 @@
-"""Quickly send messages or files to a Slack channel or person.
-
-Post messages or files to a channel (public or private) or directly to a person.
-"""
-
-__all__ = ["post_message", "post_files"]
-
-import random, slack_sdk, slack_sdk.errors, socket, textwrap, warnings, json
-from typing import Union, Tuple, Any
-from .install import _get_config, _save_config
-
-_GREETINGS = ["Kia ora!", "Howdy partner.", "G'day mate.", "What up g? :sunglasses:", "Ugh finally, this shit is done.", "Kachow! :racing_car:", "Kachigga! :racing_car:", "Sup dude.", "Woaaaaahhhh, would you look at that!", "Easy peasy.", "Rock on bro. :call_me_hand:", "Leshgoooooo!", "Let's get this bread!", "You're doing great dude. :kissing_heart:", "Another one bits the dust...", "Sup, having a good day?", "Yeeeeeeehaw cowboy! :face_with_cowboy_hat:"] 
-
-
-def post_message(to: str, message: str, silent_usernames: Union[str, list] = None, identifier: str = None, greet: bool = False, domain: str = "UI") -> None:
-    """Post a message to a Slack Channel or User.
-    
-    Send a message (with an optional header that states an identifier statement and computer name) to a Slack channel or user. If sending to a channel with multiple people that you don't wish to disturb, specific people can be given as silent_usernames and only they will be able see the message.
-
-    Args:
-        to: Where or who to post the message. To directly message someone, use their first name, full name or their nickname on Slack. E.g., "#canterbury-resilience", "Sam", "Mitchell Anderson".
-        message: The message to post.
-        silent_usernames: A single name (string) or multiple names (list) to will get notified and be able to see the message.
-        identifier: A unique identifier that should be placed as a header for the sending message.
-        greet: If True, send an informal greeting before the message.
-        domain: The Slack domain to post to. E.g. "UI" or "UC". The domain chosen should be the name you gave it in your UI configuration file.
-
-    Returns:
-        None.
-
-    Raises:
-        slack_sdk.errors.SlackApiError: Message cannot be posted due to at least one reason.
-    """
-
-    # Check which slack domain to post to
-    try:
-        config = _get_config()
-        token = config["slack"][domain]
-    except KeyError:
-        # Save this new slack domain to the UI configuration file
-        token = input(f"Unfortunately, {domain} is not in your saved Slack domains. Please type in the access token for {domain}: ")
-        config["slack"][domain] = token
-        _save_config(config)
-
-    # Start up the client to post to
-    client = slack_sdk.WebClient(token=token)
-    
-    # If it is not a channel, grab the user's ID instead to DM them
-    if not to.startswith("#"):
-        to = _get_users_information_from_name(to, "id", client)
-
-    # Generate the content used in the message
-    if identifier:
-        header, header_lines = _generate_header(identifier) 
-    else:
-        header, header_lines = "", []
-    blocks = _generate_blocks(message, header_lines, greet)
-
-    try:
-        # Send a quiet message if requested
-        if not silent_usernames:
-            if type(silent_usernames) == str:
-                silent_user_ids = [_get_users_information_from_name(silent_usernames, "id", client)]
-            elif type(silent_usernames) == list:
-                silent_user_ids = [_get_users_information_from_name(silent_username, "id", client) for silent_username in silent_usernames]
-            for silent_user_id in silent_user_ids:
-                _ = client.chat_postEphemeral(channel=to, blocks=blocks, user=silent_user_id, text=header)
-        # Or send it to a public/private channel
-        else:
-            _ = client.chat_postMessage(channel=to, blocks=blocks, text=header)
-    
-    except slack_sdk.errors.SlackApiError as error:
-        warnings.warn(f"The message could not be posted to slack. Error: {error.response['error']}")
-
-
-def _generate_header(identifier: str) -> Tuple[str, list]:
-    """
-    Generates a header, or a list of headers depending on the length of the header, to be used to quickly summarise the message to be posted to the Slack channel or User.
-    """
-    # Unfortunately, there is a 150 character limit on the header length, so split and send multiple if that is the case!
-    header = f'{identifier} |  Running on {socket.gethostname()}'
-    if len(header) > 150:
-        header_lines = textwrap.wrap(header, width=100, break_long_words=False, break_on_hyphens=False)
-    else:
-        header_lines = [header]
-
-    return header, header_lines
-
-
-def _generate_blocks(message_type: str, message: str, header_lines: list, greet: bool):
-    """
-    Generates the blocks, a JSON-based list of structured blocks presented as URL-encoded strings, to be used to display message to be posted to the Slack channel or User.
-    Example:
-    [{"type": "section", "text": {"type": "plain_text", "text": "Hello world"}}]    
-    """
-
-    greeting = random.sample(_GREETINGS, 1)[0] + " " if greet else ""
-
-    blocks=[]
-
-    if header_lines != None:
-        for header_line in header_lines:
-            blocks.append({"type": "header", 
-                            "text":
-                                {"type": "plain_text", 
-                                "text": header_line, 
-                                "emoji": True}
-                            })
-        blocks.append({"type": "divider"})
-
-    if message_type.title() ==  "Information":
-        blocks.append({ "type": "section",
-                        "text": {"type": "mrkdwn",
-                                "text": greeting+message}
-                        })       
-    elif message_type.title() == "Success":
-        blocks.append({"type": "section",
-                        "text": {"type": "mrkdwn",
-                                "text": greeting+"It is my pleasure to inform you that the procedure has been a success."}
-                        })       
-    elif message_type.title() == "Failure": 
-        # Strip away any output in stdout before the error message begins
-        lookout_phrase = "Traceback (most recent call last):"
-        if lookout_phrase in message:
-            message = message[message.index(lookout_phrase)+len(lookout_phrase):].strip()
-
-        blocks.extend([{"type": "section",
-                        "text": {"type": "mrkdwn",
-                                "text": f"{greeting}It is unfortunate that I must inform that something went wrong."}
-                        },
-                    {"type": "section",
-                    "text": {"type": "mrkdwn",
-                            "text": "*Error Traceback:*"}
-                    },
-                    {"type": "divider"},
-                    {"type": "section",
-                    "text": {"type": "mrkdwn",
-                            "text": message.strip("\r\n")}
-                    }])
-    
-    return blocks
-
-
-def post_files(to: str, filenames: Union[str, list], message: str = None, greet: bool = True, domain: str = "UI") -> None:
-    """Posts file(s) to a Slack Channel or User.
-    
-    Send files (with an optional prefacing message) to a Slack channel or user. 
-
-    Args:
-        to: Where or who to post the message. To directly message someone, use their first name, full name or their nickname on Slack. E.g., "#canterbury-resilience", "Sam", "Mitchell Anderson".
-        filenames: A list of filepaths of the files to upload. If sending one file, a string is satisfcatory. 
-        message: A prefacing message before the files are
-        greet: If True, send an informal greeting before the message.
-        domain: The Slack domain to post to. E.g. "UI" or "UC". The domain chosen should be the name you gave it in your UI configuration file.
-
-    Returns:
-        None.
-
-    Raises:
-        slack_sdk.errors.SlackApiError: Files cannot be posted due to at least one reason.
-    """
-
-    # Check which slack domain to post to
-    try:
-        config = _get_config()
-        token = config["slack"][domain]
-    except KeyError:
-        # Save this new slack domain to the UI configuration file
-        token = input(f"Unfortunately, {domain} is not in your saved Slack domains. Please type in the access token for {domain}: ")
-        config["slack"][domain] = token
-        _save_config(config)
-
-    # Start up the client to post to
-    client = slack_sdk.WebClient(token=token)
-    
-    # If it is not a channel, grab the user's ID instead to DM them
-    if not to.startswith("#"):
-        to = _get_users_information_from_name(to, "id", client)
-
-    # Add a greeting if the user asked for one
-    greeting = random.sample(_GREETINGS, 1)[0] + " " if greet else ""
-    
-    # In case only one file was passed in, then chuck the string into a list by itself
-    if type(filenames) == str:
-        filenames = [filenames]
-
-    try:
-        inital_comment_sent = False
-        for filename in filenames:
-            if not inital_comment_sent:
-                # Send the files with the initial comment as it has not been sent yet
-                _ = client.files_upload(channels=to, initial_comment=greeting+message, file=filename)
-                inital_comment_sent = True
-            else:
-                # Otherwise send just the files
-                _ = client.files_upload(channels=to, file=filename)
-    
-    except slack_sdk.errors.SlackApiError as error:
-        warnings.warn("The file {} could not be posted to slack. Error: {}".format(filename, error.response["error"]), UserWarning)
-
-
-def _get_users_information_from_name(user_name: str, wanted_information: str, client: slack_sdk.WebClient) -> Any:
-    """
-    Retrieves a specified *wanted_information* attribute of a user by the name of *user_name*. The *user_name* can be the full name of the individual or their display name. If no exact matches are found, then possible matches are considered by their full name, display name and by first name and surname.    
-    """
-
-    # Change the user_name to title case so we can == compare it with the other fields
-    user_name = user_name.title()
-    
-    # Create lists for exact and possible matches
-    exact_matches = []
-    possible_matches = []
-
-    # Query the client for a list of members
-    members = client.users_list()["members"]
-
-    for member in members:
-        # If inactive user or is a bot then continue to the next
-        if member["deleted"] or member["is_bot"]:
-            continue
-        
-        # Check for exact results of id! E.g. the user passed in the actual id of the person, so why bother looking any further!
-        if member.get("id", "") == user_name:
-            return user_name
-        
-        # Check for exact mataches against the profile
-        profile_details = member.get("profile", {})
-        if profile_details.get("real_name", "").title() == user_name:
-            exact_matches.append(member)
-        elif profile_details.get("display_name", "").title() == user_name:
-            exact_matches.append(member)
-        elif profile_details.get("real_name_normalized", "").title() == user_name:
-            exact_matches.append(member)
-        elif profile_details.get("display_name_normalized", "").title() == user_name:
-            exact_matches.append(member)
-
-        # Check for possible matches
-        elif user_name in member.get("id", ""):
-            possible_matches.append(member)
-        elif user_name in profile_details.get("real_name", "").title():
-            possible_matches.append(member)
-        elif user_name in profile_details.get("display_name", "").title():
-            possible_matches.append(member)
-        elif user_name in profile_details.get("real_name_normalized", "").title():
-            possible_matches.append(member)
-        elif user_name in profile_details.get("display_name_normalized", "").title():
-            possible_matches.append(member)
-        elif user_name.split(" ")[0] in profile_details.get("first_name", "").title():
-            possible_matches.append(member)
-        elif user_name.split(" ")[-1] in profile_details.get("last_name", "").title():
-            possible_matches.append(member)
-
-    
-    if len(exact_matches) == 1:
-        # Best case scenario!
-        chosen_user_details = exact_matches[0]
-
-    elif len(exact_matches) > 1:
-        print(f"Multiple users detected with the user_name '{user_name}'. Please define which user you are indending to post to from the current list:\n")
-        counter = 1
-        for exact_match in exact_matches:
-            print(f"Possible Match {counter}:")
-            print(exact_match, end="\n")
-            counter +=1 
-        correct_individual_number = int(input(f"From this list, which number (from 1 to {len(exact_matches)}) was the user you were wishing to post locate?"))
-        chosen_user_details = exact_matches[correct_individual_number - 1]
-    
-    else:
-        if len(possible_matches) == 1:
-            chosen_user_details = possible_matches[0]
-        else:
-            print(f"No exact matches were found for '{user_name}. However, multiple possible matches exists. Please define which user you are indending to post to from the current list:\n")
-            counter = 1
-            for possible_match in possible_matches:
-                print(f"Possible Match {counter}:")
-                print(possible_match, end="\n")
-                counter +=1 
-            correct_individual_number = int(input(f"From this list, which number (from 1 to {len(possible_matches)}) was the user you were wishing to post locate?"))
-            chosen_user_details = possible_matches[correct_individual_number - 1]
-
-    # Now grab the wanted_information from the chosen_user_details
-    if wanted_information in chosen_user_details:
-        chosen_information = chosen_user_details[wanted_information]
-    elif wanted_information in chosen_user_details["profile"]:
-        chosen_information = chosen_user_details["profile"][wanted_information]
-    else:
-        keys = sorted(set(list(chosen_user_details.keys()) + list(chosen_user_details["profile"].keys())))
-        correct_wanted_information = input(f"The user name {user_name} was found but the wanted information {wanted_information} is not within the recorded details. Please choose from the following:\n {keys}")
-        if correct_wanted_information in chosen_user_details:
-            chosen_information = chosen_user_details[correct_wanted_information]
-        elif correct_wanted_information in chosen_user_details["profile"]:
-            chosen_information = chosen_user_details["profile"][correct_wanted_information]
-    
-    return chosen_information
+"""Quickly send messages or files to a Slack channel or person.
+
+Post messages or files to a channel (public or private) or directly to a person.
+"""
+
+__all__ = ["post_message", "post_files"]
+
+import random, slack_sdk, slack_sdk.errors, socket, textwrap, warnings
+from typing import Union, Tuple, Any
+from .install import _get_config, _save_config
+
+_GREETINGS = ["Kia ora!", "Howdy partner.", "G'day mate.", "What up g? :sunglasses:", "Ugh finally, this shit is done.", "Kachow! :racing_car:", "Kachigga! :racing_car:", "Sup dude.", "Woaaaaahhhh, would you look at that!", "Easy peasy.", "Rock on bro. :call_me_hand:", "Leshgoooooo!", "Let's get this bread!", "You're doing great dude. :kissing_heart:", "Another one bits the dust...", "Sup, having a good day?", "Yeeeeeeehaw cowboy! :face_with_cowboy_hat:"] 
+
+
+def post_message(to: str, message: str, silent_usernames: Union[str, list] = None, identifier: str = None, greet: bool = False, domain: str = "UI") -> None:
+    """Post a message to a Slack Channel or User.
+    
+    Send a message (with an optional header that states an identifier statement and computer name) to a Slack channel or user. If sending to a channel with multiple people that you don't wish to disturb, specific people can be given as silent_usernames and only they will be able see the message.
+
+    Args:
+        to: Where or who to post the message. To directly message someone, use their first name, full name or their nickname on Slack. E.g., "#canterbury-resilience", "Sam", "Mitchell Anderson".
+        message: The message to post.
+        silent_usernames: A single name (string) or multiple names (list) to will get notified and be able to see the message.
+        identifier: A unique identifier that should be placed as a header for the sending message.
+        greet: If True, send an informal greeting before the message.
+        domain: The Slack domain to post to. E.g. "UI" or "UC". The domain chosen should be the name you gave it in your UI configuration file.
+
+    Returns:
+        None.
+
+    Raises:
+        slack_sdk.errors.SlackApiError: Message cannot be posted due to at least one reason.
+    """
+
+    # Check which slack domain to post to
+    config = _get_config()
+    try:
+        token = config["slack"][domain]
+    except KeyError:
+        # Save this new slack domain to the UI configuration file
+        token = input(f"Unfortunately, {domain} is not in your saved Slack domains. Please type in the access token for {domain}: ")
+        config["slack"][domain] = token
+        _save_config(config)
+
+    # Start up the client to post to
+    client = slack_sdk.WebClient(token=token)
+    
+    # If it is not a channel, grab the user's ID instead to DM them
+    if not to.startswith("#"):
+        to = _get_users_information_from_name(to, "id", client)
+
+    # Generate the content used in the message
+    if identifier:
+        header, header_lines = _generate_header(identifier) 
+    else:
+        header, header_lines = "", []
+    blocks = _generate_blocks(message, header_lines, greet)
+
+    try:
+        # Send a quiet message if requested
+        if silent_usernames != None:
+            if type(silent_usernames) == str:
+                silent_user_ids = [_get_users_information_from_name(silent_usernames, "id", client)]
+            elif type(silent_usernames) == list:
+                silent_user_ids = [_get_users_information_from_name(silent_username, "id", client) for silent_username in silent_usernames]
+            for silent_user_id in silent_user_ids:
+                _ = client.chat_postEphemeral(channel=to, blocks=blocks, user=silent_user_id, text=header)
+        # Or send it to a public/private channel
+        else:
+            _ = client.chat_postMessage(channel=to, blocks=blocks, text=header)
+    
+    except slack_sdk.errors.SlackApiError as error:
+        warnings.warn(f"The message could not be posted to slack. Error: {error.response['error']}")
+
+
+def _generate_header(identifier: str) -> Tuple[str, list]:
+    """
+    Generates a header, or a list of headers depending on the length of the header, to be used to quickly summarise the message to be posted to the Slack channel or User.
+    """
+    # Unfortunately, there is a 150 character limit on the header length, so split and send multiple if that is the case!
+    header = f'{identifier} |  Running on {socket.gethostname()}'
+    if len(header) > 150:
+        header_lines = textwrap.wrap(header, width=100, break_long_words=False, break_on_hyphens=False)
+    else:
+        header_lines = [header]
+
+    return header, header_lines
+
+
+def _generate_blocks(message: str, header_lines: list, greet: bool):
+    """
+    Generates the blocks, a JSON-based list of structured blocks presented as URL-encoded strings, to be used to display message to be posted to the Slack channel or User.
+    Example:
+    [{"type": "section", "text": {"type": "plain_text", "text": "Hello world"}}]    
+    """
+
+    greeting = random.sample(_GREETINGS, 1)[0] + " " if greet else ""
+
+    blocks = []
+    if header_lines != None:
+        for header_line in header_lines:
+            blocks.append({"type": "header", 
+                            "text":
+                                {"type": "plain_text", 
+                                "text": header_line, 
+                                "emoji": True}
+                            })
+        blocks.append({"type": "divider"})
+
+    blocks.append({ 
+        "type": "section",
+        "text": {
+            "type": "mrkdwn",
+            "text": greeting + message
+            }
+        })       
+    
+    return blocks
+
+
+def post_files(to: str, filenames: Union[str, list], message: str = None, greet: bool = True, domain: str = "UI") -> None:
+    """Posts file(s) to a Slack Channel or User.
+    
+    Send files (with an optional prefacing message) to a Slack channel or user. 
+
+    Args:
+        to: Where or who to post the message. To directly message someone, use their first name, full name or their nickname on Slack. E.g., "#canterbury-resilience", "Sam", "Mitchell Anderson".
+        filenames: A list of filepaths of the files to upload. If sending one file, a string is satisfcatory. 
+        message: A prefacing message before the files are
+        greet: If True, send an informal greeting before the message.
+        domain: The Slack domain to post to. E.g. "UI" or "UC". The domain chosen should be the name you gave it in your UI configuration file.
+
+    Returns:
+        None.
+
+    Raises:
+        slack_sdk.errors.SlackApiError: Files cannot be posted due to at least one reason.
+    """
+
+    # Check which slack domain to post to
+    config = _get_config()
+    try:
+        token = config["slack"][domain]
+    except KeyError:
+        # Save this new slack domain to the UI configuration file
+        token = input(f"Unfortunately, {domain} is not in your saved Slack domains. Please type in the access token for {domain}: ")
+        config["slack"][domain] = token
+        _save_config(config)
+
+    # Start up the client to post to
+    client = slack_sdk.WebClient(token=token)
+    
+    # If it is not a channel, grab the user's ID instead to DM them
+    if not to.startswith("#"):
+        to = _get_users_information_from_name(to, "id", client)
+
+    # Add a greeting if the user asked for one
+    greeting = random.sample(_GREETINGS, 1)[0] + " " if greet else ""
+    
+    # In case only one file was passed in, then chuck the string into a list by itself
+    if type(filenames) == str:
+        filenames = [filenames]
+
+    try:
+        inital_comment_sent = False
+        for filename in filenames:
+            if not inital_comment_sent:
+                # Send the files with the initial comment as it has not been sent yet
+                _ = client.files_upload(channels=to, initial_comment=greeting+message, file=filename)
+                inital_comment_sent = True
+            else:
+                # Otherwise send just the files
+                _ = client.files_upload(channels=to, file=filename)
+    
+    except slack_sdk.errors.SlackApiError as error:
+        warnings.warn("The file {} could not be posted to slack. Error: {}".format(filename, error.response["error"]), UserWarning)
+
+
+def _get_users_information_from_name(user_name: str, wanted_information: str, client: slack_sdk.WebClient) -> Any:
+    """
+    Retrieves a specified *wanted_information* attribute of a user by the name of *user_name*. The *user_name* can be the full name of the individual or their display name. If no exact matches are found, then possible matches are considered by their full name, display name and by first name and surname.    
+    """
+
+    # Change the user_name to title case so we can == compare it with the other fields
+    user_name = user_name.title()
+    
+    # Create lists for exact and possible matches
+    exact_matches = []
+    possible_matches = []
+
+    # Query the client for a list of members
+    members = client.users_list()["members"]
+
+    for member in members:
+        # If inactive user or is a bot then continue to the next
+        if member["deleted"] or member["is_bot"]:
+            continue
+        
+        # Check for exact results of id! E.g. the user passed in the actual id of the person, so why bother looking any further!
+        if member.get("id", "") == user_name:
+            return user_name
+        
+        # Check for exact mataches against the profile
+        profile_details = member.get("profile", {})
+        if profile_details.get("real_name", "").title() == user_name:
+            exact_matches.append(member)
+        elif profile_details.get("display_name", "").title() == user_name:
+            exact_matches.append(member)
+        elif profile_details.get("real_name_normalized", "").title() == user_name:
+            exact_matches.append(member)
+        elif profile_details.get("display_name_normalized", "").title() == user_name:
+            exact_matches.append(member)
+
+        # Check for possible matches
+        elif user_name in member.get("id", ""):
+            possible_matches.append(member)
+        elif user_name in profile_details.get("real_name", "").title():
+            possible_matches.append(member)
+        elif user_name in profile_details.get("display_name", "").title():
+            possible_matches.append(member)
+        elif user_name in profile_details.get("real_name_normalized", "").title():
+            possible_matches.append(member)
+        elif user_name in profile_details.get("display_name_normalized", "").title():
+            possible_matches.append(member)
+        elif user_name.split(" ")[0] in profile_details.get("first_name", "").title():
+            possible_matches.append(member)
+        elif user_name.split(" ")[-1] in profile_details.get("last_name", "").title():
+            possible_matches.append(member)
+
+    
+    if len(exact_matches) == 1:
+        # Best case scenario!
+        chosen_user_details = exact_matches[0]
+
+    elif len(exact_matches) > 1:
+        print(f"Multiple users detected with the user_name '{user_name}'. Please define which user you are indending to post to from the current list:\n")
+        counter = 1
+        for exact_match in exact_matches:
+            print(f"Possible Match {counter}:")
+            print(exact_match, end="\n")
+            counter +=1 
+        correct_individual_number = int(input(f"From this list, which number (from 1 to {len(exact_matches)}) was the user you were wishing to post locate?"))
+        chosen_user_details = exact_matches[correct_individual_number - 1]
+    
+    else:
+        if len(possible_matches) == 1:
+            chosen_user_details = possible_matches[0]
+        else:
+            print(f"No exact matches were found for '{user_name}. However, multiple possible matches exists. Please define which user you are indending to post to from the current list:\n")
+            counter = 1
+            for possible_match in possible_matches:
+                print(f"Possible Match {counter}:")
+                print(possible_match, end="\n")
+                counter +=1 
+            correct_individual_number = int(input(f"From this list, which number (from 1 to {len(possible_matches)}) was the user you were wishing to post locate?"))
+            chosen_user_details = possible_matches[correct_individual_number - 1]
+
+    # Now grab the wanted_information from the chosen_user_details
+    if wanted_information in chosen_user_details:
+        chosen_information = chosen_user_details[wanted_information]
+    elif wanted_information in chosen_user_details["profile"]:
+        chosen_information = chosen_user_details["profile"][wanted_information]
+    else:
+        keys = sorted(set(list(chosen_user_details.keys()) + list(chosen_user_details["profile"].keys())))
+        correct_wanted_information = input(f"The user name {user_name} was found but the wanted information {wanted_information} is not within the recorded details. Please choose from the following:\n {keys}")
+        if correct_wanted_information in chosen_user_details:
+            chosen_information = chosen_user_details[correct_wanted_information]
+        elif correct_wanted_information in chosen_user_details["profile"]:
+            chosen_information = chosen_user_details["profile"][correct_wanted_information]
+    
+    return chosen_information
```

### Comparing `uintel-0.3.9/src/uintel/styles/ui.mplstyle` & `uintel-0.4.0/src/uintel/styles/ui.mplstyle`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-### Matplotlib style for general UI blue plots.
-
-# Use Rubik font in 10pt
-font.serif : Rubik
-font.family : sans-serif
-font.size : 10
-figure.titlesize : 10
-
-# Set color cycle:
-axes.prop_cycle : cycler('color', ['0B2948', '04497C', 'F86302', 'FF8200', 'FFB451'])
-
-# Set x axis
-xtick.direction : out
-xtick.major.size : 3
-xtick.major.width : 0.5
-xtick.minor.size : 1.5
-xtick.minor.width : 0.5
-xtick.minor.visible : True
-xtick.top : False
-
-# Set y axis
-ytick.direction : out
-ytick.major.size : 3
-ytick.major.width : 0.5
-ytick.minor.size : 1.5
-ytick.minor.width : 0.5
-ytick.minor.visible : True
-ytick.right : False
-
-# Set line widths
-axes.linewidth : 0.5
-grid.linewidth : 0.5
-lines.linewidth : 1.0
-
-# Set font size of the plot elements to less than the title fontsize
-axes.titlesize : 8
-axes.labelsize : 8
-xtick.labelsize : 8 
-ytick.labelsize : 8 
-legend.fontsize : 8
-
-# Set default figure size
-figure.figsize : 7, 5
-
-# Remove legend frame
-legend.frameon : False
-
-# Always save as 'tight'
-savefig.bbox : tight
-savefig.pad_inches : 0.1
+### Matplotlib style for general UI blue plots.
+
+# Use Rubik font in 10pt
+font.serif : Rubik
+font.family : sans-serif
+font.size : 10
+figure.titlesize : 10
+
+# Set color cycle:
+axes.prop_cycle : cycler('color', ['0B2948', '04497C', 'F86302', 'FF8200', 'FFB451'])
+
+# Set x axis
+xtick.direction : out
+xtick.major.size : 3
+xtick.major.width : 0.5
+xtick.minor.size : 1.5
+xtick.minor.width : 0.5
+xtick.minor.visible : True
+xtick.top : False
+
+# Set y axis
+ytick.direction : out
+ytick.major.size : 3
+ytick.major.width : 0.5
+ytick.minor.size : 1.5
+ytick.minor.width : 0.5
+ytick.minor.visible : True
+ytick.right : False
+
+# Set line widths
+axes.linewidth : 0.5
+grid.linewidth : 0.5
+lines.linewidth : 1.0
+
+# Set font size of the plot elements to less than the title fontsize
+axes.titlesize : 8
+axes.labelsize : 8
+xtick.labelsize : 8 
+ytick.labelsize : 8 
+legend.fontsize : 8
+
+# Set default figure size
+figure.figsize : 7, 5
+
+# Remove legend frame
+legend.frameon : False
+
+# Always save as 'tight'
+savefig.bbox : tight
+savefig.pad_inches : 0.1
 savefig.dpi : 300
```

### Comparing `uintel-0.3.9/src/uintel.egg-info/PKG-INFO` & `uintel-0.4.0/src/uintel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-Metadata-Version: 2.1
-Name: uintel
-Version: 0.3.9
-Summary: Urban Intelligence's unified Python data analysis toolkit
-Home-page: https://uintel.github.io/pyui/
-Author: Sam Archie
-Author-email: sam.archie@urbanintelligence.co.nz
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
-
-<div align="center">
-  <img src="https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"><br>
-</div>
-
------------------
-
-# uintel: unified Python data analysis toolkit
-[![PyPI Latest Release](https://img.shields.io/pypi/v/uintel.svg)](https://pypi.org/project/uintel/)
-[![License](https://img.shields.io/pypi/l/uintel.svg)](https://github.com/uintel/pyui/blob/main/LICENSE)
-
-## What is it?
-
-**uintel** is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts. 
-
-
-## Main Features
-
-  - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
-  - Creating colour palettes relating to Urban Intelligence's main products
-  - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
-  - Bulk querying (public and private) ESRI servers to download geometric data with attributes
-  - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
-  - Quickly send messages or files to a Slack channel or person
-  - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
-  - Quickly convert a GeoDataFrame to a simplified topojson file
-  - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
-  - Determine the fastest transportation route between a set of origins and destinations
-
-## Where to get it
-The source code is currently hosted on GitHub at: [https://github.com/uintel/pyui](https://github.com/uintel/pyui)
-
-Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/uintel) by running:
-
-```sh
-pip install uintel
-```
-
-> If `pip install uintel` fails due to required packages that are known to be tricky, such as GDAL, the binary distributions can be downloaded from: [https://www.lfd.uci.edu/~gohlke/pythonlibs](https://www.lfd.uci.edu/~gohlke/pythonlibs). 
-
-> For more convenience on Windows, `pip install pipwin` and `pipwin install gdal` is an approach that downloads the right binary wheel from Christoph Gohlke.
-
-> For Linux distributions, check the available version of GDAL by running `ogrinfo --version` and then perform `pip install gdal==available_version`. Typically on our analyst computers, the available version is 3.0.4.
-
-## Configuration
-Each time ```uintel``` is imported,
-
-```py
-import uintel as ui
-```
-
-all necessary installations shall begin that have not been completed before. This will include creating a configuration file, installing fonts and modifying matplotlib - if it has not been done so before.
-
-If you have adjusted your computer and the UI defaults have altered, you can revert them by running:
-
-```py
-ui.reset_fonts()
-ui.reset_styles()
-ui.reset_config()
-```
-
-## Documentation
-Documentation is available at [https://uintel.github.io/pyui/](https://uintel.github.io/pyui/)
+Metadata-Version: 2.1
+Name: uintel
+Version: 0.4.0
+Summary: Urban Intelligence's unified Python data analysis toolkit
+Home-page: https://uintel.github.io/pyui/
+Author: Sam Archie
+Author-email: sam.archie@urbanintelligence.co.nz
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
+Description-Content-Type: text/markdown
+Provides-Extra: full
+License-File: LICENSE
+
+<div align="center">
+  <img src="https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"><br>
+</div>
+
+-----------------
+
+# uintel: unified Python data analysis toolkit
+[![PyPI Latest Release](https://img.shields.io/pypi/v/uintel.svg)](https://pypi.org/project/uintel/)
+[![License](https://img.shields.io/pypi/l/uintel.svg)](https://github.com/uintel/pyui/blob/main/LICENSE)
+
+## What is it?
+
+**uintel** is a Python package that provides all the common-day functions and tools for analysts at Urban Intelligence Ltd. It aims to reduce re-using of generic code between similar projects, which leads to bug duplication and further security vulnerabilities. Building upon this, another mission of this package is to install Urban Intelligence's style guides by modifying the matplotlib installation and installing fonts. 
+
+
+## Main Features
+
+  - Easy uploading of files to Amazon Web Services S3 buckets, and appropriate versioning control for data cache handling
+  - Creating colour palettes relating to Urban Intelligence's main products
+  - Connecting (and creating) databases on postgreSQL servers, as well as uploading DataFrames to a database
+  - Bulk querying (public and private) ESRI servers to download geometric data with attributes
+  - Connecting to Linux servers (e.g. Piwakawaka) to execute terminal commands, as well as uploading files and/or whole directories to the server
+  - Quickly send messages or files to a Slack channel or person
+  - Calculate statistics of raster files over a polygon geometry ("zonal statistics")
+  - Quickly convert a GeoDataFrame to a simplified topojson file
+  - Bulk querying (public and private) OGC Web Feature Services (WFS) to download geometric data with attributes
+  - Determine the fastest transportation route between a set of origins and destinations
+
+## Where to get it
+The source code is currently hosted on GitHub at: [https://github.com/uintel/pyui](https://github.com/uintel/pyui)
+
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/uintel) by running:
+
+```sh
+pip install uintel
+```
+
+> If `pip install uintel` fails due to required packages that are known to be tricky, such as GDAL, the binary distributions can be downloaded from: [https://www.lfd.uci.edu/~gohlke/pythonlibs](https://www.lfd.uci.edu/~gohlke/pythonlibs). 
+
+> For more convenience on Windows, `pip install pipwin` and `pipwin install gdal` is an approach that downloads the right binary wheel from Christoph Gohlke.
+
+> For Linux distributions, check the available version of GDAL by running `ogrinfo --version` and then perform `pip install gdal==available_version`. Typically on our analyst computers, the available version is 3.0.4.
+
+## Configuration
+Each time ```uintel``` is imported,
+
+```py
+import uintel as ui
+```
+
+all necessary installations shall begin that have not been completed before. This will include creating a configuration file, installing fonts and modifying matplotlib - if it has not been done so before.
+
+If you have adjusted your computer and the UI defaults have altered, you can revert them by running:
+
+```py
+ui.reset_fonts()
+ui.reset_styles()
+ui.reset_config()
+```
+
+## Documentation
+Documentation is available at [https://uintel.github.io/pyui/](https://uintel.github.io/pyui/)
```

### Comparing `uintel-0.3.9/src/uintel.egg-info/SOURCES.txt` & `uintel-0.4.0/src/uintel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

