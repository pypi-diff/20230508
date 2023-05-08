# Comparing `tmp/stable-ts-2.5.3.tar.gz` & `tmp/stable-ts-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.5.3.tar", last modified: Sun Apr 30 06:29:08 2023, max compression
+gzip compressed data, was "stable-ts-2.6.0.tar", last modified: Mon May  8 03:27:48 2023, max compression
```

## Comparing `stable-ts-2.5.3.tar` & `stable-ts-2.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 06:29:08.204617 stable-ts-2.5.3/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.5.3/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-30 06:29:08.203617 stable-ts-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 06:29:08.204617 stable-ts-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 06:29:08.129209 stable-ts-2.5.3/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-30 06:29:07.000000 stable-ts-2.5.3/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 06:29:08.201616 stable-ts-2.5.3/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.5.3/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.5.3/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-30 06:25:44.000000 stable-ts-2.5.3/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.5.3/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.5.3/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.5.3/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.5.3/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    34855 2023-04-24 05:25:29.000000 stable-ts-2.5.3/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13214 2023-04-30 06:27:10.000000 stable-ts-2.5.3/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.5.3/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.5.3/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.5.3/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    50492 2023-04-28 16:52:08.000000 stable-ts-2.5.3/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-05-08 03:27:48.099213 stable-ts-2.6.0/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-05-08 03:27:48.098212 stable-ts-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 03:27:48.099213 stable-ts-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 03:27:48.055173 stable-ts-2.6.0/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 03:27:48.096219 stable-ts-2.6.0/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-07 23:07:54.000000 stable-ts-2.6.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.0/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.0/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    34883 2023-05-06 20:00:11.000000 stable-ts-2.6.0/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13549 2023-05-07 22:50:34.000000 stable-ts-2.6.0/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    52677 2023-05-08 03:08:18.000000 stable-ts-2.6.0/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.5.3/LICENSE` & `stable-ts-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/PKG-INFO` & `stable-ts-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.5.3
+Version: 2.6.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.5.3/README.md` & `stable-ts-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/setup.py` & `stable-ts-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.6.0/stable_ts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.5.3
+Version: 2.6.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.5.3/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.6.0/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/audio.py` & `stable-ts-2.6.0/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/decode.py` & `stable-ts-2.6.0/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/enhancement.py` & `stable-ts-2.6.0/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/quantization.py` & `stable-ts-2.6.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/result.py` & `stable-ts-2.6.0/stable_whisper/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,14 +793,15 @@
     def reset(self):
         self.language = self.ori_dict.get('language')
         segments = self.ori_dict.get('segments')
         self.segments: List[Segment] = [Segment(**s) for s in segments] if segments else []
 
     to_srt_vtt = result_to_srt_vtt
     to_ass = result_to_ass
+    to_tsv = result_to_tsv
     save_as_json = save_as_json
 
 
 class SegmentMatch:
 
     def __init__(
             self,
```

### Comparing `stable-ts-2.5.3/stable_whisper/stabilization.py` & `stable-ts-2.6.0/stable_whisper/stabilization.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,29 +36,33 @@
     if warn and not valid:
         warnings.warn(message='Found timestamp(s) jumping backwards in time. '
                               'Use word_timestamps=True to avoid the issue.')
     return valid
 
 
 def mask2timing(
-        silence_mask: (np.ndarray, torch.Tensor)
+        silence_mask: (np.ndarray, torch.Tensor),
+        time_offset: float = 0.0,
 ) -> (Tuple[np.ndarray, np.ndarray], None):
     if silence_mask is None or not silence_mask.any():
         return
     assert silence_mask.ndim == 1
     if isinstance(silence_mask, torch.Tensor):
-        silences = silence_mask.cpu().numpy()
+        silences = silence_mask.cpu().numpy().copy()
     elif isinstance(silence_mask, np.ndarray):
         silences = silence_mask.copy()
     else:
         raise NotImplementedError(f'Expected torch.Tensor or numpy.ndarray, but got {type(silence_mask)}')
     silences[0] = False
     silences[-1] = False
     silent_starts = np.logical_and(~silences[:-1], silences[1:]).nonzero()[0] / TOKENS_PER_SECOND
-    silent_ends = np.logical_and(silences[:-1], ~silences[1:]).nonzero()[0] / TOKENS_PER_SECOND
+    silent_ends = (np.logical_and(silences[:-1], ~silences[1:]).nonzero()[0] + 1) / TOKENS_PER_SECOND
+    if time_offset:
+        silent_starts += time_offset
+        silent_ends += time_offset
     return silent_starts, silent_ends
 
 
 def timing2mask(
         silent_starts: np.ndarray,
         silent_ends: np.ndarray,
         size: int,
@@ -68,15 +72,15 @@
     ts_token_mask = torch.zeros(size, dtype=torch.bool)
     if time_offset:
         silent_starts = (silent_starts - time_offset).clip(min=0)
         silent_ends = (silent_ends - time_offset).clip(min=0)
     mask_i = (silent_starts * TOKENS_PER_SECOND).round().astype(np.int16)
     mask_e = (silent_ends * TOKENS_PER_SECOND).round().astype(np.int16)
     for mi, me in zip(mask_i, mask_e):
-        ts_token_mask[mi:me] = True
+        ts_token_mask[mi:me+1] = True
 
     return ts_token_mask
 
 
 def suppress_silence(
         result_obj,
         silent_starts: np.ndarray,
@@ -128,17 +132,18 @@
     audio_tensor = audio_tensor.abs()
     k = int(audio_tensor.numel() * 0.001)
     if k:
         top_values, _ = torch.topk(audio_tensor, k)
         threshold = top_values[-1]
     else:
         threshold = audio_tensor.quantile(0.999, dim=-1)
-    audio_tensor = audio_tensor / min(1., (threshold * 1.75))
-    token_count = round(audio_tensor.shape[-1] / N_SAMPLES_PER_TOKEN)
-    if token_count > 1:
+    if (token_count := round(audio_tensor.shape[-1] / N_SAMPLES_PER_TOKEN)+1) > 2:
+        if threshold < 1e-5:
+            return torch.zeros(token_count, dtype=audio_tensor.dtype, device=audio_tensor.device)
+        audio_tensor = audio_tensor / min(1., max(threshold * 1.75, .3))
         audio_tensor = F.interpolate(
             audio_tensor[None, None],
             size=token_count,
             mode='linear',
             align_corners=False
         )[0, 0]
         return audio_tensor
@@ -157,20 +162,20 @@
         raise NotImplementedError(f'audio size, {loudness_tensor.shape[0]}, is too short to visualize')
     else:
         width = loudness_tensor.shape[0] if width == -1 else width
         im = torch.zeros((height, width, 3), dtype=torch.uint8)
         mid = round(height / 2)
         for i, j in enumerate(loudness_tensor.tolist()):
             j = round(abs(j) * mid)
-            if j == 0 or width < i:
+            if j == 0 or width <= i:
                 continue
             im[mid - j:mid + 1, i] = 255
             im[mid + 1:mid + j + 1, i] = 255
         if not no_silence:
-            im[:, silence_mask, 1:] = 0
+            im[:, silence_mask[:width], 1:] = 0
         im = im.cpu().numpy()
         if output and not output.endswith('.png'):
             output += '.png'
         try:
             from PIL import Image
         except ModuleNotFoundError:
             try:
@@ -222,24 +227,24 @@
         mask = loudness_tensor.clone()
 
     if q_levels:
         mask = mask.mul(q_levels).round()
 
     mask = mask.bool()
 
+    if not mask.any():  # entirely silent
+        return ~mask
     temp_timings = mask2timing(mask)
-    if temp_timings is None:
-        return
     s, e = temp_timings
     se_mask = (e - s) > 0.1
     s = s[se_mask]
     e = e[se_mask]
     mask = ~timing2mask(s, e, loudness_tensor.shape[-1])
 
-    if not mask.any():
+    if not mask.any():  # no silence
         return
 
     return mask
 
 
 _model_cache = {}
 
@@ -360,12 +365,12 @@
     loudness_tensor = audio2loudness(audio)
     width = min(max_width, loudness_tensor.shape[-1])
     if loudness_tensor is None:
         raise NotImplementedError(f'Audio is too short and cannot visualized.')
 
     if vad:
         silence_timings = get_vad_silence_func()(audio, vad_threshold)
-        silence_mask = None if silence_timings is None else timing2mask(*silence_timings, size=width)
+        silence_mask = None if silence_timings is None else timing2mask(*silence_timings, size=loudness_tensor.shape[0])
     else:
         silence_mask = wav2mask(audio, q_levels=q_levels, k_size=k_size)
 
     visualize_mask(loudness_tensor, silence_mask, width=width, height=height, output=output)
```

### Comparing `stable-ts-2.5.3/stable_whisper/text_output.py` & `stable-ts-2.6.0/stable_whisper/text_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import warnings
 from typing import List, Tuple, Union, Callable
 from itertools import chain
 from .stabilization import valid_ts
 
-__all__ = ['result_to_srt_vtt', 'result_to_ass', 'save_as_json', 'load_result']
+__all__ = ['result_to_srt_vtt', 'result_to_ass', 'result_to_tsv', 'save_as_json', 'load_result']
 
 
 def _save_as_file(content: str, path: str):
     with open(path, 'w', encoding='utf-8') as f:
         f.write(content)
     print(f'Saved: {os.path.abspath(path)}')
 
@@ -26,14 +26,22 @@
 
 def sec2hhmmss(seconds: (float, int)):
     mm, ss = divmod(seconds, 60)
     hh, mm = divmod(mm, 60)
     return hh, mm, ss
 
 
+def sec2milliseconds(seconds: (float, int)) -> int:
+    return round(seconds * 1000)
+
+
+def sec2centiseconds(seconds: (float, int)) -> int:
+    return round(seconds * 100)
+
+
 def sec2vtt(seconds: (float, int)) -> str:
     hh, mm, ss = sec2hhmmss(seconds)
     return f'{hh:0>2.0f}:{mm:0>2.0f}:{ss:0>6.3f}'
 
 
 def sec2srt(seconds: (float, int)) -> str:
     return sec2vtt(seconds).replace(".", ",")
@@ -55,14 +63,20 @@
 
 
 def segment2assblock(segment: dict, idx: int, strip=True) -> str:
     return f'Dialogue: {idx},{sec2ass(segment["start"])},{sec2ass(segment["end"])},Default,,0,0,0,,' \
            f'{segment["text"].strip() if strip else segment["text"]}'
 
 
+def segment2tsvblock(segment: dict, strip=True) -> str:
+    return f'{sec2milliseconds(segment["start"])}' \
+           f'\t{sec2milliseconds(segment["end"])}' \
+           f'\t{segment["text"].strip() if strip else segment["text"]}'
+
+
 def words2segments(words: List[dict], tag: Tuple[str, str], reverse_text: bool = False) -> List[dict]:
     def add_tag(idx: int):
         return ''.join(
             (
                 f" {tag[0]}{w['word'][1:]}{tag[1]}"
                 if w['word'].startswith(' ') else
                 f"{tag[0]}{w['word']}{tag[1]}"
@@ -94,14 +108,69 @@
         chain.from_iterable(
             words2segments(s['words'], tag, reverse_text=s.get('reversed_text'))
             for s in segments
         )
     )
 
 
+def to_vtt_word_level_segments(segments: List[dict], tag: Tuple[str, str] = None) -> List[dict]:
+    def to_segment_string(segment: dict):
+        segment_string = ''
+        prev_end = 0
+        for i, word in enumerate(segment['words']):
+            if i != 0:
+                curr_start = word['start']
+                if prev_end == curr_start:
+                    segment_string += f"<{sec2vtt(curr_start)}>"
+                else:
+                    if segment_string.endswith(' '):
+                        segment_string = segment_string[:-1]
+                    elif segment['words'][i]['word'].startswith(' '):
+                        segment['words'][i]['word'] = segment['words'][i]['word'][1:]
+                    segment_string += f"<{sec2vtt(prev_end)}> <{sec2vtt(curr_start)}>"
+            segment_string += word['word']
+            prev_end = word['end']
+        return segment_string
+
+    return [
+        dict(
+            text=to_segment_string(s),
+            start=s['start'],
+            end=s['end']
+        )
+        for s in segments
+    ]
+
+
+def to_ass_word_level_segments(segments: List[dict], tag: Tuple[str, str], karaoke: bool = False) -> List[dict]:
+
+    def to_segment_string(segment: dict):
+        segment_string = ''
+        for i, word in enumerate(segment['words']):
+            curr_word, space = (word['word'][1:], " ") if word['word'].startswith(" ") else (word['word'], "")
+            segment_string += (
+                    space +
+                    r"{\k" +
+                    ("f" if karaoke else "") +
+                    f"{sec2centiseconds(word['end']-word['start'])}" +
+                    r"}" +
+                    curr_word
+            )
+        return segment_string
+
+    return [
+        dict(
+            text=to_segment_string(s),
+            start=s['start'],
+            end=s['end']
+        )
+        for s in segments
+    ]
+
+
 def to_word_level(segments: List[dict]) -> List[dict]:
     return [dict(text=w['word'], start=w['start'], end=w['end']) for s in segments for w in s['words']]
 
 
 def _confirm_word_level(segments: List[dict]) -> bool:
     if not all(bool(s.get('words')) for s in segments):
         warnings.warn('Result is missing word timestamps. Word-level timing cannot be exported. '
@@ -128,15 +197,16 @@
                   segments2blocks: Callable = None,
                   segment_level=True,
                   word_level=True,
                   min_dur: float = 0.02,
                   tag: Tuple[str, str] = None,
                   default_tag: Tuple[str, str] = None,
                   strip=True,
-                  reverse_text: Union[bool, tuple] = False):
+                  reverse_text: Union[bool, tuple] = False,
+                  to_word_level_string_callback: Callable = None):
     """
 
     Generate file from result to display segment-level and/or word-level timestamp.
 
     Returns
     -------
     string of content if no [filepath] is provided, else None
@@ -156,15 +226,17 @@
 
     if word_level and segment_level:
         if tag is None:
             if default_tag is None:
                 tag = ('<font color="#00ff00">', '</font>') if filetype == 'srt' else ('<u>', '</u>')
             else:
                 tag = default_tag
-        segments = to_word_level_segments(segments, tag)
+        if to_word_level_string_callback is None:
+            to_word_level_string_callback = to_word_level_segments
+        segments = to_word_level_string_callback(segments, tag)
     elif word_level:
         segments = to_word_level(segments)
 
     valid_ts(segments)
 
     if segments2blocks is None:
         sub_str = '\n\n'.join(segment2srtblock(s, i, strip=strip) for i, s in enumerate(segments))
@@ -222,40 +294,104 @@
     -------
     string of content if no [filepath] is provided, else None
 
     """
     is_srt = (filepath is None or not filepath.lower().endswith('.vtt')) if vtt is None else not vtt
     if is_srt:
         segments2blocks = None
+        to_word_level_string_callback = None
     else:
         def segments2blocks(segments):
             return 'WEBVTT\n\n' + '\n\n'.join(segment2vttblock(s, strip=strip) for i, s in enumerate(segments))
+        to_word_level_string_callback = to_vtt_word_level_segments if tag is None else tag
+
     return result_to_any(
         result=result,
         filepath=filepath,
         filetype=('vtt', 'srt')[is_srt],
         segments2blocks=segments2blocks,
         segment_level=segment_level,
         word_level=word_level,
         min_dur=min_dur,
         tag=tag,
         strip=strip,
+        reverse_text=reverse_text,
+        to_word_level_string_callback=to_word_level_string_callback
+    )
+
+
+def result_to_tsv(result: (dict, list),
+                  filepath: str = None,
+                  segment_level: bool = None,
+                  word_level: bool = None,
+                  min_dur: float = 0.02,
+                  strip=True,
+                  reverse_text: Union[bool, tuple] = False):
+    """
+
+    Generate TSV from result to display segment-level and/or word-level timestamp.
+
+    Parameters
+    ----------
+    result: (dict, list)
+        result from modified model
+    filepath: str:
+        path to save file. if no path is specified, the content will be returned as a str instead
+    segment_level: bool:
+        whether to use segment-level timestamps in output (default: True)
+    word_level: bool
+        whether to use word-level timestamps in output (default: False)
+    min_dur: float
+        minimum duration any word/segment is allowed to have. (default: 0.02)
+        if the duration is less than this threshold, the word/segments will be merged with adjacent word/segments.
+    strip: bool
+        whether to remove spaces before and after text on each segment for output (default: True)
+    reverse_text: Union[bool, tuple]
+        whether to reverse the order of words for each segment (default: False)
+        or provide the [prepend_punctuations] and [append_punctuations] as tuple pair instead of True
+        to match transcription settings (if True, the default punctuations will be used)
+        Note: This will not fix RTL text not displaying tags properly which is an issue with video player.
+                VLC seems to not suffer from this issue.
+
+    Returns
+    -------
+    string of content if no [filepath] is provided, else None
+
+    """
+    if segment_level is None and word_level is None:
+        segment_level = True
+    assert word_level is not segment_level, '[word_level] and [segment_level] cannot be the same ' \
+                                            'since [tag] is not support for this format'
+
+    def segments2blocks(segments):
+        return '\n\n'.join(segment2tsvblock(s, strip=strip) for i, s in enumerate(segments))
+    return result_to_any(
+        result=result,
+        filepath=filepath,
+        filetype='tsv',
+        segments2blocks=segments2blocks,
+        segment_level=segment_level,
+        word_level=word_level,
+        min_dur=min_dur,
+        strip=strip,
         reverse_text=reverse_text
     )
 
 
 def result_to_ass(result: (dict, list),
                   filepath: str = None,
                   segment_level=True,
                   word_level=True,
                   min_dur: float = 0.02,
                   tag: Tuple[str, str] = None,
                   font: str = None,
                   font_size: int = 24,
                   strip=True,
+                  highlight_color: str = None,
+                  karaoke=False,
                   reverse_text: Union[bool, tuple] = False,
                   **kwargs):
     """
 
     Generate Advanced SubStation Alpha (ASS) file from result to display segment-level and/or word-level timestamp.
 
     Note: ass file is used in the same way as srt, vtt, etc.
@@ -270,21 +406,25 @@
         whether to use segment-level timestamps in output (default: True)
     word_level: bool
         whether to use word-level timestamps in output (default: True)
     min_dur: float
         minimum duration any word/segment is allowed to have. (default: 0.02)
         if the duration is less than this threshold, the word/segments will be merged with adjacent word/segments.
     tag: Tuple[str, str]
-        tag used to change the properties a word at its timestamp (default: '{\\1c&HFF00&}', '{\\r}')
+        tag used to change the properties a word at its timestamp (default: None)
     font: str
         word font (default: Arial)
     font_size: int
         word font size (default: 48)
     strip: bool
         whether to remove spaces before and after text on each segment for output (default: True)
+    highlight_color: str
+        hexadecimal of highlight color, or [PrimaryColour], as '<bb><gg><rr>' (default: '00ff00' if highlight is needed)
+    karaoke: bool
+        whether to use progressive filling highlights (for karaoke effect) (default: False)
     reverse_text: Union[bool, tuple]
         whether to reverse the order of words for each segment (default: False)
         or provide the [prepend_punctuations] and [append_punctuations] as tuple pair instead of True
         to match transcription settings (if True, the default punctuations will be used)
         Note: This will not fix RTL text not displaying tags properly which is an issue with video player.
                 VLC seems to not suffer from this issue.
     kwargs:
@@ -294,27 +434,33 @@
         'Shadow', 'Alignment', 'MarginL', 'MarginR', 'MarginV', 'Encoding'
 
     Returns
     -------
     string of content if no [filepath] is provided, else None
 
     """
+    if highlight_color is None and (karaoke or (word_level and segment_level)):
+        highlight_color = '00ff00'
 
     def segments2blocks(segments):
         fmt_style_dict = {'Name': 'Default', 'Fontname': 'Arial', 'Fontsize': '48', 'PrimaryColour': '&Hffffff',
                           'SecondaryColour': '&Hffffff', 'OutlineColour': '&H0', 'BackColour': '&H0', 'Bold': '0',
                           'Italic': '0', 'Underline': '0', 'StrikeOut': '0', 'ScaleX': '100', 'ScaleY': '100',
                           'Spacing': '0', 'Angle': '0', 'BorderStyle': '1', 'Outline': '1', 'Shadow': '0',
                           'Alignment': '2', 'MarginL': '10', 'MarginR': '10', 'MarginV': '10', 'Encoding': '0'}
 
         for k, v in filter(lambda x: 'colour' in x[0].lower() and not str(x[1]).startswith('&H'), kwargs.items()):
             kwargs[k] = f'&H{kwargs[k]}'
 
         fmt_style_dict.update((k, v) for k, v in kwargs.items() if k in fmt_style_dict)
 
+        if highlight_color:
+            fmt_style_dict['PrimaryColour'] = \
+                highlight_color if highlight_color.startswith('&H') else f'&H{highlight_color}'
+
         if font:
             fmt_style_dict.update(Fontname=font)
         if font_size:
             fmt_style_dict.update(Fontsize=font_size)
 
         fmts = f'Format: {", ".join(map(str, fmt_style_dict.keys()))}'
 
@@ -324,26 +470,34 @@
                   f'[V4+ Styles]\n{fmts}\n{styles}\n\n' \
                   f'[Events]\nFormat: Layer, Start, End, Style, Name, MarginL, MarginR, MarginV, Effect, Text\n\n'
 
         sub_str += '\n'.join(segment2assblock(s, i, strip=strip) for i, s in enumerate(segments))
 
         return sub_str
 
+    if tag is not None and karaoke:
+        warnings.warn(f'[tag] is not support for [karaoke]=True; [tag] will be ignored.')
+
     return result_to_any(
         result=result,
         filepath=filepath,
         filetype='ass',
         segments2blocks=segments2blocks,
         segment_level=segment_level,
         word_level=word_level,
         min_dur=min_dur,
         tag=tag,
-        default_tag=(r'{\1c&' + 'HFF00&' + '}', r'{\r}'),
+        default_tag=(r'{\1c' + f'{highlight_color}&' + '}', r'{\r}'),
         strip=strip,
-        reverse_text=reverse_text
+        reverse_text=reverse_text,
+        to_word_level_string_callback=(
+            lambda s, t: to_ass_word_level_segments(s, t, karaoke=karaoke)
+            if karaoke or (word_level and segment_level)
+            else None
+        )
     )
 
 
 def save_as_json(result: dict, path: str):
     """
     Save result as json.
     """
```

### Comparing `stable-ts-2.5.3/stable_whisper/timing.py` & `stable-ts-2.6.0/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/video_output.py` & `stable-ts-2.6.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.5.3/stable_whisper/whisper_word_level.py` & `stable-ts-2.6.0/stable_whisper/whisper_word_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,35 +252,69 @@
                 audio = torch.from_numpy(audio)
             audio = resample(audio, input_sr, curr_sr, resampling_method="kaiser_window")
     if only_voice_freq:
         from .audio import voice_freq_filter
         audio = voice_freq_filter(audio, curr_sr)
     sample_padding = int(N_FFT // 2) + 1
     whole_mel = log_mel_spectrogram(audio, padding=sample_padding) if mel_first else None
+    tokenizer = None
+    initial_prompt_tokens = []
+    task = decode_options.get("task", "transcribe")
 
-    if decode_options.get("language", None) is None and model:
-        if not model.is_multilingual:
-            decode_options["language"] = "en"
-        else:
-            if verbose:
-                print("Detecting language using up to the first 30 seconds. Use `--language` to specify the language")
-            mel_segment = log_mel_spectrogram(audio[..., :N_SAMPLES], padding=sample_padding) \
-                if whole_mel is None else whole_mel[..., :N_FRAMES]
-            mel_segment = pad_or_trim(mel_segment, N_FRAMES).to(device=model.device, dtype=dtype)
-            _, probs = model.detect_language(mel_segment)
-            decode_options["language"] = max(probs, key=probs.get)
-            if verbose is not None:
-                print(f"Detected language: {LANGUAGES[decode_options['language']]}")
+    def detect_language():
+        nonlocal tokenizer
+        if tokenizer is None:
+            if decode_options.get("language", None) is None and model:
+                if not model.is_multilingual:
+                    decode_options["language"] = "en"
+                else:
+                    if verbose:
+                        print("Detecting language using up to 30 seconds following first non-silent sample. "
+                              "Use `--language` to specify the language")
+                    timing_mask = np.logical_and(
+                        segment_silence_timing[0] <= time_offset,
+                        segment_silence_timing[1] >= time_offset
+                    )
+                    start_sample = (
+                        None
+                        if segment_silence_timing is None or not timing_mask.any() else
+                        round(segment_silence_timing[1][timing_mask.nonzero()[0]][0] * SAMPLE_RATE)
+                    )
+                    if start_sample is None:
+                        nonlocal mel_segment
+                        curr_mel_segment = mel_segment
+                    else:
+                        if whole_mel is None:
+                            curr_mel_segment = log_mel_spectrogram(
+                                audio[..., start_sample:start_sample+N_SAMPLES],
+                                padding=sample_padding
+                            )
+                        else:
+                            start_frame = int(start_sample/HOP_LENGTH)
+                            curr_mel_segment = whole_mel[..., start_frame:start_frame+N_FRAMES]
+                        curr_mel_segment = pad_or_trim(curr_mel_segment, N_FRAMES).to(device=model.device, dtype=dtype)
+                    _, probs = model.detect_language(curr_mel_segment)
+                    decode_options["language"] = max(probs, key=probs.get)
+                    if verbose is not None:
+                        detected_msg = f"Detected language: {LANGUAGES[decode_options['language']]}"
+                        if tqdm_pbar.disable:
+                            print(detected_msg)
+                        else:
+                            tqdm_pbar.write(detected_msg)
 
-    language = decode_options["language"]
-    task = decode_options.get("task", "transcribe")
-    tokenizer = get_tokenizer(model.is_multilingual, language=language, task=task)
+            language = decode_options["language"]
+            tokenizer = get_tokenizer(model.is_multilingual, language=language, task=task)
+
+            if word_timestamps and task == "translate":
+                warnings.warn("Word-level timestamps on translations may not be reliable.")
 
-    if word_timestamps and task == "translate":
-        warnings.warn("Word-level timestamps on translations may not be reliable.")
+            if initial_prompt is not None:
+                nonlocal initial_prompt_tokens
+                initial_prompt_tokens = tokenizer.encode(" " + initial_prompt.strip())
+                all_tokens.extend(initial_prompt_tokens)
 
     audio_features = None
 
     def decode_with_fallback(seg: torch.Tensor,
                              ts_token_mask: torch.Tensor = None) \
             -> DecodingResult:
         nonlocal audio_features
@@ -327,20 +361,14 @@
     time_precision = (
             input_stride * HOP_LENGTH / SAMPLE_RATE
     )  # time per output token: 0.02 (seconds)
     all_tokens = []
     all_segments = []
     prompt_reset_since = 0
 
-    if initial_prompt is not None:
-        initial_prompt_tokens = tokenizer.encode(" " + initial_prompt.strip())
-        all_tokens.extend(initial_prompt_tokens)
-    else:
-        initial_prompt_tokens = []
-
     def new_segment(
             *, start: float, end: float, tokens: torch.Tensor, result: DecodingResult
     ):
         tokens = tokens.tolist()
         text_tokens = [token for token in tokens if token < tokenizer.eot]
         return {
             "seek": round(seek_sample / SAMPLE_RATE, 3),  # units in seconds
@@ -395,15 +423,15 @@
             mel_segment = pad_or_trim(mel_segment, N_FRAMES).to(device=model.device, dtype=dtype)
 
             segment_silence_timing = None
             ts_token_mask = None
             if suppress_silence:
                 if silence_timing is None:
                     ts_token_mask = wav2mask(audio_segment, q_levels=q_levels, k_size=k_size)
-                    segment_silence_timing = mask2timing(ts_token_mask)
+                    segment_silence_timing = mask2timing(ts_token_mask, time_offset=time_offset)
                 else:
                     timing_indices = np.logical_and(
                         silence_timing[1] > time_offset,
                         silence_timing[0] < time_offset + segment_duration
                     )
                     segment_silence_timing = (silence_timing[0][timing_indices], silence_timing[1][timing_indices])
 
@@ -414,14 +442,15 @@
 
                 if ts_token_mask is not None:
                     if ts_token_mask.all():  # segment is silent
                         fast_forward()
                         continue
                     ts_token_mask = pad_or_trim(ts_token_mask, 1501)
 
+            detect_language()
             decode_options["prompt"] = all_tokens[prompt_reset_since:]
             result: DecodingResult = decode_with_fallback(mel_segment, ts_token_mask=ts_token_mask)
             tokens = torch.tensor(result.tokens)
 
             if no_speech_threshold is not None:
                 # no voice activity check
                 should_skip = result.no_speech_prob > no_speech_threshold
@@ -568,22 +597,25 @@
         update_pbar()
 
     if model.device != torch.device('cpu'):
         torch.cuda.empty_cache()
 
     final_result = WhisperResult(dict(text=tokenizer.decode(all_tokens[len(initial_prompt_tokens):]),
                                       segments=all_segments,
-                                      language=language,
+                                      language=tokenizer.language,
                                       time_scale=time_scale))
     if word_timestamps and regroup:
         final_result.regroup()
 
     if time_scale is not None:
         final_result.rescale_time(1 / time_scale)
 
+    if len(final_result.text) == 0:
+        warnings.warn(f'Failed to {task} audio. Result contains no text. ')
+
     return final_result
 
 
 def modify_model(model: "Whisper"):
     """
     Modifies model instance by:
         -replacing model.decode with decode_word_level
@@ -649,15 +681,15 @@
 
     def str2bool(string: str) -> bool:
         string = string.lower()
         if string in str2val:
             return str2val[string]
         raise ValueError(f"Expected one of {set(str2val.keys())}, got {string}")
 
-    output_formats = {"srt", "ass", "json", "vtt"}
+    output_formats = {"srt", "ass", "json", "vtt", "tsv"}
 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("inputs", nargs="+", type=str,
                         help="audio/video filepath/URL(s) to transcribe "
                              "or json file(s) to process into [output_format]")
     parser.add_argument("--output", "-o", nargs="+", type=str,
                         help="output filepaths(s);"
@@ -833,14 +865,17 @@
     parser.add_argument("--no_speech_threshold", type=optional_float, default=0.6,
                         help="if the probability of the <|nospeech|> token is higher than this value AND the decoding "
                              "has failed due to `logprob_threshold`, consider the segment as silence")
     parser.add_argument("--threads", type=optional_int, default=0,
                         help="number of threads used by torch for CPU inference; "
                              "supercedes MKL_NUM_THREADS/OMP_NUM_THREADS")
 
+    parser.add_argument('--mel_first', action='store_true',
+                        help='process entire audio track into log-Mel spectrogram first instead in chunks')
+
     parser.add_argument('--only_ffmpeg', action='store_true',
                         help='whether to use only FFmpeg (and not yt-dlp) for URls')
 
     parser.add_argument('--overwrite', '-y', action='store_true',
                         help='overwrite all output files')
 
     parser.add_argument('--debug', action='store_true',
@@ -1050,14 +1085,22 @@
                 filepath=output_path,
                 segment_level=segment_level,
                 word_level=word_level,
                 tag=tag,
                 strip=strip,
                 reverse_text=reverse_text
             )
+        elif output_path.endswith('.tsv'):
+            result.to_tsv(
+                filepath=output_path,
+                segment_level=segment_level,
+                word_level=word_level,
+                strip=strip,
+                reverse_text=reverse_text
+            )
         else:
             result.to_ass(
                 filepath=output_path,
                 segment_level=segment_level,
                 word_level=word_level,
                 tag=tag,
                 font=font,
```

