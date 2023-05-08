# Comparing `tmp/pygameHat-1.1.1.tar.gz` & `tmp/pygameHat-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.1.1.tar", last modified: Wed Apr 26 17:55:18 2023, max compression
+gzip compressed data, was "pygameHat-1.1.2.tar", last modified: Mon May  8 13:22:02 2023, max compression
```

## Comparing `pygameHat-1.1.1.tar` & `pygameHat-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 17:55:18.575534 pygameHat-1.1.1/
--rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      543 2023-04-26 17:55:18.575534 pygameHat-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 17:55:18.404569 pygameHat-1.1.1/pygameHat/
--rw-rw-rw-   0        0        0    42191 2023-04-26 17:54:14.000000 pygameHat-1.1.1/pygameHat/__init__.py
--rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.1/pygameHat/pygameHat.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:55:18.568535 pygameHat-1.1.1/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      543 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 17:55:18.580534 pygameHat-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-04-26 17:54:25.000000 pygameHat-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:22:02.564541 pygameHat-1.1.2/
+-rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-05-08 13:22:02.565594 pygameHat-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 13:22:02.365582 pygameHat-1.1.2/pygameHat/
+-rw-rw-rw-   0        0        0    43860 2023-05-08 13:19:12.000000 pygameHat-1.1.2/pygameHat/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.2/pygameHat/pygameHat.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:22:02.545545 pygameHat-1.1.2/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:22:02.591503 pygameHat-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-05-08 13:21:54.000000 pygameHat-1.1.2/setup.py
```

### Comparing `pygameHat-1.1.1/PKG-INFO` & `pygameHat-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.1/pygameHat/__init__.py` & `pygameHat-1.1.2/pygameHat/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import pygame, sys, time, base64, os
+import pygame, sys, time, base64, os, json
 
 #pygame initialization
-version = "Beta 1.1.1"
+version = "Beta 1.1.2"
 print(f"\nAdditional hello from pygameHat {version} :D")
-print("\nThis version is not backwards compatible with pygameHat <= 1.0.7")
+print("\nThis version may not be compatible with older versions")
 
 pygame.init()
 pygame.font.init()
 try:
     pygame.mixer.init()
 except:
     print("WARNING: Failed to initialize audio!")
@@ -16,14 +16,15 @@
 class Object:
     def __init__(self):
         self.x = 0
         self.y = 0
         self.sprite = None
         self.visible = True
         self.active_timers = {}
+        self.tags = []
     
     def draw(self):
         draw_sprite(self.sprite, self.x, self.y)
     
     def step(self):
         pass
     def key_just_pressed(self, key):
@@ -204,19 +205,17 @@
         if key == pygame.K_F10 and Settings.enable_console:
             self.switch()
             key = ""
         
         if self.opened:
             self.text += unicode
         if key == pygame.K_RETURN:
-            try:
-                exec(self.text)
-                self.text = ""
-            except:
-                print("Something went wrong")
+            text_to_return = self.text
+            self.text = ""
+            return text_to_return
         elif key == pygame.K_BACKSPACE:
             self.delete_from_end()
     
     def delete_from_end(self):
         if len(self.text) > 0:
             self.text = self.text[:-2]
         
@@ -225,14 +224,27 @@
 
     def to_surface(self, string, size):
         return pygame.image.fromstring(base64.b64decode(string), size, "RGBA")
 
     def to_string(self, surface):
         return base64.b64encode(pygame.image.tostring(surface, "RGBA")).decode()
 surfaceStringifier = SurfaceStringifier()
+class SaveManager:
+    def save(self, jsonfile, path):
+        saveable = json.dumps(jsonfile, indent=4)
+        with open(path, "w") as file:
+            file.write(saveable)
+            file.close()
+        return saveable
+    def load(self, path):
+        with open(path, "rb") as file:
+            readable = file.read()
+            file.close()
+        return json.loads(readable)
+saveManager = SaveManager()
 
 #game settings
 class Settings:
     window_size = (1200, 700)
     room_size = (0, 0)
     window_title =  "pygameHat "+version
     fullscreen = False
@@ -243,14 +255,15 @@
 
     shameless_ad = True
 
 class RoomGotChanged(Exception):
     pass
 
 temp_icon = surfaceStringifier.to_surface("7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/3CSvv//////cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7//////3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw//////////////////////9wkr7/cJK+/3CSvv9wkr7/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw///yAP//8gD///IA///yAP//////////////////////7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD///IA///yAP//8gD///IA///yAP////////IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw///yAP//8gD///IA///yAP//8gD////////yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/w==", (70, 70))
+temp_icon = pygame.transform.scale(temp_icon, (32, 32))
 
 #first initializations
 debug_font = pygame.font.Font
 title_font = pygame.font.Font
 console_opened = False
 console = Console()
 delta_time = 0
@@ -262,60 +275,67 @@
 
 current_room = Room()
 changed_room = False
 
 def init():
     global screen, screen_size, debug_font, title_font
 
+    if Settings.icon:
+        pygame.display.set_icon(pygame.image.load(Settings.icon))
+    else:
+        pygame.display.set_icon(temp_icon)
+
     if Settings.font == "default":
         debug_font = pygame.font.Font(None, 25)
         title_font = pygame.font.Font(None, 100)
     else:
         debug_font = pygame.font.Font(Settings.font, 25)
         title_font = pygame.font.Font(Settings.font, 100)
 
     monitor = pygame.display.set_mode(Settings.window_size)
 
     rSX, rSY = Settings.room_size
     if not rSX and not rSY:
         Settings.room_size = Settings.window_size
 
-    if Settings.icon:
-        pygame.display.set_icon(pygame.image.load(Settings.icon).convert())
-    else:
-        pygame.display.set_icon(temp_icon)
     pygame.display.set_caption(Settings.window_title)
     screen.blit(title_font.render("Made with Pygame Hat", True, (255, 255, 255)), (100, 100))
     screen.blit(title_font.render(version, True, (255, 255, 255)), (100, 200))
     screen.blit(title_font.render("OWO", True, (255, 255, 255)), (100, 400))
 
     if Settings.shameless_ad:
         screen = pygame.transform.scale(screen, Settings.room_size).convert()
         monitor.blit(screen, (0, 0))
         pygame.display.flip()
         time.sleep(1.5)
     screen = pygame.surface.Surface(Settings.room_size)
     screen_size = Settings.window_size
 
-def compile_for_windows(main_file, output_directory, icon=None):
+def compile_for_windows(main_file, output_directory="./", icon=None):
     monitor = pygame.display.set_mode((900, 500))
     pygame.display.set_icon(temp_icon)
     pygame.display.set_caption("Compiler")
     monitor.blit(pygame.font.Font(None, 100).render("Please stand by", True, (255, 255, 255)), (100, 50))
     monitor.blit(pygame.font.Font(None, 100).render("(=>wO=)", True, (255, 255, 255)), (100, 150))
     pygame.display.flip()
 
     comm = ""
     if icon:
         comm = "--icon=%s" % icon
     
     os.system(f"pyinstaller --onefile --noconsole --distpath={output_directory} {comm} {main_file}")
 
-def add_object_instance(object, layer, position=(0, 0)):
-    object.x, object.y = position
+    monitor.fill((0, 0, 0))
+    monitor.blit(pygame.font.Font(None, 100).render("Done compiling!", True, (3, 252, 48)), (100, 50))
+    monitor.blit(pygame.font.Font(None, 100).render("(=OwO=)", True, (3, 252, 48)), (100, 150))
+    pygame.display.flip()
+
+def add_object_instance(object, layer, position="default"):
+    if position != "default":
+        object.x, object.y = position
     current_room.layers[layer].append(object)
     return object
 
 def find_object_by_class(object, multiple=False):
     found_objects = []
 
     for layer in current_room.layers:
@@ -327,14 +347,28 @@
         if multiple:
             return found_objects
         else:
             return found_objects[-1]
     else:
         return None
 
+def find_objects_by_tags(tag_list, searchtype="all"):
+    found_objects = []
+
+    if len(tag_list) > 0:
+        for layer in current_room.layers:
+            for instance in current_room.layers[layer]:
+                appearances = 0
+                for tag in tag_list:
+                    if tag in instance.tags:
+                        appearances += 1
+                if searchtype == "all" and appearances == len(tag_list) or searchtype == "any" and appearances > 0 or searchtype == "exall" and appearances == 0 or searchtype == "exany" and appearances < len(tag_list):
+                    found_objects.append(instance)
+    return found_objects
+
 def collide_objects(object1, object2):
     if object1 != object2 and object1.sprite and object1.sprite.collision and object2.sprite and object2.sprite.collision:
         object1_shape = object1.sprite.update_collision_shape_position(object1.x, object1.y)
         object2_shape = object2.sprite.update_collision_shape_position(object2.x, object2.y)
         if object1_shape.colliderect(object2_shape):
             return object2
 
@@ -404,14 +438,15 @@
     changed_room = True
 
 
 def start():
     timeB = 0
     last_input = None
     last_input_released = None
+    console_text = ""
     global delta_time, current_time
     global screen, screen_size
     global changed_room
 
     if Settings.fullscreen:
         monitor = pygame.display.set_mode(Settings.window_size, pygame.FULLSCREEN)
     else:
@@ -428,15 +463,15 @@
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
             
             elif event.type == pygame.KEYDOWN:
                 last_input = event.key
                 #console management
-                console.input(event.key, event.unicode)
+                console_text = console.input(event.key, event.unicode)
 
             elif event.type == pygame.KEYUP:
                 #handling keyups for objects
                 last_input_released = event.key
             
             elif event.type == pygame.MOUSEBUTTONDOWN:
                 last_input = event.button
@@ -483,7 +518,15 @@
         console.display()
 
         monitor.blit(pygame.transform.scale(screen, screen_size), (0, 0))
         pygame.display.flip()
 
         last_input = None
         last_input_released = None
+
+        #console_handling v2
+        if console_text:
+            try:
+                exec(console_text)
+            except:
+                print("Something went wrong!")
+            console_text = None
```

### Comparing `pygameHat-1.1.1/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.1.2/pygameHat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.1/setup.py` & `pygameHat-1.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'Pygame game-making engine'
 
 # Setting up
 setup(
     name="pygameHat",
     version=VERSION,
     author="Wojciech Błajda",
     #author_email="None",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pygame', 'pyinstaller'],
+    install_requires=["pygame", "sys", "time", "base64", "os", "json"],
     keywords=['python', 'engine', 'pygame', 'game', 'maker'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

