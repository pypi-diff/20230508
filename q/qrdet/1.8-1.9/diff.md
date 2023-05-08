# Comparing `tmp/qrdet-1.8.tar.gz` & `tmp/qrdet-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrdet-1.8.tar", last modified: Tue Jan 17 09:18:25 2023, max compression
+gzip compressed data, was "qrdet-1.9.tar", last modified: Thu Feb  2 13:42:10 2023, max compression
```

## Comparing `qrdet-1.8.tar` & `qrdet-1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 09:18:25.634366 qrdet-1.8/
--rw-rw-rw-   0        0        0     1089 2022-12-11 18:06:46.000000 qrdet-1.8/LICENSE
--rw-rw-rw-   0        0        0     3730 2023-01-17 09:18:25.634366 qrdet-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2804 2023-01-17 09:17:59.000000 qrdet-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-17 09:18:25.634366 qrdet-1.8/qrdet.egg-info/
--rw-rw-rw-   0        0        0     3730 2023-01-17 09:18:25.000000 qrdet-1.8/qrdet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-01-17 09:18:25.000000 qrdet-1.8/qrdet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 09:18:25.000000 qrdet-1.8/qrdet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-01-17 09:18:25.000000 qrdet-1.8/qrdet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-01-17 09:18:25.000000 qrdet-1.8/qrdet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6513 2023-01-16 22:47:21.000000 qrdet-1.8/qrdet.py
--rw-rw-rw-   0        0        0      111 2023-01-17 09:18:25.634366 qrdet-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1353 2023-01-17 09:17:52.000000 qrdet-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-02 13:42:10.370983 qrdet-1.9/
+-rw-rw-rw-   0        0        0     1089 2022-12-11 18:06:46.000000 qrdet-1.9/LICENSE
+-rw-rw-rw-   0        0        0     3730 2023-02-02 13:42:10.370983 qrdet-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2023-01-17 09:17:59.000000 qrdet-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-02 13:42:10.370983 qrdet-1.9/qrdet.egg-info/
+-rw-rw-rw-   0        0        0     3730 2023-02-02 13:42:10.000000 qrdet-1.9/qrdet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-02-02 13:42:10.000000 qrdet-1.9/qrdet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-02 13:42:10.000000 qrdet-1.9/qrdet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-02-02 13:42:10.000000 qrdet-1.9/qrdet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-02-02 13:42:10.000000 qrdet-1.9/qrdet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6915 2023-02-02 13:41:22.000000 qrdet-1.9/qrdet.py
+-rw-rw-rw-   0        0        0      111 2023-02-02 13:42:10.386877 qrdet-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1247 2023-02-02 13:41:22.000000 qrdet-1.9/setup.py
```

### Comparing `qrdet-1.8/LICENSE` & `qrdet-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qrdet-1.8/PKG-INFO` & `qrdet-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrdet
-Version: 1.8
+Version: 1.9
 Summary: Robust QR Detector based on YOLOv7
 Home-page: https://github.com/Eric-Canas/qrdet
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qrdet Version: 1.8 Summary: Robust QR Detector
+Metadata-Version: 2.1 Name: qrdet Version: 1.9 Summary: Robust QR Detector
 based on YOLOv7 Home-page: https://github.com/Eric-Canas/qrdet Author: Eric
 Canas Author-email: elcorreodeharu@gmail.com License: MIT Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Image Recognition Classifier: Topic ::
```

### Comparing `qrdet-1.8/README.md` & `qrdet-1.9/README.md`

 * *Files identical despite different names*

### Comparing `qrdet-1.8/qrdet.egg-info/PKG-INFO` & `qrdet-1.9/qrdet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrdet
-Version: 1.8
+Version: 1.9
 Summary: Robust QR Detector based on YOLOv7
 Home-page: https://github.com/Eric-Canas/qrdet
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qrdet Version: 1.8 Summary: Robust QR Detector
+Metadata-Version: 2.1 Name: qrdet Version: 1.9 Summary: Robust QR Detector
 based on YOLOv7 Home-page: https://github.com/Eric-Canas/qrdet Author: Eric
 Canas Author-email: elcorreodeharu@gmail.com License: MIT Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Image Recognition Classifier: Topic ::
```

### Comparing `qrdet-1.8/qrdet.py` & `qrdet-1.9/qrdet.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,47 +8,44 @@
 """
 
 from __future__ import annotations
 import os
 import requests
 import tqdm
 from yolov7_package import Yolov7Detector
-import numpy as np
 
 _WEIGHTS_PATH = os.path.join(os.path.dirname(__file__), '.yolov7_qrdet', 'qrdet-yolov7.pt')
 _WEIGHTS_URL = 'https://github.com/Eric-Canas/qrdet/releases/download/first_qrdet_yolov7/qrdet-yolov7.pt'
 
 
 class QRDetector:
     def __init__(self):
         """
         Initialize the QRDetector. It loads the weights of the YOLOv7 model and prepares it for inference.
         """
         if not os.path.exists(_WEIGHTS_PATH):
             self.__download_weights(url=_WEIGHTS_URL, path=_WEIGHTS_PATH)
         self.model = Yolov7Detector(weights=_WEIGHTS_PATH, img_size=None, agnostic_nms=True, traced=False)
-        # Warm the model up.
-        self.model.detect(np.zeros((16, 16, 3), dtype=np.uint8))
 
-    def detect(self, image: np.ndarray, return_confidences: bool = True, as_float: bool = False, is_bgr: bool = False) \
+    def detect(self, image, return_confidences: bool = True, as_float: bool = False, is_bgr: bool = False) \
             -> tuple[tuple[list[float, float, float, float], float], ...] | tuple[list[float, float, float, float], ...]:
         """
         Detect QR codes in the given image.
         :param image: np.ndarray. The image to detect QR codes in, in RGB format.
         :param return_confidences: bool. Whether to return the confidences of the detections or not. Default: True.
         :param as_float: bool. Whether to return the bounding boxes as floats or not (int). Default: False.
         :param is_bgr: bool. Whether the image is in BGR format (True) or RGB format (False). Default: False.
         :return: tuple[tuple[list[float, float, float, float], float], ...] |
                     tuple[list[float, float, float, float], ...]. A tuple containing the bounding boxes of the QR codes
                     detected in the image, in the format ((x1, y1, x2, y2), ...). If return_confidences is True,
                     the tuple contains the confidence of the detection as well (((x1, y1, x2, y2), confidence),...).
         """
         # Check the image is in the correct format.
-        assert type(image) is np.ndarray, f'Expected image to be a numpy array. Got {type(image)}.'
-        assert image.dtype == np.uint8, f'Expected image to be of type np.uint8. Got {image.dtype}.'
+        assert 'ndarray' in str(type(image)), f'Expected image to be a numpy array. Got {type(image)}.'
+        assert 'uint8' in image.dtype.name, f'Expected image to be of type np.uint8. Got {image.dtype}.'
         assert len(image.shape) == 3, f'Expected image to have 3 dimensions (H, W, RGB). Got {image.shape}.'
         assert image.shape[2] == 3, f'Expected image to have 3 channels (RGB). Got {image.shape[2]}.'
         # Transform the image from RGB to BGR (that's the format that yolov7_package expects).
         if not is_bgr:
             image = image[:, :, ::-1]
         dets = self.model.detect(image)
         # Check the detections return what it was expected (can be deleted after enough testing)
@@ -67,14 +64,15 @@
                            desc: str = 'Downloading weights...') -> None:
         """
         Download the weights of the YOLOv7 model.
         :param url: str. The url of the weights.
         :param path: str. The path to save the weights. Default: _WEIGHTS_PATH.
         :param desc: str. The description of the download. Default: 'Downloading YOLOv7 QRDetector weights...'.
         """
+        self.downloading_model = True
         assert not os.path.isfile(path), f'Expected the weights to not exist. Found them at {path}.'
         # Create the directory to save the weights.
         if not os.path.exists(os.path.dirname(path)):
             os.makedirs(os.path.dirname(path))
 
         # Download the weights.
         response = requests.get(url, stream=True)
@@ -85,15 +83,26 @@
                     progress_bar.update(len(data))
                     file.write(data)
 
         # Check the weights were downloaded correctly.
         if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
             # Delete the weights if the download failed.
             os.remove(path)
-            raise Exception('Error, something went wrong while downloading the weights.')
+            raise EOFError('Error, something went wrong while downloading the weights.')
+        self.downloading_model = False
+
+    def __del__(self):
+        # If the weights didn't finish downloading, delete them.
+        if hasattr(self, 'downloading_model') and self.downloading_model and os.path.isfile(_WEIGHTS_PATH):
+            os.remove(_WEIGHTS_PATH)
+            # Also remove the directory (just in case something became corrupted).
+            _dir = os.path.dirname(_WEIGHTS_PATH)
+            if os.path.exists(_dir):
+                os.rmdir(_dir)
+
 
 def _clip_bbox(bbox: list[float, float, float, float], h: int, w: int, as_float:bool = False) -> \
                 list[int | float, int | float, int | float, int | float]:
     """
     Clip the detected bbox to the image size. If as_float is False, round the bbox to int.
 
     :param bbox: list[int | float, int | float, int | float, int | float]. The detected bbox in format x1, y1, x2, y2.
@@ -110,8 +119,8 @@
     assert len(bbox) == 4, f'Expected bbox to have 4 elements. Got {len(bbox)}.'
 
     x1, y1, x2, y2 = bbox
     if as_float:
         x1, y1, x2, y2 = max(0., x1), max(0., y1), min(float(w), x2), min(float(h), y2)
     else:
         x1, y1, x2, y2 = max(0, round(x1)), max(0, round(y1)), min(w, round(x2)), min(h, round(y2))
-    return [x1, y1, x2, y2]
+    return [x1, y1, x2, y2]
```

### Comparing `qrdet-1.8/setup.py` & `qrdet-1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='qrdet',
-    version='1.8',
+    version='1.9',
     packages=find_namespace_packages(),
     # expose qreader.py as the unique module
     py_modules=['qrdet'],
     url='https://github.com/Eric-Canas/qrdet',
     license='MIT',
     author='Eric Canas',
     author_email='elcorreodeharu@gmail.com',
     description='Robust QR Detector based on YOLOv7',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
-        'numpy',
         'yolov7-package',
+        'requests',
+        'tqdm'
     ],
-    #include_package_data=True,
-    #data_files=[('.yolov7_qrdet',
-    #             ['.yolov7_qrdet/qrdet-yolov7.pt'])],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

