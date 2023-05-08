# Comparing `tmp/pyUAMMD-1.0.8.tar.gz` & `tmp/pyUAMMD-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUAMMD-1.0.8.tar", last modified: Mon May  8 10:49:38 2023, max compression
+gzip compressed data, was "pyUAMMD-1.0.9.tar", last modified: Mon May  8 10:54:21 2023, max compression
```

## Comparing `pyUAMMD-1.0.8.tar` & `pyUAMMD-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      158 2023-05-04 16:45:12.000000 pyUAMMD-1.0.8/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        9 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD/ThirdParty/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-03 13:08:59.000000 pyUAMMD-1.0.8/pyUAMMD/ThirdParty/json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-03 13:08:59.000000 pyUAMMD-1.0.8/pyUAMMD/ThirdParty/pybind11_json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1081 2023-05-03 16:55:23.000000 pyUAMMD-1.0.8/pyUAMMD/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3817 2023-05-08 10:48:26.000000 pyUAMMD-1.0.8/pyUAMMD/__main__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD/appending/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      316 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    12650 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/forceField.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4507 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/glb.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5841 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/integrator.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11469 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/patchyParticles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6664 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/simulationStep.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3477 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/state.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5514 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/structure.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4291 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/appending/system.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     8797 2023-05-03 13:49:08.000000 pyUAMMD-1.0.8/pyUAMMD/simulation.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      637 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/utils/common.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD/utils/launcher/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      510 2023-05-03 13:10:11.000000 pyUAMMD-1.0.8/pyUAMMD/utils/launcher/UAMMDlauncher.cu
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/utils/launcher/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD/utils/update/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/utils/update/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7296 2023-05-05 15:41:24.000000 pyUAMMD-1.0.8/pyUAMMD/utils/update/groups.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1711 2023-05-03 12:32:56.000000 pyUAMMD-1.0.8/pyUAMMD/utils/update/ids.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/pyUAMMD.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-08 10:49:38.000000 pyUAMMD-1.0.8/pyUAMMD.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      829 2023-05-08 10:49:38.000000 pyUAMMD-1.0.8/pyUAMMD.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-08 10:49:38.000000 pyUAMMD-1.0.8/pyUAMMD.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       27 2023-05-08 10:49:38.000000 pyUAMMD-1.0.8/pyUAMMD.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        8 2023-05-08 10:49:38.000000 pyUAMMD-1.0.8/pyUAMMD.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-08 10:49:06.000000 pyUAMMD-1.0.8/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-08 10:49:38.284640 pyUAMMD-1.0.8/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2367 2023-05-03 13:56:01.000000 pyUAMMD-1.0.8/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      158 2023-05-04 16:45:12.000000 pyUAMMD-1.0.9/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        9 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD/ThirdParty/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-03 13:08:59.000000 pyUAMMD-1.0.9/pyUAMMD/ThirdParty/json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-03 13:08:59.000000 pyUAMMD-1.0.9/pyUAMMD/ThirdParty/pybind11_json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1081 2023-05-03 16:55:23.000000 pyUAMMD-1.0.9/pyUAMMD/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3849 2023-05-08 10:53:13.000000 pyUAMMD-1.0.9/pyUAMMD/__main__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD/appending/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      316 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    12650 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/forceField.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4507 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/glb.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5841 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/integrator.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11469 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/patchyParticles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6664 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/simulationStep.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3477 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/state.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5514 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/structure.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4291 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/appending/system.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     8797 2023-05-03 13:49:08.000000 pyUAMMD-1.0.9/pyUAMMD/simulation.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      637 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/utils/common.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD/utils/launcher/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      510 2023-05-03 13:10:11.000000 pyUAMMD-1.0.9/pyUAMMD/utils/launcher/UAMMDlauncher.cu
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/utils/launcher/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD/utils/update/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/utils/update/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7296 2023-05-05 15:41:24.000000 pyUAMMD-1.0.9/pyUAMMD/utils/update/groups.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1711 2023-05-03 12:32:56.000000 pyUAMMD-1.0.9/pyUAMMD/utils/update/ids.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/pyUAMMD.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-08 10:54:21.000000 pyUAMMD-1.0.9/pyUAMMD.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      829 2023-05-08 10:54:21.000000 pyUAMMD-1.0.9/pyUAMMD.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-08 10:54:21.000000 pyUAMMD-1.0.9/pyUAMMD.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       27 2023-05-08 10:54:21.000000 pyUAMMD-1.0.9/pyUAMMD.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        8 2023-05-08 10:54:21.000000 pyUAMMD-1.0.9/pyUAMMD.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-08 10:53:46.000000 pyUAMMD-1.0.9/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-08 10:54:21.541839 pyUAMMD-1.0.9/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2367 2023-05-03 13:56:01.000000 pyUAMMD-1.0.9/setup.py
```

### Comparing `pyUAMMD-1.0.8/LICENSE` & `pyUAMMD-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/PKG-INFO` & `pyUAMMD-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUAMMD
-Version: 1.0.8
+Version: 1.0.9
 Summary: UAMMD python
 Home-page: https://github.com/PabloIbannez/pyUAMMD
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyUAMMD-1.0.8/pyUAMMD/ThirdParty/json.hpp` & `pyUAMMD-1.0.9/pyUAMMD/ThirdParty/json.hpp`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/ThirdParty/pybind11_json.hpp` & `pyUAMMD-1.0.9/pyUAMMD/ThirdParty/pybind11_json.hpp`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/__init__.py` & `pyUAMMD-1.0.9/pyUAMMD/__init__.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/__main__.py` & `pyUAMMD-1.0.9/pyUAMMD/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,16 @@
                  '-std=c++14',
                  '-O3',
                  '-DUAMMD_EXTENSIONS',
                  '-DMAXLOGLEVEL=5',
                  '-Xcompiler=\"-O3 -march=native -fPIC\"',
                  '-ccbin=g++']
 
+        print(' '.join(FLAGS))
+
     elif args.arch:
         try:
 
             NVCC_PATH = os.path.join(find_cuda_home_path(), 'bin', 'nvcc')
 
             gencode = []
```

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/forceField.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/forceField.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/glb.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/glb.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/integrator.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/integrator.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/patchyParticles.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/patchyParticles.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/simulationStep.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/simulationStep.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/state.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/state.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/structure.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/structure.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/appending/system.py` & `pyUAMMD-1.0.9/pyUAMMD/appending/system.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/simulation.py` & `pyUAMMD-1.0.9/pyUAMMD/simulation.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/utils/common.py` & `pyUAMMD-1.0.9/pyUAMMD/utils/common.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/utils/update/groups.py` & `pyUAMMD-1.0.9/pyUAMMD/utils/update/groups.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD/utils/update/ids.py` & `pyUAMMD-1.0.9/pyUAMMD/utils/update/ids.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyUAMMD.egg-info/PKG-INFO` & `pyUAMMD-1.0.9/pyUAMMD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUAMMD
-Version: 1.0.8
+Version: 1.0.9
 Summary: UAMMD python
 Home-page: https://github.com/PabloIbannez/pyUAMMD
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyUAMMD-1.0.8/pyUAMMD.egg-info/SOURCES.txt` & `pyUAMMD-1.0.9/pyUAMMD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.8/pyproject.toml` & `pyUAMMD-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-cuda-cpp", "setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="pyUAMMD"
-version="1.0.8"
+version="1.0.9"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "UAMMD python"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `pyUAMMD-1.0.8/setup.py` & `pyUAMMD-1.0.9/setup.py`

 * *Files identical despite different names*

