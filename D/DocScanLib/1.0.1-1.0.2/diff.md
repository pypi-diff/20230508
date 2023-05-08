# Comparing `tmp/DocScanLib-1.0.1.tar.gz` & `tmp/DocScanLib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DocScanLib-1.0.1.tar", last modified: Mon May  8 12:57:32 2023, max compression
+gzip compressed data, was "DocScanLib-1.0.2.tar", last modified: Mon May  8 13:17:46 2023, max compression
```

## Comparing `DocScanLib-1.0.1.tar` & `DocScanLib-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:57:32.546887 DocScanLib-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-08 12:57:32.546887 DocScanLib-1.0.1/DocScanLib.egg-info/
--rw-rw-rw-   0        0        0      619 2023-05-08 12:57:32.000000 DocScanLib-1.0.1/DocScanLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-08 12:57:32.000000 DocScanLib-1.0.1/DocScanLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:57:32.000000 DocScanLib-1.0.1/DocScanLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      288 2023-05-08 12:57:32.000000 DocScanLib-1.0.1/DocScanLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:57:32.000000 DocScanLib-1.0.1/DocScanLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      169 2023-05-08 12:57:19.000000 DocScanLib-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      619 2023-05-08 12:57:32.546887 DocScanLib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-08 12:34:33.000000 DocScanLib-1.0.1/README.md
--rw-rw-rw-   0        0        0     2476 2023-05-07 18:11:36.000000 DocScanLib-1.0.1/doc_denoiser.py
--rw-rw-rw-   0        0        0     2984 2023-05-06 11:53:20.000000 DocScanLib-1.0.1/doc_detector.py
--rw-rw-rw-   0        0        0      971 2023-05-06 12:10:48.000000 DocScanLib-1.0.1/doc_frames_blender.py
--rw-rw-rw-   0        0        0     1971 2023-05-07 16:04:43.000000 DocScanLib-1.0.1/model.py
--rw-rw-rw-   0        0        0       42 2023-05-08 12:57:32.546887 DocScanLib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-05-08 12:57:19.000000 DocScanLib-1.0.1/setup.py
--rw-rw-rw-   0        0        0   756008 2023-05-07 15:53:31.000000 DocScanLib-1.0.1/state.pth
--rw-rw-rw-   0        0        0      957 2023-05-06 10:24:44.000000 DocScanLib-1.0.1/video_frame_extractor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:17:46.271996 DocScanLib-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-08 13:17:46.271996 DocScanLib-1.0.2/DocScanLib.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-05-08 13:17:46.000000 DocScanLib-1.0.2/DocScanLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-08 13:17:46.000000 DocScanLib-1.0.2/DocScanLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:17:46.000000 DocScanLib-1.0.2/DocScanLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      288 2023-05-08 13:17:46.000000 DocScanLib-1.0.2/DocScanLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:17:46.000000 DocScanLib-1.0.2/DocScanLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      169 2023-05-08 12:57:19.000000 DocScanLib-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      619 2023-05-08 13:17:46.271996 DocScanLib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-08 12:34:33.000000 DocScanLib-1.0.2/README.md
+-rw-rw-rw-   0        0        0     2476 2023-05-07 18:11:36.000000 DocScanLib-1.0.2/doc_denoiser.py
+-rw-rw-rw-   0        0        0     2984 2023-05-06 11:53:20.000000 DocScanLib-1.0.2/doc_detector.py
+-rw-rw-rw-   0        0        0      971 2023-05-06 12:10:48.000000 DocScanLib-1.0.2/doc_frames_blender.py
+-rw-rw-rw-   0        0        0     1971 2023-05-07 16:04:43.000000 DocScanLib-1.0.2/model.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:17:46.271996 DocScanLib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-05-08 13:17:07.000000 DocScanLib-1.0.2/setup.py
+-rw-rw-rw-   0        0        0   756008 2023-05-07 15:53:31.000000 DocScanLib-1.0.2/state.pth
+-rw-rw-rw-   0        0        0      957 2023-05-06 10:24:44.000000 DocScanLib-1.0.2/video_frame_extractor.py
```

### Comparing `DocScanLib-1.0.1/DocScanLib.egg-info/PKG-INFO` & `DocScanLib-1.0.2/DocScanLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DocScanLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for scanning documents
 Home-page: https://pypi.org/project/DocScanLib/
 Author: diburakov
 Author-email: daniel.elder@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DocScanLib-1.0.1/PKG-INFO` & `DocScanLib-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DocScanLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for scanning documents
 Home-page: https://pypi.org/project/DocScanLib/
 Author: diburakov
 Author-email: daniel.elder@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DocScanLib-1.0.1/doc_denoiser.py` & `DocScanLib-1.0.2/doc_denoiser.py`

 * *Files identical despite different names*

### Comparing `DocScanLib-1.0.1/doc_detector.py` & `DocScanLib-1.0.2/doc_detector.py`

 * *Files identical despite different names*

### Comparing `DocScanLib-1.0.1/doc_frames_blender.py` & `DocScanLib-1.0.2/doc_frames_blender.py`

 * *Files identical despite different names*

### Comparing `DocScanLib-1.0.1/model.py` & `DocScanLib-1.0.2/model.py`

 * *Files identical despite different names*

### Comparing `DocScanLib-1.0.1/setup.py` & `DocScanLib-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="DocScanLib",
-    version="1.0.1",
+    version="1.0.2",
     author="diburakov",
     author_email="daniel.elder@yandex.ru",
     description="Library for scanning documents",
     long_description="This library is used for scanning documents using video stream. It contains modules for "
                      "cutting video stream into frames. detect documents on frames, blend document frames into one and "
                      "denoise it.",
     long_description_content_type="",
```

### Comparing `DocScanLib-1.0.1/state.pth` & `DocScanLib-1.0.2/state.pth`

 * *Files identical despite different names*

### Comparing `DocScanLib-1.0.1/video_frame_extractor.py` & `DocScanLib-1.0.2/video_frame_extractor.py`

 * *Files identical despite different names*

