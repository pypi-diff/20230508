# Comparing `tmp/twitch-archiver-3.0.0.dev6.tar.gz` & `tmp/twitch-archiver-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-archiver-3.0.0.dev6.tar", last modified: Fri Apr 28 03:28:59 2023, max compression
+gzip compressed data, was "twitch-archiver-3.0.1.tar", last modified: Mon May  8 12:53:12 2023, max compression
```

## Comparing `twitch-archiver-3.0.0.dev6.tar` & `twitch-archiver-3.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:59.826057 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/twitcharchiver/
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    39610 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:53:12.495687 twitch-archiver-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 12:53:12.495687 twitch-archiver-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:53:12.495687 twitch-archiver-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:53:12.491687 twitch-archiver-3.0.1/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 12:53:12.000000 twitch-archiver-3.0.1/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 12:53:12.000000 twitch-archiver-3.0.1/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:53:12.000000 twitch-archiver-3.0.1/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 12:53:12.000000 twitch-archiver-3.0.1/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 12:53:12.000000 twitch-archiver-3.0.1/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:53:12.495687 twitch-archiver-3.0.1/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-05-08 12:53:01.000000 twitch-archiver-3.0.1/twitcharchiver/utils.py
```

### Comparing `twitch-archiver-3.0.0.dev6/LICENSE` & `twitch-archiver-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/PKG-INFO` & `twitch-archiver-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.0.dev6
+Version: 3.0.1
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-3.0.0.dev6/README.md` & `twitch-archiver-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/pyproject.toml` & `twitch-archiver-3.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "3.0.0.dev6"
+version = "3.0.1"
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
 description = "A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/PKG-INFO` & `twitch-archiver-3.0.1/twitch_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.0.dev6
+Version: 3.0.1
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/SOURCES.txt` & `twitch-archiver-3.0.1/twitch_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/__init__.py` & `twitch-archiver-3.0.1/twitcharchiver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from twitcharchiver.configuration import Configuration
 from twitcharchiver.exceptions import TwitchAPIError
 from twitcharchiver.logger import Logger
 from twitcharchiver.processing import Processing
 from twitcharchiver.twitch import Twitch
 from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple, check_update_available
 
-__version__ = '3.0.0.dev6'
+__version__ = '3.0.1'
 
 
 def main():
     """
     Main processing for twitch-archiver.
     """
     parser = argparse.ArgumentParser(argument_default=None, description=textwrap.dedent(f"""\
```

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/api.py` & `twitch-archiver-3.0.1/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/arguments.py` & `twitch-archiver-3.0.1/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/configuration.py` & `twitch-archiver-3.0.1/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/database.py` & `twitch-archiver-3.0.1/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/downloader.py` & `twitch-archiver-3.0.1/twitcharchiver/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,88 +164,96 @@
 
         return False
 
     def get_chat(self, vod_json, offset=0):
         """Downloads the chat for a specified VOD, returning comments beginning from offset (if provided).
 
         :param vod_json: dict of vod information
-        :param offset: offset in seconds to begin chat retrieval from - none to begin at start
+        :param offset: offset in seconds to begin chat retrieval from
         """
         chat_log = []
+        message_ids = set()
+        prev_page = None
 
         _s = requests.session()
         _s.headers.update({'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'})
 
         # grab initial chat segment containing cursor
-        initial_segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], offset=offset)
+        initial_segment, next_page = self.get_chat_segment(_s, vod_json['vod_id'], offset)
         chat_log.extend(initial_segment)
+        message_ids.update([m['id'] for m in chat_log])
+        offset = chat_log[-1]['contentOffsetSeconds']
 
         progress = Progress()
 
-        while True:
-            if not cursor:
-                break
+        # we use the contentOffset of the last comment grabbed as a rudimentary cursor as Twitch severely restricted
+        # access to the GQL API by implementing 'kasadas' which is far more work to try and bypass than I feel is worth
+        while offset <= vod_json['duration'] and next_page:
+            # break infinite loops
+            if offset == prev_page:
+                offset += 1
+                continue
+
+            prev_page = offset
 
             try:
-                # grab next chat segment along with cursor for next segment
-                segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], cursor=cursor)
-                chat_log.extend(segment)
+                # grab next chat segment based on offset
+                segment, next_page = self.get_chat_segment(_s, vod_json['vod_id'], offset)
+                chat_log.extend([m for m in segment if m['id'] not in message_ids])
+                message_ids.update([m['id'] for m in chat_log])
+
                 # vod duration in seconds is used as the total for progress bar
                 # comment offset is used to track what's been done
                 # could be done properly if there was a way to get the total number of comments
                 if not self.quiet:
                     progress.print_progress(int(segment[-1]['contentOffsetSeconds']),
-                                            vod_json['duration'], not cursor)
+                                            vod_json['duration'], not offset)
+
+                # move cursor to offset of most recent message, or increment
+                if chat_log[-1]['contentOffsetSeconds'] > offset:
+                    offset = chat_log[-1]['contentOffsetSeconds']
+
+                else:
+                    offset += 1
 
             except TwitchAPIErrorNotFound:
                 break
 
-            finally:
-                _s.close()
+        _s.close()
 
         self.log.info('Found %s messages.', len(chat_log))
 
         return chat_log
 
-    def get_chat_segment(self, session, vod_id, offset=None, cursor=None):
+    def get_chat_segment(self, session, vod_id, offset):
         """Retrieves a single chat segment.
 
         :param session: requests session to link request to
         :param vod_id: id of vod to retrieve segment from
         :param offset: offset in seconds to begin retrieval from
-        :param cursor: cursor returned by a previous call of this function
         :return: list of comments and cursor if one is returned from twitch
+        :return: True if more pages available
         """
         # build payload
-        if offset is not None:
-            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
-                   "variables": {"videoID": vod_id, "contentOffsetSeconds": offset}}]
-
-        else:
-            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
-                   "variables": {"videoID": vod_id, "cursor": cursor}}]
+        _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
+               "variables": {"videoID": vod_id, "contentOffsetSeconds": offset}}]
 
-        _p[0]['extensions'] =\
+        _p[0]['extensions'] = \
             {'persistedQuery': {'version': 1,
                                 'sha256Hash': "b70a3591ff0f4e0313d126c6a1502d79a1c02baebb288227c582044aa76adf6a"}}
 
         for attempt in range(6):
             if attempt > 4:
-                self.log.error('Maximum attempts reached while downloading chat segment at cursor or offset: %s, %s.',
-                               cursor, offset)
+                self.log.error('Maximum attempts reached while downloading chat segment at offset: %s.', offset)
                 raise ChatDownloadError
 
             try:
                 _r = Api.post_request_with_session('https://gql.twitch.tv/gql', session, _p).json()
 
             except RequestError:
                 continue
 
             break
 
         comments = _r[0]['data']['video']['comments']
 
-        # check if next page exists
-        if comments['pageInfo']['hasNextPage']:
-            return [c['node'] for c in comments['edges']], comments['edges'][-1]['cursor']
-
-        return [c['node'] for c in comments['edges']], None
+        return [c['node'] for c in comments['edges']], comments['pageInfo']['hasNextPage']
```

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/exceptions.py` & `twitch-archiver-3.0.1/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/logger.py` & `twitch-archiver-3.0.1/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/processing.py` & `twitch-archiver-3.0.1/twitcharchiver/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.directory = args['directory']
         self.vod_directory = Path(self.directory)
         self.video = args['video']
         self.chat = args['chat']
         self.quality = args['quality']
         self.live_only = args['live_only']
         self.archive_only = args['archive_only']
+        self.real_time_archiver = args['real_time_archiver']
         self.config_dir = args['config_dir']
         self.quiet = args['quiet']
         self.debug = args['debug']
 
         self.client_id = config['client_id']
         self.client_secret = config['client_secret']
         self.oauth_token = config['oauth_token']
@@ -99,50 +100,67 @@
                     # update version 3 schema to version 4
                     if version == 3:
                         self.log.debug('Performing incremental DB update. Version 3 -> Version 4.')
                         db.update_database(3)
 
             # fetch channel info and live status
             channel_data = self.call_twitch.get_api(f'streams?user_id={user_id}')['data']
+            self.log.debug('Channel info: %s', channel_data)
             if channel_data and channel_data[0]['type'] == 'live':
                 channel_live = True
                 # ensure enough time has passed for vod api to update before archiving
                 stream_length = time_since_date(datetime.strptime(
                     channel_data[0]['started_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
 
+                self.log.debug('Current stream length: %s', stream_length)
+
                 # while we wait for the api to update we must build a temporary buffer of any parts advertised in the
                 # meantime in case there is no vod and thus no way to retrieve them after the fact
-                if stream_length < 90:
-                    self.log.debug('Stream began less than 90s ago, delaying archival start until VOD API updated.')
+                if stream_length < 300:
+                    self.log.debug('Stream began less than 5m ago, delaying archival start until VOD API updated.')
                     # create temp dir for buffer
                     Path(tmp_buffer_dir).mkdir(parents=True, exist_ok=True)
 
                     stream.unsynced_setup(tmp_buffer_dir)
                     index_uri = self.call_twitch.get_channel_hls_index(channel, self.quality)
 
                     # download new parts every 4s
-                    for i in range(int((90 - stream_length) / 4)):
+                    for i in range(int((300 - stream_length) / 4)):
                         # grab required values
                         start_timestamp = int(datetime.utcnow().timestamp())
                         incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
 
                         # create buffer and download segments to temp dir
                         stream.build_unsynced_buffer(incoming_segments)
                         stream.download_buffer(tmp_buffer_dir)
 
                         # wait if less than 5s passed since grabbing more parts
                         processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
                         if processing_time < 4:
                             sleep(4 - processing_time)
 
                     # wait any remaining time
-                    sleep((90 - stream_length) % 4)
+                    sleep((300 - stream_length) % 4)
 
             # retrieve available vods
-            available_vods = Twitch.get_channel_videos(channel)
+            available_vods: dict[int: tuple[int]] = {}
+            cursor = ''
+            try:
+                while True:
+                    _r = self.call_twitch.get_api(f'videos?user_id={user_id}&first=100&type=archive&after={cursor}')
+                    if not _r['pagination']:
+                        break
+
+                    # dict containing stream_id: (vod_id)
+                    available_vods.update(dict([(int(vod['stream_id']), (vod['id'])) for vod in _r['data']]))
+                    cursor = _r['pagination']['cursor']
+
+            except BaseException as e:
+                self.log.error('Error retrieving VODs from Twitch. Error: %s', str(e))
+                continue
 
             self.log.debug(f'Online VODs: {available_vods}')
 
             # retrieve downloaded vods
             with Database(Path(self.config_dir, 'vods.db')) as db:
                 # dict containing stream_id: (vod_id, video_downloaded, chat_downloaded)
                 downloaded_vods = dict([(i[0], (i[1], i[2], i[3])) for i in db.execute_query(
```

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/stream.py` & `twitch-archiver-3.0.1/twitcharchiver/stream.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/twitch.py` & `twitch-archiver-3.0.1/twitcharchiver/twitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,60 +99,51 @@
         }}
         """.format(vod_id=vod_id)
         _r = Api.post_request('https://gql.twitch.tv/gql', j={'query': _q}, h=_h)
 
         return _r.json()['data']['videoPlaybackAccessToken']
 
     @staticmethod
-    def get_channel_videos(channel):
-        """Retrieves archived (saved VODs) of a specified channel.
+    def get_latest_channel_broadcast(channel):
+        """Retrieves most recent archived broadcast. More reliable than helix API for VODs created within the last
+        few seconds.
 
         :param channel: Name of Twitch channel/user
-        :return: dict containing pairs of stream_id: vod_id
+        :return: set of most recent values of (stream_id, vod_id)
         """
         # Uses default client header
         _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
         _q = [{
             "extensions": {
                 "persistedQuery": {
-                    "sha256Hash": "a937f1d22e269e39a03b509f65a7490f9fc247d7f83d6ac1421523e3b68042cb",
+                    "sha256Hash": "8afefb1ed16c4d8e20fa55024a7ed1727f63b6eca47d8d33a28500770bad8479",
                     "version": 1
                 }
             },
-            "operationName": "FilterableVideoTower_Videos",
+            "operationName": "ChannelVideoShelvesQuery",
             "variables": {
-                "broadcastType": "ARCHIVE",
-                "channelOwnerLogin": f"{channel.lower()}",
-                "limit": 30,
-                "videoSort": "TIME"
+                "channelLogin": f"{channel.lower()}",
+                "first": 5,
             }
         }]
-        _cursor = True
-        _ids = {}
 
-        # fetch video pages one after another as long as cursor exists
-        while _cursor:
-            _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
-            _d = _r.json()[0]['data']['user']['videos']
-
-            # extract vod and stream ids from thumbnail url (stream id isnt provided directly with this call) and
-            # add to id dict. this will likely break at some point but requires far fewer requests if there are
-            # hundreds of vods.
-            _thumbnail_urls = [v['node']['animatedPreviewURL'].split('/') for v in _d['edges']]
-            _ids.update({int(t[3].split('_')[2]): t[5].split('-')[0] for t in _thumbnail_urls})
-
-            # set cursor if nextPage provided
-            if _d['pageInfo']['hasNextPage']:
-                _cursor = _d['edges'][-1]['cursor']
-                _q[0]['variables']['cursor'] = _cursor
+        _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
+        _d = _r.json()[0]['data']['user']['videoShelves']['edges']
 
-            else:
-                _cursor = None
+        # extract vod and stream ids from thumbnail url (stream id isnt provided with this call) and add to id list.
+        # _d will be empty if no archives available.
+        if _d:
+            # iter over edges as the order may change, or LATEST_BROADCASTS not provided if none found
+            for edge in _d:
+                if edge['node']['type'] == 'LATEST_BROADCASTS':
+                    _thumbnail_url = edge['node']['items'][0]['animatedPreviewURL'].split('/')
+                    _id = (_thumbnail_url[3].split('_')[2], _thumbnail_url[5].split('-')[0])
+                    return _id
 
-        return _ids
+        return
 
     def get_vod_index(self, vod_json, quality='best'):
         """Retrieves an index of m3u8 streams for a given VOD.
 
         :param vod_json: vod information retrieved from Twitch
         :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
         :return: url of m3u8 playlist
```

### Comparing `twitch-archiver-3.0.0.dev6/twitcharchiver/utils.py` & `twitch-archiver-3.0.1/twitcharchiver/utils.py`

 * *Files identical despite different names*

