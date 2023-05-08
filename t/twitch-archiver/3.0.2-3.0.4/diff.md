# Comparing `tmp/twitch-archiver-3.0.2.tar.gz` & `tmp/twitch-archiver-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-archiver-3.0.2.tar", last modified: Mon May  8 13:22:40 2023, max compression
+gzip compressed data, was "twitch-archiver-3.0.4.tar", last modified: Mon May  8 13:49:20 2023, max compression
```

## Comparing `twitch-archiver-3.0.2.tar` & `twitch-archiver-3.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:22:40.674878 twitch-archiver-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 13:22:40.674878 twitch-archiver-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:22:40.674878 twitch-archiver-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:22:40.674878 twitch-archiver-3.0.2/twitch_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 13:22:40.000000 twitch-archiver-3.0.2/twitch_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 13:22:40.000000 twitch-archiver-3.0.2/twitch_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:22:40.000000 twitch-archiver-3.0.2/twitch_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 13:22:40.000000 twitch-archiver-3.0.2/twitch_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 13:22:40.000000 twitch-archiver-3.0.2/twitch_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:22:40.674878 twitch-archiver-3.0.2/twitcharchiver/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-05-08 13:22:26.000000 twitch-archiver-3.0.2/twitcharchiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:49:20.532226 twitch-archiver-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 13:49:20.532226 twitch-archiver-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:49:20.532226 twitch-archiver-3.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:49:20.528226 twitch-archiver-3.0.4/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:49:20.528226 twitch-archiver-3.0.4/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/utils.py
```

### Comparing `twitch-archiver-3.0.2/LICENSE` & `twitch-archiver-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/PKG-INFO` & `twitch-archiver-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.2
+Version: 3.0.4
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-3.0.2/README.md` & `twitch-archiver-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/pyproject.toml` & `twitch-archiver-3.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0", "requests>=2.25.1", "m3u8>=0.3.12"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "3.0.2"
+version = "3.0.4"
+dependencies = [
+    "requests>=2.25.1",
+    "m3u8>=0.3.12",
+]
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
 description = "A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitch-archiver-3.0.2/twitch_archiver.egg-info/PKG-INFO` & `twitch-archiver-3.0.4/twitch_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.2
+Version: 3.0.4
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-3.0.2/twitch_archiver.egg-info/SOURCES.txt` & `twitch-archiver-3.0.4/twitch_archiver.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 twitch_archiver.egg-info/PKG-INFO
 twitch_archiver.egg-info/SOURCES.txt
 twitch_archiver.egg-info/dependency_links.txt
 twitch_archiver.egg-info/entry_points.txt
+twitch_archiver.egg-info/requires.txt
 twitch_archiver.egg-info/top_level.txt
 twitcharchiver/__init__.py
 twitcharchiver/api.py
 twitcharchiver/arguments.py
 twitcharchiver/configuration.py
 twitcharchiver/database.py
 twitcharchiver/downloader.py
```

### Comparing `twitch-archiver-3.0.2/twitcharchiver/__init__.py` & `twitch-archiver-3.0.4/twitcharchiver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from twitcharchiver.configuration import Configuration
 from twitcharchiver.exceptions import TwitchAPIError
 from twitcharchiver.logger import Logger
 from twitcharchiver.processing import Processing
 from twitcharchiver.twitch import Twitch
 from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple, check_update_available
 
-__version__ = '3.0.2'
+__version__ = '3.0.4'
 
 
 def main():
     """
     Main processing for twitch-archiver.
     """
     parser = argparse.ArgumentParser(argument_default=None, description=textwrap.dedent(f"""\
```

### Comparing `twitch-archiver-3.0.2/twitcharchiver/api.py` & `twitch-archiver-3.0.4/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/arguments.py` & `twitch-archiver-3.0.4/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/configuration.py` & `twitch-archiver-3.0.4/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/database.py` & `twitch-archiver-3.0.4/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/downloader.py` & `twitch-archiver-3.0.4/twitcharchiver/downloader.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/exceptions.py` & `twitch-archiver-3.0.4/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/logger.py` & `twitch-archiver-3.0.4/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/processing.py` & `twitch-archiver-3.0.4/twitcharchiver/processing.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/stream.py` & `twitch-archiver-3.0.4/twitcharchiver/stream.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/twitch.py` & `twitch-archiver-3.0.4/twitcharchiver/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.2/twitcharchiver/utils.py` & `twitch-archiver-3.0.4/twitcharchiver/utils.py`

 * *Files identical despite different names*

