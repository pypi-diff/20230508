# Comparing `tmp/pyautosrt-0.1.4.tar.gz` & `tmp/pyautosrt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.1.4.tar", last modified: Sat Mar  4 21:47:30 2023, max compression
+gzip compressed data, was "pyautosrt-0.1.7.tar", last modified: Sat Apr 15 02:11:55 2023, max compression
```

## Comparing `pyautosrt-0.1.4.tar` & `pyautosrt-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 21:47:30.886200 pyautosrt-0.1.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-03-04 21:47:30.886950 pyautosrt-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-04 21:47:30.863722 pyautosrt-0.1.4/pyautosrt/
--rw-rw-rw-   0        0        0    39321 2023-03-04 21:42:51.000000 pyautosrt-0.1.4/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-04 21:47:30.884701 pyautosrt-0.1.4/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-03-04 21:47:30.000000 pyautosrt-0.1.4/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-03-04 21:47:30.000000 pyautosrt-0.1.4/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 21:47:30.000000 pyautosrt-0.1.4/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-04 21:47:30.000000 pyautosrt-0.1.4/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-03-04 21:47:30.000000 pyautosrt-0.1.4/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-04 21:47:30.000000 pyautosrt-0.1.4/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-03-04 21:47:30.888446 pyautosrt-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1512 2023-03-04 21:47:18.000000 pyautosrt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.658001 pyautosrt-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-04-15 02:11:55.658750 pyautosrt-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.635524 pyautosrt-0.1.7/pyautosrt/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.1.7/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.655753 pyautosrt-0.1.7/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-15 02:11:55.000000 pyautosrt-0.1.7/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-15 02:11:55.663245 pyautosrt-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2023-04-15 02:08:56.000000 pyautosrt-0.1.7/setup.py
```

### Comparing `pyautosrt-0.1.4/LICENSE` & `pyautosrt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.4/PKG-INFO` & `pyautosrt-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.4
+Version: 0.1.7
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.4/README.md` & `pyautosrt-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.4/pyautosrt/__init__.py` & `pyautosrt-0.1.7/pyautosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -664,27 +664,27 @@
                 pool.close()
                 pool.join()
                 pool = None
                 return
             extracted_regions.append(extracted_region)
             pBar(i, len(regions), 'Converting {} speech regions to FLAC files : '.format(file_display_name), main_window)
         pBar(len(regions), len(regions), 'Converting {} speech regions to FLAC files : '.format(file_display_name), main_window)
-        
+
         if not_transcribing: return
 
         for i, transcription in enumerate(pool.imap(recognizer, extracted_regions)):
             if not_transcribing:
                 pool.close()
                 pool.join()
                 pool = None
                 return
             transcriptions.append(transcription)
             pBar(i, len(regions), 'Creating {} transcriptions : '.format(file_display_name), main_window)
         pBar(len(regions), len(regions), 'Creating {} transcriptions : '.format(file_display_name), main_window)
- 
+
         if not_transcribing: return
 
         timed_subtitles = [(r, t) for r, t in zip(regions, transcriptions) if t]
         formatter = FORMATTERS.get(subtitle_format)
         formatted_subtitles = formatter(timed_subtitles)
 
         base, ext = os.path.splitext(filename)
@@ -721,17 +721,15 @@
             for i, translated_transcription in enumerate(pool.imap(transcript_translator, created_transcripts)):
                 if not_transcribing:
                     pool.close()
                     pool.join()
                     pool = None
                     return
                 translated_transcriptions.append(translated_transcription)
-                #pBar(i, len(timed_subtitles), 'Translating %12s from %5s to %5s         : ' %(file_display_name, src, dst), main_window)
                 pBar(i, len(timed_subtitles), 'Translating {} subtitles from {} to {} : '.format(file_display_name, src, dst), main_window)
-            #pBar(len(timed_subtitles), len(timed_subtitles), 'Translating %12s from %5s to %5s         : ' %(file_display_name, src, dst), main_window)
             pBar(len(timed_subtitles), len(timed_subtitles), 'Translating {} subtitles from {} to {} : '.format(file_display_name, src, dst), main_window)
 
             if not_transcribing: return
 
             timed_translated_subtitles = [(r, t) for r, t in zip(created_regions, translated_transcriptions) if t]
             formatter = FORMATTERS.get(subtitle_format)
             formatted_translated_subtitles = formatter(timed_translated_subtitles)
@@ -791,26 +789,39 @@
     layout = [
         [sg.Text(text)],
         [sg.Push(), sg.Button('Yes'), sg.Button('No')],
     ]
     return sg.Window(title if title else text, layout, resizable=True).read(close=True)
 
 
+def make_progress_bar_window(total, info):
+    FONT_TYPE = "Arial"
+    FONT_SIZE = 9
+    sg.set_options(font=(FONT_TYPE, FONT_SIZE))
+
+    layout = [[sg.Text(info, key='-INFO-')],
+              [sg.ProgressBar(total, orientation='h', size=(30, 10), key='-PROGRESS-'), sg.Text(size=(5,1), key='-PERCENTAGE-')]]
+
+    window = sg.Window("Progress", layout, no_titlebar=False, finalize=True)
+
+    return window
+
+
 #--------------------------------------------------------------MAIN FUNCTIONS------------------------------------------------------------#
 
 
 def main():
     global all_threads, thread_transcribe, not_transcribing, pool
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('source_path', help="Path to the video or audio files to generate subtitle (use wildcard for multiple files)", nargs='*')
+    parser.add_argument('source_path', help="Path to the video or audio files to generate subtitle (use wildcard for multiple files or separate them with space eg. \"file 1.mp4\" \"file 2.mp4\")", nargs='*', default='')
     parser.add_argument('-S', '--src-language', help="Voice language", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired language for translation", default="en")
     parser.add_argument('-F', '--format', help="Destination subtitle format", default="srt")
-    parser.add_argument('-v', '--version', action='version', version='0.1.4')
+    parser.add_argument('-v', '--version', action='version', version='0.1.7')
     parser.add_argument('-lf', '--list-formats', help="List all available subtitle formats", action='store_true')
     parser.add_argument('-ll', '--list-languages', help="List all available source/translation languages", action='store_true')
 
     args = parser.parse_args()
 
     if args.list_formats:
         print("List of formats:")
@@ -861,26 +872,40 @@
               [sg.Button('Exit', expand_x=True, expand_y=True)]]
 
     main_window = sg.Window('PyAutoSRT', layout, font=font, resizable=True, keep_on_top=True, finalize=True)
     main_window['-SRC-'].block_focus()
     main_window.TKroot.option_add("*Font", font)
 
     if args.source_path:
-        for arg in args.source_path:
-            filelist += glob(arg)
-        for file in filelist:
-            if os.path.isfile(file):
-                filepath = os.path.join(os.getcwd(), file)
-                input_string = input_string + filepath + ";"
-                main_window['-INPUT-'].update(input_string)
+        if "*" in str(args.source_path) or len(args.source_path)>1:
+            for arg in args.source_path:
+                filelist += glob(arg)
+            for file in filelist:
+                if os.path.isfile(file):
+                    filepath = os.path.join(os.getcwd(), file)
+                    input_string = input_string + filepath + ";"
+                    main_window['-INPUT-'].update(input_string)
+                else:
+                    filepath = None
+                    main_window['-OUTPUT-MESSAGES-'].update('File path you typed is not exist, please browse it\n')
+
+            input_string = input_string[:-1]
+            main_window['-INPUT-'].update(input_string)
+
+        else:
+            if not os.sep in args.source_path[0]:
+                filepath = os.path.join(os.getcwd(),args.source_path[0])
+            else:
+                filepath = args.source_path[0]
+
+            if os.path.isfile(filepath):
+                main_window['-INPUT-'].update(filepath)
             else:
-                filepath = None
-                main_window['-OUTPUT-MESSAGES-'].update('File path you typed is not exist, please browse it\n')
-        input_string = input_string[:-1]
-        main_window['-INPUT-'].update(input_string)
+                main_window['-INPUT-'].update('')
+                main_window['-OUTPUT-MESSAGES-'].update('File path you typed is not exist, please browse it\n\n')
 
     if args.src_language:
         if args.src_language not in map_language_of_code.keys():
             main_window['-OUTPUT-MESSAGES-'].update('Source language you typed is not supported\nPlease select one from combobox\n\n', append=True)
         elif args.src_language in map_language_of_code.keys():
             src = args.src_language
             main_window['-SRC-'].update(map_language_of_code[src])
@@ -908,15 +933,15 @@
             main_window['-SUBTITLE-FORMAT-'].update(subtitle_format)
 
     if not args.format:
         subtitle_format = 'srt'
         main_window['-SUBTITLE-FORMAT-'].update(subtitle_format)
 
 
-    if  (sys.platform == "win32"):
+    if (sys.platform == "win32"):
         main_window.TKroot.attributes('-topmost', True)
         main_window.TKroot.attributes('-topmost', False)
 
     if not (sys.platform == "win32"):
         main_window.TKroot.attributes('-topmost', 1)
         main_window.TKroot.attributes('-topmost', 0)
 
@@ -944,21 +969,21 @@
             src = map_code_of_language[str(main_window['-SRC-'].get())]
             dst = map_code_of_language[str(main_window['-DST-'].get())]
 
         elif event == '-START-':
             src = map_code_of_language[str(main_window['-SRC-'].get())]
             dst = map_code_of_language[str(main_window['-DST-'].get())]
             filelist = []
-            filelist += values[0].split(';')
+            filelist += values['-INPUT-'].split(';')
             subtitle_format = values['-SUBTITLE-FORMAT-']
             thread_transcribe = None
             all_threads = []
             main_window['-RESULTS-'].update('', append=False)
 
-            if filelist and src and dst and subtitle_format:
+            if len(filelist)>0 and src and dst and subtitle_format:
                 not_transcribing = not not_transcribing
 
                 if not not_transcribing:
                     main_window['-START-'].update(('Cancel','Start')[not_transcribing], button_color=(('white', ('red', '#283b5b')[not_transcribing])))
                     for file in filelist:
                         if os.path.isfile(file):
                             filepath = os.path.join(os.getcwd(), file)
```

### Comparing `pyautosrt-0.1.4/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.1.7/pyautosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.4
+Version: 0.1.7
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.4/setup.py` & `pyautosrt-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'them to a different language, and finally saves the resulting subtitles to disk.'
     'It supports  a variety of input and output languages  and can currently produce '
     'subtitles in SRT, VTT, JSON, and RAW format.'
 )
 
 setup(
     name="pyautosrt",
-    version="0.1.4",
+    version="0.1.7",
     description="pyautosrt is a python based desktop app to generate subtitle and translated subtitle file",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/pyautosrt",
     packages=[str("pyautosrt")],
     entry_points={
```

