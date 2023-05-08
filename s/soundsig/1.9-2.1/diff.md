# Comparing `tmp/soundsig-1.9.tar.gz` & `tmp/soundsig-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soundsig-1.9.tar", last modified: Sun Oct 13 06:01:53 2019, max compression
+gzip compressed data, was "soundsig-2.1.tar", last modified: Mon May  8 20:27:34 2023, max compression
```

## Comparing `soundsig-1.9.tar` & `soundsig-2.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2019-10-13 06:01:53.000000 soundsig-1.9/
--rw-r--r--   0 frederictheunissen   (501) staff       (20)      465 2019-10-13 06:01:53.000000 soundsig-1.9/PKG-INFO
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1294 2018-11-28 19:49:24.000000 soundsig-1.9/README.md
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)       79 2019-10-13 06:01:53.000000 soundsig-1.9/setup.cfg
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      824 2019-10-13 06:00:27.000000 soundsig-1.9/setup.py
-drwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig/
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2017-06-09 23:50:21.000000 soundsig-1.9/soundsig/__init__.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     6772 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/basis.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      729 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/check_versions.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    37859 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/coherence.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    50518 2017-05-25 00:33:42.000000 soundsig-1.9/soundsig/colormaps.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     4211 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/complex_pca.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     6545 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/detect_peaks.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     2229 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/discrete_process.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    14240 2019-03-09 23:43:09.000000 soundsig-1.9/soundsig/discriminate.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     7492 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/entropy_estimators.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    20119 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/graph_cluster.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    14017 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/hht.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1518 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/hinton.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    15339 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/incrowd.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     8352 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/memd.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     6558 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/optimization.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    18484 2018-09-06 09:38:30.000000 soundsig-1.9/soundsig/plots.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1846 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/quasirand.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    29882 2018-09-06 09:38:30.000000 soundsig-1.9/soundsig/signal.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    67246 2019-10-13 05:59:00.000000 soundsig-1.9/soundsig/sound.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    17695 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/spikes.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      382 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/stats.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     4618 2017-05-25 18:08:25.000000 soundsig-1.9/soundsig/strf_bank.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     8320 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/strfs.py
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    30713 2018-07-10 21:22:47.000000 soundsig-1.9/soundsig/timefreq.py
-drwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig.egg-info/
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      465 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig.egg-info/PKG-INFO
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      729 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig.egg-info/SOURCES.txt
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)        1 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig.egg-info/dependency_links.txt
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)       66 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig.egg-info/requires.txt
--rwxr-xr-x   0 frederictheunissen   (501) staff       (20)        9 2019-10-13 06:01:53.000000 soundsig-1.9/soundsig.egg-info/top_level.txt
+drwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2023-05-08 20:27:34.736178 soundsig-2.1/
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1074 2023-03-15 04:15:51.000000 soundsig-2.1/LICENSE.txt
+-rw-r--r--   0 frederictheunissen   (501) staff       (20)      435 2023-05-08 20:27:34.736268 soundsig-2.1/PKG-INFO
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1294 2023-03-15 04:15:51.000000 soundsig-2.1/README.md
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)       79 2023-05-08 20:27:34.736582 soundsig-2.1/setup.cfg
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      792 2023-05-08 20:20:20.000000 soundsig-2.1/setup.py
+drwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2023-05-08 20:27:34.734973 soundsig-2.1/soundsig/
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/__init__.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     6772 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/basis.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      729 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/check_versions.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    10734 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/coherence.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    50518 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/colormaps.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     4211 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/complex_pca.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     6545 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/detect_peaks.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     2229 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/discrete_process.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    20082 2023-05-08 19:22:43.000000 soundsig-2.1/soundsig/discriminate.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     7492 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/entropy_estimators.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    20119 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/graph_cluster.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    14017 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/hht.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1518 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/hinton.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    15339 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/incrowd.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     8352 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/memd.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     6558 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/optimization.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    18484 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/plots.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     1846 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/quasirand.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    29882 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/signal.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    67849 2023-05-08 18:33:09.000000 soundsig-2.1/soundsig/sound.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    17695 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/spikes.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)      382 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/stats.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     4618 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/strf_bank.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)     8320 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/strfs.py
+-rwxr-xr-x   0 frederictheunissen   (501) staff       (20)    31148 2023-03-15 04:15:51.000000 soundsig-2.1/soundsig/timefreq.py
+drwxr-xr-x   0 frederictheunissen   (501) staff       (20)        0 2023-05-08 20:27:34.736051 soundsig-2.1/soundsig.egg-info/
+-rw-r--r--   0 frederictheunissen   (501) staff       (20)      435 2023-05-08 20:27:34.000000 soundsig-2.1/soundsig.egg-info/PKG-INFO
+-rw-r--r--   0 frederictheunissen   (501) staff       (20)      741 2023-05-08 20:27:34.000000 soundsig-2.1/soundsig.egg-info/SOURCES.txt
+-rw-r--r--   0 frederictheunissen   (501) staff       (20)        1 2023-05-08 20:27:34.000000 soundsig-2.1/soundsig.egg-info/dependency_links.txt
+-rw-r--r--   0 frederictheunissen   (501) staff       (20)       59 2023-05-08 20:27:34.000000 soundsig-2.1/soundsig.egg-info/requires.txt
+-rw-r--r--   0 frederictheunissen   (501) staff       (20)        9 2023-05-08 20:27:34.000000 soundsig-2.1/soundsig.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `soundsig-1.9/README.md` & `soundsig-2.1/README.md`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/setup.py` & `soundsig-2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup
 
 setup(
     name = 'soundsig',
-    version = '1.9',
+    version = '2.1',
     packages = ['soundsig'],
     description = 'Sound and Signal Analysis Tools for Bioacousticians and Auditory Neurophysiologists',
     author = 'Frederic Theunissen',
     author_email = 'theunissen@berkeley.edu',
     url = 'https://github.com/theunissenlab/soundsig', 
     keywords = 'bioacoustics biosound vocalization auditory',
     classifiers = ['Development Status :: 4 - Beta',
                    'Programming Language :: Python :: 3.0'],
     install_requires = ['numpy',
                       'scipy',
                       'matplotlib',
-                      'tables',
                       'h5py',
                       'mne',
                       'nitime',
                       'pandas',
                       'scikit-learn']
 )
```

### Comparing `soundsig-1.9/soundsig/basis.py` & `soundsig-2.1/soundsig/basis.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/check_versions.py` & `soundsig-2.1/soundsig/check_versions.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/colormaps.py` & `soundsig-2.1/soundsig/colormaps.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/complex_pca.py` & `soundsig-2.1/soundsig/complex_pca.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/detect_peaks.py` & `soundsig-2.1/soundsig/detect_peaks.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/discrete_process.py` & `soundsig-2.1/soundsig/discrete_process.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/entropy_estimators.py` & `soundsig-2.1/soundsig/entropy_estimators.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/graph_cluster.py` & `soundsig-2.1/soundsig/graph_cluster.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/hht.py` & `soundsig-2.1/soundsig/hht.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/hinton.py` & `soundsig-2.1/soundsig/hinton.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/incrowd.py` & `soundsig-2.1/soundsig/incrowd.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/memd.py` & `soundsig-2.1/soundsig/memd.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/optimization.py` & `soundsig-2.1/soundsig/optimization.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/plots.py` & `soundsig-2.1/soundsig/plots.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/quasirand.py` & `soundsig-2.1/soundsig/quasirand.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/signal.py` & `soundsig-2.1/soundsig/signal.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/sound.py` & `soundsig-2.1/soundsig/sound.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,48 +16,50 @@
 from scipy.io.wavfile import read as read_wavfile
 from scipy.fftpack import fft, ifft, fftfreq, fft2, ifft2, dct
 from scipy.signal import resample, firwin, filtfilt
 from scipy.linalg import inv, toeplitz
 from scipy.optimize import leastsq
 
 
+import matplotlib as mpl
 import matplotlib.pyplot as plt
-import matplotlib.cm as cmap
 import matplotlib.colors as pltcolors
 import matplotlib.mlab as mlab
 
 import colorsys
 from soundsig.signal import lowpass_filter, gaussian_window, correlation_function
 from soundsig.timefreq import gaussian_stft
 from soundsig.detect_peaks import detect_peaks
 
 
 class WavFile():
     """ Class for representing a sound and writing it to a .wav file """
 
-    def __init__(self, file_name=None, log_spectrogram=True):
+    def __init__(self, file_name=None, log_spectrogram=True, mono=False):
 
         self.log_spectrogram = log_spectrogram
         if file_name is None:
             self.sample_depth = 2  # in bytes
             self.sample_rate = 44100.0  # in Hz
             self.data = None
             self.num_channels = 1
         else:
-            wr = wave.open(file_name, 'r')
-            self.num_channels = wr.getnchannels()
-            self.sample_depth = wr.getsampwidth()
-            wr.close()
-
-            self.sample_rate, data = read_wavfile(file_name)
-            # If stereo make mono
-            if self.num_channels == 1:
-                self.data = data
+            self.sample_rate, self.data = read_wavfile(file_name)
+            self.sample_depth = 2 # 2 bytes  - used on writing to get 16 bit files.
+
+            if (len(self.data.shape) == 1):
+                self.num_channels = 1
             else:
-                self.data = data.mean(axis=1)
+                self.num_channels = self.data.shape[1]
+
+            # If multi-channel collapse
+            if mono:
+                if self.num_channels != 1:
+                    self.data = self.data[:,0]
+                    self.num_channels = 1
 
         self.analyzed = False
 
     def to_wav(self, output_file, normalize=False, max_amplitude=32767.0):
         wf = wave.open(output_file, 'w')
 
         wf.setparams( (self.num_channels, self.sample_depth, self.sample_rate, len(self.data), 'NONE', 'not compressed') )
@@ -108,15 +110,15 @@
         self.spectrogram_rms = spec_rms
         self.analyzed = True
 
     def reanalyze(self, min_freq=0, max_freq=None, spec_sample_rate=1000.0, freq_spacing=25.0, envelope_cutoff_freq=200.0, noise_level_db=80, rectify=True, cmplx=False):
         self.analyzed = False
         return self.analyze(min_freq, max_freq, spec_sample_rate, freq_spacing, envelope_cutoff_freq, noise_level_db, rectify, cmplx)
 
-    def plot(self, fig=None, show_envelope=True, min_freq=0.0, max_freq=10000.0, colormap=cmap.gist_yarg, noise_level_db=80,
+    def plot(self, fig=None, show_envelope=True, min_freq=0.0, max_freq=10000.0, colormap=mpl.colormaps['gist_yarg'], noise_level_db=80,
              start_time=0, end_time=np.inf):
 
         self.analyze(min_freq=min_freq, max_freq=max_freq, noise_level_db=noise_level_db)
 
         if show_envelope:
             spw_size = 15
             spec_size = 35
@@ -146,17 +148,21 @@
             plt.xlabel('Time (s)')
             plt.ylabel('Envelope')
             plt.axis('tight')
             
 class BioSound(object):
     """ Class for representing a communication sound using multiple feature spaces"""
 
-    def __init__(self, soundWave=np.array(0.0), fs=np.array(0.0), emitter='Unknown', calltype = 'U' ):
+    def __init__(self, soundWave=np.array([0.0]), fs=np.array(0.0), emitter='Unknown', calltype = 'U' ):
         # Note that all the fields are numpy arrays for saving to h5 files.
 
+        if (len(soundWave.shape) != 1):
+            print('Error: Biosound can only deal with single channel sounds. Returning empty class')
+            soundWave = np.array([0.0])
+
         self.sound = soundWave  # sound pressure waveform 
         self.hashid = np.string_(hashlib.md5(np.array_str(soundWave).encode('utf-8')).hexdigest())
         self.samprate = float(fs) if isinstance(fs,int) else fs      # sampling rate
         self.emitter = np.string_(emitter)  # string for id of emitter
         self.type = np.string_(calltype)    # string for call type
         self.spectro = np.asarray([])    # Log spectrogram
         self.to = np.asarray([])         # Time scale for spectrogram
@@ -351,24 +357,24 @@
             self.minfund = np.min(goodFund)
             self.cvfund = np.std(goodFund)/meanfund
             
     def play(self):
     # Plays the sound
         play_sound_array(self.sound*(2**15), self.samprate)
             
-    def plot(self, DBNOISE=50, f_low=250, f_high=10000):
-    # Plots a biosound in figures 1, 2, 3
+    def plot(self, DBNOISE=50, f_low=250, f_high=10000, wt_low=-100, wt_high=100):
+    # Plots a biosound in figures 1, 2, 3, 4
     
         # Ploting Variables
         soundlen = np.size(self.sound)
         t = np.array(range(soundlen))
         t = t*(1000.0/self.samprate)
 
         # Plot the oscillogram + spectrogram
-        plt.figure(1)
+        fig1 = plt.figure(1)
         plt.clf()
         # mngr = plt.get_current_fig_manager()
         # mngr.window.setGeometry(0, 260, 640, 545)
         
         
         # The oscillogram
         plt.axes([0.1, 0.75, 0.85, 0.20])      
@@ -396,29 +402,29 @@
             plt.imshow(soundSpect, extent = (self.to[0]*1000, self.to[-1]*1000, self.fo[0], self.fo[-1]), aspect='auto', interpolation='nearest', origin='lower', cmap=cmap, vmin=minSpect, vmax=maxB)
         
         plt.ylim(f_low, f_high)
         plt.xlim(0, t[-1])
         plt.ylabel('Frequency (Hz)')
         plt.xlabel('Time (ms)')
                      
-    # Plot the fundamental on the same figure
+         # Plot the fundamental on the same figure
         if self.f0.size != 0 :
             fundplot = self.f0
             diffFund = np.diff(fundplot)
             diffFundInd = np.concatenate(([False], abs(diffFund)>1000))
             fundplot[diffFundInd] = float('nan')
             plt.plot(self.to*1000.0, self.f0, 'k', linewidth=3)
             plt.plot(self.to*1000.0, self.f0_2, 'm', linewidth=3)
             plt.plot(self.to*1000.0, self.F1, 'r--', linewidth=3)
             plt.plot(self.to*1000.0, self.F2, 'w--', linewidth=3)
             plt.plot(self.to*1000.0, self.F3, 'b--', linewidth=3)
         plt.show()
            
-    # Plot Power Spectrum
-        plt.figure(2)
+         # Plot Power Spectrum
+        fig2 = plt.figure(2)
         plt.clf()
         # mngr = plt.get_current_fig_manager()
         # mngr.window.setGeometry(650, 260, 640, 545)
         if self.psd.size != 0 :
             plt.plot(self.fpsd, self.psd, 'k-') 
             plt.xlabel('Frequency Hz')
             plt.ylabel('Power Linear')
@@ -439,16 +445,16 @@
                 F3Mean = self.F3[~np.isnan(self.F3)].mean()
                 plt.plot([F1Mean, F1Mean], [yl, yh], 'r--', linewidth=2.0)
                 plt.plot([F2Mean, F2Mean], [yl, yh], 'c--', linewidth=2.0)
                 plt.plot([F3Mean, F3Mean], [yl, yh], 'b--', linewidth=2.0)
                 
             plt.show()
   
-    # Table of results
-        plt.figure(3)
+         # Table of results
+        fig3 = plt.figure(3)
         plt.clf()
         # mngr = plt.get_current_fig_manager()
         # mngr.window.setGeometry(320, 10, 640, 250)
         textstr = '%s  %s' % (self.emitter, self.type)
         plt.text(0.4, 1.0, textstr)
         if self.fund.size != 0:
             if self.fund2.size != 0:
@@ -476,36 +482,38 @@
         if self.rms.size != 0 and self.maxAmp.size != 0 :
             textstr = 'RMS = %.2f, Max Amp = %.2f' % (self.rms, self.maxAmp)
             plt.text(-0.1, 0.0, textstr)
         
         plt.axis('off')        
         plt.show()
         
-    # Plot Modulation Power spectrum if it exists
+         # Plot Modulation Power spectrum if it exists
     
         #ex = (spectral_freq.min(), spectral_freq.max(), temporal_freq.min(), temporal_freq.max())
+        fig4 = []
         if self.mps.size != 0 :
-            plt.figure(4)
+            fig4 = plt.figure(4)
             plt.clf()
             cmap = plt.get_cmap('jet')
             ex = (self.wt.min(), self.wt.max(), self.wf.min()*1e3, self.wf.max()*1e3)
             logMPS = 10.0*np.log10(self.mps)
             maxMPS = logMPS.max()
             minMPS = maxMPS-DBNOISE
             logMPS[logMPS < minMPS] = minMPS
             plt.imshow(logMPS, interpolation='nearest', aspect='auto', origin='lower', cmap=cmap, extent=ex)
             plt.ylabel('Spectral Frequency (Cycles/KHz)')
             plt.xlabel('Temporal Frequency (Hz)')
             plt.colorbar()
             plt.ylim((0,self.wf.max()*1e3))
+            plt.xlim((wt_low, wt_high))
             plt.title('Modulation Power Spectrum')
             plt.show()
         
         
-        plt.pause(1)   # To flush the plots?
+        return fig1, fig2, fig3, fig4
 
 
 
 def spec_colormap():
 # Makes the colormap that we like for spectrograms
 
     cmap = np.zeros((64,3))
@@ -526,15 +534,15 @@
         cmap[ir+ig+ib+1,1] = 0.5 + (ir)*(0.5/20.0)
         cmap[ir+ig+ib+1,2] = 1
 
     for ic in range(64):
         (cmap[ic,0], cmap[ic,1], cmap[ic,2]) = colorsys.hsv_to_rgb(cmap[ic,0], cmap[ic,1], cmap[ic,2])
     
     spec_cmap = pltcolors.ListedColormap(cmap, name=u'SpectroColorMap', N=64)
-    plt.register_cmap(cmap=spec_cmap)
+    mpl.colormaps.register(cmap=spec_cmap, force=True)
 
 def plot_spectrogram(t, freq, spec, ax=None, ticks=True, fmin=None, fmax=None, colormap=None, colorbar=True, log = True, dBNoise = 50):
     
     if colormap == None:
         spec_colormap()
         colormap = plt.get_cmap('SpectroColorMap')
         
@@ -850,17 +858,17 @@
         print('mps will be calculate with windows of %d points or %s s' % (nt-1, dt[-1]) )
         nWindow = nt - 1
     else:
         nWindow = np.where(dt>= window)[0][0]
     if nWindow%2 == 0:
         nWindow += 1  # Make it odd size so that we have a symmetric window
         
-    if nWindow < 64:
-        print('Error in mps: window size %d pts (%.3f s) is two small for reasonable estimates' % (nWindow, window))
-        return np.asarray([]), np.asarray([]), np.asarray([])
+    #if nWindow < 64:
+    #    print('Error in mps: window size %d pts (%.3f s) is two small for reasonable estimates' % (nWindow, window))
+    #    return np.asarray([]), np.asarray([]), np.asarray([])
         
     # Generate the Gaussian window
     gt, wg = gaussian_window(nWindow, 6)
     tShift = int(gt[-1]/3)
     nchunks = 0
     
     # Pad the spectrogram with zeros.
@@ -1065,26 +1073,27 @@
            soundLen - length of sal, fund, fund2, form1, form2, form3
     """
 
     # Band-pass filtering signal prior to auto-correlation
     soundLen = len(soundIn)
     nfilt = 1024
     if soundLen < 1024:
-        print('Error in fundEstimator: sound too short for bandpass filtering, len(soundIn)=%d' % soundLen)
-        return (np.asarray([]), np.asarray([]), np.asarray([]), np.asarray([]), np.asarray([]), np.asarray([]), soundLen)
-
-    # high pass filter the signal
-    highpassFilter = firwin(nfilt-1, 2.0*lowFc/fs, pass_zero=False)
-    padlen = min(soundLen-10, 3*len(highpassFilter))
-    soundIn = filtfilt(highpassFilter, [1.0], soundIn, padlen=padlen)
-
-    # low pass filter the signal
-    lowpassFilter = firwin(nfilt, 2.0*highFc/fs)
-    padlen = min(soundLen-10, 3*len(lowpassFilter))
-    soundIn = filtfilt(lowpassFilter, [1.0], soundIn, padlen=padlen)
+        print('Warning in fundEstimator: sound too short for bandpass filtering, len(soundIn)=%d' % soundLen)
+        print('Signal will not be filtered - you might want to filter before making Biosound oobject')
+         # return (np.asarray([]), np.asarray([]), np.asarray([]), np.asarray([]), np.asarray([]), np.asarray([]), soundLen)
+    else:
+        # high pass filter the signal
+        highpassFilter = firwin(nfilt-1, 2.0*lowFc/fs, pass_zero=False)
+        padlen = min(soundLen-10, 3*len(highpassFilter))
+        soundIn = filtfilt(highpassFilter, [1.0], soundIn, padlen=padlen)
+
+        # low pass filter the signal
+        lowpassFilter = firwin(nfilt, 2.0*highFc/fs)
+        padlen = min(soundLen-10, 3*len(lowpassFilter))
+        soundIn = filtfilt(lowpassFilter, [1.0], soundIn, padlen=padlen)
 
     # Plot a spectrogram?
     #if debugFig:
     #    plt.figure(9)
     #    (tDebug ,freqDebug ,specDebug , rms) = spectrogram(soundIn, fs, 1000.0, 50, min_freq=0, max_freq=10000, nstd=6, log=True, noise_level_db=50, rectify=True) 
     #    plot_spectrogram(tDebug, freqDebug, specDebug)
```

### Comparing `soundsig-1.9/soundsig/spikes.py` & `soundsig-2.1/soundsig/spikes.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/strf_bank.py` & `soundsig-2.1/soundsig/strf_bank.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/strfs.py` & `soundsig-2.1/soundsig/strfs.py`

 * *Files identical despite different names*

### Comparing `soundsig-1.9/soundsig/timefreq.py` & `soundsig-2.1/soundsig/timefreq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import division, print_function
 
 import time
 
 from abc import ABCMeta,abstractmethod
 import numpy as np
+from numpy.lib.stride_tricks import sliding_window_view
 
-
-from scipy.fftpack import fft,fftfreq, ifft
+from scipy.fftpack import fft, fftfreq, ifft, next_fast_len
 from scipy.signal import hilbert
 from scipy.interpolate import RectBivariateSpline
 
 import matplotlib.pyplot as plt
 
 import nitime.algorithms as ntalg
 from nitime import utils as ntutils
@@ -35,34 +35,42 @@
 
 
 class GaussianSpectrumEstimator(ComplexSpectrumEstimator):
 
     def __init__(self, nstd=6):
         ComplexSpectrumEstimator.__init__(self)
         self.nstd = nstd
+        self._gauss_window_cache = {}
 
     def get_frequencies(self, signal_length, sample_rate):
+        signal_length = next_fast_len(signal_length)
         freq = fftfreq(signal_length, d=1.0/sample_rate)
         nz = freq >= 0.0
         return freq[nz]
 
+    def _get_gauss_window(self, nwinlen):
+        if nwinlen in self._gauss_window_cache:
+            return self._gauss_window_cache[nwinlen]
+        else:
+            if nwinlen % 2 == 0:
+                nwinlen += 1
+            hnwinlen = nwinlen // 2
+            gauss_t = np.arange(-hnwinlen, hnwinlen+1, 1.0)
+            gauss_std = float(nwinlen) / float(self.nstd)
+            gauss_window = np.exp(-gauss_t**2 / (2.0*gauss_std**2)) / (gauss_std*np.sqrt(2*np.pi))
+            self._gauss_window_cache[nwinlen] = gauss_window
+            return gauss_window
+
     def estimate(self, signal, sample_rate, start_time, end_time):
         nwinlen = len(signal)
-        if nwinlen % 2 == 0:
-            nwinlen += 1
-        hnwinlen = nwinlen // 2
-
-        #construct the window
-        gauss_t = np.arange(-hnwinlen, hnwinlen+1, 1.0)
-        gauss_std = float(nwinlen) / float(self.nstd)
-        self.gauss_window = np.exp(-gauss_t**2 / (2.0*gauss_std**2)) / (gauss_std*np.sqrt(2*np.pi))
+        gauss_window = self._get_gauss_window(nwinlen)
 
+        fft_len = next_fast_len(len(signal))
         #window the signal and take the FFT
-        fft_len = len(signal)
-        windowed_slice = signal[:fft_len]*self.gauss_window[:fft_len]
+        windowed_slice = signal[:fft_len]*gauss_window[:fft_len]
         s_fft = fft(windowed_slice, n=fft_len, overwrite_x=1)
         freq = fftfreq(fft_len, d=1.0/sample_rate)
         nz = freq >= 0.0
 
         return freq[nz],s_fft[nz]
 
 
@@ -228,39 +236,37 @@
     full_freq = spectrum_estimator.get_frequencies(nwinlen, sample_rate)
     freq_index = (full_freq >= min_freq) & (full_freq <= max_freq)
     freq = full_freq[freq_index]
     nfreq = freq_index.sum()
 
     nincrement = int(np.round(sample_rate*increment))
     if zero_pad:
-        nwindows = len(s) // nincrement
         # print 'len(s)=%d, nwinlen=%d, hwinlen=%d, nincrement=%d, nwindows=%d' % (len(s), nwinlen, hnwinlen, nincrement, nwindows)
         #pad the signal with zeros
         zs = np.zeros([len(s) + 2*hnwinlen])
         zs[hnwinlen:-hnwinlen] = s
-        window_centers = np.arange(nwindows)*nincrement + hnwinlen
+        windows = sliding_window_view(zs, nwinlen, axis=0)[::nincrement]
+        window_centers = windows[:, hnwinlen]
+        nwindows = len(windows)
     else:
-        first_window_center = hnwinlen+1
-        last_window_center = len(s)-hnwinlen
-        window_centers = np.arange(first_window_center, last_window_center, nincrement, dtype='int')
+        windows = sliding_window_view(s, nwinlen, axis=0)[::nincrement]
+        window_centers = windows[:, hnwinlen]
         nwindows = len(window_centers)
         assert nwindows > 0, "nwindows=0, len(s)=%d, nwinlen=%d, nincrement=%d, window_centers=%s" % (len(s), nwinlen, nincrement, str(window_centers))
         zs = s
         assert window_centers.min() >= hnwinlen, "window_centers.minmax=(%d,%d), hnwinlen=%d, len(s)=%d" % (window_centers.min(), window_centers.max(), hnwinlen, len(s))
         assert window_centers.max() < len(s)-hnwinlen, "window_centers.minmax=(%d,%d), hnwinlen=%d, len(s)=%d" % (window_centers.min(), window_centers.max(), hnwinlen, len(s))
 
     #take the FFT of each segment, padding with zeros when necessary to keep window length the same
     #tf = np.zeros([nfreq, nwindows], dtype='complex')
     tf = np.zeros([nfreq, nwindows], dtype='complex')
-    for k in range(nwindows):
-        center = window_centers[k]
-        si = center - hnwinlen
-        ei = center + hnwinlen + 1
-
-        spec_freq,est = spectrum_estimator.estimate(zs[si:ei], sample_rate, si/sample_rate, ei/sample_rate)
+    for k, window in enumerate(windows):
+        si = window_centers[k] - hnwinlen
+        ei = window_centers[k] + hnwinlen + 1
+        spec_freq,est = spectrum_estimator.estimate(window, sample_rate, si/sample_rate, ei/sample_rate)
         findex = (spec_freq <= max_freq) & (spec_freq >= min_freq)
         #print 'k=%d' % k
         #print 'si=%d, ei=%d' % (si, ei)
         #print 'spec_freq.shape=',spec_freq.shape
         #print 'tf.shape=',tf.shape
         #print 'est.shape=',est.shape
         tf[:, k] = est[findex]
```

### Comparing `soundsig-1.9/soundsig.egg-info/SOURCES.txt` & `soundsig-2.1/soundsig.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 soundsig/__init__.py
 soundsig/basis.py
 soundsig/check_versions.py
 soundsig/coherence.py
```

