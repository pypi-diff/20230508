# Comparing `tmp/mgz-1.8.8.tar.gz` & `tmp/mgz-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgz-1.8.8.tar", last modified: Thu Mar 30 14:14:43 2023, max compression
+gzip compressed data, was "mgz-1.8.9.tar", last modified: Sun Apr  9 14:27:43 2023, max compression
```

## Comparing `mgz-1.8.8.tar` & `mgz-1.8.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.675947 mgz-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 14:14:27.000000 mgz-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-30 14:14:43.675947 mgz-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-30 14:14:27.000000 mgz-1.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz/body/
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/body/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/body/achievements.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/body/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/body/embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/common/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/common/diplomacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/common/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz/fast/
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/fast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/fast/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/fast/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/fast/header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz/header/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/achievements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/hd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/lobby.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/map_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/playerstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/header/unit_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz/model/
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/model/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/model/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/model/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.675947 mgz-1.8.8/mgz/summary/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/players.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/summary/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-03-30 14:14:27.000000 mgz-1.8.8/mgz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:14:43.671947 mgz-1.8.8/mgz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-30 14:14:43.000000 mgz-1.8.8/mgz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-30 14:14:43.000000 mgz-1.8.8/mgz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 14:14:43.000000 mgz-1.8.8/mgz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-30 14:14:43.000000 mgz-1.8.8/mgz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 14:14:43.000000 mgz-1.8.8/mgz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 14:14:43.000000 mgz-1.8.8/mgz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 14:14:43.675947 mgz-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-30 14:14:27.000000 mgz-1.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.699525 mgz-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 14:27:30.000000 mgz-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 14:27:43.699525 mgz-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-09 14:27:30.000000 mgz-1.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.695526 mgz-1.8.9/mgz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.695526 mgz-1.8.9/mgz/body/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/body/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/body/achievements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/body/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/body/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.695526 mgz-1.8.9/mgz/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/common/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/common/diplomacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/common/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.695526 mgz-1.8.9/mgz/fast/
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/fast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/fast/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/fast/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/fast/header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.699525 mgz-1.8.9/mgz/header/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/achievements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/hd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/lobby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/map_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/playerstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/header/unit_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.699525 mgz-1.8.9/mgz/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/model/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/model/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/model/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.699525 mgz-1.8.9/mgz/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/summary/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-04-09 14:27:30.000000 mgz-1.8.9/mgz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:27:43.695526 mgz-1.8.9/mgz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 14:27:43.000000 mgz-1.8.9/mgz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-09 14:27:43.000000 mgz-1.8.9/mgz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:27:43.000000 mgz-1.8.9/mgz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 14:27:43.000000 mgz-1.8.9/mgz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 14:27:43.000000 mgz-1.8.9/mgz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 14:27:43.000000 mgz-1.8.9/mgz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:27:43.699525 mgz-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-09 14:27:30.000000 mgz-1.8.9/setup.py
```

### Comparing `mgz-1.8.8/LICENSE` & `mgz-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/README.md` & `mgz-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/__init__.py` & `mgz-1.8.9/mgz/__init__.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/body/__init__.py` & `mgz-1.8.9/mgz/body/__init__.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/body/achievements.py` & `mgz-1.8.9/mgz/body/achievements.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/body/actions.py` & `mgz-1.8.9/mgz/body/actions.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/body/embedded.py` & `mgz-1.8.9/mgz/body/embedded.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/cli.py` & `mgz-1.8.9/mgz/cli.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/common/chat.py` & `mgz-1.8.9/mgz/common/chat.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/common/diplomacy.py` & `mgz-1.8.9/mgz/common/diplomacy.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/common/map.py` & `mgz-1.8.9/mgz/common/map.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/const.py` & `mgz-1.8.9/mgz/const.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/enums.py` & `mgz-1.8.9/mgz/enums.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/fast/__init__.py` & `mgz-1.8.9/mgz/fast/__init__.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/fast/actions.py` & `mgz-1.8.9/mgz/fast/actions.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/fast/enums.py` & `mgz-1.8.9/mgz/fast/enums.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/fast/header.py` & `mgz-1.8.9/mgz/fast/header.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/achievements.py` & `mgz-1.8.9/mgz/header/achievements.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/ai.py` & `mgz-1.8.9/mgz/header/ai.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/de.py` & `mgz-1.8.9/mgz/header/de.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/hd.py` & `mgz-1.8.9/mgz/header/hd.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/initial.py` & `mgz-1.8.9/mgz/header/initial.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/lobby.py` & `mgz-1.8.9/mgz/header/lobby.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/map_info.py` & `mgz-1.8.9/mgz/header/map_info.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/objects.py` & `mgz-1.8.9/mgz/header/objects.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/playerstats.py` & `mgz-1.8.9/mgz/header/playerstats.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/replay.py` & `mgz-1.8.9/mgz/header/replay.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/scenario.py` & `mgz-1.8.9/mgz/header/scenario.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/header/unit_type.py` & `mgz-1.8.9/mgz/header/unit_type.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/model/__init__.py` & `mgz-1.8.9/mgz/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,19 @@
                     if action_type not in AI_ACTIONS:
                         eapm[action_data['player_id']] += 1
                     action.player = players[action_data['player_id']]
                     del action.payload['player_id']
                 enrich_action(action, action_data, dataset, consts)
                 actions.append(action)
                 inputs.add_action(action)
+            elif op_type is fast.Operation.POSTGAME:
+                # Write down the rating of each player after the game ended.
+                players_data: list = op_data["leaderboards"][0]["players"]
+                for player, player_data in zip(players.values(), players_data):
+                    player.rate_snapshot = player_data["rating"]
         except EOFError:
             break
 
     # Compute winner(s)
     for team in teams:
         winner = not any([player for player in team if player in resigned])
         if resigned:
```

### Comparing `mgz-1.8.8/mgz/model/compat.py` & `mgz-1.8.9/mgz/model/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 color_id=p.color_id,
                 human=True,
                 winner=p.winner,
                 user_id=p.profile_id,
                 position=(p.position.x, p.position.y),
                 mvp=None,
                 score=None,
-                rate_snapshot=None,
+                rate_snapshot=p.rate_snapshot,
                 cheater=None,
                 achievements=empty_achievements(),
                 prefer_random=p.prefer_random,
                 eapm=p.eapm
             ) for p in self.match.players
         ]
```

### Comparing `mgz-1.8.8/mgz/model/definitions.py` & `mgz-1.8.9/mgz/model/definitions.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/model/inputs.py` & `mgz-1.8.9/mgz/model/inputs.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/reference.py` & `mgz-1.8.9/mgz/reference.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/__init__.py` & `mgz-1.8.9/mgz/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/dataset.py` & `mgz-1.8.9/mgz/summary/dataset.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/full.py` & `mgz-1.8.9/mgz/summary/full.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/objects.py` & `mgz-1.8.9/mgz/summary/objects.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/players.py` & `mgz-1.8.9/mgz/summary/players.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/settings.py` & `mgz-1.8.9/mgz/summary/settings.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/summary/teams.py` & `mgz-1.8.9/mgz/summary/teams.py`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/mgz/util.py` & `mgz-1.8.9/mgz/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,29 @@
 
 # pylint: disable=abstract-method,protected-access
 
 LOGGER = logging.getLogger(__name__)
 SEARCH_MAX_BYTES = 3000
 POSTGAME_LENGTH = 2096
 LOOKAHEAD = 9
+DE_MARKERS = {
+    38: b"\xa4\x70\xbd\x3f",
+    37: b"\xf6\x28\xbc\x3f",
+    26.21: b"\xf6\x28\xbc\x3f",
+    26.16: b"\x48\xe1\xba\x3f",
+    25.06: b"\x9a\x99\xb9\x3f",
+    25.03: b"\x85\xeb\x91\x3f",
+    25.02: b"\xec\x51\xb8\x3f",
+    25.01: b"\x3d\x0a\xb7\x3f",
+    20.16: b"\x8f\xc2\xb5\x3f",
+    20.06: b"\xe1\x7a\xb4\x3f",
+    13.34: b"\x33\x33\xb3\x3f",
+    13.07: b"\x29\x5c\xaf\x3f",
+    12.97: b"\x7b\x14\xae\x3f"
+}
 
 
 class Version(Enum):
     """Version enumeration.
 
     Using consts from https://github.com/goto-bus-stop/recanalyst/blob/master/src/Model/Version.php
     for consistency.
@@ -252,14 +267,15 @@
 
     # pylint: disable=chained-comparison, too-many-locals
     def _parse(self, stream, context, path):
         """Parse until the end of objects data."""
         num_players = context._._.replay.num_players
         marker_num = context.attributes.num_header_data
         save_version = context._._.save_version
+        version = find_version(context)
         start = stream.tell()
         # Have to read everything to be able to use find()
         read_bytes = stream.read()
         # Try to find the first marker, a portion of the next player structure
         # The byte that changes is the number of player stats fields
         marker = read_bytes.find(b'\x16' + struct.pack('<I', int(marker_num)) + b'\x21')
         # If it exists, we're not on the last player yet
@@ -274,52 +290,30 @@
         # Otherwise, this is the last player
         else:
             # Search for the scenario header
             # TODO: make this section more reliable
             marker_aok = read_bytes.find(b"\x9a\x99\x99\x3f")
             marker_up = read_bytes.find(b"\xf6\x28\x9c\x3f")
             marker_hd = read_bytes.find(b"\xae\x47\xa1\x3f")
-            if save_version >= 38:
-                marker_de = read_bytes.find(b"\xa4\x70\xbd\x3f")
-            elif save_version >= 37:
-                marker_de = read_bytes.find(b"\xf6\x28\xbc\x3f")
-            elif save_version >= 26.21:
-                marker_de = read_bytes.find(b"\xf6\x28\xbc\x3f")
-            elif save_version >= 26.16:
-                marker_de = read_bytes.find(b"\x48\xe1\xba\x3f")
-            elif save_version >= 25.06:
-                marker_de = read_bytes.find(b"\x9a\x99\xb9\x3f")
-            elif save_version >= 25.03:
-                marker_de = read_bytes.find(b"\x85\xeb\x91\x3f")
-            elif save_version >= 25.02:
-                marker_de = read_bytes.find(b"\xec\x51\xb8\x3f")
-            elif save_version >= 25.01:
-                marker_de = read_bytes.find(b"\x3d\x0a\xb7\x3f")
-            elif save_version >= 20.16:
-                marker_de = read_bytes.find(b"\x8f\xc2\xb5\x3f")
-            elif save_version >= 20.06:
-                marker_de = read_bytes.find(b"\xe1\x7a\xb4\x3f")
-            elif save_version >= 13.34:
-                marker_de = read_bytes.find(b"\x33\x33\xb3\x3f")
-            elif save_version >= 13.07:
-                marker_de = read_bytes.find(b"\x29\x5c\xaf\x3f")
-            else:
-                marker_de = read_bytes.find(b"\x7b\x14\xae\x3f")
-            new_marker = -1
-            if marker_up > 0 and marker_de < 0 and marker_hd < 0: # aok marker can appear in up
-                new_marker = marker_up
-            elif marker_de > 0 and marker_up < 0 and marker_aok < 0 and marker_hd < 0:
-                new_marker = marker_de
-            elif marker_aok > 0 and marker_up < 0 and marker_de < 0 and marker_hd < 0:
-                new_marker = marker_aok
-            elif marker_hd > 0 and marker_up < 0 and marker_de < 0 and marker_aok < 0:
-                new_marker = marker_hd
-            if new_marker == -1:
+            marker_de = -1
+            for sv, search in DE_MARKERS.items():
+                if save_version >= sv:
+                    marker_de = read_bytes.find(search)
+                    break
+            marker = -1
+            if marker_aok > 0 and version is Version.AOK:
+                marker = marker_aok
+            elif marker_hd > 0 and version is Version.HD:
+                marker = marker_hd
+            elif marker_de > 0 and version is Version.DE:
+                marker = marker_de
+            elif marker_up > 0:
+                marker = marker_up
+            if marker == -1:
                 raise RuntimeError("could not find scenario marker")
-            marker = new_marker
             # Backtrack through the achievements and initial structure footer
             backtrack = ((1817 * (num_players - 1)) + 4 + 19)
         # Seek to the position we found
         end = start + marker - backtrack - 2
         stream.seek(end)
         return end
```

### Comparing `mgz-1.8.8/mgz.egg-info/SOURCES.txt` & `mgz-1.8.9/mgz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mgz-1.8.8/setup.py` & `mgz-1.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 from setuptools import setup, find_packages
 
 setup(
     name='mgz',
-    version='1.8.8',
+    version='1.8.9',
     description='Parse Age of Empires 2 recorded games.',
     url='https://github.com/happyleavesaoc/aoc-mgz/',
     license='MIT',
     author='happyleaves',
     author_email='happyleaves.tfr@gmail.com',
     packages=find_packages(),
     install_requires=[
```

