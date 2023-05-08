# Comparing `tmp/tdh-tcd-2.5.2.tar.gz` & `tmp/tdh-tcd-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdh-tcd-2.5.2.tar", last modified: Sat May  6 23:39:46 2023, max compression
+gzip compressed data, was "tdh-tcd-2.5.3.tar", last modified: Mon May  8 00:41:35 2023, max compression
```

## Comparing `tdh-tcd-2.5.2.tar` & `tdh-tcd-2.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/tcd/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/example.settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/twitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/tdh_tcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:41:35.985564 tdh-tcd-2.5.3/tcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/example.settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/twitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/tdh_tcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/top_level.txt
```

### Comparing `tdh-tcd-2.5.2/LICENSE` & `tdh-tcd-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.2/PKG-INFO` & `tdh-tcd-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.2
+Version: 2.5.3
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tdh-tcd-2.5.2/README.md` & `tdh-tcd-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.2/setup.py` & `tdh-tcd-2.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', 'r') as fi:
     long_description = fi.read()
 
 
 setup(
     name='tdh-tcd',
-    version='2.5.2',
+    version='2.5.3',
 
     author='Dmitry Karikh',
     author_email='the.dr.hax@gmail.com',
 
     description='Twitch Chat Downloader',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `tdh-tcd-2.5.2/tcd/__init__.py` & `tdh-tcd-2.5.3/tcd/__init__.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.2/tcd/example.settings.json` & `tdh-tcd-2.5.3/tcd/example.settings.json`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.2/tcd/settings.py` & `tdh-tcd-2.5.3/tcd/settings.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.2/tcd/subtitles.py` & `tdh-tcd-2.5.3/tcd/subtitles.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.2/tcd/twitch.py` & `tdh-tcd-2.5.3/tcd/twitch.py`

 * *Files 12% similar despite different names*

```diff
@@ -139,70 +139,87 @@
         self.duration = video['data']['video']['lengthSeconds']
         self.title = video['data']['video']['title']
         self.creator_name = video['data']['video']['creator']['displayName']
         self.creator_id = video['data']['video']['creator']['id']
 
         if settings.get('display_progress') in [None, True]:
             self.progressbar = ProgressBar(max_value=self.duration)
-    
-    def __iter__(self):
-        hasNextPage = True
-        cursor = 0
-        hashes = set()
 
-        while hasNextPage:
-            res = gql(f'''
-                query {{
-                    video(id: "{self.video_id}") {{
-                        comments{f'(contentOffsetSeconds: {cursor})' if cursor > 0 else ''} {{
-                            edges {{
-                                cursor
-                                node {{
-                                    commenter {{
-                                        displayName
-                                        login
-                                        displayBadges(channelID: {self.creator_id}) {{
-                                            setID
-                                        }}
+    def _get_comments(self, selector: str):
+        return gql(f'''
+            query {{
+                video(id: "{self.video_id}") {{
+                    comments{selector} {{
+                        edges {{
+                            cursor
+                            node {{
+                                commenter {{
+                                    displayName
+                                    login
+                                    displayBadges(channelID: {self.creator_id}) {{
+                                        setID
                                     }}
-                                    createdAt
-                                    contentOffsetSeconds
-                                    message {{
-                                        fragments {{
-                                            text
-                                        }}
-                                        userColor
+                                }}
+                                createdAt
+                                contentOffsetSeconds
+                                message {{
+                                    fragments {{
+                                        text
                                     }}
+                                    userColor
                                 }}
                             }}
+                        }}
 
-                            pageInfo {{
-                                hasNextPage
-                            }}
+                        pageInfo {{
+                            hasNextPage
                         }}
                     }}
                 }}
-            ''')
+            }}
+        ''')['data']['video']['comments']
 
-            comments = res['data']['video']['comments']
-            hasNextPage = comments['pageInfo']['hasNextPage']
+    def __iter__(self):
+        hasNextPage = True
+        offset = 0
+        cursor = None
+        hashes = set()
 
-            # Avoid infinite loops
-            new_cursor = comments['edges'][-1]['node']['contentOffsetSeconds']
-            if new_cursor <= cursor:
-                cursor += 1
-                continue
+        while hasNextPage and offset <= self.duration:
+            if cursor:
+                selector = f'(after: "{cursor}")'
+            elif offset > 0:
+                selector = f'(contentOffsetSeconds: {offset})'
             else:
-                cursor = new_cursor
+                selector = ''
+
+            comments = self._get_comments(selector)
+
+            if not comments or len(comments) == 0:
+                if cursor:
+                    print('WARN: Cursors are not working, '
+                          'falling back to content offset')
+                    cursor = None
+                    continue
+
+                break
+
+            # Always true without cursor
+            hasNextPage = comments['pageInfo']['hasNextPage']
+
+            if offset == 0 or cursor:
+                cursor = comments['edges'][-1]['cursor']
+
+            offset = comments['edges'][-1]['node']['contentOffsetSeconds'] + 1
 
             for comment in comments['edges']:
                 # Calculate more accurate offset
                 ts = parse8601(comment['node']['createdAt'])
-                offset = (ts - self.created_at).total_seconds()
-                comment['node']['contentOffsetSeconds'] = offset
+                precise_offset = (ts - self.created_at).total_seconds()
+                comment['node']['contentOffsetSeconds'] = precise_offset
 
                 try:
                     msg = Message(comment['node'])
                 except Exception:
                     continue
             
                 msg_hash = msg.hash()
@@ -211,15 +228,15 @@
                     continue
                 else:
                     hashes.add(msg_hash)
 
                 yield msg
 
             if self.progressbar:
-                ts = comments['edges'][-1]['node']['contentOffsetSeconds']
+                ts = offset - 1
                 self.progressbar.update(min(self.duration, ts))
 
             if settings['cooldown'] > 0:
                 sleep(settings['cooldown'] / 1000)
 
 
 class Channel(object):
```

### Comparing `tdh-tcd-2.5.2/tdh_tcd.egg-info/PKG-INFO` & `tdh-tcd-2.5.3/tdh_tcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.2
+Version: 2.5.3
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
```

