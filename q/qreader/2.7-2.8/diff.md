# Comparing `tmp/qreader-2.7.tar.gz` & `tmp/qreader-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qreader-2.7.tar", last modified: Thu Feb  2 13:58:01 2023, max compression
+gzip compressed data, was "qreader-2.8.tar", last modified: Thu Feb  2 14:08:30 2023, max compression
```

## Comparing `qreader-2.7.tar` & `qreader-2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-02 13:58:01.156789 qreader-2.7/
--rw-rw-rw-   0        0        0     1089 2022-12-03 14:38:15.000000 qreader-2.7/LICENSE
--rw-rw-rw-   0        0        0     9136 2023-02-02 13:58:01.156789 qreader-2.7/PKG-INFO
--rw-rw-rw-   0        0        0     8241 2023-01-30 10:28:52.000000 qreader-2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-02 13:58:01.156789 qreader-2.7/qreader.egg-info/
--rw-rw-rw-   0        0        0     9136 2023-02-02 13:58:00.000000 qreader-2.7/qreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-02-02 13:58:00.000000 qreader-2.7/qreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-02 13:58:00.000000 qreader-2.7/qreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-02-02 13:58:00.000000 qreader-2.7/qreader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-02-02 13:58:00.000000 qreader-2.7/qreader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5750 2023-01-30 09:56:09.000000 qreader-2.7/qreader.py
--rw-rw-rw-   0        0        0      111 2023-02-02 13:58:01.156789 qreader-2.7/setup.cfg
--rw-rw-rw-   0        0        0     1257 2023-02-02 13:57:57.000000 qreader-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-02 14:08:30.686262 qreader-2.8/
+-rw-rw-rw-   0        0        0     1089 2022-12-03 14:38:15.000000 qreader-2.8/LICENSE
+-rw-rw-rw-   0        0        0     9136 2023-02-02 14:08:30.686262 qreader-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8241 2023-01-30 10:28:52.000000 qreader-2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-02-02 14:08:30.686262 qreader-2.8/qreader.egg-info/
+-rw-rw-rw-   0        0        0     9136 2023-02-02 14:08:30.000000 qreader-2.8/qreader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-02-02 14:08:30.000000 qreader-2.8/qreader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-02 14:08:30.000000 qreader-2.8/qreader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-02-02 14:08:30.000000 qreader-2.8/qreader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-02-02 14:08:30.000000 qreader-2.8/qreader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5759 2023-02-02 14:07:48.000000 qreader-2.8/qreader.py
+-rw-rw-rw-   0        0        0      111 2023-02-02 14:08:30.701958 qreader-2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2023-02-02 14:08:24.000000 qreader-2.8/setup.py
```

### Comparing `qreader-2.7/LICENSE` & `qreader-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qreader-2.7/PKG-INFO` & `qreader-2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qreader
-Version: 2.7
+Version: 2.8
 Summary: Robust and Straight-Forward solution for reading difficult and tricky QR codes within images in Python. Supported by a YOLOv7 QR Detection model.
 Home-page: https://github.com/Eric-Canas/qreader
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qreader Version: 2.7 Summary: Robust and Straight-
+Metadata-Version: 2.1 Name: qreader Version: 2.8 Summary: Robust and Straight-
 Forward solution for reading difficult and tricky QR codes within images in
 Python. Supported by a YOLOv7 QR Detection model. Home-page: https://
 github.com/Eric-Canas/qreader Author: Eric Canas Author-email:
 elcorreodeharu@gmail.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `qreader-2.7/README.md` & `qreader-2.8/README.md`

 * *Files identical despite different names*

### Comparing `qreader-2.7/qreader.egg-info/PKG-INFO` & `qreader-2.8/qreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qreader
-Version: 2.7
+Version: 2.8
 Summary: Robust and Straight-Forward solution for reading difficult and tricky QR codes within images in Python. Supported by a YOLOv7 QR Detection model.
 Home-page: https://github.com/Eric-Canas/qreader
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qreader Version: 2.7 Summary: Robust and Straight-
+Metadata-Version: 2.1 Name: qreader Version: 2.8 Summary: Robust and Straight-
 Forward solution for reading difficult and tricky QR codes within images in
 Python. Supported by a YOLOv7 QR Detection model. Home-page: https://
 github.com/Eric-Canas/qreader Author: Eric Canas Author-email:
 elcorreodeharu@gmail.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `qreader-2.7/qreader.py` & `qreader-2.8/qreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from __future__ import annotations
 
 import numpy as np
 from pyzbar.pyzbar import decode as decodeQR, ZBarSymbol
 import cv2
 
 from qrdet import QRDetector
-_SHARPEN_KERNEL = np.array(((-1, -1, -1), (-1, 9, -1), (-1, -1, -1)), dtype=np.float32)
+_SHARPEN_KERNEL = np.array(((-1., -1., -1.), (-1., 9., -1.), (-1., -1., -1.)), dtype=np.float32)
 
 class QReader:
     def __init__(self):
         """
         This class implements a robust, ML Based QR detector & decoder.
         """
         self.detector = QRDetector()
```

### Comparing `qreader-2.7/setup.py` & `qreader-2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='qreader',
-    version='2.7',
+    version='2.8',
     packages=find_namespace_packages(),
     # expose qreader.py as the unique module
     py_modules=['qreader'],
     url='https://github.com/Eric-Canas/qreader',
     license='MIT',
     author='Eric Canas',
     author_email='elcorreodeharu@gmail.com',
```

