# Comparing `tmp/jax-chacha-prng-1.4.0.post1.tar.gz` & `tmp/jax-chacha-prng-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-chacha-prng-1.4.0.post1.tar", last modified: Fri Feb  3 08:09:12 2023, max compression
+gzip compressed data, was "jax-chacha-prng-1.4.1.tar", last modified: Mon May  8 08:00:47 2023, max compression
```

## Comparing `jax-chacha-prng-1.4.0.post1.tar` & `jax-chacha-prng-1.4.1.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.049123 jax-chacha-prng-1.4.0.post1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/LICENSES/LLVM-exception.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/LICENSES/LicenseRef-pybind11License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.049123 jax-chacha-prng-1.4.0.post1/chacha/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/chacha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/chacha/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/chacha/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/chacha/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/chacha/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/chacha/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.049123 jax-chacha-prng-1.4.0.post1/cmake_config/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/cmake_config/neon_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/cmake_config/sse_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.045123 jax-chacha-prng-1.4.0.post1/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.049123 jax-chacha-prng-1.4.0.post1/extern/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.045123 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.053123 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65638 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.053123 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    50369 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    25057 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    32147 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79524 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125761 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    93848 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.053123 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.053123 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-02-03 08:08:55.000000 jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-02-03 08:09:12.000000 jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-03 08:09:12.000000 jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 08:09:12.000000 jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 08:09:12.000000 jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-03 08:09:12.000000 jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/lib/arm/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/arm/cpu_kernel_arch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/chacha_kernels.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/cpu_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/cpu_kernel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/defs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/lib/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/generic/cpu_kernel_arch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/gpu_kernel.cpp.cu
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/gpu_kernel.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/lib/intel/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/intel/cpu_kernel_arch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/lib/python_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 08:09:12.057123 jax-chacha-prng-1.4.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-03 08:08:54.000000 jax-chacha-prng-1.4.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.448313 jax-chacha-prng-1.4.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/LICENSES/LLVM-exception.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/LICENSES/LicenseRef-pybind11License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.448313 jax-chacha-prng-1.4.1/chacha/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/chacha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/chacha/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/chacha/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/chacha/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/chacha/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/chacha/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.448313 jax-chacha-prng-1.4.1/cmake_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/cmake_config/neon_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/cmake_config/sse_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.448313 jax-chacha-prng-1.4.1/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.448313 jax-chacha-prng-1.4.1/extern/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.448313 jax-chacha-prng-1.4.1/extern/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.452313 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65638 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.452313 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50369 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25057 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32147 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79524 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125761 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93848 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.452313 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/extern/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-08 08:00:36.000000 jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-08 08:00:47.000000 jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-08 08:00:47.000000 jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:00:47.000000 jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 08:00:47.000000 jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 08:00:47.000000 jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/lib/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/arm/cpu_kernel_arch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/chacha_kernels.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/cpu_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/cpu_kernel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/defs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/lib/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/generic/cpu_kernel_arch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/gpu_kernel.cpp.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/gpu_kernel.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/lib/intel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/intel/cpu_kernel_arch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/lib/python_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:00:47.456313 jax-chacha-prng-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 08:00:34.000000 jax-chacha-prng-1.4.1/tests/testconfig.py
```

### Comparing `jax-chacha-prng-1.4.0.post1/CMakeLists.txt` & `jax-chacha-prng-1.4.1/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-FileCopyrightText: © 2022 Aalto University
 
 cmake_minimum_required(VERSION 3.18)
 project(jax-chacha20-prng LANGUAGES CXX)
 
 option(BUILD_TESTING "Build tests for native kernels" OFF)
 option(FORCE_GENERIC "Build without CPU architecture optimized instructions" OFF)
+option(DISABLE_OPENMP "Do not use OpenMP parallelisation for CPU kernels" OFF)
 
 set(CMAKE_CXX_STANDARD 14)
 set(cpu_arch_path "${CMAKE_CURRENT_LIST_DIR}/lib/generic/")
 set(cpu_arch_def "ARCH_GENERIC")
 set(SSE_ENABLED "No")
 set(NEON_ENABLED "No")
 
@@ -98,19 +99,23 @@
     message(FATAL_ERROR "The pybind11 repository was not downloaded! Please run manually: git submodule update --init --recursive .")
 endif()
 
 find_package(Python3 COMPONENTS Interpreter Development.Module REQUIRED)
 add_subdirectory(extern/pybind11)
 # find_package(pybind11 REQUIRED) # broken; does not use correct Python interpreter/libraries in a conda env
 
-find_package(OpenMP)
-if(OpenMP_CXX_FOUND)
-    add_compile_definitions(OPENMP_AVAILABLE)
+if(NOT DISABLE_OPENMP)
+    find_package(OpenMP)
+    if(OpenMP_CXX_FOUND)
+        add_compile_definitions(OPENMP_AVAILABLE)
+    else()
+        message(WARNING "OpenMP not found - Compiling without, but you may see lower performance.")
+    endif()
 else()
-    message(WARNING "OpenMP not found - Compiling without, but you may see lower performance.")
+    message("-- OpenMP disabled by user")
 endif()
 
 include_directories(${CMAKE_CURRENT_LIST_DIR}/lib)
 
 pybind11_add_module(
     native
     ${CMAKE_CURRENT_LIST_DIR}/lib/cpu_kernel.cpp
```

### Comparing `jax-chacha-prng-1.4.0.post1/LICENSES/Apache-2.0.txt` & `jax-chacha-prng-1.4.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/LICENSES/CC0-1.0.txt` & `jax-chacha-prng-1.4.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/LICENSES/GPL-3.0-only.txt` & `jax-chacha-prng-1.4.1/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/LICENSES/LLVM-exception.txt` & `jax-chacha-prng-1.4.1/LICENSES/LLVM-exception.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/LICENSES/LicenseRef-pybind11License.txt` & `jax-chacha-prng-1.4.1/LICENSES/LicenseRef-pybind11License.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/LICENSES/MIT.txt` & `jax-chacha-prng-1.4.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/PKG-INFO` & `jax-chacha-prng-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-chacha-prng
-Version: 1.4.0.post1
+Version: 1.4.1
 Summary: A pseudo-random number generator for JAX based on the 20 round ChaCha cipher.
 Home-page: https://github.com/DPBayes/jax-chacha-prng
 Author: Lukas Prediger, Aalto University
 Author-email: lukas.m.prediger@aalto.fi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `jax-chacha-prng-1.4.0.post1/README.md` & `jax-chacha-prng-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/chacha/cipher.py` & `jax-chacha-prng-1.4.1/chacha/cipher.py`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/chacha/defs.py` & `jax-chacha-prng-1.4.1/chacha/defs.py`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/chacha/jax_ops.py` & `jax-chacha-prng-1.4.1/chacha/jax_ops.py`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/chacha/random.py` & `jax-chacha-prng-1.4.1/chacha/random.py`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/cmake_config/neon_test.cpp` & `jax-chacha-prng-1.4.1/cmake_config/neon_test.cpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/cmake_config/sse_test.cpp` & `jax-chacha-prng-1.4.1/cmake_config/sse_test.cpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/CMakeLists.txt` & `jax-chacha-prng-1.4.1/extern/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/attr.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/buffer_info.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/cast.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/chrono.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/complex.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/class.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/common.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/descr.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/init.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/internals.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/type_caster_base.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/detail/typeid.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/eigen.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/embed.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/eval.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/functional.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/gil.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/iostream.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/numpy.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/operators.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/options.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/pybind11.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/pytypes.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl/filesystem.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/include/pybind11/stl_bind.h` & `jax-chacha-prng-1.4.1/extern/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/FindCatch.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/FindEigen3.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/FindPythonLibsNew.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/JoinPaths.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/cmake_uninstall.cmake.in` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11Common.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11Config.cmake.in` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11NewTools.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/extern/pybind11/tools/pybind11Tools.cmake` & `jax-chacha-prng-1.4.1/extern/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/PKG-INFO` & `jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-chacha-prng
-Version: 1.4.0.post1
+Version: 1.4.1
 Summary: A pseudo-random number generator for JAX based on the 20 round ChaCha cipher.
 Home-page: https://github.com/DPBayes/jax-chacha-prng
 Author: Lukas Prediger, Aalto University
 Author-email: lukas.m.prediger@aalto.fi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `jax-chacha-prng-1.4.0.post1/jax_chacha_prng.egg-info/SOURCES.txt` & `jax-chacha-prng-1.4.1/jax_chacha_prng.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CMakeLists.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 LICENSES/Apache-2.0.txt
 LICENSES/CC0-1.0.txt
 LICENSES/GPL-3.0-only.txt
 LICENSES/LLVM-exception.txt
 LICENSES/LicenseRef-pybind11License.txt
 LICENSES/MIT.txt
@@ -63,8 +64,9 @@
 lib/cpu_kernel.hpp
 lib/defs.hpp
 lib/gpu_kernel.cpp.cu
 lib/gpu_kernel.hpp
 lib/python_bindings.cpp
 lib/arm/cpu_kernel_arch.hpp
 lib/generic/cpu_kernel_arch.hpp
-lib/intel/cpu_kernel_arch.hpp
+lib/intel/cpu_kernel_arch.hpp
+tests/testconfig.py
```

### Comparing `jax-chacha-prng-1.4.0.post1/lib/arm/cpu_kernel_arch.hpp` & `jax-chacha-prng-1.4.1/lib/arm/cpu_kernel_arch.hpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/cpu_kernel.cpp` & `jax-chacha-prng-1.4.1/lib/cpu_kernel.cpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/cpu_kernel.hpp` & `jax-chacha-prng-1.4.1/lib/cpu_kernel.hpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/defs.hpp` & `jax-chacha-prng-1.4.1/lib/defs.hpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/generic/cpu_kernel_arch.hpp` & `jax-chacha-prng-1.4.1/lib/generic/cpu_kernel_arch.hpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/gpu_kernel.cpp.cu` & `jax-chacha-prng-1.4.1/lib/gpu_kernel.cpp.cu`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/intel/cpu_kernel_arch.hpp` & `jax-chacha-prng-1.4.1/lib/intel/cpu_kernel_arch.hpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/lib/python_bindings.cpp` & `jax-chacha-prng-1.4.1/lib/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `jax-chacha-prng-1.4.0.post1/setup.py` & `jax-chacha-prng-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import setuptools
 from setuptools import Extension
 from setuptools.command.build_ext import build_ext
 import os
 import subprocess
 import re
+import sys
 
 class CMakeBuildExt(build_ext):
     # adapted from https://github.com/dfm/extending-jax
     def build_extensions(self):
 
         install_dir = os.path.abspath(
             os.path.dirname(self.get_ext_fullpath("dummy"))
@@ -20,17 +21,21 @@
         osx_architectures = ";".join(re.findall(r"-arch (\S+)", os.environ.get("ARCHFLAGS", "")))
 
         cmake_args = [
             "-DCMAKE_INSTALL_PREFIX={}".format(install_dir),
             "-DCMAKE_BUILD_TYPE={}".format(
                 "Debug" if self.debug else "Release"
             ),
-            "-DCMAKE_OSX_ARCHITECTURES={}".format(osx_architectures)
+            "-DCMAKE_OSX_ARCHITECTURES={}".format(osx_architectures),
+            "-DPython3_ROOT_DIR={}".format(sys.exec_prefix),
         ]
 
+        if os.environ.get("JAX_CHACHA_PRNG_DISABLE_OPENMP", "0") == "1":
+            cmake_args.append("-DDISABLE_OPENMP=On")
+
         os.makedirs(self.build_temp, exist_ok=True)
 
         HERE = os.path.dirname(os.path.realpath(__file__))
         subprocess.check_call(
             ["cmake", HERE] + cmake_args, cwd=self.build_temp
         )
 
@@ -76,15 +81,15 @@
 import importlib
 spec = importlib.util.spec_from_file_location("version_module", "chacha/version.py")
 version_module = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(version_module)
 
 _jax_version_lower_constraint = ' >= 0.2.12'
 _jax_version_optimistic_upper_constraint = ', <= 2.0.0'
-_jax_version_upper_constraint = ', <= 0.3.25'
+_jax_version_upper_constraint = ', <= 0.4.8'
 
 _version = version_module.VERSION
 if 'JAX_CHACHA_PRNG_BUILD' in os.environ:
     _version += f"+{os.environ['JAX_CHACHA_PRNG_BUILD']}"
 
 setuptools.setup(
     name='jax-chacha-prng',
```

