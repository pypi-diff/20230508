# Comparing `tmp/shttst-0.0.8.tar.gz` & `tmp/shttst-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shttst-0.0.8.tar", last modified: Mon May  8 06:56:15 2023, max compression
+gzip compressed data, was "shttst-0.0.9.tar", last modified: Mon May  8 09:38:24 2023, max compression
```

## Comparing `shttst-0.0.8.tar` & `shttst-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.345450 shttst-0.0.8/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      418 2023-05-08 06:56:15.344453 shttst-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.8/README.md
--rw-rw-rw-   0        0        0      582 2023-05-08 06:55:59.000000 shttst-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 06:56:15.345450 shttst-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.261087 shttst-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.271187 shttst-0.0.8/src/shttst/
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.301351 shttst-0.0.8/src/shttst/audio/
--rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.8/src/shttst/audio/__init__.py
--rw-rw-rw-   0        0        0     1510 2023-05-04 10:05:14.000000 shttst-0.0.8/src/shttst/audio/audiomentation.py
--rw-rw-rw-   0        0        0     3134 2023-05-07 21:15:32.000000 shttst-0.0.8/src/shttst/audio/tools.py
--rw-rw-rw-   0        0        0     1444 2023-05-08 06:49:09.000000 shttst-0.0.8/src/shttst/audio/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.307684 shttst-0.0.8/src/shttst/dataset/
--rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.8/src/shttst/dataset/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-05-03 08:55:12.000000 shttst-0.0.8/src/shttst/dataset/dataset_files.py
--rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.8/src/shttst/dataset/transcription_line.py
--rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.8/src/shttst/dataset/transcriptions.py
--rw-rw-rw-   0        0        0     1553 2023-05-02 14:08:28.000000 shttst-0.0.8/src/shttst/files.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.323202 shttst-0.0.8/src/shttst/models/
--rw-rw-rw-   0        0        0       94 2023-05-07 21:15:53.000000 shttst-0.0.8/src/shttst/models/__init__.py
--rw-rw-rw-   0        0        0     2511 2023-05-08 06:53:33.000000 shttst-0.0.8/src/shttst/models/silero_vad.py
--rw-rw-rw-   0        0        0    37912 2023-05-08 06:54:40.000000 shttst-0.0.8/src/shttst/models/ultimate_vocal_remover.py
--rw-rw-rw-   0        0        0    19617 2023-05-07 06:02:29.000000 shttst-0.0.8/src/shttst/models/vocal_remover.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.326194 shttst-0.0.8/src/shttst/processing/
--rw-rw-rw-   0        0        0       31 2023-05-02 13:33:57.000000 shttst-0.0.8/src/shttst/processing/__init__.py
--rw-rw-rw-   0        0        0     2125 2023-05-02 14:36:45.000000 shttst-0.0.8/src/shttst/processing/audio_to_dataset.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.334879 shttst-0.0.8/src/shttst/recipes/
--rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.8/src/shttst/recipes/__init__.py
--rw-rw-rw-   0        0        0     3901 2023-05-07 07:35:41.000000 shttst-0.0.8/src/shttst/recipes/chomik.py
--rw-rw-rw-   0        0        0     1126 2023-05-02 13:26:12.000000 shttst-0.0.8/src/shttst/recipes/multiset.py
--rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.8/src/shttst/recipes/prepare_tts_wavs.py
--rw-rw-rw-   0        0        0     2211 2023-05-02 09:25:02.000000 shttst-0.0.8/src/shttst/recipes/transcribe_directory.py
--rw-rw-rw-   0        0        0     1445 2023-05-07 22:01:16.000000 shttst-0.0.8/src/shttst/recipes/yt.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.343455 shttst-0.0.8/src/shttst/text/
--rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.8/src/shttst/text/__init__.py
--rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.8/src/shttst/text/shmart_cleaner.py
--rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.8/src/shttst/text/shmart_nums.py
--rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.8/src/shttst/text/symbols.py
--rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.8/src/shttst/text/text.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.295821 shttst-0.0.8/src/shttst.egg-info/
--rw-rw-rw-   0        0        0      418 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.979344 shttst-0.0.9/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      418 2023-05-08 09:38:24.979344 shttst-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.9/README.md
+-rw-rw-rw-   0        0        0      582 2023-05-08 09:38:07.000000 shttst-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 09:38:24.980492 shttst-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.693554 shttst-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.718918 shttst-0.0.9/src/shttst/
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.783140 shttst-0.0.9/src/shttst/audio/
+-rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.9/src/shttst/audio/__init__.py
+-rw-rw-rw-   0        0        0     1510 2023-05-04 10:05:14.000000 shttst-0.0.9/src/shttst/audio/audiomentation.py
+-rw-rw-rw-   0        0        0     3134 2023-05-07 21:15:32.000000 shttst-0.0.9/src/shttst/audio/tools.py
+-rw-rw-rw-   0        0        0     1444 2023-05-08 06:49:09.000000 shttst-0.0.9/src/shttst/audio/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.818765 shttst-0.0.9/src/shttst/dataset/
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.9/src/shttst/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1679 2023-05-03 08:55:12.000000 shttst-0.0.9/src/shttst/dataset/dataset_files.py
+-rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.9/src/shttst/dataset/transcription_line.py
+-rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.9/src/shttst/dataset/transcriptions.py
+-rw-rw-rw-   0        0        0     1553 2023-05-02 14:08:28.000000 shttst-0.0.9/src/shttst/files.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.851380 shttst-0.0.9/src/shttst/models/
+-rw-rw-rw-   0        0        0       94 2023-05-07 21:15:53.000000 shttst-0.0.9/src/shttst/models/__init__.py
+-rw-rw-rw-   0        0        0     2511 2023-05-08 06:53:33.000000 shttst-0.0.9/src/shttst/models/silero_vad.py
+-rw-rw-rw-   0        0        0    37952 2023-05-08 09:33:27.000000 shttst-0.0.9/src/shttst/models/ultimate_vocal_remover.py
+-rw-rw-rw-   0        0        0    19617 2023-05-07 06:02:29.000000 shttst-0.0.9/src/shttst/models/vocal_remover.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.868205 shttst-0.0.9/src/shttst/processing/
+-rw-rw-rw-   0        0        0       31 2023-05-02 13:33:57.000000 shttst-0.0.9/src/shttst/processing/__init__.py
+-rw-rw-rw-   0        0        0     2125 2023-05-02 14:36:45.000000 shttst-0.0.9/src/shttst/processing/audio_to_dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.918491 shttst-0.0.9/src/shttst/recipes/
+-rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.9/src/shttst/recipes/__init__.py
+-rw-rw-rw-   0        0        0     3901 2023-05-07 07:35:41.000000 shttst-0.0.9/src/shttst/recipes/chomik.py
+-rw-rw-rw-   0        0        0     1126 2023-05-02 13:26:12.000000 shttst-0.0.9/src/shttst/recipes/multiset.py
+-rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.9/src/shttst/recipes/prepare_tts_wavs.py
+-rw-rw-rw-   0        0        0     2211 2023-05-02 09:25:02.000000 shttst-0.0.9/src/shttst/recipes/transcribe_directory.py
+-rw-rw-rw-   0        0        0     1800 2023-05-08 09:36:06.000000 shttst-0.0.9/src/shttst/recipes/yt.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.977325 shttst-0.0.9/src/shttst/text/
+-rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.9/src/shttst/text/__init__.py
+-rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.9/src/shttst/text/shmart_cleaner.py
+-rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.9/src/shttst/text/shmart_nums.py
+-rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.9/src/shttst/text/symbols.py
+-rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.9/src/shttst/text/text.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:38:24.745839 shttst-0.0.9/src/shttst.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-05-08 09:38:24.000000 shttst-0.0.9/src/shttst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2023-05-08 09:38:24.000000 shttst-0.0.9/src/shttst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 09:38:24.000000 shttst-0.0.9/src/shttst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-08 09:38:24.000000 shttst-0.0.9/src/shttst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 09:38:24.000000 shttst-0.0.9/src/shttst.egg-info/top_level.txt
```

### Comparing `shttst-0.0.8/LICENSE` & `shttst-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/pyproject.toml` & `shttst-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shttst"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Shmart TTS tools."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `shttst-0.0.8/src/shttst/audio/audiomentation.py` & `shttst-0.0.9/src/shttst/audio/audiomentation.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/audio/tools.py` & `shttst-0.0.9/src/shttst/audio/tools.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/audio/utils.py` & `shttst-0.0.9/src/shttst/audio/utils.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/dataset/dataset_files.py` & `shttst-0.0.9/src/shttst/dataset/dataset_files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/dataset/transcriptions.py` & `shttst-0.0.9/src/shttst/dataset/transcriptions.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/files.py` & `shttst-0.0.9/src/shttst/files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/models/silero_vad.py` & `shttst-0.0.9/src/shttst/models/silero_vad.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/models/ultimate_vocal_remover.py` & `shttst-0.0.9/src/shttst/models/ultimate_vocal_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 import shutil
 import soundfile as sf
 import threading
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from tqdm import tqdm
-
 from shttst.audio.utils import convert_to_mono_channel, save_audio
 from zipfile import ZipFile
 
 CHECKPOINT_CACHE_PATH = os.path.expanduser('~/.cache/shttst/ultimate_vocal_remover/HP2-4BAND-3090_4band_2.pth')
 ZIP_PATH = os.path.expanduser('~/.cache/shttst/ultimate_vocal_remover/uvr.zip')
 
 def get_checkpoint():
@@ -150,16 +148,16 @@
 
         thread = threading.Thread(target=run_thread, kwargs={'y': wave_left, 'n_fft': n_fft, 'hop_length': hop_length})
         thread.start()
         spec_right = librosa.stft(wave_right, n_fft=n_fft, hop_length=hop_length)
         thread.join()
         spec = np.asfortranarray([spec_left_mt, spec_right])
     else:
-        spec_left = librosa.stft(wave_left, n_fft, hop_length=hop_length)
-        spec_right = librosa.stft(wave_right, n_fft, hop_length=hop_length)
+        spec_left = librosa.stft(wave_left, n_fft=n_fft, hop_length=hop_length)
+        spec_right = librosa.stft(wave_right, n_fft=n_fft, hop_length=hop_length)
         spec = np.asfortranarray([spec_left, spec_right])
 
     return spec
     
 
 def convert_channels(spec, mp, band):
     cc = mp.param['band'][band].get('convert_channels')
@@ -485,15 +483,15 @@
     for d in range(bands_n - 1, 0, -1):
         os.remove(os.path.join('tmp', f'{tmp_basename}_cstw_b{d}_sr' + str(mp.param['band'][d]['sr']) + '.wav'))
         tmp_wav2 = os.path.join('tmp', f'{tmp_basename}_cstw_b{d}_sr' + str(mp.param['sr']) + '.wav')
         wave2, _ = librosa.load(tmp_wav2, sr=mp.param['sr'], mono=False, dtype=np.float32, res_type="sinc_fastest")
         os.remove(tmp_wav2)
         wave = np.add(wave, wave2)
 
-    return wave.T
+    return np.float32(wave.T)
 
 '''
 def fft_lp_filter(spec, bin_start, bin_stop):
     g = 1.0
     for b in range(bin_start, bin_stop):
         g -= 1 / (bin_stop - bin_start)
         spec[:, b, :] = g * spec[:, b, :]
@@ -853,15 +851,15 @@
         self.device = device
         self.window_size = window_size
 
     def _execute(self, X_mag_pad, roi_size, n_window, params):
         self.model.eval()
         with torch.no_grad():
             preds = []
-            for i in tqdm(range(n_window)):
+            for i in range(n_window):
                 start = i * roi_size
                 X_mag_window = X_mag_pad[None, :, :, start:start + self.window_size]
                 X_mag_window = torch.from_numpy(X_mag_window).to(self.device)
 
                 pred = self.model.predict(X_mag_window, params)
 
                 pred = pred.detach().cpu().numpy()
@@ -1009,9 +1007,10 @@
 
         vocals_wave = torch.from_numpy(vocals_wave).permute(1,0)
 
         return convert_to_mono_channel(vocals_wave), convert_to_mono_channel(instruments_wave)
 
 if __name__ == '__main__':
     vocals, instruments = ShmartUltimateVocalRemover()('C:/model/1.wav', tta=True)
+    os.makedirs('/content/vr', exist_ok=True)
     save_audio('/content/vr/vocals.wav', vocals)
     save_audio('/content/vr/instruments.wav', instruments)
```

### Comparing `shttst-0.0.8/src/shttst/models/vocal_remover.py` & `shttst-0.0.9/src/shttst/models/vocal_remover.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/processing/audio_to_dataset.py` & `shttst-0.0.9/src/shttst/processing/audio_to_dataset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/recipes/chomik.py` & `shttst-0.0.9/src/shttst/recipes/chomik.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/recipes/multiset.py` & `shttst-0.0.9/src/shttst/recipes/multiset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/recipes/prepare_tts_wavs.py` & `shttst-0.0.9/src/shttst/recipes/prepare_tts_wavs.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/recipes/transcribe_directory.py` & `shttst-0.0.9/src/shttst/recipes/transcribe_directory.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/text/shmart_cleaner.py` & `shttst-0.0.9/src/shttst/text/shmart_cleaner.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/text/shmart_nums.py` & `shttst-0.0.9/src/shttst/text/shmart_nums.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst/text/text.py` & `shttst-0.0.9/src/shttst/text/text.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.8/src/shttst.egg-info/SOURCES.txt` & `shttst-0.0.9/src/shttst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

