# Comparing `tmp/playgroundrl-0.0.7.tar.gz` & `tmp/playgroundrl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl-0.0.7.tar", last modified: Tue Apr 11 19:38:39 2023, max compression
+gzip compressed data, was "playgroundrl-0.0.8.tar", last modified: Tue Apr 11 19:54:28 2023, max compression
```

## Comparing `playgroundrl-0.0.7.tar` & `playgroundrl-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.720244 playgroundrl-0.0.7/
--rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:38:39.720313 playgroundrl-0.0.7/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      162 2023-04-08 20:30:44.000000 playgroundrl-0.0.7/README.md
--rw-r--r--   0 langston   (501) staff       (20)       38 2023-04-11 19:38:39.720487 playgroundrl-0.0.7/setup.cfg
--rw-r--r--   0 langston   (501) staff       (20)      443 2023-04-11 19:38:32.000000 playgroundrl-0.0.7/setup.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.717758 playgroundrl-0.0.7/src/
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.719127 playgroundrl-0.0.7/src/playgroundrl/
--rw-r--r--   0 langston   (501) staff       (20)        0 2023-04-08 20:30:44.000000 playgroundrl-0.0.7/src/playgroundrl/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     8937 2023-04-08 21:07:04.000000 playgroundrl-0.0.7/src/playgroundrl/client.py
--rw-r--r--   0 langston   (501) staff       (20)     5104 2023-04-08 21:07:04.000000 playgroundrl-0.0.7/src/playgroundrl/state.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.720115 playgroundrl-0.0.7/src/playgroundrl.egg-info/
--rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      309 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/SOURCES.txt
--rw-r--r--   0 langston   (501) staff       (20)        1 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/dependency_links.txt
--rw-r--r--   0 langston   (501) staff       (20)       52 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/requires.txt
--rw-r--r--   0 langston   (501) staff       (20)       13 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/top_level.txt
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.830499 playgroundrl-0.0.8/
+-rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:54:28.830595 playgroundrl-0.0.8/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      162 2023-04-08 20:30:44.000000 playgroundrl-0.0.8/README.md
+-rw-r--r--   0 langston   (501) staff       (20)       38 2023-04-11 19:54:28.830778 playgroundrl-0.0.8/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)      443 2023-04-11 19:53:51.000000 playgroundrl-0.0.8/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.827894 playgroundrl-0.0.8/src/
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.829229 playgroundrl-0.0.8/src/playgroundrl/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-04-08 20:30:44.000000 playgroundrl-0.0.8/src/playgroundrl/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     8938 2023-04-11 19:53:08.000000 playgroundrl-0.0.8/src/playgroundrl/client.py
+-rw-r--r--   0 langston   (501) staff       (20)     5104 2023-04-08 21:07:04.000000 playgroundrl-0.0.8/src/playgroundrl/state.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.830335 playgroundrl-0.0.8/src/playgroundrl.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      309 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)       52 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)       13 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/top_level.txt
```

### Comparing `playgroundrl-0.0.7/src/playgroundrl/client.py` & `playgroundrl-0.0.8/src/playgroundrl/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import socketio
 from abc import ABC, abstractmethod
 import requests
 import webbrowser
 from urllib.parse import urljoin
 from typing import Dict, Union
 from enum import Enum
-from state import *
+from .state import *
 import cattrs
 import json
 
 class GameType(Enum):
     """Enumeration of different supported games"""
     SNAKE = 'snake'
```

### Comparing `playgroundrl-0.0.7/src/playgroundrl/state.py` & `playgroundrl-0.0.8/src/playgroundrl/state.py`

 * *Files identical despite different names*

