# Comparing `tmp/el_decko_core-2023.5.6.1.tar.gz` & `tmp/el_decko_core-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "el_decko_core-2023.5.6.1.tar", last modified: Sat May  6 21:08:18 2023, max compression
+gzip compressed data, was "el_decko_core-2023.5.7.tar", last modified: Sun May  7 17:09:37 2023, max compression
```

## Comparing `el_decko_core-2023.5.6.1.tar` & `el_decko_core-2023.5.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:08:18.326711 el_decko_core-2023.5.6.1/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.6.1/LICENSE
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4806 2023-05-06 21:08:18.326711 el_decko_core-2023.5.6.1/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4440 2023-05-06 21:00:41.000000 el_decko_core-2023.5.6.1/README.md
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:08:18.326711 el_decko_core-2023.5.6.1/ed_core/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      996 2023-05-06 21:05:13.000000 el_decko_core-2023.5.6.1/ed_core/__init__.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.6.1/ed_core/dyn_data.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1818 2023-05-06 19:47:12.000000 el_decko_core-2023.5.6.1/ed_core/streamdeck.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.6.1/ed_core/streamdeck_config.py
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:08:18.326711 el_decko_core-2023.5.6.1/el_decko_core.egg-info/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4806 2023-05-06 21:08:18.000000 el_decko_core-2023.5.6.1/el_decko_core.egg-info/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-05-06 21:08:18.000000 el_decko_core-2023.5.6.1/el_decko_core.egg-info/SOURCES.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-06 21:08:18.000000 el_decko_core-2023.5.6.1/el_decko_core.egg-info/dependency_links.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      104 2023-05-06 21:08:18.000000 el_decko_core-2023.5.6.1/el_decko_core.egg-info/entry_points.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-06 21:08:18.000000 el_decko_core-2023.5.6.1/el_decko_core.egg-info/requires.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-06 21:08:18.000000 el_decko_core-2023.5.6.1/el_decko_core.egg-info/top_level.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      831 2023-05-06 21:05:06.000000 el_decko_core-2023.5.6.1/pyproject.toml
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-06 21:08:18.326711 el_decko_core-2023.5.6.1/setup.cfg
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.7/LICENSE
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4440 2023-05-06 21:00:41.000000 el_decko_core-2023.5.7/README.md
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/ed_core/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1213 2023-05-07 16:58:46.000000 el_decko_core-2023.5.7/ed_core/__init__.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.7/ed_core/dyn_data.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1663 2023-05-07 16:56:06.000000 el_decko_core-2023.5.7/ed_core/streamdeck.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.7/ed_core/streamdeck_config.py
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/el_decko_core.egg-info/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       40 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/entry_points.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/requires.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-07 17:09:37.000000 el_decko_core-2023.5.7/el_decko_core.egg-info/top_level.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      740 2023-05-07 16:57:24.000000 el_decko_core-2023.5.7/pyproject.toml
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-07 17:09:37.144622 el_decko_core-2023.5.7/setup.cfg
```

### Comparing `el_decko_core-2023.5.6.1/LICENSE` & `el_decko_core-2023.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.6.1/PKG-INFO` & `el_decko_core-2023.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: el_decko_core
-Version: 2023.5.6.1
+Version: 2023.5.7
 Summary: El Decko Core
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_core
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_core/issues
 Platform: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: backends
```

### Comparing `el_decko_core-2023.5.6.1/README.md` & `el_decko_core-2023.5.7/README.md`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.6.1/ed_core/__init__.py` & `el_decko_core-2023.5.7/ed_core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import threading
 from importlib.metadata import entry_points
 
 from ed_core import streamdeck
 from ed_core.streamdeck_config import load_config, apply_config
 
-VERSION = "2023.5.6.1"
+VERSION = "2023.5.7"
 BACKENDS = {}
 
 
-def run():
+def run(standalone: bool = True):
     try:
         print("El Decko Core running.")
         load_config()
         discovered_backends = entry_points(group='eldecko.backend')
         for edb in discovered_backends:
             edb_id = edb.value.split(":")[0]
             edb_function = edb.load()
@@ -20,14 +21,20 @@
                 edb_function()
             else:
                 if edb_id not in BACKENDS:
                     BACKENDS[edb_id] = {}
                 BACKENDS[edb_id][edb_name] = edb_function
 
         streamdeck.initialize(BACKENDS)
+        if standalone:
+            for t in threading.enumerate():
+                try:
+                    t.join()
+                except RuntimeError:
+                    pass
     except KeyboardInterrupt:
         streamdeck.shutdown()
         for backend in BACKENDS:
             print(backend)
             shutdown = BACKENDS[backend]["stop"]
             shutdown()
```

### Comparing `el_decko_core-2023.5.6.1/ed_core/dyn_data.py` & `el_decko_core-2023.5.7/ed_core/dyn_data.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.6.1/ed_core/streamdeck.py` & `el_decko_core-2023.5.7/ed_core/streamdeck.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import threading
-
 from StreamDeck.DeviceManager import DeviceManager
 from StreamDeck.Devices.StreamDeck import StreamDeck
 
 from ed_core import streamdeck_config
 
 stream_decks = DeviceManager().enumerate()
 backends = []
@@ -22,20 +20,14 @@
         print("Opened '{}' device (serial number: '{}', fw: '{}')".format(
             deck.deck_type(), deck.get_serial_number(), deck.get_firmware_version()
         ))
 
         streamdeck_config.apply_config(deck)
         deck.set_key_callback(__key_change_callback)
 
-        for t in threading.enumerate():
-            try:
-                t.join()
-            except RuntimeError:
-                pass
-
 
 def shutdown():
     for index, deck in enumerate(stream_decks):
         if not deck.is_visual():
             continue
         deck.reset()
         deck.close()
```

### Comparing `el_decko_core-2023.5.6.1/ed_core/streamdeck_config.py` & `el_decko_core-2023.5.7/ed_core/streamdeck_config.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.6.1/el_decko_core.egg-info/PKG-INFO` & `el_decko_core-2023.5.7/el_decko_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: el-decko-core
-Version: 2023.5.6.1
+Version: 2023.5.7
 Summary: El Decko Core
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_core
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_core/issues
 Platform: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: backends
```

