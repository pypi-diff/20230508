# Comparing `tmp/lightning_rod-0.1.0.tar.gz` & `tmp/lightning_rod-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.1.0.tar", max compression
+gzip compressed data, was "lightning_rod-0.2.0.tar", max compression
```

## Comparing `lightning_rod-0.1.0.tar` & `lightning_rod-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1061 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/LICENSE
--rw-r--r--   0        0        0      347 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/README.md
--rw-r--r--   0        0        0      307 2023-04-23 21:36:34.750693 lightning_rod-0.1.0/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      567 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4614 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       36 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0      144 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     1593 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      581 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     2418 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0       35 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0      374 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/rebindable.bolt
--rw-r--r--   0        0        0       86 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1047 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2111 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-04-23 21:35:36.721408 lightning_rod-0.1.0/lightning_rod/py.typed
--rw-r--r--   0        0        0     1238 2023-04-23 21:36:34.770694 lightning_rod-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 lightning_rod-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/LICENSE
+-rw-r--r--   0        0        0      347 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/README.md
+-rw-r--r--   0        0        0      307 2023-05-08 17:01:07.385005 lightning_rod-0.2.0/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      601 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4614 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       36 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      144 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     1593 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      581 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     2418 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0       35 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0      374 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/rebindable.bolt
+-rw-r--r--   0        0        0       86 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1047 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2111 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1238 2023-05-08 17:01:07.401005 lightning_rod-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 lightning_rod-0.2.0/PKG-INFO
```

### Comparing `lightning_rod-0.1.0/LICENSE` & `lightning_rod-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/api.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/api.bolt`

 * *Files 3% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 from ./effect import effect, raw_effect
 from ./give import give
 from ./clear import clear
 from ./gamemode import get_gamemode, set_gamemode
 from ./math import random, sqrt, pow
 from ./time import get_gametime, get_time, get_day, set_time
 from ./xp import get_xp, get_level, set_xp, set_level, set_xp_percent
+from ./comment import add_comment
```

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/bossbar.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/effect.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/gamemode.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/gamemode.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/math.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/math.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/time.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/time.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/lightning_rod/modules/xp.bolt` & `lightning_rod-0.2.0/lightning_rod/modules/xp.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.1.0/pyproject.toml` & `lightning_rod-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.1.0"
+version = "0.2.0"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
```

### Comparing `lightning_rod-0.1.0/PKG-INFO` & `lightning_rod-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-rod
-Version: 0.1.0
+Version: 0.2.0
 Summary: Function library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/lightning-rod
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

