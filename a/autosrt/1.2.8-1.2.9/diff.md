# Comparing `tmp/autosrt-1.2.8.tar.gz` & `tmp/autosrt-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.2.8.tar", last modified: Tue May  2 12:00:43 2023, max compression
+gzip compressed data, was "autosrt-1.2.9.tar", last modified: Tue May  2 19:12:11 2023, max compression
```

## Comparing `autosrt-1.2.8.tar` & `autosrt-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.670415 autosrt-1.2.8/
--rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 autosrt-1.2.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 autosrt-1.2.8/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 12:00:43.671018 autosrt-1.2.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5260 2023-04-30 04:22:31.000000 autosrt-1.2.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.662201 autosrt-1.2.8/autosrt/
--rwxrwxrwx   0 root         (0) root         (0)     9271 2023-05-02 11:58:44.000000 autosrt-1.2.8/autosrt/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    33439 2023-05-02 10:41:14.000000 autosrt-1.2.8/autosrt/autosrt.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.667758 autosrt-1.2.8/autosrt.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      112 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-02 12:00:43.672433 autosrt-1.2.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1695 2023-05-02 12:00:07.000000 autosrt-1.2.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.669526 autosrt-1.2.8/test/
--rwxrwxrwx   0 root         (0) root         (0)     6874 2023-04-30 02:05:08.000000 autosrt-1.2.8/test/test1.py
--rwxrwxrwx   0 root         (0) root         (0)     4087 2023-04-30 02:05:48.000000 autosrt-1.2.8/test/test2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.342594 autosrt-1.2.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 autosrt-1.2.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 autosrt-1.2.9/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 19:12:11.342956 autosrt-1.2.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5260 2023-04-30 04:22:31.000000 autosrt-1.2.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.334160 autosrt-1.2.9/autosrt/
+-rwxrwxrwx   0 root         (0) root         (0)     9904 2023-05-02 18:58:47.000000 autosrt-1.2.9/autosrt/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    41313 2023-05-02 18:58:47.000000 autosrt-1.2.9/autosrt/autosrt.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.339510 autosrt-1.2.9/autosrt.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      112 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-05-02 19:12:11.000000 autosrt-1.2.9/autosrt.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-02 19:12:11.344352 autosrt-1.2.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1723 2023-05-02 18:58:47.000000 autosrt-1.2.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 19:12:11.341842 autosrt-1.2.9/test/
+-rwxrwxrwx   0 root         (0) root         (0)     7362 2023-05-02 18:58:47.000000 autosrt-1.2.9/test/test1.py
+-rwxrwxrwx   0 root         (0) root         (0)     4465 2023-05-02 18:58:47.000000 autosrt-1.2.9/test/test2.py
```

### Comparing `autosrt-1.2.8/LICENSE` & `autosrt-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.8/PKG-INFO` & `autosrt-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.2.8
+Version: 1.2.9
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.2.8/README.md` & `autosrt-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.8/autosrt/__init__.py` & `autosrt-1.2.9/autosrt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,43 +3,46 @@
 import argparse
 import os
 import sys
 import multiprocessing
 from glob import glob
 from progressbar import ProgressBar, Percentage, Bar, ETA
 
-from .autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
+from .autosrt import VERSION, Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter, \
     stop_ffmpeg_windows, stop_ffmpeg_linux, remove_temp_files, is_same_language, is_video_file, is_audio_file
 
-def show_progress(percentage):
+def show_progress(progress):
     global pbar
-    pbar.update(percentage)
+    pbar.update(progress)
+
+def show_error_messages(messages):
+    print(messages)
 
 def main():
     global pbar
 
     if sys.platform == "win32":
-        stop_ffmpeg_windows()
+        stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
-        stop_ffmpeg_linux()
+        stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
-    remove_temp_files("flac")
-    remove_temp_files("wav")
+    remove_temp_files("flac", error_messages_callback=show_error_messages)
+    remove_temp_files("wav", error_messages_callback=show_error_messages)
 
     parser = argparse.ArgumentParser()
     parser.add_argument('source_path', help="File path of the video or audio files to generate subtitles files (use wildcard for multiple files or separate them with a space character)", nargs='*')
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
     parser.add_argument('-o', '--output', help="Output file path for subtitles (by default, subtitles are saved in the same directory and named with the source_path base name)")
     parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
     parser.add_argument('-lf', '--list-formats', help="List all supported subtitle formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
-    parser.add_argument('-v', '--version', action='version', version='1.2.8')
+    parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
@@ -96,23 +99,23 @@
             print("{} is not exist".format(arg))
 
     for media_filepath in media_filepaths:
         print("Processing {} :".format(media_filepath))
 
         widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
-        wav_converter = WavConverter()
-        audio_filepath, audio_rate = wav_converter(media_filepath, progress_callback=show_progress)
+        wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
+        wav_filepath, sample_rate = wav_converter(media_filepath)
         pbar.finish()
 
-        region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6)
-        regions = region_finder(audio_filepath)
+        region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
+        regions = region_finder(wav_filepath)
 
-        converter = FLACConverter(wav_filepath=audio_filepath)
-        recognizer = SpeechRecognizer(language=args.src_language, rate=audio_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw")
+        converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
+        recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
 
         pool = multiprocessing.Pool(args.concurrency)
 
         if regions:
             try:
                 widgets = ["Converting speech regions to FLAC files : ", Percentage(), ' ', Bar(), ' ', ETA()]
                 pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
@@ -131,15 +134,15 @@
                 pbar.finish()
 
             except KeyboardInterrupt:
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
-                print("Cancelling transcription")
+                print("Cancelling all tasks")
                 return 1
 
             except Exception as e:
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
@@ -155,55 +158,56 @@
                 subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=subtitle_format)
             else:
                 subtitle_filepath = args.output
         else:
             base, ext = os.path.splitext(media_filepath)
             subtitle_filepath = "{base}.{format}".format(base=base, format=subtitle_format)
 
-        writer = SubtitleWriter(regions, transcripts, subtitle_format)
+        writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
         writer.write(subtitle_filepath)
 
         if do_translate:
-
             # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
             # NO NEED TO TRANSLATE ALL transcript IN transcripts
             # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
             # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
             timed_subtitles = writer.timed_subtitles
             created_regions = []
             created_subtitles = []
             for entry in timed_subtitles:
                 created_regions.append(entry[0])
                 created_subtitles.append(entry[1])
 
             prompt = "Translating from %8s to %8s   : " %(args.src_language, args.dst_language)
             widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
-            transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language)
+
+            transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
+
             translated_subtitles = []
             for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                 translated_subtitles.append(translated_subtitle)
                 pbar.update(i)
             pbar.finish()
 
             translated_subtitle_filepath = subtitle_filepath[ :-4] + '.translated.' + subtitle_format
-            translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format)
+            translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
             translation_writer.write(translated_subtitle_filepath)
 
         print('Done.')
         if do_translate:
             print("Original subtitles file created at      : {}".format(subtitle_filepath))
             print('Translated subtitles file created at    : {}' .format(translated_subtitle_filepath))
         else:
             print("Subtitles file created at               : {}".format(subtitle_filepath))
 
     if sys.platform == "win32":
-        stop_ffmpeg_windows()
+        stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
-        stop_ffmpeg_linux()
+        stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     pool.close()
     pool.join()
 
     remove_temp_files("flac")
     remove_temp_files("wav")
```

### Comparing `autosrt-1.2.8/autosrt/autosrt.py` & `autosrt-1.2.9/autosrt/autosrt.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,52 +20,89 @@
 import pysrt
 import six
 # ADDITIONAL IMPORT
 import ffmpeg_progress_yield
 from ffmpeg_progress_yield import FfmpegProgress
 import magic
 
+VERSION = "1.2.9"
 
-def stop_ffmpeg_windows():
+def stop_ffmpeg_windows(error_messages_callback=None):
     try:
         tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         ffmpeg_pid = None
         for line in tasklist_output.split('\n'):
             if "ffmpeg" in line:
                 ffmpeg_pid = line.split()[1]
                 break
         if ffmpeg_pid:
             devnull = open(os.devnull, 'w')
             subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
     except Exception as e:
-        print(e)
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
         return
 
 
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
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
     except Exception as e:
-        print(e)
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
         return
 
 
-def remove_temp_files(extension):
-    temp_dir = tempfile.gettempdir()
-    for root, dirs, files in os.walk(temp_dir):
-        for file in files:
-            if file.endswith("." + extension):
-                os.remove(os.path.join(root, file))
+def remove_temp_files(extension, error_messages_callback=None):
+    try:
+        temp_dir = tempfile.gettempdir()
+        for root, dirs, files in os.walk(temp_dir):
+            for file in files:
+                if file.endswith("." + extension):
+                    os.remove(os.path.join(root, file))
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
 
 
 def is_same_language(src, dst):
     return src.split("-")[0] == dst.split("-")[0]
 
 
 def is_video_file(file_path):
@@ -517,26 +554,34 @@
     def ffmpeg_check():
         if WavConverter.which("ffmpeg"):
             return "ffmpeg"
         if WavConverter.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, channels=1, rate=48000):
+    def __init__(self, channels=1, rate=48000, progress_callback=None, error_messages_callback=None):
         self.channels = channels
         self.rate = rate
+        self.progress_callback = progress_callback
+        self.error_messages_callback = error_messages_callback
 
-    def __call__(self, media_filepath, progress_callback=None):
+    def __call__(self, media_filepath):
         temp = tempfile.NamedTemporaryFile(suffix='.wav', delete=False)
         if not os.path.isfile(media_filepath):
-            print("The given file does not exist: {0}".format(media_filepath))
-            raise Exception("Invalid file: {0}".format(media_filepath))
+            if self.error_messages_callback:
+                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+            else:
+                print("The given file does not exist: {0}".format(media_filepath))
+                raise Exception("Invalid file: {0}".format(media_filepath))
         if not self.ffmpeg_check():
-            print("ffmpeg: Executable not found on machine.")
-            raise Exception("Dependency not found: ffmpeg")
+            if self.error_messages_callback:
+                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+            else:
+                print("ffmpeg: Executable not found on machine.")
+                raise Exception("Dependency not found: ffmpeg")
 
         command = [
                     "ffmpeg",
                     "-y",
                     "-i", media_filepath,
                     "-ac", str(self.channels),
                     "-ar", str(self.rate),
@@ -551,54 +596,72 @@
             #subprocess.check_output(command, stdin=open(os.devnull), shell=use_shell)
 
             # RUNNING ffmpeg WITH PROGRESSS
             ff = FfmpegProgress(command)
             percentage = 0
             for progress in ff.run_command_with_progress():
                 percentage = progress
-                if progress_callback:
-                    progress_callback(percentage)
+                if self.progress_callback:
+                    self.progress_callback(percentage)
             temp.close()
         
             return temp.name, self.rate
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
             return
 
         except Exception as e:
-            print(e)
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
             return
 
 
 # DEFINE progress_callback FUNCTION TO SHOW ffmpeg PROGRESS
 # IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
-# global main_window
-# main_window.write_event_value('-UPDATE-PROGRESS-', percentage) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
-def show_progress(percentage):
-    global pbar
-    pbar.update(percentage)
+#def show_progress(percentage):
+    #global main_window
+    #main_window.write_event_value('-UPDATE-PROGRESS-', percentage) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
+# IF WE'RE IN console ENVIRONMENT WE CAN DO :
+#def show_progress(percentage):
+    #global pbar
+    #pbar.update(percentage)
+
+# DEFINE error_messages_callback FUNCTION TO SHOW ERROR MESSAGES
+# IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
+#def show_error_messages(messages):
+    #global main_window
+    #main_window.write_event_value('-EXCEPTION-', messages) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
+# IF WE'RE IN console ENVIRONMENT WE CAN DO :
+#def show_error_messages(messages):
+    #print(messages)
 
 
 class SpeechRegionFinder:
     @staticmethod
     def percentile(arr, percent):
         arr = sorted(arr)
         k = (len(arr) - 1) * percent
         f = math.floor(k)
         c = math.ceil(k)
         if f == c: return arr[int(k)]
         d0 = arr[int(f)] * (c - k)
         d1 = arr[int(c)] * (k - f)
         return d0 + d1
 
-    def __init__(self, frame_width=4096, min_region_size=0.5, max_region_size=6):
+    def __init__(self, frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=None):
         self.frame_width = frame_width
         self.min_region_size = min_region_size
         self.max_region_size = max_region_size
+        self.error_messages_callback = error_messages_callback
 
     def __call__(self, wav_filepath):
         try:
             reader = wave.open(wav_filepath)
             sample_width = reader.getsampwidth()
             rate = reader.getframerate()
             n_channels = reader.getnchannels()
@@ -622,27 +685,34 @@
                         region_start = None
                 elif (not region_start) and (not is_silence):
                     region_start = elapsed_time
                 elapsed_time += chunk_duration
             return regions
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
             return
 
         except Exception as e:
-            print(e)
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
             return
 
 
 class FLACConverter(object):
-    def __init__(self, wav_filepath, include_before=0.25, include_after=0.25):
+    def __init__(self, wav_filepath, include_before=0.25, include_after=0.25, error_messages_callback=None):
         self.wav_filepath = wav_filepath
         self.include_before = include_before
         self.include_after = include_after
+        self.error_messages_callback = error_messages_callback
 
     def __call__(self, region):
         try:
             start, end = region
             start = max(0, start - self.include_before)
             end += self.include_after
             temp = tempfile.NamedTemporaryFile(suffix='.flac', delete=False)
@@ -657,29 +727,36 @@
                       ]
             subprocess.check_output(command, stdin=open(os.devnull))
             content = temp.read()
             temp.close()
             return content
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
             return
 
         except Exception as e:
-            print(e)
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
             return
 
 
 class SpeechRecognizer(object):
-    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", timeout=30):
+    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", timeout=30, error_messages_callback=None):
         self.language = language
         self.rate = rate
         self.api_key = api_key
         self.retries = retries
         self.timeout = timeout
+        self.error_messages_callback = error_messages_callback
 
     def __call__(self, data):
         try:
             for i in range(self.retries):
                 url = "http://www.google.com/speech-api/v2/recognize?client=chromium&lang={lang}&key={key}".format(lang=self.language, key=self.api_key)
                 headers = {"Content-Type": "audio/x-flac rate=%d" % self.rate}
 
@@ -697,27 +774,35 @@
                         line = line['result'][0]['alternative'][0]['transcript']
                         return line[:1].upper() + line[1:]
                     except:
                         # no result
                         continue
 
         except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
             return
 
         except Exception as e:
-            print(e)
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
             return
 
 
 class SentenceTranslator(object):
-    def __init__(self, src, dst, patience=-1, timeout=30):
+    def __init__(self, src, dst, patience=-1, timeout=30, error_messages_callback=None):
         self.src = src
         self.dst = dst
         self.patience = patience
         self.timeout = timeout
+        self.error_messages_callback = error_messages_callback
 
     def __call__(self, sentence):
         try:
             translated_sentence = []
             # handle the special case: empty string.
             if not sentence:
                 return None
@@ -731,19 +816,25 @@
                     patience -= 1
                 else:
                     fail_to_translate = False
 
             return translated_sentence
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
             return
 
         except Exception as e:
-            print(e)
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
             return
 
     def GoogleTranslate(self, text, src, dst, timeout=30):
         url = 'https://translate.googleapis.com/translate_a/'
         params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
         headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
 
@@ -767,40 +858,65 @@
                     translation = ""
                     for i in range(length):
                         translation = translation + response_json[i][0]
                     return translation
                 return
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
             return
 
         except Exception as e:
-            print(e)
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
             return
 
 
 class SubtitleFormatter:
     supported_formats = ['srt', 'vtt', 'json', 'raw']
 
-    def __init__(self, format_type):
+    def __init__(self, format_type, error_messages_callback=None):
         self.format_type = format_type.lower()
+        self.error_messages_callback = error_messages_callback
         
     def __call__(self, subtitles, padding_before=0, padding_after=0):
-        if self.format_type == 'srt':
-            return self.srt_formatter(subtitles, padding_before, padding_after)
-        elif self.format_type == 'vtt':
-            return self.vtt_formatter(subtitles, padding_before, padding_after)
-        elif self.format_type == 'json':
-            return self.json_formatter(subtitles)
-        elif self.format_type == 'raw':
-            return self.raw_formatter(subtitles)
-        else:
-            raise ValueError(f'Unsupported format type: {self.format_type}')
-        
+        try:
+            if self.format_type == 'srt':
+                return self.srt_formatter(subtitles, padding_before, padding_after)
+            elif self.format_type == 'vtt':
+                return self.vtt_formatter(subtitles, padding_before, padding_after)
+            elif self.format_type == 'json':
+                return self.json_formatter(subtitles)
+            elif self.format_type == 'raw':
+                return self.raw_formatter(subtitles)
+            else:
+                if error_messages_callback:
+                    error_messages_callback(f'Unsupported format type: {self.format_type}')
+                else:
+                    raise ValueError(f'Unsupported format type: {self.format_type}')
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
+            else:
+                print(e)
+            return
+
     def srt_formatter(self, subtitles, padding_before=0, padding_after=0):
         """
         Serialize a list of subtitles according to the SRT format, with optional time padding.
         """
         sub_rip_file = pysrt.SubRipFile()
         for i, ((start, end), text) in enumerate(subtitles, start=1):
             item = pysrt.SubRipItem()
@@ -838,30 +954,102 @@
         """
         Serialize a list of subtitles as a newline-delimited string.
         """
         return ' '.join(text for (_rng, text) in subtitles)
 
 
 class SubtitleWriter:
-    def __init__(self, regions, transcripts, format):
+    def __init__(self, regions, transcripts, format, error_messages_callback=None):
         self.regions = regions
         self.transcripts = transcripts
         self.format = format
         self.timed_subtitles = [(r, t) for r, t in zip(self.regions, self.transcripts) if t]
+        self.error_messages_callback = error_messages_callback
 
     def get_timed_subtitles(self):
         return self.timed_subtitles
 
     def write(self, declared_subtitle_filepath):
-        formatter = SubtitleFormatter(self.format)
-        formatted_subtitles = formatter(self.timed_subtitles)
-        saved_subtitle_filepath = declared_subtitle_filepath
-        if saved_subtitle_filepath:
-            subtitle_file_base, subtitle_file_ext = os.path.splitext(saved_subtitle_filepath)
-            if not subtitle_file_ext:
-                saved_subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=self.format)
-            else:
-                saved_subtitle_filepath = declared_subtitle_filepath
-        with open(saved_subtitle_filepath, 'wb') as f:
-            f.write(formatted_subtitles.encode("utf-8"))
-        with open(saved_subtitle_filepath, 'a') as f:
-            f.write("\n")
+        try:
+            formatter = SubtitleFormatter(self.format)
+            formatted_subtitles = formatter(self.timed_subtitles)
+            saved_subtitle_filepath = declared_subtitle_filepath
+            if saved_subtitle_filepath:
+                subtitle_file_base, subtitle_file_ext = os.path.splitext(saved_subtitle_filepath)
+                if not subtitle_file_ext:
+                    saved_subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=self.format)
+                else:
+                    saved_subtitle_filepath = declared_subtitle_filepath
+            with open(saved_subtitle_filepath, 'wb') as f:
+                f.write(formatted_subtitles.encode("utf-8"))
+            #with open(saved_subtitle_filepath, 'a') as f:
+            #    f.write("\n")
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
+            else:
+                print(e)
+            return
+
+
+class SRTFileReader:
+    def __init__(self, srt_file_path, error_messages_callback=None):
+        self.timed_subtitles = self(srt_file_path)
+        self.error_messages_callback = error_messages_callback
+
+    @staticmethod
+    def __call__(srt_file_path):
+        try:
+            """
+            Read SRT formatted subtitle file and return subtitles as list of tuples
+            """
+            timed_subtitles = []
+            with open(srt_file_path, 'r') as srt_file:
+                lines = srt_file.readlines()
+                # Split the subtitle file into subtitle blocks
+                subtitle_blocks = []
+                block = []
+                for line in lines:
+                    if line.strip() == '':
+                        subtitle_blocks.append(block)
+                        block = []
+                    else:
+                        block.append(line.strip())
+                subtitle_blocks.append(block)
+
+                # Parse each subtitle block and store as tuple in timed_subtitles list
+                for block in subtitle_blocks:
+                    if block:
+                        # Extract start and end times from subtitle block
+                        start_time_str, end_time_str = block[1].split(' --> ')
+                        time_format = '%H:%M:%S,%f'
+                        start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
+                        start_time_total_seconds = start_time_time_delta.total_seconds()
+                        end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
+                        end_time_total_seconds = end_time_time_delta.total_seconds()
+                        # Extract subtitle text from subtitle block
+                        subtitle = ' '.join(block[2:])
+                        timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitle))
+                return timed_subtitles
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
+            else:
+                print(e)
+            return
+
```

### Comparing `autosrt-1.2.8/autosrt.egg-info/PKG-INFO` & `autosrt-1.2.9/autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.2.8
+Version: 1.2.9
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.2.8/setup.py` & `autosrt-1.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import unicode_literals
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
+from autosrt import VERSION
 
 long_description = (
     'autosrt is a utility for automatic speech recognition and subtitle generation.'
     'It takes a video or an audio file as input, performs voice activity detection '
     'to find speech regions,  makes parallel requests to Google Web Speech API  to '
     'generate transcriptions for those regions,  (optionally) translates them to a '
     'different language, and finally saves the resulting subtitles file to disk.   '
@@ -31,15 +32,15 @@
 elif sys.platform == "linux":
     install_requires.append("python-magic>=0.4.27")
 else:
     install_requires.append("python-magic>=0.4.27")
 
 setup(
     name="autosrt",
-    version="1.2.8",
+    version=VERSION,
     description="a utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/autosrt",
     packages=["autosrt"],
     entry_points={
```

### Comparing `autosrt-1.2.8/test/test1.py` & `autosrt-1.2.9/test/test1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import sys
 import multiprocessing
+from progressbar import ProgressBar, Percentage, Bar, ETA
+
 
 from autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter
 
 # CREATE A progress_callback FUNCTION TO SHOW PROGRESS WHEN CONVERT TO A TEMPORARY WAV FILE
 def show_progress(progress):
    global pbar
    pbar.update(progress)
 
 
+def show_error_messages(messages):
+    print(messages)
+
+
 def main():
     global pbar
 
     media_filepath = "balas budi.mp4"
 
     language = Language()
 
@@ -72,38 +78,39 @@
     # ALTERNATIVE 2
     #dst_language_name = "Indonesian"
     #dst_language_code = language.code_of_name[dst_language_name]
     #print("dst_language_code = {}".format(dst_language_code))
 
 
     # CONVERT MEDIA FILE TO A TEMPORARY WAV FILE
-    wav_converter = WavConverter()
 
     # CONVERT WITHOUT SHOWING THE PROGRESS
-    audio_filepath, audio_rate = wav_converter(media_filepath)
+    #wav_converter = WavConverter(channels=1, rate=48000, progress_callback=None, error_messages_callback=show_error_messages)
+    #wav_filepath, sample_rate = wav_converter(media_filepath)
 
     # CONVERT WITH SHOWING THE PROGRESS
-    #widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
-    #pbar = ProgressBar(widgets=widgets, maxval=100).start()
-    #audio_filepath, audio_rate = wav_converter(media_filepath, progress_callback=show_progress) 
-    #pbar.finish()
+    wav_converter = WavConverter(channels=1, rate=48000, progress_callback=show_progress, error_messages_callback=show_error_messages)
+    widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
+    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+    wav_filepath, sample_rate = wav_converter(media_filepath)
+    pbar.finish()
 
-    print("audio_filepath = {}".format(audio_filepath))
-    print("audio_rate = {}".format(audio_rate))
+    print("wav_filepath = {}".format(wav_filepath))
+    print("sample_rate = {}".format(sample_rate))
 
 
     # FIND SPEECH REGIONS OF TEMPORARY WAV FILE
-    region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6)
-    regions = region_finder(audio_filepath)
+    region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
+    regions = region_finder(wav_filepath)
     print("regions = {}".format(regions))
 
 
     # PREPARE FOR SPEECH RECOGNITION PROGRESS
-    converter = FLACConverter(wav_filepath=audio_filepath)
-    recognizer = SpeechRecognizer(language=src, rate=audio_rate)
+    converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
+    recognizer = SpeechRecognizer(language=src, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
 
     pool = multiprocessing.Pool(10)
 
     # GET AUDIO DATA OF EACH REGIONS (CONTENT OF TEMPORARY FLAC FILES)
     extracted_regions = []
     for i, extracted_region in enumerate(pool.imap(converter, regions)):
         print("Get region {} audio data".format(i))
@@ -167,20 +174,18 @@
 
     translated_subtitle_filepath = subtitle_filepath[ :-4] + '.translated.' + subtitle_format
     with open(translated_subtitle_filepath, 'wb') as tf:
         tf.write(formatted_translated_subtitles.encode("utf-8"))
     with open(translated_subtitle_filepath, 'a') as tf:
         tf.write("\n")
 
-
     # ALTERNATIVE 2 TO WRITE TRANSLATED SUBTITLE FILE USING SubtitleWriter CLASS
     #translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format)
     #translation_writer.write(translated_subtitle_filepath)
 
-
     print('Done.')
     print("Original subtitles file created at      : {}".format(subtitle_filepath))
     print('Translated subtitles file created at    : {}' .format(translated_subtitle_filepath))
 
 
 if __name__ == '__main__':
     multiprocessing.freeze_support()
```

### Comparing `autosrt-1.2.8/test/test2.py` & `autosrt-1.2.9/test/test2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 from autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter
 
 def show_progress(percentage):
     global pbar
     pbar.update(percentage)
 
+def show_error_messages(messages):
+    print(messages)
+
 def main():
     global pbar
 
     media_filepath = "balas budi.mp4"
     src = "zh-CN"
     dst = "id"
     subtitle_format = "srt"
 
     widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
     pbar = ProgressBar(widgets=widgets, maxval=100).start()
-    wav_converter = WavConverter()
-    audio_filepath, audio_rate = wav_converter(media_filepath, progress_callback=show_progress)
+    wav_converter = WavConverter(channels=1, rate=48000, progress_callback=show_progress, error_messages_callback=show_error_messages)
+    wav_filepath, sample_rate = wav_converter(media_filepath)
     pbar.finish()
 
-    speech_region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6)
-    regions = speech_region_finder(audio_filepath)
+    region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
+    regions = region_finder(wav_filepath)
 
-    converter = FLACConverter(wav_filepath=audio_filepath)
-    recognizer = SpeechRecognizer(language=src, rate=audio_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw")
+    converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
+    recognizer = SpeechRecognizer(language=src, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
 
     pool = multiprocessing.Pool(10)
 
     if regions:
         try:
             widgets = ["Converting speech regions to FLAC files : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
@@ -48,36 +51,36 @@
                 transcripts.append(transcript)
                 pbar.update(i)
             pbar.finish()
 
             subtitle_filepath = "harry.srt"
             subtitle_format = "srt"
 
-            writer = SubtitleWriter(regions, transcripts, subtitle_format)
+            writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
             writer.write(subtitle_filepath)
             timed_subtitles = writer.timed_subtitles
 
             created_regions = []
             created_subtitles = []
             for entry in timed_subtitles:
                 created_regions.append(entry[0])
                 created_subtitles.append(entry[1])
 
             prompt = "Translating from %8s to %8s   : " %(src, dst)
             widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
-            transcript_translator = SentenceTranslator(src=src, dst=dst)
+            transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
             translated_subtitles = []
             for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                 translated_subtitles.append(translated_subtitle)
                 pbar.update(i)
             pbar.finish()
 
             translated_subtitle_filepath = subtitle_filepath[ :-4] + '.translated.' + subtitle_format
-            translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format)
+            translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
             translation_writer.write(translated_subtitle_filepath)
 
             print('Done.')
             print("Original subtitles file created at      : {}".format(subtitle_filepath))
             print('Translated subtitles file created at    : {}' .format(translated_subtitle_filepath))
 
         except KeyboardInterrupt:
```

