# Comparing `tmp/pyvium-0.1.8b0.tar.gz` & `tmp/pyvium-0.1.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvium-0.1.8b0.tar", max compression
+gzip compressed data, was "pyvium-0.1.9b0.tar", max compression
```

## Comparing `pyvium-0.1.8b0.tar` & `pyvium-0.1.9b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      618 2023-02-13 12:29:09.992636 pyvium-0.1.8b0/LICENSE
--rw-r--r--   0        0        0     1415 2023-05-04 20:02:40.515194 pyvium-0.1.8b0/pyproject.toml
--rw-r--r--   0        0        0       52 2023-05-03 22:44:37.236878 pyvium-0.1.8b0/pyvium/__init__.py
--rw-r--r--   0        0        0      306 2023-05-04 18:47:48.314812 pyvium-0.1.8b0/pyvium/core/__init__.py
--rw-r--r--   0        0        0      143 2023-05-04 19:24:19.702820 pyvium-0.1.8b0/pyvium/core/constants.py
--rw-r--r--   0        0        0      936 2023-05-04 20:02:28.229224 pyvium-0.1.8b0/pyvium/core/core_base.py
--rw-r--r--   0        0        0    10741 2023-05-04 19:32:48.053240 pyvium-0.1.8b0/pyvium/core/direct_mode_functions.py
--rw-r--r--   0        0        0     4551 2023-05-04 19:34:42.515380 pyvium-0.1.8b0/pyvium/core/generic_functions.py
--rw-r--r--   0        0        0     5745 2023-05-04 19:23:09.727741 pyvium-0.1.8b0/pyvium/core/method_mode_functions.py
--rw-r--r--   0        0        0     2539 2023-05-04 19:23:11.379740 pyvium-0.1.8b0/pyvium/core/we32_functions.py
--rw-r--r--   0        0        0      325 2023-02-13 12:29:10.046638 pyvium-0.1.8b0/pyvium/errors/__init__.py
--rw-r--r--   0        0        0      197 2023-02-13 12:29:10.047636 pyvium-0.1.8b0/pyvium/errors/cell_off.py
--rw-r--r--   0        0        0      317 2023-02-13 12:29:10.047636 pyvium-0.1.8b0/pyvium/errors/device_busy.py
--rw-r--r--   0        0        0      298 2023-02-13 12:29:10.047636 pyvium-0.1.8b0/pyvium/errors/device_not_connected_to_iviumsoft.py
--rw-r--r--   0        0        0      272 2023-02-13 12:29:10.048636 pyvium-0.1.8b0/pyvium/errors/driver_not_open.py
--rw-r--r--   0        0        0      289 2023-02-13 12:29:10.048636 pyvium-0.1.8b0/pyvium/errors/no_device_detected.py
--rw-r--r--   0        0        0      269 2023-02-13 12:29:10.048636 pyvium-0.1.8b0/pyvium/errors/no_iviumsoft_running.py
--rw-r--r--   0        0        0  5131844 2023-02-13 12:29:10.031671 pyvium-0.1.8b0/pyvium/IVIUM_remdriver.dll
--rw-r--r--   0        0        0  2187264 2023-02-13 12:29:10.045638 pyvium-0.1.8b0/pyvium/Ivium_remdriver64.dll
--rw-r--r--   0        0        0      250 2023-05-04 18:57:45.028858 pyvium-0.1.8b0/pyvium/pyvium/__init__.py
--rw-r--r--   0        0        0     9022 2023-05-04 18:55:01.107663 pyvium-0.1.8b0/pyvium/pyvium/direct_mode_functions.py
--rw-r--r--   0        0        0     5755 2023-05-04 18:55:22.266023 pyvium-0.1.8b0/pyvium/pyvium/generic_functions.py
--rw-r--r--   0        0        0     4324 2023-05-04 19:52:25.297439 pyvium-0.1.8b0/pyvium/pyvium/method_mode_functions.py
--rw-r--r--   0        0        0     1941 2023-02-13 12:29:10.049636 pyvium-0.1.8b0/pyvium/pyvium_verifiers.py
--rw-r--r--   0        0        0       52 2023-02-13 12:29:10.049636 pyvium-0.1.8b0/pyvium/util/__init__.py
--rw-r--r--   0        0        0      477 2023-02-13 12:29:10.050636 pyvium-0.1.8b0/pyvium/util/get_ivium_dll_path.py
--rw-r--r--   0        0        0     1620 2023-02-13 12:29:09.992636 pyvium-0.1.8b0/README.md
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyvium-0.1.8b0/setup.py
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pyvium-0.1.8b0/PKG-INFO
+-rw-r--r--   0        0        0      618 2023-02-13 12:29:09.992636 pyvium-0.1.9b0/LICENSE
+-rw-r--r--   0        0        0     1415 2023-05-04 20:11:45.649292 pyvium-0.1.9b0/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-05-03 22:44:37.236878 pyvium-0.1.9b0/pyvium/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-04 18:47:48.314812 pyvium-0.1.9b0/pyvium/core/__init__.py
+-rw-r--r--   0        0        0      143 2023-05-04 19:24:19.702820 pyvium-0.1.9b0/pyvium/core/constants.py
+-rw-r--r--   0        0        0      936 2023-05-04 20:02:28.229224 pyvium-0.1.9b0/pyvium/core/core_base.py
+-rw-r--r--   0        0        0    10741 2023-05-04 19:32:48.053240 pyvium-0.1.9b0/pyvium/core/direct_mode_functions.py
+-rw-r--r--   0        0        0     4551 2023-05-04 19:34:42.515380 pyvium-0.1.9b0/pyvium/core/generic_functions.py
+-rw-r--r--   0        0        0     5745 2023-05-04 19:23:09.727741 pyvium-0.1.9b0/pyvium/core/method_mode_functions.py
+-rw-r--r--   0        0        0     2539 2023-05-04 19:23:11.379740 pyvium-0.1.9b0/pyvium/core/we32_functions.py
+-rw-r--r--   0        0        0      325 2023-02-13 12:29:10.046638 pyvium-0.1.9b0/pyvium/errors/__init__.py
+-rw-r--r--   0        0        0      197 2023-02-13 12:29:10.047636 pyvium-0.1.9b0/pyvium/errors/cell_off.py
+-rw-r--r--   0        0        0      317 2023-02-13 12:29:10.047636 pyvium-0.1.9b0/pyvium/errors/device_busy.py
+-rw-r--r--   0        0        0      298 2023-02-13 12:29:10.047636 pyvium-0.1.9b0/pyvium/errors/device_not_connected_to_iviumsoft.py
+-rw-r--r--   0        0        0      272 2023-02-13 12:29:10.048636 pyvium-0.1.9b0/pyvium/errors/driver_not_open.py
+-rw-r--r--   0        0        0      289 2023-02-13 12:29:10.048636 pyvium-0.1.9b0/pyvium/errors/no_device_detected.py
+-rw-r--r--   0        0        0      269 2023-02-13 12:29:10.048636 pyvium-0.1.9b0/pyvium/errors/no_iviumsoft_running.py
+-rw-r--r--   0        0        0  5131844 2023-02-13 12:29:10.031671 pyvium-0.1.9b0/pyvium/IVIUM_remdriver.dll
+-rw-r--r--   0        0        0  2187264 2023-02-13 12:29:10.045638 pyvium-0.1.9b0/pyvium/Ivium_remdriver64.dll
+-rw-r--r--   0        0        0      250 2023-05-04 18:57:45.028858 pyvium-0.1.9b0/pyvium/pyvium/__init__.py
+-rw-r--r--   0        0        0     9022 2023-05-04 18:55:01.107663 pyvium-0.1.9b0/pyvium/pyvium/direct_mode_functions.py
+-rw-r--r--   0        0        0     5747 2023-05-04 20:11:13.835864 pyvium-0.1.9b0/pyvium/pyvium/generic_functions.py
+-rw-r--r--   0        0        0     4324 2023-05-04 19:52:25.297439 pyvium-0.1.9b0/pyvium/pyvium/method_mode_functions.py
+-rw-r--r--   0        0        0     1941 2023-02-13 12:29:10.049636 pyvium-0.1.9b0/pyvium/pyvium_verifiers.py
+-rw-r--r--   0        0        0       52 2023-02-13 12:29:10.049636 pyvium-0.1.9b0/pyvium/util/__init__.py
+-rw-r--r--   0        0        0      477 2023-02-13 12:29:10.050636 pyvium-0.1.9b0/pyvium/util/get_ivium_dll_path.py
+-rw-r--r--   0        0        0     1620 2023-02-13 12:29:09.992636 pyvium-0.1.9b0/README.md
+-rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyvium-0.1.9b0/setup.py
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pyvium-0.1.9b0/PKG-INFO
```

### Comparing `pyvium-0.1.8b0/LICENSE` & `pyvium-0.1.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyproject.toml` & `pyvium-0.1.9b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 homepage = "https://github.com/SF-Tec/pyvium"
 keywords = ["ivium", "iviumsoft", "ivium software", "ivium compactstat"]
 repository = "https://github.com/SF-Tec/pyvium"
 license = "Apache-2.0"
 name = "pyvium"
 packages = [{ include = "pyvium" }]
 readme = "README.md"
-version = "0.1.8beta"
+version = "0.1.9beta"
 classifiers = [
     # How mature is this project? Common values are
     #   3 - Alpha
     #   4 - Beta
     #   5 - Production/Stable
     'Development Status :: 4 - Beta',
```

### Comparing `pyvium-0.1.8b0/pyvium/core/core_base.py` & `pyvium-0.1.9b0/pyvium/core/core_base.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/core/direct_mode_functions.py` & `pyvium-0.1.9b0/pyvium/core/direct_mode_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/core/generic_functions.py` & `pyvium-0.1.9b0/pyvium/core/generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/core/method_mode_functions.py` & `pyvium-0.1.9b0/pyvium/core/method_mode_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/core/we32_functions.py` & `pyvium-0.1.9b0/pyvium/core/we32_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/IVIUM_remdriver.dll` & `pyvium-0.1.9b0/pyvium/IVIUM_remdriver.dll`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/Ivium_remdriver64.dll` & `pyvium-0.1.9b0/pyvium/Ivium_remdriver64.dll`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/pyvium/direct_mode_functions.py` & `pyvium-0.1.9b0/pyvium/pyvium/direct_mode_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/pyvium/generic_functions.py` & `pyvium-0.1.9b0/pyvium/pyvium/generic_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,26 +45,26 @@
         result_code = Core.IV_getdevicestatus()
         return result_code, status_labels[str(result_code)]
 
     @staticmethod
     def is_iviumsoft_running() -> bool:
         '''It returns true if if the selected instance of IviumSoft is running'''
         PyviumVerifiers.verify_driver_is_open()
-        return not Core.IV_getdevicestatus() == -1
+        return Core.IV_getdevicestatus() != -1
 
     @staticmethod
     def get_active_iviumsoft_instances():
         '''Returns a list of active(open) IviumSoft instances'''
         PyviumVerifiers.verify_driver_is_open()
         active_instances = []
         first_active_instance_number = 0
         for instance_number in range(1, 32):
             Core.IV_selectdevice(instance_number)
 
-            if not Core.IV_getdevicestatus() == -1:
+            if Core.IV_getdevicestatus() != -1:
                 active_instances.append(instance_number)
 
                 if first_active_instance_number == 0:
                     first_active_instance_number = instance_number
 
         if first_active_instance_number == 0:
             first_active_instance_number = 1
```

### Comparing `pyvium-0.1.8b0/pyvium/pyvium/method_mode_functions.py` & `pyvium-0.1.9b0/pyvium/pyvium/method_mode_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/pyvium/pyvium_verifiers.py` & `pyvium-0.1.9b0/pyvium/pyvium_verifiers.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/README.md` & `pyvium-0.1.9b0/README.md`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.8b0/setup.py` & `pyvium-0.1.9b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cffi>=1.15.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyvium',
-    'version': '0.1.8b0',
+    'version': '0.1.9b0',
     'description': 'A tiny Python wrapper around the <Software development driver DLL> for IviumSoft.',
     'long_description': '# PYVIUM\n\nTiny Python wrapper around the "Software development driver DLL" for IviumSoft.\n\n# Important:\n\nThis module uses a dll from the IviumSoft application. You need to have this software installed on a Windows machine. The IviumSoft application can be downloaded from here: https://www.ivium.com/support/#Software%20update\n\nThis version of Pyvium has been tested for IviumSoft release 4.1100.\n\n## Installation\n\nInstall PYVIUM easily with pip:\n\n```\npip install pyvium\n```\n\nOr with poetry:\n\n```\npoetry add pyvium\n```\n\n## Usage Example (Using IviumSoft Core functions)\n\nTo use the same functions available in the "IviumSoft driver DLL" you can import the Core class as follows. All functions return a result code (integer) and a result value if available. For further information you can check the IviumSoft documentation.\n\n```\nfrom pyvium import Core\n\nCore.IV_open()\nCore.IV_getdevicestatus()\nCore.IV_close()\n```\n\n## Usage Example (Using Pyvium methods)\n\nThis is a wrapper around the Core functions that adds a few things:\n\n- Exception management (you can find an example [here](https://github.com/SF-Tec/pyvium/blob/main/docs/error_management.md))\n- New functionalities\n\n```\nfrom pyvium import Pyvium\n\nPyvium.open_driver()\nPyvium.get_device_status()\nPyvium.close_driver()\n\n```\n\n## Supported functions\n\nThe list of currently supported and implemented functions can be found [here](https://github.com/SF-Tec/pyvium/blob/main/docs/method_list.md).\n\n## Links\n\n- [See on GitHub](https://github.com/sf-tec/pyvium)\n- [See on PyPI](https://pypi.org/project/pyvium)\n',
     'author': 'Alejandro Gutiérrez',
     'author_email': 'agutierrez@stec.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SF-Tec/pyvium',
```

### Comparing `pyvium-0.1.8b0/PKG-INFO` & `pyvium-0.1.9b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvium
-Version: 0.1.8b0
+Version: 0.1.9b0
 Summary: A tiny Python wrapper around the <Software development driver DLL> for IviumSoft.
 Home-page: https://github.com/SF-Tec/pyvium
 License: Apache-2.0
 Keywords: ivium,iviumsoft,ivium software,ivium compactstat
 Author: Alejandro Gutiérrez
 Author-email: agutierrez@stec.es
 Requires-Python: >=3.11,<4.0
```

