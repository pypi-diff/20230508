# Comparing `tmp/podqueue-0.1.2.tar.gz` & `tmp/podqueue-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podqueue-0.1.2.tar", last modified: Wed May  4 11:22:15 2022, max compression
+gzip compressed data, was "podqueue-0.1.3.tar", last modified: Mon May  8 10:17:37 2023, max compression
```

## Comparing `podqueue-0.1.2.tar` & `podqueue-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 11:22:15.263290 podqueue-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-04 11:22:03.000000 podqueue-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-04 11:22:03.000000 podqueue-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8381 2022-05-04 11:22:15.263290 podqueue-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7780 2022-05-04 11:22:03.000000 podqueue-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 11:22:15.263290 podqueue-0.1.2/podqueue/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-04 11:22:03.000000 podqueue-0.1.2/podqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-04 11:22:03.000000 podqueue-0.1.2/podqueue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11853 2022-05-04 11:22:03.000000 podqueue-0.1.2/podqueue/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 11:22:15.263290 podqueue-0.1.2/podqueue/podqueue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8381 2022-05-04 11:22:14.000000 podqueue-0.1.2/podqueue/podqueue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-05-04 11:22:15.000000 podqueue-0.1.2/podqueue/podqueue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 11:22:14.000000 podqueue-0.1.2/podqueue/podqueue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-04 11:22:15.000000 podqueue-0.1.2/podqueue/podqueue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-04 11:22:15.000000 podqueue-0.1.2/podqueue/podqueue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-04 11:22:03.000000 podqueue-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-05-04 11:22:15.263290 podqueue-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-05-04 11:22:03.000000 podqueue-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:17:37.051042 podqueue-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 10:17:23.000000 podqueue-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 10:17:23.000000 podqueue-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-08 10:17:37.051042 podqueue-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-08 10:17:23.000000 podqueue-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:17:37.051042 podqueue-0.1.3/podqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 10:17:23.000000 podqueue-0.1.3/podqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-08 10:17:23.000000 podqueue-0.1.3/podqueue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-05-08 10:17:23.000000 podqueue-0.1.3/podqueue/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:17:37.051042 podqueue-0.1.3/podqueue/podqueue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-08 10:17:37.000000 podqueue-0.1.3/podqueue/podqueue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 10:17:37.000000 podqueue-0.1.3/podqueue/podqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:17:37.000000 podqueue-0.1.3/podqueue/podqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 10:17:37.000000 podqueue-0.1.3/podqueue/podqueue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 10:17:37.000000 podqueue-0.1.3/podqueue/podqueue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 10:17:23.000000 podqueue-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-08 10:17:37.051042 podqueue-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-08 10:17:23.000000 podqueue-0.1.3/setup.py
```

### Comparing `podqueue-0.1.2/LICENSE` & `podqueue-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `podqueue-0.1.2/PKG-INFO` & `podqueue-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: podqueue
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automate the archiving of podcast feeds, including show notes and images.
 Home-page: https://github.com/tquin/podqueue
 Download-URL: https://pypi.org/project/podqueue/
 Author: Tyler Quinlivan
 Author-email: hello@tylerquinlivan.com
 License: MIT
 Keywords: podcast,podqueue,archive,download
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -161,8 +160,7 @@
 
 # Todos
 
 * Distro packaging
 * Better config file location, eg $HOME/.config/podqueue.conf
 * Built-in systemd/cron timers
 * Option to only download after X date (--no-backlog or --earliest ?)
-
```

### Comparing `podqueue-0.1.2/README.md` & `podqueue-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `podqueue-0.1.2/podqueue/main.py` & `podqueue-0.1.3/podqueue/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 #!/bin/env python3
 
-import feedparser
-import argparse
-import os
-from os import path, getcwd
-import xml.etree.ElementTree as ET
-from io import IOBase
-import json
-import requests
+# Builtins
 import time
-from configparser import ConfigParser
 import re
+import os
+import json
+from io import IOBase
+import xml.etree.ElementTree as ET
 import logging
 
+# Async
+import asyncio
+import httpx
+import aiofiles
+
+# PIP
+import argparse
+from configparser import ConfigParser
+import feedparser
+
 # ----- ----- ----- ----- -----
 
 class podqueue():
 
+  # ----- ----- ----- ----- -----
+  # RUN-ONCE
+  # ----- ----- ----- ----- -----
+
 
   def __init__(self):
     # Initialise to defaults before checking config file / CLI args
     self.verbose = False
     self.opml = None
     self.dest = os.path.join(os.getcwd(), 'output')
     self.time_format = '%Y-%m-%d'
     self.log_file = 'podqueue.log'
     self.feeds = []
     self.FEED_FIELDS = ['title', 'link', 'description', 'published', 'image', 'categories',]
     self.EPISODE_FIELDS = ['title', 'link', 'description', 'published_parsed', 'links',]
+    self.http_session = None
 
     # If a config file exists, ingest it
     self.check_config()
 
     # Overwrite any config file defaults with CLI params
     self.cli_args()
 
@@ -41,47 +52,47 @@
     try:
       assert self.opml is not None
     except Exception as e:
       logging.error('OPML file or destination dir was not provided')
       exit()
 
 
-  def config_logging(self):
+  def config_logging(self) -> None:
 
     # Always log to file; only stdout if -v
     handlers = [logging.FileHandler(self.log_file)]
     if (self.verbose): handlers.append(logging.StreamHandler())
 
     # Config settings
     level = logging.INFO if (self.verbose) else logging.WARNING
     logging.basicConfig(level=level, datefmt='%Y-%m-%d %H:%M:%S', handlers=handlers,
                         format='%(asctime)s [%(levelname)s] %(message)s')
 
     # Add header for append-mode file logging
     logging.info('\n----- ----- ----- ----- -----\nInitialising\n----- ----- ----- ----- -----')
 
 
-  def ascii_normalise(self, input_str, ):
+  def ascii_normalise(self, input_str: str) -> str:
     try:
-      # Replace non-simple chars with dunders
+      # Replace non-simple chars with unders
       input_str = re.sub(r'[^a-zA-Z0-9\-\_\/\\\.]', '_', input_str)
       # Replace any strings of 2+ puncts with a single underscore
       input_str = re.sub(r'_+', r'_', input_str)
       input_str = re.sub(r'([^a-zA-Z0-9]{2,})', r'_', input_str)
       # Remove any trailing puncts
       input_str = re.sub(r'(_|\.)$', r'', input_str)
       
     except Exception as e:
       logging.error(f'\t\tError normalising file name: {e}')
       exit()
 
     return input_str
 
 
-  def check_config(self):
+  def check_config(self) -> None:
     # get the path to podqueue.conf
     config_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'podqueue.conf')
 
     # Check if the file has been created
     if not os.path.exists(config_path):
       logging.info(f'Config file does not exist: {config_path}')
       return None
@@ -92,19 +103,17 @@
     for key in ['opml', 'dest', 'time_format', 'verbose', 'log_file']:
       if conf['podqueue'].get(key, None):
         setattr(self, key, conf['podqueue'].get(key, None))
 
     # If we just changed verbose to str, make sure it's back to a bool
     if self.verbose:
       self.verbose = bool(self.verbose)
-    
-    return
 
 
-  def cli_args(self):
+  def cli_args(self) -> None:
     parser = argparse.ArgumentParser(add_help=True)
 
     parser.add_argument('-o', '--opml', dest='opml', default=None, type=argparse.FileType('r'),
       help='Pass an OPML file that contains a podcast subscription list.')
     parser.add_argument('-d', '--dest', dest='dest', type=self.args_path,
       help='The destination folder for downloads. Will be created if required, including sub-directories for each separate podcast.')
     parser.add_argument('-t', '--time_format', dest='time_format',
@@ -119,89 +128,106 @@
     result = vars(parser.parse_args())
     for key, value in result.items():
       # Don't overwrite if it's not provided in CLI
       if value is not None:
         setattr(self, key, value)
 
 
-  def args_path(self, directory):
+  def args_path(self, directory: str) -> str:
     # Create the directory, if required
     if not os.path.isdir(directory):
       os.makedirs(directory)
 
     return directory
 
 
-  def parse_opml(self, opml):
+  def parse_opml(self, opml) -> None:
     logging.info(f'Parsing OPML file: {opml.name}')
 
     # Check if we have an actual file handle (CLI arg), 
     # Or a string path (config file), and we need to get our own handle
     with (opml if isinstance(opml, IOBase) else open(opml, 'r')) as opml_f:
       xml_root = ET.parse(opml_f).getroot()
 
     # Get all RSS feeds with a 'xmlUrl' attribute
     for feed in [x.attrib for x in xml_root.findall(".//outline[@type='rss']")]:
       feed_url = feed.get('xmlUrl', None)
       if feed_url:
         self.feeds.append(feed_url)
 
 
-  def get_feeds(self, feeds):
-    logging.info(f'Fetching feeds:')
+  # ----- ----- ----- ----- -----
+  # PER-FEED
+  # ----- ----- ----- ----- -----
 
-    for feed in feeds:
-      try:
-        content = feedparser.parse(feed)
 
-      # The remote RSS server can close the HTTP connection
-      # except http.client.RemoteDisconnected:
-      except:
-        logging.warning(f'Feed server unexpectedly closed connection: {feed}')
-        continue
+  async def get_feed(self, feed: str) -> None:
+    logging.info(f'Fetching feed: {feed}')
+    
+    try:
+      html_response = await self.http_session.get(feed, 
+        follow_redirects=True
+      )
+      html_response.raise_for_status()
+      html = html_response.text
+    # The remote RSS server can close the HTTP connection
+    except Exception as error:
+      logging.warning(f'Error fetching RSS feed for: {feed}, {error=}')
+      return None
 
-      # If feedparser library reports bad XML, warn and skip
-      # Test str: 'http://feedparser.org/tests/illformed/rss/aaa_illformed.xml'
-      if content.get('bozo', False):
-        logging.warning(f'Feed is misformatted: {feed}')
-        continue
+    content = feedparser.parse(html)
 
-      title = content.feed.get('title', 'Unknown Title')
+    # If feedparser library reports bad XML, warn and skip
+    # CharacterEncodingOverride is a false positive, ATP for example
+    # Test str: 'http://feedparser.org/tests/illformed/rss/aaa_illformed.xml'
+    if content.get('bozo', False) and not isinstance(
+      content.bozo_exception, 
+      feedparser.exceptions.CharacterEncodingOverride
+    ):
+      logging.warning(f'Feed is misformatted: {feed}, {content.bozo_exception}')
+      return None
 
-      logging.info(f'\tProcessing feed: {title}')
+    title = content.feed.get('title', 'Unknown Title')
+    logging.info(f'\tProcessing feed: {title}')
 
-      # Normalise the podcast name with no spaces or non-simple ascii
-      feed_dir_name = '_'.join([x for x in title.split(' ')])
-      feed_dir_name = self.ascii_normalise(feed_dir_name)
+    directory = self.create_feed_directories(title)
 
-      # Create the directory we need (no spaces) if it doesn't exist
-      directory = os.path.join(self.dest, feed_dir_name)
-      if not os.path.isdir(directory):
-        os.makedirs(directory)
+    # Get content.feed metadata - podcast title, icon, description, etc.
+    # And write it to disk as <<PODCAST>>/<<PODCAST>>.json
+    feed_metadata = await self.write_feed_metadata(content, directory)
 
-      # Also create the <<PODCAST>>/episodes subdirectory
-      if not os.path.isdir(os.path.join(directory, 'episodes')):
-        os.makedirs(os.path.join(directory, 'episodes'))
+    # Also fetch the podcast logo, if available
+    if feed_metadata.get('image', None):
+      await self.write_feed_image(feed_metadata['image'], directory)
 
-      # Get content.feed metadata - podcast title, icon, description, etc.
-      # And write it to disk as <<PODCAST>>/<<PODCAST>>.json
-      feed_metadata = self.process_feed_metadata(content, directory)
+    # Then, process the episodes each and write to disk
+    for episode in content.entries:
+      await self.process_feed_episode(episode, directory)
 
-      # Also fetch the podcast logo, if available
-      if feed_metadata.get('image', None):
-        self.get_feed_image(feed_metadata['image'], directory)
 
-      # Then, process the episodes each and write to disk
-      for episode in content.entries:
-        episode_data = self.process_feed_episode(episode, directory)
+  def create_feed_directories(self, title: str) -> str:
+    # Normalise the podcast name with no spaces or non-simple ascii
+    feed_dir_name = '_'.join([x for x in title.split(' ')])
+    feed_dir_name = self.ascii_normalise(feed_dir_name)
 
-    return None
+    # Create the directory we need (no spaces) if it doesn't exist
+    directory = os.path.join(self.dest, feed_dir_name)
+    if not os.path.exists(directory) or not os.path.isdir(directory):
+      os.makedirs(directory)
+
+    # Also create the <<PODCAST>>/episodes subdirectory
+    if not os.path.isdir(os.path.join(directory, 'episodes')):
+      os.makedirs(os.path.join(directory, 'episodes'))
+    
+    return directory
 
 
-  def process_feed_metadata(self, content, directory):
+  async def write_feed_metadata(self, 
+              content: feedparser.util.FeedParserDict, 
+              directory: str) -> dict:
     logging.info(f'\t\tProcessing feed metadata')
     
     feed_metadata = {}
 
     for field in self.FEED_FIELDS:
       # .image is a dict structure where we only want href, 
       # the rest are strs, so special case
@@ -213,67 +239,62 @@
       feed_metadata[field] = value
 
     # Additional calculated metadata based on structure:
     feed_metadata['episode_count'] = len(content.entries)
 
     metadata_filename = os.path.join(directory, f'{os.path.split(directory)[1]}.json')
 
-    with open(metadata_filename, 'w') as meta_f:
-      meta_f.write(json.dumps(feed_metadata))
+    async with aiofiles.open(metadata_filename, 'w') as meta_f:
+      await meta_f.write(json.dumps(feed_metadata))
 
     return feed_metadata
 
 
-  def get_feed_image(self, image_url, directory):
-
-    try:
-      img = requests.get(image_url)
-      img.raise_for_status()
-    except Exception as e:
-      logging.warning(f'\t\tImage could not be found: {image_url}, for reason: {e}')
-      return
-
+  async def write_feed_image(self, image_url: str, directory: str) -> None:
     image_filename_ext = os.path.splitext(image_url)[1]
+    image_filename_ext = image_filename_ext if image_filename_ext else '.jpg'
     image_filename = os.path.join(directory, f'{os.path.split(directory)[1]}{image_filename_ext}')
 
-    with open(image_filename, 'wb') as img_f:
-      for chunk in img.iter_content(chunk_size=1024*8):
-        img_f.write(chunk)
+    async with self.http_session.stream('GET', 
+      image_url,
+      follow_redirects=True
+      ) as response:
+
+      response.raise_for_status()
+      
+      async with aiofiles.open(image_filename, 'wb') as img_f:
+        async for chunk in response.aiter_bytes(chunk_size=1024*8):
+          await img_f.write(chunk)
 
     logging.info(f'\t\tAdded image to disk: {os.path.split(image_filename)[1]}')
-    return
 
 
-  def process_feed_episode(self, episode, directory):
+  # ----- ----- ----- ----- -----
+  # PER-EPISODE
+  # ----- ----- ----- ----- -----
 
+
+  async def process_feed_episode(self, 
+              episode: feedparser.util.FeedParserDict, 
+              directory: str) -> None:
     episode_metadata = {}
     for field in self.EPISODE_FIELDS:
       episode_metadata[field] = episode.get(field, None)
 
     # Change the time_struct tuple to a human string
     if episode_metadata.get('published_parsed', None):
       episode_metadata['published_parsed'] = time.strftime(self.time_format, \
-                                            episode_metadata['published_parsed'])
-
-    # Change the links{} into a single audio URL
-    if episode_metadata.get('links', None):
-      for link in episode_metadata['links']:
-        if link.get('type', None):
-          if 'audio' in link.get('type', None):
-            episode_metadata['link'] = link.get('href', None)
-            break
-
-      # Remove the old complicated links{}
-      episode_metadata.pop('links', None)
+                                          episode_metadata['published_parsed'])
 
     # Get a unique episode filename(s)
     episode_title = f'{episode_metadata["published_parsed"]}_{episode_metadata["title"]}'
 
     # Special case - the final file name (not path) can't have a slash in it
-    # Also replace colons as they are invalid in filenames on Windows (used for Alternate Data Streams on NTFS)
+    # Also replace colons as they are invalid in filenames on Windows ...
+    # ... (used for Alternate Data Streams on NTFS)
     episode_title = re.sub(r'(\/|\\|:|\?|")', r'_', episode_title)
     episode_title = self.ascii_normalise(episode_title)
 
     # Check the title isn't going to overshoot 255 bytes
     # This is the limit in ZFS, BTRFS, ext*, NTFS, APFS, XFS, etc ...
     # Otherwise, file.write will raise OSError 36 - "File name too long"
     # I'm looking at you, Memory Palace 73. I mean really, 55 words and 316 characters long?
@@ -285,48 +306,84 @@
                         f'{episode_title}.json')
     episode_audio_filename = os.path.join(os.path.join(directory, 'episodes'), \
                         f'{episode_title}.mp3')
 
     # Check if the file already exists on disk (if so, skip)
     if os.path.exists(episode_meta_filename) and os.path.exists(episode_audio_filename):
       logging.info(f'\t\tEpisode already saved, skipping: {episode_title}')
-      return
+      return None
+
+    episode_metadata = await self.write_episode_metadata(episode_title, 
+      episode_metadata, episode_meta_filename
+    )
+
+    if episode_metadata.get('link', None):
+      await self.write_episode_audio(episode_title, 
+        episode_metadata.get('link'), episode_audio_filename
+      )
+
+
+  async def write_episode_metadata(self, 
+              episode_title: str, 
+              episode_metadata: dict, 
+              episode_meta_filename: str) -> dict:
+    # Change the links{} into a single audio URL
+    if episode_metadata.get('links', None):
+      for link in episode_metadata['links']:
+        if link.get('type', None):
+          if 'audio' in link.get('type', None):
+            episode_metadata['link'] = link.get('href', None)
+            break
+
+      # Remove the old complicated links{}
+      episode_metadata.pop('links', None)
 
     # Write metadata to disk
-    with open(episode_meta_filename, 'w') as ep_meta_f:
-        ep_meta_f.write(json.dumps(episode_metadata))
+    async with aiofiles.open(episode_meta_filename, 'w') as ep_meta_f:
+        await ep_meta_f.write(json.dumps(episode_metadata))
 
-    logging.info(f'\t\t\tAdded episode metadata to disk: {episode_title}')
+    logging.info(f'\t\tAdded episode metadata to disk: {episode_title}')
+    return episode_metadata
 
-    # Download the audio file
-    if episode_metadata.get('link', None):
-      try:
-        audio = requests.get(episode_metadata['link'])
-        audio.raise_for_status()
-      except Exception as e:
-        logging.warning(f'\t\t\tAudio could not be found: {episode_metadata["link"]}')
-        return
-
-    # Write audio to disk
-    with open(episode_audio_filename, 'wb') as audio_f:
-      for chunk in audio.iter_content(chunk_size=1024*8):
-        audio_f.write(chunk)
-    logging.info(f'\t\t\tAdded episode audio to disk: {episode_title}')
 
-    return
+  async def write_episode_audio(self, 
+              episode_title: str, 
+              audio_url: dict, 
+              episode_audio_filename: str) -> None:
+
+    async with self.http_session.stream('GET', 
+      audio_url,
+      follow_redirects=True
+      ) as response:
+
+      response.raise_for_status()
+      
+      async with aiofiles.open(episode_audio_filename, 'wb') as audio_f:
+        async for chunk in response.aiter_bytes(chunk_size=1024*8):
+          await audio_f.write(chunk)
+
+    logging.info(f'\t\tAdded episode audio to disk: {episode_title}')
 
 
 # ----- ----- ----- ----- -----
 
-def entry():
+async def entry():
   # Initialise the config - from file, or CLI args
   pq = podqueue()
   
   # Parse all feed URLs out of the OPML XML into pq.feeds=[]
   pq.parse_opml(pq.opml)
 
-  # Download the metadata, images, and any missing episodes
-  pq.get_feeds(pq.feeds)
+  async with httpx.AsyncClient() as http_session:
+    pq.http_session = http_session
+
+    # Download the metadata, images, and any missing episodes
+    tasks = [asyncio.create_task(
+              pq.get_feed(feed))
+            for feed in pq.feeds]
+
+    done, pending = await asyncio.wait(tasks)
+    logging.info('Async {done=}, {pending=}')
 
 
 if __name__ == '__main__':
-  entry()
+  asyncio.run(entry())
```

### Comparing `podqueue-0.1.2/podqueue/podqueue.egg-info/PKG-INFO` & `podqueue-0.1.3/podqueue/podqueue.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: podqueue
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automate the archiving of podcast feeds, including show notes and images.
 Home-page: https://github.com/tquin/podqueue
 Download-URL: https://pypi.org/project/podqueue/
 Author: Tyler Quinlivan
 Author-email: hello@tylerquinlivan.com
 License: MIT
 Keywords: podcast,podqueue,archive,download
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -161,8 +160,7 @@
 
 # Todos
 
 * Distro packaging
 * Better config file location, eg $HOME/.config/podqueue.conf
 * Built-in systemd/cron timers
 * Option to only download after X date (--no-backlog or --earliest ?)
-
```

### Comparing `podqueue-0.1.2/setup.cfg` & `podqueue-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = podqueue
-version = 0.1.2
+version = 0.1.3
 author = Tyler Quinlivan
 description = Automate the archiving of podcast feeds, including show notes and images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tquin/podqueue
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `podqueue-0.1.2/setup.py` & `podqueue-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name = 'podqueue',
-    version = '0.1.2',
+    version = '0.1.3',
     description = 'Automate the archiving of podcast feeds, including show notes and images.',
     long_description_content_type = "text/markdown",
     long_description = README,
     license = 'MIT',
     packages = find_packages(),
     author = 'Tyler Quinlivan',
     author_email = 'hello@tylerquinlivan.com',
```

