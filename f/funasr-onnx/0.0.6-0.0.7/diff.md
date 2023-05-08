# Comparing `tmp/funasr_onnx-0.0.6.tar.gz` & `tmp/funasr_onnx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr_onnx-0.0.6.tar", last modified: Fri Apr 21 11:17:57 2023, max compression
+gzip compressed data, was "funasr_onnx-0.0.7.tar", last modified: Sun May  7 16:24:50 2023, max compression
```

## Comparing `funasr_onnx-0.0.6.tar` & `funasr_onnx-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6094 2023-04-21 03:10:43.000000 funasr_onnx-0.0.6/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr_onnx-0.0.6/funasr_onnx/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr_onnx-0.0.6/funasr_onnx/paraformer_bin.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr_onnx-0.0.6/funasr_onnx/punc_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr_onnx-0.0.6/funasr_onnx/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr_onnx-0.0.6/funasr_onnx/utils/e2e_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15848 2023-04-21 11:13:25.000000 funasr_onnx-0.0.6/funasr_onnx/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr_onnx-0.0.6/funasr_onnx/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr_onnx-0.0.6/funasr_onnx/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr_onnx-0.0.6/funasr_onnx/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr_onnx-0.0.6/funasr_onnx/vad_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      485 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1393 2023-04-21 11:13:25.000000 funasr_onnx-0.0.6/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:24:50.617407 funasr_onnx-0.0.7/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8882 2023-05-07 16:24:50.617139 funasr_onnx-0.0.7/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     8264 2023-04-23 09:14:56.000000 funasr_onnx-0.0.7/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:24:50.612841 funasr_onnx-0.0.7/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.0.7/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr_onnx-0.0.7/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12279 2023-05-05 07:04:25.000000 funasr_onnx-0.0.7/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:24:50.616681 funasr_onnx-0.0.7/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.0.7/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.0.7/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr_onnx-0.0.7/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.0.7/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.0.7/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr_onnx-0.0.7/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr_onnx-0.0.7/funasr_onnx/vad_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:24:50.614096 funasr_onnx-0.0.7/funasr_onnx.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8882 2023-05-07 16:24:50.000000 funasr_onnx-0.0.7/funasr_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)      485 2023-05-07 16:24:50.000000 funasr_onnx-0.0.7/funasr_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-07 16:24:50.000000 funasr_onnx-0.0.7/funasr_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       90 2023-05-07 16:24:50.000000 funasr_onnx-0.0.7/funasr_onnx.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-05-07 16:24:50.000000 funasr_onnx-0.0.7/funasr_onnx.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-07 16:24:50.617464 funasr_onnx-0.0.7/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-05-07 16:24:45.000000 funasr_onnx-0.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `funasr_onnx-0.0.6/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.0.7/funasr_onnx/paraformer_bin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os.path
 from pathlib import Path
 from typing import List, Union, Tuple
 
 import copy
 import librosa
@@ -15,14 +17,19 @@
 from .utils.frontend import WavFrontend
 from .utils.timestamp_utils import time_stamp_lfr6_onnx
 
 logging = get_logger()
 
 
 class Paraformer():
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
+    https://arxiv.org/abs/2206.08317
+    """
     def __init__(self, model_dir: Union[str, Path] = None,
                  batch_size: int = 1,
                  device_id: Union[str, int] = "-1",
                  plot_timestamp_to: str = "",
                  quantize: bool = False,
                  intra_op_num_threads: int = 4,
                  ):
```

### Comparing `funasr_onnx-0.0.6/funasr_onnx/punc_bin.py` & `funasr_onnx-0.0.7/funasr_onnx/punc_bin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os.path
 from pathlib import Path
 from typing import List, Union, Tuple
 import numpy as np
 
 from .utils.utils import (ONNXRuntimeError,
```

### Comparing `funasr_onnx-0.0.6/funasr_onnx/utils/e2e_vad.py` & `funasr_onnx-0.0.7/funasr_onnx/utils/e2e_vad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
 from enum import Enum
 from typing import List, Tuple, Dict, Any
 
 import math
 import numpy as np
 
 class VadStateMachine(Enum):
@@ -185,14 +189,19 @@
         return AudioChangeState.kChangeStateInvalid
 
     def FrameSizeMs(self) -> int:
         return int(self.frame_size_ms)
 
 
 class E2EVadModel():
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
     def __init__(self, vad_post_args: Dict[str, Any]):
         super(E2EVadModel, self).__init__()
         self.vad_opts = VADXOptions(**vad_post_args)
         self.windows_detector = WindowDetector(self.vad_opts.window_size_ms,
                                                self.vad_opts.sil_to_speech_time_thres,
                                                self.vad_opts.speech_to_sil_time_thres,
                                                self.vad_opts.frame_in_ms)
@@ -216,18 +225,19 @@
 
         self.output_data_buf = []
         self.output_data_buf_offset = 0
         self.frame_probs = []
         self.max_end_sil_frame_cnt_thresh = self.vad_opts.max_end_silence_time - self.vad_opts.speech_to_sil_time_thres
         self.speech_noise_thres = self.vad_opts.speech_noise_thres
         self.scores = None
+        self.idx_pre_chunk = 0
         self.max_time_out = False
         self.decibel = []
-        self.data_buf = None
-        self.data_buf_all = None
+        self.data_buf_size = 0
+        self.data_buf_all_size = 0
         self.waveform = None
         self.ResetDetection()
 
     def AllResetDetection(self):
         self.is_final = False
         self.data_buf_start_frame = 0
         self.frm_cnt = 0
@@ -246,18 +256,19 @@
 
         self.output_data_buf = []
         self.output_data_buf_offset = 0
         self.frame_probs = []
         self.max_end_sil_frame_cnt_thresh = self.vad_opts.max_end_silence_time - self.vad_opts.speech_to_sil_time_thres
         self.speech_noise_thres = self.vad_opts.speech_noise_thres
         self.scores = None
+        self.idx_pre_chunk = 0
         self.max_time_out = False
         self.decibel = []
-        self.data_buf = None
-        self.data_buf_all = None
+        self.data_buf_size = 0
+        self.data_buf_all_size = 0
         self.waveform = None
         self.ResetDetection()
 
     def ResetDetection(self):
         self.continous_silence_frame_count = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
@@ -267,51 +278,48 @@
         self.windows_detector.Reset()
         self.sil_frame = 0
         self.frame_probs = []
 
     def ComputeDecibel(self) -> None:
         frame_sample_length = int(self.vad_opts.frame_length_ms * self.vad_opts.sample_rate / 1000)
         frame_shift_length = int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
-        if self.data_buf_all is None:
-            self.data_buf_all = self.waveform[0]  # self.data_buf is pointed to self.waveform[0]
-            self.data_buf = self.data_buf_all
+        if self.data_buf_all_size == 0:
+            self.data_buf_all_size = len(self.waveform[0])
+            self.data_buf_size = self.data_buf_all_size
         else:
-            self.data_buf_all = np.concatenate((self.data_buf_all, self.waveform[0]))
+            self.data_buf_all_size += len(self.waveform[0])
         for offset in range(0, self.waveform.shape[1] - frame_sample_length + 1, frame_shift_length):
             self.decibel.append(
                 10 * math.log10(np.square((self.waveform[0][offset: offset + frame_sample_length])).sum() + \
                                 0.000001))
 
     def ComputeScores(self, scores: np.ndarray) -> None:
         # scores = self.encoder(feats, in_cache)  # return B * T * D
         self.vad_opts.nn_eval_block_size = scores.shape[1]
         self.frm_cnt += scores.shape[1]  # count total frames
-        if self.scores is None:
-            self.scores = scores  # the first calculation
-        else:
-            self.scores = np.concatenate((self.scores, scores), axis=1)
+        self.scores=scores
 
     def PopDataBufTillFrame(self, frame_idx: int) -> None:  # need check again
         while self.data_buf_start_frame < frame_idx:
-            if len(self.data_buf) >= int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):
+            if self.data_buf_size >= int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):
                 self.data_buf_start_frame += 1
-                self.data_buf = self.data_buf_all[self.data_buf_start_frame * int(
-                    self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):]
+                self.data_buf_size = self.data_buf_all_size-self.data_buf_start_frame * int(
+                    self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
 
     def PopDataToOutputBuf(self, start_frm: int, frm_cnt: int, first_frm_is_start_point: bool,
                            last_frm_is_end_point: bool, end_point_is_sent_end: bool) -> None:
         self.PopDataBufTillFrame(start_frm)
         expected_sample_number = int(frm_cnt * self.vad_opts.sample_rate * self.vad_opts.frame_in_ms / 1000)
         if last_frm_is_end_point:
             extra_sample = max(0, int(self.vad_opts.frame_length_ms * self.vad_opts.sample_rate / 1000 - \
                                       self.vad_opts.sample_rate * self.vad_opts.frame_in_ms / 1000))
             expected_sample_number += int(extra_sample)
         if end_point_is_sent_end:
-            expected_sample_number = max(expected_sample_number, len(self.data_buf))
-        if len(self.data_buf) < expected_sample_number:
+            expected_sample_number = max(expected_sample_number, self.data_buf_size)
+        if self.data_buf_size < expected_sample_number:
             print('error in calling pop data_buf\n')
 
         if len(self.output_data_buf) == 0 or first_frm_is_start_point:
             self.output_data_buf.append(E2EVadSpeechBufWithDoa())
             self.output_data_buf[-1].Reset()
             self.output_data_buf[-1].start_ms = start_frm * self.vad_opts.frame_in_ms
             self.output_data_buf[-1].end_ms = self.output_data_buf[-1].start_ms
@@ -321,18 +329,18 @@
             print('warning\n')
         out_pos = len(cur_seg.buffer)  # cur_seg.buff现在没做任何操作
         data_to_pop = 0
         if end_point_is_sent_end:
             data_to_pop = expected_sample_number
         else:
             data_to_pop = int(frm_cnt * self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
-        if data_to_pop > len(self.data_buf):
-            print('VAD data_to_pop is bigger than self.data_buf.size()!!!\n')
-            data_to_pop = len(self.data_buf)
-            expected_sample_number = len(self.data_buf)
+        if data_to_pop > self.data_buf_size:
+            print('VAD data_to_pop is bigger than self.data_buf_size!!!\n')
+            data_to_pop = self.data_buf_size
+            expected_sample_number = self.data_buf_size
 
         cur_seg.doa = 0
         for sample_cpy_out in range(0, data_to_pop):
             # cur_seg.buffer[out_pos ++] = data_buf_.back();
             out_pos += 1
         for sample_cpy_out in range(data_to_pop, expected_sample_number):
             # cur_seg.buffer[out_pos++] = data_buf_.back()
@@ -407,15 +415,15 @@
             return frame_state
 
         sum_score = 0.0
         noise_prob = 0.0
         assert len(self.sil_pdf_ids) == self.vad_opts.silence_pdf_num
         if len(self.sil_pdf_ids) > 0:
             assert len(self.scores) == 1  # 只支持batch_size = 1的测试
-            sil_pdf_scores = [self.scores[0][t][sil_pdf_id] for sil_pdf_id in self.sil_pdf_ids]
+            sil_pdf_scores = [self.scores[0][t - self.idx_pre_chunk][sil_pdf_id] for sil_pdf_id in self.sil_pdf_ids]
             sum_score = sum(sil_pdf_scores)
             noise_prob = math.log(sum_score) * self.vad_opts.speech_2_noise_ratio
             total_score = 1.0
             sum_score = total_score - sum_score
         speech_prob = math.log(sum_score)
         if self.vad_opts.output_frame_probs:
             frame_prob = E2EVadFrameProb()
@@ -489,15 +497,15 @@
     def DetectCommonFrames(self) -> int:
         if self.vad_state_machine == VadStateMachine.kVadInStateEndPointDetected:
             return 0
         for i in range(self.vad_opts.nn_eval_block_size - 1, -1, -1):
             frame_state = FrameState.kFrameStateInvalid
             frame_state = self.GetFrameState(self.frm_cnt - 1 - i)
             self.DetectOneFrame(frame_state, self.frm_cnt - 1 - i, False)
-
+        self.idx_pre_chunk += self.scores.shape[1]
         return 0
 
     def DetectLastFrames(self) -> int:
         if self.vad_state_machine == VadStateMachine.kVadInStateEndPointDetected:
             return 0
         for i in range(self.vad_opts.nn_eval_block_size - 1, -1, -1):
             frame_state = FrameState.kFrameStateInvalid
```

### Comparing `funasr_onnx-0.0.6/funasr_onnx/utils/frontend.py` & `funasr_onnx-0.0.7/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.6/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.0.7/funasr_onnx/utils/postprocess_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright (c) Alibaba, Inc. and its affiliates.
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import string
 import logging
 from typing import Any, List, Union
 
 
 def isChinese(ch: str):
```

### Comparing `funasr_onnx-0.0.6/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.0.7/funasr_onnx/utils/timestamp_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
 import numpy as np
 
 
 def time_stamp_lfr6_onnx(us_cif_peak, char_list, begin_time=0.0, total_offset=-1.5):
     if not len(char_list):
         return []
     START_END_THRESHOLD = 5
```

### Comparing `funasr_onnx-0.0.6/funasr_onnx/utils/utils.py` & `funasr_onnx-0.0.7/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.6/funasr_onnx/vad_bin.py` & `funasr_onnx-0.0.7/funasr_onnx/vad_bin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os.path
 from pathlib import Path
 from typing import List, Union, Tuple
 
 import copy
 import librosa
```

### Comparing `funasr_onnx-0.0.6/setup.py` & `funasr_onnx-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.6'
+VERSION_NUM = '0.0.7'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
```

