# Comparing `tmp/aocref-2.0.8.tar.gz` & `tmp/aocref-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aocref-2.0.8.tar", last modified: Tue Jan 31 12:42:09 2023, max compression
+gzip compressed data, was "aocref-2.0.9.tar", last modified: Sun May  7 23:22:07 2023, max compression
```

## Comparing `aocref-2.0.8.tar` & `aocref-2.0.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.862870 aocref-2.0.8/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)       66 2021-04-18 17:22:22.000000 aocref-2.0.8/MANIFEST.in
--rw-rw-r--   0 mzander   (1000) mzander   (1000)      153 2023-01-31 12:42:09.862870 aocref-2.0.8/PKG-INFO
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     1299 2023-01-16 14:12:23.000000 aocref-2.0.8/README.md
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.850870 aocref-2.0.8/aocref/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)        0 2021-04-11 14:48:02.000000 aocref-2.0.8/aocref/__init__.py
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.850870 aocref-2.0.8/aocref/data/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     2399 2022-10-27 12:48:20.000000 aocref-2.0.8/aocref/data/constants.json
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.854869 aocref-2.0.8/aocref/data/datasets/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)    34711 2021-11-07 15:50:27.000000 aocref-2.0.8/aocref/data/datasets/0.json
--rw-rw-r--   0 mzander   (1000) mzander   (1000)    55361 2021-11-07 15:50:27.000000 aocref-2.0.8/aocref/data/datasets/1.json
--rw-rw-r--   0 mzander   (1000) mzander   (1000)    62436 2023-01-09 21:00:47.000000 aocref-2.0.8/aocref/data/datasets/100.json
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     9039 2021-11-07 15:50:27.000000 aocref-2.0.8/aocref/data/datasets/2.json
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     8065 2021-11-07 15:50:27.000000 aocref-2.0.8/aocref/data/datasets/200.json
--rw-rw-r--   0 mzander   (1000) mzander   (1000)    58550 2021-11-07 15:50:27.000000 aocref-2.0.8/aocref/data/datasets/300.json
--rw-rw-r--   0 mzander   (1000) mzander   (1000)    52141 2021-11-07 15:50:27.000000 aocref-2.0.8/aocref/data/datasets/7.json
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.850870 aocref-2.0.8/aocref.egg-info/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)      153 2023-01-31 12:42:09.000000 aocref-2.0.8/aocref.egg-info/PKG-INFO
--rw-rw-r--   0 mzander   (1000) mzander   (1000)      803 2023-01-31 12:42:09.000000 aocref-2.0.8/aocref.egg-info/SOURCES.txt
--rw-rw-r--   0 mzander   (1000) mzander   (1000)        1 2023-01-31 12:42:09.000000 aocref-2.0.8/aocref.egg-info/dependency_links.txt
--rw-rw-r--   0 mzander   (1000) mzander   (1000)       15 2023-01-31 12:42:09.000000 aocref-2.0.8/aocref.egg-info/top_level.txt
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.858869 aocref-2.0.8/scripts/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)        0 2022-06-19 00:32:13.000000 aocref-2.0.8/scripts/__init__.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     4956 2022-09-22 17:48:33.000000 aocref-2.0.8/scripts/aoeelo.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     2137 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/ci.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     1101 2023-01-14 18:32:33.000000 aocref-2.0.8/scripts/cities.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)      468 2022-01-28 19:23:17.000000 aocref-2.0.8/scripts/convert.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     1367 2023-01-29 15:49:35.000000 aocref-2.0.8/scripts/discord.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     1245 2022-06-19 00:39:33.000000 aocref-2.0.8/scripts/helpers.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     4931 2023-01-16 14:06:51.000000 aocref-2.0.8/scripts/liquipedia.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     4681 2023-01-14 23:54:41.000000 aocref-2.0.8/scripts/new_players.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     5549 2022-11-03 19:51:13.000000 aocref-2.0.8/scripts/teams.py
-drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-01-31 12:42:09.862870 aocref-2.0.8/scripts/util/
--rw-rw-r--   0 mzander   (1000) mzander   (1000)       27 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/__init__.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     7222 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/data_processor.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     1263 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/error.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)    16630 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/index.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     2299 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/io.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)      535 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/platforms.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     6914 2022-01-16 16:52:43.000000 aocref-2.0.8/scripts/util/players.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     3137 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/requests.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)     2332 2021-11-09 13:20:39.000000 aocref-2.0.8/scripts/util/teams.py
--rw-rw-r--   0 mzander   (1000) mzander   (1000)       38 2023-01-31 12:42:09.862870 aocref-2.0.8/setup.cfg
--rw-rw-r--   0 mzander   (1000) mzander   (1000)      361 2023-01-31 12:42:03.000000 aocref-2.0.8/setup.py
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.491064 aocref-2.0.9/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)       66 2021-04-18 17:22:22.000000 aocref-2.0.9/MANIFEST.in
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)      198 2023-05-07 23:22:07.491064 aocref-2.0.9/PKG-INFO
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     1337 2023-03-07 19:48:09.000000 aocref-2.0.9/README.md
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.483065 aocref-2.0.9/aocref/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)        0 2021-04-11 14:48:02.000000 aocref-2.0.9/aocref/__init__.py
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.483065 aocref-2.0.9/aocref/data/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     2399 2023-04-11 23:26:37.000000 aocref-2.0.9/aocref/data/constants.json
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.483065 aocref-2.0.9/aocref/data/datasets/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)    34711 2021-11-07 15:50:27.000000 aocref-2.0.9/aocref/data/datasets/0.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)    55361 2021-11-07 15:50:27.000000 aocref-2.0.9/aocref/data/datasets/1.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)    62436 2023-01-09 21:00:47.000000 aocref-2.0.9/aocref/data/datasets/100.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     1075 2023-05-07 23:21:32.000000 aocref-2.0.9/aocref/data/datasets/101.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     9039 2021-11-07 15:50:27.000000 aocref-2.0.9/aocref/data/datasets/2.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     8065 2021-11-07 15:50:27.000000 aocref-2.0.9/aocref/data/datasets/200.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)    58550 2021-11-07 15:50:27.000000 aocref-2.0.9/aocref/data/datasets/300.json
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)    52141 2021-11-07 15:50:27.000000 aocref-2.0.9/aocref/data/datasets/7.json
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.483065 aocref-2.0.9/aocref.egg-info/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)      198 2023-05-07 23:22:07.000000 aocref-2.0.9/aocref.egg-info/PKG-INFO
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)      833 2023-05-07 23:22:07.000000 aocref-2.0.9/aocref.egg-info/SOURCES.txt
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)        1 2023-05-07 23:22:07.000000 aocref-2.0.9/aocref.egg-info/dependency_links.txt
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)       15 2023-05-07 23:22:07.000000 aocref-2.0.9/aocref.egg-info/top_level.txt
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.487064 aocref-2.0.9/scripts/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)        0 2022-06-19 00:32:13.000000 aocref-2.0.9/scripts/__init__.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     4956 2022-09-22 17:48:33.000000 aocref-2.0.9/scripts/aoeelo.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     2137 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/ci.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     1101 2023-01-14 18:32:33.000000 aocref-2.0.9/scripts/cities.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)      468 2022-01-28 19:23:17.000000 aocref-2.0.9/scripts/convert.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     1367 2023-01-29 15:49:35.000000 aocref-2.0.9/scripts/discord.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     1245 2022-06-19 00:39:33.000000 aocref-2.0.9/scripts/helpers.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     4909 2023-02-19 22:01:28.000000 aocref-2.0.9/scripts/liquipedia.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     4674 2023-05-04 14:33:22.000000 aocref-2.0.9/scripts/new_players.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     5540 2023-04-23 14:56:06.000000 aocref-2.0.9/scripts/teams.py
+drwxrwxr-x   0 mzander   (1000) mzander   (1000)        0 2023-05-07 23:22:07.491064 aocref-2.0.9/scripts/util/
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)       27 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/__init__.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     7222 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/data_processor.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     1263 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/error.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)    16630 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/index.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     2299 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/io.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)      535 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/platforms.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     6914 2022-01-16 16:52:43.000000 aocref-2.0.9/scripts/util/players.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     3137 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/requests.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)     2332 2021-11-09 13:20:39.000000 aocref-2.0.9/scripts/util/teams.py
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)       38 2023-05-07 23:22:07.491064 aocref-2.0.9/setup.cfg
+-rw-rw-r--   0 mzander   (1000) mzander   (1000)      361 2023-05-07 21:50:24.000000 aocref-2.0.9/setup.py
```

### Comparing `aocref-2.0.8/README.md` & `aocref-2.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 Most data changes rarely. However, the player data needs to be consistently updated. Assistance would be welcomed.
 
 ### Player Notability
 
 Only notable players for games of the Age of Empires franchise may be added. Notability is defined as meeting at least one of the following criteria:
 
-1. Has a page on the [Age of Empires Liquipedia](https://liquipedia.net/ageofempires/Main_Page).
+1. Has a notable player page on the [Age of Empires Liquipedia](https://liquipedia.net/ageofempires/Main_Page).
 1. Was ever a top 200 player listed on [Aoe Tournament Elo](https://aoe-elo.com/).
-1. Was ever a top 250 player on the [primary competitive 1v1 ladder](https://www.ageofempires.com/stats/) for at least one month.
+1. Was ever a top 250 player on the [primary competitive 1v1 ladder](https://www.ageofempires.com/stats/) for at least one month while actively playing.
 1. Is a [Twitch Partner](https://www.twitch.tv/p/partners/) and primarily streams a game of the Age of Empires franchise.
 
 Other players may be added based on the maintainer's discretion for the benefit of the community at large.
 
 ### Team Notability
 
 Only notable teams may be added. A team is notable if it has at least one player meeting any of the first three player notability requirements.
```

### Comparing `aocref-2.0.8/aocref/data/constants.json` & `aocref-2.0.9/aocref/data/constants.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/0.json` & `aocref-2.0.9/aocref/data/datasets/0.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/1.json` & `aocref-2.0.9/aocref/data/datasets/1.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/100.json` & `aocref-2.0.9/aocref/data/datasets/100.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/2.json` & `aocref-2.0.9/aocref/data/datasets/2.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/200.json` & `aocref-2.0.9/aocref/data/datasets/200.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/300.json` & `aocref-2.0.9/aocref/data/datasets/300.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref/data/datasets/7.json` & `aocref-2.0.9/aocref/data/datasets/7.json`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/aocref.egg-info/SOURCES.txt` & `aocref-2.0.9/aocref.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 aocref.egg-info/SOURCES.txt
 aocref.egg-info/dependency_links.txt
 aocref.egg-info/top_level.txt
 aocref/data/constants.json
 aocref/data/datasets/0.json
 aocref/data/datasets/1.json
 aocref/data/datasets/100.json
+aocref/data/datasets/101.json
 aocref/data/datasets/2.json
 aocref/data/datasets/200.json
 aocref/data/datasets/300.json
 aocref/data/datasets/7.json
 scripts/__init__.py
 scripts/aoeelo.py
 scripts/ci.py
```

### Comparing `aocref-2.0.8/scripts/aoeelo.py` & `aocref-2.0.9/scripts/aoeelo.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/ci.py` & `aocref-2.0.9/scripts/ci.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/cities.py` & `aocref-2.0.9/scripts/cities.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/discord.py` & `aocref-2.0.9/scripts/discord.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/helpers.py` & `aocref-2.0.9/scripts/helpers.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/liquipedia.py` & `aocref-2.0.9/scripts/liquipedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 LOGGER = logging.getLogger(__name__)
 WAIT_SECS = 30
 PAGE_SIZE = 500
 CONDITIONS = [
     'Category:Age of Empires II Players',
-    'Is player::true'
 ]
 PROPS = [
     'Has id',
     'Has team',
     'Has twitch stream',
     'Has youtube channel',
     'Has twitter'
```

### Comparing `aocref-2.0.8/scripts/new_players.py` & `aocref-2.0.9/scripts/new_players.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 BLACKLIST = ['simtom', 'Ardeshir', 'Adam', 'Maxxtro', 'Xerxes', 'GyoreE', 'trombone', 'Rideg', 'Kiwi', '']
 LOGGER = logging.getLogger(__name__)
 WAIT_SECS = 30
 PAGE_SIZE = 500
 CONDITIONS = [
     'Category:Age of Empires II Players',
-    'Is player::true',
+    #'Is player::true',
     'Has aoe2net id::+'
 ]
 PROPS = [
     'Has pagename',
 ]
 HEADERS = {'User-Agent': 'https://github.com/SiegeEngineers/aoc-reference-data'}
 API = "https://liquipedia.net/ageofempires/api.php"
@@ -41,15 +41,14 @@
             'User-Agent': 'https://github.com/SiegeEngineers/aoc-reference-data'
         })
 
         try:
             data = resp.json()
         except json.decoder.JSONDecodeError:
             LOGGER.exception("failed to fetch: %s", resp.content)
-
         for result in data['query']['results'].values():
             record = result['printouts']
             page = record['Has pagename'][0]['fulltext']
             name = record['Has pagename'][0]['displaytitle']
             url = record['Has pagename'][0]['fullurl']
             output.append(dict(page=page, name=name, url=url))
 
@@ -87,14 +86,15 @@
     return name.lower().replace("_", " ").strip()
 
 def find_new(result_data, player_data, last_id):
     seen = set([clean(p['liquipedia']) for p in player_data if 'liquipedia' in p])
     seen |= set([clean(p['name']) for p in player_data])
     for n in result_data:
         if clean(n['name']) not in seen:
+            print("WHO", n['name'])
             props = get_props(n['page'], ['country', 'aoe2net_id', 'aoe-elo.com_id'])
             if 'aoe2net_id' not in props or not props['aoe2net_id']:
                 print(f"error: no aoe2net id for {n['name']}")
                 continue
             country_code = pycountry.countries.search_fuzzy(props['country'])[0].alpha_2.lower()
             last_id += 1
             if n['name'] in BLACKLIST:
@@ -105,15 +105,14 @@
                 country=country_code,
                 platforms=dict(
                     rl=[x.strip() for x in props['aoe2net_id'].split(',')]
                 ),
                 liquipedia=n['name'],
                 id=last_id,
                 aoeelo=int(props['aoe-elo.com_id']) if 'aoe-elo.com_id' in props and props['aoe-elo.com_id'] else None,
-                notability=dict(aoe2=True)
             ))
 
 
 def strip_leading_double_space(stream):
     if stream.startswith("  "):
         stream = stream[2:]
     return stream.replace("\n  ", "\n")
```

### Comparing `aocref-2.0.8/scripts/teams.py` & `aocref-2.0.9/scripts/teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,22 @@
 
 BLACKLIST = ['simtom']
 LOGGER = logging.getLogger(__name__)
 WAIT_SECS = 30
 PAGE_SIZE = 500
 SQUAD_CONDITIONS = [
     'Is number in roster::>0',
-    'Is player::true',
     'Is active::true'
 ]
 SQUAD_PROPS = [
     'Has id',
     'Has team'
 ]
 PLAYER_CONDITIONS = [
     'Category:Age of Empires II Players',
-    'Is player::true'
 ]
 PLAYER_PROPS = [
     'Has pagename',
     'Has team'
 ]
 HEADERS = {'User-Agent': 'https://github.com/SiegeEngineers/aoc-reference-data'}
 API = "https://liquipedia.net/ageofempires/api.php"
@@ -88,15 +86,16 @@
 
 
 MANUAL = {
     'CZ': {'Skull'},
     'Hot Young Masters': {'Dr.Kozmonot', 'Ubetnir'},
     'One Punch': {'fatman'},
     'Dark Empire': {'Xhing'},
-    'İstanbul Wildcats': {'Kasva'}
+    'İstanbul Wildcats': {'Kasva'},
+    'Clown Legion': {'Blackheart'}
 }
 
 def main():
     logging.basicConfig(level=logging.INFO)
 
     yaml = YAML()
     yaml.indent(sequence=4, offset=2)
```

### Comparing `aocref-2.0.8/scripts/util/data_processor.py` & `aocref-2.0.9/scripts/util/data_processor.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/error.py` & `aocref-2.0.9/scripts/util/error.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/index.py` & `aocref-2.0.9/scripts/util/index.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/io.py` & `aocref-2.0.9/scripts/util/io.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/platforms.py` & `aocref-2.0.9/scripts/util/platforms.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/players.py` & `aocref-2.0.9/scripts/util/players.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/requests.py` & `aocref-2.0.9/scripts/util/requests.py`

 * *Files identical despite different names*

### Comparing `aocref-2.0.8/scripts/util/teams.py` & `aocref-2.0.9/scripts/util/teams.py`

 * *Files identical despite different names*

