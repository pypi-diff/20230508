# Comparing `tmp/visual-compare-0.1.0.tar.gz` & `tmp/visual-compare-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-compare-0.1.0.tar", last modified: Mon May  8 07:02:47 2023, max compression
+gzip compressed data, was "visual-compare-0.1.1.tar", last modified: Mon May  8 07:13:21 2023, max compression
```

## Comparing `visual-compare-0.1.0.tar` & `visual-compare-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:02:47.047294 visual-compare-0.1.0/
--rw-rw-rw-   0        0        0      928 2023-05-08 07:02:47.047294 visual-compare-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-05-08 03:46:52.000000 visual-compare-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 07:02:47.047294 visual-compare-0.1.0/doc/
--rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.0/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:02:47.047294 visual-compare-0.1.0/doc/image/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.0/doc/image/__init__.py
--rw-rw-rw-   0        0        0    28334 2023-05-08 02:01:53.000000 visual-compare-0.1.0/doc/image/compare_image.py
--rw-rw-rw-   0        0        0     1912 2023-05-08 02:42:08.000000 visual-compare-0.1.0/doc/image/image.py
--rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.0/doc/image/ocr.py
--rw-rw-rw-   0        0        0    55668 2023-05-08 07:00:09.000000 visual-compare-0.1.0/doc/visual_test.py
--rw-rw-rw-   0        0        0      145 2023-05-08 07:02:47.047294 visual-compare-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-05-08 03:44:57.000000 visual-compare-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:02:47.047294 visual-compare-0.1.0/utils/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.0/utils/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-05-06 02:31:44.000000 visual-compare-0.1.0/utils/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:02:47.047294 visual-compare-0.1.0/visual_compare.egg-info/
--rw-rw-rw-   0        0        0      928 2023-05-08 07:02:46.000000 visual-compare-0.1.0/visual_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-08 07:02:47.000000 visual-compare-0.1.0/visual_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:02:47.000000 visual-compare-0.1.0/visual_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.0/visual_compare.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-05-08 07:02:47.000000 visual-compare-0.1.0/visual_compare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 07:13:21.410945 visual-compare-0.1.1/
+-rw-rw-rw-   0        0        0      928 2023-05-08 07:13:21.410945 visual-compare-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-05-08 03:46:52.000000 visual-compare-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 07:13:21.405318 visual-compare-0.1.1/doc/
+-rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.1/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:13:21.410945 visual-compare-0.1.1/doc/image/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.1/doc/image/__init__.py
+-rw-rw-rw-   0        0        0    28334 2023-05-08 02:01:53.000000 visual-compare-0.1.1/doc/image/compare_image.py
+-rw-rw-rw-   0        0        0     1912 2023-05-08 02:42:08.000000 visual-compare-0.1.1/doc/image/image.py
+-rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.1/doc/image/ocr.py
+-rw-rw-rw-   0        0        0    55668 2023-05-08 07:00:09.000000 visual-compare-0.1.1/doc/visual_test.py
+-rw-rw-rw-   0        0        0      145 2023-05-08 07:13:21.410945 visual-compare-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-05-08 07:13:17.000000 visual-compare-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:13:21.410945 visual-compare-0.1.1/utils/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.1/utils/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-05-06 02:31:44.000000 visual-compare-0.1.1/utils/downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:13:21.410945 visual-compare-0.1.1/visual_compare.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-05-08 07:13:21.000000 visual-compare-0.1.1/visual_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-08 07:13:21.000000 visual-compare-0.1.1/visual_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:13:21.000000 visual-compare-0.1.1/visual_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.1/visual_compare.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-05-08 07:13:21.000000 visual-compare-0.1.1/visual_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 07:13:21.000000 visual-compare-0.1.1/visual_compare.egg-info/top_level.txt
```

### Comparing `visual-compare-0.1.0/PKG-INFO` & `visual-compare-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 0.1.0
+Version: 0.1.1
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
```

### Comparing `visual-compare-0.1.0/doc/image/compare_image.py` & `visual-compare-0.1.1/doc/image/compare_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.0/doc/image/image.py` & `visual-compare-0.1.1/doc/image/image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.0/doc/image/ocr.py` & `visual-compare-0.1.1/doc/image/ocr.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.0/doc/visual_test.py` & `visual-compare-0.1.1/doc/visual_test.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.0/setup.py` & `visual-compare-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="visual-compare",
-    version="0.1.0",
+    version="0.1.1",
     description="Image and PDF Compare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/visual-compare",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
@@ -28,10 +28,20 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="visual compare image pdf diff",
     packages=find_packages(exclude=("tests",)),
     install_requires=[
+        "opencv-python-headless~=4.7",
+        "numpy~=1.24.3",
+        "imutils~=0.5.4",
+        "scikit-image~=0.20",
+        "pytesseract~=0.3.10",
+        "parsimonious~=0.10",
+        "PyMuPDF~=1.22",
+        "pyzbar~=0.1.9",
+        "pylibdmtx~=0.1.10",
+        "Wand~=0.6.11"
     ],
     zip_safe=False,
 )
```

### Comparing `visual-compare-0.1.0/utils/downloader.py` & `visual-compare-0.1.1/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.0/visual_compare.egg-info/PKG-INFO` & `visual-compare-0.1.1/visual_compare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 0.1.0
+Version: 0.1.1
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
```

