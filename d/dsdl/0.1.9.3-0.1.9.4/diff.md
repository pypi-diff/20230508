# Comparing `tmp/dsdl-0.1.9.3.tar.gz` & `tmp/dsdl-0.1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dsdl-0.1.9.3.tar", last modified: Tue Nov  1 04:37:42 2022, max compression
+gzip compressed data, was "dist\dsdl-0.1.9.4.tar", last modified: Tue Nov  1 12:20:51 2022, max compression
```

## Comparing `dsdl-0.1.9.3.tar` & `dsdl-0.1.9.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/
--rw-rw-rw-   0        0        0    11604 2022-09-19 02:10:48.000000 dsdl-0.1.9.3/LICENSE
--rw-rw-rw-   0        0        0     6664 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     6280 2022-09-20 09:26:25.000000 dsdl-0.1.9.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/
--rw-rw-rw-   0        0        0      211 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/__init__.py
--rw-rw-rw-   0        0        0      117 2022-11-01 04:36:50.000000 dsdl-0.1.9.3/dsdl/__version__.py
--rw-rw-rw-   0        0        0      283 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/cli.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/dataset/
--rw-rw-rw-   0        0        0      259 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dataset/__init__.py
--rw-rw-rw-   0        0        0     3796 2022-10-31 07:44:22.000000 dsdl-0.1.9.3/dsdl/dataset/base_dataset.py
--rw-rw-rw-   0        0        0      336 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dataset/demo_dataset.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/dataset/utils/
--rw-rw-rw-   0        0        0      162 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0     1792 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dataset/utils/commons.py
--rw-rw-rw-   0        0        0     1737 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dataset/utils/parser.py
--rw-rw-rw-   0        0        0     6835 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/dataset/utils/visualizer.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/dsdl_py_library/
--rw-rw-rw-   0        0        0      684 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dsdl_py_library/CIFAR10_test_data.py
--rw-rw-rw-   0        0        0        0 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dsdl_py_library/__init__.py
--rw-rw-rw-   0        0        0     1410 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/dsdl_py_library/example.py
--rw-rw-rw-   0        0        0      313 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/exception.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/geometry/
--rw-rw-rw-   0        0        0      601 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/geometry/__init__.py
--rw-rw-rw-   0        0        0      635 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/geometry/attrbutes.py
--rw-rw-rw-   0        0        0      174 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/geometry/base_geometry.py
--rw-rw-rw-   0        0        0     2288 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/geometry/box.py
--rw-rw-rw-   0        0        0     2820 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/geometry/class_domain.py
--rw-rw-rw-   0        0        0     1100 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/geometry/class_domain_attributes.py
--rw-rw-rw-   0        0        0     3299 2022-11-01 04:32:13.000000 dsdl-0.1.9.3/dsdl/geometry/keypoint.py
--rw-rw-rw-   0        0        0     5046 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/geometry/label.py
--rw-rw-rw-   0        0        0     1028 2022-10-20 13:05:25.000000 dsdl-0.1.9.3/dsdl/geometry/media.py
--rw-rw-rw-   0        0        0     2341 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/geometry/polygon.py
--rw-rw-rw-   0        0        0     1851 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/geometry/registry.py
--rw-rw-rw-   0        0        0     2205 2022-10-26 09:39:49.000000 dsdl-0.1.9.3/dsdl/geometry/segmap.py
--rw-rw-rw-   0        0        0     2110 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/geometry/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/objectio/
--rw-rw-rw-   0        0        0      142 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/objectio/__init__.py
--rw-rw-rw-   0        0        0      852 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/objectio/ali_oss.py
--rw-rw-rw-   0        0        0      234 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/objectio/base.py
--rw-rw-rw-   0        0        0      333 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/objectio/local.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/parser/
--rw-rw-rw-   0        0        0       88 2022-09-20 09:26:25.000000 dsdl-0.1.9.3/dsdl/parser/__init__.py
--rw-rw-rw-   0        0        0     4927 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/parser/parse_class.py
--rw-rw-rw-   0        0        0    10829 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/parser/parse_field.py
--rw-rw-rw-   0        0        0    10614 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/parser/parse_params.py
--rw-rw-rw-   0        0        0    15362 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/parser/parser.py
--rw-rw-rw-   0        0        0     2349 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/parser/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/tools/
--rw-rw-rw-   0        0        0       60 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/tools/__init__.py
--rw-rw-rw-   0        0        0     3270 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/tools/commons.py
--rw-rw-rw-   0        0        0     4157 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/tools/visualize.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl/types/
--rw-rw-rw-   0        0        0      675 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/types/__init__.py
--rw-rw-rw-   0        0        0      506 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/types/field.py
--rw-rw-rw-   0        0        0     1683 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/dsdl/types/generic.py
--rw-rw-rw-   0        0        0     3422 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/types/special.py
--rw-rw-rw-   0        0        0     3372 2022-10-31 07:44:23.000000 dsdl-0.1.9.3/dsdl/types/struct.py
--rw-rw-rw-   0        0        0     1404 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/types/unstructure.py
--rw-rw-rw-   0        0        0      231 2022-10-18 06:09:44.000000 dsdl-0.1.9.3/dsdl/warning.py
-drwxrwxrwx   0        0        0        0 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/
--rw-rw-rw-   0        0        0     6664 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/dsdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-01 04:37:42.000000 dsdl-0.1.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1273 2022-09-16 10:04:08.000000 dsdl-0.1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/
+-rw-rw-rw-   0        0        0    11604 2022-09-19 02:10:48.000000 dsdl-0.1.9.4/LICENSE
+-rw-rw-rw-   0        0        0     6664 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6280 2022-09-20 09:26:25.000000 dsdl-0.1.9.4/README.md
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/
+-rw-rw-rw-   0        0        0      211 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/__init__.py
+-rw-rw-rw-   0        0        0      117 2022-11-01 12:19:46.000000 dsdl-0.1.9.4/dsdl/__version__.py
+-rw-rw-rw-   0        0        0      283 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/cli.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/dataset/
+-rw-rw-rw-   0        0        0      259 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dataset/__init__.py
+-rw-rw-rw-   0        0        0     3796 2022-10-31 07:44:22.000000 dsdl-0.1.9.4/dsdl/dataset/base_dataset.py
+-rw-rw-rw-   0        0        0      336 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dataset/demo_dataset.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/dataset/utils/
+-rw-rw-rw-   0        0        0      162 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0     1792 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dataset/utils/commons.py
+-rw-rw-rw-   0        0        0     1737 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dataset/utils/parser.py
+-rw-rw-rw-   0        0        0     6835 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/dataset/utils/visualizer.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/dsdl_py_library/
+-rw-rw-rw-   0        0        0      684 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dsdl_py_library/CIFAR10_test_data.py
+-rw-rw-rw-   0        0        0        0 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dsdl_py_library/__init__.py
+-rw-rw-rw-   0        0        0     1410 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/dsdl_py_library/example.py
+-rw-rw-rw-   0        0        0      313 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/exception.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/geometry/
+-rw-rw-rw-   0        0        0      601 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/geometry/__init__.py
+-rw-rw-rw-   0        0        0      635 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/geometry/attrbutes.py
+-rw-rw-rw-   0        0        0      174 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/geometry/base_geometry.py
+-rw-rw-rw-   0        0        0     2288 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/geometry/box.py
+-rw-rw-rw-   0        0        0     2820 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/geometry/class_domain.py
+-rw-rw-rw-   0        0        0     1100 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/geometry/class_domain_attributes.py
+-rw-rw-rw-   0        0        0     3358 2022-11-01 12:20:31.000000 dsdl-0.1.9.4/dsdl/geometry/keypoint.py
+-rw-rw-rw-   0        0        0     5046 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/geometry/label.py
+-rw-rw-rw-   0        0        0     1028 2022-10-20 13:05:25.000000 dsdl-0.1.9.4/dsdl/geometry/media.py
+-rw-rw-rw-   0        0        0     2341 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/geometry/polygon.py
+-rw-rw-rw-   0        0        0     1851 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/geometry/registry.py
+-rw-rw-rw-   0        0        0     2205 2022-10-26 09:39:49.000000 dsdl-0.1.9.4/dsdl/geometry/segmap.py
+-rw-rw-rw-   0        0        0     2110 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/geometry/utils.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/objectio/
+-rw-rw-rw-   0        0        0      142 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/objectio/__init__.py
+-rw-rw-rw-   0        0        0      852 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/objectio/ali_oss.py
+-rw-rw-rw-   0        0        0      234 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/objectio/base.py
+-rw-rw-rw-   0        0        0      333 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/objectio/local.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/parser/
+-rw-rw-rw-   0        0        0       88 2022-09-20 09:26:25.000000 dsdl-0.1.9.4/dsdl/parser/__init__.py
+-rw-rw-rw-   0        0        0     4927 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/parser/parse_class.py
+-rw-rw-rw-   0        0        0    10829 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/parser/parse_field.py
+-rw-rw-rw-   0        0        0    10614 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/parser/parse_params.py
+-rw-rw-rw-   0        0        0    15362 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/parser/parser.py
+-rw-rw-rw-   0        0        0     2349 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/parser/utils.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/tools/
+-rw-rw-rw-   0        0        0       60 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/tools/__init__.py
+-rw-rw-rw-   0        0        0     3270 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/tools/commons.py
+-rw-rw-rw-   0        0        0     4157 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/tools/visualize.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl/types/
+-rw-rw-rw-   0        0        0      675 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/types/__init__.py
+-rw-rw-rw-   0        0        0      506 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/types/field.py
+-rw-rw-rw-   0        0        0     1683 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/dsdl/types/generic.py
+-rw-rw-rw-   0        0        0     3422 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/types/special.py
+-rw-rw-rw-   0        0        0     3372 2022-10-31 07:44:23.000000 dsdl-0.1.9.4/dsdl/types/struct.py
+-rw-rw-rw-   0        0        0     1404 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/types/unstructure.py
+-rw-rw-rw-   0        0        0      231 2022-10-18 06:09:44.000000 dsdl-0.1.9.4/dsdl/warning.py
+drwxrwxrwx   0        0        0        0 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/
+-rw-rw-rw-   0        0        0     6664 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      111 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/dsdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-01 12:20:51.000000 dsdl-0.1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2022-09-16 10:04:08.000000 dsdl-0.1.9.4/setup.py
```

### Comparing `dsdl-0.1.9.3/LICENSE` & `dsdl-0.1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/PKG-INFO` & `dsdl-0.1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsdl
-Version: 0.1.9.3
+Version: 0.1.9.4
 Summary: Python SDK for DSDL
 Author: DSDL team
 Author-email: dsdl-team@pjlab.org.cn
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsdl Version: 0.1.9.3 Summary: Python SDK for DSDL
+Metadata-Version: 2.1 Name: dsdl Version: 0.1.9.4 Summary: Python SDK for DSDL
 Author: DSDL team Author-email: dsdl-team@pjlab.org.cn Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                           [resources/opendatalab.svg]
                                         
                          OpenDataLab website HOT
```

### Comparing `dsdl-0.1.9.3/README.md` & `dsdl-0.1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/dataset/base_dataset.py` & `dsdl-0.1.9.4/dsdl/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/dataset/utils/commons.py` & `dsdl-0.1.9.4/dsdl/dataset/utils/commons.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/dataset/utils/parser.py` & `dsdl-0.1.9.4/dsdl/dataset/utils/parser.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/dataset/utils/visualizer.py` & `dsdl-0.1.9.4/dsdl/dataset/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/dsdl_py_library/CIFAR10_test_data.py` & `dsdl-0.1.9.4/dsdl/dsdl_py_library/CIFAR10_test_data.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/dsdl_py_library/example.py` & `dsdl-0.1.9.4/dsdl/dsdl_py_library/example.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/__init__.py` & `dsdl-0.1.9.4/dsdl/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/attrbutes.py` & `dsdl-0.1.9.4/dsdl/geometry/attrbutes.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/box.py` & `dsdl-0.1.9.4/dsdl/geometry/box.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/class_domain.py` & `dsdl-0.1.9.4/dsdl/geometry/class_domain.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/class_domain_attributes.py` & `dsdl-0.1.9.4/dsdl/geometry/class_domain_attributes.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/keypoint.py` & `dsdl-0.1.9.4/dsdl/geometry/keypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,7 +105,10 @@
                     palette[label_] = tuple(np.random.randint(0, 255, size=[3]))
                 point_color = palette[label_]
                 x, y = point.point
                 draw_obj.ellipse((x - point_radius, y - point_radius, x + point_radius, y + point_radius),
                                  fill=(*point_color, 255))
         del draw_obj
         return image
+
+    def __repr__(self):
+        return str(self.value)
```

### Comparing `dsdl-0.1.9.3/dsdl/geometry/label.py` & `dsdl-0.1.9.4/dsdl/geometry/label.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/media.py` & `dsdl-0.1.9.4/dsdl/geometry/media.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/polygon.py` & `dsdl-0.1.9.4/dsdl/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/registry.py` & `dsdl-0.1.9.4/dsdl/geometry/registry.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/segmap.py` & `dsdl-0.1.9.4/dsdl/geometry/segmap.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/geometry/utils.py` & `dsdl-0.1.9.4/dsdl/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/objectio/ali_oss.py` & `dsdl-0.1.9.4/dsdl/objectio/ali_oss.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/parser/parse_class.py` & `dsdl-0.1.9.4/dsdl/parser/parse_class.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/parser/parse_field.py` & `dsdl-0.1.9.4/dsdl/parser/parse_field.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/parser/parse_params.py` & `dsdl-0.1.9.4/dsdl/parser/parse_params.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/parser/parser.py` & `dsdl-0.1.9.4/dsdl/parser/parser.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/parser/utils.py` & `dsdl-0.1.9.4/dsdl/parser/utils.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/tools/commons.py` & `dsdl-0.1.9.4/dsdl/tools/commons.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/tools/visualize.py` & `dsdl-0.1.9.4/dsdl/tools/visualize.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/types/__init__.py` & `dsdl-0.1.9.4/dsdl/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/types/generic.py` & `dsdl-0.1.9.4/dsdl/types/generic.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/types/special.py` & `dsdl-0.1.9.4/dsdl/types/special.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/types/struct.py` & `dsdl-0.1.9.4/dsdl/types/struct.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl/types/unstructure.py` & `dsdl-0.1.9.4/dsdl/types/unstructure.py`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/dsdl.egg-info/PKG-INFO` & `dsdl-0.1.9.4/dsdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsdl
-Version: 0.1.9.3
+Version: 0.1.9.4
 Summary: Python SDK for DSDL
 Author: DSDL team
 Author-email: dsdl-team@pjlab.org.cn
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsdl Version: 0.1.9.3 Summary: Python SDK for DSDL
+Metadata-Version: 2.1 Name: dsdl Version: 0.1.9.4 Summary: Python SDK for DSDL
 Author: DSDL team Author-email: dsdl-team@pjlab.org.cn Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                           [resources/opendatalab.svg]
                                         
                          OpenDataLab website HOT
```

### Comparing `dsdl-0.1.9.3/dsdl.egg-info/SOURCES.txt` & `dsdl-0.1.9.4/dsdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsdl-0.1.9.3/setup.py` & `dsdl-0.1.9.4/setup.py`

 * *Files identical despite different names*

