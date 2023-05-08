# Comparing `tmp/linc-1.4.0.tar.gz` & `tmp/linc-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linc-1.4.0.tar", max compression
+gzip compressed data, was "linc-1.5.0.tar", max compression
```

## Comparing `linc-1.4.0.tar` & `linc-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      136 2023-02-20 02:18:41.067533 linc-1.4.0/README.md
--rw-r--r--   0        0        0      316 2023-02-22 15:13:25.251690 linc-1.4.0/linc/__init__.py
--rw-r--r--   0        0        0     1065 2023-02-15 15:29:59.756081 linc-1.4.0/linc/cli.py
--rw-r--r--   0        0        0       92 2023-02-15 15:29:59.756081 linc-1.4.0/linc/config/__init__.py
--rw-r--r--   0        0        0       34 2023-02-15 17:30:56.063904 linc-1.4.0/linc/config/default-config.toml
--rw-r--r--   0        0        0     1015 2023-03-25 20:52:23.083165 linc-1.4.0/linc/config/models.py
--rw-r--r--   0        0        0      931 2023-02-16 02:55:41.005378 linc-1.4.0/linc/config/read.py
--rw-r--r--   0        0        0     3037 2023-04-10 00:00:05.393895 linc-1.4.0/linc/convertion.py
--rw-r--r--   0        0        0     2727 2023-02-19 01:05:47.201474 linc-1.4.0/linc/models.py
--rw-r--r--   0        0        0       77 2023-02-15 15:29:59.756081 linc-1.4.0/linc/parse/__init__.py
--rw-r--r--   0        0        0       41 2023-02-18 22:47:13.181551 linc-1.4.0/linc/parse/constants.py
--rw-r--r--   0        0        0      983 2023-02-16 21:11:51.157824 linc-1.4.0/linc/parse/dataset.py
--rw-r--r--   0        0        0      247 2023-02-15 15:29:59.756081 linc-1.4.0/linc/parse/file.py
--rw-r--r--   0        0        0     2767 2023-02-15 15:29:59.756081 linc-1.4.0/linc/parse/header.py
--rw-r--r--   0        0        0      344 2023-02-19 00:12:32.110253 linc-1.4.0/linc/parse/utils.py
--rw-r--r--   0        0        0     1762 2023-04-09 23:59:51.673896 linc-1.4.0/linc/reader.py
--rw-r--r--   0        0        0     1158 2023-02-20 02:01:56.477632 linc-1.4.0/linc/utils.py
--rw-r--r--   0        0        0     1293 2023-02-18 17:19:25.786396 linc-1.4.0/linc/write/common.py
--rw-r--r--   0        0        0      636 2023-02-19 02:08:52.266358 linc-1.4.0/linc/write/types.py
--rw-r--r--   0        0        0     4257 2023-04-10 00:13:34.203778 linc-1.4.0/linc/write/writer_nc.py
--rw-r--r--   0        0        0      629 2023-04-10 00:12:50.773786 linc-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 linc-1.4.0/setup.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 linc-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2023-02-20 02:18:41.067533 linc-1.5.0/README.md
+-rw-r--r--   0        0        0      316 2023-02-22 15:13:25.251690 linc-1.5.0/linc/__init__.py
+-rw-r--r--   0        0        0     1065 2023-02-15 15:29:59.756081 linc-1.5.0/linc/cli.py
+-rw-r--r--   0        0        0       92 2023-02-15 15:29:59.756081 linc-1.5.0/linc/config/__init__.py
+-rw-r--r--   0        0        0       34 2023-02-15 17:30:56.063904 linc-1.5.0/linc/config/default-config.toml
+-rw-r--r--   0        0        0     1188 2023-04-11 02:58:40.653993 linc-1.5.0/linc/config/models.py
+-rw-r--r--   0        0        0      931 2023-02-16 02:55:41.005378 linc-1.5.0/linc/config/read.py
+-rw-r--r--   0        0        0     3037 2023-04-10 00:00:05.393895 linc-1.5.0/linc/convertion.py
+-rw-r--r--   0        0        0     2727 2023-02-19 01:05:47.201474 linc-1.5.0/linc/models.py
+-rw-r--r--   0        0        0       77 2023-02-15 15:29:59.756081 linc-1.5.0/linc/parse/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-18 22:47:13.181551 linc-1.5.0/linc/parse/constants.py
+-rw-r--r--   0        0        0      983 2023-02-16 21:11:51.157824 linc-1.5.0/linc/parse/dataset.py
+-rw-r--r--   0        0        0      247 2023-02-15 15:29:59.756081 linc-1.5.0/linc/parse/file.py
+-rw-r--r--   0        0        0     2767 2023-02-15 15:29:59.756081 linc-1.5.0/linc/parse/header.py
+-rw-r--r--   0        0        0      344 2023-02-19 00:12:32.110253 linc-1.5.0/linc/parse/utils.py
+-rw-r--r--   0        0        0     1762 2023-04-09 23:59:51.673896 linc-1.5.0/linc/reader.py
+-rw-r--r--   0        0        0     1413 2023-04-15 01:59:49.664279 linc-1.5.0/linc/utils.py
+-rw-r--r--   0        0        0     1293 2023-02-18 17:19:25.786396 linc-1.5.0/linc/write/common.py
+-rw-r--r--   0        0        0     6044 2023-04-11 15:37:40.743083 linc-1.5.0/linc/write/writer_nc.py
+-rw-r--r--   0        0        0      629 2023-04-11 15:36:38.533097 linc-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 linc-1.5.0/setup.py
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 linc-1.5.0/PKG-INFO
```

### Comparing `linc-1.4.0/linc/cli.py` & `linc-1.5.0/linc/cli.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/config/models.py` & `linc-1.5.0/linc/config/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import Any
 
 from pydantic import BaseModel, Field
 
 
 DEFAULT_ATTRS: dict[str, Any] = {"generated_by": "linc-python"}
 
+class OptionalVariable(BaseModel):
+    name: str
+    type: str
 
 class Options(BaseModel):
     channel_not_present_all_ok: bool = False
+    time_lidar_variables: list[OptionalVariable] = []
+    time_channel_variables: list[OptionalVariable] = []
 
 class LidarChannel(BaseModel):
     name: str
     link_to: str # The device ID
 
 
 class LidarConfig(BaseModel):
```

### Comparing `linc-1.4.0/linc/config/read.py` & `linc-1.5.0/linc/config/read.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/convertion.py` & `linc-1.5.0/linc/convertion.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/models.py` & `linc-1.5.0/linc/models.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/parse/dataset.py` & `linc-1.5.0/linc/parse/dataset.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/parse/header.py` & `linc-1.5.0/linc/parse/header.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/reader.py` & `linc-1.5.0/linc/reader.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/linc/utils.py` & `linc-1.5.0/linc/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,7 +40,16 @@
         case _:
             raise ValueError("Input type not supported")
 
 
 def device_id_to_str(device_id: DeviceId) -> str:
     return f"{device_id.type}{device_id.number}"
 
+
+def str_to_device_id(device_id: str) -> DeviceId:
+    sep_index = 3 if device_id.startswith("S2") else 2
+
+    # set_trace()
+    return DeviceId(
+        type=device_id[:sep_index], # type: ignore
+        number=device_id[sep_index:] # type: ignore
+    )
```

### Comparing `linc-1.4.0/linc/write/common.py` & `linc-1.5.0/linc/write/common.py`

 * *Files identical despite different names*

### Comparing `linc-1.4.0/pyproject.toml` & `linc-1.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linc"
-version = "1.4.0"
+version = "1.5.0"
 description = "A package to handle LICEL Binary format"
 authors = ["Juan Diego <jdlar@eafit.edu.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `linc-1.4.0/setup.py` & `linc-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['linc = linc.cli:app']}
 
 setup_kwargs = {
     'name': 'linc',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'A package to handle LICEL Binary format',
     'long_description': '# Linc\n---\nLinc is a fast way to convert [Licel Raw Format](https://licel.com/raw_data_format.html) into netCDF4 to handle data easier.\n',
     'author': 'Juan Diego',
     'author_email': 'jdlar@eafit.edu.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `linc-1.4.0/PKG-INFO` & `linc-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linc
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package to handle LICEL Binary format
 License: MIT
 Author: Juan Diego
 Author-email: jdlar@eafit.edu.co
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

