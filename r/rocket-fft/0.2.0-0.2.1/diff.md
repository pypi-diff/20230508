# Comparing `tmp/rocket-fft-0.2.0.tar.gz` & `tmp/rocket-fft-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocket-fft-0.2.0.tar", last modified: Sun Mar 12 12:40:39 2023, max compression
+gzip compressed data, was "rocket-fft-0.2.1.tar", last modified: Mon May  8 17:09:15 2023, max compression
```

## Comparing `rocket-fft-0.2.0.tar` & `rocket-fft-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:40:39.937715 rocket-fft-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-03-12 12:40:39.937715 rocket-fft-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:40:39.937715 rocket-fft-0.2.0/rocket_fft/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/_pocketfft_numba.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/_special_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/extutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/imputils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34160 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/pocketfft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/rocket_fft/typutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:40:39.937715 rocket-fft-0.2.0/rocket_fft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-03-12 12:40:39.000000 rocket-fft-0.2.0/rocket_fft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-12 12:40:39.000000 rocket-fft-0.2.0/rocket_fft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 12:40:39.000000 rocket-fft-0.2.0/rocket_fft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-12 12:40:39.000000 rocket-fft-0.2.0/rocket_fft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-12 12:40:39.000000 rocket-fft-0.2.0/rocket_fft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-12 12:40:39.000000 rocket-fft-0.2.0/rocket_fft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 12:40:39.937715 rocket-fft-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:40:39.937715 rocket-fft-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_fftlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_low_level_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_multithreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_numpy_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_numpy_testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_overwrite_and_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_scipy_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    58791 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_scipy_testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-03-12 12:40:18.000000 rocket-fft-0.2.0/tests/test_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:09:15.422398 rocket-fft-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-08 17:08:53.000000 rocket-fft-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-08 17:09:15.418398 rocket-fft-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-08 17:08:53.000000 rocket-fft-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:09:15.418398 rocket-fft-0.2.1/rocket_fft/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/_pocketfft_numba.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/_special_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/extutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/imputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35109 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/pocketfft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/rocket_fft/typutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:09:15.418398 rocket-fft-0.2.1/rocket_fft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-08 17:09:15.000000 rocket-fft-0.2.1/rocket_fft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 17:09:15.000000 rocket-fft-0.2.1/rocket_fft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:09:15.000000 rocket-fft-0.2.1/rocket_fft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 17:09:15.000000 rocket-fft-0.2.1/rocket_fft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 17:09:15.000000 rocket-fft-0.2.1/rocket_fft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 17:09:15.000000 rocket-fft-0.2.1/rocket_fft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:09:15.422398 rocket-fft-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:09:15.418398 rocket-fft-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_fftlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_low_level_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_multithreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_numpy_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_numpy_testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_overwrite_and_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_scipy_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58791 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_scipy_testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-05-08 17:08:54.000000 rocket-fft-0.2.1/tests/test_typing.py
```

### Comparing `rocket-fft-0.2.0/LICENSE` & `rocket-fft-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/PKG-INFO` & `rocket-fft-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: rocket-fft
-Version: 0.2.0
+Version: 0.2.1
 Summary: Rocket-FFT extends Numba by scipy.fft and numpy.fft
 Home-page: https://github.com/styfenschaer/rocket-fft
 Download-URL: https://github.com/styfenschaer/rocket-fft
 Author: Styfen Schär
 Author-email: styfen.schaer.blog@gmail.com
 License: BSD
 Keywords: FFT,Fourier,Numba,SciPy,NumPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -26,17 +27,17 @@
 # Rocket-FFT
 [![PyPI version](https://img.shields.io/pypi/v/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![License](https://img.shields.io/pypi/l/rocket-fft?color=%2376519B)](https://opensource.org/licenses/BSD-3-Clause)
 [![python](https://img.shields.io/pypi/pyversions/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![status](https://img.shields.io/pypi/status/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![downloads](https://img.shields.io/pypi/dm/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 
-![](https://raw.githubusercontent.com/styfenschaer/rocket-fft/release0.2.0/assets/fourier.gif)
+![](https://raw.githubusercontent.com/styfenschaer/rocket-fft/release0.2.1/assets/fourier.gif)
 
-Rocket-FFT makes [Numba](https://numba.pydata.org/) aware of `numpy.fft` and `scipy.fft`. It takes its name from the [PocketFFT](https://github.com/hayguen/pocketfft) Fast Fourier Transformation library that powers it, and Numba's goal of making your scientific Python code blazingly fast - like a rocket. 
+Rocket-FFT makes [Numba](https://numba.pydata.org/) aware of `numpy.fft` and `scipy.fft`. It takes its name from the [PocketFFT](https://github.com/mreineck/pocketfft) Fast Fourier Transformation library that powers it, and Numba's goal of making your scientific Python code blazingly fast - like a rocket. 
 
 ## Getting Started
 The easiest way to get Rocket-FFT is to:
 ```
 $ pip install rocket-fft
 ```
 Alternatively, you can build it from source:
@@ -95,8 +96,8 @@
 def dct(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], type: i8, fct: f4 | f8, ortho: b1, nthreads: i8) -> None: ...
 def r2r_separable_hartley(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], fct: f4 | f8, nthreads: i8) -> None: ...
 def r2r_genuine_hartley(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], fct: f4 | f8, nthreads: i8) -> None: ...
 def r2r_fftpack(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], real2hermitian: b1, forward: b1, fct: f4 | f8, nthreads: i8) -> None: ...
 def good_size(target: i8, real: b1) -> i8: ...
 ```
 Note that the low-level interface provides a lower level of safety and convenience compared to the SciPy-like and NumPy-like interfaces. 
-There is almost no safety net, and it is up to the user to ensure proper usage. You may want to consult the original [PocketFFT](https://github.com/hayguen/pocketfft) C++ implementation before using it.
+There is almost no safety net, and it is up to the user to ensure proper usage. You may want to consult the original [PocketFFT](https://github.com/mreineck/pocketfft) C++ implementation before using it.
```

### Comparing `rocket-fft-0.2.0/README.md` & `rocket-fft-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Rocket-FFT
 [![PyPI version](https://img.shields.io/pypi/v/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![License](https://img.shields.io/pypi/l/rocket-fft?color=%2376519B)](https://opensource.org/licenses/BSD-3-Clause)
 [![python](https://img.shields.io/pypi/pyversions/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![status](https://img.shields.io/pypi/status/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![downloads](https://img.shields.io/pypi/dm/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 
-![](https://raw.githubusercontent.com/styfenschaer/rocket-fft/release0.2.0/assets/fourier.gif)
+![](https://raw.githubusercontent.com/styfenschaer/rocket-fft/release0.2.1/assets/fourier.gif)
 
-Rocket-FFT makes [Numba](https://numba.pydata.org/) aware of `numpy.fft` and `scipy.fft`. It takes its name from the [PocketFFT](https://github.com/hayguen/pocketfft) Fast Fourier Transformation library that powers it, and Numba's goal of making your scientific Python code blazingly fast - like a rocket. 
+Rocket-FFT makes [Numba](https://numba.pydata.org/) aware of `numpy.fft` and `scipy.fft`. It takes its name from the [PocketFFT](https://github.com/mreineck/pocketfft) Fast Fourier Transformation library that powers it, and Numba's goal of making your scientific Python code blazingly fast - like a rocket. 
 
 ## Getting Started
 The easiest way to get Rocket-FFT is to:
 ```
 $ pip install rocket-fft
 ```
 Alternatively, you can build it from source:
@@ -70,8 +70,8 @@
 def dct(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], type: i8, fct: f4 | f8, ortho: b1, nthreads: i8) -> None: ...
 def r2r_separable_hartley(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], fct: f4 | f8, nthreads: i8) -> None: ...
 def r2r_genuine_hartley(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], fct: f4 | f8, nthreads: i8) -> None: ...
 def r2r_fftpack(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], real2hermitian: b1, forward: b1, fct: f4 | f8, nthreads: i8) -> None: ...
 def good_size(target: i8, real: b1) -> i8: ...
 ```
 Note that the low-level interface provides a lower level of safety and convenience compared to the SciPy-like and NumPy-like interfaces. 
-There is almost no safety net, and it is up to the user to ensure proper usage. You may want to consult the original [PocketFFT](https://github.com/hayguen/pocketfft) C++ implementation before using it.
+There is almost no safety net, and it is up to the user to ensure proper usage. You may want to consult the original [PocketFFT](https://github.com/mreineck/pocketfft) C++ implementation before using it.
```

### Comparing `rocket-fft-0.2.0/rocket_fft/__init__.py` & `rocket-fft-0.2.1/rocket_fft/__init__.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/rocket_fft/__init__.pyi` & `rocket-fft-0.2.1/rocket_fft/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -8,107 +8,107 @@
     ain: Union[NDArray[complex64], NDArray[complex128]],
     aout: Union[NDArray[complex64], NDArray[complex128]],
     axes: NDArray[int64],
     forward: bool8,
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def r2c(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[complex64], NDArray[complex128]],
     axes: NDArray[int64],
     forward: bool8,
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def c2r(
     ain: Union[NDArray[complex64], NDArray[complex128]],
     aout: Union[NDArray[float32], NDArray[float64]],
     axes: NDArray[int64],
     forward: bool8,
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def c2c_sym(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[complex64], NDArray[complex128]],
     axes: NDArray[int64],
     forward: bool8,
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
     """Similar to c2c, but takes a real-valued input array. 
     It uses symmetry to speed up the calculation.
-    Please refer to https://github.com/hayguen/pocketfft for documentation.
+    Please refer to https://github.com/mreineck/pocketfft for documentation.
     """
 
 
 def dst(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[float32], NDArray[float64]],
     axes: NDArray[int64],
     type: int64,
     fct: Union[float32, float64],
     ortho: bool8,
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def dct(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[float32], NDArray[float64]],
     axes: NDArray[int64],
     type: int64,
     fct: Union[float32, float64],
     ortho: bool8,
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def r2r_separable_hartley(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[float32], NDArray[float64]],
     axes: NDArray[int64],
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def r2r_genuine_hartley(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[float32], NDArray[float64]],
     axes: NDArray[int64],
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 def r2r_fftpack(
     ain: Union[NDArray[float32], NDArray[float64]],
     aout: Union[NDArray[float32], NDArray[float64]],
     axes: NDArray[int64],
     real2hermitian: bool8,
     forward: bool8,
     fct: Union[float32, float64],
     nthreads: int64
 ) -> None:
-    """Please refer to https://github.com/hayguen/pocketfft for documentation."""
+    """Please refer to https://github.com/mreineck/pocketfft for documentation."""
 
 
 separable_hartley = r2r_separable_hartley
 genuine_hartley = r2r_genuine_hartley
 fftpack = r2r_fftpack
```

### Comparing `rocket-fft-0.2.0/rocket_fft/_pocketfft_numba.cpp` & `rocket-fft-0.2.1/rocket_fft/_pocketfft_numba.cpp`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/rocket_fft/_special_helpers.cpp` & `rocket-fft-0.2.1/rocket_fft/_special_helpers.cpp`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/rocket_fft/extutils.py` & `rocket-fft-0.2.1/rocket_fft/extutils.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/rocket_fft/imputils.py` & `rocket-fft-0.2.1/rocket_fft/imputils.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/rocket_fft/overloads.py` & `rocket-fft-0.2.1/rocket_fft/overloads.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 from numba.cpython.unsafe.tuple import tuple_setitem
 from numba.extending import overload, register_jitable
 from numba.np.numpy_support import is_nonelike
 
 from . import pocketfft
 from . import typutils as tu
 from .imputils import implements_jit, implements_overload, otherwise
-from .typutils import (is_integer, is_integer_2tuple, is_literal_bool,
-                       is_literal_integer, is_nonelike, is_not_nonelike,
-                       typing_check)
+from .typutils import (is_contiguous_array, is_integer, is_integer_2tuple,
+                       is_literal_bool, is_literal_integer, is_nonelike,
+                       is_not_nonelike, is_scalar, typing_check)
 
 # Unlike NumPy, SciPy is an optional runtime dependency
 try:
     import scipy.fft
+
     from . import special
     _scipy_installed_ = True
 except ImportError:
     _scipy_installed_ = False
 
 # SciPy and NumPy differ in when they convert types and handle duplicate axes.
 # These functions mimic their behavior. They must be called before the compilation
@@ -202,15 +203,15 @@
             axes[i] += x.ndim
 
 # NumPy allows passing duplicate axes for fft2, fftn, ifft2 and ifft
 # while SciPy doesn't
 
 @register_jitable(locals={"slots": types.UniTuple(types.byte, 32)})
 def _scipy_assert_unique_axes(axes):
-    slots = (0,) * 32  # maximum ndim of ndarray
+    slots = (0,) * 32  # np.MAXDIMS
     for ax in axes:
         if slots[ax] != 0:
             raise ValueError("All axes must be unique.")
         slots = tuple_setitem(slots, ax, 1)
 
 
 @register_jitable
@@ -772,91 +773,123 @@
     _common_dst = dict(trafo=pocketfft.numba_dst, delta=1)
     scipy_r1d_builder(r2rn, **_common_dst, forward=True).overload(scipy.fft.dst)
     scipy_rnd_builder(r2rn, **_common_dst, forward=True).overload(scipy.fft.dstn)
     scipy_r1d_builder(r2rn, **_common_dst, forward=False).overload(scipy.fft.idst)
     scipy_rnd_builder(r2rn, **_common_dst, forward=False).overload(scipy.fft.idstn)
 
 
+def _get_slice_tuple(arr):
+    pass 
+
+
+@overload(_get_slice_tuple)
+def _get_slice_tuple_impl(arr):
+    tup = (slice(None),) * arr.ndim
+    return lambda arr: tup
+
+
+@register_jitable
+def _roll_core_impl(a, shift, axis):
+    axis, shift = np.broadcast_arrays(axis, shift)
+
+    shifts = {ax: 0 for ax in range(a.ndim)}
+    for ax, sh in zip(axis, shift):
+        if (ax >= a.ndim) or (ax < -a.ndim):
+            raise ValueError("axis is out of bounds")
+        if ax < 0:
+            ax += a.ndim
+        shifts[ax] += sh
+
+    n_sclices = a.shape
+    out_slices = [(slice(None), slice(None))] * a.ndim
+    arr_slices = [(slice(None), slice(None))] * a.ndim
+    for ax, sh in shifts.items():
+        sh %= a.shape[ax] or 1
+        n_sclices = tuple_setitem(n_sclices, ax, (2 if sh else 1))
+        if sh:
+            out_slices[ax] = (slice(None, sh), slice(sh, None))
+            arr_slices[ax] = (slice(-sh, None), slice(None, -sh))
+
+    out = np.empty(a.shape, dtype=a.dtype)
+
+    arr_index = _get_slice_tuple(a)
+    out_index = _get_slice_tuple(a)
+    for index in np.ndindex(n_sclices):
+        for ax, i in enumerate(index):
+            arr_index = tuple_setitem(arr_index, ax, arr_slices[ax][i])
+            out_index = tuple_setitem(out_index, ax, out_slices[ax][i])
+
+        out[out_index] = a[arr_index]
+
+    return out
+
+
 @implements_overload(np.roll)
 def roll(a, shift, axis=None):
-    # TODO: Make multidimensional case more efficient!
-    typing_check(types.Array)(a, "The 1st argument 'a' must be an array.")
-    typing_check(types.Integer, as_seq=True)(
+    typing_check((types.Number, types.Boolean), as_seq=True)(
+        a, "The 1st argument 'a' must be array-like.")
+    typing_check((types.Integer, types.Boolean), as_seq=True)(
         shift, ("The 2nd argument 'shift' must be a"
                 " sequence of integers or an integer."))
-    typing_check(types.Integer, as_seq=True, allow_none=True)(
-        axis, ("The 3rd argument 'axis' must be a"
+    typing_check((types.Integer, types.Boolean), as_seq=True, allow_none=True)(
+        axis, ("If specified, the 3rd argument 'axis' must be a"
                " sequence of integers or an integer."))
 
+                     
+@roll.impl(a=is_scalar)
+def _(a, shift, axis=None):
+    return np.asarray(a)
+
 
 @roll.impl(axis=is_nonelike)
 def _(a, shift, axis=None):
-    r = np.empty(a.shape, dtype=a.dtype)
-    if a.size == 0:
-        return r
+    arr = np.asarray(a)
+    out = np.empty(arr.shape, dtype=arr.dtype)
+
+    shift = np.asarray(shift)
+    if shift.ndim > 1:
+        ValueError("'shift' must be scalars or 1D sequence")
+        
+    sh = shift.sum() % (arr.size or 1)
+    inv_sh = arr.size - sh
     
-    if a.size == 1:
-        r[0] = a[0]
-        return r
+    for i in range(inv_sh):
+        out.flat[sh + i] = arr.flat[i]
+    for i in range(sh):
+        out.flat[i] = arr.flat[inv_sh + i]
     
-    sh = np.asarray(shift).sum() % a.size
-    r_flat = r.ravel()
-    a_flat = a.ravel()
-    r_flat[sh:] = a_flat[:-sh]
-    r_flat[:sh] = a_flat[-sh:]
-    return r
+    return out
 
 
-@roll.impl(otherwise)
+@roll.impl(a=is_contiguous_array(layout="C"))
 def _(a, shift, axis=None):
-    axis, shift = np.broadcast_arrays(axis, shift)
-    # Axis is readonly but we eventually need to write it
-    axis = axis.copy()
-    wraparound_axes(a, axis)
-
-    a_index = a.shape
-    for i in range(a.ndim):
-        a_index = tuple_setitem(a_index, i, 0)
+    return _roll_core_impl(a, shift, axis)
 
-    r_index = a_index
-    for ax, sh in zip(axis, shift):
-        r_index = tuple_setitem(r_index, ax, r_index[ax] + sh)
 
-    for i in range(a.ndim):
-        if a.shape[i] == 0:
-            r_index = tuple_setitem(r_index, i, 0)
-        elif r_index[i] > 0:
-            val = (r_index[i] % a.shape[i]) - a.shape[i]
-            r_index = tuple_setitem(r_index, i, val)
-
-    r_index_init = r_index
-
-    r = np.empty(a.shape, dtype=a.dtype)
-    if r.size == 0:
-        return r
-
-    # Like np.ndindex but maintains two index tuples
-    # in parallel; a normal one and a shifted one
-    done = False
-    while not done:
-        r[r_index] = a[a_index]
-
-        done = True
-        for i in range(a.ndim):
-            r_index = tuple_setitem(r_index, i, r_index[i] + 1)
-            a_index = tuple_setitem(a_index, i, a_index[i] + 1)
-
-            if a_index[i] < a.shape[i]:
-                done = False
-                break
+@register_jitable
+def _transpose_axes(axis, ndim):
+    axis = np.atleast_1d(np.asarray(axis))
+    return np.array([(ndim - ax - 1) % ndim for ax in axis])
+
+
+@roll.impl(a=is_contiguous_array(layout="F"))
+def _(a, shift, axis=None):
+    axis = _transpose_axes(axis, a.ndim)
+    return _roll_core_impl(a.T, shift, axis).T
 
-            r_index = tuple_setitem(r_index, i, r_index_init[i])
-            a_index = tuple_setitem(a_index, i, 0)
 
-    return r
+@roll.impl(otherwise)
+def _(a, shift, axis=None):
+    arr = np.asarray(a)
+    
+    if arr.strides[0] >= arr.strides[-1]:
+        return _roll_core_impl(arr, shift, axis)
+
+    axis = _transpose_axes(axis, arr.ndim)
+    return _roll_core_impl(arr.T, shift, axis).T
 
 
 fftshift_typing = tu.TypingChecker(
     x=tu.Check(
         types.Array,
         msg="The {} argument '{}' must be an array."),
     axes=tu.Check(
@@ -959,21 +992,21 @@
         N = n // 2 + 1
         results = np.arange(N)
         return results * val
 
     return impl
 
 
-def next_fast_len(target, real):
+def next_fast_len(target, real=False):
     typing_check(types.Integer)(
         target, "The 1st argument 'target' must be an integer.")
     typing_check(types.Boolean)(
         real, "The 2nd argument 'real' must be a boolean.")
 
-    def impl(target, real):
+    def impl(target, real=False):
         if target < 0:
             raise ValueError("Target cannot be negative.")
         return pocketfft.numba_good_size(target, real)
 
     return impl
 
 
@@ -1051,28 +1084,28 @@
         return impl
         
         
     @register_jitable
     def _fhtq(a, u):
         if np.isinf(u[0]):
             # TODO: Is there a better solution for dealing with warnings?
-            print('WARNING: singular transform; consider changing the bias')
+            print("WARNING: singular transform; consider changing the bias")
             u = u.copy()
             u[0] = 0
         A = np.fft.rfft(a) 
         A *= u
         A = np.fft.irfft(A, a.shape[-1])
         return A[..., ::-1]
 
 
     @register_jitable
     def _ifhtq(a, u):
         if u[0] == 0:
             # TODO: Is there a better solution for dealing with warnings?
-            print('WARNING: singular inverse transform; consider changing the bias')
+            print("WARNING: singular inverse transform; consider changing the bias")
             u = u.copy()
             u[0] = np.inf
         A = np.fft.rfft(a) 
         A /= u.conj()
         A = np.fft.irfft(A, a.shape[-1])
         return A[..., ::-1]
```

### Comparing `rocket-fft-0.2.0/rocket_fft/pocketfft.py` & `rocket-fft-0.2.1/rocket_fft/pocketfft.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,32 +140,36 @@
 _tmpl = """
 def _(typingctx, ain, aout, axes, {0}):
     if ain.ndim != aout.ndim:
         raise TypingError("Input and output array must have"
                           "the same number of dimensions")
     if axes.ndim != 1:
         raise TypingError("Axes must be a one-dimensional array")
+        
     copy_axes = not (isinstance(axes.dtype, types.Integer)
                      and (axes.layout in ("C", "F"))
                      and (axes.dtype.bitwidth == 64))
+                     
     def codegen(context, builder, sig, args):
         ain, aout, axes, *rest = args
         ain_t, aout_t, axes_t, *_ = sig.args
         if copy_axes:
             new_t = types.Array(uint64, ndim=1, layout="C")
             sig = new_t(axes_t, uint64)
             args = (axes, uint64)
             axes = array_astype(context, builder, sig, args)
             axes_t = new_t
+            
         ndim = ll_uint64(ain_t.ndim)
         ain_ptr = array_as_voidptr(context, builder, ain_t, ain)
         aout_ptr = array_as_voidptr(context, builder, aout_t, aout)
         ax_ptr = array_as_voidptr(context, builder, axes_t, axes)
         args = (ndim, ain_ptr, aout_ptr, ax_ptr, *rest)
         Pocketfft.{1}(builder, ll_cast(builder, args))
+        
     sig = void(ain, aout, axes, {0})
     return sig, codegen
 """
 
 
 class Builder:
     __slots__ = ("extra_args")
@@ -210,8 +214,8 @@
         n, real = args
         n = builder.zext(n, ll_uint64)
         real = builder.trunc(real, ll_bool)
         ret = Pocketfft.good_size(builder, (n, real))
         return ret
 
     sig = uint64(n, real)
-    return sig, codegen
+    return sig, codegen
```

### Comparing `rocket-fft-0.2.0/rocket_fft/special.py` & `rocket-fft-0.2.1/rocket_fft/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes
 
 from llvmlite import ir
-from numba import TypingError, generated_jit, types, vectorize
+from numba import TypingError, types, vectorize
 from numba.core.cgutils import get_or_insert_function
-from numba.extending import intrinsic
+from numba.extending import intrinsic, overload
 
 from .extutils import get_extension_path, load_extension_library_permanently
 
 special_helpers_module = "_special_helpers"
 load_extension_library_permanently(special_helpers_module)
 
 lib_path = get_extension_path(special_helpers_module)
@@ -72,16 +72,20 @@
         z = builder.fpext(args[0], ll_double)
         return builder.call(fn, [z])
 
     sig = types.double(z)
     return sig, codegen
 
 
-@generated_jit
 def _loggamma(z):
+    pass 
+
+
+@overload(_loggamma)
+def _loggamma_impl(z):
     if isinstance(z, types.Complex):
         return lambda z: _complex_loggamma(z)
     if isinstance(z, types.Float):
         return lambda z: _real_loggamma(z)
     raise TypingError("Argument 'z' must be a float or complex")
```

### Comparing `rocket-fft-0.2.0/rocket_fft/typutils.py` & `rocket-fft-0.2.1/rocket_fft/typutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import numba as nb
 from numba import TypingError
 from numba.core import types
 from numba.np.numpy_support import is_nonelike
 
 
 def is_sequence_like(arg):
-    seq_like = (types.Tuple, types.Array, types.Set,
-                types.ListType, types.Sequence)
+    seq_like = (types.Tuple, types.ListType,
+                types.Array, types.Sequence)
     return isinstance(arg, seq_like)
 
 
 def is_integer(arg):
-    return isinstance(arg, types.Integer)
+    return isinstance(arg, (types.Integer, types.Boolean))
+
+
+def is_scalar(arg):
+    return isinstance(arg, (types.Number, types.Boolean))
 
 
 def is_integer_2tuple(arg):
     return (isinstance(arg, types.UniTuple)
             and (arg.count == 2)
-            and isinstance(arg.dtype, types.Integer))
+            and is_integer(arg.dtype))
 
 
 def is_literal_integer(val):
     def impl(arg):
         if not isinstance(arg, types.IntegerLiteral):
             return False
         return arg.literal_value == val
@@ -34,14 +38,23 @@
         if not isinstance(arg, types.BooleanLiteral):
             return False
         return arg.literal_value == val
 
     return impl
 
 
+def is_contiguous_array(layout):
+    def impl(arg):
+        if not isinstance(arg, types.Array):
+            return False
+        return arg.layout == layout
+
+    return impl
+
+
 def is_not_nonelike(arg):
     return not is_nonelike(arg)
 
 
 class Check:
     __slots__ = ("ty", "as_one", "as_seq", "allow_none", "msg")
 
@@ -96,8 +109,8 @@
         self.checks.update(kwargs)
         return self
 
     @staticmethod
     def get_ordinal(n):
         ordinals = ("th", "st", "nd", "rd", "th",
                     "th", "th", "th", "th", "th")
-        return str(n) + ordinals[n % 10]
+        return str(n) + ordinals[n % 10]
```

### Comparing `rocket-fft-0.2.0/rocket_fft.egg-info/PKG-INFO` & `rocket-fft-0.2.1/rocket_fft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: rocket-fft
-Version: 0.2.0
+Version: 0.2.1
 Summary: Rocket-FFT extends Numba by scipy.fft and numpy.fft
 Home-page: https://github.com/styfenschaer/rocket-fft
 Download-URL: https://github.com/styfenschaer/rocket-fft
 Author: Styfen Schär
 Author-email: styfen.schaer.blog@gmail.com
 License: BSD
 Keywords: FFT,Fourier,Numba,SciPy,NumPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -26,17 +27,17 @@
 # Rocket-FFT
 [![PyPI version](https://img.shields.io/pypi/v/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![License](https://img.shields.io/pypi/l/rocket-fft?color=%2376519B)](https://opensource.org/licenses/BSD-3-Clause)
 [![python](https://img.shields.io/pypi/pyversions/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![status](https://img.shields.io/pypi/status/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 [![downloads](https://img.shields.io/pypi/dm/rocket-fft?color=%2376519B)](https://pypi.org/project/rocket-fft/)
 
-![](https://raw.githubusercontent.com/styfenschaer/rocket-fft/release0.2.0/assets/fourier.gif)
+![](https://raw.githubusercontent.com/styfenschaer/rocket-fft/release0.2.1/assets/fourier.gif)
 
-Rocket-FFT makes [Numba](https://numba.pydata.org/) aware of `numpy.fft` and `scipy.fft`. It takes its name from the [PocketFFT](https://github.com/hayguen/pocketfft) Fast Fourier Transformation library that powers it, and Numba's goal of making your scientific Python code blazingly fast - like a rocket. 
+Rocket-FFT makes [Numba](https://numba.pydata.org/) aware of `numpy.fft` and `scipy.fft`. It takes its name from the [PocketFFT](https://github.com/mreineck/pocketfft) Fast Fourier Transformation library that powers it, and Numba's goal of making your scientific Python code blazingly fast - like a rocket. 
 
 ## Getting Started
 The easiest way to get Rocket-FFT is to:
 ```
 $ pip install rocket-fft
 ```
 Alternatively, you can build it from source:
@@ -95,8 +96,8 @@
 def dct(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], type: i8, fct: f4 | f8, ortho: b1, nthreads: i8) -> None: ...
 def r2r_separable_hartley(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], fct: f4 | f8, nthreads: i8) -> None: ...
 def r2r_genuine_hartley(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], fct: f4 | f8, nthreads: i8) -> None: ...
 def r2r_fftpack(ain: NDArray[f4] | NDArray[f8], aout: NDArray[f4] | NDArray[f8], axes: NDArray[i8], real2hermitian: b1, forward: b1, fct: f4 | f8, nthreads: i8) -> None: ...
 def good_size(target: i8, real: b1) -> i8: ...
 ```
 Note that the low-level interface provides a lower level of safety and convenience compared to the SciPy-like and NumPy-like interfaces. 
-There is almost no safety net, and it is up to the user to ensure proper usage. You may want to consult the original [PocketFFT](https://github.com/hayguen/pocketfft) C++ implementation before using it.
+There is almost no safety net, and it is up to the user to ensure proper usage. You may want to consult the original [PocketFFT](https://github.com/mreineck/pocketfft) C++ implementation before using it.
```

### Comparing `rocket-fft-0.2.0/rocket_fft.egg-info/SOURCES.txt` & `rocket-fft-0.2.1/rocket_fft.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 rocket_fft.egg-info/entry_points.txt
 rocket_fft.egg-info/requires.txt
 rocket_fft.egg-info/top_level.txt
 tests/test_caching.py
 tests/test_fftlog.py
 tests/test_low_level_interface.py
 tests/test_misc.py
+tests/test_multiprocessing.py
 tests/test_multithreading.py
 tests/test_numpy_like.py
 tests/test_numpy_testsuite.py
 tests/test_overwrite_and_dtype.py
 tests/test_scipy_like.py
 tests/test_scipy_testsuite.py
 tests/test_typing.py
```

### Comparing `rocket-fft-0.2.0/setup.py` & `rocket-fft-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from distutils.command.build_ext import build_ext as build_ext_distutils
 from distutils.errors import CompileError
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 from setuptools import Extension, find_packages, setup
 
-py_versions_supported = ("3.8", "3.9", "3.10")
+py_versions_supported = ("3.8", "3.9", "3.10", "3.11")
 
 
 py_version = "{}.{}".format(*sys.version_info[:2])
 if py_version not in py_versions_supported:
     sys.exit(f"Unsupported Python version {py_version};"
              f" must be one of {py_versions_supported}")
 
@@ -106,14 +106,15 @@
         "build_ext": build_ext,
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
```

### Comparing `rocket-fft-0.2.0/tests/test_caching.py` & `rocket-fft-0.2.1/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_fftlog.py` & `rocket-fft-0.2.1/tests/test_fftlog.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_low_level_interface.py` & `rocket-fft-0.2.1/tests/test_low_level_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
 
 @pytest.mark.parametrize("axes_type", (np.int64(1), np.uint64(1),
                                        np.int32(1), np.uint32(1),
                                        np.int16(1), np.uint16(1),
                                        np.int8(1), np.uint8(1),
                                        np.float64(1), np.float32(1),))
-@pytest.mark.parametrize("forward", (np.bool8(False), np.bool8(1), True))
+@pytest.mark.parametrize("forward", (np.bool_(False), np.bool_(1), True))
 @pytest.mark.parametrize("fct", (np.float32(1.0), np.float64(1.0)))
 @pytest.mark.parametrize("nthreads", (np.int64(1), np.uint64(1),
                                       np.int32(1), np.uint32(1),
                                       np.int16(1), np.uint16(1),
                                       np.int8(1), np.uint8(1)))
 def test_low_level_typing_noraise(axes_type, forward, fct, nthreads):
     a = np.random.rand(42).astype(np.complex128)
```

### Comparing `rocket-fft-0.2.0/tests/test_multithreading.py` & `rocket-fft-0.2.1/tests/test_multithreading.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_numpy_like.py` & `rocket-fft-0.2.1/tests/test_numpy_like.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_numpy_testsuite.py` & `rocket-fft-0.2.1/tests/test_numpy_testsuite.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_overwrite_and_dtype.py` & `rocket-fft-0.2.1/tests/test_overwrite_and_dtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     assert x is not y
     assert y.dtype == np.complex128
 
     x = np.random.rand(42).astype(np.float64)
     y = fft(x, overwrite_x=True)
     assert x is not y
 
-    x = np.random.rand(42).astype(np.bool8)
+    x = np.random.rand(42).astype(np.bool_)
     y = fft(x)
     assert x is not y
     assert y.dtype == np.complex128
 
-    x = np.random.rand(42).astype(np.bool8)
+    x = np.random.rand(42).astype(np.bool_)
     y = fft(x, overwrite_x=True)
     assert x is not y
```

### Comparing `rocket-fft-0.2.0/tests/test_scipy_like.py` & `rocket-fft-0.2.1/tests/test_scipy_like.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_scipy_testsuite.py` & `rocket-fft-0.2.1/tests/test_scipy_testsuite.py`

 * *Files identical despite different names*

### Comparing `rocket-fft-0.2.0/tests/test_typing.py` & `rocket-fft-0.2.1/tests/test_typing.py`

 * *Files identical despite different names*

