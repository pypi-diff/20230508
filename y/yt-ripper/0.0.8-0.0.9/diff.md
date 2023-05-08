# Comparing `tmp/yt_ripper-0.0.8.tar.gz` & `tmp/yt_ripper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_ripper-0.0.8.tar", last modified: Mon Mar  6 18:20:58 2023, max compression
+gzip compressed data, was "yt_ripper-0.0.9.tar", last modified: Mon May  8 21:02:21 2023, max compression
```

## Comparing `yt_ripper-0.0.8.tar` & `yt_ripper-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-03-06 18:20:58.554219 yt_ripper-0.0.8/
--rw-r--r--   0 jona      (1000) jona      (1000)     1653 2023-03-06 18:20:58.554219 yt_ripper-0.0.8/PKG-INFO
--rw-r--r--   0 jona      (1000) jona      (1000)     1101 2023-03-06 18:16:09.000000 yt_ripper-0.0.8/README.md
--rw-r--r--   0 jona      (1000) jona      (1000)       38 2023-03-06 18:20:58.554219 yt_ripper-0.0.8/setup.cfg
--rw-r--r--   0 jona      (1000) jona      (1000)      962 2023-03-06 18:20:34.000000 yt_ripper-0.0.8/setup.py
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-03-06 18:20:58.550219 yt_ripper-0.0.8/yt_ripper/
--rw-r--r--   0 jona      (1000) jona      (1000)        0 2023-03-06 18:02:56.000000 yt_ripper-0.0.8/yt_ripper/__init__.py
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-03-06 18:20:58.553219 yt_ripper-0.0.8/yt_ripper/cli/
--rw-r--r--   0 jona      (1000) jona      (1000)        0 2023-03-06 17:41:26.000000 yt_ripper-0.0.8/yt_ripper/cli/__init__.py
--rw-r--r--   0 jona      (1000) jona      (1000)      332 2023-03-06 17:41:26.000000 yt_ripper-0.0.8/yt_ripper/cli/loading.py
--rw-r--r--   0 jona      (1000) jona      (1000)     1111 2023-03-06 18:19:57.000000 yt_ripper-0.0.8/yt_ripper/cli/menu.py
--rw-r--r--   0 jona      (1000) jona      (1000)     1693 2023-03-06 18:20:07.000000 yt_ripper-0.0.8/yt_ripper/cli/youtube.py
--rw-r--r--   0 jona      (1000) jona      (1000)     2519 2023-03-06 18:14:01.000000 yt_ripper-0.0.8/yt_ripper/main.py
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-03-06 18:20:58.553219 yt_ripper-0.0.8/yt_ripper/path/
--rw-r--r--   0 jona      (1000) jona      (1000)        0 2023-03-06 17:41:26.000000 yt_ripper-0.0.8/yt_ripper/path/__init__.py
--rw-r--r--   0 jona      (1000) jona      (1000)      429 2023-03-06 17:41:26.000000 yt_ripper-0.0.8/yt_ripper/path/utils.py
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-03-06 18:20:58.552219 yt_ripper-0.0.8/yt_ripper.egg-info/
--rw-r--r--   0 jona      (1000) jona      (1000)     1653 2023-03-06 18:20:58.000000 yt_ripper-0.0.8/yt_ripper.egg-info/PKG-INFO
--rw-r--r--   0 jona      (1000) jona      (1000)      407 2023-03-06 18:20:58.000000 yt_ripper-0.0.8/yt_ripper.egg-info/SOURCES.txt
--rw-r--r--   0 jona      (1000) jona      (1000)        1 2023-03-06 18:20:58.000000 yt_ripper-0.0.8/yt_ripper.egg-info/dependency_links.txt
--rw-r--r--   0 jona      (1000) jona      (1000)       49 2023-03-06 18:20:58.000000 yt_ripper-0.0.8/yt_ripper.egg-info/entry_points.txt
--rw-r--r--   0 jona      (1000) jona      (1000)       21 2023-03-06 18:20:58.000000 yt_ripper-0.0.8/yt_ripper.egg-info/requires.txt
--rw-r--r--   0 jona      (1000) jona      (1000)       10 2023-03-06 18:20:58.000000 yt_ripper-0.0.8/yt_ripper.egg-info/top_level.txt
+drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-05-08 21:02:21.471053 yt_ripper-0.0.9/
+-rw-r--r--   0 jona      (1000) jona      (1000)     1702 2023-05-08 21:02:21.471053 yt_ripper-0.0.9/PKG-INFO
+-rw-r--r--   0 jona      (1000) jona      (1000)     1150 2023-03-06 18:23:15.000000 yt_ripper-0.0.9/README.md
+-rw-r--r--   0 jona      (1000) jona      (1000)       38 2023-05-08 21:02:21.471053 yt_ripper-0.0.9/setup.cfg
+-rw-r--r--   0 jona      (1000) jona      (1000)      962 2023-05-08 20:57:53.000000 yt_ripper-0.0.9/setup.py
+drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-05-08 21:02:21.470053 yt_ripper-0.0.9/yt_ripper/
+-rw-r--r--   0 jona      (1000) jona      (1000)        0 2023-03-06 18:02:56.000000 yt_ripper-0.0.9/yt_ripper/__init__.py
+drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-05-08 21:02:21.471053 yt_ripper-0.0.9/yt_ripper/cli/
+-rw-r--r--   0 jona      (1000) jona      (1000)        0 2023-03-06 17:41:26.000000 yt_ripper-0.0.9/yt_ripper/cli/__init__.py
+-rw-r--r--   0 jona      (1000) jona      (1000)      332 2023-03-06 17:41:26.000000 yt_ripper-0.0.9/yt_ripper/cli/loading.py
+-rw-r--r--   0 jona      (1000) jona      (1000)     1111 2023-03-06 18:19:57.000000 yt_ripper-0.0.9/yt_ripper/cli/menu.py
+-rw-r--r--   0 jona      (1000) jona      (1000)     1784 2023-05-08 20:48:05.000000 yt_ripper-0.0.9/yt_ripper/cli/youtube.py
+-rw-r--r--   0 jona      (1000) jona      (1000)     2519 2023-03-06 18:14:01.000000 yt_ripper-0.0.9/yt_ripper/main.py
+drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-05-08 21:02:21.471053 yt_ripper-0.0.9/yt_ripper/path/
+-rw-r--r--   0 jona      (1000) jona      (1000)        0 2023-03-06 17:41:26.000000 yt_ripper-0.0.9/yt_ripper/path/__init__.py
+-rw-r--r--   0 jona      (1000) jona      (1000)      429 2023-03-06 17:41:26.000000 yt_ripper-0.0.9/yt_ripper/path/utils.py
+drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2023-05-08 21:02:21.470053 yt_ripper-0.0.9/yt_ripper.egg-info/
+-rw-r--r--   0 jona      (1000) jona      (1000)     1702 2023-05-08 21:02:21.000000 yt_ripper-0.0.9/yt_ripper.egg-info/PKG-INFO
+-rw-r--r--   0 jona      (1000) jona      (1000)      407 2023-05-08 21:02:21.000000 yt_ripper-0.0.9/yt_ripper.egg-info/SOURCES.txt
+-rw-r--r--   0 jona      (1000) jona      (1000)        1 2023-05-08 21:02:21.000000 yt_ripper-0.0.9/yt_ripper.egg-info/dependency_links.txt
+-rw-r--r--   0 jona      (1000) jona      (1000)       49 2023-05-08 21:02:21.000000 yt_ripper-0.0.9/yt_ripper.egg-info/entry_points.txt
+-rw-r--r--   0 jona      (1000) jona      (1000)       21 2023-05-08 21:02:21.000000 yt_ripper-0.0.9/yt_ripper.egg-info/requires.txt
+-rw-r--r--   0 jona      (1000) jona      (1000)       10 2023-05-08 21:02:21.000000 yt_ripper-0.0.9/yt_ripper.egg-info/top_level.txt
```

### Comparing `yt_ripper-0.0.8/PKG-INFO` & `yt_ripper-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_ripper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Project with Python to download videos and mp3 files of youtube in the terminal
 Home-page: https://github.com/atticus64/yt_ripper
 Author: Jonathani Atticus64
 Author-email: jonaenglish64@gmail.com
 Keywords: youtube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,14 +46,20 @@
 pacman -R ffmpeg4.0
 ```
 And verify you have ffmpeg with:
 ```
 ffmpeg --version
 ```
 
+## Installation 
+
+```
+pip install yt_ripper
+```
+
 ## Init virtual env
 
 ```bash
 python3 -m venv .env
 ```
 
 ## install Dependencies
```

### Comparing `yt_ripper-0.0.8/README.md` & `yt_ripper-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 pacman -R ffmpeg4.0
 ```
 And verify you have ffmpeg with:
 ```
 ffmpeg --version
 ```
 
+## Installation 
+
+```
+pip install yt_ripper
+```
+
 ## Init virtual env
 
 ```bash
 python3 -m venv .env
 ```
 
 ## install Dependencies
```

### Comparing `yt_ripper-0.0.8/setup.py` & `yt_ripper-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     README = f.read()
 
 setuptools.setup(
     name="yt_ripper",
-    version="0.0.8",
+    version="0.0.9",
     author="Jonathani Atticus64",
     author_email="jonaenglish64@gmail.com",
     description="Project with Python to download videos and mp3 files of youtube in the terminal", 
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/atticus64/yt_ripper",
     packages=setuptools.find_packages(),
```

### Comparing `yt_ripper-0.0.8/yt_ripper/cli/menu.py` & `yt_ripper-0.0.9/yt_ripper/cli/menu.py`

 * *Files identical despite different names*

### Comparing `yt_ripper-0.0.8/yt_ripper/cli/youtube.py` & `yt_ripper-0.0.9/yt_ripper/cli/youtube.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from yt_ripper.cli.loading import loading_bar
 
 def get_url():
     url = input(Fore.LIGHTWHITE_EX + "Url: " + Fore.LIGHTYELLOW_EX + "")
     return url
 
 def download_video(url, path):
-    yt = YouTube(url)
+    yt = YouTube(url, use_oauth=True , allow_oauth_cache=True)
     print(Fore.BLUE + "Fetching Video")
-    yt.streams.filter(progressive=True, file_extension="mp4").first().download(
-        path
-    )
+    yt.streams.get_highest_resolution().download(path)
+    # filter(progressive=True, file_extension="mp4").first().download(
+    #     path
+    # )
     loading_bar('Downloading video')
     print(Fore.LIGHTBLUE_EX + "Download Finish :D")
 
 def download_audio_win(yt, path):
     print(Fore.BLUE + "Downloading Audio")
     video = yt.streams.filter(only_audio=True).first()
     fileDownloaded = video.download(path)
```

### Comparing `yt_ripper-0.0.8/yt_ripper/main.py` & `yt_ripper-0.0.9/yt_ripper/main.py`

 * *Files identical despite different names*

### Comparing `yt_ripper-0.0.8/yt_ripper.egg-info/PKG-INFO` & `yt_ripper-0.0.9/yt_ripper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-ripper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Project with Python to download videos and mp3 files of youtube in the terminal
 Home-page: https://github.com/atticus64/yt_ripper
 Author: Jonathani Atticus64
 Author-email: jonaenglish64@gmail.com
 Keywords: youtube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,14 +46,20 @@
 pacman -R ffmpeg4.0
 ```
 And verify you have ffmpeg with:
 ```
 ffmpeg --version
 ```
 
+## Installation 
+
+```
+pip install yt_ripper
+```
+
 ## Init virtual env
 
 ```bash
 python3 -m venv .env
 ```
 
 ## install Dependencies
```

