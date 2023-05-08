# Comparing `tmp/audioviz-0.1.8.dev0.tar.gz` & `tmp/audioviz-0.1.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.8.dev0.tar", last modified: Sun May  7 08:34:37 2023, max compression
+gzip compressed data, was "audioviz-0.1.8.dev1.tar", last modified: Mon May  8 15:30:25 2023, max compression
```

## Comparing `audioviz-0.1.8.dev0.tar` & `audioviz-0.1.8.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.1.8.dev0/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.8.dev0/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.8.dev0/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.8.dev0/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.8.dev0/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev0/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.8.dev0/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev0/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.1.8.dev0/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.8.dev0/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.1.8.dev0/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.8.dev0/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       80 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1375 2023-05-07 08:34:06.000000 audioviz-0.1.8.dev0/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.1.8.dev1/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.8.dev1/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.8.dev1/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.8.dev1/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2165 2023-05-08 15:29:02.000000 audioviz-0.1.8.dev1/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev1/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.8.dev1/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev1/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.1.8.dev1/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.8.dev1/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.1.8.dev1/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.8.dev1/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1329 2023-05-08 15:29:07.000000 audioviz-0.1.8.dev1/setup.py
```

### Comparing `audioviz-0.1.8.dev0/PKG-INFO` & `audioviz-0.1.8.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.8.dev0
+Version: 0.1.8.dev1
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.8.dev0/README.md` & `audioviz-0.1.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/BeatAnalysis.py` & `audioviz-0.1.8.dev1/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/ChordAnalysis.py` & `audioviz-0.1.8.dev1/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/GeneralAnalysis.py` & `audioviz-0.1.8.dev1/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/Panel.py` & `audioviz-0.1.8.dev1/audioviz/Panel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 import numpy as np
 import librosa
 import matplotlib.pyplot as plt
 
-from madmom.audio.chroma import DeepChromaProcessor
-from madmom.features.chords import DeepChromaChordRecognitionProcessor
+from .ChordAnalysis import *
 
 class Dashboard():
     
     def __init__(self, fn) -> None:
         
         self.fn = fn
         self._y, self._sr = librosa.load(fn)
         
     def simple_chord_helper(self):
 
-        dcp = DeepChromaProcessor()
-        decode = DeepChromaChordRecognitionProcessor()
-        chroma = dcp(self.fn)
-        chrod_rec_res = decode(chroma)
-        
-        chord_seq = [c[2] for c in chrod_rec_res]
-        time_slice = [np.round(c[0], 1) for c in chrod_rec_res]
-        end_time = np.round(chrod_rec_res[-1][1], 1)
-        duration = np.arange(0, end_time, 0.1)
-        color_encode_list = list(set(chord_seq))
-        
-        chord_hm = np.ones((len(color_encode_list), len(duration)))
-        for i in range(1, len(time_slice)):
-            chord_hm[color_encode_list.index(chord_seq[i-1])][int(time_slice[i-1]*10):int(time_slice[i]*10)] = 0
-            
-        return chord_hm, color_encode_list, duration
+        X, Fs_X, x, Fs, x_dur = compute_chromagram_from_filename(self.fn)
+        _, chord_max = chord_recognition_template(X, norm_sim='max', nonchord=True)
+        
+        return chord_max, x_dur
     
     def simple_pitch_helper(self):
         
         f0, _, _ = librosa.pyin(self._y,
                                 fmin=librosa.note_to_hz('C2'),
                                 fmax=librosa.note_to_hz('C7'))
         
@@ -50,25 +37,26 @@
         ax0 = fig.add_subplot(3, 1, 1)
         times = np.arange(len(self._y)) / self._sr
         ax0.plot(times, self._y)
         ax0.xaxis.set_ticklabels([])
         ax0.set_title('Waveform')
         
         # A simple version of chord recognition
-        chord_map, enlist, dur = self.simple_chord_helper()
+        chord_map, dur = self.simple_chord_helper()
         ax1 = fig.add_subplot(3, 1, 2)
-        ax1.imshow(chord_map, interpolation='none', cmap='spring', aspect='auto')
-        ax1.set_xticks(np.arange(0, len(dur), 300), dur[::300])
+        ax1.imshow(chord_map, interpolation='none', cmap='gray_r', aspect='auto', origin='lower')
+        times = np.round(np.linspace(0, dur, chord_map.shape[1]), 1)
+        chord_labels = get_chord_labels(nonchord=True)
+        ax1.set_xticks(np.arange(0, len(times), 323), times[::323])
         ax1.xaxis.set_ticklabels([])
-        ax1.set_yticks(np.arange(0, len(enlist)), enlist)
+        ax1.set_yticks(np.arange(0, len(chord_labels)), chord_labels)
         ax1.set_ylabel('Chord')
         ax1.set_title('Chord Recognition')
         
         # Pitch
         ax2 = fig.add_subplot(3, 1, 3)
         f0_contour, f0_times, D = self.simple_pitch_helper()
         img = librosa.display.specshow(D, x_axis='time', y_axis='log', ax=ax2)
         ax2.set_title('Fundamental Frequency')
         ax2.plot(f0_times, f0_contour, label='f0', color='cyan', linewidth=3)
         ax2.legend(loc='upper right')
-
```

### Comparing `audioviz-0.1.8.dev0/audioviz/PitchAnalysis.py` & `audioviz-0.1.8.dev1/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/StructureAnalysis.py` & `audioviz-0.1.8.dev1/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/TimbreAnalysis.py` & `audioviz-0.1.8.dev1/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/colabInterface.py` & `audioviz-0.1.8.dev1/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz/utils.py` & `audioviz-0.1.8.dev1/audioviz/utils.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev0/audioviz.egg-info/PKG-INFO` & `audioviz-0.1.8.dev1/audioviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.8.dev0
+Version: 0.1.8.dev1
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.8.dev0/setup.py` & `audioviz-0.1.8.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.8.dev0',
+    version='0.1.8.dev1',
     
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
@@ -20,15 +20,14 @@
     keywords=['Music Information Retrieval', "Academia Sinica", "NTHU"],
 
     install_requires = ["numpy", 
                         "matplotlib",
                         "pandas",
                         "scipy", 
                         "librosa", 
-                        "madmom==0.17.dev0", 
                         "libfmp", 
                         "plotly",
                         "soundfile",
                         ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
```

