# Comparing `tmp/periodic_element_properties-0.1.5.tar.gz` & `tmp/periodic_element_properties-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodic_element_properties-0.1.5.tar", max compression
+gzip compressed data, was "periodic_element_properties-0.2.0.tar", max compression
```

## Comparing `periodic_element_properties-0.1.5.tar` & `periodic_element_properties-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       83 2023-05-08 15:12:25.099016 periodic_element_properties-0.1.5/periodic_element_properties/__init__.py
--rw-r--r--   0        0        0     1611 2023-05-08 15:10:13.203950 periodic_element_properties-0.1.5/periodic_element_properties/elements.py
--rw-r--r--   0        0        0    64278 2023-05-08 06:51:13.870866 periodic_element_properties-0.1.5/periodic_element_properties/properties_of_elements.json
--rw-r--r--   0        0        0      505 2023-05-08 15:11:05.364864 periodic_element_properties-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 06:41:58.784088 periodic_element_properties-0.1.5/README.md
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 periodic_element_properties-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-05-08 16:20:27.230424 periodic_element_properties-0.2.0/periodic_element_properties/__init__.py
+-rw-r--r--   0        0        0     2927 2023-05-08 16:20:18.804444 periodic_element_properties-0.2.0/periodic_element_properties/elements.py
+-rw-r--r--   0        0        0    64278 2023-05-08 06:51:13.870866 periodic_element_properties-0.2.0/periodic_element_properties/properties_of_elements.json
+-rw-r--r--   0        0        0      505 2023-05-08 16:21:04.860716 periodic_element_properties-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      957 2023-05-08 16:28:00.597231 periodic_element_properties-0.2.0/README.md
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 periodic_element_properties-0.2.0/PKG-INFO
```

### Comparing `periodic_element_properties-0.1.5/periodic_element_properties/properties_of_elements.json` & `periodic_element_properties-0.2.0/periodic_element_properties/properties_of_elements.json`

 * *Files identical despite different names*

