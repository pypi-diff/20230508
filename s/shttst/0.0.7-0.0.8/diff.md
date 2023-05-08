# Comparing `tmp/shttst-0.0.7.tar.gz` & `tmp/shttst-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shttst-0.0.7.tar", last modified: Sun May  7 14:49:36 2023, max compression
+gzip compressed data, was "shttst-0.0.8.tar", last modified: Mon May  8 06:56:15 2023, max compression
```

## Comparing `shttst-0.0.7.tar` & `shttst-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:36.054608 shttst-0.0.7/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      418 2023-05-07 14:49:36.053611 shttst-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.7/README.md
--rw-rw-rw-   0        0        0      582 2023-05-07 14:49:12.000000 shttst-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 14:49:36.054608 shttst-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.699798 shttst-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.730460 shttst-0.0.7/src/shttst/
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.805442 shttst-0.0.7/src/shttst/audio/
--rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.7/src/shttst/audio/__init__.py
--rw-rw-rw-   0        0        0     1510 2023-05-04 10:05:14.000000 shttst-0.0.7/src/shttst/audio/audiomentation.py
--rw-rw-rw-   0        0        0     3110 2023-05-07 06:02:34.000000 shttst-0.0.7/src/shttst/audio/tools.py
--rw-rw-rw-   0        0        0     1133 2023-04-30 12:00:44.000000 shttst-0.0.7/src/shttst/audio/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.860175 shttst-0.0.7/src/shttst/dataset/
--rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.7/src/shttst/dataset/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-05-03 08:55:12.000000 shttst-0.0.7/src/shttst/dataset/dataset_files.py
--rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.7/src/shttst/dataset/transcription_line.py
--rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.7/src/shttst/dataset/transcriptions.py
--rw-rw-rw-   0        0        0     1553 2023-05-02 14:08:28.000000 shttst-0.0.7/src/shttst/files.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.896241 shttst-0.0.7/src/shttst/models/
--rw-rw-rw-   0        0        0       55 2023-05-01 09:12:33.000000 shttst-0.0.7/src/shttst/models/__init__.py
--rw-rw-rw-   0        0        0     2360 2023-05-07 14:47:03.000000 shttst-0.0.7/src/shttst/models/silero_vad.py
--rw-rw-rw-   0        0        0    19617 2023-05-07 06:02:29.000000 shttst-0.0.7/src/shttst/models/vocal_remover.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.917777 shttst-0.0.7/src/shttst/processing/
--rw-rw-rw-   0        0        0       31 2023-05-02 13:33:57.000000 shttst-0.0.7/src/shttst/processing/__init__.py
--rw-rw-rw-   0        0        0     2125 2023-05-02 14:36:45.000000 shttst-0.0.7/src/shttst/processing/audio_to_dataset.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.984777 shttst-0.0.7/src/shttst/recipes/
--rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.7/src/shttst/recipes/__init__.py
--rw-rw-rw-   0        0        0     3901 2023-05-07 07:35:41.000000 shttst-0.0.7/src/shttst/recipes/chomik.py
--rw-rw-rw-   0        0        0     1126 2023-05-02 13:26:12.000000 shttst-0.0.7/src/shttst/recipes/multiset.py
--rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.7/src/shttst/recipes/prepare_tts_wavs.py
--rw-rw-rw-   0        0        0     2211 2023-05-02 09:25:02.000000 shttst-0.0.7/src/shttst/recipes/transcribe_directory.py
--rw-rw-rw-   0        0        0     1445 2023-05-03 08:50:38.000000 shttst-0.0.7/src/shttst/recipes/yt.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:36.051519 shttst-0.0.7/src/shttst/text/
--rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.7/src/shttst/text/__init__.py
--rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.7/src/shttst/text/shmart_cleaner.py
--rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.7/src/shttst/text/shmart_nums.py
--rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.7/src/shttst/text/symbols.py
--rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.7/src/shttst/text/text.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.760250 shttst-0.0.7/src/shttst.egg-info/
--rw-rw-rw-   0        0        0      418 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.345450 shttst-0.0.8/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      418 2023-05-08 06:56:15.344453 shttst-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.8/README.md
+-rw-rw-rw-   0        0        0      582 2023-05-08 06:55:59.000000 shttst-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:56:15.345450 shttst-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.261087 shttst-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.271187 shttst-0.0.8/src/shttst/
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.301351 shttst-0.0.8/src/shttst/audio/
+-rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.8/src/shttst/audio/__init__.py
+-rw-rw-rw-   0        0        0     1510 2023-05-04 10:05:14.000000 shttst-0.0.8/src/shttst/audio/audiomentation.py
+-rw-rw-rw-   0        0        0     3134 2023-05-07 21:15:32.000000 shttst-0.0.8/src/shttst/audio/tools.py
+-rw-rw-rw-   0        0        0     1444 2023-05-08 06:49:09.000000 shttst-0.0.8/src/shttst/audio/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.307684 shttst-0.0.8/src/shttst/dataset/
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.8/src/shttst/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1679 2023-05-03 08:55:12.000000 shttst-0.0.8/src/shttst/dataset/dataset_files.py
+-rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.8/src/shttst/dataset/transcription_line.py
+-rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.8/src/shttst/dataset/transcriptions.py
+-rw-rw-rw-   0        0        0     1553 2023-05-02 14:08:28.000000 shttst-0.0.8/src/shttst/files.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.323202 shttst-0.0.8/src/shttst/models/
+-rw-rw-rw-   0        0        0       94 2023-05-07 21:15:53.000000 shttst-0.0.8/src/shttst/models/__init__.py
+-rw-rw-rw-   0        0        0     2511 2023-05-08 06:53:33.000000 shttst-0.0.8/src/shttst/models/silero_vad.py
+-rw-rw-rw-   0        0        0    37912 2023-05-08 06:54:40.000000 shttst-0.0.8/src/shttst/models/ultimate_vocal_remover.py
+-rw-rw-rw-   0        0        0    19617 2023-05-07 06:02:29.000000 shttst-0.0.8/src/shttst/models/vocal_remover.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.326194 shttst-0.0.8/src/shttst/processing/
+-rw-rw-rw-   0        0        0       31 2023-05-02 13:33:57.000000 shttst-0.0.8/src/shttst/processing/__init__.py
+-rw-rw-rw-   0        0        0     2125 2023-05-02 14:36:45.000000 shttst-0.0.8/src/shttst/processing/audio_to_dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.334879 shttst-0.0.8/src/shttst/recipes/
+-rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.8/src/shttst/recipes/__init__.py
+-rw-rw-rw-   0        0        0     3901 2023-05-07 07:35:41.000000 shttst-0.0.8/src/shttst/recipes/chomik.py
+-rw-rw-rw-   0        0        0     1126 2023-05-02 13:26:12.000000 shttst-0.0.8/src/shttst/recipes/multiset.py
+-rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.8/src/shttst/recipes/prepare_tts_wavs.py
+-rw-rw-rw-   0        0        0     2211 2023-05-02 09:25:02.000000 shttst-0.0.8/src/shttst/recipes/transcribe_directory.py
+-rw-rw-rw-   0        0        0     1445 2023-05-07 22:01:16.000000 shttst-0.0.8/src/shttst/recipes/yt.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.343455 shttst-0.0.8/src/shttst/text/
+-rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.8/src/shttst/text/__init__.py
+-rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.8/src/shttst/text/shmart_cleaner.py
+-rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.8/src/shttst/text/shmart_nums.py
+-rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.8/src/shttst/text/symbols.py
+-rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.8/src/shttst/text/text.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:56:15.295821 shttst-0.0.8/src/shttst.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 06:56:15.000000 shttst-0.0.8/src/shttst.egg-info/top_level.txt
```

### Comparing `shttst-0.0.7/LICENSE` & `shttst-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/pyproject.toml` & `shttst-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shttst"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Shmart TTS tools."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `shttst-0.0.7/src/shttst/audio/audiomentation.py` & `shttst-0.0.8/src/shttst/audio/audiomentation.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/audio/tools.py` & `shttst-0.0.8/src/shttst/audio/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import huggingface_hub
 import torch
 from typing import Tuple
 
 from audclas.tortoise_audio_classifier import TortoiseAudioClassifier
 from shttst.audio.utils import save_audio
-from shttst.models import ShmartSileroVad, ShmartVocalRemover
+from shttst.models import ShmartSileroVad, ShmartUltimateVocalRemover
 
 initialized_models= {}
 
 def initialize_model(type):
     model = None
     
     if type == 'classifier':
         model = TortoiseAudioClassifier()
     elif type == 'denoiser':
-        model = ShmartVocalRemover()
+        model = ShmartUltimateVocalRemover()
     elif type == 'titanet':
         from nemo.collections.asr.models import EncDecSpeakerLabelModel
         model = EncDecSpeakerLabelModel.from_pretrained("nvidia/speakerverification_en_titanet_large", map_location='cpu')
         model.cuda().eval()
     elif type == 'resemblyzer':
         from resemblyzer import VoiceEncoder
         model = VoiceEncoder('cuda', verbose=False)
@@ -44,15 +44,15 @@
     return model(file_path)
 
 def split_by_vad(file_path: str, max_duration: int, min_silence: int) -> str:
     model: ShmartSileroVad = get_model('vad')
     return model.vad_process(file_path, min_silence_duration=min_silence, desired_max_speech_duration=max_duration)
 
 def clean_audio_noise(file_path: str) -> str:
-    vr_model: ShmartVocalRemover = get_model('denoiser')
+    vr_model: ShmartUltimateVocalRemover = get_model('denoiser')
     vocals, instruments = vr_model(file_path, tta=True)
     save_audio(file_path, vocals)
 
 def get_custom_embedding(file_path, type='titanet'):
     if type == 'titanet':
         from nemo.collections.asr.models import EncDecSpeakerLabelModel
         titanet_model: EncDecSpeakerLabelModel = get_model(type)
```

### Comparing `shttst-0.0.7/src/shttst/dataset/dataset_files.py` & `shttst-0.0.8/src/shttst/dataset/dataset_files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/dataset/transcriptions.py` & `shttst-0.0.8/src/shttst/dataset/transcriptions.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/files.py` & `shttst-0.0.8/src/shttst/files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/models/silero_vad.py` & `shttst-0.0.8/src/shttst/models/silero_vad.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 import os
 import torch
 
-from shttst.audio.utils import make_default_tts_wav, save_audio
+from shttst.audio.utils import make_default_tts_wav, resample, save_audio
 from shttst.files import destroy_file
 
 class ShmartSileroVad():
     def __init__(self) -> None:
         vad_model, utils = torch.hub.load(repo_or_dir='snakers4/silero-vad',
                                 model='silero_vad',
                                 force_reload=False,
                                 onnx=False)
         self.vad_model = vad_model
         self.get_speech_timestamps = utils[0]
-        self.read_audio = utils[2]
+        # self.read_audio = utils[2] # replaced with resample to sr=16000 as silero used faulty torchaudio method (see: resample from shttst.audio.utils)
 
     def vad_process(self, audio_file, min_silence_duration = 200, initial_max_speech_duration=30, desired_max_speech_duration=14):
         with torch.no_grad():
-            audio_to_split = self.read_audio(audio_file, sampling_rate=16000)
+            tts_sr = 22050
+            silero_sr = 16000
+            end_frames_fix = int(tts_sr / 12)
+            frames_scale = tts_sr / silero_sr
+            
+            audio_to_split = make_default_tts_wav(audio_file)
+
             timestamps = self.get_speech_timestamps(
-                audio_to_split,
+                resample(audio_to_split, tts_sr, silero_sr),
                 self.vad_model,
                 0.90,  # speech prob threshold
                 16000,  # sample rate
                 800,  # min speech duration in ms
                 initial_max_speech_duration,  # max speech duration in seconds
                 min_silence_duration,  # min silence duration
                 512,  # window size
                 200,  # spech pad ms
             )
 
-            target_sr = 22050
-            post_fix = int(target_sr / 12)
-            scale = target_sr / 16000
 
             result = []
-            audio_to_split = make_default_tts_wav(audio_file)
 
             for i,t in enumerate(timestamps):
-                start = int(t['start'] * scale)
-                end = int(t['end'] * scale) + post_fix
+                start = int(t['start'] * frames_scale)
+                end = int(t['end'] * frames_scale) + end_frames_fix
                 result_audio = audio_to_split[...,start:end]
                 if (result_audio.size(0) > 0):
                     name = os.path.splitext(os.path.basename(audio_file))[0]
                     sample_path = os.path.join(os.path.dirname(audio_file), f'{name}_{i}.wav')
                     save_audio(sample_path, result_audio)
-                    if (result_audio.size(1) > target_sr * desired_max_speech_duration):
+                    if (result_audio.size(1) > tts_sr * desired_max_speech_duration):
                         result.extend(self.vad_process(sample_path, min_silence_duration * 0.75, desired_max_speech_duration * 0.75))
                         destroy_file(sample_path)
                     else:
                         result.append(sample_path)
 
             return result
```

### Comparing `shttst-0.0.7/src/shttst/models/vocal_remover.py` & `shttst-0.0.8/src/shttst/models/vocal_remover.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/processing/audio_to_dataset.py` & `shttst-0.0.8/src/shttst/processing/audio_to_dataset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/recipes/chomik.py` & `shttst-0.0.8/src/shttst/recipes/chomik.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/recipes/multiset.py` & `shttst-0.0.8/src/shttst/recipes/multiset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/recipes/prepare_tts_wavs.py` & `shttst-0.0.8/src/shttst/recipes/prepare_tts_wavs.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/recipes/transcribe_directory.py` & `shttst-0.0.8/src/shttst/recipes/transcribe_directory.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/recipes/yt.py` & `shttst-0.0.8/src/shttst/recipes/yt.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/text/shmart_cleaner.py` & `shttst-0.0.8/src/shttst/text/shmart_cleaner.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/text/shmart_nums.py` & `shttst-0.0.8/src/shttst/text/shmart_nums.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst/text/text.py` & `shttst-0.0.8/src/shttst/text/text.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.7/src/shttst.egg-info/SOURCES.txt` & `shttst-0.0.8/src/shttst.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/shttst/audio/utils.py
 src/shttst/dataset/__init__.py
 src/shttst/dataset/dataset_files.py
 src/shttst/dataset/transcription_line.py
 src/shttst/dataset/transcriptions.py
 src/shttst/models/__init__.py
 src/shttst/models/silero_vad.py
+src/shttst/models/ultimate_vocal_remover.py
 src/shttst/models/vocal_remover.py
 src/shttst/processing/__init__.py
 src/shttst/processing/audio_to_dataset.py
 src/shttst/recipes/__init__.py
 src/shttst/recipes/chomik.py
 src/shttst/recipes/multiset.py
 src/shttst/recipes/prepare_tts_wavs.py
```

