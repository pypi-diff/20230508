# Comparing `tmp/xhs-0.1.7.tar.gz` & `tmp/xhs-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.7.tar", last modified: Sat May  6 08:03:41 2023, max compression
+gzip compressed data, was "xhs-0.1.8.tar", last modified: Mon May  8 03:51:06 2023, max compression
```

## Comparing `xhs-0.1.7.tar` & `xhs-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:03:41.943554 xhs-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-06 08:03:25.000000 xhs-0.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-06 08:03:25.000000 xhs-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 08:03:25.000000 xhs-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-06 08:03:41.943554 xhs-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-06 08:03:25.000000 xhs-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 08:03:25.000000 xhs-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 08:03:41.943554 xhs-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-06 08:03:25.000000 xhs-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:03:41.943554 xhs-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-06 08:03:25.000000 xhs-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-06 08:03:25.000000 xhs-0.1.7/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-06 08:03:25.000000 xhs-0.1.7/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 08:03:25.000000 xhs-0.1.7/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:03:41.943554 xhs-0.1.7/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 08:03:25.000000 xhs-0.1.7/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-06 08:03:25.000000 xhs-0.1.7/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-05-06 08:03:25.000000 xhs-0.1.7/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-06 08:03:25.000000 xhs-0.1.7/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-06 08:03:25.000000 xhs-0.1.7/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:03:41.943554 xhs-0.1.7/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-06 08:03:41.000000 xhs-0.1.7/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-06 08:03:41.000000 xhs-0.1.7/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:03:41.000000 xhs-0.1.7/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:03:41.000000 xhs-0.1.7/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 08:03:41.000000 xhs-0.1.7/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 08:03:41.000000 xhs-0.1.7/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-08 03:50:52.000000 xhs-0.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 03:50:52.000000 xhs-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 03:50:52.000000 xhs-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 03:51:06.000518 xhs-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-08 03:50:52.000000 xhs-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 03:50:52.000000 xhs-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 03:51:06.000518 xhs-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-08 03:50:52.000000 xhs-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.7/CHANGELOG.md` & `xhs-0.1.8/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.8
+
+### Added
+
+- add get img and video to help
+
+### Changed
+
+- change get_img_url to help
+
 ## 0.1.7
 
 ### Fixed
 
 - client init without cookie will casue a exception
 
 ### Added
```

### Comparing `xhs-0.1.7/LICENSE` & `xhs-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.7/setup.py` & `xhs-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.7/tests/__init__.py` & `xhs-0.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.7/tests/test_help.py` & `xhs-0.1.8/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.7/tests/test_xhs.py` & `xhs-0.1.8/tests/test_xhs.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.7/xhs/core.py` & `xhs-0.1.8/xhs/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from typing import NamedTuple
 
 import requests
 
 from xhs.exception import DataFetchError, IPBlockError
 
 from .help import (cookie_jar_to_cookie_str, cookie_str_to_cookie_dict,
-                   get_search_id, sign, update_session_cookies_from_cookie)
+                   download_file, get_imgs_url_from_note, get_search_id,
+                   get_valid_path_name, get_video_url_from_note, sign,
+                   update_session_cookies_from_cookie)
 
 
 class FeedType(Enum):
     # 推荐
     RECOMMEND = "homefeed_recommend"
     # 穿搭
     FASION = "homefeed.fashion_v3"
@@ -80,26 +82,14 @@
     comment_count: str
     liked_count: str
     share_count: str
     time: int
     last_update_time: int
 
 
-def download_file(url: str, filename: str):
-    with requests.get(url, stream=True) as r:
-        r.raise_for_status()
-        with open(filename, 'wb') as f:
-            for chunk in r.iter_content(chunk_size=8192):
-                f.write(chunk)
-
-
-def get_img_url_by_trace_id(trace_id: str):
-    return f"https://sns-img-bd.xhscdn.com/{trace_id}?imageView2/format/png"
-
-
 class XhsClient:
     def __init__(self,
                  cookie=None,
                  user_agent=None,
                  timeout=10,
                  proxies=None):
         """constructor"""
@@ -230,18 +220,16 @@
 
         :param note_id: note_id that you want to fetch
         :type note_id: str
         :param dir_path: in fact, files will be stored in your dir_path/note_title directory
         :type dir_path: str
         """
         note = self.get_note_by_id(note_id)
-        title = note["title"]
 
-        invalid_chars = '<>:"/\\|?*'
-        title = re.sub('[{}]'.format(re.escape(invalid_chars)), '_', title)
+        title = get_valid_path_name(note["title"])
 
         if not title:
             title = note_id
 
         new_dir_path = os.path.join(dir_path, title)
         if not os.path.exists(new_dir_path):
             os.mkdir(new_dir_path)
@@ -252,39 +240,14 @@
             download_file(video_url, video_filename)
         else:
             img_urls = self._get_img_urls_from_note(note)
             for index, img_url in enumerate(img_urls):
                 img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
                 download_file(img_url, img_file_name)
 
-    def _get_img_urls_from_note(self, note) -> list:
-        """get all no watermark img url from note
-
-        :param note: note info
-        :type note: dict
-        :return: images url list
-        :rtype: list
-        """
-        imgs = note["image_list"]
-        if not len(imgs):
-            return []
-        return [get_img_url_by_trace_id(img["trace_id"]) for img in imgs]
-
-    def _get_video_url_from_note(self, note) -> str:
-        """find video url from note
-
-        :param note: note info
-        :type note: dict
-        :return: video url
-        :rtype: str
-        """
-        if not note.get("video"):
-            return ""
-        return f"http://sns-video-bd.xhscdn.com/{note['video']['consumer']['origin_video_key']}"
-
     def get_self_info(self):
         uri = "/api/sns/web/v1/user/selfinfo"
         res = self.get(uri)
         return res
 
     def get_user_info(self, user_id: str):
         """
@@ -385,16 +348,16 @@
                 interact_info = note["interact_info"]
                 note_info = Note(
                     note_id=note["note_id"],
                     title=note["title"],
                     desc=note["desc"],
                     type=note["type"],
                     user=note["user"],
-                    img_urls=self._get_img_urls_from_note(note),
-                    video_url=self._get_video_url_from_note(note),
+                    img_urls=get_imgs_url_from_note(note),
+                    video_url=get_video_url_from_note(note),
                     tag_list=note["tag_list"],
                     at_user_list=note["at_user_list"],
                     collected_count=interact_info["collected_count"],
                     comment_count=interact_info["comment_count"],
                     liked_count=interact_info["liked_count"],
                     share_count=interact_info["share_count"],
                     time=note["time"],
```

### Comparing `xhs-0.1.7/xhs/help.py` & `xhs-0.1.8/xhs/help.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import binascii
 import ctypes
 import hashlib
 import json
 import random
+import re
 import string
 import time
 import urllib.parse
 
 import requests
 
 
@@ -56,14 +57,93 @@
     return {
         "x-s": x_s,
         "x-t": x_t,
         "x-s-common": x_s_common,
     }
 
 
+def get_a1_and_web_id():
+    """generate a1 and webid cookie str, the first return value is a1, second is webId
+
+    for example: a1, web_id = get_a1_and_web_id()
+    """
+    def random_str(length):
+        alphabet = string.ascii_letters + string.digits
+        return ''.join(random.choice(alphabet) for _ in range(length))
+
+    d = hex(int(time.time() * 1000))[2:] + random_str(30) + "5" + "0" + "000"
+    g = (d + str(binascii.crc32(str(d).encode('utf-8'))))[:52]
+    return g, hashlib.md5(g.encode('utf-8')).hexdigest()
+
+
+img_cdns = [
+    "https://sns-img-qc.xhscdn.com",
+    "https://sns-img-hw.xhscdn.com",
+    "https://sns-img-bd.xhscdn.com",
+    "https://sns-img-qn.xhscdn.com",
+]
+
+
+def get_img_url_by_trace_id(trace_id: str, format: str = "png"):
+    return f"{random.choice(img_cdns)}/{trace_id}?imageView2/format/{format}"
+
+
+def get_img_urls_by_trace_id(trace_id: str, format: str = "png"):
+    return [f"{cdn}/{trace_id}?imageView2/format/{format}" for cdn in img_cdns]
+
+
+def get_imgs_url_from_note(note) -> list:
+    """the return type is [img1_url, img2_url, ...]"""
+    imgs = note["image_list"]
+    if not len(imgs):
+        return []
+    return [get_img_url_by_trace_id(img["trace_id"]) for img in imgs]
+
+
+def get_imgs_urls_from_note(note) -> list:
+    """the return type is [[img1_url1, img1_url2, img1_url3], [img2_url, img2_url2, img2_url3], ...]"""
+    imgs = note["image_list"]
+    if not len(imgs):
+        return []
+    return [get_img_urls_by_trace_id(img["trace_id"]) for img in imgs]
+
+
+video_cdns = [
+    "https://sns-video-qc.xhscdn.com",
+    "https://sns-video-hw.xhscdn.com",
+    "https://sns-video-bd.xhscdn.com",
+    "https://sns-video-qn.xhscdn.com",
+]
+
+
+def get_video_url_from_note(note) -> str:
+    if not note.get("video"):
+        return ""
+    origin_video_key = note['video']['consumer']['origin_video_key']
+    return f"{random.choice(video_cdns)}/{origin_video_key}"
+
+
+def get_video_urls_from_note(note) -> list:
+    origin_video_key = note['video']['consumer']['origin_video_key']
+    return [f"{cdn}/{origin_video_key}?imageView2/format/{format}" for cdn in video_cdns]
+
+
+def download_file(url: str, filename: str):
+    with requests.get(url, stream=True) as r:
+        r.raise_for_status()
+        with open(filename, 'wb') as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
+
+
+def get_valid_path_name(text):
+    invalid_chars = '<>:"/\\|?*'
+    return re.sub('[{}]'.format(re.escape(invalid_chars)), '_', text)
+
+
 def mrc(e):
     ie = [
         0, 1996959894, 3993919788, 2567524794, 124634137, 1886057615, 3915621685,
         2657392035, 249268274, 2044508324, 3772115230, 2547177864, 162941995,
         2125561021, 3887607047, 2428444049, 498536548, 1789927666, 4089016648,
         2227061214, 450548861, 1843258603, 4107580753, 2211677639, 325883990,
         1684777152, 4251122042, 2321926636, 335633487, 1661365465, 4195302755,
@@ -114,28 +194,14 @@
         return (val + (MAX32INT + 1)) % (2 * (MAX32INT + 1)) - MAX32INT - 1
 
     for n in range(57):
         o = ie[(o & 255) ^ ord(e[n])] ^ right_without_sign(o, 8)
     return o ^ -1 ^ 3988292384
 
 
-def get_a1_and_web_id():
-    """generate a1 and webid cookie str, the first return value is a1, second is webId
-
-    for example: a1, web_id = get_a1_and_web_id()
-    """
-    def random_str(length):
-        alphabet = string.ascii_letters + string.digits
-        return ''.join(random.choice(alphabet) for _ in range(length))
-
-    d = hex(int(time.time() * 1000))[2:] + random_str(30) + "5" + "0" + "000"
-    g = (d + str(binascii.crc32(str(d).encode('utf-8'))))[:52]
-    return g, hashlib.md5(g.encode('utf-8')).hexdigest()
-
-
 lookup = [
     "Z",
     "m",
     "s",
     "e",
     "r",
     "b",
```

