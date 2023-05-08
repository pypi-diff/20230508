# Comparing `tmp/Lab93DatabaseSystem-0.0.1.tar.gz` & `tmp/Lab93DatabaseSystem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93DatabaseSystem-0.0.1.tar", last modified: Tue Apr 18 18:29:58 2023, max compression
+gzip compressed data, was "Lab93DatabaseSystem-0.0.2.tar", last modified: Mon May  8 13:06:35 2023, max compression
```

## Comparing `Lab93DatabaseSystem-0.0.1.tar` & `Lab93DatabaseSystem-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-04-18 18:29:58.301963 Lab93DatabaseSystem-0.0.1/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      554 2023-04-18 18:29:58.301963 Lab93DatabaseSystem-0.0.1/PKG-INFO
--rw-r--r--   0 hunter    (1000) hunter    (1000)      651 2023-04-18 18:28:50.000000 Lab93DatabaseSystem-0.0.1/pyproject.toml
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2023-04-18 18:29:58.301963 Lab93DatabaseSystem-0.0.1/setup.cfg
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-04-18 18:29:58.289963 Lab93DatabaseSystem-0.0.1/src/
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-04-18 18:29:58.293963 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem/
--rw-r--r--   0 hunter    (1000) hunter    (1000)        0 2023-04-18 17:56:35.000000 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem/__init__.py
--rw-r--r--   0 hunter    (1000) hunter    (1000)     7080 2023-04-18 18:08:34.000000 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem/dbSystem.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-04-18 18:29:58.297963 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem.egg-info/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      554 2023-04-18 18:29:58.000000 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem.egg-info/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      274 2023-04-18 18:29:58.000000 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2023-04-18 18:29:58.000000 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       20 2023-04-18 18:29:58.000000 Lab93DatabaseSystem-0.0.1/src/Lab93DatabaseSystem.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2505 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      652 2023-05-08 13:03:57.000000 Lab93DatabaseSystem-0.0.2/pyproject.toml
+-rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)     1950 2023-04-19 18:29:25.000000 Lab93DatabaseSystem-0.0.2/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.582907 Lab93DatabaseSystem-0.0.2/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.586241 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5722 2023-05-08 12:36:38.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.592908 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     7444 2023-05-08 12:55:53.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-08 12:54:50.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-04-21 17:54:30.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 12:40:34.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.589574 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/
+-rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)     2505 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/PKG-INFO
+-rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
+-rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
+-rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/top_level.txt
```

### Comparing `Lab93DatabaseSystem-0.0.1/pyproject.toml` & `Lab93DatabaseSystem-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93DatabaseSystem"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "An API for interfacing with SQLite3 databases from the command line."
 readme = "readme.md"
 requires-python = ">=3.10"
@@ -16,8 +16,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/guyyatsu/Lab93-Database-System"
-"Bug Tracker" = "https://github.com/guyyatsu/Lab93-Database-System/issues"
+"Bug Tracker" = "https://github.com/guyyatsu/Lab93-Database-System/issues"
```

