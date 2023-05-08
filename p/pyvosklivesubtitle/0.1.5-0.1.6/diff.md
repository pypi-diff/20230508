# Comparing `tmp/pyvosklivesubtitle-0.1.5.tar.gz` & `tmp/pyvosklivesubtitle-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvosklivesubtitle-0.1.5.tar", last modified: Thu Apr 27 13:24:16 2023, max compression
+gzip compressed data, was "pyvosklivesubtitle-0.1.6.tar", last modified: Mon May  8 21:18:06 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.5.tar` & `pyvosklivesubtitle-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:24:16.932245 pyvosklivesubtitle-0.1.5/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1617 2023-04-27 13:24:16.932995 pyvosklivesubtitle-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 13:24:16.906771 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0   143370 2023-04-27 12:27:06.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:24:16.929998 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1617 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-27 13:24:16.000000 pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-27 13:24:16.936740 pyvosklivesubtitle-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1610 2023-04-27 12:28:32.000000 pyvosklivesubtitle-0.1.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 21:18:06.420709 pyvosklivesubtitle-0.1.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.6/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1588 2023-05-08 21:18:06.421023 pyvosklivesubtitle-0.1.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 21:18:06.408891 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle/
+-rwxrwxrwx   0 root         (0) root         (0)   146492 2023-05-08 21:17:21.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 21:18:06.419909 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1588 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       63 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      139 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       19 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-08 21:18:06.422471 pyvosklivesubtitle-0.1.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1721 2023-05-08 18:46:09.000000 pyvosklivesubtitle-0.1.6/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.5/LICENSE` & `pyvosklivesubtitle-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.5/PKG-INFO` & `pyvosklivesubtitle-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: pyvosklivesubtitle
-Version: 0.1.5
-Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
-Home-page: https://github.com/botbahlul/pyvosklivesubtitle
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 Bot Bahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+Metadata-Version: 2.1
+Name: pyvosklivesubtitle
+Version: 0.1.6
+Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
+Home-page: https://github.com/botbahlul/pyvosklivesubtitle
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 Bot Bahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+
```

### Comparing `pyvosklivesubtitle-0.1.5/README.md` & `pyvosklivesubtitle-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.5/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.6/pyvosklivesubtitle/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     import Queue  # Python 2 import
 
 import tempfile
 from datetime import datetime, timedelta
 import subprocess
 import multiprocessing
 import ctypes
-import ctypes.wintypes
+if sys.platform == "win32":
+    import win32clipboard
 from streamlink import Streamlink
 from streamlink.exceptions import NoPluginError, StreamlinkError, StreamError
 import six
 import pysrt
 import shutil
 import re
 import select
@@ -556,14 +557,16 @@
     def GetPendingChunks(self):
         return _c.vosk_batch_recognizer_get_pending_chunks(self._handle)
 
 #=======================================================================================================================================#
 
 #============================================================== APP PARTS ==============================================================#
 
+VERSION = '0.1.6'
+
 arraylist_models = []
 arraylist_models.append("ca-es");
 arraylist_models.append("zh-cn")
 arraylist_models.append("cs-cz");
 arraylist_models.append("nl-nl");
 arraylist_models.append("en-us")
 arraylist_models.append("eo-eo");
@@ -1177,73 +1180,138 @@
         parser.exit(0)
 
     except Exception as e:
         parser.exit(type(e).__name__ + ": " + str(e))
 
 
 class SentenceTranslator(object):
-    def __init__(self, src, dst, patience=-1):
+    def __init__(self, src, dst, patience=-1, timeout=30, error_messages_callback=None):
         self.src = src
         self.dst = dst
         self.patience = patience
+        self.timeout = timeout
+        self.error_messages_callback = error_messages_callback
 
     def __call__(self, sentence):
-        translated_sentence = []
-        # handle the special case: empty string.
-        if not sentence:
-            return None
+        try:
+            translated_sentence = []
+            # handle the special case: empty string.
+            if not sentence:
+                return None
+            translated_sentence = self.GoogleTranslate(sentence, src=self.src, dst=self.dst, timeout=self.timeout)
+            fail_to_translate = translated_sentence[-1] == '\n'
+            while fail_to_translate and patience:
+                translated_sentence = self.GoogleTranslate(translated_sentence, src=self.src, dst=self.dst, timeout=self.timeout).text
+                if translated_sentence[-1] == '\n':
+                    if patience == -1:
+                        continue
+                    patience -= 1
+                else:
+                    fail_to_translate = False
 
-        translated_sentence = GoogleTranslate(sentence, src=self.src, dst=self.dst)
+            return translated_sentence
 
-        fail_to_translate = translated_sentence[-1] == '\n'
-        while fail_to_translate and patience:
-            translated_sentence = GoogleTranslate(translated_sentence, src=self.src, dst=self.dst).text
-            if translated_sentence[-1] == '\n':
-                if patience == -1:
-                    continue
-                patience -= 1
+        except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
+            return
+
+        except Exception as e:
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
+            return
+
+    def GoogleTranslate(self, text, src, dst, timeout=30):
+        url = 'https://translate.googleapis.com/translate_a/'
+        params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
+        headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
+
+        try:
+            response = requests.get(url+params, headers=headers, timeout=self.timeout)
+            if response.status_code == 200:
+                response_json = response.json()[0]
+                length = len(response_json)
+                translation = ""
+                for i in range(length):
+                    translation = translation + response_json[i][0]
+                return translation
+            return
+
+        except requests.exceptions.ConnectionError:
+            with httpx.Client() as client:
+                response = client.get(url+params, headers=headers, timeout=self.timeout)
+                if response.status_code == 200:
+                    response_json = response.json()[0]
+                    length = len(response_json)
+                    translation = ""
+                    for i in range(length):
+                        translation = translation + response_json[i][0]
+                    return translation
+                return
+
+        except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
+            return
+
+        except Exception as e:
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
             else:
-                fail_to_translate = False
-        return translated_sentence
+                print(e)
+            return
 
-'''
-def GoogleTranslate(text, src, dst):
+
+def GoogleTranslate(text, src, dst, timeout=30, error_messages_callback=None):
     url = 'https://translate.googleapis.com/translate_a/'
     params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
-    with httpx.Client(http2=True) as client:
-        client.headers.update({'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',})
-        response = client.get(url+params)
-        #print("response.status_code = {}".format(response.status_code))
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
+
+    try:
+        response = requests.get(url+params, headers=headers, timeout=timeout)
         if response.status_code == 200:
             response_json = response.json()[0]
-            #print("response_json = {}".format(response_json))
-            if response_json!= None:
+            length = len(response_json)
+            translation = ""
+            for i in range(length):
+                translation = translation + response_json[i][0]
+            return translation
+        return
+
+    except requests.exceptions.ConnectionError:
+        with httpx.Client() as client:
+            response = client.get(url+params, headers=headers, timeout=timeout)
+            if response.status_code == 200:
+                response_json = response.json()[0]
                 length = len(response_json)
-                #print("length = {}".format(length))
                 translation = ""
                 for i in range(length):
-                    #print("{} {}".format(i, response_json[i][0]))
                     translation = translation + response_json[i][0]
                 return translation
+            return
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
         return
-'''
 
-def GoogleTranslate(text, src, dst):
-    url = 'https://translate.googleapis.com/translate_a/'
-    params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
-    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
-    response = requests.get(url+params, headers=headers)
-    if response.status_code == 200:
-        response_json = response.json()[0]
-        length = len(response_json)
-        translation = ""
-        for i in range(length):
-            translation = translation + response_json[i][0]
-        return translation
-    return
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
 
 
 def worker_timed_translate(src, dst):
     global main_window, recognizing
 
     while (recognizing==True):
         if not recognizing:
@@ -1252,15 +1320,15 @@
         partial_result_filepath = os.path.join(tempfile.gettempdir(), partial_result_filename)
         if os.path.isfile(partial_result_filepath):
             partial_result_file = open(partial_result_filepath, "r")
             partial_result = partial_result_file.read()
 
             n_words = len(partial_result.split())
             if partial_result and n_words % 3 == 0:
-                translated_text = GoogleTranslate(partial_result, src, dst)
+                translated_text = GoogleTranslate(partial_result, src, dst, error_messages_callback=show_error_messages)
                 main_window.write_event_value('-EVENT-VOICE-TRANSLATED-', translated_text)
 
 
 def stop_thread(thread):
     global main_window
 
     exc = ctypes.py_object(SystemExit)
@@ -1485,40 +1553,67 @@
     thread = Thread(target=run_ffmpeg)
     if recognizing: thread.start()
 
     # Return the thread object so that the caller can join it if needed
     return thread
 
 
-def stop_ffmpeg_windows():
+def stop_ffmpeg_windows(error_messages_callback=None):
+    try:
+        tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
+        ffmpeg_pid = None
+        for line in tasklist_output.split('\n'):
+            if "ffmpeg" in line:
+                ffmpeg_pid = line.split()[1]
+                break
+        if ffmpeg_pid:
+            devnull = open(os.devnull, 'w')
+            subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
 
-    tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
-    ffmpeg_pid = None
-    for line in tasklist_output.split('\n'):
-        if "ffmpeg" in line:
-            ffmpeg_pid = line.split()[1]
-            break
-    if ffmpeg_pid:
-        devnull = open(os.devnull, 'w')
-        #subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=devnull, stderr=devnull, creationflags=subprocess.CREATE_NO_WINDOW)
-        subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
 
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
 
-def stop_ffmpeg_linux():
 
+def stop_ffmpeg_linux(error_messages_callback=None):
     process_name = 'ffmpeg'
     try:
         output = subprocess.check_output(['ps', '-ef'])
         pid = [line.split()[1] for line in output.decode('utf-8').split('\n') if process_name in line][0]
         subprocess.call(['kill', '-9', str(pid)])
         #print(f"{process_name} has been killed")
     except IndexError:
         #print(f"{process_name} is not running")
         pass
 
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
+
+
 def stop_record_streaming_windows():
     global main_window, thread_record_streaming
 
     if thread_record_streaming and thread_record_streaming.is_alive():
         # Use ctypes to call the TerminateThread() function from the Windows API
         # This forcibly terminates the thread, which can be unsafe in some cases
         kernel32 = ctypes.windll.kernel32
@@ -1659,14 +1754,15 @@
     except Exception as e:
         not_transcribing = True
         msg = [e, n_channels, str(n_channels)]
         sg.Popup(msg, title="Info", line_width=50)
         main_window.write_event_value('-EXCEPTION-', e)
 
     if not_transcribing: return
+
     if sys.platform == "win32":
         subprocess.check_output(command, stdin=open(os.devnull), creationflags=subprocess.CREATE_NO_WINDOW)
     else:
         subprocess.check_output(command, stdin=open(os.devnull))
 
     return temp.name, rate
 
@@ -1694,17 +1790,16 @@
 
 def vosk_transcribe(src, dst, video_filepath, subtitle_format):
     global all_transcribe_threads, thread_vosk_transcribe, not_transcribing, main_window, regions, transcriptions, \
         created_regions, created_subtitles, translated_transcriptions, saved_src_subtitle_filepath, saved_dst_subtitle_filepath, \
         subtitle_filepath, subtitle_file_extension
 
     if not os.path.isfile(video_filepath):
-        FONT_TYPE = "Helvetica"
-        FONT_SIZE = 9
-        sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+        FONT = ("Helvetica", 10)
+        sg.set_options(font=FONT)
         sg.Popup("{} is not exist!".format(video_filepath), title="Info", line_width=50)
         return
 
     if not_transcribing: return
 
     pool = multiprocessing.Pool(10, initializer=NoConsoleProcess)
     wav_filepath = None
@@ -1858,15 +1953,15 @@
             append_flag = True
             main_window.write_event_value('-EVENT-TRANSCRIBE-SEND-MESSAGES-', (window_key, msg, append_flag))
 
             info = 'Translating {} subtitles from {} to {}'.format(file_display_name, src, dst)
             total = 100
             main_window.write_event_value('-EVENT-TRANSCRIBE-UPDATE-PROGRESS-BAR-', (info, "0%", 0))
 
-            transcript_translator = SentenceTranslator(src=src, dst=dst)
+            transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
             translated_transcriptions = []
 
             for i, translated_transcription in enumerate(pool.imap(transcript_translator, created_subtitles)):
 
                 if not_transcribing:
                     pool.close()
                     pool.join()
@@ -2081,17 +2176,14 @@
     transcriptions_filename = "transcriptions"
     transcriptions_filepath = os.path.join(tempfile.gettempdir(), transcriptions_filename)
     regions = None
     transcriptions = None
 
     transcribe_is_done_filename = "transcribe_is_done"
     transcribe_is_done_filepath = os.path.join(tempfile.gettempdir(), transcribe_is_done_filename)
-    #transcribe_is_done_file = open(transcribe_is_done_filepath, "r")
-    #transcribe_is_done = transcribe_is_done_file.read()
-    #transcribe_is_done_file.close()
 
     while True:
         if os.path.isfile(transcribe_is_done_filepath):
             if os.path.isfile(regions_filepath):
                 regions_file = open(regions_filepath, "r")
                 regions = tuple(json.load(regions_file))
                 regions_file.close()
@@ -2114,17 +2206,16 @@
                 created_regions = []
                 created_subtitles = []
                 for entry in timed_subtitles:
                     created_regions.append(entry[0])
                     created_subtitles.append(entry[1])
 
             else:
-                FONT_TYPE = "Helvetica"
-                FONT_SIZE = 9
-                sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+                FONT = ("Helvetica", 10)
+                sg.set_options(font=FONT)
                 sg.Popup("Subtitle format you typed is not supported, subtitle file will be saved in TXT format.", title="Info", line_width=50)
                 subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format="txt")
                 shutil.copy(tmp_src_txt_transcription_filepath, subtitle_filepath)
 
             # SAVING TRANSLATED SUBTITLE FILE WITH FILENAME BASED ON SUBTITLE FILENAME DECLARED IN COMMAND LINE ARGUMENTS
             if not is_same_language(src, dst):
 
@@ -2201,99 +2292,81 @@
     f = tf.Font(family=Font , size = Size)
     length = f.measure(Text)
     #print(length)
     return length
 
 
 def popup_yes_no(text, title=None):
+    FONT = ("Helvetica", 10)
+    sg.set_options(font=FONT)
+
     layout = [
-        [sg.Text(text)],
+        [sg.Text(text, size=(50,1))],
         [sg.Push(), sg.Button('Yes'), sg.Button('No')],
     ]
     return sg.Window(title if title else text, layout, resizable=True).read(close=True)
 
 
 def make_progress_bar_window(info, total):
 
-    FONT_TYPE = "Helvetica"
-    FONT_SIZE = 9
-    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+    FONT = ("Helvetica", 10)
+    sg.set_options(font=FONT)
 
     layout = [
                 [sg.Text(info, key='-INFO-')],
                 [sg.ProgressBar(total, orientation='h', size=(30, 10), key='-PROGRESS-'), sg.Text(size=(5,1), key='-PERCENTAGE-')]
              ]
 
     progress_bar_window = sg.Window("Progress", layout, no_titlebar=False, finalize=True)
     progress_bar_window['-PROGRESS-'].update(max=total)
     move_center(progress_bar_window)
 
     return progress_bar_window
 
 
+def show_error_messages(messages):
+    global main_window, not_transcribing
+    not_transcribing = True
+    main_window.write_event_value("-EXCEPTION-", messages)
+
+
 def make_transcribe_window(info, total):
     global not_transcribing
 
-    FONT_TYPE = "Helvetica"
-    FONT_SIZE = 9
-    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+    FONT = ("Helvetica", 10)
+    sg.set_options(font=FONT)
 
     layout = [
                 [sg.Text("Progress info", key='-INFO-')],
                 [
                     sg.ProgressBar(100, orientation='h', size=(50, 10), key='-PROGRESS-'),
                     sg.Text("0%", size=(5,1), key='-PERCENTAGE-')
                 ],
                 [sg.Multiline(size=(60, 10), expand_x=True, expand_y=True, key='-OUTPUT-MESSAGES-')],
-                [sg.Button('Cancel', font=("Helvetica", 9), expand_x=True, expand_y=True, key='-CANCEL-')]
+                [sg.Button('Cancel', font=FONT, expand_x=True, expand_y=True, key='-CANCEL-')]
              ]
 
-    transcribe_window = sg.Window('Transcribe', layout, font=FONT_TYPE, resizable=True, keep_on_top=True, finalize=True)
+    transcribe_window = sg.Window('Transcribe', layout, font=FONT, resizable=True, keep_on_top=True, finalize=True)
     transcribe_window['-PROGRESS-'].update(max=total)
     move_center(transcribe_window)
 
     return transcribe_window
 
 
 def make_overlay_translation_window(translated_text):
     xmax, ymax = sg.Window.get_screen_size()
 
-    '''
-    max_columns = None
-    max_lines = None
-
-    if sys.platform == "win32":
-        SM_CXSCREEN = 0
-        SM_CYSCREEN = 1
-        width = ctypes.windll.user32.GetSystemMetrics(SM_CXSCREEN)
-        height = ctypes.windll.user32.GetSystemMetrics(SM_CYSCREEN)
-
-        max_columns = int(width/8.5)
-        max_lines = int(height/18)
-
-    else:
-        try:
-            output = subprocess.check_output(['xrandr'], check=True)
-            primary_line = [line for line in output.decode().splitlines() if ' connected primary' in line][0]
-            primary_size = primary_line.split()[3].replace("+"," ").split()[0]
-            max_columns, max_lines = int(primary_size.split('x')[0]) // 8, int(primary_size.split('x')[1]) // 18
-
-        except subprocess.CalledProcessError:
-            max_columns = int(os.environ.get('COLUMNS', 80))
-            max_lines = int(os.environ.get('LINES', 24))
-    '''
-
     max_columns = int(os.environ.get('COLUMNS', 80))
     max_lines = int(os.environ.get('LINES', 24))
 
     columns = max_columns
     rows = max_lines
 
-    FONT_TYPE = 'Helvetica'
-    FONT_SIZE = 16
+    FONT = ("Helvetica", 16)
+    sg.set_options(font=FONT)
 
     if len(translated_text)<=96:
         window_width = int(9.9*(xmax/1280)*len(translated_text) + 60)
         #window_width = font_length(translated_text, FONT_TYPE, FONT_SIZE)
     else:
         window_width=int(960*xmax/1280)
 
@@ -2311,15 +2384,16 @@
         window_y = int(528*ymax/720)
     else:
         window_y = int((528-(nl-1)*28)*ymax/720)
 
     if xmax > 1280: FONT_SIZE = 14
     if xmax <= 1280: FONT_SIZE = 16
 
-    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+    FONT_TYPE = "Helvetica"
+    sg.set_options(font=FONT)
 
     multiline_width = len(translated_text)
     multiline_height = nl
 
     TRANSPARENT_BLACK='#add123'
 
     if not (sys.platform == "win32"):
@@ -2360,112 +2434,106 @@
 
 
 def move_center(window):
     screen_width, screen_height = window.get_screen_dimensions()
     win_width, win_height = window.size
     x, y = (screen_width-win_width)//2, (screen_height-win_height)//2 - 30
     window.move(x, y)
+    window.refresh()
 
 
 def get_clipboard_text():
-    return subprocess.check_output(['xclip', '-selection', 'clipboard', '-out']).decode()
+    try:
+        clipboard_data = subprocess.check_output(['xclip', '-selection', 'clipboard', '-o'], universal_newlines=True)
+        return clipboard_data.strip()
+    except subprocess.CalledProcessError:
+        # Handle the case when clipboard is empty or unsupported
+        return None
 
 
 def set_clipboard_text(text):
-    subprocess.run(['xclip', '-selection', 'clipboard'], input=text.encode())
+    try:
+        subprocess.run(['xclip', '-selection', 'clipboard'], input=text.encode())
+    except subprocess.CalledProcessError as e:
+        pass
 
 
 #------------------------------------------------------------ MAIN PROGRAM ------------------------------------------------------------#
 
 
 def main():
     global main_window, thread_recognize, thread_timed_translate, thread_record_streaming, text, recognizing, \
         Device, SampleRate, wav_filepath, tmp_recorded_streaming_filepath, regions, transcriptions, \
         created_regions, created_subtitles, translated_transcriptions, start_button_click_time, ffmpeg_start_run_time, \
         get_tmp_recorded_streaming_filepath_time, first_streaming_duration_recorded, is_valid_url_streaming, \
         transcribe_window, thread_vosk_transcribe, all_transcribe_threads, not_transcribing, \
         saved_src_subtitle_filepath, saved_dst_subtitle_filepath, subtitle_filepath, subtitle_file_extension
 
-    if sys.platform == "win32":
-        user32 = ctypes.windll.user32
-        kernel32 = ctypes.windll.kernel32
-        kernel32.GlobalLock.argtypes = [ctypes.wintypes.HGLOBAL]
-        kernel32.GlobalLock.restype = ctypes.wintypes.LPVOID
-        kernel32.GlobalSize.argtypes = [ctypes.wintypes.HGLOBAL]
-        kernel32.GlobalSize.restype = ctypes.c_size_t
-        user32.OpenClipboard.argtypes = [ctypes.wintypes.HWND]
-        user32.OpenClipboard.restype = ctypes.wintypes.BOOL
-        user32.CloseClipboard.argtypes = []
-        user32.CloseClipboard.restype = ctypes.wintypes.BOOL
-        user32.GetClipboardData.argtypes = [ctypes.wintypes.UINT]
-        user32.GetClipboardData.restype = ctypes.wintypes.HANDLE
-
 
 #------------------------------------------------------------- GUI PARTS -------------------------------------------------------------#
 
     xmax, ymax = sg.Window.get_screen_size()
     main_window_width = int(0.5*xmax)
     main_window_height = int(0.5*ymax)
     multiline_width = int(0.15*main_window_width)
     multiline_height = int(0.0125*main_window_height)
-    FONT_TYPE = "Helvetica"
-    FONT_SIZE = 9
-    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+    FONT = ("Helvetica", 10)
+    sg.set_options(font=FONT)
 
     layout =  [
                 [sg.Frame('Hints',[
                                     [sg.Text('Click \"Start\" button to start listening and printing subtitles on screen.', expand_x=True, expand_y=True)],
                                     [sg.Text('Paste the streaming URL into URL inputbox then check the \"Record Streaming\" checkbox to record the streaming.', expand_x=True, expand_y=True)],
-                                    #[sg.Text('If you record the streaming, when you save transcriptions, all timestamps will be relative to the \"Start\" button clicked time.', expand_x=True, expand_y=True)],
-                                    #[sg.Text('If you don\'t record the streaming, all timestamps will be based on your system clock.', expand_x=True, expand_y=True)],
-                                ], border_width=2, expand_x=True, expand_y=True)],
+                                  ],
+                                  border_width=2, expand_x=True, expand_y=True)
+                ],
                 [
                     sg.Text('URL', size=(12, 1)),
-                    sg.Input(size=(20, 1), expand_x=True, expand_y=True, key='-URL-', enable_events=True, right_click_menu=['&Edit', ['&Paste',]]),
+                    sg.Input(size=(16, 1), expand_x=True, expand_y=True, key='-URL-', enable_events=True, right_click_menu=['&Edit', ['&Copy','&Paste',]]),
                     sg.Checkbox("Record Streaming", key='-RECORD-STREAMING-', enable_events=True)
                 ],
                 [
                     #sg.Text('', size=(3, 1)),
                     sg.Text('Thread status', size=(12, 1)),
-                    sg.Text('NOT RECORDING', size=(24, 1), background_color='green1', text_color='black', expand_x=True, expand_y=True, key='-RECORD-STREAMING-STATUS-'),
+                    sg.Text('NOT RECORDING', size=(20, 1), background_color='green1', text_color='black', expand_x=True, expand_y=True, key='-RECORD-STREAMING-STATUS-'),
                     sg.Text('Duration recorded', size=(16, 1)),
-                    sg.Text('0:00:00.000000', size=(9, 1), background_color='green1', text_color='black', expand_x=True, expand_y=True, key='-STREAMING-DURATION-RECORDED-'),
-                    sg.Text('', size=(12, 1), expand_x=True, expand_y=True)
+                    sg.Text('0:00:00.000000', size=(14, 1), background_color='green1', text_color='black', expand_x=True, expand_y=True, key='-STREAMING-DURATION-RECORDED-'),
+                    sg.Text('', size=(16, 1), expand_x=True, expand_y=True)
                 ],
                 [sg.Text('', expand_x=True, expand_y=True),
                  sg.Button('SAVE RECORDED STREAMING', size=(31,1), expand_x=True, expand_y=True, key='-EVENT-SAVE-RECORDED-STREAMING-'),
                  sg.Text('', expand_x=True, expand_y=True)],
-                [sg.Text('Audio language', size=(12, 1), expand_x=True, expand_y=True),
-                 sg.Combo(list(map_src_of_language), size=(int(0.2*multiline_width), 1), default_value="English", expand_x=True, expand_y=True, key='-SRC-')],
-                [sg.Multiline(size=(multiline_width, multiline_height), expand_x=True, expand_y=True, key='-ML-SRC-RESULTS-')],
-                [sg.Multiline(size=(multiline_width, 0.5*multiline_height), expand_x=True, expand_y=True, key='-ML-SRC-PARTIAL-RESULTS-')],
+                [sg.Text('Audio language', size=(10, 1), expand_x=True, expand_y=True),
+                 sg.Combo(list(map_src_of_language), size=(12, 1), default_value="English", expand_x=True, expand_y=True, key='-SRC-')],
+                [sg.Multiline(size=(96, 5), expand_x=True, expand_y=True, right_click_menu=['&Edit', ['&Copy','&Paste',]], key='-ML-SRC-RESULTS-')],
+                [sg.Multiline(size=(96, 3), expand_x=True, expand_y=True, right_click_menu=['&Edit', ['&Copy','&Paste',]], key='-ML-SRC-PARTIAL-RESULTS-')],
                 [sg.Text('', expand_x=True, expand_y=True),
                  sg.Button('SAVE TRANSCRIPTION', size=(31,1), expand_x=True, expand_y=True, key='-EVENT-SAVE-SRC-TRANSCRIPTION-'),
                  sg.Text('', expand_x=True, expand_y=True)],
-                [sg.Text('Translation language', size=(12, 1),expand_x=True, expand_y=True),
-                 sg.Combo(list(map_dst_of_language), size=(int(0.2*multiline_width), 1), default_value="Indonesian", expand_x=True, expand_y=True, key='-DST-')],
-                [sg.Multiline(size=(multiline_width, multiline_height), expand_x=True, expand_y=True, key='-ML-DST-RESULTS-')],
-                [sg.Multiline(size=(multiline_width, 0.5*multiline_height), expand_x=True, expand_y=True, key='-ML-DST-PARTIAL-RESULTS-')],
+                [sg.Text('Translation language', size=(10, 1),expand_x=True, expand_y=True),
+                 sg.Combo(list(map_dst_of_language), size=(12, 1), default_value="Indonesian", expand_x=True, expand_y=True, key='-DST-')],
+                [sg.Multiline(size=(96, 5), expand_x=True, expand_y=True, right_click_menu=['&Edit', ['&Copy','&Paste',]], key='-ML-DST-RESULTS-')],
+                [sg.Multiline(size=(96, 3), expand_x=True, expand_y=True, right_click_menu=['&Edit', ['&Copy','&Paste',]], key='-ML-DST-PARTIAL-RESULTS-')],
                 [sg.Text('', expand_x=True, expand_y=True, key='-SPACES3-'),
                  sg.Button('SAVE TRANSLATED TRANSCRIPTION', size=(31,1), expand_x=True, expand_y=True, key='-EVENT-SAVE-DST-TRANSCRIPTION-'),
                  sg.Text('', expand_x=True, expand_y=True, key='-SPACES4-')],
                 [sg.Button('Start', expand_x=True, expand_y=True, button_color=('white', '#283b5b'), key='-START-BUTTON-'),
                  sg.Button('Exit', expand_x=True, expand_y=True)],
             ]
 
 
 #--------------------------------------------------------- NON GUI PARTS -------------------------------------------------------------#
 
     # VOSK LogLevel
     SetLogLevel(-1)
 
     if sys.platform == "win32":
-        stop_ffmpeg_windows()
+        stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
-        stop_ffmpeg_linux()
+        stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     last_selected_src = None
     last_selected_dst = None
 
     src_filename = "src"
     src_filepath = os.path.join(tempfile.gettempdir(), src_filename)
     if os.path.isfile(src_filepath):
@@ -2479,16 +2547,15 @@
         last_selected_dst = dst_file.read()
 
     recognizing = False
     not_transcribing = True
 
     tmp_recorded_streaming_filename = "record.mp4"
     tmp_recorded_streaming_filepath = os.path.join(tempfile.gettempdir(), tmp_recorded_streaming_filename)
-    if os.path.isfile(tmp_recorded_streaming_filepath):
-        os.remove(tmp_recorded_streaming_filepath)
+    if os.path.isfile(tmp_recorded_streaming_filepath): os.remove(tmp_recorded_streaming_filepath)
 
     saved_recorded_streaming_filename = None
 
     partial_result_filename = "partial_result"
     partial_result_filepath = os.path.join(tempfile.gettempdir(), partial_result_filename)
     if os.path.isfile(partial_result_filepath): os.remove(partial_result_filepath)
 
@@ -2581,15 +2648,15 @@
     parser.add_argument("-af", "--audio-filename", type=str, metavar="AUDIO_FILENAME", help="audio file to store recording to", default=None)
     parser.add_argument("-d", "--device", type=int_or_str, help="input device (numeric ID or substring)")
     parser.add_argument("-r", "--samplerate", type=int, help="sampling rate in Hertz for example 8000, 16000, 44100, or 48000", default=16000)
 
     parser.add_argument("-u", "--url", type=str, metavar="URL", help="URL of live streaming if you want to record the streaming")
     parser.add_argument("-vf", "--video-filename", type=str, metavar="VIDEO_FILENAME", help="video file to store recording to", default=None)
 
-    parser.add_argument('-v', '--version', action='version', version='0.1.5')
+    parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args(remaining)
     args = parser.parse_args()
 
     if args.src_language:
         src = args.src_language
         last_selected_src = src
@@ -2633,17 +2700,16 @@
     if args.audio_filename:
         wav_filepath = args.audio_filename
         dump_fn = open(args.audio_filename, "wb")
     else:
         dump_fn = None
 
     if args.subtitle_format not in FORMATTERS.keys():
-        FONT_TYPE = "Helvetica"
-        FONT_SIZE = 9
-        sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+        FONT = ("Helvetica", 10)
+        sg.set_options(font=FONT)
         sg.Popup("Subtitle format is not supported, you can choose it later when you save transcriptions.", title="Info", line_width=50)
 
     subtitle_format = args.subtitle_format
 
     if args.video_filename:
         saved_recorded_streaming_basename, saved_recorded_streaming_extension = os.path.splitext(os.path.basename(args.video_filename))
         saved_recorded_streaming_extension = saved_recorded_streaming_extension[1:]
@@ -2652,37 +2718,39 @@
         else:
             saved_recorded_streaming_filename = args.video_filename
 
 
 #------------------------------------ REMAINING GUI PARTS NEEDED TO LOAD AT LAST BEFORE MAIN LOOP ------------------------------------#
 
 
-    main_window = sg.Window('VOSK Live Subtitles', layout, resizable=True, keep_on_top=True, finalize=True)
+    main_window = sg.Window('PyVOSKLiveSubtitles-'+VERSION, layout, resizable=True, keep_on_top=True, finalize=True)
     main_window['-SRC-'].block_focus()
+    main_window.bind("<Button-3>", "right_click")
+    main_window['-URL-'].bind("<FocusIn>", "FocusIn")
+    main_window['-ML-SRC-RESULTS-'].bind("<FocusIn>", "FocusIn")
+    main_window['-ML-SRC-PARTIAL-RESULTS-'].bind("<FocusIn>", "FocusIn")
+    main_window['-ML-DST-RESULTS-'].bind("<FocusIn>", "FocusIn")
+    main_window['-ML-DST-PARTIAL-RESULTS-'].bind("<FocusIn>", "FocusIn")
 
     if (sys.platform == "win32"):
         if main_window.TKroot is not None:
             main_window.TKroot.attributes('-topmost', True)
             main_window.TKroot.attributes('-topmost', False)
 
     if not (sys.platform == "win32"):
         if main_window.TKroot is not None:
             main_window.TKroot.attributes('-topmost', 1)
             main_window.TKroot.attributes('-topmost', 0)
 
     overlay_translation_window = None
     move_center(main_window)
 
-    FONT_TYPE = "Helvetica"
-    FONT_SIZE = 9
-    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+    FONT = ("Helvetica", 10)
+    sg.set_options(font=FONT)
 
-    #transcribe_window = make_transcribe_window("", 100)
-    #move_center(transcribe_window)
-    #transcribe_window.Hide()
     transcribe_window = None
 
     progressbar = make_progress_bar_window("", 100)
     progressbar.Hide()
 
     main_window['-URL-'].update("")
     main_window['-RECORD-STREAMING-'].update(False)
@@ -2693,15 +2761,14 @@
 
     if args.dst_language:
         combo_dst = map_language_of_dst[args.dst_language]
         main_window['-DST-'].update(combo_dst)
 
     if args.url:
         is_valid_url_streaming = is_streaming_url(args.url)
-        #print("is_valid_url_streaming = {}".format(is_valid_url_streaming))
         if is_valid_url_streaming:
             url = args.url
             main_window['-URL-'].update(url)
             main_window['-RECORD-STREAMING-'].update(True)
 
     main_window['-ML-SRC-PARTIAL-RESULTS-'].update("")
     main_window['-ML-SRC-RESULTS-'].update("")
@@ -2738,23 +2805,88 @@
         dst = map_dst_of_language[str(main_window['-DST-'].get())]
         last_selected_dst = dst
         dst_file = open(dst_filepath, "w")
         dst_file.write(dst)
         dst_file.close()
 
 
+        if event == 'right_click':
+
+            x, y = main_window.TKroot.winfo_pointerxy()
+            widget = main_window.TKroot.winfo_containing(x, y)
+            widget.focus_set()
+
+
+        if event == 'Copy':
+
+            key = main_window.find_element_with_focus().Key
+            widget = main_window[key].Widget
+            selected_text = None
+            try:
+                selected_text = widget.selection_get()
+            except:
+                pass
+            if sys.platform == "win32":
+                if selected_text:
+                    win32clipboard.OpenClipboard()
+                    win32clipboard.EmptyClipboard()
+                    win32clipboard.SetClipboardText(selected_text)
+                    win32clipboard.CloseClipboard()
+            elif sys.platform == "linux":
+                if selected_text:
+                    set_clipboard_text(selected_text)
+
+
+        elif event == 'Paste':
+
+            key = main_window.find_element_with_focus().Key
+            current_value = values[key]
+            text_elem = main_window[key]
+            element_type = type(text_elem)
+            strings = str(text_elem.Widget.index('insert'))
+            cursor_position_strings = ""
+            if "Input" in str(element_type):
+                cursor_position_strings = strings
+            elif "Multiline" in str(element_type):
+                cursor_position_strings = strings[2:]
+            cursor_position = int(cursor_position_strings)
+            clipboard_data = None
+            if sys.platform == "win32":
+                try:
+                    win32clipboard.OpenClipboard()
+                    clipboard_data = win32clipboard.GetClipboardData()
+                except Exception as e:
+                    #show_error_messages(e)
+                    pass
+            elif sys.platform == "linux":
+                try:
+                    clipboard_data = get_clipboard_text()
+                except:
+                    pass
+                    
+            if clipboard_data:
+                new_value = current_value[:cursor_position] + clipboard_data + current_value[cursor_position:]
+                main_window[key].update(new_value)
+                cursor_position += len(clipboard_data)
+                if "Multiline" in str(element_type):
+                    text_elem.Widget.mark_set('insert', f'1.{cursor_position}')
+                    text_elem.Widget.see(f'1.{cursor_position}')
+                elif "Input" in str(element_type):
+                    text_elem.Widget.icursor(cursor_position)
+                    text_elem.Widget.xview_moveto(1.0)
+
+
         if event == 'Exit' or event == sg.WIN_CLOSED:
 
             if transcribe_window is not None and window == transcribe_window:
 
                 if not not_transcribing:
-                    FONT_TYPE = "Helvetica"
-                    FONT_SIZE = 9
-                    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
-                    answer = popup_yes_no('             Are you sure?              ', title='Confirm')
+                    FONT = ("Helvetica", 10)
+                    sg.set_options(font=FONT)
+                    answer = popup_yes_no('Are you sure?', title='Confirm')
                     if 'Yes' in answer:
                         not_transcribing = True
                         if thread_vosk_transcribe and thread_vosk_transcribe.is_alive(): stop_thread(thread_vosk_transcribe)
                         transcribe_window.close()
                         main_window.Normal()
                 else:
                     not_transcribing = True
@@ -2795,38 +2927,22 @@
                 user32.CloseClipboard()
             elif sys.platform == "linux":
                 text = get_clipboard_text()
                 if text:
                     main_window['-URL-'].update(text.strip())
 
 
-        elif event == 'Paste':
-
-            if sys.platform == "win32":
-                user32.OpenClipboard(None)
-                clipboard_data = user32.GetClipboardData(1)  # 1 is CF_TEXT
-                if clipboard_data:
-                    data = ctypes.c_char_p(clipboard_data)
-                    main_window['-URL-'].update(data.value.decode('utf-8'))
-                user32.CloseClipboard()
-            elif sys.platform == "linux":
-                text = get_clipboard_text()
-                if text:
-                    main_window['-URL-'].update(text.strip())
-
-
         elif event == '-RECORD-STREAMING-':
 
             if values['-RECORD-STREAMING-']:
                 is_valid_url_streaming = is_streaming_url(str(values['-URL-']).strip())
                 if not is_valid_url_streaming:
-                    FONT_TYPE = "Helvetica"
-                    FONT_SIZE = 9
-                    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
-                    sg.Popup('Invalid URL, please enter a valid URL.                   ', title="Info", line_width=50)
+                    FONT = ("Helvetica", 10)
+                    sg.set_options(font=FONT)
+                    sg.Popup('Invalid URL, please enter a valid URL', title="Info", line_width=50)
                     main_window['-RECORD-STREAMING-'].update(False)
 
 
         elif event == '-START-BUTTON-':
             recognizing = not recognizing
             #print("Start button clicked, changing recognizing status")
             #print("recognizing = {}".format(recognizing))
@@ -2876,18 +2992,17 @@
                             thread_record_streaming.start()
 
                         elif sys.platform == "linux":
                             thread_record_streaming = Thread(target=record_streaming_linux, args=(stream_url.url, tmp_recorded_streaming_filepath))
                             thread_record_streaming.start()
 
                     else:
-                        FONT_TYPE = "Helvetica"
-                        FONT_SIZE = 9
-                        sg.set_options(font=(FONT_TYPE, FONT_SIZE))
-                        sg.Popup('Invalid URL, please enter a valid URL.                   ', title="Info", line_width=50)
+                        FONT = ("Helvetica", 10)
+                        sg.set_options(font=FONT)
+                        sg.Popup('Invalid URL, please enter a valid URL', title="Info", line_width=50)
                         recognizing = False
                         main_window['-START-BUTTON-'].update(('Stop','Start')[not recognizing], button_color=(('white', ('red', '#283b5b')[not recognizing])))
                         main_window['-RECORD-STREAMING-'].update(False)
 
                 regions = []
                 transcriptions = []
 
@@ -3008,15 +3123,15 @@
                 main_window.TKroot.attributes('-topmost', 0)
 
 
         elif event == '-EVENT-RESULTS-' and recognizing==True:
 
             line = str(values[event]).strip().lower()
             main_window['-ML-SRC-RESULTS-'].update(line + "\n", background_color_for_value='yellow1', append=True, autoscroll=True)
-            translated_line = GoogleTranslate(line, src, dst)
+            translated_line = GoogleTranslate(line, src, dst, error_messages_callback=show_error_messages)
             main_window['-ML-DST-RESULTS-'].update(translated_line + "\n", background_color_for_value='yellow1', append=True, autoscroll=True)
             if overlay_translation_window is not None:
                 overlay_translation_window.UnHide
                 overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_line, background_color_for_value='black', visible=True, autoscroll=True)
             else:
                 overlay_translation_window = make_overlay_translation_window(100*' ')
                 overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_line, background_color_for_value='black', visible=True, autoscroll=True)
@@ -3063,17 +3178,16 @@
 
             pb = values[event]
             info = pb[0]
             total = pb[1]
             percentage = pb[2]
             progress = pb[3]
 
-            FONT_TYPE = "Helvetica"
-            FONT_SIZE = 9
-            sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+            FONT = ("Helvetica", 10)
+            sg.set_options(font=FONT)
 
             progressbar.UnHide()
 
             progressbar['-INFO-'].update(info)
             progressbar['-PERCENTAGE-'].update(percentage)
             progressbar['-PROGRESS-'].update(progress)
             if progress == total:
@@ -3083,25 +3197,24 @@
 
         elif event == '-EVENT-TRANSCRIBE-PREPARE-WINDOW-':
 
             prepare = values[event]
 
             if prepare:
 
-                FONT_TYPE = "Helvetica"
-                FONT_SIZE = 9
-                sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+                FONT = ("Helvetica", 10)
+                sg.set_options(font=FONT)
                 #transcribe_window.UnHide()
                 transcribe_window = make_transcribe_window("", 100)
 
                 for element in transcribe_window.element_list():
                     if isinstance(element, sg.Text) or isinstance(element, sg.Multiline):
-                        element.update(font=(FONT_TYPE, FONT_SIZE))
+                        element.update(font=FONT)
                     if isinstance(element, sg.Button):
-                        transcribe_window['-CANCEL-'].Widget.config(font=(FONT_TYPE, FONT_SIZE))
+                        transcribe_window['-CANCEL-'].Widget.config(font=FONT)
 
                 transcribe_window['-OUTPUT-MESSAGES-'].update("")
                 transcribe_window['-INFO-'].update("Progress info")
                 transcribe_window['-PROGRESS-'].update(0)
                 transcribe_window['-PERCENTAGE-'].update("0%")
                 move_center(transcribe_window)
                 transcribe_window.refresh()
@@ -3186,30 +3299,29 @@
             else:
                 tmp_recorded_streaming_filename = args.video_filename
 
             tmp_recorded_streaming_filepath = os.path.join(tempfile.gettempdir(), tmp_recorded_streaming_filename)
 
             if os.path.isfile(tmp_recorded_streaming_filepath):
 
-                saved_recorded_streaming_filename = sg.popup_get_file('', no_window=True, save_as=True, font=(FONT_TYPE, FONT_SIZE), default_path=saved_recorded_streaming_filename, file_types=video_file_types)
+                saved_recorded_streaming_filename = sg.popup_get_file('', no_window=True, save_as=True, font=FONT, default_path=saved_recorded_streaming_filename, file_types=video_file_types)
 
                 if saved_recorded_streaming_filename:
                     shutil.copy(tmp_recorded_streaming_filepath, saved_recorded_streaming_filename)
 
             else:
-                FONT_TYPE = "Helvetica"
-                FONT_SIZE = 9
-                sg.set_options(font=(FONT_TYPE, FONT_SIZE))
-                sg.Popup("No streaming was recorded.                             ", title="Info", line_width=50)
+                FONT = ("Helvetica", 10)
+                sg.set_options(font=FONT)
+                sg.Popup("No streaming was recorded", title="Info", line_width=50)
 
 
         elif event == '-EVENT-SAVE-SRC-TRANSCRIPTION-':
             if os.path.isfile(tmp_src_txt_transcription_filepath):
 
-                saved_src_subtitle_filename = sg.popup_get_file('', no_window=True, save_as=True, font=(FONT_TYPE, FONT_SIZE), file_types=subtitle_file_types)
+                saved_src_subtitle_filename = sg.popup_get_file('', no_window=True, save_as=True, font=FONT, file_types=subtitle_file_types)
 
                 if saved_src_subtitle_filename:
 
                     selected_subtitle_format = saved_src_subtitle_filename.split('.')[-1]
 
                     if selected_subtitle_format in FORMATTERS.keys():
                         timed_subtitles = [(r, t) for r, t in zip(regions, transcriptions) if t]
@@ -3226,25 +3338,24 @@
                         for line in tmp_src_txt_transcription_file:
                             if line:
                                 saved_src_subtitle_file.write(line)
                         saved_src_subtitle_file.close()
                         tmp_src_txt_transcription_file.close()
 
             else:
-                FONT_TYPE = "Helvetica"
-                FONT_SIZE = 9
-                sg.set_options(font=(FONT_TYPE, FONT_SIZE))
-                sg.Popup("No transcriptions was recorded                             ", title="Info", line_width=50)
+                FONT = ("Helvetica", 10)
+                sg.set_options(font=FONT)
+                sg.Popup("No transcriptions was recorded", title="Info", line_width=50)
 
 
         elif event == '-EVENT-SAVE-DST-TRANSCRIPTION-':
 
             if os.path.isfile(tmp_dst_txt_transcription_filepath):
 
-                saved_dst_subtitle_filename = sg.popup_get_file('', no_window=True, save_as=True, font=(FONT_TYPE, FONT_SIZE), file_types=subtitle_file_types)
+                saved_dst_subtitle_filename = sg.popup_get_file('', no_window=True, save_as=True, font=FONT, file_types=subtitle_file_types)
 
                 if saved_dst_subtitle_filename:
 
                     selected_subtitle_format = saved_dst_subtitle_filename.split('.')[-1]
 
                     if selected_subtitle_format in FORMATTERS.keys():
                         timed_translated_subtitles = [(r, t) for r, t in zip(created_regions, translated_transcriptions) if t]
@@ -3259,23 +3370,21 @@
                         tmp_dst_txt_transcription_file = open(tmp_dst_txt_transcription_filepath, "r")
                         for line in tmp_dst_txt_transcription_file:
                             if line:
                                 saved_dst_subtitle_file.write(line)
                         saved_dst_subtitle_file.close()
                         tmp_dst_txt_transcription_file.close()
             else:
-                FONT_TYPE = "Helvetica"
-                FONT_SIZE = 9
-                sg.set_options(font=(FONT_TYPE, FONT_SIZE))
-                sg.Popup("No translated transcriptions was recorded                 ", title="Info", line_width=50)
+                FONT = ("Helvetica", 10)
+                sg.set_options(font=FONT)
+                sg.Popup("No translated transcriptions was recorded", title="Info", line_width=50)
 
 
         elif event == '-EXCEPTION-':
             e = str(values[event]).strip()
-            #sg.Popup("File format is not supported", title="Info", line_width=50)
             sg.Popup(e, title="Info", line_width=50)
             if transcribe_window: transcribe_window['-OUTPUT-MESSAGES-'].update("", append=False)
 
 
         elif event == '-LIVE-THREAD-':
             t = values[event]
             main_window['-DEBUG-'].update(t)
@@ -3323,14 +3432,15 @@
     if tmp_src_txt_transcription_filepath and os.path.isfile(tmp_src_txt_transcription_filepath): os.remove(tmp_src_txt_transcription_filepath)
     if tmp_dst_txt_transcription_filepath and os.path.isfile(tmp_dst_txt_transcription_filepath): os.remove(tmp_dst_txt_transcription_filepath)
     if os.path.isfile(regions_filepath): os.remove(regions_filepath)
     if os.path.isfile(transcriptions_filepath): os.remove(transcriptions_filepath)
     if os.path.isfile(transcribe_is_done_filepath): os.remove(transcribe_is_done_filepath)
 
     remove_temp_files("wav")
+    remove_temp_files("mp4")
 
     main_window.close()
     sys.exit(0)
 
 
 if __name__ == "__main__":
     multiprocessing.freeze_support()
```

### Comparing `pyvosklivesubtitle-0.1.5/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: pyvosklivesubtitle
-Version: 0.1.5
-Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
-Home-page: https://github.com/botbahlul/pyvosklivesubtitle
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 Bot Bahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+Metadata-Version: 2.1
+Name: pyvosklivesubtitle
+Version: 0.1.6
+Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
+Home-page: https://github.com/botbahlul/pyvosklivesubtitle
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 Bot Bahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+
```

### Comparing `pyvosklivesubtitle-0.1.5/setup.py` & `pyvosklivesubtitle-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-    #!/usr/bin/env python3
+#!/usr/bin/env python3.8
 from __future__ import unicode_literals
-
 import sys
 import os
 import stat
+from pyvosklivesubtitle import VERSION
 
 #from setuptools import setup
 #from setuptools.command.install import install
 #from distutils import log
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
+
 if sys.version_info < (2, 6):
     print("THIS MODULE REQUIRES PYTHON 2.6, 2.7, OR 3.3+. YOU ARE CURRENTLY USING PYTHON {0}".format(sys.version))
     sys.exit(1)
 
 
 long_description = (
     'pyvosklivesubtitle is a python based desktop aplication which can recognize any live streaming'
     'in 21 languages that supported by VOSK then translate and display it as LIVE SUBTITLES'
     )
 
+install_requires=[
+    "sounddevice>=0.4.4",
+    "vosk>=0.3.44",
+    "pysimplegui>=4.60.1",
+    "httpx>=0.13.3",
+    "streamlink>=5.3.1",
+    "six>=1.16.0",
+    "pysrt>=1.1.2",
+    "requests>=2.27.1",
+    "tqdm>=4.64.0",
+]
+
+if sys.platform == "win32":
+    install_requires.append("pywin32>=306")
+
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
-    version="0.1.5",
+    version=VERSION,
     include_package_data=True,
     author='Bot Bahlul',
     author_email='bot.bahlul@gmail.com',
     url='https://github.com/botbahlul/pyvosklivesubtitle',
     packages=[str('pyvosklivesubtitle')],
     entry_points={
         'console_scripts': [
             'pyvosklivesubtitle = pyvosklivesubtitle:main',
         ],
     },
-    install_requires=[
-        'sounddevice>=0.4.4',
-        'vosk>=0.3.44',
-        'pysimplegui>=4.60.1',
-        "httpx>=0.13.3",
-        "streamlink>=5.3.1",
-        "six>=1.16.0",
-        "pysrt>=1.1.2",
-        "requests>=2.27.1",
-        "tqdm>=4.64.0",
-    ],
+    install_requires=install_requires,
     license=open("LICENSE").read()
 )
```

