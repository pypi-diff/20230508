# Comparing `tmp/pynetcf-0.4.0.tar.gz` & `tmp/pynetcf-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynetcf-0.4.0.tar", last modified: Tue Jan 31 21:04:11 2023, max compression
+gzip compressed data, was "pynetcf-0.5.0.tar", last modified: Mon May  8 08:12:02 2023, max compression
```

## Comparing `pynetcf-0.4.0.tar` & `pynetcf-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.376609 pynetcf-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-01-31 21:04:03.000000 pynetcf-0.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.368609 pynetcf-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.372609 pynetcf-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-31 21:04:03.000000 pynetcf-0.4.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-31 21:04:03.000000 pynetcf-0.4.0/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-01-31 21:04:03.000000 pynetcf-0.4.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-31 21:04:03.000000 pynetcf-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-31 21:04:03.000000 pynetcf-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-31 21:04:03.000000 pynetcf-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-01-31 21:04:03.000000 pynetcf-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-31 21:04:03.000000 pynetcf-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-01-31 21:04:11.376609 pynetcf-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-01-31 21:04:03.000000 pynetcf-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.372609 pynetcf-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.372609 pynetcf-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-31 21:04:03.000000 pynetcf-0.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-31 21:04:03.000000 pynetcf-0.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-31 21:04:03.000000 pynetcf-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-31 21:04:11.376609 pynetcf-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-31 21:04:03.000000 pynetcf-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.368609 pynetcf-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.372609 pynetcf-0.4.0/src/pynetcf/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-31 21:04:03.000000 pynetcf-0.4.0/src/pynetcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-01-31 21:04:03.000000 pynetcf-0.4.0/src/pynetcf/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-01-31 21:04:03.000000 pynetcf-0.4.0/src/pynetcf/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-01-31 21:04:03.000000 pynetcf-0.4.0/src/pynetcf/point_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    59836 2023-01-31 21:04:03.000000 pynetcf-0.4.0/src/pynetcf/time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.372609 pynetcf-0.4.0/src/pynetcf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-01-31 21:04:11.000000 pynetcf-0.4.0/src/pynetcf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-31 21:04:11.000000 pynetcf-0.4.0/src/pynetcf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 21:04:11.000000 pynetcf-0.4.0/src/pynetcf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 21:04:11.000000 pynetcf-0.4.0/src/pynetcf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-31 21:04:11.000000 pynetcf-0.4.0/src/pynetcf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 21:04:11.000000 pynetcf-0.4.0/src/pynetcf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:11.376609 pynetcf-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/test_point_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    46614 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tests/test_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-01-31 21:04:03.000000 pynetcf-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.503177 pynetcf-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 08:11:47.000000 pynetcf-0.5.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.495177 pynetcf-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.499177 pynetcf-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 08:11:47.000000 pynetcf-0.5.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 08:11:47.000000 pynetcf-0.5.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 08:11:47.000000 pynetcf-0.5.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 08:11:47.000000 pynetcf-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-08 08:11:47.000000 pynetcf-0.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-08 08:11:47.000000 pynetcf-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-08 08:11:47.000000 pynetcf-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 08:11:47.000000 pynetcf-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-08 08:12:02.503177 pynetcf-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-08 08:11:47.000000 pynetcf-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.499177 pynetcf-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.499177 pynetcf-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 08:11:47.000000 pynetcf-0.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 08:11:47.000000 pynetcf-0.5.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 08:11:47.000000 pynetcf-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 08:12:02.503177 pynetcf-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-08 08:11:47.000000 pynetcf-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.495177 pynetcf-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.499177 pynetcf-0.5.0/src/pynetcf/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-08 08:11:47.000000 pynetcf-0.5.0/src/pynetcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-05-08 08:11:47.000000 pynetcf-0.5.0/src/pynetcf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-05-08 08:11:47.000000 pynetcf-0.5.0/src/pynetcf/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-08 08:11:47.000000 pynetcf-0.5.0/src/pynetcf/point_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59836 2023-05-08 08:11:47.000000 pynetcf-0.5.0/src/pynetcf/time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.499177 pynetcf-0.5.0/src/pynetcf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-08 08:12:02.000000 pynetcf-0.5.0/src/pynetcf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-08 08:12:02.000000 pynetcf-0.5.0/src/pynetcf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:12:02.000000 pynetcf-0.5.0/src/pynetcf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:12:02.000000 pynetcf-0.5.0/src/pynetcf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 08:12:02.000000 pynetcf-0.5.0/src/pynetcf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 08:12:02.000000 pynetcf-0.5.0/src/pynetcf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:12:02.503177 pynetcf-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/test_point_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46614 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tests/test_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-08 08:11:47.000000 pynetcf-0.5.0/tox.ini
```

### Comparing `pynetcf-0.4.0/.coveragerc` & `pynetcf-0.5.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/.github/workflows/ubuntu.yml` & `pynetcf-0.5.0/.github/workflows/ubuntu.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 jobs:
   build:
     name: Build py${{ matrix.python-version }} @ ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8']
+        python-version: ['3.8', '3.9', '3.10']
         os: ["ubuntu-latest"]
 
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: false # does not work with self-hosted testdata
       - name: Checkout Testdata
         shell: bash -l {0}
         run : |
           git submodule init
           git submodule update
-      - uses: conda-incubator/setup-miniconda@v2.0.1
+      - uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: "latest"
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
           environment-file: environment.yml
           activate-environment: pynetcf
           auto-activate-base: false
```

### Comparing `pynetcf-0.4.0/.github/workflows/upload_pypi.yml` & `pynetcf-0.5.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/.github/workflows/windows.yml` & `pynetcf-0.5.0/.github/workflows/windows.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 jobs:
   build:
     name: Build py${{ matrix.python-version }} @ ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8']
+        python-version: ['3.10']
         os: ['windows-latest']
 
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: false # does not work with self-hosted testdata
       - name: Checkout Testdata
         shell: bash -l {0}
         run : |
           git submodule init
           git submodule update
-      - uses: conda-incubator/setup-miniconda@v2.0.1
+      - uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: "latest"
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
           environment-file: environment.yml
           activate-environment: pynetcf
           auto-activate-base: false
```

### Comparing `pynetcf-0.4.0/.gitignore` & `pynetcf-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/CHANGELOG.rst` & `pynetcf-0.5.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 0.5.0
+=============
+
+- Add test for writing strings to netcdf
+- Zlib compress always off for non-numeric data
+
 Version 0.4.0
 =============
 
 - Replace read_ts, write_ts with read, write
 - Replace read_all_ts with read_all
 - Replace write_ts_all_loc with write_all
 - Pep8 fix
```

### Comparing `pynetcf-0.4.0/LICENSE.txt` & `pynetcf-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/PKG-INFO` & `pynetcf-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynetcf
-Version: 0.4.0
+Version: 0.5.0
 Summary: Reading and writing netCDF files according to CF conventions
 Home-page: http://geo.tuwien.ac.at/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Project-URL: Documentation, http://pynetcf.readthedocs.org/
 Platform: any
```

### Comparing `pynetcf-0.4.0/README.rst` & `pynetcf-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/docs/Makefile` & `pynetcf-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/docs/conf.py` & `pynetcf-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/docs/index.rst` & `pynetcf-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/setup.cfg` & `pynetcf-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
-install_requires = importlib-metadata; numpy; scipy; pandas; netCDF4; pygeogrids; pygeobase
+install_requires = importlib-metadata; numpy; pandas; netCDF4; pygeogrids; pygeobase
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `pynetcf-0.4.0/setup.py` & `pynetcf-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/src/pynetcf/__init__.py` & `pynetcf-0.5.0/src/pynetcf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/src/pynetcf/base.py` & `pynetcf-0.5.0/src/pynetcf/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,17 @@
             fill_value = attr.pop("_FillValue")
 
         if dtype is None:
             dtype = data.dtype
 
         if zlib is None:
             zlib = self.zlib
+        if not np.issubdtype(dtype, np.number):
+            # Only numeric data can be compressed
+            zlib = False
         if complevel is None:
             complevel = self.complevel
 
         if name in self.dataset.variables.keys():
             var = self.dataset.variables[name]
         else:
             var = self.dataset.createVariable(name,
```

### Comparing `pynetcf-0.4.0/src/pynetcf/image.py` & `pynetcf-0.5.0/src/pynetcf/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,7 +333,8 @@
         data = {}
         for i, gp in enumerate(gpi):
             row, column = self.grid.gpi2rowcol(gp)
             for var in self.variables:
                 data[var] = self.dataset.variables[var][:, row, column]
 
         return pd.DataFrame(data, index=self.times)
+
```

### Comparing `pynetcf-0.4.0/src/pynetcf/point_data.py` & `pynetcf-0.5.0/src/pynetcf/point_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,18 +351,23 @@
 
                     # check if custom metadata is included
                     if data.dtype.metadata is not None:
                         metadata = data.dtype.metadata
                         if "dims" in metadata and var_data in metadata["dims"]:
                             dimensions = metadata["dims"][var_data]
 
+                    comp = self.compression_info.copy()
+
+                    if not np.issubdtype(dtype, np.number):
+                        comp['zlib'] = False
+
                     self.nc.createVariable(var_data,
                                            dtype,
                                            dimensions=dimensions,
-                                           **self.compression_info)
+                                           **comp)
 
                 self.nc.variables[var_data][idx] = data[var_data]
 
             var_loc_id = self.var["loc_id"]["name"]
             self.nc.variables[var_loc_id][idx] = loc_id
 
             if lon is not None:
```

### Comparing `pynetcf-0.4.0/src/pynetcf/time_series.py` & `pynetcf-0.5.0/src/pynetcf/time_series.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/src/pynetcf.egg-info/PKG-INFO` & `pynetcf-0.5.0/src/pynetcf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynetcf
-Version: 0.4.0
+Version: 0.5.0
 Summary: Reading and writing netCDF files according to CF conventions
 Home-page: http://geo.tuwien.ac.at/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Project-URL: Documentation, http://pynetcf.readthedocs.org/
 Platform: any
```

### Comparing `pynetcf-0.4.0/src/pynetcf.egg-info/SOURCES.txt` & `pynetcf-0.5.0/src/pynetcf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/tests/test_base.py` & `pynetcf-0.5.0/tests/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,35 @@
 
         with ncbase.Dataset(self.testfilename) as self.dataset:
             data = self.dataset.read_var("test")
             nptest.assert_array_equal(
                 data, np.concatenate([np.arange(15),
                                       np.arange(15)]))
 
+    def test_write_append_read_1D_str_w(self):
+        indat = np.array([str(i) for i in np.arange(15)])
+        with ncbase.Dataset(self.testfilename, file_format="NETCDF4",
+                            mode="w", zlib=True) as self.dataset:
+            # create unlimited Dimension
+            self.dataset.create_dim("dim", None)
+            self.dataset.write_var("test", indat, dim=("dim",))
+
+        with ncbase.Dataset(self.testfilename) as self.dataset:
+            data = self.dataset.read_var("test")
+            nptest.assert_array_equal(data, indat)
+
+        with ncbase.Dataset(self.testfilename, mode="a") as self.dataset:
+            self.dataset.append_var("test", np.array(['16']))
+
+        with ncbase.Dataset(self.testfilename) as self.dataset:
+            data = self.dataset.read_var("test")
+            nptest.assert_array_equal(
+                data, np.concatenate([indat, np.array(['16'])])
+            )
+
     def test_write_append_read_1D_autmaskscale_enabled(self):
 
         with ncbase.Dataset(self.testfilename, file_format="NETCDF4",
                             mode="w") as self.dataset:
             # create unlimited Dimension
             self.dataset.create_dim("dim", None)
             self.dataset.write_var("test",
```

### Comparing `pynetcf-0.4.0/tests/test_image.py` & `pynetcf-0.5.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/tests/test_point_data.py` & `pynetcf-0.5.0/tests/test_point_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,29 +51,49 @@
         Delete test file.
         """
         try:
             os.remove(self.fn)
         except OSError:
             pass
 
+    def test_io_str(self):
+        """
+        Write/read test.
+        """
+        loc_ids = np.arange(0, 5)
+        data1 = np.array([str(n) for n in np.arange(5, 10)])
+        data2 = np.arange(10, 15)
+
+        with PointData(self.fn, mode="w", n_obs=5) as nc:
+            for loc_id, d1, d2 in zip(loc_ids, data1, data2):
+                nc.write(loc_id, {"var1": d1, "var2": d2})
+
+        with PointData(self.fn) as nc:
+            nptest.assert_array_equal(
+                nc["var1"], np.array([str(n) for n in range(5, 10)]))
+            assert nc.nc["var1"].filters()["zlib"] is False
+            assert nc.nc["var2"].filters()["zlib"] is True
+            nptest.assert_array_equal(nc["var1"][1], np.array(['6']))
+            nptest.assert_array_equal(nc["var2"][1], np.array([11]))
+
     def test_io(self):
         """
         Write/read test.
         """
         loc_ids = np.arange(0, 5)
         data1 = np.arange(5, 10)
         data2 = np.arange(10, 15)
 
         with PointData(self.fn, mode="w", n_obs=5) as nc:
             for loc_id, d1, d2 in zip(loc_ids, data1, data2):
                 nc.write(loc_id, {"var1": np.array(d1), "var2": np.array(d2)})
 
         with PointData(self.fn) as nc:
             nptest.assert_array_equal(nc["var1"], range(5, 10))
-            assert nc.nc["var1"].filters()["zlib"] == True
+            assert nc.nc["var1"].filters()["zlib"] is True
             nptest.assert_array_equal(nc["var2"][1], np.array([11]))
 
     def test_ioerror(self):
         """
         Should raise IOError if the files does not exist.
         """
         with pytest.raises(IOError):
```

### Comparing `pynetcf-0.4.0/tests/test_profiling.py` & `pynetcf-0.5.0/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/tests/test_time_series.py` & `pynetcf-0.5.0/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `pynetcf-0.4.0/tox.ini` & `pynetcf-0.5.0/tox.ini`

 * *Files identical despite different names*

