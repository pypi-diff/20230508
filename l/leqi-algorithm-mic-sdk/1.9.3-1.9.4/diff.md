# Comparing `tmp/leqi-algorithm-mic-sdk-1.9.3.tar.gz` & `tmp/leqi-algorithm-mic-sdk-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\leqi-algorithm-mic-sdk-1.9.3.tar", last modified: Fri Aug 13 06:53:39 2021, max compression
+gzip compressed data, was "dist\leqi-algorithm-mic-sdk-1.9.4.tar", last modified: Fri Aug 13 07:26:40 2021, max compression
```

## Comparing `leqi-algorithm-mic-sdk-1.9.3.tar` & `leqi-algorithm-mic-sdk-1.9.4.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxrwx   0        0        0        0 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/
-drwxrwxrwx   0        0        0        0 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/
-drwxrwxrwx   0        0        0        0 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/
--rw-rw-rw-   0        0        0      919 2021-02-03 11:31:01.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/fluorescent_pen_recognition.py
--rw-rw-rw-   0        0        0      870 2021-06-22 02:46:44.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/music_score_recognition.py
--rw-rw-rw-   0        0        0      886 2021-05-10 03:03:59.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/ocr_rec.py
--rw-rw-rw-   0        0        0     1597 2021-06-07 07:27:13.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/paper_rotation.py
--rw-rw-rw-   0        0        0     1175 2021-08-12 07:31:11.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/photo_to_cartoon.py
--rw-rw-rw-   0        0        0      900 2021-02-03 11:30:04.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/region_marquee.py
--rw-rw-rw-   0        0        0     1235 2021-06-22 02:47:57.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/skin_recognition.py
--rw-rw-rw-   0        0        0      884 2021-03-02 09:40:51.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/speech_recognition_chinese.py
--rw-rw-rw-   0        0        0      861 2021-04-20 02:11:34.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/speech_recognition_english.py
--rw-rw-rw-   0        0        0      794 2021-07-02 06:53:14.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/speech_synthesis.py
--rw-rw-rw-   0        0        0      930 2021-01-07 09:37:51.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/topic.py
--rw-rw-rw-   0        0        0      937 2021-08-04 05:19:05.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/topic_loc.py
--rw-rw-rw-   0        0        0      859 2021-01-07 07:21:00.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/trace_elimination.py
--rw-rw-rw-   0        0        0      844 2021-05-24 03:08:50.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/watermark_removal.py
--rw-rw-rw-   0        0        0      325 2021-08-04 05:16:53.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/__init__.py
--rw-rw-rw-   0        0        0     1471 2021-05-10 05:03:35.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/auth.py
--rw-rw-rw-   0        0        0     8361 2021-08-10 07:03:31.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/base.py
--rw-rw-rw-   0        0        0     1155 2020-12-29 00:42:53.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/error.py
--rw-rw-rw-   0        0        0     3138 2020-12-29 00:38:00.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/response.py
--rw-rw-rw-   0        0        0     2879 2021-02-22 06:30:42.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/tools.py
-drwxrwxrwx   0        0        0        0 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws/
--rw-rw-rw-   0        0        0     2582 2021-06-01 09:32:46.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws/speech_recognition_chinese.py
--rw-rw-rw-   0        0        0     2623 2021-06-01 09:32:46.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws/speech_recognition_english.py
--rw-rw-rw-   0        0        0       72 2021-02-19 07:16:59.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws/__init__.py
--rw-rw-rw-   0        0        0     1911 2021-02-18 07:09:24.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws_base.py
--rw-rw-rw-   0        0        0      779 2021-08-13 06:19:59.000000 leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/
--rw-rw-rw-   0        0        0        1 2021-08-13 06:53:38.000000 leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     8079 2021-08-13 06:53:38.000000 leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       26 2021-08-13 06:53:38.000000 leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1317 2021-08-13 06:53:38.000000 leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       18 2021-08-13 06:53:38.000000 leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8079 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/setup.cfg
--rw-rw-rw-   0        0        0      903 2021-08-13 06:51:34.000000 leqi-algorithm-mic-sdk-1.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-13 06:53:39.000000 leqi-algorithm-mic-sdk-1.9.3/test/
--rw-rw-rw-   0        0        0     1436 2021-08-11 08:21:42.000000 leqi-algorithm-mic-sdk-1.9.3/test/test2.py
+drwxrwxrwx   0        0        0        0 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/
+drwxrwxrwx   0        0        0        0 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/
+drwxrwxrwx   0        0        0        0 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/
+-rw-rw-rw-   0        0        0      919 2021-02-03 11:31:01.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/fluorescent_pen_recognition.py
+-rw-rw-rw-   0        0        0      870 2021-06-22 02:46:44.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/music_score_recognition.py
+-rw-rw-rw-   0        0        0      886 2021-05-10 03:03:59.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/ocr_rec.py
+-rw-rw-rw-   0        0        0     1597 2021-06-07 07:27:13.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/paper_rotation.py
+-rw-rw-rw-   0        0        0     1175 2021-08-12 07:31:11.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/photo_to_cartoon.py
+-rw-rw-rw-   0        0        0      900 2021-02-03 11:30:04.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/region_marquee.py
+-rw-rw-rw-   0        0        0     1235 2021-06-22 02:47:57.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/skin_recognition.py
+-rw-rw-rw-   0        0        0      884 2021-03-02 09:40:51.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/speech_recognition_chinese.py
+-rw-rw-rw-   0        0        0      861 2021-04-20 02:11:34.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/speech_recognition_english.py
+-rw-rw-rw-   0        0        0      794 2021-07-02 06:53:14.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/speech_synthesis.py
+-rw-rw-rw-   0        0        0      930 2021-01-07 09:37:51.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/topic.py
+-rw-rw-rw-   0        0        0      937 2021-08-04 05:19:05.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/topic_loc.py
+-rw-rw-rw-   0        0        0      859 2021-01-07 07:21:00.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/trace_elimination.py
+-rw-rw-rw-   0        0        0      844 2021-05-24 03:08:50.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/watermark_removal.py
+-rw-rw-rw-   0        0        0      325 2021-08-04 05:16:53.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1471 2021-05-10 05:03:35.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/auth.py
+-rw-rw-rw-   0        0        0     8361 2021-08-10 07:03:31.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/base.py
+-rw-rw-rw-   0        0        0     1155 2020-12-29 00:42:53.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/error.py
+-rw-rw-rw-   0        0        0     3138 2020-12-29 00:38:00.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/response.py
+-rw-rw-rw-   0        0        0     2879 2021-02-22 06:30:42.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/tools.py
+drwxrwxrwx   0        0        0        0 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws/
+-rw-rw-rw-   0        0        0     2582 2021-06-01 09:32:46.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws/speech_recognition_chinese.py
+-rw-rw-rw-   0        0        0     2623 2021-06-01 09:32:46.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws/speech_recognition_english.py
+-rw-rw-rw-   0        0        0       72 2021-02-19 07:16:59.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws/__init__.py
+-rw-rw-rw-   0        0        0     1911 2021-02-18 07:09:24.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws_base.py
+-rw-rw-rw-   0        0        0      755 2021-08-13 07:21:43.000000 leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     8047 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1352 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       18 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2021-08-13 06:50:50.000000 leqi-algorithm-mic-sdk-1.9.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      143 2021-08-13 07:26:36.000000 leqi-algorithm-mic-sdk-1.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8047 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6620 2021-08-13 07:22:17.000000 leqi-algorithm-mic-sdk-1.9.4/README.rst
+-rw-rw-rw-   0        0        0       42 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      904 2021-08-13 07:18:50.000000 leqi-algorithm-mic-sdk-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-13 07:26:40.000000 leqi-algorithm-mic-sdk-1.9.4/test/
+-rw-rw-rw-   0        0        0     1436 2021-08-11 08:21:42.000000 leqi-algorithm-mic-sdk-1.9.4/test/test2.py
```

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/fluorescent_pen_recognition.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/fluorescent_pen_recognition.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/music_score_recognition.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/music_score_recognition.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/ocr_rec.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/ocr_rec.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/paper_rotation.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/paper_rotation.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/photo_to_cartoon.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/photo_to_cartoon.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/region_marquee.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/region_marquee.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/skin_recognition.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/skin_recognition.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/speech_recognition_chinese.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/speech_recognition_chinese.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/speech_recognition_english.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/speech_recognition_english.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/speech_synthesis.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/speech_synthesis.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/topic.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/topic.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/topic_loc.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/topic_loc.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/trace_elimination.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/trace_elimination.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/algorithms/watermark_removal.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/algorithms/watermark_removal.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/auth.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/base.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/base.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/error.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/error.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/response.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/response.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/tools.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/tools.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws/speech_recognition_chinese.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws/speech_recognition_chinese.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws/speech_recognition_english.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws/speech_recognition_english.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/ws_base.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/ws_base.py`

 * *Files identical despite different names*

### Comparing `leqi-algorithm-mic-sdk-1.9.3/algorithm_mic_sdk/__init__.py` & `leqi-algorithm-mic-sdk-1.9.4/algorithm_mic_sdk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 安装
-pip install git+https://github.com/panyunsuo/algorithm_sdk
+pip install leqi-algorithm-mic-sdk
 
 算法模块
 algorithm_mic_sdk.error 异常模块
 algorithm_mic_sdk.error.AbnormalAlgorithmPlatform API网关相关异常
 algorithm_mic_sdk.auth.AuthInfo 账号信息,需要初始化后作为参数给其他需要验证的模块调用
 
 algorithm_mic_sdk.base 基础类库模块
 algorithm_mic_sdk.base.Base 主要是对图片算法的处理,可以上传/下载图片, 获取算法结果等,详细使用见模块说明
 algorithm_mic_sdk.base.AlgoBase 对Base模块的封装,主要是有同步/异步发布算法的功能
 
 algorithm_mic_sdk.algorithms.topic.Topic 错题本算法
 algorithm_mic_sdk.algorithms.trace_elimination.TraceElimination 手写痕迹消除算法
 """
-__version__ = '1.9.3'
+__version__ = '1.9.4'
```

### Comparing `leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/PKG-INFO` & `leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: leqi-algorithm-mic-sdk
-Version: 1.9.3
+Version: 1.9.4
 Summary: LeQi
 Home-page: https://www.yuque.com/fenfendeyouzhiqingnian/algorithm
 Author: panso
 Author-email: panrs@venpoo.com
 License: MIT
 Description: # 安装  
-        `pip install git+https://github.com/panyunsuo/AlgorithmicMicroserviceSDK.git`
+        `pip install leqi-algorithm-mic-sdk`
         
         # 算法模块
         
         * `algorithm_mic_sdk.error` 异常模块  
         * * `algorithm_mic_sdk.error.AbnormalAlgorithmPlatform` API网关相关异常  
         * `algorithm_mic_sdk.auth.AuthInfo` 账号信息,需要初始化后作为参数给其他需要验证的模块调用  
         * `algorithm_mic_sdk.base` 基础类库模块
@@ -32,15 +32,16 @@
         * `algorithm_mic_sdk.algorithms.speech_synthesis.SpeechSynthesis` 语音合成算法
         * `algorithm_mic_sdk.algorithms.topic_loc.TopicLoc` 错题本题干检测定位算法
         
         * `algorithm_mic_sdk.ws.speech_recognition_chinese.SpeechRecognitionChinese` 中文识别算法(socket 版本)
         * `algorithm_mic_sdk.ws.speech_recognition_english.SpeechRecognitionEnglish` 英文识别算法(socket 版本)
         
         
-        # 使用示例1 (http api): 
+        # 使用示例1 (http api):
+        
         > 错题本算法
         
         ```python
         import time
         
         from algorithm_mic_sdk import error
         from algorithm_mic_sdk.algorithms.topic import Topic
```

### Comparing `leqi-algorithm-mic-sdk-1.9.3/leqi_algorithm_mic_sdk.egg-info/SOURCES.txt` & `leqi-algorithm-mic-sdk-1.9.4/leqi_algorithm_mic_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+LICENSE.txt
+MANIFEST.in
+README.rst
 setup.py
 algorithm_mic_sdk/__init__.py
 algorithm_mic_sdk/auth.py
 algorithm_mic_sdk/base.py
 algorithm_mic_sdk/error.py
 algorithm_mic_sdk/response.py
 algorithm_mic_sdk/tools.py
```

### Comparing `leqi-algorithm-mic-sdk-1.9.3/PKG-INFO` & `leqi-algorithm-mic-sdk-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: leqi-algorithm-mic-sdk
-Version: 1.9.3
+Version: 1.9.4
 Summary: LeQi
 Home-page: https://www.yuque.com/fenfendeyouzhiqingnian/algorithm
 Author: panso
 Author-email: panrs@venpoo.com
 License: MIT
 Description: # 安装  
-        `pip install git+https://github.com/panyunsuo/AlgorithmicMicroserviceSDK.git`
+        `pip install leqi-algorithm-mic-sdk`
         
         # 算法模块
         
         * `algorithm_mic_sdk.error` 异常模块  
         * * `algorithm_mic_sdk.error.AbnormalAlgorithmPlatform` API网关相关异常  
         * `algorithm_mic_sdk.auth.AuthInfo` 账号信息,需要初始化后作为参数给其他需要验证的模块调用  
         * `algorithm_mic_sdk.base` 基础类库模块
@@ -32,15 +32,16 @@
         * `algorithm_mic_sdk.algorithms.speech_synthesis.SpeechSynthesis` 语音合成算法
         * `algorithm_mic_sdk.algorithms.topic_loc.TopicLoc` 错题本题干检测定位算法
         
         * `algorithm_mic_sdk.ws.speech_recognition_chinese.SpeechRecognitionChinese` 中文识别算法(socket 版本)
         * `algorithm_mic_sdk.ws.speech_recognition_english.SpeechRecognitionEnglish` 英文识别算法(socket 版本)
         
         
-        # 使用示例1 (http api): 
+        # 使用示例1 (http api):
+        
         > 错题本算法
         
         ```python
         import time
         
         from algorithm_mic_sdk import error
         from algorithm_mic_sdk.algorithms.topic import Topic
```

### Comparing `leqi-algorithm-mic-sdk-1.9.3/setup.py` & `leqi-algorithm-mic-sdk-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ------------
 @Model Name:   安装命令:python setup.py install
 """
 from setuptools import find_packages, setup
 
 PACKAGE = 'algorithm_mic_sdk'
 
-with open("README.MD", "r", encoding='UTF-8') as fh:
+with open("README.rst", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 VERSION = __import__(PACKAGE).__version__
 setup(
     name="leqi-algorithm-mic-sdk",
     version=VERSION,
     description="LeQi",
```

### Comparing `leqi-algorithm-mic-sdk-1.9.3/test/test2.py` & `leqi-algorithm-mic-sdk-1.9.4/test/test2.py`

 * *Files identical despite different names*

