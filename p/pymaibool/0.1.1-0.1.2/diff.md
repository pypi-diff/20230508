# Comparing `tmp/pymaibool-0.1.1.tar.gz` & `tmp/pymaibool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymaibool-0.1.1.tar", last modified: Mon May  8 03:12:07 2023, max compression
+gzip compressed data, was "pymaibool-0.1.2.tar", last modified: Mon May  8 03:14:26 2023, max compression
```

## Comparing `pymaibool-0.1.1.tar` & `pymaibool-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:12:07.979928 pymaibool-0.1.1/
--rw-r--r--   0 torisan4   (501) staff       (20)     1067 2023-05-08 03:02:42.000000 pymaibool-0.1.1/LICENSE
--rw-r--r--   0 torisan4   (501) staff       (20)     1039 2023-05-08 03:12:07.979810 pymaibool-0.1.1/PKG-INFO
--rw-r--r--   0 torisan4   (501) staff       (20)      850 2023-05-08 03:11:22.000000 pymaibool-0.1.1/README.md
-drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:12:07.978838 pymaibool-0.1.1/pymaibool/
--rw-r--r--   0 torisan4   (501) staff       (20)       33 2023-05-08 02:57:21.000000 pymaibool-0.1.1/pymaibool/__init__.py
--rw-r--r--   0 torisan4   (501) staff       (20)     1501 2023-05-08 02:50:31.000000 pymaibool-0.1.1/pymaibool/pymaibool.py
-drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:12:07.979451 pymaibool-0.1.1/pymaibool.egg-info/
--rw-r--r--   0 torisan4   (501) staff       (20)     1039 2023-05-08 03:12:07.000000 pymaibool-0.1.1/pymaibool.egg-info/PKG-INFO
--rw-r--r--   0 torisan4   (501) staff       (20)      216 2023-05-08 03:12:07.000000 pymaibool-0.1.1/pymaibool.egg-info/SOURCES.txt
--rw-r--r--   0 torisan4   (501) staff       (20)        1 2023-05-08 03:12:07.000000 pymaibool-0.1.1/pymaibool.egg-info/dependency_links.txt
--rw-r--r--   0 torisan4   (501) staff       (20)       10 2023-05-08 03:12:07.000000 pymaibool-0.1.1/pymaibool.egg-info/top_level.txt
--rw-r--r--   0 torisan4   (501) staff       (20)       38 2023-05-08 03:12:07.979975 pymaibool-0.1.1/setup.cfg
--rw-r--r--   0 torisan4   (501) staff       (20)      369 2023-05-08 03:11:15.000000 pymaibool-0.1.1/setup.py
-drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:12:07.979557 pymaibool-0.1.1/test/
--rw-r--r--   0 torisan4   (501) staff       (20)      150 2023-05-08 03:11:52.000000 pymaibool-0.1.1/test/test.py
+drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:14:26.121303 pymaibool-0.1.2/
+-rw-r--r--   0 torisan4   (501) staff       (20)     1067 2023-05-08 03:02:42.000000 pymaibool-0.1.2/LICENSE
+-rw-r--r--   0 torisan4   (501) staff       (20)     1044 2023-05-08 03:14:26.121189 pymaibool-0.1.2/PKG-INFO
+-rw-r--r--   0 torisan4   (501) staff       (20)      855 2023-05-08 03:13:54.000000 pymaibool-0.1.2/README.md
+drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:14:26.120255 pymaibool-0.1.2/pymaibool/
+-rw-r--r--   0 torisan4   (501) staff       (20)       33 2023-05-08 02:57:21.000000 pymaibool-0.1.2/pymaibool/__init__.py
+-rw-r--r--   0 torisan4   (501) staff       (20)     1501 2023-05-08 02:50:31.000000 pymaibool-0.1.2/pymaibool/pymaibool.py
+drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:14:26.120824 pymaibool-0.1.2/pymaibool.egg-info/
+-rw-r--r--   0 torisan4   (501) staff       (20)     1044 2023-05-08 03:14:26.000000 pymaibool-0.1.2/pymaibool.egg-info/PKG-INFO
+-rw-r--r--   0 torisan4   (501) staff       (20)      216 2023-05-08 03:14:26.000000 pymaibool-0.1.2/pymaibool.egg-info/SOURCES.txt
+-rw-r--r--   0 torisan4   (501) staff       (20)        1 2023-05-08 03:14:26.000000 pymaibool-0.1.2/pymaibool.egg-info/dependency_links.txt
+-rw-r--r--   0 torisan4   (501) staff       (20)       10 2023-05-08 03:14:26.000000 pymaibool-0.1.2/pymaibool.egg-info/top_level.txt
+-rw-r--r--   0 torisan4   (501) staff       (20)       38 2023-05-08 03:14:26.121344 pymaibool-0.1.2/setup.cfg
+-rw-r--r--   0 torisan4   (501) staff       (20)      369 2023-05-08 03:14:01.000000 pymaibool-0.1.2/setup.py
+drwxr-xr-x   0 torisan4   (501) staff       (20)        0 2023-05-08 03:14:26.120935 pymaibool-0.1.2/test/
+-rw-r--r--   0 torisan4   (501) staff       (20)      150 2023-05-08 03:11:52.000000 pymaibool-0.1.2/test/test.py
```

### Comparing `pymaibool-0.1.1/LICENSE` & `pymaibool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymaibool-0.1.1/PKG-INFO` & `pymaibool-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pymaibool
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pymy
+# pymaibool
 
 ## Overview
 pymaibool is a library for adding ambiguity to bool.  
 
 ## Usage
 ```python
 from pymaibool import pBool
@@ -90,12 +90,12 @@
 False
 True
 False
 True
 ```
 
 ## version
-0.1.1
+0.1.2
 
 ## Github
 https://github.com/toripppppy/pymaibool
```

### Comparing `pymaibool-0.1.1/README.md` & `pymaibool-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pymy
+# pymaibool
 
 ## Overview
 pymaibool is a library for adding ambiguity to bool.  
 
 ## Usage
 ```python
 from pymaibool import pBool
@@ -80,11 +80,11 @@
 False
 True
 False
 True
 ```
 
 ## version
-0.1.1
+0.1.2
 
 ## Github
 https://github.com/toripppppy/pymaibool
```

### Comparing `pymaibool-0.1.1/pymaibool/pymaibool.py` & `pymaibool-0.1.2/pymaibool/pymaibool.py`

 * *Files identical despite different names*

### Comparing `pymaibool-0.1.1/pymaibool.egg-info/PKG-INFO` & `pymaibool-0.1.2/pymaibool.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pymaibool
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pymy
+# pymaibool
 
 ## Overview
 pymaibool is a library for adding ambiguity to bool.  
 
 ## Usage
 ```python
 from pymaibool import pBool
@@ -90,12 +90,12 @@
 False
 True
 False
 True
 ```
 
 ## version
-0.1.1
+0.1.2
 
 ## Github
 https://github.com/toripppppy/pymaibool
```

