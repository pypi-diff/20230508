# Comparing `tmp/Package_Name_Example-0.1.tar.gz` & `tmp/package_name_example-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Package_Name_Example-0.1.tar", last modified: Mon May  8 12:19:51 2023, max compression
+gzip compressed data, was "package_name_example-1.0.0.tar", last modified: Mon May  8 12:41:39 2023, max compression
```

## Comparing `Package_Name_Example-0.1.tar` & `package_name_example-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-08 12:19:51.887918 Package_Name_Example-0.1/
--rw-rw-r--   0 user      (1000) user      (1000)      353 2023-05-08 12:19:51.887918 Package_Name_Example-0.1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-08 12:19:51.887918 Package_Name_Example-0.1/Package_Name_Example.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      353 2023-05-08 12:19:51.000000 Package_Name_Example-0.1/Package_Name_Example.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      184 2023-05-08 12:19:51.000000 Package_Name_Example-0.1/Package_Name_Example.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-08 12:19:51.000000 Package_Name_Example-0.1/Package_Name_Example.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-08 12:19:51.000000 Package_Name_Example-0.1/Package_Name_Example.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-08 12:19:51.887918 Package_Name_Example-0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-05-08 12:17:41.000000 Package_Name_Example-0.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-08 12:41:39.411291 package_name_example-1.0.0/
+-rw-rw-r--   0 user      (1000) user      (1000)      355 2023-05-08 12:41:39.411291 package_name_example-1.0.0/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-08 12:41:39.411291 package_name_example-1.0.0/package_name_example.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      355 2023-05-08 12:41:39.000000 package_name_example-1.0.0/package_name_example.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      184 2023-05-08 12:41:39.000000 package_name_example-1.0.0/package_name_example.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-08 12:41:39.000000 package_name_example-1.0.0/package_name_example.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-08 12:41:39.000000 package_name_example-1.0.0/package_name_example.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-08 12:41:39.411291 package_name_example-1.0.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      399 2023-05-08 12:41:09.000000 package_name_example-1.0.0/setup.py
```

