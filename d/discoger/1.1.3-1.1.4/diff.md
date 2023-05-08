# Comparing `tmp/discoger-1.1.3.tar.gz` & `tmp/discoger-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.3.tar", last modified: Tue May  2 20:53:56 2023, max compression
+gzip compressed data, was "discoger-1.1.4.tar", last modified: Mon May  8 21:28:04 2023, max compression
```

## Comparing `discoger-1.1.3.tar` & `discoger-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:56.298656 discoger-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 20:53:33.000000 discoger-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:53:56.298656 discoger-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 20:53:33.000000 discoger-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:56.298656 discoger-1.1.3/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:33.000000 discoger-1.1.3/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:53:33.000000 discoger-1.1.3/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-05-02 20:53:33.000000 discoger-1.1.3/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:56.298656 discoger-1.1.3/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 20:53:56.298656 discoger-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 20:53:33.000000 discoger-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:28:04.155207 discoger-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 21:27:48.000000 discoger-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 21:28:04.155207 discoger-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 21:27:48.000000 discoger-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:28:04.155207 discoger-1.1.4/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:27:48.000000 discoger-1.1.4/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 21:27:48.000000 discoger-1.1.4/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-05-08 21:27:48.000000 discoger-1.1.4/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:28:04.155207 discoger-1.1.4/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 21:28:04.155207 discoger-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 21:27:48.000000 discoger-1.1.4/setup.py
```

### Comparing `discoger-1.1.3/LICENSE` & `discoger-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.3/PKG-INFO` & `discoger-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.3
+Version: 1.1.4
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.3.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.4.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.3/README.md` & `discoger-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.1.3/discoger/discoger.py` & `discoger-1.1.4/discoger/discoger.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,19 +95,23 @@
 @bot.message_handler(regexp="^https://www.discogs.com/.*(release|master)/.*")
 def handle_message(message):
     release_info = dict()
     chat_id = message.chat.id
     release_id = re.findall(r'\d+', message.text)[0]
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     if not db.search("release_list[?release_id=='%s']" % (release_id)):
-        relase_all_info = d.release(release_id)
+        if len(re.findall(r'\/master\/\d+', message.text)) == 1:
+            master_release_info = d.master(release_id)
+            release_all_info = d.release(master_release_info.main_release.id)
+        else:
+            release_all_info = d.release(release_id)
         db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
         release_info["release_id"] = release_id
-        release_info["artist"] = relase_all_info.artists[0].name
-        release_info["title"] = relase_all_info.title
+        release_info["artist"] = release_all_info.artists[0].name
+        release_info["title"] = release_all_info.title
         release_info["url"] = message.text
         if len(re.findall(r'\/master\/\d+', message.text)) == 1:
             release_info["type"] = "master"
         else:
             release_info["type"] = "release"
         release_info["last_sell"] = dict()
         db["release_list"].append(release_info)
```

### Comparing `discoger-1.1.3/discoger.egg-info/PKG-INFO` & `discoger-1.1.4/discoger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.3
+Version: 1.1.4
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.3.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.4.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.3/setup.py` & `discoger-1.1.4/setup.py`

 * *Files identical despite different names*

