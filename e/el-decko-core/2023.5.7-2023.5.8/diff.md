# Comparing `tmp/el_decko_core-2023.5.7.tar.gz` & `tmp/el_decko_core-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "el_decko_core-2023.5.7.tar", last modified: Sun May  7 17:09:37 2023, max compression
+gzip compressed data, was "el_decko_core-2023.5.8.tar", last modified: Mon May  8 15:52:52 2023, max compression
```

## Comparing `el_decko_core-2023.5.7.tar` & `el_decko_core-2023.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.7/LICENSE
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4440 2023-05-06 21:00:41.000000 el_decko_core-2023.5.7/README.md
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/ed_core/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1213 2023-05-07 16:58:46.000000 el_decko_core-2023.5.7/ed_core/__init__.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.7/ed_core/dyn_data.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1663 2023-05-07 16:56:06.000000 el_decko_core-2023.5.7/ed_core/streamdeck.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.7/ed_core/streamdeck_config.py
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/el_decko_core.egg-info/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/SOURCES.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/dependency_links.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       40 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/entry_points.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/requires.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/top_level.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      740 2023-05-07 16:57:24.000000 el_decko_core-2023.5.7/pyproject.toml
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/setup.cfg
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.8/LICENSE
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4440 2023-05-06 21:00:41.000000 el_decko_core-2023.5.8/README.md
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/ed_core/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1315 2023-05-08 14:49:14.000000 el_decko_core-2023.5.8/ed_core/__init__.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.8/ed_core/dyn_data.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2015 2023-05-08 14:09:42.000000 el_decko_core-2023.5.8/ed_core/streamdeck.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.8/ed_core/streamdeck_config.py
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/el_decko_core.egg-info/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       40 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/entry_points.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/requires.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/top_level.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      740 2023-05-07 16:57:24.000000 el_decko_core-2023.5.8/pyproject.toml
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/setup.cfg
```

### Comparing `el_decko_core-2023.5.7/LICENSE` & `el_decko_core-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.7/PKG-INFO` & `el_decko_core-2023.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: el_decko_core
-Version: 2023.5.7
+Version: 2023.5.8
 Summary: El Decko Core
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_core
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_core/issues
 Platform: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: backends
```

### Comparing `el_decko_core-2023.5.7/README.md` & `el_decko_core-2023.5.8/README.md`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.7/ed_core/__init__.py` & `el_decko_core-2023.5.8/ed_core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 from importlib.metadata import entry_points
 
 from ed_core import streamdeck
 from ed_core.streamdeck_config import load_config, apply_config
 
-VERSION = "2023.5.7"
+VERSION = "2023.5.8"
 BACKENDS = {}
 
 
 def run(standalone: bool = True):
     try:
         print("El Decko Core running.")
         load_config()
@@ -28,16 +28,25 @@
         if standalone:
             for t in threading.enumerate():
                 try:
                     t.join()
                 except RuntimeError:
                     pass
     except KeyboardInterrupt:
-        streamdeck.shutdown()
-        for backend in BACKENDS:
-            print(backend)
-            shutdown = BACKENDS[backend]["stop"]
-            shutdown()
+        stop_core()
+
+
+def stop_core():
+    print("Stopping El Decko Core")
+    streamdeck.shutdown()
+    __stop_backends()
+
+
+def __stop_backends():
+    for backend in BACKENDS:
+        print(backend)
+        shutdown = BACKENDS[backend]["stop"]
+        shutdown()
 
 
 def backends():
     return BACKENDS
```

### Comparing `el_decko_core-2023.5.7/ed_core/dyn_data.py` & `el_decko_core-2023.5.8/ed_core/dyn_data.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.7/ed_core/streamdeck.py` & `el_decko_core-2023.5.8/ed_core/streamdeck.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,24 @@
     deck.key_count()
 
 
 def set_brightness(deck, brightness: int):
     deck.set_brightness(brightness)
 
 
+def get_key_config(deck_serial: str, key_num: int):
+    for index, deck in enumerate(stream_decks):
+        deck.open()
+        if deck.get_serial_number() == deck_serial:
+            streamdeck_config.load_config()
+            cfg = streamdeck_config.DECK_CFG[deck_serial]["key_config"][str(key_num)]
+            deck.close()
+            return cfg
+
+
 def __key_change_callback(deck: StreamDeck, key, state):
     if state:
         cfg = streamdeck_config.DECK_CFG[deck.get_serial_number()]
         edb_id: str = cfg["key_config"][str(key)]["backend"]
         edb_event: str = cfg["key_config"][str(key)]["event"]
         edb_params: dict = cfg["key_config"][str(key)]["event_parameters"]
         if edb_id:
```

### Comparing `el_decko_core-2023.5.7/ed_core/streamdeck_config.py` & `el_decko_core-2023.5.8/ed_core/streamdeck_config.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.7/el_decko_core.egg-info/PKG-INFO` & `el_decko_core-2023.5.8/el_decko_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: el-decko-core
-Version: 2023.5.7
+Version: 2023.5.8
 Summary: El Decko Core
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_core
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_core/issues
 Platform: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: backends
```

### Comparing `el_decko_core-2023.5.7/pyproject.toml` & `el_decko_core-2023.5.8/pyproject.toml`

 * *Files identical despite different names*

