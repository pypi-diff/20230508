# Comparing `tmp/hatlib-0.0.8.tar.gz` & `tmp/hatlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatlib-0.0.8.tar", last modified: Tue Mar 29 10:42:34 2022, max compression
+gzip compressed data, was "hatlib-0.0.9.tar", last modified: Thu Mar 31 05:11:05 2022, max compression
```

## Comparing `hatlib-0.0.8.tar` & `hatlib-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.412708 hatlib-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.404708 hatlib-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.408708 hatlib-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-03-29 10:42:07.000000 hatlib-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-03-29 10:42:07.000000 hatlib-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-03-29 10:42:07.000000 hatlib-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-03-29 10:42:07.000000 hatlib-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-03-29 10:42:07.000000 hatlib-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-03-29 10:42:34.412708 hatlib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9325 2022-03-29 10:42:07.000000 hatlib-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-03-29 10:42:07.000000 hatlib-0.0.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-03-29 10:42:07.000000 hatlib-0.0.8/SUPPORT.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.408708 hatlib-0.0.8/hatlib/
--rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/arg_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    10017 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/benchmark_hat_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     5603 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/cuda_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/gpu_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/hat.py
--rw-r--r--   0 runner    (1001) docker     (121)    22569 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/hat_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/hat_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     8160 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/hat_to_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6246 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/hat_to_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/platform_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    28809 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/pyhip_hip.py
--rw-r--r--   0 runner    (1001) docker     (121)     8774 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/pyhip_hiprtc.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/rocm_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.412708 hatlib-0.0.8/hatlib/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/test/test_benchmark_hat_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/test/test_hat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/test/test_hat_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/test/test_hat_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-03-29 10:42:07.000000 hatlib-0.0.8/hatlib/verify_hat_package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.412708 hatlib-0.0.8/hatlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-03-29 10:42:33.000000 hatlib-0.0.8/hatlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-03-29 10:42:34.000000 hatlib-0.0.8/hatlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 10:42:33.000000 hatlib-0.0.8/hatlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-03-29 10:42:34.000000 hatlib-0.0.8/hatlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-03-29 10:42:34.000000 hatlib-0.0.8/hatlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-29 10:42:34.000000 hatlib-0.0.8/hatlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-03-29 10:42:07.000000 hatlib-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.412708 hatlib-0.0.8/samples/
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2022-03-29 10:42:07.000000 hatlib-0.0.8/samples/sample_gemm_library.hat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 10:42:34.412708 hatlib-0.0.8/schema/
--rw-r--r--   0 runner    (1001) docker     (121)    15256 2022-03-29 10:42:07.000000 hatlib-0.0.8/schema/hat.tosd
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-03-29 10:42:34.412708 hatlib-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.828875 hatlib-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.820875 hatlib-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.824875 hatlib-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-03-31 05:10:43.000000 hatlib-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      763 2022-03-31 05:10:43.000000 hatlib-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-03-31 05:10:43.000000 hatlib-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-03-31 05:10:43.000000 hatlib-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-03-31 05:10:43.000000 hatlib-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10241 2022-03-31 05:11:05.828875 hatlib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9325 2022-03-31 05:10:43.000000 hatlib-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-03-31 05:10:43.000000 hatlib-0.0.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-03-31 05:10:43.000000 hatlib-0.0.9/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.824875 hatlib-0.0.9/hatlib/
+-rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/arg_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9917 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/benchmark_hat_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/cuda_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/gpu_headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/hat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21719 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/hat_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/hat_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8897 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/hat_to_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6080 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/hat_to_lib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/platform_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.824875 hatlib-0.0.9/hatlib/pyhip/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/pyhip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28819 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/pyhip/hip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8780 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/pyhip/hiprtc.py
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/rocm_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-03-31 05:10:43.000000 hatlib-0.0.9/hatlib/verify_hat_package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.824875 hatlib-0.0.9/hatlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10241 2022-03-31 05:11:05.000000 hatlib-0.0.9/hatlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-03-31 05:11:05.000000 hatlib-0.0.9/hatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 05:11:05.000000 hatlib-0.0.9/hatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-03-31 05:11:05.000000 hatlib-0.0.9/hatlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-03-31 05:11:05.000000 hatlib-0.0.9/hatlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-31 05:11:05.000000 hatlib-0.0.9/hatlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-03-31 05:10:43.000000 hatlib-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.824875 hatlib-0.0.9/samples/
+-rw-r--r--   0 runner    (1001) docker     (121)     6291 2022-03-31 05:10:43.000000 hatlib-0.0.9/samples/sample_gemm_library.hat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.824875 hatlib-0.0.9/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)    15256 2022-03-31 05:10:43.000000 hatlib-0.0.9/schema/hat.tosd
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-03-31 05:11:05.828875 hatlib-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 05:11:05.828875 hatlib-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-31 05:10:43.000000 hatlib-0.0.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-31 05:10:43.000000 hatlib-0.0.9/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-03-31 05:10:43.000000 hatlib-0.0.9/test/test_benchmark_hat_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-03-31 05:10:43.000000 hatlib-0.0.9/test/test_hat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-03-31 05:10:43.000000 hatlib-0.0.9/test/test_hat_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-03-31 05:10:43.000000 hatlib-0.0.9/test/test_hat_package.py
```

### Comparing `hatlib-0.0.8/.github/workflows/ci.yml` & `hatlib-0.0.9/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         cache: 'pip'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -r hatlib/requirements.txt
     - name: Unittest
       run: |
-        python -m pip install -r hatlib/test/requirements.txt
-        python -m unittest discover hatlib/test
+        python -m pip install -r test/requirements.txt
+        python -m unittest discover test
     - name: Build whl
       run: |
         python -m pip install build
         python -m build
     - name: Install whl
       shell: pwsh
       run: |
```

### Comparing `hatlib-0.0.8/.github/workflows/publish.yml` & `hatlib-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/.gitignore` & `hatlib-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/LICENSE` & `hatlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/PKG-INFO` & `hatlib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: hatlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for HAT (Header Annotated with TOML) packages
+Home-page: https://www.github.com/microsoft/hat
 Author: Microsoft Research AI Compilers Team
 Author-email: mlodev@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

#### html2text {}

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1 Name: hatlib Version: 0.0.8 Summary: Tools for HAT
-(Header Annotated with TOML) packages Author: Microsoft Research AI Compilers
-Team Author-email: mlodev@microsoft.com License: UNKNOWN Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-C++ Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: ~=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE ![HAT](https://upload.wikimedia.org/
-wikipedia/commons/8/80/Crystal_Project_wizard.png) [PyPI_package_version]
-[Python_versions] ![MIT License](https://img.shields.io/pypi/l/hatlib) # HAT
-file format HAT is a format for packaging compiled libraries in the C
-programming language. HAT stands for "**H**eader **A**nnotated with **T**OML",
-and implies that standard C header files are decorated with useful metadata in
-the [TOML](https://toml.io/) markup language. A HAT package includes one
-library file and one or more `.hat` files. The library file can be a static
-library (a `.a` file on Posix systems or a `.lib` file on Windows systems) or a
-dynamic library (a `.so` file on Posix systems or a `.dll` file and its
-accompanying `.lib` import library file on Windows systems). For simplicity of
-documentation, when discussing the "library file" as a unit in a HAT package we
-are referring to either the single static library file (`.a` or `.lib`), the
-single dynamic library file (`.so`) on Posix, or the pair of library files that
-comprise a dynamic library on Windows (`.dll` and `.lib` import library file).
-Note that since a HAT package includes only one "library file" it cannot
-contain both a static and dynamic library, so in the case of a HAT package
-containing a Windows dynamic library, the `.lib` file in the package is always
-the import library and there is no ambiguity in which file (or pair of files)
-is being referenced by "library file". The library file contains all the
-compiled object code that implements the functions in the HAT package. Each
-`.hat` file contains a combination of standard C function declarations (like a
-typical `.h` file) and metadata in the TOML markup language. The metadata that
-accompanies each function declaration describes how the function should be
-called and how it was implemented. The metadata is intended to be both human-
-readable and machine-readable, providing structured and systematic
-documentation and allowing downstream tools to examine the package contents.
-Each `.hat` file has the convenient property that it is simultaneously a valid
-h-file and a valid TOML file. In other words, the file is structured such that
-a C compiler will ignore the TOML metadata, while a TOML parser will understand
-the entire file as a valid TOML file. We accomplish this using a technique we
-call *the hat trick*, which is explained below. # What problem does the HAT
-format solve? C is among the most popular programming languages, but it also
-has serious shortcomings. In particular, C libraries are typically opaque and
-lack mechanisms for systematic documentation and introspection. This is best
+Metadata-Version: 2.1 Name: hatlib Version: 0.0.9 Summary: Tools for HAT
+(Header Annotated with TOML) packages Home-page: https://www.github.com/
+microsoft/hat Author: Microsoft Research AI Compilers Team Author-email:
+mlodev@microsoft.com License: UNKNOWN Platform: UNKNOWN Classifier: License ::
+OSI Approved :: MIT License Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Programming Language :: C++ Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: ~=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE ![HAT](https://upload.wikimedia.org/wikipedia/commons/8/
+80/Crystal_Project_wizard.png) [PyPI_package_version] [Python_versions] ![MIT
+License](https://img.shields.io/pypi/l/hatlib) # HAT file format HAT is a
+format for packaging compiled libraries in the C programming language. HAT
+stands for "**H**eader **A**nnotated with **T**OML", and implies that standard
+C header files are decorated with useful metadata in the [TOML](https://
+toml.io/) markup language. A HAT package includes one library file and one or
+more `.hat` files. The library file can be a static library (a `.a` file on
+Posix systems or a `.lib` file on Windows systems) or a dynamic library (a
+`.so` file on Posix systems or a `.dll` file and its accompanying `.lib` import
+library file on Windows systems). For simplicity of documentation, when
+discussing the "library file" as a unit in a HAT package we are referring to
+either the single static library file (`.a` or `.lib`), the single dynamic
+library file (`.so`) on Posix, or the pair of library files that comprise a
+dynamic library on Windows (`.dll` and `.lib` import library file). Note that
+since a HAT package includes only one "library file" it cannot contain both a
+static and dynamic library, so in the case of a HAT package containing a
+Windows dynamic library, the `.lib` file in the package is always the import
+library and there is no ambiguity in which file (or pair of files) is being
+referenced by "library file". The library file contains all the compiled object
+code that implements the functions in the HAT package. Each `.hat` file
+contains a combination of standard C function declarations (like a typical `.h`
+file) and metadata in the TOML markup language. The metadata that accompanies
+each function declaration describes how the function should be called and how
+it was implemented. The metadata is intended to be both human-readable and
+machine-readable, providing structured and systematic documentation and
+allowing downstream tools to examine the package contents. Each `.hat` file has
+the convenient property that it is simultaneously a valid h-file and a valid
+TOML file. In other words, the file is structured such that a C compiler will
+ignore the TOML metadata, while a TOML parser will understand the entire file
+as a valid TOML file. We accomplish this using a technique we call *the hat
+trick*, which is explained below. # What problem does the HAT format solve? C
+is among the most popular programming languages, but it also has serious
+shortcomings. In particular, C libraries are typically opaque and lack
+mechanisms for systematic documentation and introspection. This is best
 explained with an example: Say that we use C to implement an in-place column-
 wise normalization of a 10x10 matrix. In other words, this function takes a
 10x10 matrix `A` and divides each column by the Euclidean norm of that column.
 A highly-optimized implementation of this function would be tailored to the
 target computer's specific hardware properties, such as its cache size, the
 number of CPU cores, and perhaps even the presence of a GPU. The declaration of
 this function in an h-file would look something like this: ``` void normalize
```

### Comparing `hatlib-0.0.8/README.md` & `hatlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/SECURITY.md` & `hatlib-0.0.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/SUPPORT.md` & `hatlib-0.0.9/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/hatlib/README.md` & `hatlib-0.0.9/hatlib/README.md`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/hatlib/arg_info.py` & `hatlib-0.0.9/hatlib/arg_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import ctypes
 import numpy as np
 import sys
 from dataclasses import dataclass
-from typing import Any, Tuple
-from functools import reduce
-from typing import List
+from typing import Any, List, Tuple
+
+from . import hat_file
 
 
 @dataclass
 class ArgInfo:
     """Extracts necessary information from the description of a function argument in a hat file"""
     hat_declared_type: str
     numpy_shape: Tuple[int]
     numpy_strides: Tuple[int]
     numpy_dtype: type
     element_num_bytes: int
     ctypes_pointer_type: Any
-    usage: str = ""
+    usage: hat_file.UsageType = None
 
-    def __init__(self, param_description):
-        self.hat_declared_type = param_description["declared_type"]
-        self.numpy_shape = tuple(param_description["shape"])
-        self.usage = param_description["usage"]
+    def __init__(self, param_description: hat_file.Parameter):
+        self.hat_declared_type = param_description.declared_type
+        self.numpy_shape = tuple(param_description.shape)
+        self.usage = param_description.usage
         if self.hat_declared_type == "float16_t*":
             self.numpy_dtype = np.float16
             self.element_num_bytes = 2
-            self.ctypes_pointer_type = ctypes.POINTER(
-                ctypes.c_uint16)  # same bitwidth as float16
+            self.ctypes_pointer_type = ctypes.POINTER(ctypes.c_uint16)    # same bitwidth as float16
         elif self.hat_declared_type == "float*":
             self.numpy_dtype = np.float32
             self.element_num_bytes = 4
             self.ctypes_pointer_type = ctypes.POINTER(ctypes.c_float)
         elif self.hat_declared_type == "double*":
             self.numpy_dtype = np.float64
             self.element_num_bytes = 8
@@ -49,31 +48,26 @@
             self.ctypes_pointer_type = ctypes.POINTER(ctypes.c_int16)
         elif self.hat_declared_type == "int8_t*":
             self.numpy_dtype = np.int8
             self.element_num_bytes = 1
             self.ctypes_pointer_type = ctypes.POINTER(ctypes.c_int8)
 
         else:
-            raise NotImplementedError(
-                f"Unsupported declared_type {self.hat_declared_type} in hat file"
-            )
+            raise NotImplementedError(f"Unsupported declared_type {self.hat_declared_type} in hat file")
 
-        self.numpy_strides = tuple([
-            self.element_num_bytes * x for x in param_description["affine_map"]
-        ])
+        self.numpy_strides = tuple([self.element_num_bytes * x for x in param_description.affine_map])
 
 
-def verify_args(args, arg_infos, function_name):
+# TODO: Update this to take a HATFunction instead, instead of arg_infos and function_name
+def verify_args(args: List, arg_infos: List[ArgInfo], function_name: str):
     """ Verifies that a list of arguments matches a list of argument descriptions in a HAT file
     """
     # check number of args
     if len(args) != len(arg_infos):
-        sys.exit(
-            f"Error calling {function_name}(...): expected {len(arg_infos)} arguments but received {len(args)}"
-        )
+        sys.exit(f"Error calling {function_name}(...): expected {len(arg_infos)} arguments but received {len(args)}")
 
     # for each arg
     for i in range(len(args)):
         arg = args[i]
         arg_info = arg_infos[i]
 
         # confirm that the arg is a numpy ndarray
@@ -95,28 +89,7 @@
             )
 
         # confirm that the arg strides are correct
         if arg_info.numpy_strides != arg.strides:
             sys.exit(
                 f"Error calling {function_name}(...): expected argument {i} to have strides={arg_info.numpy_strides} but received strides={arg.strides}"
             )
-
-
-def generate_input_sets(parameters: List[ArgInfo],
-                        input_sets_minimum_size_MB: int = 0,
-                        num_additional: int = 0):
-    shapes_to_sizes = [
-        reduce(lambda x, y: x * y, p.numpy_shape) for p in parameters
-    ]
-    set_size = reduce(lambda x, y: x + y, [
-        size * p.element_num_bytes
-        for size, p in zip(shapes_to_sizes, parameters)
-    ])
-
-    num_input_sets = (input_sets_minimum_size_MB * 1024 * 1024 //
-                      set_size) + 1 + num_additional
-    input_sets = [[
-        np.random.random(p.numpy_shape).astype(p.numpy_dtype)
-        for p in parameters
-    ] for _ in range(num_input_sets)]
-
-    return input_sets[0] if len(input_sets) == 1 else input_sets
```

### Comparing `hatlib-0.0.8/hatlib/benchmark_hat_package.py` & `hatlib-0.0.9/hatlib/benchmark_hat_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,32 @@
 import pandas as pd
 import sys
 import time
 import toml
 import traceback
 from pathlib import Path
 
-if __package__:
-    from .hat_file import HATFile
-    from .hat_to_dynamic import create_dynamic_package
-    from .hat import load, ArgInfo, generate_input_sets
-else:
-    from hat_file import HATFile
-    from hat_to_dynamic import create_dynamic_package
-    from hat import load, ArgInfo, generate_input_sets
+from .hat_file import HATFile
+from .hat import load, generate_input_sets_for_func
 
 
 class Benchmark:
     """A basic python-based benchmark.
     Useful for comparison only, due to overhead in the Python layer.
 
     Requirements:
         A compilation toolchain in your PATH: cl.exe & link.exe (Windows), gcc (Linux), or clang (macOS)
     """
-
-    def __init__(self, hat_path):
-        self.hat_path = Path(hat_path)
-
-        self.hat_package = load(self.hat_path)
-        self.hat_functions = self.hat_package.names
+    def __init__(self, hat_path: str):
+        self.hat_path = hat_path
+        self.hat_package, self.func_dict = load(self.hat_path)
+        self.hat_functions = self.func_dict.names
 
         # create dictionary of function descriptions defined in the hat file
-        t = toml.load(self.hat_path)
-        function_descriptions = t["functions"]
-        self.hat_arg_descriptions = {key: [ArgInfo(
-            d) for d in val["arguments"]] for key, val in function_descriptions.items()}
+        self.function_descriptions = self.hat_package.hat_file.function_map
 
     def run(self,
             function_name: str,
             warmup_iterations: int = 10,
             min_timing_iterations: int = 100,
             min_time_in_sec: int = 10,
             input_sets_minimum_size_MB=50) -> float:
@@ -54,72 +43,77 @@
             min_timing_iterations: minimum number of timing iterations
             min_time_in_sec: minimum amount of time to run the benchmark
             input_sets_minimum_size_MB: generate enough input sets to exceed this size to avoid cache hits
         Returns:
             Mean duration in seconds,
             Vector of timings in seconds for each batch that was run
         """
-        if function_name not in self.hat_package.names:
+        if function_name not in self.hat_functions:
             raise ValueError(f"{function_name} is not found")
 
         # TODO: support packing and unpacking functions
 
         mean_elapsed_time, batch_timings = self._profile(
-            function_name, warmup_iterations, min_timing_iterations, min_time_in_sec, input_sets_minimum_size_MB)
+            function_name, warmup_iterations, min_timing_iterations,
+            min_time_in_sec, input_sets_minimum_size_MB)
         print(
-            f"[Benchmarking] Mean duration per iteration: {mean_elapsed_time:.8f}s")
+            f"[Benchmarking] Mean duration per iteration: {mean_elapsed_time:.8f}s"
+        )
 
         return mean_elapsed_time, batch_timings
 
-    def _profile(self, function_name, warmup_iterations, min_timing_iterations, min_time_in_sec, input_sets_minimum_size_MB):
-
+    def _profile(self, function_name, warmup_iterations, min_timing_iterations,
+                 min_time_in_sec, input_sets_minimum_size_MB):
         def get_perf_counter():
             if hasattr(time, 'perf_counter_ns'):
                 perf_counter = time.perf_counter_ns
                 perf_counter_scale = 1000000000
             else:
                 perf_counter = time.perf_counter
                 perf_counter_scale = 1
             return perf_counter, perf_counter_scale
 
-        parameters = self.hat_arg_descriptions[function_name]
+        func = self.function_descriptions[function_name]
 
         # generate sufficient input sets to overflow the L3 cache, since we don't know the size of the model
         # we'll make a guess based on the minimum input set size
-        input_sets = generate_input_sets(
-            parameters, input_sets_minimum_size_MB, num_additional=10)
+        input_sets = generate_input_sets_for_func(func,
+                                                  input_sets_minimum_size_MB,
+                                                  num_additional=10)
 
         set_size = 0
         for i in input_sets[0]:
             set_size += i.size * i.dtype.itemsize
 
         print(
-            f"[Benchmarking] Using {len(input_sets)} input sets, each {set_size} bytes")
+            f"[Benchmarking] Using {len(input_sets)} input sets, each {set_size} bytes"
+        )
 
         perf_counter, perf_counter_scale = get_perf_counter()
         print(
             f"[Benchmarking] Warming up for {warmup_iterations} iterations...")
 
         for _ in range(warmup_iterations):
             for calling_args in input_sets:
-                self.hat_package[function_name](*calling_args)
+                self.func_dict[function_name](*calling_args)
 
         print(
-            f"[Benchmarking] Timing for at least {min_time_in_sec}s and at least {min_timing_iterations} iterations...")
+            f"[Benchmarking] Timing for at least {min_time_in_sec}s and at least {min_timing_iterations} iterations..."
+        )
         start_time = perf_counter()
         end_time = perf_counter()
 
         i = 0
         i_max = len(input_sets)
         iterations = 1
         batch_timings = []
         while ((end_time - start_time) / perf_counter_scale) < min_time_in_sec:
             batch_start_time = perf_counter()
             for _ in range(min_timing_iterations):
-                self.hat_package[function_name](*input_sets[i])
+                self.func_dict[function_name](*input_sets[i])
                 i = iterations % i_max
                 iterations += 1
             end_time = perf_counter()
             batch_timings.append(
                 (end_time - batch_start_time) / perf_counter_scale)
 
         elapsed_time = ((end_time - start_time) / perf_counter_scale)
@@ -136,96 +130,121 @@
     hat_func.auxiliary["mean_duration_in_sec"] = mean_time_secs
 
     hat_file.Serialize(hat_path)
 
     # Workaround to remove extra empty lines
     with open(hat_path, "r") as f:
         lines = f.readlines()
-        lines = [lines[i] for i in range(len(lines)) if not(lines[i] == "\n"
-                                                            and i < len(lines)-1 and lines[i+1] == "\n")]
+        lines = [
+            lines[i] for i in range(len(lines))
+            if not (lines[i] == "\n" and i < len(lines) -
+                    1 and lines[i + 1] == "\n")
+        ]
     with open(hat_path, "w") as f:
         f.writelines(lines)
 
 
-def run_benchmark(hat_path, store_in_hat=False, batch_size=10, min_time_in_sec=10, input_sets_minimum_size_MB=50):
+def run_benchmark(hat_path,
+                  store_in_hat=False,
+                  batch_size=10,
+                  min_time_in_sec=10,
+                  input_sets_minimum_size_MB=50):
     results = []
 
     benchmark = Benchmark(hat_path)
     functions = benchmark.hat_functions
     for function_name in functions:
         print(f"\nBenchmarking function: {function_name}")
         if "Initialize" in function_name or "_debug_check_allclose" in function_name:  # Skip init and debug functions
             continue
 
         try:
-            _, batch_timings = benchmark.run(function_name,
-                                             warmup_iterations=batch_size,
-                                             min_timing_iterations=batch_size,
-                                             min_time_in_sec=min_time_in_sec,
-                                             input_sets_minimum_size_MB=input_sets_minimum_size_MB)
+            _, batch_timings = benchmark.run(
+                function_name,
+                warmup_iterations=batch_size,
+                min_timing_iterations=batch_size,
+                min_time_in_sec=min_time_in_sec,
+                input_sets_minimum_size_MB=input_sets_minimum_size_MB)
 
             sorted_batch_means = np.array(sorted(batch_timings)) / batch_size
             num_batches = len(batch_timings)
 
             mean_of_means = sorted_batch_means.mean()
-            median_of_means = sorted_batch_means[num_batches//2]
-            mean_of_small_means = sorted_batch_means[0: num_batches//2].mean()
-            robust_mean_of_means = sorted_batch_means[num_batches //
-                                                      5: -num_batches//5].mean()
+            median_of_means = sorted_batch_means[num_batches // 2]
+            mean_of_small_means = sorted_batch_means[0:num_batches // 2].mean()
+            robust_means = sorted_batch_means[(num_batches //
+                                               5):(-num_batches // 5)]
+            robust_mean_of_means = robust_means.mean()
             min_of_means = sorted_batch_means[0]
 
             if store_in_hat:
-                write_runtime_to_hat_file(
-                    hat_path, function_name, mean_of_means)
-            results.append({"function_name": function_name,
-                            "mean": mean_of_means,
-                            "median_of_means": median_of_means,
-                            "mean_of_small_means": mean_of_small_means,
-                            "robust_mean": robust_mean_of_means,
-                            "min_of_means": min_of_means,
-                            })
+                write_runtime_to_hat_file(hat_path, function_name,
+                                          mean_of_means)
+            results.append({
+                "function_name": function_name,
+                "mean": mean_of_means,
+                "median_of_means": median_of_means,
+                "mean_of_small_means": mean_of_small_means,
+                "robust_mean": robust_mean_of_means,
+                "min_of_means": min_of_means,
+            })
         except Exception as e:
             exc_type, exc_val, exc_tb = sys.exc_info()
-            traceback.print_exception(
-                exc_type, exc_val, exc_tb, file=sys.stderr)
+            traceback.print_exception(exc_type,
+                                      exc_val,
+                                      exc_tb,
+                                      file=sys.stderr)
             print("\nException message: ", e)
             print(
-                f"WARNING: Failed to run function {function_name}, skipping this benchmark.")
+                f"WARNING: Failed to run function {function_name}, skipping this benchmark."
+            )
     return results
 
 
 def main(argv):
     arg_parser = argparse.ArgumentParser(
-        description="Benchmarks each function in a HAT package and estimates its duration.\n"
+        description=
+        "Benchmarks each function in a HAT package and estimates its duration.\n"
         "Example:\n"
         "    hatlib.benchmark_hat_package <hat_path>\n")
 
     arg_parser.add_argument("hat_path",
                             help="Path to the HAT file",
                             default=None)
-    arg_parser.add_argument("--store_in_hat",
-                            help="If set, will write the duration as meta-data back into the hat file",
-                            action='store_true')
+    arg_parser.add_argument(
+        "--store_in_hat",
+        help=
+        "If set, will write the duration as meta-data back into the hat file",
+        action='store_true')
     arg_parser.add_argument("--results_file",
                             help="Full path where the results will be written",
                             default="results.csv")
-    arg_parser.add_argument("--batch_size",
-                            help="The number of function calls in each batch (at least one full batch is executed)",
-                            default=10)
-    arg_parser.add_argument("--min_time_in_sec",
-                            help="Minimum number of seconds to run the benchmark for",
-                            default=30)
-    arg_parser.add_argument("--input_sets_minimum_size_MB",
-                            help="Minimum size in MB of the input sets. Typically this is large enough to ensure eviction of the biggest cache on the target (e.g. L3 on an desktop CPU)",
-                            default=50)
+    arg_parser.add_argument(
+        "--batch_size",
+        help=
+        "The number of function calls in each batch (at least one full batch is executed)",
+        default=10)
+    arg_parser.add_argument(
+        "--min_time_in_sec",
+        help="Minimum number of seconds to run the benchmark for",
+        default=30)
+    arg_parser.add_argument(
+        "--input_sets_minimum_size_MB",
+        help=
+        "Minimum size in MB of the input sets. Typically this is large enough to ensure eviction of the biggest cache on the target (e.g. L3 on an desktop CPU)",
+        default=50)
 
     args = vars(arg_parser.parse_args(argv))
 
-    results = run_benchmark(args["hat_path"], args["store_in_hat"], batch_size=int(args["batch_size"]), min_time_in_sec=int(
-        args["min_time_in_sec"]), input_sets_minimum_size_MB=int(args["input_sets_minimum_size_MB"]))
+    results = run_benchmark(args["hat_path"],
+                            args["store_in_hat"],
+                            batch_size=int(args["batch_size"]),
+                            min_time_in_sec=int(args["min_time_in_sec"]),
+                            input_sets_minimum_size_MB=int(
+                                args["input_sets_minimum_size_MB"]))
     df = pd.DataFrame(results)
     df.to_csv(args["results_file"], index=False)
     pd.options.display.float_format = '{:8.8f}'.format
     print(df)
 
     print(f"Results saved to {args['results_file']}")
```

### Comparing `hatlib-0.0.8/hatlib/cuda_loader.py` & `hatlib-0.0.9/hatlib/cuda_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 from typing import List
 
 # CUDA stuff
 # TODO: move from pvnrtc module to cuda entirely to reduce dependencies
 from pynvrtc.compiler import Program
 from cuda import cuda, nvrtc
 
-try:
-    from .arg_info import ArgInfo, verify_args
-    from .gpu_headers import CUDA_HEADER_MAP
-except:
-    from arg_info import ArgInfo, verify_args
-    from gpu_headers import CUDA_HEADER_MAP
+from .arg_info import ArgInfo, verify_args
+from .gpu_headers import CUDA_HEADER_MAP
+from .hat_file import Function
 
 
 def ASSERT_DRV(err):
     if isinstance(err, cuda.CUresult):
         if err != cuda.CUresult.CUDA_SUCCESS:
-            raise RuntimeError("Cuda Error: {}".format(
-                cuda.cuGetErrorString(err)[1].decode('utf-8')))
+            raise RuntimeError("Cuda Error: {}".format(cuda.cuGetErrorString(err)[1].decode('utf-8')))
     elif isinstance(err, nvrtc.nvrtcResult):
         if err != nvrtc.nvrtcResult.NVRTC_SUCCESS:
             raise RuntimeError("Nvrtc Error: {}".format(err))
     else:
         raise RuntimeError("Unknown error type: {}".format(err))
 
 
@@ -47,23 +43,20 @@
 
     return cuda_path
 
 
 def compile_cuda_program(cuda_src_path: pathlib.Path, func_name):
     src = cuda_src_path.read_text()
 
-    prog = Program(src=src,
-                   name=func_name,
-                   headers=CUDA_HEADER_MAP.values(),
-                   include_names=CUDA_HEADER_MAP.keys())
+    prog = Program(src=src, name=func_name, headers=CUDA_HEADER_MAP.values(), include_names=CUDA_HEADER_MAP.keys())
     ptx = prog.compile([
         '-use_fast_math',
         '-default-device',
         '-std=c++11',
-        '-arch=sm_52',  # TODO: is this needed?
+        '-arch=sm_52',    # TODO: is this needed?
     ])
 
     return ptx
 
 
 def initialize_cuda():
     # Initialize CUDA Driver API
@@ -87,35 +80,28 @@
     err, kernel = cuda.cuModuleGetFunction(ptx_mod, func_name.encode('utf-8'))
     ASSERT_DRV(err)
 
     return kernel
 
 
 def _arg_size(arg_info: ArgInfo):
-    return arg_info.element_num_bytes * reduce(lambda x, y: x * y,
-                                               arg_info.numpy_shape)
+    return arg_info.element_num_bytes * reduce(lambda x, y: x * y, arg_info.numpy_shape)
 
 
-def transfer_mem_host_to_cuda(device_args: List, host_args: List[np.array],
-                              arg_infos: List[ArgInfo]):
-    for device_arg, host_arg, arg_info in zip(device_args, host_args,
-                                              arg_infos):
-        if 'input' in arg_info.usage:
-            err, = cuda.cuMemcpyHtoD(device_arg, host_arg.ctypes.data,
-                                     _arg_size(arg_info))
+def transfer_mem_host_to_cuda(device_args: List, host_args: List[np.array], arg_infos: List[ArgInfo]):
+    for device_arg, host_arg, arg_info in zip(device_args, host_args, arg_infos):
+        if 'input' in arg_info.usage.value:
+            err, = cuda.cuMemcpyHtoD(device_arg, host_arg.ctypes.data, _arg_size(arg_info))
             ASSERT_DRV(err)
 
 
-def transfer_mem_cuda_to_host(device_args: List, host_args: List[np.array],
-                              arg_infos: List[ArgInfo]):
-    for device_arg, host_arg, arg_info in zip(device_args, host_args,
-                                              arg_infos):
-        if 'output' in arg_info.usage:
-            err, = cuda.cuMemcpyDtoH(host_arg.ctypes.data, device_arg,
-                                     _arg_size(arg_info))
+def transfer_mem_cuda_to_host(device_args: List, host_args: List[np.array], arg_infos: List[ArgInfo]):
+    for device_arg, host_arg, arg_info in zip(device_args, host_args, arg_infos):
+        if 'output' in arg_info.usage.value:
+            err, = cuda.cuMemcpyDtoH(host_arg.ctypes.data, device_arg, _arg_size(arg_info))
             ASSERT_DRV(err)
 
 
 def allocate_cuda_mem(arg_infos: List[ArgInfo]):
     device_mem = []
     for arg in arg_infos:
         err, mem = cuda.cuMemAlloc(_arg_size(arg))
@@ -129,50 +115,48 @@
     # CUDA python example says this is subject to change
     ptrs = [np.array([int(d_arg)], dtype=np.uint64) for d_arg in device_args]
     ptrs = np.array([ptr.ctypes.data for ptr in ptrs], dtype=np.uint64)
 
     return ptrs
 
 
-def create_loader_for_device_function(device_func, hat_details):
-    hat_path: pathlib.Path = hat_details.path
-    cuda_src_path: pathlib.Path = hat_path.parent / device_func["provider"]
-    func_name = device_func["name"]
+def create_loader_for_device_function(device_func: Function, hat_dir_path: str):
+    if not device_func.provider:
+        raise RuntimeError("Expected a provider for the device function")
+
+    cuda_src_path: pathlib.Path = pathlib.Path(hat_dir_path) / device_func.provider
+    func_name = device_func.name
 
     ptx = compile_cuda_program(cuda_src_path, func_name)
 
     initialize_cuda()
 
     kernel = get_func_from_ptx(ptx, func_name)
 
-    hat_arg_descriptions = device_func["arguments"]
+    hat_arg_descriptions = device_func.arguments
     arg_infos = [ArgInfo(d) for d in hat_arg_descriptions]
-    launch_parameters = device_func["launch_parameters"]
+    launch_parameters = device_func.launch_parameters
 
     def f(*args):
         verify_args(args, arg_infos, func_name)
         device_mem = allocate_cuda_mem(arg_infos)
-        transfer_mem_host_to_cuda(device_args=device_mem,
-                                  host_args=args,
-                                  arg_infos=arg_infos)
+        transfer_mem_host_to_cuda(device_args=device_mem, host_args=args, arg_infos=arg_infos)
         ptrs = device_args_to_ptr_list(device_mem)
 
         err, stream = cuda.cuStreamCreate(0)
         ASSERT_DRV(err)
 
         err, = cuda.cuLaunchKernel(
             kernel,
-            *launch_parameters,  # [ grid[x-z], block[x-z] ]
-            0,  # dynamic shared memory
-            stream,  # stream
-            ptrs.ctypes.data,  # kernel arguments
-            0,  # extra (ignore)
+            *launch_parameters,    # [ grid[x-z], block[x-z] ]
+            0,    # dynamic shared memory
+            stream,    # stream
+            ptrs.ctypes.data,    # kernel arguments
+            0,    # extra (ignore)
         )
         ASSERT_DRV(err)
         err, = cuda.cuStreamSynchronize(stream)
         ASSERT_DRV(err)
 
-        transfer_mem_cuda_to_host(device_args=device_mem,
-                                  host_args=args,
-                                  arg_infos=arg_infos)
+        transfer_mem_cuda_to_host(device_args=device_mem, host_args=args, arg_infos=arg_infos)
 
     return f
```

### Comparing `hatlib-0.0.8/hatlib/gpu_headers.py` & `hatlib-0.0.9/hatlib/gpu_headers.py`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/hatlib/hat_file.py` & `hatlib-0.0.9/hatlib/hat_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 # Utility to parse the TOML metadata from HAT files
-from enum import Enum
-from dataclasses import dataclass, field
 import os
-from pathlib import Path
-
 import tomlkit
+from dataclasses import dataclass, field
+from enum import Enum
+from pathlib import Path
+from typing import Dict, List
 
 # TODO : type-checking on leaf node values
 
 
 def _read_toml_file(filepath):
     path = os.path.abspath(filepath)
     toml_doc = None
@@ -101,15 +101,16 @@
 
     @staticmethod
     def parse_from_table(table):
         return Description(
             author=table["author"],
             version=table["version"],
             license_url=table["license_url"],
-            auxiliary=AuxiliarySupportedTable.parse_auxiliary(table))
+            auxiliary=AuxiliarySupportedTable.parse_auxiliary(table)
+        )
 
 
 @dataclass
 class Parameter:
     # All parameter keys
     name: str = ""
     description: str = ""
@@ -143,57 +144,52 @@
             table.append("size", self.size)
 
         return table
 
     # TODO : change "usage" to "role" in schema
     @staticmethod
     def parse_from_table(param_table):
-        required_table_entries = [
-            "name", "description", "logical_type", "declared_type",
-            "element_type", "usage"
-        ]
+        required_table_entries = ["name", "description", "logical_type", "declared_type", "element_type", "usage"]
         _check_required_table_entries(param_table, required_table_entries)
-        affine_array_required_table_entries = [
-            "shape", "affine_map", "affine_offset"
-        ]
+        affine_array_required_table_entries = ["shape", "affine_map", "affine_offset"]
         runtime_array_required_table_entries = ["size"]
 
         name = param_table["name"]
         description = param_table["description"]
         logical_type = ParameterType(param_table["logical_type"])
         declared_type = param_table["declared_type"]
         element_type = param_table["element_type"]
         usage = UsageType(param_table["usage"])
 
-        param = Parameter(name=name,
-                          description=description,
-                          logical_type=logical_type,
-                          declared_type=declared_type,
-                          element_type=element_type,
-                          usage=usage)
+        param = Parameter(
+            name=name,
+            description=description,
+            logical_type=logical_type,
+            declared_type=declared_type,
+            element_type=element_type,
+            usage=usage
+        )
 
         if logical_type == ParameterType.AffineArray:
-            _check_required_table_entries(param_table,
-                                          affine_array_required_table_entries)
+            _check_required_table_entries(param_table, affine_array_required_table_entries)
             param.shape = param_table["shape"]
             param.affine_map = param_table["affine_map"]
             param.affine_offset = param_table["affine_offset"]
 
         elif logical_type == ParameterType.RuntimeArray:
-            _check_required_table_entries(
-                param_table, runtime_array_required_table_entries)
+            _check_required_table_entries(param_table, runtime_array_required_table_entries)
             param.size = param_table["size"]
 
         return param
 
 
 @dataclass
 class Function(AuxiliarySupportedTable):
     # required
-    arguments: list = field(default_factory=list)
+    arguments: List[Parameter] = field(default_factory=list)
     calling_convention: CallingConventionType = None
     description: str = ""
     hat_file: any = None
     link_target: Path = None
     name: str = ""
     return_info: Parameter = None
 
@@ -210,15 +206,15 @@
         table.add("calling_convention", self.calling_convention.value)
         arg_tables = [arg.to_table() for arg in self.arguments]
         arg_array = tomlkit.array()
         for arg_table in arg_tables:
             arg_array.append(arg_table)
         table.add(
             "arguments", arg_array
-        )  # TODO : figure out why this isn't indenting after serialization in some cases
+        )    # TODO : figure out why this isn't indenting after serialization in some cases
 
         if self.launch_parameters:
             table.add("launch_parameters", self.launch_parameters)
 
         if self.launches:
             table.add("launches", self.launches)
 
@@ -232,68 +228,58 @@
 
         self.add_auxiliary_table(table)
 
         return table
 
     @staticmethod
     def parse_from_table(function_table):
-        required_table_entries = [
-            "name", "description", "calling_convention", "arguments", "return"
-        ]
+        required_table_entries = ["name", "description", "calling_convention", "arguments", "return"]
         _check_required_table_entries(function_table, required_table_entries)
-        arguments = [
-            Parameter.parse_from_table(param_table)
-            for param_table in function_table["arguments"]
-        ]
+        arguments = [Parameter.parse_from_table(param_table) for param_table in function_table["arguments"]]
 
-        launch_parameters = function_table[
-            "launch_parameters"] if "launch_parameters" in function_table else []
+        launch_parameters = function_table["launch_parameters"] if "launch_parameters" in function_table else []
 
-        launches = function_table[
-            "launches"] if "launches" in function_table else ""
+        launches = function_table["launches"] if "launches" in function_table else ""
 
-        provider = function_table[
-            "provider"] if "provider" in function_table else ""
+        provider = function_table["provider"] if "provider" in function_table else ""
 
-        runtime = function_table[
-            "runtime"] if "runtime" in function_table else ""
+        runtime = function_table["runtime"] if "runtime" in function_table else ""
 
         return_info = Parameter.parse_from_table(function_table["return"])
 
         return Function(
             name=function_table["name"],
             description=function_table["description"],
-            calling_convention=CallingConventionType(
-                function_table["calling_convention"]),
+            calling_convention=CallingConventionType(function_table["calling_convention"]),
             arguments=arguments,
             return_info=return_info,
             launch_parameters=launch_parameters,
             launches=launches,
             provider=provider,
             runtime=runtime,
-            auxiliary=AuxiliarySupportedTable.parse_auxiliary(function_table))
+            auxiliary=AuxiliarySupportedTable.parse_auxiliary(function_table)
+        )
 
 
 class FunctionTableCommon:
+
     def __init__(self, function_map):
         self.function_map = function_map
         self.functions = self.function_map.values()
 
     def to_table(self):
         func_table = tomlkit.table()
         for function_key in self.function_map:
-            func_table.add(function_key,
-                           self.function_map[function_key].to_table())
+            func_table.add(function_key, self.function_map[function_key].to_table())
         return func_table
 
     @classmethod
     def parse_from_table(cls, all_functions_table):
         function_map = {
-            function_key:
-            Function.parse_from_table(all_functions_table[function_key])
+            function_key: Function.parse_from_table(all_functions_table[function_key])
             for function_key in all_functions_table
         }
         return cls(function_map)
 
 
 class FunctionTable(FunctionTableCommon):
     TableName = "functions"
@@ -301,16 +287,18 @@
 
 class DeviceFunctionTable(FunctionTableCommon):
     TableName = "device_functions"
 
 
 @dataclass
 class Target:
+
     @dataclass
     class Required:
+
         @dataclass
         class CPU:
             TableName = TargetType.CPU.value
 
             # required
             architecture: str = ""
             extensions: list = field(default_factory=list)
@@ -332,17 +320,16 @@
             def parse_from_table(table):
                 required_table_entries = ["architecture", "extensions"]
                 _check_required_table_entries(table, required_table_entries)
 
                 runtime = table.get("runtime", "")
 
                 return Target.Required.CPU(
-                    architecture=table["architecture"],
-                    extensions=table["extensions"],
-                    runtime=runtime)
+                    architecture=table["architecture"], extensions=table["extensions"], runtime=runtime
+                )
 
         @dataclass
         class GPU:
             TableName = TargetType.GPU.value
             blocks: int = 0
             instruction_set_version: str = ""
             min_threads: int = 0
@@ -353,16 +340,15 @@
             runtime: str = ""
 
             def to_table(self):
                 table = tomlkit.table()
                 table.add("model", self.model)
                 table.add("runtime", self.runtime)
                 table.add("blocks", self.blocks)
-                table.add("instruction_set_version",
-                          self.instruction_set_version)
+                table.add("instruction_set_version", self.instruction_set_version)
                 table.add("min_threads", self.min_threads)
                 table.add("min_global_memory_KB", self.min_global_memory_KB)
                 table.add("min_shared_memory_KB", self.min_shared_memory_KB)
                 table.add("min_texture_memory_KB", self.min_texture_memory_KB)
 
                 return table
 
@@ -378,15 +364,16 @@
                     runtime=table["runtime"],
                     model=table["model"],
                     blocks=table["blocks"],
                     instruction_set_version=table["instruction_set_version"],
                     min_threads=table["min_threads"],
                     min_global_memory_KB=table["min_global_memory_KB"],
                     min_shared_memory_KB=table["min_shared_memory_KB"],
-                    min_texture_memory_KB=table["min_texture_memory_KB"])
+                    min_texture_memory_KB=table["min_texture_memory_KB"]
+                )
 
         TableName = "required"
         os: OperatingSystem = None
         cpu: CPU = None
         gpu: GPU = None
 
         def to_table(self):
@@ -397,19 +384,17 @@
                 table.add(Target.Required.GPU.TableName, self.gpu.to_table())
             return table
 
         @staticmethod
         def parse_from_table(table):
             required_table_entries = ["os", Target.Required.CPU.TableName]
             _check_required_table_entries(table, required_table_entries)
-            cpu_info = Target.Required.CPU.parse_from_table(
-                table[Target.Required.CPU.TableName])
+            cpu_info = Target.Required.CPU.parse_from_table(table[Target.Required.CPU.TableName])
             if Target.Required.GPU.TableName in table:
-                gpu_info = Target.Required.GPU.parse_from_table(
-                    table[Target.Required.GPU.TableName])
+                gpu_info = Target.Required.GPU.parse_from_table(table[Target.Required.GPU.TableName])
             else:
                 gpu_info = Target.Required.GPU()
             return Target.Required(os=table["os"], cpu=cpu_info, gpu=gpu_info)
 
     # TODO : support optimized_for table
     class OptimizedFor:
         TableName = "optimized_for"
@@ -425,27 +410,24 @@
     required: Required = None
     optimized_for: OptimizedFor = None
 
     def to_table(self):
         table = tomlkit.table()
         table.add(Target.Required.TableName, self.required.to_table())
         if self.optimized_for is not None:
-            table.add(Target.OptimizedFor.TableName,
-                      self.optimized_for.to_table())
+            table.add(Target.OptimizedFor.TableName, self.optimized_for.to_table())
         return table
 
     @staticmethod
     def parse_from_table(target_table):
         required_table_entries = [Target.Required.TableName]
         _check_required_table_entries(target_table, required_table_entries)
-        required_data = Target.Required.parse_from_table(
-            target_table[Target.Required.TableName])
+        required_data = Target.Required.parse_from_table(target_table[Target.Required.TableName])
         if Target.OptimizedFor.TableName in target_table:
-            optimized_for_data = Target.OptimizedFor.parse_from_table(
-                target_table[Target.OptimizedFor.TableName])
+            optimized_for_data = Target.OptimizedFor.parse_from_table(target_table[Target.OptimizedFor.TableName])
         else:
             optimized_for_data = Target.OptimizedFor()
         return Target(required=required_data, optimized_for=optimized_for_data)
 
 
 @dataclass
 class LibraryReference:
@@ -458,17 +440,15 @@
         table.append("name", self.name)
         table.append("version", self.version)
         table.append("target_file", self.target_file)
         return table
 
     @staticmethod
     def parse_from_table(table):
-        return LibraryReference(name=table["name"],
-                                version=table["version"],
-                                target_file=table["target_file"])
+        return LibraryReference(name=table["name"], version=table["version"], target_file=table["target_file"])
 
 
 @dataclass
 class Dependencies(AuxiliarySupportedTable):
     TableName = "dependencies"
     link_target: str = ""
     deploy_files: list = field(default_factory=list)
@@ -486,25 +466,22 @@
 
         self.add_auxiliary_table(table)
         return table
 
     @staticmethod
     def parse_from_table(dependencies_table):
         required_table_entries = ["link_target", "deploy_files", "dynamic"]
-        _check_required_table_entries(dependencies_table,
-                                      required_table_entries)
-        dynamic = [
-            LibraryReference.parse_from_table(lib_ref_table)
-            for lib_ref_table in dependencies_table["dynamic"]
-        ]
-        return Dependencies(link_target=dependencies_table["link_target"],
-                            deploy_files=dependencies_table["deploy_files"],
-                            dynamic=dynamic,
-                            auxiliary=AuxiliarySupportedTable.parse_auxiliary(
-                                dependencies_table))
+        _check_required_table_entries(dependencies_table, required_table_entries)
+        dynamic = [LibraryReference.parse_from_table(lib_ref_table) for lib_ref_table in dependencies_table["dynamic"]]
+        return Dependencies(
+            link_target=dependencies_table["link_target"],
+            deploy_files=dependencies_table["deploy_files"],
+            dynamic=dynamic,
+            auxiliary=AuxiliarySupportedTable.parse_auxiliary(dependencies_table)
+        )
 
 
 @dataclass
 class CompiledWith:
     TableName = "compiled_with"
     compiler: str = ""
     flags: str = ""
@@ -523,24 +500,24 @@
         table.add("libraries", libraries_arr)
 
         return table
 
     @staticmethod
     def parse_from_table(compiled_with_table):
         required_table_entries = ["compiler", "flags", "crt", "libraries"]
-        _check_required_table_entries(compiled_with_table,
-                                      required_table_entries)
+        _check_required_table_entries(compiled_with_table, required_table_entries)
         libraries = [
-            LibraryReference.parse_from_table(lib_ref_table)
-            for lib_ref_table in compiled_with_table["libraries"]
+            LibraryReference.parse_from_table(lib_ref_table) for lib_ref_table in compiled_with_table["libraries"]
         ]
-        return CompiledWith(compiler=compiled_with_table["compiler"],
-                            flags=compiled_with_table["flags"],
-                            crt=compiled_with_table["crt"],
-                            libraries=libraries)
+        return CompiledWith(
+            compiler=compiled_with_table["compiler"],
+            flags=compiled_with_table["flags"],
+            crt=compiled_with_table["crt"],
+            libraries=libraries
+        )
 
 
 @dataclass
 class Declaration:
     TableName = "declaration"
     code: str = ""
 
@@ -548,16 +525,15 @@
         table = tomlkit.table()
         table.add("code", self.code)
         return table
 
     @staticmethod
     def parse_from_table(declaration_table):
         required_table_entries = ["code"]
-        _check_required_table_entries(declaration_table,
-                                      required_table_entries)
+        _check_required_table_entries(declaration_table, required_table_entries)
         return Declaration(code=declaration_table["code"])
 
 
 @dataclass
 class HATFile:
     """Encapsulates a HAT file. An instance of this class can be created by calling the
     Deserialize class method e.g.:
@@ -569,50 +545,47 @@
     """
     name: str = ""
     description: Description = None
     _function_table: FunctionTable = None
     _device_function_table: DeviceFunctionTable = None
     functions: list = field(default_factory=list)
     device_functions: list = field(default_factory=list)
-    function_map: dict = field(default_factory=dict)
-    device_function_map: list = field(default_factory=list)
+    function_map: Dict[str, Function] = field(default_factory=dict)
+    device_function_map: Dict[str, Function] = field(default_factory=dict)
     target: Target = None
     dependencies: Dependencies = None
     compiled_with: CompiledWith = None
     declaration: Declaration = None
     path: Path = None
 
     HATPrologue = "\n#ifndef __{0}__\n#define __{0}__\n\n#ifdef TOML\n"
     HATEpilogue = "\n#endif // TOML\n\n#endif // __{0}__\n"
 
     def __post_init__(self):
         self.functions = self._function_table.functions
         self.function_map = self._function_table.function_map
         for func in self.functions:
             func.hat_file = self
-            func.link_target = Path(self.path).resolve(
-            ).parent / self.dependencies.link_target
+            func.link_target = Path(self.path).resolve().parent / self.dependencies.link_target
 
         if not self._device_function_table:
             self._device_function_table = DeviceFunctionTable({})
         self.device_function_map = self._device_function_table.function_map
         self.device_functions = self._device_function_table.functions
 
     def Serialize(self, filepath=None):
         """Serilizes the HATFile to disk using the file location specified by `filepath`.
         If `filepath` is not specified then the object's `path` attribute is used."""
         if filepath is None:
             filepath = self.path
         root_table = tomlkit.table()
         root_table.add(Description.TableName, self.description.to_table())
-        root_table.add(FunctionTable.TableName,
-                       self._function_table.to_table())
+        root_table.add(FunctionTable.TableName, self._function_table.to_table())
         if self.device_function_map:
-            root_table.add(DeviceFunctionTable.TableName,
-                           self._device_function_table.to_table())
+            root_table.add(DeviceFunctionTable.TableName, self._device_function_table.to_table())
         root_table.add(Target.TableName, self.target.to_table())
         root_table.add(Dependencies.TableName, self.dependencies.to_table())
         root_table.add(CompiledWith.TableName, self.compiled_with.to_table())
         root_table.add(Declaration.TableName, self.declaration.to_table())
         with open(filepath, "w") as out_file:
             # MSVC does not allow "." in macro definitions
             name = self.name.replace(".", "_")
@@ -622,33 +595,26 @@
 
     @staticmethod
     def Deserialize(filepath) -> "HATFile":
         """Creates an instance of A HATFile class by deserializing the contents of the file at `filepath`"""
         hat_toml = _read_toml_file(filepath)
         name = os.path.splitext(os.path.basename(filepath))[0]
         required_entries = [
-            Description.TableName, FunctionTable.TableName, Target.TableName,
-            Dependencies.TableName, CompiledWith.TableName,
-            Declaration.TableName
+            Description.TableName, FunctionTable.TableName, Target.TableName, Dependencies.TableName,
+            CompiledWith.TableName, Declaration.TableName
         ]
         _check_required_table_entries(hat_toml, required_entries)
         device_function_table = None
         if DeviceFunctionTable.TableName in hat_toml:
-            device_function_table = DeviceFunctionTable.parse_from_table(
-                hat_toml[DeviceFunctionTable.TableName])
+            device_function_table = DeviceFunctionTable.parse_from_table(hat_toml[DeviceFunctionTable.TableName])
         hat_file = HATFile(
             name=name,
-            description=Description.parse_from_table(
-                hat_toml[Description.TableName]),
-            _function_table=FunctionTable.parse_from_table(
-                hat_toml[FunctionTable.TableName]),
+            description=Description.parse_from_table(hat_toml[Description.TableName]),
+            _function_table=FunctionTable.parse_from_table(hat_toml[FunctionTable.TableName]),
             _device_function_table=device_function_table,
-            target=Target.parse_from_table(
-                hat_toml[Target.TableName]),
-            dependencies=Dependencies.parse_from_table(
-                hat_toml[Dependencies.TableName]),
-            compiled_with=CompiledWith.parse_from_table(
-                hat_toml[CompiledWith.TableName]),
-            declaration=Declaration.parse_from_table(
-                hat_toml[Declaration.TableName]),
-            path=Path(filepath).resolve())
+            target=Target.parse_from_table(hat_toml[Target.TableName]),
+            dependencies=Dependencies.parse_from_table(hat_toml[Dependencies.TableName]),
+            compiled_with=CompiledWith.parse_from_table(hat_toml[CompiledWith.TableName]),
+            declaration=Declaration.parse_from_table(hat_toml[Declaration.TableName]),
+            path=Path(filepath).resolve()
+        )
         return hat_file
```

### Comparing `hatlib-0.0.8/hatlib/hat_to_dynamic.py` & `hatlib-0.0.9/hatlib/hat_to_dynamic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-
 """Converts a statically-linked HAT package into a Dynamically-linked HAT package
 
 HAT packages come in two varieties: statically-linked and dynamically-linked. A statically-linked
 HAT package contains a binary file with the extension '.o', '.obj', '.a', or `.lib`. A dynamically-linked
 HAT package contains a binary file with the extension '.dll' or '.so'. This tool converts a
 statically-linked HAT package into a dynamically-linked HAT package.
 
@@ -20,66 +19,77 @@
 
 import sys
 import os
 import argparse
 import shutil
 from secrets import token_hex
 
-if __package__:
-    from .hat_file import HATFile, OperatingSystem
-    from .platform_utilities import get_platform, ensure_compiler_in_path, run_command
-else:
-    from hat_file import HATFile, OperatingSystem
-    from platform_utilities import get_platform, ensure_compiler_in_path, run_command
+from .hat_file import HATFile, OperatingSystem
+from .hat_package import HATPackage
+from .platform_utilities import get_platform, ensure_compiler_in_path, run_command
 
 
-def linux_create_dynamic_package(input_hat_path, input_hat_binary_path, output_hat_path, hat_file, quiet=True):
+def linux_create_dynamic_package(input_hat_path,
+                                 input_hat_binary_path,
+                                 output_hat_path,
+                                 hat_file,
+                                 quiet=True):
     """Creates a dynamic HAT (.so) from a static HAT (.o/.a) on a Linux/macOS platform"""
     # Confirm that this is a static hat library
     _, extension = os.path.splitext(input_hat_binary_path)
     if extension not in [".o", ".a"]:
         sys.exit(
-            f"ERROR: Expected input library to have extension .o or .a, but received {input_hat_binary_path} instead")
+            f"ERROR: Expected input library to have extension .o or .a, but received {input_hat_binary_path} instead"
+        )
 
     # Create a C source file to resolve inline functions defined in the static HAT package
     include_path = os.path.dirname(input_hat_binary_path)
     inline_c_path = os.path.join(include_path, "inline.c")
     inline_obj_path = os.path.join(include_path, "inline.o")
     with open(inline_c_path, "w") as f:
         f.write(f"#include <{os.path.basename(input_hat_path)}>")
     # compile it separately so that we can suppress the warnings about the missing terminating ' character
     run_command(
-        f'gcc -c -w -fPIC -o "{inline_obj_path}" -I"{include_path}" "{inline_c_path}"', quiet=quiet)
+        f'gcc -c -w -fPIC -o "{inline_obj_path}" -I"{include_path}" "{inline_c_path}"',
+        quiet=quiet)
 
     # create new HAT binary
     prefix, _ = os.path.splitext(output_hat_path)
     # always create a new so file (avoids cases where so file is already loaded)
     suffix = token_hex(4)
     output_hat_binary_path = f"{prefix}_{suffix}.so"
     libraries = " ".join(
         [d.target_file for d in hat_file.dependencies.dynamic])
     run_command(
-        f'gcc -shared -fPIC -o "{output_hat_binary_path}" "{inline_obj_path}" "{input_hat_binary_path}" {libraries}', quiet=quiet)
+        f'gcc -shared -fPIC -o "{output_hat_binary_path}" "{inline_obj_path}" "{input_hat_binary_path}" {libraries}',
+        quiet=quiet)
 
     # create new HAT file
     # previous dependencies are now part of the binary
     hat_file.dependencies.dynamic = []
     hat_file.dependencies.link_target = os.path.basename(
         output_hat_binary_path)
     hat_file.Serialize(output_hat_path)
 
+    return HATPackage(output_hat_path)
+
 
-def windows_create_dynamic_package(input_hat_path, input_hat_binary_path, output_hat_path, hat_file, quiet=True):
+def windows_create_dynamic_package(input_hat_path,
+                                   input_hat_binary_path,
+                                   output_hat_path,
+                                   hat_file,
+                                   quiet=True):
     """Creates a Windows dynamic HAT package (.dll) from a static HAT package (.obj/.lib)"""
 
     # Confirm that this is a static hat library
     _, extension = os.path.splitext(input_hat_binary_path)
     if extension not in [".obj", ".lib"]:
         sys.exit(
-            f"ERROR: Expected input library to have extension .obj or .lib, but received {input_hat_binary_path} instead")
+            f"ERROR: Expected input library to have extension .obj or .lib, but received {input_hat_binary_path} instead"
+        )
 
     # Create all file in a directory named build
     if not os.path.exists("build"):
         os.mkdir("build")
 
     cwd = os.getcwd()
     try:
@@ -87,17 +97,19 @@
 
         # Create a C source file for the DLL entry point and compile in into an obj
         with open("dllmain.cpp", "w") as f:
             f.write("#include <windows.h>\n")
             # Resolve inline functions defined in the static HAT package
             f.write("#include <{}>\n".format(os.path.basename(input_hat_path)))
             f.write(
-                "BOOL APIENTRY DllMain(HMODULE, DWORD, LPVOID) { return TRUE; }\n")
+                "BOOL APIENTRY DllMain(HMODULE, DWORD, LPVOID) { return TRUE; }\n"
+            )
         run_command(
-            f'cl.exe /nologo /I"{os.path.dirname(input_hat_path)}" /Fodllmain.obj /c dllmain.cpp', quiet=quiet)
+            f'cl.exe /nologo /I"{os.path.dirname(input_hat_path)}" /Fodllmain.obj /c dllmain.cpp',
+            quiet=quiet)
 
         # create the new HAT binary dll
         # always create a new dll (avoids case where dll is already loaded)
         suffix = token_hex(4)
         prefix, _ = os.path.splitext(output_hat_path)
         output_hat_binary_path = f"{prefix}_{suffix}.dll"
 
@@ -117,71 +129,97 @@
         hat_file.dependencies.link_target = os.path.basename(
             output_hat_binary_path)
         hat_file.Serialize("out.hat")
         shutil.copyfile("out.hat", output_hat_path)
     finally:
         os.chdir(cwd)  # restore the current working directory
 
+    return HATPackage(output_hat_path)
+
 
 def parse_args():
     """Parses and checks the command line arguments"""
-    parser = argparse.ArgumentParser(description="Creates a dynamically-linked HAT package from a statically-linked HAT package.\n"
-                                     "Example:\n"
-                                     "    hatlib.hat_to_dynamic input.hat output.hat\n")
-
-    parser.add_argument("input_hat_path", type=str,
-                        help="Path to the existing HAT file, which represents a statically-linked HAT package")
-    parser.add_argument("output_hat_path", type=str,
-                        help="Path to the new HAT file, which will represent a dynamically-linked HAT package")
-    parser.add_argument('-v', "--verbose", action='store_true', help="Enable verbose output")
+    parser = argparse.ArgumentParser(
+        description=
+        "Creates a dynamically-linked HAT package from a statically-linked HAT package.\n"
+        "Example:\n"
+        "    hatlib.hat_to_dynamic input.hat output.hat\n")
+
+    parser.add_argument(
+        "input_hat_path",
+        type=str,
+        help=
+        "Path to the existing HAT file, which represents a statically-linked HAT package"
+    )
+    parser.add_argument(
+        "output_hat_path",
+        type=str,
+        help=
+        "Path to the new HAT file, which will represent a dynamically-linked HAT package"
+    )
+    parser.add_argument('-v',
+                        "--verbose",
+                        action='store_true',
+                        help="Enable verbose output")
     args = parser.parse_args()
 
     # check args
     if not os.path.exists(args.input_hat_path):
         sys.exit(f"ERROR: File {args.input_hat_path} not found")
 
-    if os.path.abspath(args.input_hat_path) == os.path.abspath(args.output_hat_path):
+    if os.path.abspath(args.input_hat_path) == os.path.abspath(
+            args.output_hat_path):
         sys.exit("ERROR: Output file must be different from input file")
 
     _, extension = os.path.splitext(args.input_hat_path)
     if extension != ".hat":
         sys.exit(
-            f"ERROR: Expected input file to have extension .hat, but received {extension} instead")
+            f"ERROR: Expected input file to have extension .hat, but received {extension} instead"
+        )
 
     _, extension = os.path.splitext(args.output_hat_path)
     if extension != ".hat":
         sys.exit(
-            f"ERROR: Expected output file to have extension .hat, but received {extension} instead")
+            f"ERROR: Expected output file to have extension .hat, but received {extension} instead"
+        )
 
     return args
 
 
 def create_dynamic_package(input_hat_path, output_hat_path, quiet=True):
     platform = get_platform()
     ensure_compiler_in_path()
 
     # load the function decscriptions and the library path from the hat file
     input_hat_path = os.path.abspath(input_hat_path)
     hat_file = HATFile.Deserialize(input_hat_path)
 
     # get the absolute path to the input binary
     input_hat_binary_filename = hat_file.dependencies.link_target
-    input_hat_binary_path = os.path.join(
-        os.path.dirname(input_hat_path), input_hat_binary_filename)
+    input_hat_binary_path = os.path.join(os.path.dirname(input_hat_path),
+                                         input_hat_binary_filename)
 
     # create the dynamic package
     output_hat_path = os.path.abspath(output_hat_path)
     if platform == OperatingSystem.Windows:
-        windows_create_dynamic_package(
-            input_hat_path, input_hat_binary_path, output_hat_path, hat_file, quiet=quiet)
+        windows_create_dynamic_package(input_hat_path,
+                                       input_hat_binary_path,
+                                       output_hat_path,
+                                       hat_file,
+                                       quiet=quiet)
     elif platform in [OperatingSystem.Linux, OperatingSystem.MacOS]:
-        linux_create_dynamic_package(
-            input_hat_path, input_hat_binary_path, output_hat_path, hat_file, quiet=quiet)
+        linux_create_dynamic_package(input_hat_path,
+                                     input_hat_binary_path,
+                                     output_hat_path,
+                                     hat_file,
+                                     quiet=quiet)
 
 
 def main():
     args = parse_args()
-    create_dynamic_package(args.input_hat_path, args.output_hat_path, quiet=not args.verbose)
+    create_dynamic_package(args.input_hat_path,
+                           args.output_hat_path,
+                           quiet=not args.verbose)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hatlib-0.0.8/hatlib/hat_to_lib.py` & `hatlib-0.0.9/hatlib/hat_to_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,16 @@
 """
 
 import sys
 import os
 import argparse
 import shutil
 
-if __package__:
-    from .hat_file import HATFile, OperatingSystem
-    from .platform_utilities import get_platform, ensure_compiler_in_path, run_command
-else:
-    from hat_file import HATFile, OperatingSystem
-    from platform_utilities import get_platform, ensure_compiler_in_path, run_command
+from .hat_file import HATFile, OperatingSystem
+from .platform_utilities import get_platform, ensure_compiler_in_path, run_command
 
 
 def linux_create_static_package(input_hat_binary_path, output_hat_path, hat_file, quiet=True):
     """Creates a static HAT (.a) from a static HAT (.o) on a Linux/macOS platform"""
     # Confirm that this is a static .o hat library
     _, extension = os.path.splitext(input_hat_binary_path)
     if extension != ".o":
```

### Comparing `hatlib-0.0.8/hatlib/platform_utilities.py` & `hatlib-0.0.9/hatlib/platform_utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 import os
 import platform
 import shlex
 import shutil
 import subprocess
 import sys
 
-if __package__:
-    from .hat_file import OperatingSystem
-else:
-    from hat_file import OperatingSystem
+from .hat_file import OperatingSystem
 
 
 def _preprocess_command(command_to_run, shell):
     if platform.system() == "Windows":
         return command_to_run
     elif type(command_to_run) == str and not shell:
         return shlex.split(command_to_run)
@@ -29,45 +26,34 @@
     if isinstance(iostream, io.TextIOBase):
         with open(iostream.name, "r") as f:
             print(f.name)
             print(f.read())
 
 
 def run_command(
-        command_to_run,
-        working_directory=None,
-        stdout=None,
-        stderr=None,
-        shell=False,
-        pretend=False,
-        quiet=True):
+    command_to_run, working_directory=None, stdout=None, stderr=None, shell=False, pretend=False, quiet=True
+):
     if not working_directory:
         working_directory = os.getcwd()
 
     if not quiet:
         print(f"\ncd {working_directory}")
         print(f"{command_to_run}\n")
 
     command_to_run = _preprocess_command(command_to_run, shell)
 
     if not pretend:
-        with subprocess.Popen(
-                command_to_run,
-                close_fds=(platform.system() != "Windows"),
-                shell=shell,
-                stdout=stdout,
-                stderr=stderr,
-                cwd=working_directory) as proc:
+        with subprocess.Popen(command_to_run, close_fds=(platform.system() != "Windows"), shell=shell, stdout=stdout,
+                              stderr=stderr, cwd=working_directory) as proc:
 
             proc.wait()
             if proc.returncode:
                 _dump_file_contents(stderr)
                 _dump_file_contents(stdout)
-                raise subprocess.CalledProcessError(
-                    proc.returncode, command_to_run)
+                raise subprocess.CalledProcessError(proc.returncode, command_to_run)
 
 
 def get_platform():
     """Returns the current platform: Linux, Windows, or OS X"""
 
     if sys.platform.startswith("linux"):
         return OperatingSystem.Linux
@@ -80,33 +66,31 @@
 
 
 def linux_ensure_compiler_in_path():
     """Ensures that PATH contains the $CXX/$CC (or gcc) compiler.
     Prompts the user if not found."""
     compiler = os.environ.get("CXX") or (os.environ.get("CC") or "gcc")
     if not shutil.which(compiler):
-        sys.exit(
-            'ERROR: Could not find any valid C or C++ compiler, please install gcc before continuing')
+        sys.exit('ERROR: Could not find any valid C or C++ compiler, please install gcc before continuing')
 
 
 def windows_ensure_compiler_in_path():
     """Ensures that PATH contains the cl.exe compiler from Microsoft Visual Studio.
     Prompts the user if not found."""
     import vswhere
     vs_path = vswhere.get_latest_path()
     if not vs_path:
-        sys.exit(
-            "ERROR: Could not find Visual Studio, please ensure that you have Visual Studio installed")
+        sys.exit("ERROR: Could not find Visual Studio, please ensure that you have Visual Studio installed")
 
     # Check if cl.exe is in PATH
-    if not shutil.which("cl"):  # returns 0 if found, !0 otherwise
-        vcvars_script_path = os.path.join(
-            vs_path, r"VC\Auxiliary\Build\vcvars64.bat")
+    if not shutil.which("cl"):    # returns 0 if found, !0 otherwise
+        vcvars_script_path = os.path.join(vs_path, r"VC\Auxiliary\Build\vcvars64.bat")
         sys.exit(
-            f'ERROR: Could not find cl.exe, please run "{vcvars_script_path}" (including quotes) to setup your command prompt')
+            f'ERROR: Could not find cl.exe, please run "{vcvars_script_path}" (including quotes) to setup your command prompt'
+        )
 
 
 def ensure_compiler_in_path():
     platform = get_platform()
     if platform == OperatingSystem.Windows:
         windows_ensure_compiler_in_path()
     else:
```

### Comparing `hatlib-0.0.8/hatlib/pyhip_hip.py` & `hatlib-0.0.9/hatlib/pyhip/hip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Python interface to hip library
 lifted from https://github.com/jatinx/PyHIP
 TODO: move to a submodule
 """
 
-import sys, ctypes
+import ctypes
+import sys
 
 _libhip_libname = 'libamdhip64.so'
 
 _libhip = None
 if 'linux' in sys.platform:
     _libhip = ctypes.cdll.LoadLibrary(_libhip_libname)
 else:
     # Currently we do not support windows, mainly because I do not have a windows build of hip
     raise RuntimeError('Only linux is supported')
 
-if _libhip == None:
+if _libhip is None:
     raise OSError('hiprtc library not found')
 
 
 def POINTER(obj):
     """
     ctype pointer to object
     """
@@ -478,15 +479,15 @@
         Pointer to allocated device memory.
 
     """
 
     ptr = ctypes.c_void_p()
     status = _libhip.hipMalloc(ctypes.byref(ptr), count)
     hipCheckStatus(status)
-    if ctype != None:
+    if ctype is not None:
         ptr = ctypes.cast(ptr, ctypes.POINTER(ctype))
     return ptr
 
 
 _libhip.hipFree.restype = int
 _libhip.hipFree.argtypes = [ctypes.c_void_p]
```

### Comparing `hatlib-0.0.8/hatlib/pyhip_hiprtc.py` & `hatlib-0.0.9/hatlib/pyhip/hiprtc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Python interface to hiprtc
 lifted from https://github.com/jatinx/PyHIP
 TODO: move to a submodule
 """
 
-import sys, ctypes
+import ctypes
+import sys
 
 # _libhiprtc_libname = 'libhiprtc.so' # Currently its the same library
 _libhiprtc_libname = 'libamdhip64.so'
 
 _libhiprtc = None
 if 'linux' in sys.platform:
     _libhiprtc = ctypes.cdll.LoadLibrary(_libhiprtc_libname)
 else:
     # Currently we do not support windows, mainly because I do not have a windows build of hip
     raise RuntimeError('Only linux is supported')
 
-if _libhiprtc == None:
+if _libhiprtc is None:
     raise OSError('hiprtc library not found')
 
 
 def POINTER(obj):
     """
     ctype pointer to object
     """
```

### Comparing `hatlib-0.0.8/hatlib/rocm_loader.py` & `hatlib-0.0.9/hatlib/rocm_loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 import ctypes
 import pathlib
 import numpy as np
 from functools import reduce
 from typing import List
 
-try:
-    from .arg_info import ArgInfo, verify_args
-    from .gpu_headers import ROCM_HEADER_MAP
-    from .pyhip_hip import *
-    from .pyhip_hiprtc import *
-except ModuleNotFoundError:
-    from arg_info import ArgInfo, verify_args
-    from gpu_headers import ROCM_HEADER_MAP
-    from pyhip_hip import *
-    from pyhip_hiprtc import *
+from .arg_info import ArgInfo, verify_args
+from .hat_file import Function
+from .gpu_headers import ROCM_HEADER_MAP
+from .pyhip.hip import *
+from .pyhip.hiprtc import *
 
 
 def _arg_size(arg_info: ArgInfo):
-    return arg_info.element_num_bytes * reduce(lambda x, y: x * y,
-                                               arg_info.numpy_shape)
+    return arg_info.element_num_bytes * reduce(lambda x, y: x * y, arg_info.numpy_shape)
 
 
 def initialize_rocm():
     # Initialize ROCM Driver API
     hipInit(0)
 
 
 def compile_rocm_program(rocm_src_path: pathlib.Path, func_name):
     src = rocm_src_path.read_text()
 
-    prog = hiprtcCreateProgram(source=src,
-                               name=func_name + ".cu",
-                               header_names=ROCM_HEADER_MAP.keys(),
-                               header_sources=ROCM_HEADER_MAP.values())
+    prog = hiprtcCreateProgram(
+        source=src,
+        name=func_name + ".cu",
+        header_names=ROCM_HEADER_MAP.keys(),
+        header_sources=ROCM_HEADER_MAP.values()
+    )
     device_properties = hipGetDeviceProperties(0)
-    hiprtcCompileProgram(prog, [
-        f'--offload-arch={device_properties.gcnArchName}',
-        '-D__HIP_PLATFORM_AMD__'
-    ])
+    hiprtcCompileProgram(prog, [f'--offload-arch={device_properties.gcnArchName}', '-D__HIP_PLATFORM_AMD__'])
     print(hiprtcGetProgramLog(prog))
     code = hiprtcGetCode(prog)
 
     return code
 
 
 def get_func_from_rocm_program(rocm_program, func_name):
@@ -55,75 +48,64 @@
     for arg in arg_infos:
         mem = hipMalloc(_arg_size(arg))
         device_mem.append(mem)
 
     return device_mem
 
 
-def transfer_mem_host_to_rocm(device_args: List, host_args: List[np.array],
-                              arg_infos: List[ArgInfo]):
-    for device_arg, host_arg, arg_info in zip(device_args, host_args,
-                                              arg_infos):
-        if 'input' in arg_info.usage:
-            hipMemcpy_htod(dst=device_arg,
-                           src=host_arg.ctypes.data,
-                           count=_arg_size(arg_info))
-
-
-def transfer_mem_rocm_to_host(device_args: List, host_args: List[np.array],
-                              arg_infos: List[ArgInfo]):
-    for device_arg, host_arg, arg_info in zip(device_args, host_args,
-                                              arg_infos):
-        if 'output' in arg_info.usage:
-            hipMemcpy_dtoh(dst=host_arg.ctypes.data,
-                           src=device_arg,
-                           count=_arg_size(arg_info))
+def transfer_mem_host_to_rocm(device_args: List, host_args: List[np.array], arg_infos: List[ArgInfo]):
+    for device_arg, host_arg, arg_info in zip(device_args, host_args, arg_infos):
+        if 'input' in arg_info.usage.value:
+            hipMemcpy_htod(dst=device_arg, src=host_arg.ctypes.data, count=_arg_size(arg_info))
+
+
+def transfer_mem_rocm_to_host(device_args: List, host_args: List[np.array], arg_infos: List[ArgInfo]):
+    for device_arg, host_arg, arg_info in zip(device_args, host_args, arg_infos):
+        if 'output' in arg_info.usage.value:
+            hipMemcpy_dtoh(dst=host_arg.ctypes.data, src=device_arg, count=_arg_size(arg_info))
 
 
 def device_args_to_ptr_list(device_args: List):
     ptrs = [np.array([int(d_arg)], dtype=np.uint64) for d_arg in device_args]
     ptrs = np.array([ptr.ctypes.data for ptr in ptrs], dtype=np.uint64)
 
     return ptrs
 
 
-def create_loader_for_device_function(device_func, hat_details):
-    hat_path: pathlib.Path = hat_details.path
-    rocm_src_path: pathlib.Path = hat_path.parent / device_func["provider"]
-    func_name = device_func["name"]
+def create_loader_for_device_function(device_func: Function, hat_dir_path: str):
+    if not device_func.provider:
+        raise RuntimeError("Expected a provider for the device function")
+
+    rocm_src_path: pathlib.Path = pathlib.Path(hat_dir_path) / device_func.provider
+    func_name = device_func.name
 
     rocm_program = compile_rocm_program(rocm_src_path, func_name)
 
     initialize_rocm()
 
     kernel = get_func_from_rocm_program(rocm_program, func_name)
 
-    hat_arg_descriptions = device_func["arguments"]
+    hat_arg_descriptions = device_func.arguments
     arg_infos = [ArgInfo(d) for d in hat_arg_descriptions]
-    launch_parameters = device_func["launch_parameters"]
+    launch_parameters = device_func.launch_parameters
 
     class DataStruct(ctypes.Structure):
-        _fields_ = [(f"arg{i}", ctypes.c_void_p)
-                    for i in range(len(arg_infos))]
+        _fields_ = [(f"arg{i}", ctypes.c_void_p) for i in range(len(arg_infos))]
 
     def f(*args):
         verify_args(args, arg_infos, func_name)
         device_mem = allocate_rocm_mem(arg_infos)
-        transfer_mem_host_to_rocm(device_args=device_mem,
-                                  host_args=args,
-                                  arg_infos=arg_infos)
+        transfer_mem_host_to_rocm(device_args=device_mem, host_args=args, arg_infos=arg_infos)
         data = DataStruct(*device_mem)
 
         hipModuleLaunchKernel(
             kernel,
-            *launch_parameters,  # [ grid[x-z], block[x-z] ]
-            0,  # dynamic shared memory
-            0,  # stream
-            data,  # data
+            *launch_parameters,    # [ grid[x-z], block[x-z] ]
+            0,    # dynamic shared memory
+            0,    # stream
+            data,    # data
         )
         hipDeviceSynchronize()
 
-        transfer_mem_rocm_to_host(device_args=device_mem,
-                                  host_args=args,
-                                  arg_infos=arg_infos)
+        transfer_mem_rocm_to_host(device_args=device_mem, host_args=args, arg_infos=arg_infos)
 
     return f
```

### Comparing `hatlib-0.0.8/hatlib/test/test_benchmark_hat_package.py` & `hatlib-0.0.9/test/test_benchmark_hat_package.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python3
 import unittest
 import os
 import sys
 import accera as acc
-
-sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
-
-from benchmark_hat_package import run_benchmark
+from hatlib import run_benchmark
 
 
 class BenchmarkHATPackage_test(unittest.TestCase):
+
     def test_benchmark(self):
         A = acc.Array(role=acc.Array.Role.INPUT, shape=(256, 256))
         B = acc.Array(role=acc.Array.Role.INPUT, shape=(256, 256))
         C = acc.Array(role=acc.Array.Role.INPUT_OUTPUT, shape=(256, 256))
 
         nest = acc.Nest(shape=(256, 256, 256))
         i, j, k = nest.get_indices()
 
         @nest.iteration_logic
         def _():
             C[i, j] += A[i, k] * B[k, j]
 
         package = acc.Package()
         package.add(nest, args=(A, B, C), base_name="test_function")
-        package.build(name="BenchmarkHATPackage_test_benchmark",
-                      output_dir="test_acccgen",
-                      format=acc.Package.Format.HAT_DYNAMIC)
-
-        run_benchmark("test_acccgen/BenchmarkHATPackage_test_benchmark.hat",
-                      store_in_hat=False,
-                      batch_size=2,
-                      min_time_in_sec=1,
-                      input_sets_minimum_size_MB=1)
+        package.build(
+            name="BenchmarkHATPackage_test_benchmark", output_dir="test_acccgen", format=acc.Package.Format.HAT_DYNAMIC
+        )
+
+        run_benchmark(
+            "test_acccgen/BenchmarkHATPackage_test_benchmark.hat",
+            store_in_hat=False,
+            batch_size=2,
+            min_time_in_sec=1,
+            input_sets_minimum_size_MB=1
+        )
 
     def test_benchmark_multiple_functions(self):
         A = acc.Array(role=acc.Array.Role.INPUT, shape=(256, 256))
         B = acc.Array(role=acc.Array.Role.INPUT, shape=(256, 256))
         C = acc.Array(role=acc.Array.Role.INPUT_OUTPUT, shape=(256, 256))
-        D = acc.Array(role=acc.Array.Role.INPUT, shape=(256, 256)) # dummy argument
+        D = acc.Array(role=acc.Array.Role.INPUT, shape=(256, 256))    # dummy argument
 
         nest = acc.Nest(shape=(256, 256, 256))
         i, j, k = nest.get_indices()
 
         @nest.iteration_logic
         def _():
             C[i, j] += A[i, k] * B[k, j]
@@ -50,20 +50,22 @@
         package = acc.Package()
         package.add(nest, args=(A, B, C), base_name="test_function")
 
         # add another function with a dummy argument - run_benchmark should be able to call it
         # with the correct signature
         package.add(nest, args=(A, B, C, D), base_name="test_function_dummy")
 
-        package.build(name="BenchmarkHATPackage_test_benchmark",
-                      output_dir="test_acccgen",
-                      format=acc.Package.Format.HAT_DYNAMIC)
-
-        run_benchmark("test_acccgen/BenchmarkHATPackage_test_benchmark.hat",
-                      store_in_hat=False,
-                      batch_size=2,
-                      min_time_in_sec=1,
-                      input_sets_minimum_size_MB=1)
+        package.build(
+            name="BenchmarkHATPackage_test_benchmark", output_dir="test_acccgen", format=acc.Package.Format.HAT_DYNAMIC
+        )
+
+        run_benchmark(
+            "test_acccgen/BenchmarkHATPackage_test_benchmark.hat",
+            store_in_hat=False,
+            batch_size=2,
+            min_time_in_sec=1,
+            input_sets_minimum_size_MB=1
+        )
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `hatlib-0.0.8/hatlib/test/test_hat.py` & `hatlib-0.0.9/test/test_hat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 #!/usr/bin/env python3
 import accera as acc
 import numpy as np
 import os
 import sys
 import unittest
-
-sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
-
-from hat import load
-from hat_to_dynamic import create_dynamic_package
-from hat_to_lib import create_static_package
+from hatlib import load, create_dynamic_package, create_static_package
 
 
 class HAT_test(unittest.TestCase):
 
     def test_load(self):
 
         # Generate a HAT package
@@ -28,39 +23,35 @@
             B[i, j] += A[i, j]
 
         package = acc.Package()
         function = package.add(nest, args=(A, B), base_name="test_function")
 
         for mode in [acc.Package.Mode.RELEASE, acc.Package.Mode.DEBUG]:
             package_name = f"HAT_test_load_{mode.value}"
-            package.build(name=package_name,
-                          output_dir="test_acccgen",
-                          format=acc.Package.Format.HAT_STATIC,
-                          mode=mode)
+            package.build(name=package_name, output_dir="test_acccgen", format=acc.Package.Format.HAT_STATIC, mode=mode)
 
-            create_dynamic_package(f"test_acccgen/{package_name}.hat",
-                                   f"test_acccgen/{package_name}.dyn.hat")
+            create_dynamic_package(f"test_acccgen/{package_name}.hat", f"test_acccgen/{package_name}.dyn.hat")
 
-            hat_package = load(f"test_acccgen/{package_name}.dyn.hat")
+            _, func_dict = load(f"test_acccgen/{package_name}.dyn.hat")
 
-            for name in hat_package.names:
+            for name in func_dict.names:
                 print(name)
 
             # create numpy arguments with the correct shape and dtype
             A = np.random.rand(16, 16).astype(np.float32)
             B = np.random.rand(16, 16).astype(np.float32)
             B_ref = B + A
 
             # find the function by basename
-            test_function = hat_package["test_function"]
+            test_function = func_dict["test_function"]
             test_function(A, B)
 
             # check for correctness
             np.testing.assert_allclose(B, B_ref)
 
             # find the function by actual name
             B_ref = B + A
-            test_function1 = hat_package[function.name]
+            test_function1 = func_dict[function.name]
             test_function1(A, B)
 
             # check for correctness
             np.testing.assert_allclose(B, B_ref)
```

### Comparing `hatlib-0.0.8/hatlib/test/test_hat_file.py` & `hatlib-0.0.9/test/test_hat_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 import unittest
 from pathlib import Path
-
-sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
-
-from hat_file import (CallingConventionType, CompiledWith, Declaration,
-                      Dependencies, Description, Function, FunctionTable,
-                      HATFile, OperatingSystem, Parameter, ParameterType,
-                      Target, UsageType)
+from hatlib import (
+    CallingConventionType, CompiledWith, Declaration, Dependencies, Description, Function, FunctionTable, HATFile,
+    OperatingSystem, Parameter, ParameterType, Target, UsageType
+)
 
 
 class HATFile_test(unittest.TestCase):
 
     def test_file_basic_serialize(self):
         # Construct a HAT file from scratch
         # Start with a function definition
         my_function = Function(
             name="my_function",
             description="Some description",
             calling_convention=CallingConventionType.StdCall,
-            return_info=Parameter(logical_type=ParameterType.RuntimeArray,
-                                  declared_type="float*",
-                                  element_type="float",
-                                  usage=UsageType.Input,
-                                  shape="[16, 16]",
-                                  affine_map=[16, 1],
-                                  size="16 * 16 * sizeof(float)"))
+            return_info=Parameter(
+                logical_type=ParameterType.RuntimeArray,
+                declared_type="float*",
+                element_type="float",
+                usage=UsageType.Input,
+                shape="[16, 16]",
+                affine_map=[16, 1],
+                size="16 * 16 * sizeof(float)"
+            )
+        )
         # Create the function table
         functions = FunctionTable({"my_function": my_function})
         # Create the HATFile object
         hat_file1 = HATFile(
             name="test_file",
             description=Description(
-                version="0.0.1",
-                author="me",
-                license_url="https://www.apache.org/licenses/LICENSE-2.0.html"
+                version="0.0.1", author="me", license_url="https://www.apache.org/licenses/LICENSE-2.0.html"
             ),
             _function_table=functions,
-            target=Target(required=Target.Required(os=OperatingSystem.Windows,
-                                                   cpu=Target.Required.CPU(
-                                                       architecture="Haswell",
-                                                       extensions=["AVX2"]),
-                                                   gpu=None),
-                          optimized_for=Target.OptimizedFor()),
+            target=Target(
+                required=Target.Required(
+                    os=OperatingSystem.Windows,
+                    cpu=Target.Required.CPU(architecture="Haswell", extensions=["AVX2"]),
+                    gpu=None
+                ),
+                optimized_for=Target.OptimizedFor()
+            ),
             dependencies=Dependencies(link_target="my_lib.lib"),
             compiled_with=CompiledWith(compiler="VC++"),
             declaration=Declaration(),
-            path=Path(".").resolve())
+            path=Path(".").resolve()
+        )
         # Serialize it to disk
         test_file_name = "test_file_serialize.hat"
 
         try:
             hat_file1.Serialize(test_file_name)
             # Deserialize it and verify it has what we expect
             hat_file2 = HATFile.Deserialize(test_file_name)
@@ -61,33 +62,31 @@
             # Remove the file
             os.remove(test_file_name)
 
         # Do basic verification that the deserialized HatFile contains what we
         # specified when we created the HATFile directly
         self.assertEqual(hat_file1.description, hat_file2.description)
         self.assertEqual(hat_file1.dependencies, hat_file2.dependencies)
-        self.assertEqual(hat_file1.compiled_with.to_table(),
-                         hat_file2.compiled_with.to_table())
+        self.assertEqual(hat_file1.compiled_with.to_table(), hat_file2.compiled_with.to_table())
         self.assertTrue("my_function" in hat_file2.function_map)
 
     def test_file_basic_deserialize(self):
         # Load a HAT file from the samples directory
         hat_file1 = HATFile.Deserialize(
-            os.path.join(os.path.dirname(__file__), "..", "..", "samples",
-                         "sample_gemm_library.hat"))
+            os.path.join(os.path.dirname(__file__), "..", "samples", "sample_gemm_library.hat")
+        )
         description = {
             "author": "John Doe",
             "version": "1.2.3.5",
             "license_url": "https://www.apache.org/licenses/LICENSE-2.0.html",
         }
 
         # Do basic verification of known values in the file
         # Verify the description has entries we expect
-        self.assertLessEqual(description.items(),
-                             hat_file1.description.to_table().items())
+        self.assertLessEqual(description.items(), hat_file1.description.to_table().items())
         # Verify the list of functions
         self.assertTrue(len(hat_file1.functions) == 2)
         self.assertTrue("GEMM_B94D27B9934D3E08" in hat_file1.function_map)
         self.assertTrue("blas_sgemm_row_major" in hat_file1.function_map)
 
 
 if __name__ == '__main__':
```

### Comparing `hatlib-0.0.8/hatlib/test/test_hat_package.py` & `hatlib-0.0.9/test/test_hat_package.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 #!/usr/bin/env python3
 
 import sys
 import os
 import unittest
 from pathlib import Path
-
-sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
-
-from hat_file import (CallingConventionType, CompiledWith, Declaration,
-                      Dependencies, Description, Function, FunctionTable,
-                      HATFile, OperatingSystem, Parameter, ParameterType,
-                      Target, UsageType)
+from hatlib import (
+    CallingConventionType, CompiledWith, Declaration, Dependencies, Description, Function, FunctionTable, HATFile,
+    OperatingSystem, Parameter, ParameterType, Target, UsageType
+)
 
 
 class HATFile_test(unittest.TestCase):
 
     def test_file_basic_serialize(self):
         # Construct a HAT file from scratch
         # Start with a function definition
         my_function = Function(
             name="my_function",
             description="Some description",
             calling_convention=CallingConventionType.StdCall,
-            return_info=Parameter(logical_type=ParameterType.RuntimeArray,
-                                  declared_type="float*",
-                                  element_type="float",
-                                  usage=UsageType.Input,
-                                  shape="[16, 16]",
-                                  affine_map=[16, 1],
-                                  size="16 * 16 * sizeof(float)"))
+            return_info=Parameter(
+                logical_type=ParameterType.RuntimeArray,
+                declared_type="float*",
+                element_type="float",
+                usage=UsageType.Input,
+                shape="[16, 16]",
+                affine_map=[16, 1],
+                size="16 * 16 * sizeof(float)"
+            )
+        )
         # Create the function table
         functions = FunctionTable({"my_function": my_function})
         # Create the HATFile object
         hat_file1 = HATFile(
             name="test_file",
             description=Description(
-                version="0.0.1",
-                author="me",
-                license_url="https://www.apache.org/licenses/LICENSE-2.0.html"
+                version="0.0.1", author="me", license_url="https://www.apache.org/licenses/LICENSE-2.0.html"
             ),
             _function_table=functions,
-            target=Target(required=Target.Required(os=OperatingSystem.Windows,
-                                                   cpu=Target.Required.CPU(
-                                                       architecture="Haswell",
-                                                       extensions=["AVX2"]),
-                                                   gpu=None),
-                          optimized_for=Target.OptimizedFor()),
+            target=Target(
+                required=Target.Required(
+                    os=OperatingSystem.Windows,
+                    cpu=Target.Required.CPU(architecture="Haswell", extensions=["AVX2"]),
+                    gpu=None
+                ),
+                optimized_for=Target.OptimizedFor()
+            ),
             dependencies=Dependencies(link_target="my_lib.lib"),
             compiled_with=CompiledWith(compiler="VC++"),
             declaration=Declaration(),
-            path=Path(".").resolve())
+            path=Path(".").resolve()
+        )
         # Serialize it to disk
         test_file_name = "test_file_serialize.hat"
 
         try:
             hat_file1.Serialize(test_file_name)
             # Deserialize it and verify it has what we expect
             hat_file2 = HATFile.Deserialize(test_file_name)
@@ -61,33 +62,31 @@
             # Remove the file
             os.remove(test_file_name)
 
         # Do basic verification that the deserialized HatFile contains what we
         # specified when we created the HATFile directly
         self.assertEqual(hat_file1.description, hat_file2.description)
         self.assertEqual(hat_file1.dependencies, hat_file2.dependencies)
-        self.assertEqual(hat_file1.compiled_with.to_table(),
-                         hat_file2.compiled_with.to_table())
+        self.assertEqual(hat_file1.compiled_with.to_table(), hat_file2.compiled_with.to_table())
         self.assertTrue("my_function" in hat_file2.function_map)
 
     def test_file_basic_deserialize(self):
         # Load a HAT file from the samples directory
         hat_file1 = HATFile.Deserialize(
-            os.path.join(os.path.dirname(__file__), "..", "..", "samples",
-                         "sample_gemm_library.hat"))
+            os.path.join(os.path.dirname(__file__), "..", "samples", "sample_gemm_library.hat")
+        )
         description = {
             "author": "John Doe",
             "version": "1.2.3.5",
             "license_url": "https://www.apache.org/licenses/LICENSE-2.0.html",
         }
 
         # Do basic verification of known values in the file
         # Verify the description has entries we expect
-        self.assertLessEqual(description.items(),
-                             hat_file1.description.to_table().items())
+        self.assertLessEqual(description.items(), hat_file1.description.to_table().items())
         # Verify the list of functions
         self.assertTrue(len(hat_file1.function_map) == 2)
         self.assertTrue("GEMM_B94D27B9934D3E08" in hat_file1.function_map)
         self.assertTrue("blas_sgemm_row_major" in hat_file1.function_map)
 
 
 if __name__ == '__main__':
```

### Comparing `hatlib-0.0.8/hatlib/verify_hat_package.py` & `hatlib-0.0.9/hatlib/verify_hat_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 #!/usr/bin/env python3
 
 import argparse
 from ast import arg
 import enum
 import sys
 
-if __package__:
-    from . import hat
-else:
-    import hat
+from . import hat
 
 
 def verify_hat_package(hat_path):
     funcs = hat.load(hat_path)
     inputs = hat.generate_input_sets_for_hat_file(hat_path)
     for name, fn in funcs.items():
         print(f"Verifying function {name} --")
         func_inputs = inputs[name]
 
         print("Inputs before function call:")
         for i, func_input in enumerate(func_inputs):
-            print(
-                f"\tInput {i}: {','.join(map(str, func_input.flatten()[:32]))}"
-            )
+            print(f"\tInput {i}: {','.join(map(str, func_input.ravel()[:32]))}")
 
         fn(*inputs[name])
 
         print("Inputs after function call:")
         for i, func_input in enumerate(func_inputs):
-            print(
-                f"\tInput {i}: {','.join(map(str, func_input.flatten()[:32]))}"
-            )
+            print(f"\tInput {i}: {','.join(map(str, func_input.ravel()[:32]))}")
 
 
 def main():
     arg_parser = argparse.ArgumentParser(
-        description="Executes every available function in the hat package \
-            with randomized inputs. Meant for quick verification.\n"
-        "Example:\n"
-        "    hatlib.verify_hat_package <hat_path>\n")
-
-    arg_parser.add_argument("hat_path",
-                            help="Path to the HAT file",
-                            default=None)
+        description=(
+            "Executes every available function in the hat package with randomized inputs. Meant for quick verification.\n"
+            "Example:\n"
+            "    hatlib.verify_hat_package <hat_path>\n"
+        )
+    )
+
+    arg_parser.add_argument("hat_path", help="Path to the HAT file", default=None)
 
     args = vars(arg_parser.parse_args())
     verify_hat_package(args["hat_path"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hatlib-0.0.8/hatlib.egg-info/PKG-INFO` & `hatlib-0.0.9/hatlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: hatlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for HAT (Header Annotated with TOML) packages
+Home-page: https://www.github.com/microsoft/hat
 Author: Microsoft Research AI Compilers Team
 Author-email: mlodev@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

#### html2text {}

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1 Name: hatlib Version: 0.0.8 Summary: Tools for HAT
-(Header Annotated with TOML) packages Author: Microsoft Research AI Compilers
-Team Author-email: mlodev@microsoft.com License: UNKNOWN Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-C++ Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: ~=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE ![HAT](https://upload.wikimedia.org/
-wikipedia/commons/8/80/Crystal_Project_wizard.png) [PyPI_package_version]
-[Python_versions] ![MIT License](https://img.shields.io/pypi/l/hatlib) # HAT
-file format HAT is a format for packaging compiled libraries in the C
-programming language. HAT stands for "**H**eader **A**nnotated with **T**OML",
-and implies that standard C header files are decorated with useful metadata in
-the [TOML](https://toml.io/) markup language. A HAT package includes one
-library file and one or more `.hat` files. The library file can be a static
-library (a `.a` file on Posix systems or a `.lib` file on Windows systems) or a
-dynamic library (a `.so` file on Posix systems or a `.dll` file and its
-accompanying `.lib` import library file on Windows systems). For simplicity of
-documentation, when discussing the "library file" as a unit in a HAT package we
-are referring to either the single static library file (`.a` or `.lib`), the
-single dynamic library file (`.so`) on Posix, or the pair of library files that
-comprise a dynamic library on Windows (`.dll` and `.lib` import library file).
-Note that since a HAT package includes only one "library file" it cannot
-contain both a static and dynamic library, so in the case of a HAT package
-containing a Windows dynamic library, the `.lib` file in the package is always
-the import library and there is no ambiguity in which file (or pair of files)
-is being referenced by "library file". The library file contains all the
-compiled object code that implements the functions in the HAT package. Each
-`.hat` file contains a combination of standard C function declarations (like a
-typical `.h` file) and metadata in the TOML markup language. The metadata that
-accompanies each function declaration describes how the function should be
-called and how it was implemented. The metadata is intended to be both human-
-readable and machine-readable, providing structured and systematic
-documentation and allowing downstream tools to examine the package contents.
-Each `.hat` file has the convenient property that it is simultaneously a valid
-h-file and a valid TOML file. In other words, the file is structured such that
-a C compiler will ignore the TOML metadata, while a TOML parser will understand
-the entire file as a valid TOML file. We accomplish this using a technique we
-call *the hat trick*, which is explained below. # What problem does the HAT
-format solve? C is among the most popular programming languages, but it also
-has serious shortcomings. In particular, C libraries are typically opaque and
-lack mechanisms for systematic documentation and introspection. This is best
+Metadata-Version: 2.1 Name: hatlib Version: 0.0.9 Summary: Tools for HAT
+(Header Annotated with TOML) packages Home-page: https://www.github.com/
+microsoft/hat Author: Microsoft Research AI Compilers Team Author-email:
+mlodev@microsoft.com License: UNKNOWN Platform: UNKNOWN Classifier: License ::
+OSI Approved :: MIT License Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Programming Language :: C++ Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: ~=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE ![HAT](https://upload.wikimedia.org/wikipedia/commons/8/
+80/Crystal_Project_wizard.png) [PyPI_package_version] [Python_versions] ![MIT
+License](https://img.shields.io/pypi/l/hatlib) # HAT file format HAT is a
+format for packaging compiled libraries in the C programming language. HAT
+stands for "**H**eader **A**nnotated with **T**OML", and implies that standard
+C header files are decorated with useful metadata in the [TOML](https://
+toml.io/) markup language. A HAT package includes one library file and one or
+more `.hat` files. The library file can be a static library (a `.a` file on
+Posix systems or a `.lib` file on Windows systems) or a dynamic library (a
+`.so` file on Posix systems or a `.dll` file and its accompanying `.lib` import
+library file on Windows systems). For simplicity of documentation, when
+discussing the "library file" as a unit in a HAT package we are referring to
+either the single static library file (`.a` or `.lib`), the single dynamic
+library file (`.so`) on Posix, or the pair of library files that comprise a
+dynamic library on Windows (`.dll` and `.lib` import library file). Note that
+since a HAT package includes only one "library file" it cannot contain both a
+static and dynamic library, so in the case of a HAT package containing a
+Windows dynamic library, the `.lib` file in the package is always the import
+library and there is no ambiguity in which file (or pair of files) is being
+referenced by "library file". The library file contains all the compiled object
+code that implements the functions in the HAT package. Each `.hat` file
+contains a combination of standard C function declarations (like a typical `.h`
+file) and metadata in the TOML markup language. The metadata that accompanies
+each function declaration describes how the function should be called and how
+it was implemented. The metadata is intended to be both human-readable and
+machine-readable, providing structured and systematic documentation and
+allowing downstream tools to examine the package contents. Each `.hat` file has
+the convenient property that it is simultaneously a valid h-file and a valid
+TOML file. In other words, the file is structured such that a C compiler will
+ignore the TOML metadata, while a TOML parser will understand the entire file
+as a valid TOML file. We accomplish this using a technique we call *the hat
+trick*, which is explained below. # What problem does the HAT format solve? C
+is among the most popular programming languages, but it also has serious
+shortcomings. In particular, C libraries are typically opaque and lack
+mechanisms for systematic documentation and introspection. This is best
 explained with an example: Say that we use C to implement an in-place column-
 wise normalization of a 10x10 matrix. In other words, this function takes a
 10x10 matrix `A` and divides each column by the Euclidean norm of that column.
 A highly-optimized implementation of this function would be tailored to the
 target computer's specific hardware properties, such as its cache size, the
 number of CPU cores, and perhaps even the presence of a GPU. The declaration of
 this function in an h-file would look something like this: ``` void normalize
```

### Comparing `hatlib-0.0.8/hatlib.egg-info/SOURCES.txt` & `hatlib-0.0.9/hatlib.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 hatlib/gpu_headers.py
 hatlib/hat.py
 hatlib/hat_file.py
 hatlib/hat_package.py
 hatlib/hat_to_dynamic.py
 hatlib/hat_to_lib.py
 hatlib/platform_utilities.py
-hatlib/pyhip_hip.py
-hatlib/pyhip_hiprtc.py
 hatlib/requirements.txt
 hatlib/rocm_loader.py
 hatlib/verify_hat_package.py
 hatlib.egg-info/PKG-INFO
 hatlib.egg-info/SOURCES.txt
 hatlib.egg-info/dependency_links.txt
 hatlib.egg-info/entry_points.txt
 hatlib.egg-info/requires.txt
 hatlib.egg-info/top_level.txt
-hatlib/test/__init__.py
-hatlib/test/requirements.txt
-hatlib/test/test_benchmark_hat_package.py
-hatlib/test/test_hat.py
-hatlib/test/test_hat_file.py
-hatlib/test/test_hat_package.py
+hatlib/pyhip/__init__.py
+hatlib/pyhip/hip.py
+hatlib/pyhip/hiprtc.py
 samples/sample_gemm_library.hat
-schema/hat.tosd
+schema/hat.tosd
+test/__init__.py
+test/requirements.txt
+test/test_benchmark_hat_package.py
+test/test_hat.py
+test/test_hat_file.py
+test/test_hat_package.py
```

### Comparing `hatlib-0.0.8/samples/sample_gemm_library.hat` & `hatlib-0.0.9/samples/sample_gemm_library.hat`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/schema/hat.tosd` & `hatlib-0.0.9/schema/hat.tosd`

 * *Files identical despite different names*

### Comparing `hatlib-0.0.8/setup.cfg` & `hatlib-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = hatlib
 author = Microsoft Research AI Compilers Team
 author_email = mlodev@microsoft.com
 summary = Tools for HAT (Header Annotated with TOML) packages
+url = https://www.github.com/microsoft/hat
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 	Topic :: Software Development
@@ -16,28 +17,35 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
-packages = hatlib
 python_requires = ~=3.7
 install_requires = 
 	numpy
 	pandas
 	toml
 	tomlkit
 	vswhere; sys_platform == "win32"
 package_dir = 
 	hatlib = hatlib
+packages = find:
+
+[options.packages.find]
+exclude = 
+	test*
 
 [options.entry_points]
 console_scripts = 
 	hatlib.benchmark_hat = hatlib.benchmark_hat_package:main_command
 	hatlib.hat_to_dynamic = hatlib.hat_to_dynamic:main
 	hatlib.verify_hat = hatlib.verify_hat_package:main
 
+[pycodestyle]
+max-line-length = 120
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

