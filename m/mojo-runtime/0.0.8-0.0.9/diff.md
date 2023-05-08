# Comparing `tmp/mojo_runtime-0.0.8.tar.gz` & `tmp/mojo_runtime-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_runtime-0.0.8.tar", max compression
+gzip compressed data, was "mojo_runtime-0.0.9.tar", max compression
```

## Comparing `mojo_runtime-0.0.8.tar` & `mojo_runtime-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1083 2023-03-17 16:04:50.913098 mojo_runtime-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      121 2023-03-17 16:04:50.913098 mojo_runtime-0.0.8/README.md
--rw-r--r--   0        0        0      685 2023-03-20 23:06:29.929808 mojo_runtime-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-17 16:04:50.917098 mojo_runtime-0.0.8/source/packages/mojo/runtime/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 16:04:50.917098 mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/__init__.py
--rwxr-xr-x   0        0        0     9715 2023-03-20 22:50:36.561844 mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/base.py
--rw-r--r--   0        0        0     3338 2023-03-20 22:50:57.546020 mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/console.py
--rw-r--r--   0        0        0     2771 2023-03-20 22:50:57.546020 mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/service.py
--rw-r--r--   0        0        0     1313 2023-03-17 16:37:26.538200 mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/testrun.py
--rw-r--r--   0        0        0     2397 2023-03-17 16:36:47.325651 mojo_runtime-0.0.8/source/packages/mojo/runtime/configuration.py
--rw-r--r--   0        0        0      858 2023-03-17 16:27:43.624938 mojo_runtime-0.0.8/source/packages/mojo/runtime/context.py
--rw-r--r--   0        0        0     4488 2023-03-18 15:38:10.582214 mojo_runtime-0.0.8/source/packages/mojo/runtime/initialize.py
--rw-r--r--   0        0        0     9773 2023-03-20 22:54:43.335909 mojo_runtime-0.0.8/source/packages/mojo/runtime/paths.py
--rw-r--r--   0        0        0    15347 2023-03-20 22:50:57.546020 mojo_runtime-0.0.8/source/packages/mojo/runtime/variables.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 mojo_runtime-0.0.8/setup.py
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 mojo_runtime-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-17 16:04:50.913098 mojo_runtime-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      121 2023-03-17 16:04:50.913098 mojo_runtime-0.0.9/README.md
+-rw-r--r--   0        0        0      685 2023-03-21 22:07:19.714767 mojo_runtime-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-17 16:04:50.917098 mojo_runtime-0.0.9/source/packages/mojo/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-17 16:04:50.917098 mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/__init__.py
+-rwxr-xr-x   0        0        0     9717 2023-03-21 22:06:38.338280 mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/base.py
+-rw-r--r--   0        0        0     3338 2023-03-20 22:50:57.546020 mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/console.py
+-rw-r--r--   0        0        0     2771 2023-03-20 22:50:57.546020 mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/service.py
+-rw-r--r--   0        0        0     1313 2023-03-17 16:37:26.538200 mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/testrun.py
+-rw-r--r--   0        0        0     2397 2023-03-17 16:36:47.325651 mojo_runtime-0.0.9/source/packages/mojo/runtime/configuration.py
+-rw-r--r--   0        0        0      858 2023-03-17 16:27:43.624938 mojo_runtime-0.0.9/source/packages/mojo/runtime/context.py
+-rw-r--r--   0        0        0     4484 2023-03-21 22:06:08.221927 mojo_runtime-0.0.9/source/packages/mojo/runtime/initialize.py
+-rw-r--r--   0        0        0     9773 2023-03-20 22:54:43.335909 mojo_runtime-0.0.9/source/packages/mojo/runtime/paths.py
+-rw-r--r--   0        0        0    15347 2023-03-20 22:50:57.546020 mojo_runtime-0.0.9/source/packages/mojo/runtime/variables.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 mojo_runtime-0.0.9/setup.py
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 mojo_runtime-0.0.9/PKG-INFO
```

### Comparing `mojo_runtime-0.0.8/LICENSE.txt` & `mojo_runtime-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/pyproject.toml` & `mojo_runtime-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-runtime"
 description = "Automation Mojo Runtime Module (mojo-runtime)"
-version = "0.0.8"
+version = "0.0.9"
 authors = []
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/base.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,8 +203,8 @@
 
         env["output_directory"] = outdir_full
 
 
 
 # Activation Step - 7: Import the logging module so we can be the trigger the logging configuration
 # for standard out
-from mojo.xmods.xlogging.foundations # pylint: disable=unused-import,wrong-import-position
+import mojo.xmods.xlogging.foundations # pylint: disable=unused-import,wrong-import-position
```

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/console.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/console.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/service.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/service.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/activation/testrun.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/activation/testrun.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/configuration.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/context.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/context.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/initialize.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/initialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,12 +114,12 @@
     MOJO_RUNTIME_OVERRIDES.MJR_CONFIG_USE_TOPOLOGY = use_topology
     MOJO_RUNTIME_OVERRIDES.DEFAULT_CONFIGURATION = default_configuration
 
     if service_name is not None:
         MOJO_RUNTIME_OVERRIDES.MJR_SERVICE_NAME = service_name
 
     for field in dir(aliases):
-        if not field.startswith("MJR_"):
+        if field.startswith("MJR_"):
             alias = getattr(aliases, field)
             setattr(MojoRuntimeAlias, field, alias)
 
     return
```

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/paths.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/paths.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/source/packages/mojo/runtime/variables.py` & `mojo_runtime-0.0.9/source/packages/mojo/runtime/variables.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-0.0.8/setup.py` & `mojo_runtime-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['coverage>=7.0.4,<8.0.0', 'mojo-xmodules>=0.0.8,<0.0.9']
 
 setup_kwargs = {
     'name': 'mojo-runtime',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Automation Mojo Runtime Module (mojo-runtime)',
     'long_description': '# Contextualize\nA package used to create a global context that allows for the distribution of options and configuration.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_runtime-0.0.8/PKG-INFO` & `mojo_runtime-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-runtime
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation Mojo Runtime Module (mojo-runtime)
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

