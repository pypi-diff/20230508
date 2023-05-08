# Comparing `tmp/periodic_element_properties-0.1.3.tar.gz` & `tmp/periodic_element_properties-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodic_element_properties-0.1.3.tar", max compression
+gzip compressed data, was "periodic_element_properties-0.1.4.tar", max compression
```

## Comparing `periodic_element_properties-0.1.3.tar` & `periodic_element_properties-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       83 2023-05-08 14:59:06.886695 periodic_element_properties-0.1.3/periodic_element_properties/__init__.py
--rw-r--r--   0        0        0     1580 2023-05-08 15:02:00.071154 periodic_element_properties-0.1.3/periodic_element_properties/elements.py
--rw-r--r--   0        0        0    64278 2023-05-08 06:51:13.870866 periodic_element_properties-0.1.3/periodic_element_properties/properties_of_elements.json
--rw-r--r--   0        0        0      505 2023-05-08 15:02:52.069920 periodic_element_properties-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 06:41:58.784088 periodic_element_properties-0.1.3/README.md
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 periodic_element_properties-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-05-08 14:59:06.886695 periodic_element_properties-0.1.4/periodic_element_properties/__init__.py
+-rw-r--r--   0        0        0     1580 2023-05-08 15:02:00.071154 periodic_element_properties-0.1.4/periodic_element_properties/elements.py
+-rw-r--r--   0        0        0    64278 2023-05-08 06:51:13.870866 periodic_element_properties-0.1.4/periodic_element_properties/properties_of_elements.json
+-rw-r--r--   0        0        0      505 2023-05-08 15:05:40.642452 periodic_element_properties-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 06:41:58.784088 periodic_element_properties-0.1.4/README.md
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 periodic_element_properties-0.1.4/PKG-INFO
```

### Comparing `periodic_element_properties-0.1.3/periodic_element_properties/elements.py` & `periodic_element_properties-0.1.4/periodic_element_properties/elements.py`

 * *Files identical despite different names*

### Comparing `periodic_element_properties-0.1.3/periodic_element_properties/properties_of_elements.json` & `periodic_element_properties-0.1.4/periodic_element_properties/properties_of_elements.json`

 * *Files identical despite different names*

### Comparing `periodic_element_properties-0.1.3/PKG-INFO` & `periodic_element_properties-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodic-element-properties
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package contains information about periodic elements and their properties
 Author: Prithivee7
 Author-email: getprithivee@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

