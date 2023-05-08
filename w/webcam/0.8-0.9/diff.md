# Comparing `tmp/webcam-0.8.tar.gz` & `tmp/webcam-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.8.tar", last modified: Mon May  8 10:49:32 2023, max compression
+gzip compressed data, was "webcam-0.9.tar", last modified: Mon May  8 12:05:00 2023, max compression
```

## Comparing `webcam-0.8.tar` & `webcam-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:32.101922 webcam-0.8/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.8/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-08 10:49:32.099918 webcam-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 10:49:32.101922 webcam-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-08 10:07:24.000000 webcam-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:32.060756 webcam-0.8/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-0.8/webcam/__init__.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.8/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.8/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    13261 2023-05-08 10:47:17.000000 webcam-0.8/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:32.096966 webcam-0.8/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 10:49:31.000000 webcam-0.8/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 12:05:00.464250 webcam-0.9/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.9/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-08 12:05:00.463251 webcam-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:05:00.464250 webcam-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-08 12:04:13.000000 webcam-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:05:00.438249 webcam-0.9/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-0.9/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.9/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.9/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    13299 2023-05-08 12:04:13.000000 webcam-0.9/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:05:00.453257 webcam-0.9/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.8/LICENSE` & `webcam-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.8/PKG-INFO` & `webcam-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.8
+Version: 0.9
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.8/setup.py` & `webcam-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.8',
+    version='0.9',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.8/webcam/_video_webcam.py` & `webcam-0.9/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.8/webcam/_webcam_background.py` & `webcam-0.9/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.8/webcam/webcam.py` & `webcam-0.9/webcam/webcam.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self,
         src: int | str = 0,
         h: int | None = None,
         w: int | None = None,
         as_bgr: bool = False,
         batch_size: int | None = None,
         run_in_background: bool = False,
-        max_frame_rate: int | None = 60,
+        max_frame_rate: int | None = None,
         on_aspect_ratio_lost: str = CROP,
     ):
         """
         Initialize the WebcamReader.
 
         :param src: int or str. The index of the webcam or its path.
         :param h: int or None. Desired height of the frames. If None and `_w` is provided, the aspect ratio will be preserved.
@@ -46,21 +46,20 @@
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
         """
         assert on_aspect_ratio_lost in (CROP, RESIZE), f"Invalid value for `on_aspect_ratio_lost`: {on_aspect_ratio_lost}." \
                                                        f" Valid values are: {CROP}, {RESIZE}"
         self._background = run_in_background
         self.on_aspect_ratio_lost = on_aspect_ratio_lost
-        if run_in_background:
-            raise NotImplementedError("Background reading is not implemented yet.")
-            #self.cap = _WebcamBackground(src=webcam_src).start()
-        elif isinstance(src, str) and os.path.isfile(src):
+        # Initialize it for videos if the source is a string and a file exists at the path
+        if isinstance(src, str) and os.path.isfile(src):
             self.cap = _VideoWebcam(video_path=src)
+        # Otherwise assume it is a webcam (both webcam or RTSP stream)
         else:
-            self.cap = cv2.VideoCapture(src)
+            self.cap = cv2.VideoCapture(src) if not run_in_background else _WebcamBackground(src=src)
         self.as_bgr = as_bgr
 
         # Calculate and set output frame size
         self.frame_size_hw = self._calculate_and_set_desired_resolution(h, w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
```

### Comparing `webcam-0.8/webcam.egg-info/PKG-INFO` & `webcam-0.9/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.8
+Version: 0.9
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

