# Comparing `tmp/gopro-video-sync-0.0.2.tar.gz` & `tmp/gopro-video-sync-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-video-sync-0.0.2.tar", last modified: Mon Mar 13 05:45:42 2023, max compression
+gzip compressed data, was "gopro-video-sync-0.0.3.tar", last modified: Mon May  8 00:17:20 2023, max compression
```

## Comparing `gopro-video-sync-0.0.2.tar` & `gopro-video-sync-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 05:45:42.740032 gopro-video-sync-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-03-02 20:25:13.000000 gopro-video-sync-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2447 2023-03-13 05:45:42.739032 gopro-video-sync-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1854 2023-03-02 23:15:06.000000 gopro-video-sync-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 05:45:42.722030 gopro-video-sync-0.0.2/gopro_video_sync/
--rw-rw-rw-   0        0        0       33 2023-03-02 16:45:56.000000 gopro-video-sync-0.0.2/gopro_video_sync/__init__.py
--rw-rw-rw-   0        0        0     1658 2023-03-13 05:44:21.000000 gopro-video-sync-0.0.2/gopro_video_sync/audio_offset.py
--rw-rw-rw-   0        0        0     1000 2023-02-28 20:43:11.000000 gopro-video-sync-0.0.2/gopro_video_sync/cross_correlation.py
--rw-rw-rw-   0        0        0    10545 2023-02-24 09:03:12.000000 gopro-video-sync-0.0.2/gopro_video_sync/gopro_data.py
--rw-rw-rw-   0        0        0     2207 2023-03-01 09:58:36.000000 gopro-video-sync-0.0.2/gopro_video_sync/offset.py
--rw-rw-rw-   0        0        0     2055 2023-03-02 23:06:11.000000 gopro-video-sync-0.0.2/gopro_video_sync/sensor_offset.py
-drwxrwxrwx   0        0        0        0 2023-03-13 05:45:42.737032 gopro-video-sync-0.0.2/gopro_video_sync.egg-info/
--rw-rw-rw-   0        0        0     2447 2023-03-13 05:45:42.000000 gopro-video-sync-0.0.2/gopro_video_sync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-03-13 05:45:42.000000 gopro-video-sync-0.0.2/gopro_video_sync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 05:45:42.000000 gopro-video-sync-0.0.2/gopro_video_sync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-03-13 05:45:42.000000 gopro-video-sync-0.0.2/gopro_video_sync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-13 05:45:42.000000 gopro-video-sync-0.0.2/gopro_video_sync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 05:45:42.740032 gopro-video-sync-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-03-13 05:45:23.000000 gopro-video-sync-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:17:20.200469 gopro-video-sync-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-02 20:25:13.000000 gopro-video-sync-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2447 2023-05-08 00:17:20.199468 gopro-video-sync-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1854 2023-03-02 23:15:06.000000 gopro-video-sync-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 00:17:20.181464 gopro-video-sync-0.0.3/gopro_video_sync/
+-rw-rw-rw-   0        0        0       33 2023-03-02 16:45:56.000000 gopro-video-sync-0.0.3/gopro_video_sync/__init__.py
+-rw-rw-rw-   0        0        0     1658 2023-03-13 05:44:21.000000 gopro-video-sync-0.0.3/gopro_video_sync/audio_offset.py
+-rw-rw-rw-   0        0        0     1000 2023-02-28 20:43:11.000000 gopro-video-sync-0.0.3/gopro_video_sync/cross_correlation.py
+-rw-rw-rw-   0        0        0    10742 2023-05-08 00:12:18.000000 gopro-video-sync-0.0.3/gopro_video_sync/gopro_data.py
+-rw-rw-rw-   0        0        0     2207 2023-03-01 09:58:36.000000 gopro-video-sync-0.0.3/gopro_video_sync/offset.py
+-rw-rw-rw-   0        0        0     2055 2023-03-02 23:06:11.000000 gopro-video-sync-0.0.3/gopro_video_sync/sensor_offset.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:17:20.198469 gopro-video-sync-0.0.3/gopro_video_sync.egg-info/
+-rw-rw-rw-   0        0        0     2447 2023-05-08 00:17:20.000000 gopro-video-sync-0.0.3/gopro_video_sync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-05-08 00:17:20.000000 gopro-video-sync-0.0.3/gopro_video_sync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 00:17:20.000000 gopro-video-sync-0.0.3/gopro_video_sync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 00:17:20.000000 gopro-video-sync-0.0.3/gopro_video_sync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 00:17:20.000000 gopro-video-sync-0.0.3/gopro_video_sync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 00:17:20.200469 gopro-video-sync-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-05-08 00:13:45.000000 gopro-video-sync-0.0.3/setup.py
```

### Comparing `gopro-video-sync-0.0.2/LICENSE` & `gopro-video-sync-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gopro-video-sync-0.0.2/PKG-INFO` & `gopro-video-sync-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-video-sync
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to determine the offset between videos from two jointly mounted GoPros based on a combination of audio, accelerometer, and gyroscope data.
 Home-page: https://github.com/evoth/gopro-video-sync
 Author: Ethan Voth
 Author-email: ethanvoth7@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gopro-video-sync-0.0.2/README.md` & `gopro-video-sync-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gopro-video-sync-0.0.2/gopro_video_sync/audio_offset.py` & `gopro-video-sync-0.0.3/gopro_video_sync/audio_offset.py`

 * *Files identical despite different names*

### Comparing `gopro-video-sync-0.0.2/gopro_video_sync/cross_correlation.py` & `gopro-video-sync-0.0.3/gopro_video_sync/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `gopro-video-sync-0.0.2/gopro_video_sync/gopro_data.py` & `gopro-video-sync-0.0.3/gopro_video_sync/gopro_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,18 @@
     duration = 0
     sample_count = 0
     name = ""
     units = ""
     for sample in samples:
         # Finds the top-level "strm" box for the sensor data stream
         strm = None
+        try:
+            strm_boxes = get_gpmf_boxes(f, sample.offset, sample.size, ["DEVC", "STRM"])
+        except:
+            raise ValueError(f"Error parsing GPMF payload; may be corrupted.")
         strm_boxes = get_gpmf_boxes(f, sample.offset, sample.size, ["DEVC", "STRM"])
         for box in strm_boxes:
             if get_gpmf_boxes(f, box.offset, box.size, ["STRM", sensor_key]):
                 strm = box
                 break
         if strm is None:
             raise ValueError(f"GPMF payload does not contain {sensor_key} data.")
```

### Comparing `gopro-video-sync-0.0.2/gopro_video_sync/offset.py` & `gopro-video-sync-0.0.3/gopro_video_sync/offset.py`

 * *Files identical despite different names*

### Comparing `gopro-video-sync-0.0.2/gopro_video_sync/sensor_offset.py` & `gopro-video-sync-0.0.3/gopro_video_sync/sensor_offset.py`

 * *Files identical despite different names*

### Comparing `gopro-video-sync-0.0.2/gopro_video_sync.egg-info/PKG-INFO` & `gopro-video-sync-0.0.3/gopro_video_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-video-sync
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to determine the offset between videos from two jointly mounted GoPros based on a combination of audio, accelerometer, and gyroscope data.
 Home-page: https://github.com/evoth/gopro-video-sync
 Author: Ethan Voth
 Author-email: ethanvoth7@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gopro-video-sync-0.0.2/setup.py` & `gopro-video-sync-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="gopro-video-sync",
     packages=["gopro_video_sync"],
-    version="0.0.2",
+    version="0.0.3",
     author="Ethan Voth",
     author_email="ethanvoth7@gmail.com",
     url="https://github.com/evoth/gopro-video-sync",
     description="A tool to determine the offset between videos from two jointly mounted GoPros based on a combination of audio, accelerometer, and gyroscope data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

