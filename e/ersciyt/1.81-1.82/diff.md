# Comparing `tmp/ersciyt-1.81.tar.gz` & `tmp/ersciyt-1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.81.tar", last modified: Sun May  7 12:42:35 2023, max compression
+gzip compressed data, was "ersciyt-1.82.tar", last modified: Sun May  7 21:37:31 2023, max compression
```

## Comparing `ersciyt-1.81.tar` & `ersciyt-1.82.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.230172 ersciyt-1.81/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-07 12:42:12.000000 ersciyt-1.81/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-07 12:42:12.000000 ersciyt-1.81/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      796 2023-05-07 12:42:35.230172 ersciyt-1.81/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-07 12:42:12.000000 ersciyt-1.81/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.228172 ersciyt-1.81/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.229172 ersciyt-1.81/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.230172 ersciyt-1.81/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     6901 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.229172 ersciyt-1.81/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      796 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-07 12:42:35.231173 ersciyt-1.81/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-07 12:42:12.000000 ersciyt-1.81/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 21:37:31.337403 ersciyt-1.82/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-07 21:37:23.000000 ersciyt-1.82/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-07 21:37:23.000000 ersciyt-1.82/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      796 2023-05-07 21:37:31.337403 ersciyt-1.82/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-07 21:37:23.000000 ersciyt-1.82/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 21:37:31.336403 ersciyt-1.82/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 21:37:31.337403 ersciyt-1.82/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 21:37:31.337403 ersciyt-1.82/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     7341 2023-05-07 21:37:23.000000 ersciyt-1.82/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 21:37:31.337403 ersciyt-1.82/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      796 2023-05-07 21:37:31.000000 ersciyt-1.82/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-07 21:37:31.000000 ersciyt-1.82/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 21:37:31.000000 ersciyt-1.82/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-07 21:37:31.000000 ersciyt-1.82/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-07 21:37:31.000000 ersciyt-1.82/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-07 21:37:31.338403 ersciyt-1.82/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-07 21:37:23.000000 ersciyt-1.82/setup.py
```

### Comparing `ersciyt-1.81/LICENSE` & `ersciyt-1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.81/PKG-INFO` & `ersciyt-1.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.81
+Version: 1.82
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.81/README.md` & `ersciyt-1.82/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.81/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.82/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.81/ersciyt/views.py` & `ersciyt-1.82/ersciyt/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pyqrcode
 import os,subprocess
 from django.http import HttpResponse,FileResponse
 #from youtube_transcript_api import YouTubeTranscriptApi
 #from youtube_transcript_api.formatters import WebVTTFormatter
 #pip install googletrans==4.0.0-rc1
 #from googletrans import Translator
-import re
+import re,base64
 from django.contrib.staticfiles import finders
 
 
 def ytdwn(request,link):
     try:        
         #os.system('sudo apt-get install -y ffmpeg') 
         os.system('yt-dlp  -f 18 -o a.mp4 https://www.youtube.com/watch?v={}'.format(link))        
@@ -143,28 +143,39 @@
         response['Content-Disposition'] = 'attachment; filename=%s' % fn
         os.remove(media_dir + '/' + file)
         os.remove(media_dir + '/m1.mp3')
         return response
     except:
         return HttpResponse (video.description)
 '''
-
-def helping(request):
+def shqr(request):
     try:
-        qr_code = pyqrcode.create(request.headers['Host'])
+        pic=request.GET['idx']
+        qr_code = pyqrcode.create(pic)#request.headers['HTTP_REFERER'])
         qr_code.svg('a.svg', scale=6)
-        return HttpResponse ('''
+        img=open('a.svg', "r")
+        #image_data = base64.b64encode(img.read()).decode('utf-8')
+        imgdata = "{}".format(img.read())
+        return HttpResponse (imgdata)
+    except:
+        return HttpResponse ('Youtube Url Is Mistake!!!!')
+        
+def helping(request):
+    try:
+        return HttpResponse ('''<!Doctype html><html><head></head><body>
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         enter Youtube ID after YourSiteName address - for play in firefox -  : <br>
         <b>YourSiteName/xazlZh1lTpM</b><br>        
         <a href="/static/ersci_viddown_tab2.xpi">Video download firefox Addon direct link</a><br>
         or<br>
         <a href="https://addons.mozilla.org/en-US/firefox/addon/ersci_viddown_tab2">video download firefox Addon mozilla site link</a>
         <br>
-        <b>{}</b>
-        <img src='{}' />
+        <br>
+        <a href="#" onclick="window.open('/shqr?idx=' + window.location.href);">show QR Code for this site </a>
+        <br>
         </p>
-        '''.format(request.headers['Host'],finders.find('a.svg')))
+        </body></html>
+        ''')
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!')
```

### Comparing `ersciyt-1.81/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.82/ersciyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.81
+Version: 1.82
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.81/setup.cfg` & `ersciyt-1.82/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.81
+version = 1.82
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

