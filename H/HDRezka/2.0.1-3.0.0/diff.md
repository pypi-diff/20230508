# Comparing `tmp/HDRezka-2.0.1.tar.gz` & `tmp/HDRezka-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HDRezka-2.0.1.tar", last modified: Sat Apr 22 04:07:34 2023, max compression
+gzip compressed data, was "HDRezka-3.0.0.tar", last modified: Mon May  8 10:51:33 2023, max compression
```

## Comparing `HDRezka-2.0.1.tar` & `HDRezka-3.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.498551 HDRezka-2.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.438351 HDRezka-2.0.1/HDRezka.egg-info/
--rw-rw-rw-   0        0        0     4446 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     4446 2023-04-22 04:07:34.497551 HDRezka-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-04-19 13:06:04.000000 HDRezka-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.465246 HDRezka-2.0.1/hdrezka/
--rw-rw-rw-   0        0        0      901 2023-04-19 13:04:35.000000 HDRezka-2.0.1/hdrezka/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-04-19 10:05:55.000000 HDRezka-2.0.1/hdrezka/_antiobfuscation.py
--rw-rw-rw-   0        0        0      299 2023-04-08 03:54:33.000000 HDRezka-2.0.1/hdrezka/_bs4.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.470365 HDRezka-2.0.1/hdrezka/api/
--rw-rw-rw-   0        0        0       42 2023-04-06 11:57:13.000000 HDRezka-2.0.1/hdrezka/api/__init__.py
--rw-rw-rw-   0        0        0     1363 2023-04-19 13:10:55.000000 HDRezka-2.0.1/hdrezka/api/ajax.py
--rw-rw-rw-   0        0        0      315 2023-04-06 11:55:17.000000 HDRezka-2.0.1/hdrezka/api/http.py
--rw-rw-rw-   0        0        0     1164 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/api/search.py
--rw-rw-rw-   0        0        0      365 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.478696 HDRezka-2.0.1/hdrezka/post/
--rw-rw-rw-   0        0        0       40 2023-04-06 11:11:48.000000 HDRezka-2.0.1/hdrezka/post/__init__.py
--rw-rw-rw-   0        0        0      110 2023-04-06 11:12:40.000000 HDRezka-2.0.1/hdrezka/post/_dataclass.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.481697 HDRezka-2.0.1/hdrezka/post/info/
--rw-rw-rw-   0        0        0       42 2023-04-02 10:26:20.000000 HDRezka-2.0.1/hdrezka/post/info/__init__.py
--rw-rw-rw-   0        0        0      582 2023-04-06 11:53:58.000000 HDRezka-2.0.1/hdrezka/post/info/fields.py
--rw-rw-rw-   0        0        0     5313 2023-04-19 12:59:55.000000 HDRezka-2.0.1/hdrezka/post/info/info.py
--rw-rw-rw-   0        0        0     3154 2023-04-19 12:53:06.000000 HDRezka-2.0.1/hdrezka/post/page.py
--rw-rw-rw-   0        0        0     2444 2023-04-06 11:57:13.000000 HDRezka-2.0.1/hdrezka/post/post.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.490583 HDRezka-2.0.1/hdrezka/post/urls/
--rw-rw-rw-   0        0        0       61 2023-04-19 12:43:33.000000 HDRezka-2.0.1/hdrezka/post/urls/__init__.py
--rw-rw-rw-   0        0        0      408 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/post/urls/_regexes.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.494551 HDRezka-2.0.1/hdrezka/post/urls/kind/
--rw-rw-rw-   0        0        0       68 2023-04-19 10:43:34.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/__init__.py
--rw-rw-rw-   0        0        0      739 2023-04-19 11:56:29.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/quality.py
--rw-rw-rw-   0        0        0     1448 2023-04-19 12:37:33.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/subtitle.py
--rw-rw-rw-   0        0        0     1975 2023-04-19 12:09:56.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/video.py
--rw-rw-rw-   0        0        0      528 2023-04-19 10:30:04.000000 HDRezka-2.0.1/hdrezka/post/urls/short.py
--rw-rw-rw-   0        0        0      455 2023-04-19 12:43:14.000000 HDRezka-2.0.1/hdrezka/post/urls/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.496553 HDRezka-2.0.1/hdrezka/stream/
--rw-rw-rw-   0        0        0       22 2023-04-03 14:41:41.000000 HDRezka-2.0.1/hdrezka/stream/__init__.py
--rw-rw-rw-   0        0        0     2535 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/stream/player.py
--rw-rw-rw-   0        0        0      387 2023-04-06 11:53:59.000000 HDRezka-2.0.1/hdrezka/translators.py
--rw-rw-rw-   0        0        0       42 2023-04-22 04:07:34.498551 HDRezka-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2007 2023-04-22 04:06:12.000000 HDRezka-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.575274 HDRezka-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.498828 HDRezka-3.0.0/HDRezka.egg-info/
+-rw-rw-rw-   0        0        0     4844 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4844 2023-05-08 10:51:33.574276 HDRezka-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-05-08 10:44:42.000000 HDRezka-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.504842 HDRezka-3.0.0/hdrezka/
+-rw-rw-rw-   0        0        0      910 2023-05-08 10:49:23.000000 HDRezka-3.0.0/hdrezka/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/_antiobfuscation.py
+-rw-rw-rw-   0        0        0      309 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/_bs4.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.508828 HDRezka-3.0.0/hdrezka/api/
+-rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/api/__init__.py
+-rw-rw-rw-   0        0        0     1472 2023-05-08 09:52:32.000000 HDRezka-3.0.0/hdrezka/api/ajax.py
+-rw-rw-rw-   0        0        0      370 2023-05-08 06:08:44.000000 HDRezka-3.0.0/hdrezka/api/http.py
+-rw-rw-rw-   0        0        0      832 2023-05-08 10:49:50.000000 HDRezka-3.0.0/hdrezka/api/search.py
+-rw-rw-rw-   0        0        0      383 2023-05-08 10:49:13.000000 HDRezka-3.0.0/hdrezka/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.522065 HDRezka-3.0.0/hdrezka/post/
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/_dataclass.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.525066 HDRezka-3.0.0/hdrezka/post/info/
+-rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/info/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/info/fields.py
+-rw-rw-rw-   0        0        0     5459 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/info/info.py
+-rw-rw-rw-   0        0        0     2905 2023-05-08 10:49:40.000000 HDRezka-3.0.0/hdrezka/post/page.py
+-rw-rw-rw-   0        0        0     2609 2023-05-08 09:52:32.000000 HDRezka-3.0.0/hdrezka/post/post.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.536023 HDRezka-3.0.0/hdrezka/post/urls/
+-rw-rw-rw-   0        0        0       64 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/_regexes.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.570276 HDRezka-3.0.0/hdrezka/post/urls/kind/
+-rw-rw-rw-   0        0        0       71 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/__init__.py
+-rw-rw-rw-   0        0        0      768 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/quality.py
+-rw-rw-rw-   0        0        0     1490 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/subtitle.py
+-rw-rw-rw-   0        0        0     2037 2023-05-08 10:43:14.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/video.py
+-rw-rw-rw-   0        0        0      553 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/short.py
+-rw-rw-rw-   0        0        0      469 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.573325 HDRezka-3.0.0/hdrezka/stream/
+-rw-rw-rw-   0        0        0       23 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/stream/__init__.py
+-rw-rw-rw-   0        0        0     3458 2023-05-08 10:06:08.000000 HDRezka-3.0.0/hdrezka/stream/player.py
+-rw-rw-rw-   0        0        0      398 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/translators.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:51:33.575274 HDRezka-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2007 2023-05-08 10:08:16.000000 HDRezka-3.0.0/setup.py
```

### Comparing `HDRezka-2.0.1/HDRezka.egg-info/PKG-INFO` & `HDRezka-3.0.0/HDRezka.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 2.0.1
+Version: 3.0.0
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -38,38 +38,50 @@
 # Install
 
 `pip install HDRezka`
 
 # Example
 
 ```python
+import asyncio
 from hdrezka import Search
 
-player = Search('Breaking Bad')[1, 0].player  # page 1 element 0; or just use Player(646)
-print(player.post.info, end='\n\n')
+async def main():
+    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use Player(646)
+    print(player.post.info, end='\n\n')
+
+    translator_id = None  # default
+    for name, id_ in player.post.translators.name_id.items():
+        if 'субтитры' in name.casefold(): translator_id = id_; break
+
+    stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
+    video = stream.video
+    print(video.last_url)  # best quality (.m3u8)
+    print(video[video.min].last_url.mp4, end='\n\n')  # worst quality (.mp4)
 
-translator_id = None  # default
-for name, id_ in player.post.translators.name_id.items():
-    if 'субтитры' in name.casefold(): translator_id = id_; break
-
-stream = player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
-video = stream.video
-print(video.last_url)  # best quality
-print(video[video.min].last_url.mp4, end='\n\n')
+    subtitles = stream.subtitles
+    print(subtitles.default.url)  # subtitles.ru.url or subtitles['Русский'].url
 
-subtitles = stream.subtitles
-print(subtitles.default.url)  # subtitles.ru.url or subtitles['Русский'].url
+if __name__ == '__main__': asyncio.run(main())
 ```
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 3.0.0
+
+- **Now a fully asynchronous package.**
+
+- ### post.page.Page
+    - Implements `__aiter__` and `__anext__` methods that list all the pages found.
+    - Instead of `get_pages`, now only the `get_page` method
+
 ## 2.0.1
 
 - Fixed bug with PIP
 
 ## 2.0.0
 
 Backward incompatible changes have been made
```

### Comparing `HDRezka-2.0.1/HDRezka.egg-info/SOURCES.txt` & `HDRezka-3.0.0/HDRezka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HDRezka-2.0.1/LICENSE` & `HDRezka-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HDRezka-2.0.1/PKG-INFO` & `HDRezka-3.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 2.0.1
+Version: 3.0.0
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -38,38 +38,50 @@
 # Install
 
 `pip install HDRezka`
 
 # Example
 
 ```python
+import asyncio
 from hdrezka import Search
 
-player = Search('Breaking Bad')[1, 0].player  # page 1 element 0; or just use Player(646)
-print(player.post.info, end='\n\n')
+async def main():
+    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use Player(646)
+    print(player.post.info, end='\n\n')
+
+    translator_id = None  # default
+    for name, id_ in player.post.translators.name_id.items():
+        if 'субтитры' in name.casefold(): translator_id = id_; break
+
+    stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
+    video = stream.video
+    print(video.last_url)  # best quality (.m3u8)
+    print(video[video.min].last_url.mp4, end='\n\n')  # worst quality (.mp4)
 
-translator_id = None  # default
-for name, id_ in player.post.translators.name_id.items():
-    if 'субтитры' in name.casefold(): translator_id = id_; break
-
-stream = player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
-video = stream.video
-print(video.last_url)  # best quality
-print(video[video.min].last_url.mp4, end='\n\n')
+    subtitles = stream.subtitles
+    print(subtitles.default.url)  # subtitles.ru.url or subtitles['Русский'].url
 
-subtitles = stream.subtitles
-print(subtitles.default.url)  # subtitles.ru.url or subtitles['Русский'].url
+if __name__ == '__main__': asyncio.run(main())
 ```
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 3.0.0
+
+- **Now a fully asynchronous package.**
+
+- ### post.page.Page
+    - Implements `__aiter__` and `__anext__` methods that list all the pages found.
+    - Instead of `get_pages`, now only the `get_page` method
+
 ## 2.0.1
 
 - Fixed bug with PIP
 
 ## 2.0.0
 
 Backward incompatible changes have been made
```

### Comparing `HDRezka-2.0.1/hdrezka/__init__.py` & `HDRezka-3.0.0/hdrezka/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 `pip install HDRezka`
 
 # Example
 
 ```python
 from hdrezka import Search
 
-player = Search('Breaking Bad')[1, 0].player  # page 1 element 0; or just use Player(646)
+player = Search('Breaking Bad').get_page(1)[0].player  # page 1 element 0; or just use Player(646)
 print(player.post.info, end='\n\n')
 
 translator_id = None  # default
 for name, id_ in player.post.translators.name_id.items():
     if 'субтитры' in name.casefold(): translator_id = id_; break
 
 stream = player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
```

### Comparing `HDRezka-2.0.1/hdrezka/_antiobfuscation.py` & `HDRezka-3.0.0/hdrezka/_antiobfuscation.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import re
-from binascii import a2b_base64
-
-__all__ = ('clear_trash',)
-
-_sub_trash = re.compile(
-    '#h|//_//|I0A=|I0Ah|I0Aj|I0Ak|I0BA|I0Be|I14=|I14h|I14j|I14k|I15A|I15e|ISE=|ISEh|ISEj|ISEk|ISFA|ISFe|ISM=|ISMh'
-    '|ISMj|ISMk|ISNA|ISNe|ISQ=|ISQh|ISQj|ISQk|ISRA|ISRe|IUA=|IUAh|IUAj|IUAk|IUBA|IUBe|IV4=|IV4h|IV4j|IV4k|IV5A|IV5e'
-    '|IyE=|IyEh|IyEj|IyEk|IyFA|IyFe|IyM=|IyMh|IyMj|IyMk|IyNA|IyNe|IyQ=|IyQh|IyQj|IyQk|IyRA|IyRe|JCE=|JCEh|JCEj|JCEk'
-    '|JCFA|JCFe|JCM=|JCMh|JCMj|JCMk|JCNA|JCNe|JCQ=|JCQh|JCQj|JCQk|JCRA|JCRe|JEA=|JEAh|JEAj|JEAk|JEBA|JEBe|JF4=|JF4h'
-    '|JF4j|JF4k|JF5A|JF5e|QCE=|QCEh|QCEj|QCEk|QCFA|QCFe|QCM=|QCMh|QCMj|QCMk|QCNA|QCNe|QCQ=|QCQh|QCQj|QCQk|QCRA|QCRe'
-    '|QEA=|QEAh|QEAj|QEAk|QEBA|QEBe|QF4=|QF4h|QF4j|QF4k|QF5A|QF5e|XiE=|XiEh|XiEj|XiEk|XiFA|XiFe|XiM=|XiMh|XiMj|XiMk'
-    '|XiNA|XiNe|XiQ=|XiQh|XiQj|XiQk|XiRA|XiRe|XkA=|XkAh|XkAj|XkAk|XkBA|XkBe|Xl4=|Xl4h|Xl4j|Xl4k|Xl5A|Xl5e').sub
-
-
-def clear_trash(trash_string: str) -> str:
-    return a2b_base64(b'%b==' % _sub_trash('', trash_string).encode('ASCII')).decode('ASCII')
+import re
+from binascii import a2b_base64
+
+__all__ = ('clear_trash',)
+
+_sub_trash = re.compile(
+    '#h|//_//|I0A=|I0Ah|I0Aj|I0Ak|I0BA|I0Be|I14=|I14h|I14j|I14k|I15A|I15e|ISE=|ISEh|ISEj|ISEk|ISFA|ISFe|ISM=|ISMh'
+    '|ISMj|ISMk|ISNA|ISNe|ISQ=|ISQh|ISQj|ISQk|ISRA|ISRe|IUA=|IUAh|IUAj|IUAk|IUBA|IUBe|IV4=|IV4h|IV4j|IV4k|IV5A|IV5e'
+    '|IyE=|IyEh|IyEj|IyEk|IyFA|IyFe|IyM=|IyMh|IyMj|IyMk|IyNA|IyNe|IyQ=|IyQh|IyQj|IyQk|IyRA|IyRe|JCE=|JCEh|JCEj|JCEk'
+    '|JCFA|JCFe|JCM=|JCMh|JCMj|JCMk|JCNA|JCNe|JCQ=|JCQh|JCQj|JCQk|JCRA|JCRe|JEA=|JEAh|JEAj|JEAk|JEBA|JEBe|JF4=|JF4h'
+    '|JF4j|JF4k|JF5A|JF5e|QCE=|QCEh|QCEj|QCEk|QCFA|QCFe|QCM=|QCMh|QCMj|QCMk|QCNA|QCNe|QCQ=|QCQh|QCQj|QCQk|QCRA|QCRe'
+    '|QEA=|QEAh|QEAj|QEAk|QEBA|QEBe|QF4=|QF4h|QF4j|QF4k|QF5A|QF5e|XiE=|XiEh|XiEj|XiEk|XiFA|XiFe|XiM=|XiMh|XiMj|XiMk'
+    '|XiNA|XiNe|XiQ=|XiQh|XiQj|XiQk|XiRA|XiRe|XkA=|XkAh|XkAj|XkAk|XkBA|XkBe|Xl4=|Xl4h|Xl4j|Xl4k|Xl5A|Xl5e').sub
+
+
+def clear_trash(trash_string: str) -> str:
+    return a2b_base64(b'%b==' % _sub_trash('', trash_string).encode('ASCII')).decode('ASCII')
```

### Comparing `HDRezka-2.0.1/hdrezka/post/info/info.py` & `HDRezka-3.0.0/hdrezka/post/info/info.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import re
-from inspect import getdoc
-from typing import Any
-
-from bs4 import Tag
-
-from .fields import *
-from ..urls import Quality
-from ..._bs4 import BeautifulSoup
-
-__all__ = ('PostInfo',)
-_find_any_digit = re.compile(r'\d+').findall
-
-
-def _get_int(value: Any, /, default: int = 0) -> int:
-    if not isinstance(value, str):
-        value = str(value)
-    if digits := _find_any_digit(value):
-        return int(''.join(digits))
-    return default
-
-
-class PostInfo:
-    __slots__ = ('rating', 'places', 'slogan', 'release', 'country', 'director', 'genre',
-                 'quality', 'translator', 'age_rating', 'duration', 'from_', 'characters',
-                 '_view', 'fields', 'title', 'orig_title', 'poster', 'description')
-    FILL_FIELDS: tuple[str] = __slots__[:13]
-
-    def __init__(self, soup: BeautifulSoup):
-        post_info = soup.find(class_='b-post__info')
-        self.title = soup.find(class_='b-post__title').text.strip()
-        orig_title = soup.find(class_='b-post__origtitle')
-        self.orig_title = orig_title.text.strip() if orig_title else self.title
-        poster = soup.select_one('.b-sidecover>a')
-        self.poster = Poster(poster['href'], poster.find('img')['src'])
-        self.description = soup.find(class_='b-post__description_text').text.strip()
-        self._view = self._form_view(post_info.find_all('tr'))
-
-        raw_fields = post_info.select('tr>td')
-        if len(raw_fields) % 2:
-            raw_fields.append(raw_fields[-1])
-
-        fields = {raw_fields[i].find('h2').text.strip().removesuffix(':'): raw_fields[-~i]
-                  for i in range(0, len(raw_fields), 2)}
-        for field in self.FILL_FIELDS:
-            meth = getattr(self, f'_get_field_{field}', None)
-            field_name = '' if meth is None else (getdoc(meth) or '').strip()
-            item = fields.get(field_name)
-            if not item:
-                setattr(self, field, None)
-                continue
-            processed = meth(item)
-            fields[field_name] = processed
-            setattr(self, field.removeprefix('_get_field_'), processed)
-        self.fields = fields
-
-    @staticmethod
-    def _get_field_rating(tag: Tag) -> dict[str, Rating]:
-        """Рейтинги"""
-        result = {}
-        for span in tag.find_all('span', class_='b-post__info_rates'):
-            classes: list[str] = span.get('class')
-            classes.remove('b-post__info_rates')
-            service = span.find('a').text
-            votes = span.find('i')
-            if votes:
-                votes = _get_int(votes.text)
-            result[classes[0] if classes else service] = Rating(
-                service=service, rating=float(span.find('span').text), votes=votes)
-        return result
-
-    @staticmethod
-    def _get_field_places(tag: Tag) -> tuple[Place]:
-        """Входит в списки"""
-        return *(Place(a.text, _get_int(a.next_element.next_element)) for a in tag.find_all('a')),
-
-    @staticmethod
-    def _get_field_slogan(tag: Tag) -> str:
-        """Слоган"""
-        return tag.get_text(strip=True)
-
-    @staticmethod
-    def _get_field_release(tag: Tag) -> Release:
-        """Дата выхода"""
-        return Release(day=tag.next_element.text.strip(), year=_get_int(tag.find('a').text))
-
-    @staticmethod
-    def _get_field_country(tag: Tag) -> tuple[str]:
-        """Страна"""
-        return *map(str.strip, tag.text.split(',')),
-
-    @staticmethod
-    def _get_field_director(tag: Tag) -> str:
-        """Режиссер"""
-        return tag.get_text(strip=True)
-
-    @staticmethod
-    def _get_field_genre(tag: Tag) -> tuple[str]:
-        """Жанр"""
-        return *map(str.strip, tag.text.split(',')),
-
-    @staticmethod
-    def _get_field_quality(tag: Tag):
-        """В качестве"""
-        return Quality(tag.text.strip())
-
-    @staticmethod
-    def _get_field_translator(tag: Tag) -> str:
-        """В переводе"""
-        return tag.get_text(strip=True)
-
-    @staticmethod
-    def _get_field_age_rating(tag: Tag) -> AgeRating:
-        """Возраст"""
-        return AgeRating(_get_int(span := tag.find('span').next_element), span.next_element.get_text(strip=True))
-
-    @staticmethod
-    def _get_field_duration(tag: Tag) -> Duration:
-        """Время"""
-        return Duration(*tag.text.split(' ', 1))
-
-    @staticmethod
-    def _get_field_from_(tag: Tag) -> tuple[str]:
-        """Из серии"""
-        return *(a.text for a in tag.find_all('a')),
-
-    @staticmethod
-    def _get_field_characters(tag: Tag) -> tuple[str]:
-        """В ролях актеры"""
-        return *(span.text for span in tag.select('span[itemprop="name"]')),
-
-    def _form_view(self, table: list[Tag]) -> str:
-        return '{0}\n\n{1}\n\n{2}'.format(
-            self.title if self.orig_title == self.title else f'{self.title} ({self.orig_title})',
-            '\n'.join(tr.text.replace(')', ') ').strip() for tr in table),
-            self.description
-        )
-
-    def __str__(self):
-        return self._view
-
-    def __repr__(self):
-        # noinspection PyUnboundLocalVariable
-        return f"""{self.__class__.__qualname__}<{', '.join(
-            f'{name}={attr!r}' for name in self.__slots__
-            if not name.startswith('_') and (attr := getattr(self, name)))}>"""
+import re
+from inspect import getdoc
+from typing import Any
+
+from bs4 import Tag
+
+from .fields import *
+from ..urls import Quality
+from ..._bs4 import BeautifulSoup
+
+__all__ = ('PostInfo',)
+_find_any_digit = re.compile(r'\d+').findall
+
+
+def _get_int(value: Any, /, default: int = 0) -> int:
+    if not isinstance(value, str):
+        value = str(value)
+    if digits := _find_any_digit(value):
+        return int(''.join(digits))
+    return default
+
+
+class PostInfo:
+    __slots__ = ('rating', 'places', 'slogan', 'release', 'country', 'director', 'genre',
+                 'quality', 'translator', 'age_rating', 'duration', 'from_', 'characters',
+                 '_view', 'fields', 'title', 'orig_title', 'poster', 'description')
+    FILL_FIELDS: tuple[str] = __slots__[:13]
+
+    def __init__(self, soup: BeautifulSoup):
+        post_info = soup.find(class_='b-post__info')
+        self.title = soup.find(class_='b-post__title').text.strip()
+        orig_title = soup.find(class_='b-post__origtitle')
+        self.orig_title = orig_title.text.strip() if orig_title else self.title
+        poster = soup.select_one('.b-sidecover>a')
+        self.poster = Poster(poster['href'], poster.find('img')['src'])
+        self.description = soup.find(class_='b-post__description_text').text.strip()
+        self._view = self._form_view(post_info.find_all('tr'))
+
+        raw_fields = post_info.select('tr>td')
+        if len(raw_fields) % 2:
+            raw_fields.append(raw_fields[-1])
+
+        fields = {raw_fields[i].find('h2').text.strip().removesuffix(':'): raw_fields[-~i]
+                  for i in range(0, len(raw_fields), 2)}
+        for field in self.FILL_FIELDS:
+            meth = getattr(self, f'_get_field_{field}', None)
+            field_name = '' if meth is None else (getdoc(meth) or '').strip()
+            item = fields.get(field_name)
+            if not item:
+                setattr(self, field, None)
+                continue
+            processed = meth(item)
+            fields[field_name] = processed
+            setattr(self, field.removeprefix('_get_field_'), processed)
+        self.fields = fields
+
+    @staticmethod
+    def _get_field_rating(tag: Tag) -> dict[str, Rating]:
+        """Рейтинги"""
+        result = {}
+        for span in tag.find_all('span', class_='b-post__info_rates'):
+            classes: list[str] = span.get('class')
+            classes.remove('b-post__info_rates')
+            service = span.find('a').text
+            votes = span.find('i')
+            if votes:
+                votes = _get_int(votes.text)
+            result[classes[0] if classes else service] = Rating(
+                service=service, rating=float(span.find('span').text), votes=votes)
+        return result
+
+    @staticmethod
+    def _get_field_places(tag: Tag) -> tuple[Place]:
+        """Входит в списки"""
+        return *(Place(a.text, _get_int(a.next_element.next_element)) for a in tag.find_all('a')),
+
+    @staticmethod
+    def _get_field_slogan(tag: Tag) -> str:
+        """Слоган"""
+        return tag.get_text(strip=True)
+
+    @staticmethod
+    def _get_field_release(tag: Tag) -> Release:
+        """Дата выхода"""
+        return Release(day=tag.next_element.text.strip(), year=_get_int(tag.find('a').text))
+
+    @staticmethod
+    def _get_field_country(tag: Tag) -> tuple[str]:
+        """Страна"""
+        return *map(str.strip, tag.text.split(',')),
+
+    @staticmethod
+    def _get_field_director(tag: Tag) -> str:
+        """Режиссер"""
+        return tag.get_text(strip=True)
+
+    @staticmethod
+    def _get_field_genre(tag: Tag) -> tuple[str]:
+        """Жанр"""
+        return *map(str.strip, tag.text.split(',')),
+
+    @staticmethod
+    def _get_field_quality(tag: Tag):
+        """В качестве"""
+        return Quality(tag.text.strip())
+
+    @staticmethod
+    def _get_field_translator(tag: Tag) -> str:
+        """В переводе"""
+        return tag.get_text(strip=True)
+
+    @staticmethod
+    def _get_field_age_rating(tag: Tag) -> AgeRating:
+        """Возраст"""
+        return AgeRating(_get_int(span := tag.find('span').next_element), span.next_element.get_text(strip=True))
+
+    @staticmethod
+    def _get_field_duration(tag: Tag) -> Duration:
+        """Время"""
+        return Duration(*tag.text.split(' ', 1))
+
+    @staticmethod
+    def _get_field_from_(tag: Tag) -> tuple[str]:
+        """Из серии"""
+        return *(a.text for a in tag.find_all('a')),
+
+    @staticmethod
+    def _get_field_characters(tag: Tag) -> tuple[str]:
+        """В ролях актеры"""
+        return *(span.text for span in tag.select('span[itemprop="name"]')),
+
+    def _form_view(self, table: list[Tag]) -> str:
+        return '{0}\n\n{1}\n\n{2}'.format(
+            self.title if self.orig_title == self.title else f'{self.title} ({self.orig_title})',
+            '\n'.join(tr.text.replace(')', ') ').strip() for tr in table),
+            self.description
+        )
+
+    def __str__(self):
+        return self._view
+
+    def __repr__(self):
+        # noinspection PyUnboundLocalVariable
+        return f"""{self.__class__.__qualname__}<{', '.join(
+            f'{name}={attr!r}' for name in self.__slots__
+            if not name.startswith('_') and (attr := getattr(self, name)))}>"""
```

### Comparing `HDRezka-2.0.1/hdrezka/post/post.py` & `HDRezka-3.0.0/hdrezka/post/post.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-from .info import PostInfo
-from .urls import long_url, short_url
-from .._bs4 import BeautifulSoup
-from ..api.http import get_response
-from ..translators import Translators
-
-__all__ = ('Post',)
-
-
-class Post:
-    """Stores information about the post"""
-    __slots__ = ('url', 'translator_id', 'id', 'name', 'type', 'info', 'translators', 'other_parts_urls',
-                 '_soup_inst')
-
-    def __init__(self, url: str):
-        url = long_url(url)
-        _response = get_response('GET', url)
-        if _response.status_code in {301, 302}:  # redirect
-            _response = get_response('GET', _response.url.join(_response.headers['location']))
-        _response = _response.text
-        self.url = url
-        self._soup_inst = BeautifulSoup(_response)
-        self.type = self._get_type()
-
-        self.translator_id = int(i) if (i := _response.split(
-            'sof.tv.' + {'tv_series': 'initCDNSeriesEvents', 'movie': 'initCDNMoviesEvents'}[self.type],
-            1)[-1].split(',')[1].strip()).isnumeric() else None
-        self.info = self._get_post_info()
-        self.translators = self._get_translators()
-
-        self.id = self._extract_id()
-        self.name = self._get_name()
-        self.other_parts_urls = self._parts_urls
-
-    def _extract_id(self) -> int:
-        return int(self._soup_inst.find(id='post_id')['value'])
-
-    def _get_name(self) -> str:
-        return self._soup_inst.find(class_='b-post__title').text.strip()
-
-    def _get_type(self) -> str:
-        return self._soup_inst.find('meta', property='og:type')['content'].removeprefix('video.')
-
-    def _get_post_info(self) -> PostInfo:
-        return PostInfo(self._soup_inst)
-
-    def _get_translators(self) -> Translators:
-        translators_list = self._soup_inst.find(id='translators-list')
-        arr = {child.text.strip(): int(child['data-translator_id']) for child in
-               translators_list.find_all(recursive=False) if child.text} if translators_list else {}
-        if not arr:
-            arr[self.info.translator] = self.translator_id
-        return Translators(arr)
-
-    @property
-    def _parts_urls(self) -> tuple[str]:
-        self.other_parts_urls = *(
-            i.attrs['data-url'] for i in
-            self._soup_inst.select('.b-post__partcontent_item[data-url]')),
-        return *map(short_url, self.other_parts_urls),
-
-    def __repr__(self):
-        return f'{self.__class__.__qualname__}<{self.name!r}; {self.type!r}>'
+from .info import PostInfo
+from .urls import long_url, short_url
+from .._bs4 import BeautifulSoup
+from ..api.http import get_response
+from ..translators import Translators
+
+__all__ = ('Post',)
+
+
+class Post:
+    """Stores information about the post"""
+    __slots__ = ('url', 'translator_id', 'id', 'name', 'type', 'info', 'translators', 'other_parts_urls',
+                 '_soup_inst')
+
+    def __init__(self, url: str):
+        """Also you should call the `ainit` method"""
+        url = long_url(url)
+        self.url = url
+
+    async def ainit(self):
+        _response = await get_response('GET', self.url)
+        if _response.status_code in {301, 302}:  # redirect
+            _response = await get_response('GET', _response.url.join(_response.headers['location']))
+        _response = _response.text
+        self._soup_inst = BeautifulSoup(_response)
+        self.type = self._get_type()
+
+        self.translator_id = int(i) if (i := _response.split(
+            'sof.tv.' + {'tv_series': 'initCDNSeriesEvents', 'movie': 'initCDNMoviesEvents'}[self.type],
+            1)[-1].split(',')[1].strip()).isnumeric() else None
+        self.info = self._get_post_info()
+        self.translators = self._get_translators()
+
+        self.id = self._extract_id()
+        self.name = self._get_name()
+        self.other_parts_urls = self._parts_urls
+
+    def _extract_id(self) -> int:
+        return int(self._soup_inst.find(id='post_id')['value'])
+
+    def _get_name(self) -> str:
+        return self._soup_inst.find(class_='b-post__title').text.strip()
+
+    def _get_type(self) -> str:
+        return self._soup_inst.find('meta', property='og:type')['content'].removeprefix('video.')
+
+    def _get_post_info(self) -> PostInfo:
+        return PostInfo(self._soup_inst)
+
+    def _get_translators(self) -> Translators:
+        translators_list = self._soup_inst.find(id='translators-list')
+        arr = {child.text.strip(): int(child['data-translator_id']) for child in
+               translators_list.find_all(recursive=False) if child.text} if translators_list else {}
+        if not arr:
+            arr[self.info.translator] = self.translator_id
+        return Translators(arr)
+
+    @property
+    def _parts_urls(self) -> tuple[str]:
+        self.other_parts_urls = *(
+            i.attrs['data-url'] for i in
+            self._soup_inst.select('.b-post__partcontent_item[data-url]')),
+        return *map(short_url, self.other_parts_urls),
+
+    def __repr__(self):
+        return f'{self.__class__.__qualname__}<{self.name!r}; {self.type!r}>'
```

### Comparing `HDRezka-2.0.1/hdrezka/post/urls/kind/quality.py` & `HDRezka-3.0.0/hdrezka/post/urls/kind/quality.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .._regexes import match_quality_int
-
-__all__ = ('Quality',)
-
-
-class Quality(str):
-    __slots__ = ('_i', 'addon')
-    addon: str  # can contain 'ultra'
-
-    def __init__(self, *_, **__):
-        _i = match_quality_int(self)
-        if not _i:
-            raise ValueError(f'{self!r} is not quality.')
-        _i, self.addon = _i.groups()
-        self.addon = self.addon.casefold()
-        self._i = int(_i)
-
-    def __int__(self):
-        """
-        returns pixels height
-        """
-        return self._i
-
-    def __lt__(self, other):
-        if not isinstance(other, self.__class__):
-            return super().__le__(other)
-        if not (self.addon or other.addon):
-            return self._i < int(other)
-        return False
+from .._regexes import match_quality_int
+
+__all__ = ('Quality',)
+
+
+class Quality(str):
+    __slots__ = ('_i', 'addon')
+    addon: str  # can contain 'ultra'
+
+    def __init__(self, *_, **__):
+        _i = match_quality_int(self)
+        if not _i:
+            raise ValueError(f'{self!r} is not quality.')
+        _i, self.addon = _i.groups()
+        self.addon = self.addon.casefold()
+        self._i = int(_i)
+
+    def __int__(self):
+        """
+        returns pixels height
+        """
+        return self._i
+
+    def __lt__(self, other):
+        if not isinstance(other, self.__class__):
+            return super().__le__(other)
+        if not (self.addon or other.addon):
+            return self._i < int(other)
+        return False
```

### Comparing `HDRezka-2.0.1/hdrezka/post/urls/kind/subtitle.py` & `HDRezka-3.0.0/hdrezka/post/urls/kind/subtitle.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from .._regexes import findall_subtitles
-from ..._dataclass import frozen_slots_dataclass
-
-__all__ = ('SubtitleURL', 'SubtitleURLs')
-
-
-@frozen_slots_dataclass
-class SubtitleURL:
-    url: str
-    # language:
-    name: str
-    code: str
-
-
-class SubtitleURLs:
-    __slots__ = ('subtitles', 'has_subtitles', 'subtitle_names', 'subtitle_codes', 'default')
-
-    def __init__(self, subtitle: str | bool, subtitle_lns: dict[str, str] | bool, subtitle_def: str | bool):
-        self.has_subtitles = not subtitle
-        if not subtitle_lns:
-            subtitle_lns = {'off': ''}
-        self.subtitles: tuple[SubtitleURL] = *(
-            SubtitleURL(url, name, subtitle_lns[name]) for name, url in findall_subtitles(subtitle or '')),
-        self.subtitles += SubtitleURL('', '', 'off'),
-        self.subtitle_names = {}
-        self.subtitle_codes = {}
-        for subtitle in self.subtitles:
-            self.subtitle_names[subtitle.name] = self.subtitle_codes[subtitle.code] = subtitle
-
-        self.default: SubtitleURL | None = self.subtitle_codes.get(subtitle_def)
-
-    def __getitem__(self, item: str) -> SubtitleURL | None:
-        return self.subtitle_names.get(item, self.subtitle_codes.get(item))
-
-    def __getattr__(self, item: str) -> SubtitleURL:
-        return self.subtitle_codes[item]
-
-    def __bool__(self):
-        return self.has_subtitles
-
-    def __repr__(self):
-        return f'{self.__class__.__qualname__}<{self.subtitles!r}>'
+from .._regexes import findall_subtitles
+from ..._dataclass import frozen_slots_dataclass
+
+__all__ = ('SubtitleURL', 'SubtitleURLs')
+
+
+@frozen_slots_dataclass
+class SubtitleURL:
+    url: str
+    # language:
+    name: str
+    code: str
+
+
+class SubtitleURLs:
+    __slots__ = ('subtitles', 'has_subtitles', 'subtitle_names', 'subtitle_codes', 'default')
+
+    def __init__(self, subtitle: str | bool, subtitle_lns: dict[str, str] | bool, subtitle_def: str | bool):
+        self.has_subtitles = not subtitle
+        if not subtitle_lns:
+            subtitle_lns = {'off': ''}
+        self.subtitles: tuple[SubtitleURL] = *(
+            SubtitleURL(url, name, subtitle_lns[name]) for name, url in findall_subtitles(subtitle or '')),
+        self.subtitles += SubtitleURL('', '', 'off'),
+        self.subtitle_names = {}
+        self.subtitle_codes = {}
+        for subtitle in self.subtitles:
+            self.subtitle_names[subtitle.name] = self.subtitle_codes[subtitle.code] = subtitle
+
+        self.default: SubtitleURL | None = self.subtitle_codes.get(subtitle_def)
+
+    def __getitem__(self, item: str) -> SubtitleURL | None:
+        return self.subtitle_names.get(item, self.subtitle_codes.get(item))
+
+    def __getattr__(self, item: str) -> SubtitleURL:
+        return self.subtitle_codes[item]
+
+    def __bool__(self):
+        return self.has_subtitles
+
+    def __repr__(self):
+        return f'{self.__class__.__qualname__}<{self.subtitles!r}>'
```

### Comparing `HDRezka-2.0.1/hdrezka/post/urls/kind/video.py` & `HDRezka-3.0.0/hdrezka/post/urls/kind/video.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import Iterable, SupportsInt
-
-from .quality import Quality
-from .._regexes import findall_qualities
-from ...._antiobfuscation import clear_trash
-
-__all__ = ('VideoURL', 'VideoURLs')
-
-
-class VideoURL(str):
-    __slots__ = ('mp4',)
-
-    def __init__(self, *_, **__):
-        self.mp4 = self.removesuffix('8').removesuffix(':hls:manifest.m3u')
-
-
-class VideoURLs:
-    __slots__ = ('raw_data', 'qualities', 'min')
-
-    def __init__(self, data: str | dict):
-        self.raw_data: dict[Quality, VideoURL] = (
-            {Quality(q): VideoURL(u) for q, u in findall_qualities(clear_trash(data))}
-            if isinstance(data, str) else data)
-        self.qualities: tuple[Quality] = *sorted(self.raw_data),
-        self.min = int(self.qualities[0]) if self.qualities else 1
-
-    @property
-    def last_url(self) -> VideoURL:
-        return self[-1].raw_data.popitem()[1]
-
-    def __getitem__(self, item: str | SupportsInt | Iterable | slice):
-        isiter = False
-        if not isinstance(item, str):
-            if isinstance(item, slice):
-                item = item.start, item.stop, item.step
-            isiter = isinstance(item, Iterable) and item
-        if isiter:
-            result = self
-            for part in item:
-                if part is not None:
-                    result = result[part]
-            result = result.raw_data
-        elif isinstance(item, int):
-            if item < self.min:
-                item = self.qualities[item]
-                result = {item: self.raw_data[item]}
-            else:
-                result = {q: v for q, v in self.raw_data.items() if int(q) == item}
-        elif isinstance(item, str):
-            item = item.casefold()
-            result = {q: v for q, v in self.raw_data.items() if q.addon == item}
-        else:
-            raise TypeError(f'Invalid type {type(item)}')
-        return self.__class__(result)
-
-    def __repr__(self):
-        return f"{self.__class__.__qualname__}({self.raw_data})"
+from typing import Iterable, SupportsInt
+
+from .quality import Quality
+from .._regexes import findall_qualities
+from ...._antiobfuscation import clear_trash
+
+__all__ = ('VideoURL', 'VideoURLs')
+
+
+class VideoURL(str):
+    __slots__ = ('mp4',)
+
+    def __init__(self, *_, **__):
+        self.mp4 = str(self.removesuffix('8').removesuffix(':hls:manifest.m3u'))
+
+
+class VideoURLs:
+    __slots__ = ('raw_data', 'qualities', 'min')
+
+    def __init__(self, data: str | dict):
+        self.raw_data: dict[Quality, VideoURL] = (
+            {Quality(q): VideoURL(u) for q, u in findall_qualities(clear_trash(data))}
+            if isinstance(data, str) else data)
+        self.qualities: tuple[Quality] = *sorted(self.raw_data),
+        self.min = int(self.qualities[0]) if self.qualities else 1
+
+    @property
+    def last_url(self) -> VideoURL:
+        return self[-1].raw_data.popitem()[1]
+
+    def __getitem__(self, item: str | SupportsInt | Iterable | slice):
+        isiter = False
+        if not isinstance(item, str):
+            if isinstance(item, slice):
+                item = item.start, item.stop, item.step
+            isiter = isinstance(item, Iterable) and item
+        if isiter:
+            result = self
+            for part in item:
+                if part is not None:
+                    result = result[part]
+            result = result.raw_data
+        elif isinstance(item, int):
+            if item < self.min:
+                item = self.qualities[item]
+                result = {item: self.raw_data[item]}
+            else:
+                result = {q: v for q, v in self.raw_data.items() if int(q) == item}
+        elif isinstance(item, str):
+            item = item.casefold()
+            result = {q: v for q, v in self.raw_data.items() if q.addon == item}
+        else:
+            raise TypeError(f'Invalid type {type(item)}')
+        return self.__class__(result)
+
+    def __repr__(self):
+        return f"{self.__class__.__qualname__}({self.raw_data})"
```

### Comparing `HDRezka-2.0.1/hdrezka/stream/player.py` & `HDRezka-3.0.0/hdrezka/stream/player.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,105 @@
-from collections import defaultdict
-from functools import lru_cache
-from typing import Any, SupportsInt, TypeVar
-
-from .._bs4 import BeautifulSoup
-from ..api.ajax import AJAX
-from ..errors import UnknownContentType
-from ..post import *
-
-__all__ = ('Player', 'PlayerType', 'PlayerBase', 'PlayerMovie', 'PlayerSeries')
-
-
-class PlayerBase:
-    __slots__ = ('post',)
-
-    def __init__(self, url_or_cast: Any):
-        if isinstance(url_or_cast, PlayerBase):
-            self.post = url_or_cast.post
-            return
-        elif not isinstance(url_or_cast, str):
-            url_or_cast = str(url_or_cast)
-        self.post = Post(url_or_cast)
-
-    def _translator(self, translator_id: SupportsInt = None) -> int:
-        if translator_id is None:
-            return self.post.translator_id
-        translator_id = int(translator_id)
-        return self.post.translators.ids[abs(translator_id)] if translator_id <= 0 else translator_id
-
-    def __repr__(self):
-        return f"{self.__class__.__qualname__}({short_url(self.post.url)!r})"
-
-
-class PlayerMovie(PlayerBase):
-    __slots__ = ()
-
-    def get_stream(self, translator_id: SupportsInt = None) -> URLs:
-        return urls_from_ajax_response(AJAX.get_movie(self.post.id, self._translator(translator_id)))
-
-
-class PlayerSeries(PlayerBase):
-    __slots__ = ()
-
-    def get_episodes(self, translator_id: SupportsInt = None) -> defaultdict[int, tuple[int]]:
-        episodes = BeautifulSoup(AJAX.get_episodes(self.post.id, self._translator(translator_id))['episodes'])
-        result: defaultdict[int, tuple[int]] = defaultdict(tuple)
-        for i in episodes.find_all(class_='b-simple_episode__item', attrs=('data-season_id', 'data-episode_id')):
-            result[int(i.get('data-season_id'))] += int(i.get('data-episode_id')),
-        return result
-
-    def get_stream(self, season: int, episode: int, translator_id: SupportsInt = None) -> URLs:
-        return urls_from_ajax_response(AJAX.get_stream(self.post.id, self._translator(translator_id), season, episode))
-
-
-PlayerType = TypeVar('PlayerType', PlayerBase, PlayerMovie, PlayerSeries)
-
-
-@lru_cache(512)
-def player(url_or_path: Any) -> PlayerType:
-    """
-    Returns either Player Series if series, or PlayerMovie if movie, otherwise raises UnknownContentType
-    """
-    cast = PlayerBase(url_or_path)
-    type = cast.post.type
-    match type:
-        case 'tv_series':
-            return PlayerSeries(cast)
-        case 'movie':
-            return PlayerMovie(cast)
-    raise UnknownContentType(type)
-
-
-Player = player
+import sys
+from collections import defaultdict
+from typing import Any, SupportsInt, TypeVar
+
+from .._bs4 import BeautifulSoup
+from ..api.ajax import AJAX
+from ..errors import UnknownContentType
+from ..post import *
+
+__all__ = ('Player', 'PlayerType', 'PlayerBase', 'PlayerMovie', 'PlayerSeries')
+
+
+class _CacheStorage:
+    __slots__ = ('max_size', '__storage')
+
+    def __init__(self, max_size: int = 256):
+        self.max_size = max_size
+        self.__storage = {}
+
+    def get(self, key):
+        return self.__storage.get(key)
+
+    def set(self, key, value):
+        self.__storage[key] = value
+        for k in self.__storage.keys():
+            if sys.getsizeof(self.__storage) <= self.max_size:
+                break
+            del self.__storage[k]
+
+
+__CACHE = _CacheStorage()
+
+
+class PlayerBase:
+    __slots__ = ('post',)
+
+    def __init__(self, url_or_cast: Any):
+        """Also you should call the `ainit` method"""
+        if isinstance(url_or_cast, PlayerBase):
+            self.post = url_or_cast.post
+            return
+        elif not isinstance(url_or_cast, str):
+            url_or_cast = str(url_or_cast)
+        self.post = Post(url_or_cast)
+
+    async def ainit(self):
+        await self.post.ainit()
+
+    def _translator(self, translator_id: SupportsInt = None) -> int:
+        if translator_id is None:
+            return self.post.translator_id
+        translator_id = int(translator_id)
+        return self.post.translators.ids[abs(translator_id)] if translator_id <= 0 else translator_id
+
+    def __repr__(self):
+        return f"{self.__class__.__qualname__}({short_url(self.post.url)!r})"
+
+
+class PlayerMovie(PlayerBase):
+    __slots__ = ()
+
+    async def get_stream(self, translator_id: SupportsInt = None) -> URLs:
+        return urls_from_ajax_response(await AJAX.get_movie(self.post.id, self._translator(translator_id)))
+
+
+class PlayerSeries(PlayerBase):
+    __slots__ = ()
+
+    async def get_episodes(self, translator_id: SupportsInt = None) -> defaultdict[int, tuple[int]]:
+        episodes = BeautifulSoup((await AJAX.get_episodes(self.post.id, self._translator(translator_id)))['episodes'])
+        result: defaultdict[int, tuple[int]] = defaultdict(tuple)
+        for i in episodes.find_all(class_='b-simple_episode__item', attrs=('data-season_id', 'data-episode_id')):
+            result[int(i.get('data-season_id'))] += int(i.get('data-episode_id')),
+        return result
+
+    async def get_stream(self, season: int, episode: int, translator_id: SupportsInt = None) -> URLs:
+        return urls_from_ajax_response(
+            await AJAX.get_stream(self.post.id, self._translator(translator_id), season, episode))
+
+
+PlayerType = TypeVar('PlayerType', PlayerBase, PlayerMovie, PlayerSeries)
+
+
+async def player(url_or_path: Any) -> PlayerType:
+    """
+    Returns either Player Series if series, or PlayerMovie if movie, otherwise raises UnknownContentType
+    """
+    cast = PlayerBase(url_or_path)
+    cached = __CACHE.get(cast.post.url)
+    if cached is not None:
+        return cached
+    await cast.ainit()
+    type = cast.post.type
+    match type:
+        case 'tv_series':
+            value = PlayerSeries(cast)
+        case 'movie':
+            value = PlayerMovie(cast)
+        case _:
+            raise UnknownContentType(type)
+    __CACHE.set(cast.post.url, value)
+    return value
+
+
+Player = player
```

### Comparing `HDRezka-2.0.1/setup.py` & `HDRezka-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('README.md', encoding='UTF-8') as f:
     long_description = f.read().strip()
 with open('CHANGELOG.md', encoding='UTF-8') as f:
     long_description += f'\n\n---\n\n{f.read().strip()}\n'
 
 setuptools.setup(
     name='HDRezka',
-    version='2.0.1',
+    version='3.0.0',
 
     author='Nikita (NIKDISSV)',
     author_email='nikdissv@proton.me',
 
     description='HDRezka (rezka.ag) Python API',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

