# Comparing `tmp/pybsc-0.1.8.tar.gz` & `tmp/pybsc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybsc-0.1.8.tar", last modified: Sat Oct  9 10:55:04 2021, max compression
+gzip compressed data, was "pybsc-0.1.9.tar", last modified: Sat Oct  9 18:43:35 2021, max compression
```

## Comparing `pybsc-0.1.8.tar` & `pybsc-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 10:55:04.322632 pybsc-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-10-09 10:54:56.000000 pybsc-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-09 10:54:56.000000 pybsc-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-10-09 10:55:04.322632 pybsc-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-10-09 10:54:56.000000 pybsc-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 10:55:04.318632 pybsc-0.1.8/pybsc/
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 10:55:04.322632 pybsc-0.1.8/pybsc/apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/apps/readable_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/cache_readline_history.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/closest_indices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/get_target_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     4483 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/is_nan.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/iter_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/pickle_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/rm_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/sort_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/split.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/timestamp_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2021-10-09 10:54:56.000000 pybsc-0.1.8/pybsc/video_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 10:55:04.322632 pybsc-0.1.8/pybsc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-09 10:55:04.000000 pybsc-0.1.8/pybsc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-10-09 10:54:56.000000 pybsc-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-10-09 10:55:04.326632 pybsc-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2021-10-09 10:54:56.000000 pybsc-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 18:43:35.309493 pybsc-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-10-09 18:43:27.000000 pybsc-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-09 18:43:27.000000 pybsc-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-10-09 18:43:35.309493 pybsc-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2021-10-09 18:43:27.000000 pybsc-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 18:43:35.309493 pybsc-0.1.9/pybsc/
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 18:43:35.309493 pybsc-0.1.9/pybsc/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/apps/readable_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/cache_readline_history.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/closest_indices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/get_target_ext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4483 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/is_nan.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/iter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/pickle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/rm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/sort_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/split.py
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/timestamp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9074 2021-10-09 18:43:27.000000 pybsc-0.1.9/pybsc/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 18:43:35.309493 pybsc-0.1.9/pybsc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-09 18:43:35.000000 pybsc-0.1.9/pybsc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-10-09 18:43:27.000000 pybsc-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-10-09 18:43:35.309493 pybsc-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2281 2021-10-09 18:43:27.000000 pybsc-0.1.9/setup.py
```

### Comparing `pybsc-0.1.8/LICENSE` & `pybsc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/PKG-INFO` & `pybsc-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybsc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A little useful library (like a Backscratcher).
 Home-page: https://github.com/iory/pybsc
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybsc-0.1.8/pybsc/__init__.py` & `pybsc-0.1.9/pybsc/__init__.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/closest_indices.py` & `pybsc-0.1.9/pybsc/closest_indices.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/colormap.py` & `pybsc-0.1.9/pybsc/colormap.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/download.py` & `pybsc-0.1.9/pybsc/download.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/image_utils.py` & `pybsc-0.1.9/pybsc/image_utils.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/iter_utils.py` & `pybsc-0.1.9/pybsc/iter_utils.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/json_utils.py` & `pybsc-0.1.9/pybsc/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/split.py` & `pybsc-0.1.9/pybsc/split.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/timestamp_utils.py` & `pybsc-0.1.9/pybsc/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/pybsc/video_utils.py` & `pybsc-0.1.9/pybsc/video_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import shutil
 import subprocess
 import tempfile
 from tempfile import NamedTemporaryFile
 
 import cv2
 import skvideo.io
+from tqdm import tqdm
 
 from pybsc.timestamp_utils import get_timestamp_indices_wrt_base
 
 
 def hhmmss_to_seconds(ts):
     try:
         return float(ts)
@@ -62,61 +63,80 @@
         fps = get_video_avg_frame_rate(video_path)
         return int(fps * get_video_duration(video_path))
     return int(metadata['video']['@nb_frames'])
 
 
 def split_video(video_file_path, output_path=None,
                 start_time=None, end_time=None,
-                hflip=False, vflip=False):
+                hflip=False, vflip=False,
+                out_to_null=True):
     if start_time is None and end_time is None:
         raise ValueError
     start_time = start_time or 0.0
     end_time = end_time or get_video_duration(video_file_path)
     command = ['ffmpeg',
                '-y',
                '-ss', str(start_time),
                '-t', str(end_time - start_time),
                '-i', str(video_file_path)]
     if hflip is True:
         command.extend(['-vf', 'hflip'])
     if vflip is True:
         command.extend(['-vf', 'vflip'])
+
+    stdout = None
+    stderr = None
+    if out_to_null:
+        stdout = subprocess.DEVNULL
+        stderr = subprocess.DEVNULL
     if output_path is None:
         suffix = Path(video_file_path).suffix
         with NamedTemporaryFile(delete=True, suffix=suffix) as tmp:
             command.append(tmp.name)
-            print(f'Running \"{" ".join(command)}\"')
-            subprocess.call(command)
+            if not out_to_null:
+                print(f'Running \"{" ".join(command)}\"')
+            proc = subprocess.Popen(command,
+                                    stdout=stdout,
+                                    stderr=stderr)
+            proc.wait()
             shutil.copy(tmp.name, video_file_path)
     else:
         command.append(str(output_path))
-        print(f'Running \"{" ".join(command)}\"')
-        subprocess.call(command)
+        if not out_to_null:
+            print(f'Running \"{" ".join(command)}\"')
+        proc = subprocess.Popen(command,
+                                stdout=stdout,
+                                stderr=stderr)
+        proc.wait()
 
 
 def split_video_from_stamps(
         video_file_path,
         start_stamps, end_stamps,
         output_paths=None,
         output_dirpath=None,
-        filename_tmpl='video_{start_frame:05}_{end_frame:05}.mp4'):
+        filename_tmpl='video_{start_frame:05}_{end_frame:05}.mp4',
+        show_progress=True):
     if len(start_stamps) != len(end_stamps):
         raise RuntimeError(
             'Length not much len(start_stamps) != len(end_stamps)'
             '({})!=({})'.format(len(start_stamps), len(end_stamps)))
     fps = get_video_avg_frame_rate(video_file_path)
     if output_paths is None:
         output_paths = []
         if output_dirpath is None:
             tmp_output_dir = tempfile.TemporaryDirectory()
             tmp_output_dir.cleanup()
             os.makedirs(tmp_output_dir.name, exist_ok=True)
             output_dirpath = tmp_output_dir.name
         output_dirpath = Path(output_dirpath)
-        for i, (s, e) in enumerate(zip(start_stamps, end_stamps)):
+        for i, (s, e) in tqdm(
+                enumerate(zip(start_stamps, end_stamps)),
+                total=len(min(start_stamps, end_stamps)),
+                disable=show_progress is False):
             start_frame = int(math.ceil(s * fps))
             end_frame = int(math.ceil(e * fps))
             output_paths.append(output_dirpath
                                 / filename_tmpl.format(
                                     start_frame=start_frame,
                                     end_frame=end_frame))
     for i, (s, e, video_out) in enumerate(zip(start_stamps, end_stamps,
```

### Comparing `pybsc-0.1.8/pybsc.egg-info/PKG-INFO` & `pybsc-0.1.9/pybsc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybsc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A little useful library (like a Backscratcher).
 Home-page: https://github.com/iory/pybsc
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybsc-0.1.8/pybsc.egg-info/SOURCES.txt` & `pybsc-0.1.9/pybsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybsc-0.1.8/setup.py` & `pybsc-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.8"
+version = "0.1.9"
 
 
 if sys.argv[-1] == "release":
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
```

