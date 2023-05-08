# Comparing `tmp/webcam-0.7.tar.gz` & `tmp/webcam-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.7.tar", last modified: Fri May  5 14:27:17 2023, max compression
+gzip compressed data, was "webcam-0.8.tar", last modified: Mon May  8 10:49:32 2023, max compression
```

## Comparing `webcam-0.7.tar` & `webcam-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:27:17.386033 webcam-0.7/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.7/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 14:27:17.386033 webcam-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 14:27:17.386033 webcam-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-05 14:27:01.000000 webcam-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:27:17.354786 webcam-0.7/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.7/webcam/__init__.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.7/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.7/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    12714 2023-05-05 13:05:54.000000 webcam-0.7/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:27:17.386033 webcam-0.7/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 14:27:16.000000 webcam-0.7/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-05 14:27:17.000000 webcam-0.7/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:27:16.000000 webcam-0.7/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-05 14:27:17.000000 webcam-0.7/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 14:27:17.000000 webcam-0.7/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 10:49:32.101922 webcam-0.8/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.8/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-08 10:49:32.099918 webcam-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:49:32.101922 webcam-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-08 10:07:24.000000 webcam-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:49:32.060756 webcam-0.8/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-0.8/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.8/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.8/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    13261 2023-05-08 10:47:17.000000 webcam-0.8/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:49:32.096966 webcam-0.8/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.7/LICENSE` & `webcam-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.7/PKG-INFO` & `webcam-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.7
+Version: 0.8
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.7/setup.py` & `webcam-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.7',
+    version='0.8',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.7/webcam/_video_webcam.py` & `webcam-0.8/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.7/webcam/_webcam_background.py` & `webcam-0.8/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.7/webcam/webcam.py` & `webcam-0.8/webcam/webcam.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,47 +22,45 @@
 from webcam._webcam_background import _WebcamBackground
 
 CROP, RESIZE = 'crop', 'resize'
 
 class Webcam:
     def __init__(
         self,
-        webcam_src: int | str = 0,
+        src: int | str = 0,
         h: int | None = None,
         w: int | None = None,
         as_bgr: bool = False,
         batch_size: int | None = None,
         run_in_background: bool = False,
         max_frame_rate: int | None = 60,
         on_aspect_ratio_lost: str = CROP,
     ):
         """
         Initialize the WebcamReader.
 
-        :param webcam_src: int or str. The index of the webcam or its path.
+        :param src: int or str. The index of the webcam or its path.
         :param h: int or None. Desired height of the frames. If None and `_w` is provided, the aspect ratio will be preserved.
         :param w: int or None. Desired width of the frames. If None and `_h` is provided, the aspect ratio will be preserved.
         :param as_bgr: bool. If True, the frames will be returned in BGR format, otherwise in RGB format.
         :param batch_size: int or None. If not None, the iterator will yield batches of frames (B, H, W, C). If None, the iterator will yield single frames (H, W, C).
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
         """
         assert on_aspect_ratio_lost in (CROP, RESIZE), f"Invalid value for `on_aspect_ratio_lost`: {on_aspect_ratio_lost}." \
                                                        f" Valid values are: {CROP}, {RESIZE}"
         self._background = run_in_background
         self.on_aspect_ratio_lost = on_aspect_ratio_lost
         if run_in_background:
             raise NotImplementedError("Background reading is not implemented yet.")
             #self.cap = _WebcamBackground(src=webcam_src).start()
-        elif isinstance(webcam_src, str):
-            #TODO: Improve the check for video file
-            assert os.path.isfile(webcam_src), f"Video file not found: {webcam_src}"
-            self.cap = _VideoWebcam(video_path=webcam_src)
+        elif isinstance(src, str) and os.path.isfile(src):
+            self.cap = _VideoWebcam(video_path=src)
         else:
-            self.cap = cv2.VideoCapture(webcam_src)
+            self.cap = cv2.VideoCapture(src)
         self.as_bgr = as_bgr
 
         # Calculate and set output frame size
         self.frame_size_hw = self._calculate_and_set_desired_resolution(h, w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
@@ -302,7 +300,21 @@
 
     def __del__(self):
         # Close the video
         if self._background:
             self.stop()
         self.release()
         self.cap = None
+
+def get_rtsp_url(ip: str, username: str, password: str, port: int = 554, channel: int = 1, stream: int = 0) -> str:
+    """
+    Generate an RTSP URL for connecting to an IP camera.
+
+    :param ip: str. The IP address of the camera.
+    :param username: str. The username for accessing the camera.
+    :param password: str. The password for accessing the camera.
+    :param port: int. The RTSP port (default: 554).
+    :param channel: int. The camera channel (default: 1).
+    :param stream: int. The stream type (default: 0).
+    :return: str. The generated RTSP URL.
+    """
+    return f"rtsp://{username}:{password}@{ip}:{port}/cam/realmonitor?channel={channel}&subtype={stream}"
```

### Comparing `webcam-0.7/webcam.egg-info/PKG-INFO` & `webcam-0.8/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.7
+Version: 0.8
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

