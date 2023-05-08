# Comparing `tmp/graia-ariadne-0.9.8.tar.gz` & `tmp/graia-ariadne-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia-ariadne-0.9.8.tar", last modified: Sun Oct 16 16:07:34 2022, max compression
+gzip compressed data, was "graia-ariadne-0.9.9.tar", last modified: Tue Dec 27 01:42:02 2022, max compression
```

## Comparing `graia-ariadne-0.9.8.tar` & `graia-ariadne-0.9.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-16 16:07:21.880290 graia-ariadne-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-10-16 16:07:21.880290 graia-ariadne-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-10-16 16:07:23.008291 graia-ariadne-0.9.8/src/graia/ariadne/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    72130 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6372 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/connection/_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/connection/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6176 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/connection/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/connection/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     6670 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/connection/ws.py
--rw-r--r--   0 runner    (1001) docker     (121)     9271 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/console/saya.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5548 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     8745 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/entry/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/entry/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/entry/message.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/entry/saya.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/entry/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/event/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     7646 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/event/message.py
--rw-r--r--   0 runner    (1001) docker     (121)    40279 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/event/mirai.py
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17779 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/chain.py
--rw-r--r--   0 runner    (1001) docker     (121)    23381 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/commander/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/commander/creart.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/commander/saya.py
--rw-r--r--   0 runner    (1001) docker     (121)     9657 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/commander/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    22815 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/element.py
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15294 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    29614 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/parser/twilight.py
--rw-r--r--   0 runner    (1001) docker     (121)     9112 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/message/parser/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     7046 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8370 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/model/relationship.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/model/util.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9729 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     5919 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)    11470 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7042 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/util/async_exec.py
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-10-16 16:07:21.884290 graia-ariadne-0.9.8/src/graia/ariadne/util/cooldown.py
--rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-10-16 16:07:21.888290 graia-ariadne-0.9.8/src/graia/ariadne/util/interrupt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4860 2022-10-16 16:07:21.888290 graia-ariadne-0.9.8/src/graia/ariadne/util/saya.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-10-16 16:07:21.888290 graia-ariadne-0.9.8/src/graia/ariadne/util/send.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-10-16 16:07:21.888290 graia-ariadne-0.9.8/src/graia/ariadne/util/validator.py
--rw-------   0 runner    (1001) docker     (121)     5341 2022-10-16 16:07:34.740317 graia-ariadne-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-27 01:41:51.792107 graia-ariadne-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2022-12-27 01:41:51.792107 graia-ariadne-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-27 01:41:52.832126 graia-ariadne-0.9.9/src/graia/ariadne/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73112 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/connection/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/connection/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/connection/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/connection/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/connection/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/console/saya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/entry/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/entry/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/entry/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/entry/saya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/entry/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/event/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/event/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40091 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/event/mirai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/commander/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/commander/creart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/commander/saya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/commander/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29586 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/parser/twilight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/message/parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2022-12-27 01:41:51.796107 graia-ariadne-0.9.9/src/graia/ariadne/model/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/model/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/async_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/cooldown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/saya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2022-12-27 01:41:51.800107 graia-ariadne-0.9.9/src/graia/ariadne/util/validator.py
+-rw-------   0 runner    (1001) docker     (123)     5341 2022-12-27 01:42:02.996296 graia-ariadne-0.9.9/PKG-INFO
```

### Comparing `graia-ariadne-0.9.8/LICENSE` & `graia-ariadne-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/README.md` & `graia-ariadne-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/pyproject.toml` & `graia-ariadne-0.9.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "graia-broadcast~=0.19",
     "aiohttp~=3.8",
     "pydantic~=1.9",
-    "typing-extensions~=4.3",
-    "graia-amnesia~=0.6.0",
+    "typing-extensions>=4.4,<5.0",
+    "graia-amnesia~=0.7.0",
     "creart-graia<1.0.0,>=0.1.5",
     "launart~=0.6",
 ]
 name = "graia-ariadne"
 description = "Another elegant Python QQ Bot framework for mirai and mirai-api-http v2."
 readme = "README.md"
 keywords = [
@@ -36,79 +36,75 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dynamic = []
-version = "0.9.8"
+version = "0.9.9"
 
 [project.urls]
 repository = "https://github.com/GraiaProject/Ariadne"
 documentation = "https://graia.readthedocs.io/projects/ariadne"
 
 [project.entry-points."creart.creators"]
 commander = "graia.ariadne.message.commander.creart:CommanderCreator"
 commander_behaviour = "graia.ariadne.message.commander.creart:CommanderBehaviourCreator"
 
 [project.optional-dependencies]
 standard = [
     "richuru~=0.1",
-    "graia-scheduler~=0.0",
+    "graia-scheduler~=0.1",
     "graia-saya~=0.0",
 ]
 graia = [
-    "graia-scheduler~=0.0",
+    "graia-scheduler~=0.1",
     "graia-saya~=0.0",
 ]
 fastapi = [
     "fastapi<1.0.0,>=0.74.1",
     "uvicorn[standard]<1.0.0,>=0.17.5",
 ]
 full = [
     "richuru~=0.1",
-    "graia-scheduler~=0.0",
+    "graia-scheduler~=0.1",
     "graia-saya~=0.0",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=22.6.0",
-    "isort>=5.10.1",
     "pytest<8.0,>=7.1",
     "coverage<7.0,>=6.4",
-    "flake8>=5.0.4",
     "pytest-asyncio<1.0.0,>=0.19.0",
     "devtools>=0.9",
     "pre-commit<3.0,>=2.20",
     "mkdocstrings[python]<1.0.0,>=0.19.0",
     "mkdocs-material<9.0.0,>=8.4.0",
     "mkdocs-gen-files<1.0.0,>=0.3.5",
     "mkdocs-section-index<1.0.0,>=0.3.4",
     "mkdocs-literate-nav<1.0.0,>=0.4.1",
     "ipykernel<7.0.0,>=6.15.1",
     "richuru<1.0.0,>=0.1.1",
     "graia-scheduler<1.0,>=0.0",
     "fastapi<1.0.0,>=0.79.0",
     "uvicorn[standard]<1.0.0,>=0.18.2",
     "graia-saya>=0.0.16",
+    "ruff>=0.0.132",
 ]
 
 [tool.pdm.build]
 includes = [
     "src/graia",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "src/graia/ariadne/__init__.py"
 
-[tool.isort]
-profile = "black"
-
 [tool.black]
 line-length = 110
 target-version = [
     "py39",
 ]
 
 [tool.coverage.run]
@@ -133,16 +129,66 @@
 ignore = [
     "docs/**",
     "**/site-packages/**/*.py",
     "**/test*/**/*.py",
     "**/adapter/**",
     "**/temp/**/*.py",
 ]
+reportShadowedImports = false
 
-[tool.pydocstyle]
-match-dir = "(?!\\.)(?!test).*"
+[tool.ruff]
+line-length = 110
+select = [
+    "E",
+    "F",
+    "I",
+    "UP",
+    "C",
+    "T",
+    "Q",
+]
+ignore = [
+    "C901",
+]
+extend-exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "src/graia/ariadne/entry/*",
+    "src/test/**",
+    "src/test_old/**",
+    "gen_ref.py",
+    "extract-release-notes.py",
+]
+target-version = "py38"
+
+[tool.ruff.per-file-ignores]
+
+[tool.ruff.isort]
+known-first-party = [
+    "graia",
+]
+extra-standard-library = [
+    "typing_extensions",
+]
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/app.py` & `graia-ariadne-0.9.9/src/graia/ariadne/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import base64
 import io
 import os
 import signal
 import sys
 import traceback
 from contextlib import ExitStack
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import (
+    IO,
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
     ClassVar,
     Dict,
     Iterable,
     List,
@@ -21,20 +22,21 @@
     Optional,
     Type,
     Union,
     cast,
     overload,
 )
 
+from launart import Launart
+from loguru import logger
+
 from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 from graia.amnesia.transport.common.storage import CacheStorage
 from graia.broadcast import Broadcast
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from launart import Launart
-from loguru import logger
 
 from .connection import ConnectionInterface
 from .connection._info import U_Info
 from .connection.util import CallMethod, UploadMethod, build_event
 from .context import enter_context, enter_message_send_context
 from .event import MiraiEvent
 from .event.message import (
@@ -45,16 +47,16 @@
     FriendMessage,
     GroupMessage,
     MessageEvent,
     TempMessage,
 )
 from .event.mirai import FriendEvent, GroupEvent
 from .exception import AriadneConfigurationError, UnknownTarget
+from .message import Source
 from .message.chain import MessageChain, MessageContainer
-from .message.element import Source
 from .model import (
     Announcement,
     FileInfo,
     Friend,
     Group,
     GroupConfig,
     LogConfig,
@@ -68,15 +70,15 @@
 from .service import ElizabethService
 from .typing import (
     SendMessageActionProtocol,
     SendMessageDict,
     SendMessageException,
     Sentinel,
     T,
-    classmethod,
+    class_property,
 )
 from .util import (
     RichLogInstallOptions,
     ariadne_api,
     camel_to_snake,
     loguru_exc_callback,
     loguru_exc_callback_async,
@@ -95,26 +97,24 @@
     instances: ClassVar[Dict[int, "Ariadne"]] = {}
 
     account: int
     connection: ConnectionInterface
     default_send_action: SendMessageActionProtocol
     log_config: LogConfig
 
-    @classmethod
-    @property
+    @class_property
     def broadcast(cls) -> Broadcast:
         """获取 Ariadne 的事件系统.
 
         Returns:
             Broadcast: 事件系统
         """
         return cls.service.broadcast
 
-    @classmethod
-    @property
+    @class_property
     def default_account(cls) -> int:
         """获取默认账号.
 
         Returns:
             int: 默认账号
         """
         if "default_account" in Ariadne.options:
@@ -221,46 +221,51 @@
     async def _event_hook(self, event: MiraiEvent):
         with ExitStack() as stack:
             stack.enter_context(enter_context(self, event))
             sys.audit("AriadnePostRemoteEvent", event)
             cache_set = self.launch_manager.get_interface(Memcache).set
 
             if isinstance(event, (MessageEvent, ActiveMessage)):
-                await cache_set(f"account.{self.account}.message.{int(event)}", event)
-                if event.message_chain.only(Source):
+                await cache_set(f"account.{self.account}.message.{int(event)}", event, timedelta(seconds=120))
+                if not event.message_chain:
                     event.message_chain.append("<! 不支持的消息类型 !>")
 
             if isinstance(event, FriendEvent):
                 stack.enter_context(enter_message_send_context(UploadMethod.Friend))
 
                 friend: Optional[Friend] = getattr(event, "sender", None) or getattr(event, "friend", None)
                 if friend:
-                    await cache_set(f"account.{self.account}.friend.{int(friend)}", friend)
+                    await cache_set(
+                        f"account.{self.account}.friend.{int(friend)}", friend, timedelta(seconds=120)
+                    )
 
             elif isinstance(event, GroupEvent):
                 stack.enter_context(enter_message_send_context(UploadMethod.Group))
-                group: Optional[Group] = None
-
-                member: Optional[Member] = getattr(event, "sender", None) or getattr(event, "member", None)
-                if member:
-                    group = member.group
-                    await asyncio.gather(
-                        cache_set(f"account.{self.account}.group.{int(group)}", group),
-                        cache_set(f"account.{self.account}.group.{int(group)}.member.{int(member)}", member),
-                    )
+                group = cast(Optional[Group], getattr(event, "group", None))
 
-                member: Optional[Member] = getattr(event, "operator", None) or getattr(event, "inviter", None)
+                member = cast(
+                    Optional[Member],
+                    getattr(event, "sender", None)
+                    or getattr(event, "member", None)
+                    or getattr(event, "operator", None)
+                    or getattr(event, "inviter", None),
+                )
                 if member:
                     if not group:
                         group = member.group
-                        await cache_set(f"account.{self.account}.group.{int(group)}", group)
-                    await cache_set(f"account.{self.account}.group.{int(group)}.member.{int(member)}", member)
+                    await cache_set(
+                        f"account.{self.account}.group.{int(group)}.member.{int(member)}",
+                        member,
+                        timedelta(seconds=120),
+                    )
 
-                if not group and (group := getattr(event, "group", None)):
-                    await cache_set(f"account.{self.account}.group.{int(group)}", group)
+                if group:
+                    await cache_set(
+                        f"account.{self.account}.group.{int(group)}", group, timedelta(seconds=120)
+                    )
 
             self.service.broadcast.postEvent(event)
 
     @classmethod
     def _patch_launch_manager(cls) -> None:
         from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
         from graia.amnesia.transport.common.server import AbstractRouter
@@ -287,14 +292,16 @@
     @classmethod
     def launch_blocking(cls, stop_signals: Iterable[signal.Signals] = (signal.SIGINT,)):
         """以阻塞方式启动 Ariadne
 
         Args:
             stop_signals (Iterable[signal.Signals], optional): 要监听的停止信号，默认为 `(signal.SIGINT,)`
         """
+        if not cls.instances:
+            raise ValueError("No account specified.")
         cls._patch_launch_manager()
         try:
             cls.launch_manager.launch_blocking(loop=cls.service.loop, stop_signal=stop_signals)
         except asyncio.CancelledError:
             logger.info("Launch manager exited.", style="red")
 
     @classmethod
@@ -351,15 +358,15 @@
         Returns:
             str: 版本信息.
         """
         interface = self.launch_manager.get_interface(Memcache)
         if cache and (version := await interface.get(f"account.{self.account}.version")):
             return version
         version = (await self.connection.call("about", CallMethod.GET, {}, in_session=False))["version"]
-        await interface.set(f"account.{self.account}.version", version)
+        await interface.set(f"account.{self.account}.version", version, timedelta(seconds=120))
         return version
 
     @ariadne_api
     async def get_bot_list(self) -> List[int]:
         """获取所有当前登录账号. 需要 Mirai API HTTP 2.6.0+.
 
         Returns:
@@ -501,15 +508,15 @@
         target = target.id if isinstance(target, Group) else target
 
         result = await self.connection.call(
             "file_mkdir",
             CallMethod.POST,
             {
                 "id": id,
-                "name": name,
+                "directoryName": name,
                 "target": target,
             },
         )
 
         return FileInfo.parse_obj(result)
 
     @ariadne_api
@@ -613,26 +620,26 @@
                 "renameTo": dest_name,
             },
         )
 
     @ariadne_api
     async def upload_file(
         self,
-        data: Union[bytes, io.IOBase, os.PathLike],
+        data: Union[bytes, IO[bytes], os.PathLike],
         method: Union[str, UploadMethod, None] = None,
         target: Union[Friend, Group, int] = -1,
         path: str = "",
         name: str = "",
     ) -> "FileInfo":
         """
         上传文件到指定目标, 需要提供: 文件的原始数据(bytes), 文件的上传类型, \
         上传目标, (可选)上传目录ID.
 
         Args:
-            data (Union[bytes, io.IOBase, os.PathLike]): 文件的原始数据
+            data (Union[bytes, IO[bytes], os.PathLike]): 文件的原始数据
             method (str | UploadMethod, optional): 文件的上传类型
             target (Union[Friend, Group, int]): 文件上传目标, 即群组
             path (str): 目标路径, 默认为根路径.
             name (str): 文件名, 可选, 若 path 存在斜杠可从 path 推断.
 
         Returns:
             FileInfo: 文件信息
@@ -661,20 +668,20 @@
             },
         )
 
         return FileInfo.parse_obj(result)
 
     @ariadne_api
     async def upload_image(
-        self, data: Union[bytes, io.IOBase, os.PathLike], method: Union[None, str, UploadMethod] = None
+        self, data: Union[bytes, IO[bytes], os.PathLike], method: Union[None, str, UploadMethod] = None
     ) -> "Image":
         """上传一张图片到远端服务器, 需要提供: 图片的原始数据(bytes), 图片的上传类型.
 
         Args:
-            data (Union[bytes, io.IOBase, os.PathLike]): 图片的原始数据
+            data (Union[bytes, IO[bytes], os.PathLike]): 图片的原始数据
             method (str | UploadMethod, optional): 图片的上传类型, 可从上下文推断
         Returns:
             Image: 生成的图片消息元素
         """
         from .context import upload_method_ctx
         from .message.element import Image
 
@@ -692,20 +699,20 @@
             },
         )
 
         return Image.parse_obj(result)
 
     @ariadne_api
     async def upload_voice(
-        self, data: Union[bytes, io.IOBase, os.PathLike], method: Union[None, str, UploadMethod] = None
+        self, data: Union[bytes, IO[bytes], os.PathLike], method: Union[None, str, UploadMethod] = None
     ) -> "Voice":
         """上传语音到远端服务器, 需要提供: 语音的原始数据(bytes), 语音的上传类型.
 
         Args:
-            data (Union[bytes, io.IOBase, os.PathLike]): 语音的原始数据
+            data (Union[bytes, IO[bytes], os.PathLike]): 语音的原始数据
             method (str | UploadMethod, optional): 语音的上传类型, 可从上下文推断
         Returns:
             Voice: 生成的语音消息元素
         """
         from .context import upload_method_ctx
         from .message.element import Voice
 
@@ -1041,25 +1048,14 @@
         Returns:
             None: 没有返回.
         """
         if isinstance(message, GroupMessage):
             target = message.sender.group
         elif isinstance(message, ActiveGroupMessage):
             target = message.subject
-        elif target is None:
-            from warnings import warn
-
-            warning = DeprecationWarning(  # FIXME: deprecated
-                "Passing Source or int as message without passing target to Ariadne.set_essence() "
-                "is deprecated in Ariadne 0.9, and scheduled for removal in Ariadne 0.10."
-            )
-            warn(warning, stacklevel=2)
-            logger.opt(depth=1).warning(
-                "".join(traceback.format_exception_only(type(warning), warning)).strip()
-            )
 
         if tuple(map(int, (await self.get_version(cache=True)).split("."))) >= (2, 6, 0):
             if target is not None:
                 pass
             elif (
                 event := await self.launch_manager.get_interface(Memcache).get(
                     f"account.{self.account}.message.{int(message)}"
@@ -1255,15 +1251,17 @@
                 "friendList",
                 CallMethod.GET,
                 {},
             )
         ]
 
         cache_set = self.launch_manager.get_interface(Memcache).set
-        await asyncio.gather(*(cache_set(f"account.{self.account}.friend.{int(i)}", i) for i in result))
+        await asyncio.gather(
+            *(cache_set(f"account.{self.account}.friend.{int(i)}", i, timedelta(seconds=120)) for i in result)
+        )
         return result
 
     @overload
     async def get_friend(
         self, friend_id: int, *, assertion: Literal[False] = False, cache: bool = False
     ) -> Optional[Friend]:
         """从已知的可能的好友 ID, 获取 Friend 实例.
@@ -1336,15 +1334,17 @@
                 "groupList",
                 CallMethod.GET,
                 {},
             )
         ]
 
         cache_set = self.launch_manager.get_interface(Memcache).set
-        await asyncio.gather(*(cache_set(f"account.{self.account}.group.{int(i)}", i) for i in result))
+        await asyncio.gather(
+            *(cache_set(f"account.{self.account}.group.{int(i)}", i, timedelta(120)) for i in result)
+        )
         return result
 
     @overload
     async def get_group(
         self, group_id: int, *, assertion: Literal[False] = False, cache: bool = False
     ) -> Optional[Group]:
         """尝试从已知的群组唯一ID, 获取对应群组的信息; 可能返回 None.
@@ -1426,16 +1426,21 @@
                 },
             )
         ]
 
         cache_set = self.launch_manager.get_interface(Memcache).set
 
         await asyncio.gather(
-            cache_set(f"account.{self.account}.group.{group_id}", result[0].group),
-            *(cache_set(f"account.{self.account}.group.{group_id}.member.{int(i)}", i) for i in result),
+            cache_set(f"account.{self.account}.group.{group_id}", result[0].group, timedelta(seconds=120)),
+            *(
+                cache_set(
+                    f"account.{self.account}.group.{group_id}.member.{int(i)}", i, timedelta(seconds=120)
+                )
+                for i in result
+            ),
         )
 
         return result
 
     @ariadne_api
     async def get_member(self, group: Union[Group, int], member_id: int, *, cache: bool = False) -> Member:
         """尝试从已知的群组唯一 ID 和已知的群组成员的 ID, 获取对应成员的信息.
@@ -1463,15 +1468,16 @@
                     "target": group_id,
                     "memberId": member_id,
                 },
             )
         )
 
         await asyncio.gather(
-            interface.set(f"account.{self.account}.group.{group_id}", result), interface.set(key, result)
+            interface.set(f"account.{self.account}.group.{group_id}", result, timedelta(seconds=120)),
+            interface.set(key, result, timedelta(seconds=120)),
         )
 
         return result
 
     @ariadne_api
     async def get_bot_profile(self) -> Profile:
         """获取本实例绑定账号的 Profile.
@@ -1570,25 +1576,14 @@
             message (Union[Source, int]): 指定的消息.
             target (Union[Friend, Group, Member, Stranger, Client, int], optional): 指定的好友或群组. \
                 message 类型为 Source 或 int 时必需.
 
         Returns:
             MessageEvent: 提取的事件.
         """
-        if target is None:
-            from warnings import warn
-
-            warning = DeprecationWarning(  # FIXME: deprecated
-                "Not passing target to Ariadne.get_message_from_id() is deprecated in Ariadne 0.9, "
-                "and scheduled for removal in Ariadne 0.10."
-            )
-            warn(warning, stacklevel=2)
-            logger.opt(depth=1).warning(
-                "".join(traceback.format_exception_only(type(warning), warning)).strip()
-            )
 
         if tuple(map(int, (await self.get_version(cache=True)).split("."))) >= (2, 6, 0):
             if target is not None:
                 pass
             elif event := await self.launch_manager.get_interface(Memcache).get(
                 f"account.{self.account}.message.{message}"
             ):
@@ -1616,31 +1611,46 @@
 
     @ariadne_api
     async def send_friend_message(
         self,
         target: Union[Friend, int],
         message: MessageContainer,
         *,
-        quote: Optional[Union[Source, int, MessageChain]] = None,
+        quote: Optional[Union[Source, int]] = None,
+        action: Union[SendMessageActionProtocol, Literal[Sentinel], None] = Sentinel,
     ) -> ActiveFriendMessage:
         """发送消息给好友, 可以指定回复的消息.
 
         Args:
             target (Union[Friend, int]): 指定的好友
             message (MessageContainer): 有效的消息容器.
-            quote (Optional[Union[Source, int, MessageChain]], optional): 需要回复的消息, 不要忽视我啊喂?!!, 默认为 None.
+            quote (Optional[Union[Source, int]], optional): 需要回复的消息, 不要忽视我啊喂?!!, 默认为 None.
 
         Returns:
             ActiveFriendMessage: 即当前会话账号所发出消息的事件, 可用于回复.
         """
         from .event.message import ActiveFriendMessage
 
         message = MessageChain(message)
         if isinstance(quote, MessageChain):
-            quote = quote.get_first(Source)
+            raise TypeError(
+                "Using MessageChain as quote target is removed! Get a `Source` from event instead!"
+            )
+
+        if action is not None:  # TODO: REFACTOR
+            return cast(
+                ActiveFriendMessage,
+                await self.send_message(
+                    await self.get_friend(target, assertion=True) if isinstance(target, int) else target,
+                    message,
+                    quote=quote or False,
+                    action=action,
+                ),
+            )
+
         if isinstance(quote, Source):
             quote = quote.id
 
         with enter_message_send_context(UploadMethod.Friend):
             message = message.as_sendable()
             try:
                 result = await self.connection.call(
@@ -1649,15 +1659,16 @@
                     {
                         "target": int(target),
                         "messageChain": message.dict()["__root__"],
                         **({"quote": quote} if quote else {}),
                     },
                 )
                 event = ActiveFriendMessage(
-                    messageChain=MessageChain(Source(id=result["messageId"], time=datetime.now()), message),
+                    messageChain=MessageChain(message),
+                    source=Source(id=result["messageId"], time=datetime.now()),
                     subject=(await self.get_friend(int(target), assertion=True, cache=True)),
                 )
                 with enter_context(self, event):
                     await self.log_config.log(self, event)
                     self.service.broadcast.postEvent(event)
                 if result["messageId"] < 0:
                     logger.warning("Failed to send message, your account may be blocked.")
@@ -1670,34 +1681,50 @@
 
     @ariadne_api
     async def send_group_message(
         self,
         target: Union[Group, Member, int],
         message: MessageContainer,
         *,
-        quote: Optional[Union[Source, int, MessageChain]] = None,
+        quote: Optional[Union[Source, int]] = None,
+        action: Union[SendMessageActionProtocol, Literal[Sentinel], None] = Sentinel,
     ) -> ActiveGroupMessage:
         """发送消息到群组内, 可以指定回复的消息.
 
         Args:
             target (Union[Group, Member, int]): 指定的群组, 可以是群组的 ID 也可以是 Group 或 Member 实例.
             message (MessageContainer): 有效的消息容器.
-            quote (Optional[Union[Source, int, MessageChain]], optional): 需要回复的消息, 不要忽视我啊喂?!!, 默认为 None.
+            quote (Optional[Union[Source, int]], optional): 需要回复的消息, 不要忽视我啊喂?!!, 默认为 None.
+            action (SendMessageActionProtocol, optional): 消息发送的处理 action
 
         Returns:
             ActiveGroupMessage: 即当前会话账号所发出消息的事件, 可用于回复.
         """
         from .event.message import ActiveGroupMessage
 
         message = MessageChain(message)
         if isinstance(target, Member):
             target = target.group
 
+        if action is not None:  # TODO: REFACTOR
+            return cast(
+                ActiveGroupMessage,
+                await self.send_message(
+                    await self.get_group(target, assertion=True) if isinstance(target, int) else target,
+                    message,
+                    quote=quote or False,
+                    action=action,
+                ),
+            )
+
         if isinstance(quote, MessageChain):
-            quote = quote.get_first(Source)
+            raise TypeError(
+                "Using MessageChain as quote target is removed! Get a `Source` from event instead!"
+            )
+
         if isinstance(quote, Source):
             quote = quote.id
 
         with enter_message_send_context(UploadMethod.Group):
             message = message.as_sendable().copy()
             try:
                 result = await self.connection.call(
@@ -1706,15 +1733,16 @@
                     {
                         "target": int(target),
                         "messageChain": message.dict()["__root__"],
                         **({"quote": quote} if quote else {}),
                     },
                 )
                 event = ActiveGroupMessage(
-                    messageChain=MessageChain(Source(id=result["messageId"], time=datetime.now()), message),
+                    messageChain=MessageChain(message),
+                    source=Source(id=result["messageId"], time=datetime.now()),
                     subject=(await self.get_group(int(target), assertion=True, cache=True)),
                 )
                 with enter_context(self, event):
                     await self.log_config.log(self, event)
                     self.service.broadcast.postEvent(event)
                 if result["messageId"] < 0:
                     logger.warning("Failed to send message, your account may be blocked.")
@@ -1728,56 +1756,75 @@
     @ariadne_api
     async def send_temp_message(
         self,
         target: Union[Member, int],
         message: MessageContainer,
         group: Optional[Union[Group, int]] = None,
         *,
-        quote: Optional[Union[Source, int, MessageChain]] = None,
+        quote: Optional[Union[Source, int]] = None,
+        action: Union[SendMessageActionProtocol, Literal[Sentinel], None] = Sentinel,
     ) -> ActiveTempMessage:
         """发送临时会话给群组中的特定成员, 可指定回复的消息.
 
         Warning:
             本 API 大概率会导致账号风控/冻结. 请谨慎使用.
 
         Args:
             group (Union[Group, int]): 指定的群组, 可以是群组的 ID 也可以是 Group 实例.
             target (Union[Member, int]): 指定的群组成员, 可以是成员的 ID 也可以是 Member 实例.
             message (MessageContainer): 有效的消息容器.
             quote (Optional[Union[Source, int]], optional): 需要回复的消息, 不要忽视我啊喂?!!, 默认为 None.
+            action (SendMessageActionProtocol, optional): 消息发送的处理 action
 
         Returns:
             ActiveTempMessage: 即当前会话账号所发出消息的事件, 可用于回复.
         """
         from .event.message import ActiveTempMessage
 
         message = MessageChain(message)
+
         if isinstance(quote, MessageChain):
-            quote = quote.get_first(Source)
-        if isinstance(quote, Source):
-            quote = quote.id
+            raise TypeError(
+                "Using MessageChain as quote target is removed! Get a `Source` from event instead!"
+            )
 
         new_msg = message.copy().as_sendable()
         group = target.group if (isinstance(target, Member) and not group) else group
         if not group:
             raise ValueError("Missing necessary argument: group")
+
+        if action is not None:  # TODO: REFACTOR
+            return cast(
+                ActiveTempMessage,
+                await self.send_message(
+                    await self.get_member(group, target, cache=True) if isinstance(target, int) else target,
+                    message,
+                    quote=quote or False,
+                    action=action,
+                ),
+            )
+
+        if isinstance(quote, Source):
+            quote = quote.id
+
         with enter_message_send_context(UploadMethod.Temp):
             try:
                 result = await self.connection.call(
                     "sendTempMessage",
                     CallMethod.POST,
                     {
                         "group": int(group),
                         "qq": int(target),
                         "messageChain": new_msg.dict()["__root__"],
                         **({"quote": quote} if quote else {}),
                     },
                 )
                 event: ActiveTempMessage = ActiveTempMessage(
-                    messageChain=MessageChain(Source(id=result["messageId"], time=datetime.now()), message),
+                    messageChain=MessageChain(message),
+                    source=Source(id=result["messageId"], time=datetime.now()),
                     subject=(await self.get_member(int(group), int(target), cache=True)),
                 )
                 with enter_context(self, event):
                     await self.log_config.log(self, event)
                     self.service.broadcast.postEvent(event)
                 if result["messageId"] < 0:
                     logger.warning("Failed to send message, your account may be limited.")
@@ -1846,15 +1893,15 @@
 
     @ariadne_api
     async def send_message(
         self,
         target: Union[MessageEvent, Group, Friend, Member],
         message: MessageContainer,
         *,
-        quote: Union[bool, int, Source, MessageChain] = False,
+        quote: Union[bool, int, Source] = False,
         action: Union[SendMessageActionProtocol["T"], Literal[Sentinel]] = Sentinel,
     ) -> "T":
         """
         依据传入的 `target` 自动发送消息.
 
         请注意发送给群成员时会自动作为临时消息发送.
 
@@ -1869,46 +1916,52 @@
 
         Returns:
             Union[T, R]: 默认实现为 ActiveMessage
         """
         action = action if action is not Sentinel else self.default_send_action
         data: Dict[Any, Any] = {"message": MessageChain(message)}
         # quote
-        if isinstance(quote, bool) and quote and isinstance(target, MessageEvent):
-            data["quote"] = target.message_chain.get_first(Source)
+        if isinstance(quote, bool):
+            if quote:
+                if isinstance(target, MessageEvent):
+                    data["quote"] = target.source
+                raise TypeError("Passing `quote=True` is only valid when passing a MessageEvent.")
         elif isinstance(quote, (int, Source)):
             data["quote"] = quote
         elif isinstance(quote, MessageChain):
-            data["quote"] = quote.get_first(Source)
+            raise TypeError(
+                "Using MessageChain as quote target is removed! Get a `Source` from event instead!"
+            )
         # target: MessageEvent
         if isinstance(target, GroupMessage):
             data["target"] = target.sender.group
         elif isinstance(target, (FriendMessage, TempMessage)):
             data["target"] = target.sender
         else:  # target: sender
             data["target"] = target
         send_data: SendMessageDict = SendMessageDict(**data)
         # send message
         data = await action.param(send_data)  # type: ignore
 
         try:
             if isinstance(data["target"], Friend):
-                val = await self.send_friend_message(**data)
+                val = await self.send_friend_message(**data, action=None)
             elif isinstance(data["target"], Group):
-                val = await self.send_group_message(**data)
+                val = await self.send_group_message(**data, action=None)
             elif isinstance(data["target"], Member):
-                val = await self.send_temp_message(**data)
+                val = await self.send_temp_message(**data, action=None)
             else:
                 logger.warning(
                     f"Unable to send {data['message']} to {data['target']} of type {type(data['target'])}"
                 )
                 return await action.result(
                     ActiveMessage(
                         type="Unknown",
-                        messageChain=MessageChain(Source(id=-1, time=datetime.now()), data["message"]),
+                        messageChain=MessageChain(data["message"]),
+                        source=Source(id=-1, time=datetime.now()),
                         subject=data["target"],
                     )
                 )
         except SendMessageException as e:
             e.send_data = send_data  # type: ignore
             return await action.exception(e)
         else:
@@ -1968,25 +2021,14 @@
             pass
         elif isinstance(message, GroupMessage):
             target = message.sender.group
         elif isinstance(message, MessageEvent):
             target = message.sender
         elif isinstance(message, ActiveMessage):
             target = message.subject
-        else:
-            from warnings import warn
-
-            warning = DeprecationWarning(  # FIXME: deprecated
-                "Passing Source or int as message without passing target to Ariadne.recall_message() "
-                "is deprecated in Ariadne 0.9, and scheduled for removal in Ariadne 0.10."
-            )
-            warn(warning, stacklevel=2)
-            logger.opt(depth=1).warning(
-                "".join(traceback.format_exception_only(type(warning), warning)).strip()
-            )
 
         if tuple(map(int, (await self.get_version(cache=True)).split("."))) >= (2, 6, 0):
             if target is not None:
                 pass
             elif event := await self.launch_manager.get_interface(Memcache).get(
                 f"account.{self.account}.message.{int(message)}"
             ):
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/connection/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/connection/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,41 @@
 from __future__ import annotations
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Awaitable,
-    Callable,
-    ClassVar,
-    Dict,
-    Generic,
-    List,
-    Optional,
-    Set,
-    Type,
-)
-
-from graia.amnesia.transport.common.status import (
-    ConnectionStatus as BaseConnectionStatus,
-)
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, ClassVar, Generic, Optional
+from typing_extensions import Self
+
 from launart import ExportInterface, Launchable, LaunchableStatus
 from statv import Stats
-from typing_extensions import Self
+
+from graia.amnesia.transport.common.status import ConnectionStatus as BaseConnectionStatus
 
 from ..event import MiraiEvent
 from ..util import camel_to_snake
-from ._info import (
-    HttpClientInfo,
-    HttpServerInfo,
-    T_Info,
-    U_Info,
-    WebsocketClientInfo,
-    WebsocketServerInfo,
-)
+from ._info import HttpClientInfo, HttpServerInfo, T_Info, U_Info, WebsocketClientInfo, WebsocketServerInfo
 from .util import CallMethod
 
 if TYPE_CHECKING:
     from ..service import ElizabethService
 
 
 class ConnectionStatus(BaseConnectionStatus, LaunchableStatus):
     """连接状态"""
 
     alive = Stats[bool]("alive", default=False)
 
     def __init__(self) -> None:
-        self._session_key: Optional[str] = None
+        self._session_key: str | None = None
         super().__init__()
 
     @property
-    def session_key(self) -> Optional[str]:
+    def session_key(self) -> str | None:
         return self._session_key
 
     @session_key.setter
-    def session_key(self, value: Optional[str]) -> None:
+    def session_key(self, value: str | None) -> None:
         self._session_key = value
         self.connected = value is not None
 
     @property
     def available(self) -> bool:
         return bool(self.connected and self.session_key and self.alive)
 
@@ -71,21 +51,21 @@
             )
         )
 
 
 class ConnectionMixin(Launchable, Generic[T_Info]):
     status: ConnectionStatus
     info: T_Info
-    dependencies: ClassVar[Set[str | type[ExportInterface]]]
+    dependencies: ClassVar[set[str | type[ExportInterface]]]
 
     fallback: Optional["HttpClientConnection"]
-    event_callbacks: List[Callable[[MiraiEvent], Awaitable[Any]]]
+    event_callbacks: list[Callable[[MiraiEvent], Awaitable[Any]]]
 
     @property
-    def required(self) -> Set[str | type[ExportInterface]]:
+    def required(self) -> set[str | type[ExportInterface]]:
         return self.dependencies
 
     @property
     def stages(self):
         return {}
 
     def __init__(self, info: T_Info) -> None:
@@ -102,15 +82,15 @@
         self.event_callbacks = []
         self.status = ConnectionStatus()
 
     async def call(
         self,
         command: str,
         method: CallMethod,
-        params: Optional[dict] = None,
+        params: dict | None = None,
         *,
         in_session: bool = True,
     ) -> Any:
         """调用下层 API
 
         Args:
             command (str): 命令
@@ -128,29 +108,29 @@
 
 
 from .http import HttpClientConnection as HttpClientConnection  # noqa: E402
 from .http import HttpServerConnection as HttpServerConnection  # noqa: E402
 from .ws import WebsocketClientConnection as WebsocketClientConnection  # noqa: E402
 from .ws import WebsocketServerConnection as WebsocketServerConnection  # noqa: E402
 
-CONFIG_MAP: Dict[Type[U_Info], Type[ConnectionMixin]] = {
+CONFIG_MAP: dict[type[U_Info], type[ConnectionMixin]] = {
     HttpClientInfo: HttpClientConnection,
     HttpServerInfo: HttpServerConnection,
     WebsocketClientInfo: WebsocketClientConnection,
     WebsocketServerInfo: WebsocketServerConnection,
 }
 
 
 class ConnectionInterface(ExportInterface["ElizabethService"]):
     """Elizabeth 连接接口"""
 
     service: "ElizabethService"
-    connection: Optional[ConnectionMixin]
+    connection: ConnectionMixin | None
 
-    def __init__(self, service: "ElizabethService", account: Optional[int] = None) -> None:
+    def __init__(self, service: "ElizabethService", account: int | None = None) -> None:
         """初始化连接接口
 
         Args:
             service (ElizabethService): 连接服务
             account (int, optional): 对应账号
         """
         self.service = service
@@ -173,15 +153,15 @@
 
     async def call(
         self,
         command: str,
         method: CallMethod,
         params: dict,
         *,
-        account: Optional[int] = None,
+        account: int | None = None,
         in_session: bool = True,
     ) -> Any:
         """发起一个调用
 
         Args:
             command (str): 调用命令
             method (CallMethod): 调用方法
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/connection/_info.py` & `graia-ariadne-0.9.9/src/graia/ariadne/connection/_info.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/connection/config.py` & `graia-ariadne-0.9.9/src/graia/ariadne/connection/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-from typing import (
-    TYPE_CHECKING,
-    Dict,
-    List,
-    NamedTuple,
-    Sequence,
-    Type,
-    Union,
-    overload,
-)
-
+from typing import TYPE_CHECKING, Dict, List, NamedTuple, Sequence, Type, Union, overload
 from typing_extensions import NotRequired, Required, TypedDict
 
 from ..typing import DictStrAny
-from ._info import (
-    HttpClientInfo,
-    HttpServerInfo,
-    U_Info,
-    WebsocketClientInfo,
-    WebsocketServerInfo,
-)
+from ._info import HttpClientInfo, HttpServerInfo, U_Info, WebsocketClientInfo, WebsocketServerInfo
 
 if TYPE_CHECKING:
     from ..app import Ariadne
 
 
 class WebsocketClientConfig(NamedTuple):
     """Websocket 客户端配置"""
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/connection/http.py` & `graia-ariadne-0.9.9/src/graia/ariadne/connection/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
 import json as json_mod
 from typing import Any, Optional
 
 from aiohttp import FormData
+from launart import Launart
+from launart.utilles import wait_fut
+from loguru import logger
+
 from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
 from graia.amnesia.builtins.memcache import Memcache
 from graia.amnesia.json import Json
 from graia.amnesia.transport import Transport
 from graia.amnesia.transport.common.http import AbstractServerRequestIO, HttpEndpoint
 from graia.amnesia.transport.common.http.extra import HttpRequest
 from graia.amnesia.transport.common.server import AbstractRouter
-from launart import Launart
-from launart.utilles import wait_fut
-from loguru import logger
 
 from ..exception import InvalidSession
 from . import ConnectionMixin
 from ._info import HttpClientInfo, HttpServerInfo
 from .util import CallMethod, DatetimeJsonEncoder, build_event, validate_response
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/connection/util.py` & `graia-ariadne-0.9.9/src/graia/ariadne/connection/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
 from datetime import datetime
 from enum import Enum
 from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Dict, Literal, Optional, Type, Union, overload
+from typing import TYPE_CHECKING, Any, Literal, overload
 
 from loguru import logger
 
 from ..exception import (
     AccountMuted,
     AccountNotFound,
     InvalidArgument,
@@ -22,15 +22,15 @@
 )
 from ..util import gen_subclass
 
 if TYPE_CHECKING:
     from ..event import MiraiEvent
 
 
-code_exceptions_mapping: Dict[int, Type[Exception]] = {
+code_exceptions_mapping: dict[int, type[Exception]] = {
     1: InvalidVerifyKey,
     2: AccountNotFound,
     3: InvalidSession,
     4: UnVerifiedSession,
     5: UnknownTarget,
     6: FileNotFoundError,
     10: PermissionError,
@@ -38,15 +38,15 @@
     30: MessageTooLong,
     400: InvalidArgument,
     500: RemoteException,
 }
 
 
 @overload
-def validate_response(data: Any, raising: Literal[False]) -> Union[Any, Exception]:
+def validate_response(data: Any, raising: Literal[False]) -> Any | Exception:
     ...
 
 
 @overload
 def validate_response(data: Any, raising: Literal[True] = True) -> Any:
     ...
 
@@ -59,15 +59,15 @@
     exc = exc_cls(exc_cls.__doc__, data) if exc_cls else UnknownError(data)
     if raising:
         raise exc
     return exc
 
 
 @lru_cache(maxsize=1024)
-def extract_event_type(event_type: str) -> Optional[Type[MiraiEvent]]:
+def extract_event_type(event_type: str) -> type[MiraiEvent] | None:
     from ..event import MiraiEvent
 
     return next((cls for cls in gen_subclass(MiraiEvent) if cls.__name__ == event_type), None)
 
 
 def build_event(data: dict) -> MiraiEvent:
     """
@@ -79,18 +79,18 @@
     Raises:
         InvalidArgument: 目标对象中不包含字段 `type`
         ValueError: 没有找到对应的字段, 通常的, 这意味着应用获取到了一个尚未被定义的事件, 请报告问题.
 
     Returns:
         MiraiEvent: 已经被序列化的事件
     """
-    event_type: Optional[str] = data.get("type")
+    event_type: str | None = data.get("type")
     if not event_type or not isinstance(event_type, str):
         raise InvalidArgument("Unable to find 'type' field for automatic parsing", data)
-    event_class: Optional[Type[MiraiEvent]] = extract_event_type(event_type)
+    event_class: type[MiraiEvent] | None = extract_event_type(event_type)
     if not event_class:
         logger.error("An event is not recognized! Please report with your log to help us diagnose.")
         raise ValueError(f"Unable to find event: {event_type}", data)
     data = {k: v for k, v in data.items() if k != "type"}
     return event_class.parse_obj(data)
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/connection/ws.py` & `graia-ariadne-0.9.9/src/graia/ariadne/connection/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import asyncio
 import json as json_mod
 import secrets
 from typing import Any, Dict, MutableMapping, Optional
 from weakref import WeakValueDictionary
 
+from launart import Launart
+from launart.utilles import wait_fut
+from loguru import logger
+from yarl import URL
+
 from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
 from graia.amnesia.builtins.memcache import Memcache
 from graia.amnesia.transport import Transport
 from graia.amnesia.transport.common.http.extra import HttpRequest
 from graia.amnesia.transport.common.server import AbstractRouter
 from graia.amnesia.transport.common.websocket import (
     AbstractWebsocketIO,
@@ -17,18 +22,14 @@
     WebsocketReceivedEvent,
     WebsocketReconnect,
     WSConnectionAccept,
     WSConnectionClose,
 )
 from graia.amnesia.transport.common.websocket.shortcut import data_type, json_require
 from graia.amnesia.transport.utilles import TransportRegistrar
-from launart import Launart
-from launart.utilles import wait_fut
-from loguru import logger
-from yarl import URL
 
 from . import ConnectionMixin
 from ._info import T_Info, WebsocketClientInfo, WebsocketServerInfo
 from .util import CallMethod, DatetimeJsonEncoder, build_event, validate_response
 
 t = TransportRegistrar()
 
@@ -139,15 +140,14 @@
         for k, v in self.info.headers.items():
             if req.headers.get(k) != v:
                 return await io.extra(WSConnectionClose)
         for k, v in self.info.params.items():
             if req.query_params.get(k) != v:
                 return await io.extra(WSConnectionClose)
         await io.extra(WSConnectionAccept)
-        logger.info("WebsocketServer")
         await io.send(
             {
                 "syncId": "#",
                 "command": "verify",
                 "content": {
                     "verifyKey": self.info.verify_key,
                     "sessionKey": None,
@@ -177,15 +177,16 @@
         config = self.info
         async with self.stage("blocking"):
             rider = self.http_interface.websocket(
                 str(
                     (URL(config.host) / "all").with_query(
                         {"qq": config.account, "verifyKey": config.verify_key}
                     )
-                )
+                ),
+                heartbeat=30.0,
             )
             await wait_fut(
                 [rider.use(self), mgr.status.wait_for_sigexit()],
                 return_when=asyncio.FIRST_COMPLETED,
             )
 
     @t.on(WebsocketConnectEvent)
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/console/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/console/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import contextlib
 import importlib.metadata
 import sys
 from asyncio.events import AbstractEventLoop
 from asyncio.tasks import Task
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
+from loguru import logger
+from prompt_toolkit.formatted_text import AnyFormattedText
+from prompt_toolkit.patch_stdout import StdoutProxy
+from prompt_toolkit.shortcuts.prompt import PromptSession
+from prompt_toolkit.styles import Style
+
 from graia.broadcast import Broadcast
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.dispatcher import BaseDispatcher
 from graia.broadcast.entities.exectarget import ExecTarget
 from graia.broadcast.exceptions import DisabledNamespace, PropagationCancelled
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from loguru import logger
-from prompt_toolkit.formatted_text import AnyFormattedText
-from prompt_toolkit.patch_stdout import StdoutProxy
-from prompt_toolkit.shortcuts.prompt import PromptSession
-from prompt_toolkit.styles import Style
 
 from ..dispatcher import ContextDispatcher
 from ..event.lifecycle import ApplicationLaunch, ApplicationShutdown
 from ..util import resolve_dispatchers_mixin
 
 
 class Console:
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/console/saya.py` & `graia-ariadne-0.9.9/src/graia/ariadne/console/saya.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/context.py` & `graia-ariadne-0.9.9/src/graia/ariadne/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 """本模块创建了 Ariadne 中的上下文变量"""
+from __future__ import annotations
 
 from contextlib import contextmanager, suppress
 from contextvars import ContextVar
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from asyncio.events import AbstractEventLoop
 
     from graia.broadcast import Broadcast
     from graia.broadcast.entities.event import Dispatchable
 
     from .app import Ariadne
     from .connection.util import UploadMethod
 
-    ariadne_ctx: ContextVar[Ariadne] = ContextVar("ariadne")
-    event_ctx: ContextVar[Dispatchable] = ContextVar("event")
-    event_loop_ctx: ContextVar[AbstractEventLoop] = ContextVar("event_loop")
-    broadcast_ctx: ContextVar[Broadcast] = ContextVar("broadcast")
-    upload_method_ctx: ContextVar[UploadMethod] = ContextVar("upload_method")
-else:  # for not crashing pdoc
-    ariadne_ctx = ContextVar("ariadne")
-    event_ctx = ContextVar("event")
-    event_loop_ctx = ContextVar("event_loop")
-    broadcast_ctx = ContextVar("broadcast")
-    upload_method_ctx = ContextVar("upload_method")
+ariadne_ctx: ContextVar[Ariadne] = ContextVar("ariadne")
+event_ctx: ContextVar[Dispatchable] = ContextVar("event")
+event_loop_ctx: ContextVar[AbstractEventLoop] = ContextVar("event_loop")
+broadcast_ctx: ContextVar[Broadcast] = ContextVar("broadcast")
+upload_method_ctx: ContextVar[UploadMethod] = ContextVar("upload_method")
 
-context_map: Dict[str, ContextVar] = {
+
+context_map: dict[str, ContextVar] = {
     "Ariadne": ariadne_ctx,
     "Dispatchable": event_ctx,
     "AbstractEventLoop": event_loop_ctx,
     "Broadcast": broadcast_ctx,
     "UploadMethod": upload_method_ctx,
 }
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/dispatcher.py` & `graia-ariadne-0.9.9/src/graia/ariadne/dispatcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 """Ariadne 内置的 Dispatcher"""
 
-import asyncio
-import contextlib
-
-from graia.broadcast import Broadcast
-from graia.broadcast.entities.dispatcher import BaseDispatcher as AbstractDispatcher
-from graia.broadcast.entities.signatures import Force
-from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-
-from .message.chain import MessageChain
-from .message.element import Quote, Source
-from .model.relationship import Friend, Group, Member
-from .typing import generic_isinstance, generic_issubclass
+import asyncio
+import contextlib
+
+from launart import ExportInterface, Launart
+
+from graia.broadcast import Broadcast
+from graia.broadcast.entities.dispatcher import BaseDispatcher as AbstractDispatcher
+from graia.broadcast.entities.signatures import Force
+from graia.broadcast.interfaces.dispatcher import DispatcherInterface
+
+from .message.chain import MessageChain
+from .message.element import Quote, Source
+from .model.relationship import Friend, Group, Member
+from .typing import generic_isinstance, generic_issubclass
 
 
 class MessageChainDispatcher(AbstractDispatcher):
     """从 MessageEvent 提取 MessageChain 的 Dispatcher"""
 
     @staticmethod
     async def catch(interface: DispatcherInterface):
         from .event.message import ActiveMessage, MessageEvent
-        from .message.exp import MessageChain as ExpMessageChain
 
-        if isinstance(interface.event, (MessageEvent, ActiveMessage)):
-            # FIXME: ExpMessageChain as native.
-            if generic_issubclass(MessageChain, interface.annotation):
-                return interface.event.message_chain
-            elif generic_issubclass(ExpMessageChain, interface.annotation):
-                return ExpMessageChain(
-                    interface.event.message_chain.exclude(Source, Quote).content, inline=True
-                )
+        if isinstance(interface.event, (MessageEvent, ActiveMessage)) and generic_issubclass(
+            MessageChain, interface.annotation
+        ):
+            return interface.event.message_chain
 
 
 class ContextDispatcher(AbstractDispatcher):
     """提取上下文的 Dispatcher"""
 
     @staticmethod
     async def catch(interface: DispatcherInterface):
@@ -48,14 +45,31 @@
         if generic_issubclass(asyncio.AbstractEventLoop, interface.annotation):
             return Ariadne.service.broadcast.loop
 
         if generic_issubclass(Ariadne, interface.annotation):
             return Ariadne.current()
 
 
+class LaunartInterfaceDispatcher(AbstractDispatcher):
+    @staticmethod
+    async def catch(interface: DispatcherInterface):
+        from graia.ariadne.typing import Unions, get_args, get_origin
+
+        if isinstance(interface.annotation, type) and issubclass(interface.annotation, ExportInterface):
+            manager = Launart.current()
+            with contextlib.suppress(ValueError):
+                return manager.get_interface(interface.annotation)
+        elif get_origin(interface.annotation) in Unions and (types := get_args(interface.annotation)):
+            manager = Launart.current()
+            for anno in types:
+                if isinstance(anno, type) and issubclass(anno, ExportInterface):
+                    with contextlib.suppress(ValueError):
+                        return manager.get_interface(anno)
+
+
 class NoneDispatcher(AbstractDispatcher):
     """给 Optional[...] 提供 None 的 Dispatcher"""
 
     @staticmethod
     async def catch(interface: DispatcherInterface):
         if generic_isinstance(None, interface.annotation):
             return Force(None)
@@ -70,14 +84,27 @@
 
         if isinstance(interface.event, (MessageEvent, ActiveMessage)) and generic_issubclass(
             Source, interface.annotation
         ):
             return interface.event.source
 
 
+class QuoteDispatcher(AbstractDispatcher):
+    """提取 MessageEvent 消息链 Quote 元素的 Dispatcher"""
+
+    @staticmethod
+    async def catch(interface: DispatcherInterface):
+        from .event.message import ActiveMessage, MessageEvent
+
+        if isinstance(interface.event, (MessageEvent, ActiveMessage)) and generic_issubclass(
+            Quote, interface.annotation
+        ):
+            return interface.event.quote
+
+
 class SenderDispatcher(AbstractDispatcher):
     """从 MessageEvent 提取 sender 的 Dispatcher."""
 
     @staticmethod
     async def catch(interface: DispatcherInterface):
         from .event.message import MessageEvent
 
@@ -138,27 +165,24 @@
 
 
 class OperatorDispatcher(AbstractDispatcher):
     """提取 Operator 的 Dispatcher"""
 
     @staticmethod
     async def catch(interface: DispatcherInterface):
-        if operator := interface.event.operator:
-            if generic_issubclass(Member, interface.annotation):
-                return operator
-            elif generic_issubclass(Group, interface.annotation):
-                return operator.group
+        if generic_issubclass(Member, interface.annotation):
+            return interface.event.operator
+        elif generic_issubclass(Group, interface.annotation):
+            # NOTE: operator 不为 None。因为 operator 可为 None 的事件必有 group 属性，
+            # 会由 dispatcher 之前的 GroupDispatcher 处理，不可能进入此处。
+            return interface.event.operator.group
 
 
 class OperatorMemberDispatcher(AbstractDispatcher):
     """提取 Operator 的 Dispatcher (同时有 Member 和 Operator)"""
 
-    mixin = [MemberDispatcher]
-
     @staticmethod
     async def catch(interface: DispatcherInterface):
-        if (
-            interface.name == "operator"
-            and generic_issubclass(Member, interface.annotation)
-            and (operator := interface.event.operator)
-        ):
-            return operator
+        if generic_issubclass(Member, interface.annotation):
+            return interface.event.operator if interface.name == "operator" else interface.event.member
+        elif generic_issubclass(Group, interface.annotation):
+            return interface.event.member.group
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/entry/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/entry/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,30 @@
 """Ariadne 一站式导入的提供模块"""
 
 import contextlib
 from typing import TYPE_CHECKING
 
+from . import event as event
+from . import message as message
 from ..app import Ariadne as Ariadne
+from .broadcast import *
 from ..connection.config import HttpClientConfig as HttpClientConfig
 from ..connection.config import HttpServerConfig as HttpServerConfig
 from ..connection.config import WebsocketClientConfig as WebsocketClientConfig
 from ..connection.config import WebsocketServerConfig as WebsocketServerConfig
 from ..connection.config import config as config
 from ..connection.util import UploadMethod as UploadMethod
 from ..context import ariadne_ctx as ariadne_ctx
 from ..context import broadcast_ctx as broadcast_ctx
 from ..context import event_ctx as event_ctx
 from ..context import event_loop_ctx as event_loop_ctx
 from ..context import upload_method_ctx as upload_method_ctx
 from ..dispatcher import ContextDispatcher as ContextDispatcher
 from ..dispatcher import MessageChainDispatcher as MessageChainDispatcher
 from ..dispatcher import SourceDispatcher as SourceDispatcher
-from ..exception import AccountMuted as AccountMuted
-from ..exception import AccountNotFound as AccountNotFound
-from ..exception import InvalidArgument as InvalidArgument
-from ..exception import InvalidEventTypeDefinition as InvalidEventTypeDefinition
-from ..exception import InvalidSession as InvalidSession
-from ..exception import InvalidVerifyKey as InvalidVerifyKey
-from ..exception import MessageTooLong as MessageTooLong
-from ..exception import UnknownError as UnknownError
-from ..exception import UnknownTarget as UnknownTarget
-from ..exception import UnVerifiedSession as UnVerifiedSession
-from ..model import *
-from ..util.async_exec import cpu_bound as cpu_bound
-from ..util.async_exec import io_bound as io_bound
-from ..util.cooldown import CoolDown as CoolDown
-from ..util.send import Bypass as Bypass
-from ..util.send import Ignore as Ignore
-from ..util.send import Safe as Safe
-from ..util.send import Strict as Strict
-from ..util.validator import Certain as Certain
-from ..util.validator import CertainFriend as CertainFriend
-from ..util.validator import CertainGroup as CertainGroup
-from ..util.validator import CertainMember as CertainMember
-from ..util.validator import Quoting as Quoting
-from . import event as event
-from . import message as message
-from .broadcast import *
 from .event import AccountLaunch as AccountLaunch
 from .event import AccountShutdown as AccountShutdown
 from .event import ActiveFriendMessage as ActiveFriendMessage
 from .event import ActiveGroupMessage as ActiveGroupMessage
 from .event import ActiveMessage as ActiveMessage
 from .event import ActiveStrangerMessage as ActiveStrangerMessage
 from .event import ActiveTempMessage as ActiveTempMessage
@@ -73,17 +50,15 @@
 from .event import FriendMessage as FriendMessage
 from .event import FriendNickChangedEvent as FriendNickChangedEvent
 from .event import FriendRecallEvent as FriendRecallEvent
 from .event import FriendSyncMessage as FriendSyncMessage
 from .event import GroupAllowAnonymousChatEvent as GroupAllowAnonymousChatEvent
 from .event import GroupAllowConfessTalkEvent as GroupAllowConfessTalkEvent
 from .event import GroupAllowMemberInviteEvent as GroupAllowMemberInviteEvent
-from .event import (
-    GroupEntranceAnnouncementChangeEvent as GroupEntranceAnnouncementChangeEvent,
-)
+from .event import GroupEntranceAnnouncementChangeEvent as GroupEntranceAnnouncementChangeEvent
 from .event import GroupEvent as GroupEvent
 from .event import GroupMessage as GroupMessage
 from .event import GroupMuteAllEvent as GroupMuteAllEvent
 from .event import GroupNameChangeEvent as GroupNameChangeEvent
 from .event import GroupRecallEvent as GroupRecallEvent
 from .event import GroupSyncMessage as GroupSyncMessage
 from .event import MemberCardChangeEvent as MemberCardChangeEvent
@@ -104,14 +79,24 @@
 from .event import OtherClientOnlineEvent as OtherClientOnlineEvent
 from .event import RequestEvent as RequestEvent
 from .event import StrangerMessage as StrangerMessage
 from .event import StrangerSyncMessage as StrangerSyncMessage
 from .event import SyncMessage as SyncMessage
 from .event import TempMessage as TempMessage
 from .event import TempSyncMessage as TempSyncMessage
+from ..exception import AccountMuted as AccountMuted
+from ..exception import AccountNotFound as AccountNotFound
+from ..exception import InvalidArgument as InvalidArgument
+from ..exception import InvalidEventTypeDefinition as InvalidEventTypeDefinition
+from ..exception import InvalidSession as InvalidSession
+from ..exception import InvalidVerifyKey as InvalidVerifyKey
+from ..exception import MessageTooLong as MessageTooLong
+from ..exception import UnknownError as UnknownError
+from ..exception import UnknownTarget as UnknownTarget
+from ..exception import UnVerifiedSession as UnVerifiedSession
 from .message import App as App
 from .message import Arg as Arg
 from .message import ArgResult as ArgResult
 from .message import ArgumentMatch as ArgumentMatch
 from .message import At as At
 from .message import AtAll as AtAll
 from .message import Bypass as Bypass
@@ -155,24 +140,27 @@
 from .message import Source as Source
 from .message import Sparkle as Sparkle
 from .message import Strict as Strict
 from .message import Twilight as Twilight
 from .message import UnionMatch as UnionMatch
 from .message import Voice as Voice
 from .message import WildcardMatch as WildcardMatch
+from ..model import *
 from .saya import *
 from .scheduler import *
+from ..util.async_exec import cpu_bound as cpu_bound
+from ..util.async_exec import io_bound as io_bound
+from ..util.cooldown import CoolDown as CoolDown
+from ..util.send import Bypass as Bypass
+from ..util.send import Ignore as Ignore
+from ..util.send import Safe as Safe
+from ..util.send import Strict as Strict
+from ..util.validator import Certain as Certain
+from ..util.validator import CertainFriend as CertainFriend
+from ..util.validator import CertainGroup as CertainGroup
+from ..util.validator import CertainMember as CertainMember
+from ..util.validator import Quoting as Quoting
 
 with contextlib.suppress(ImportError):
     from ..console import Console as Console
     from ..console.saya import ConsoleBehaviour as ConsoleBehaviour
     from ..console.saya import ConsoleSchema as ConsoleSchema
-
-# We are using the star import because the dependencies may not be present
-if not TYPE_CHECKING:
-
-    def __getattr__(name):
-        if name == "BotMessage":
-            from ..model import BotMessage
-
-            return BotMessage
-        raise AttributeError
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/entry/broadcast.py` & `graia-ariadne-0.9.9/src/graia/ariadne/entry/broadcast.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/entry/event.py` & `graia-ariadne-0.9.9/src/graia/ariadne/entry/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 from ..event.message import StrangerMessage as StrangerMessage
 from ..event.message import StrangerSyncMessage as StrangerSyncMessage
 from ..event.message import SyncMessage as SyncMessage
 from ..event.message import TempMessage as TempMessage
 from ..event.message import TempSyncMessage as TempSyncMessage
 from ..event.mirai import BotEvent as BotEvent
 from ..event.mirai import BotGroupPermissionChangeEvent as BotGroupPermissionChangeEvent
-from ..event.mirai import (
-    BotInvitedJoinGroupRequestEvent as BotInvitedJoinGroupRequestEvent,
-)
+from ..event.mirai import BotInvitedJoinGroupRequestEvent as BotInvitedJoinGroupRequestEvent
 from ..event.mirai import BotJoinGroupEvent as BotJoinGroupEvent
 from ..event.mirai import BotLeaveEventActive as BotLeaveEventActive
 from ..event.mirai import BotLeaveEventKick as BotLeaveEventKick
 from ..event.mirai import BotMuteEvent as BotMuteEvent
 from ..event.mirai import BotOfflineEventActive as BotOfflineEventActive
 from ..event.mirai import BotOfflineEventDropped as BotOfflineEventDropped
 from ..event.mirai import BotOfflineEventForce as BotOfflineEventForce
@@ -40,17 +38,15 @@
 from ..event.mirai import FriendEvent as FriendEvent
 from ..event.mirai import FriendInputStatusChangedEvent as FriendInputStatusChangedEvent
 from ..event.mirai import FriendNickChangedEvent as FriendNickChangedEvent
 from ..event.mirai import FriendRecallEvent as FriendRecallEvent
 from ..event.mirai import GroupAllowAnonymousChatEvent as GroupAllowAnonymousChatEvent
 from ..event.mirai import GroupAllowConfessTalkEvent as GroupAllowConfessTalkEvent
 from ..event.mirai import GroupAllowMemberInviteEvent as GroupAllowMemberInviteEvent
-from ..event.mirai import (
-    GroupEntranceAnnouncementChangeEvent as GroupEntranceAnnouncementChangeEvent,
-)
+from ..event.mirai import GroupEntranceAnnouncementChangeEvent as GroupEntranceAnnouncementChangeEvent
 from ..event.mirai import GroupEvent as GroupEvent
 from ..event.mirai import GroupMuteAllEvent as GroupMuteAllEvent
 from ..event.mirai import GroupNameChangeEvent as GroupNameChangeEvent
 from ..event.mirai import GroupRecallEvent as GroupRecallEvent
 from ..event.mirai import MemberCardChangeEvent as MemberCardChangeEvent
 from ..event.mirai import MemberHonorChangeEvent as MemberHonorChangeEvent
 from ..event.mirai import MemberJoinEvent as MemberJoinEvent
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/entry/message.py` & `graia-ariadne-0.9.9/src/graia/ariadne/entry/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Ariadne 消息相关的导入集合"""
 
 
+from ..message import Quote as Quote
+from ..message import Source as Source
 from ..message.chain import MessageChain as MessageChain
 from ..message.commander import Arg as Arg
 from ..message.commander import Commander as Commander
 from ..message.commander import Slot as Slot
 from ..message.commander import chain_validator as chain_validator
 from ..message.element import App as App
 from ..message.element import At as At
@@ -19,16 +21,14 @@
 from ..message.element import Image as Image
 from ..message.element import ImageType as ImageType
 from ..message.element import MultimediaElement as MultimediaElement
 from ..message.element import MusicShare as MusicShare
 from ..message.element import Plain as Plain
 from ..message.element import Poke as Poke
 from ..message.element import PokeMethods as PokeMethods
-from ..message.element import Quote as Quote
-from ..message.element import Source as Source
 from ..message.element import Voice as Voice
 from ..message.formatter import Formatter as Formatter
 from ..message.parser.base import ContainKeyword as ContainKeyword
 from ..message.parser.base import DetectPrefix as DetectPrefix
 from ..message.parser.base import DetectSuffix as DetectSuffix
 from ..message.parser.base import FuzzyDispatcher as FuzzyDispatcher
 from ..message.parser.base import FuzzyMatch as FuzzyMatch
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/entry/saya.py` & `graia-ariadne-0.9.9/src/graia/ariadne/entry/saya.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import contextlib
 
 __all__ = []
 
 
 with contextlib.suppress(ImportError):
     from graia.saya import Saya as Saya
-    from graia.saya import SayaModuleInstalled as SayaModuleInstalled
-    from graia.saya import SayaModuleUninstall as SayaModuleUninstall
-    from graia.saya import SayaModuleUninstalled as SayaModuleUninstalled
-    from graia.saya.builtins.broadcast.behaviour import (
-        BroadcastBehaviour as BroadcastBehaviour,
-    )
+    from graia.saya.builtins.broadcast.behaviour import BroadcastBehaviour as BroadcastBehaviour
     from graia.saya.builtins.broadcast.schema import ListenerSchema as ListenerSchema
+    from graia.saya.event import SayaModuleInstalled as SayaModuleInstalled
+    from graia.saya.event import SayaModuleUninstall as SayaModuleUninstall
+    from graia.saya.event import SayaModuleUninstalled as SayaModuleUninstalled
 
     from ..util.saya import decorate as decorate
     from ..util.saya import dispatch as dispatch
     from ..util.saya import listen as listen
 
     __all__ = [
         "Saya",
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/entry/scheduler.py` & `graia-ariadne-0.9.9/src/graia/ariadne/entry/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 __all__ = []
 
 with contextlib.suppress(ImportError):
     from graia.scheduler import GraiaScheduler as GraiaScheduler
     from graia.scheduler import SchedulerTask as SchedulerTask
     from graia.scheduler.exception import AlreadyStarted as AlreadyStarted
-    from graia.scheduler.saya.behaviour import (
-        GraiaSchedulerBehaviour as GraiaSchedulerBehaviour,
-    )
+    from graia.scheduler.saya.behaviour import GraiaSchedulerBehaviour as GraiaSchedulerBehaviour
     from graia.scheduler.saya.behaviour import SchedulerSchema as SchedulerSchema
     from graia.scheduler.timers import crontabify as crontabify
     from graia.scheduler.timers import every as every
     from graia.scheduler.timers import every_custom_hours as every_custom_hours
     from graia.scheduler.timers import every_custom_minutes as every_custom_minutes
     from graia.scheduler.timers import every_custom_seconds as every_custom_seconds
     from graia.scheduler.timers import every_hours as every_hours
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/event/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/event/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Ariadne 的事件"""
-from graia.broadcast import Dispatchable
 from pydantic import validator
 
+from graia.broadcast import Dispatchable
+
 from ..dispatcher import BaseDispatcher
 from ..exception import InvalidEventTypeDefinition
 from ..model import AriadneBaseModel
 
 
 class MiraiEvent(Dispatchable, AriadneBaseModel):
     """Ariadne 的事件基类"""
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/event/lifecycle.py` & `graia-ariadne-0.9.9/src/graia/ariadne/event/lifecycle.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/event/message.py` & `graia-ariadne-0.9.9/src/graia/ariadne/event/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 """Ariadne 消息事件"""
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union
+
+from pydantic import Field, root_validator
 
 from graia.amnesia.message import Element
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from pydantic import Field, root_validator
 
 from ..dispatcher import (
     BaseDispatcher,
     MessageChainDispatcher,
+    QuoteDispatcher,
     SenderDispatcher,
     SourceDispatcher,
     SubjectDispatcher,
 )
 from ..message.chain import MessageChain
 from ..message.element import Quote, Source
 from ..model import Client, Friend, Group, Member, Stranger
 from ..typing import generic_issubclass
 from . import MiraiEvent
 from .mirai import FriendEvent, GroupEvent
 
 
 def _set_source_quote(_, values: Dict[str, Any]) -> Dict[str, Any]:
-    for element in values["messageChain"][:2]:
+    chain: List[Union[Dict[str, Any], Element]] = values["messageChain"]
+    for element in chain[:2]:
         if isinstance(element, dict):
             elem_typ: str = element.get("type", "Unknown")
         elif isinstance(element, Element):
             elem_typ: str = element.__class__.__name__
         else:
             continue
         if elem_typ == "Source":
             values["source"] = element
         elif elem_typ == "Quote":
             values["quote"] = element
+    values["messageChain"] = list(
+        filter(
+            lambda x: (x.get("type", "Unknown") if isinstance(x, dict) else x.__class__.__name__)
+            not in ("Source", "Quote"),
+            chain,
+        )
+    )
     return values
 
 
 class MessageEvent(MiraiEvent):
     """Ariadne 消息事件基类"""
 
     type: str = "MessageEvent"
 
     message_chain: MessageChain = Field(..., alias="messageChain")
     """消息链"""
 
     sender: Union[Friend, Member, Client, Stranger]
     """发送者"""
 
-    source: Source = cast(Source, ...)
+    source: Source
     """消息元数据标识"""
 
     quote: Optional[Quote] = None
     """可能的引用消息对象"""
 
     __source_quote_setter = root_validator(pre=True, allow_reuse=True)(_set_source_quote)
 
@@ -58,15 +68,15 @@
         return self.id
 
     @property
     def id(self) -> int:
         return self.source.id
 
     class Dispatcher(BaseDispatcher):
-        mixin = [MessageChainDispatcher, SourceDispatcher, SenderDispatcher]
+        mixin = [MessageChainDispatcher, SourceDispatcher, QuoteDispatcher, SenderDispatcher]
 
 
 class FriendMessage(MessageEvent, FriendEvent):
     """好友消息"""
 
     type: str = "FriendMessage"
 
@@ -134,28 +144,28 @@
     """消息链"""
 
     sender: Stranger
     """发送者"""
 
 
 class ActiveMessage(MiraiEvent):
-    """主动消息: Bot 账号发送给他人的消息"""
+    """主动消息：Bot 账号发送给他人的消息"""
 
     type: str
 
     message_chain: MessageChain = Field(..., alias="messageChain")
     """消息链"""
 
     subject: Union[Friend, Group, Member, Stranger]
     """消息接收者"""
 
     sync: bool = False
     """是否为同步消息"""
 
-    source: Source = cast(Source, ...)
+    source: Source
     """消息元数据标识"""
 
     quote: Optional[Quote] = None
     """可能的引用消息对象"""
 
     __source_quote_setter = root_validator(pre=True, allow_reuse=True)(_set_source_quote)
 
@@ -163,51 +173,15 @@
         return self.id
 
     @property
     def id(self) -> int:
         return self.source.id
 
     class Dispatcher(BaseDispatcher):
-        mixin = [MessageChainDispatcher, SourceDispatcher, SubjectDispatcher]
-
-    if not TYPE_CHECKING:
-
-        @property
-        def messageId(self) -> int:
-            from traceback import format_exception_only
-            from warnings import warn
-
-            from loguru import logger
-
-            warning = DeprecationWarning(  # FIXME: deprecated
-                "ActiveMessage.messageId is deprecated since Ariadne 0.9, "
-                "and scheduled for removal in in Ariadne 0.10. "
-                "Use ActiveMessage.id or int(ActiveMessage) instead."
-            )
-            warn(warning, stacklevel=2)
-            logger.opt(depth=1).warning("".join(format_exception_only(type(warning), warning)).strip())
-
-            return self.id
-
-        @property
-        def origin(self) -> MessageChain:
-            from traceback import format_exception_only
-            from warnings import warn
-
-            from loguru import logger
-
-            warning = DeprecationWarning(  # FIXME: deprecated
-                "ActiveMessage.origin is deprecated since Ariadne 0.9, "
-                "and scheduled for removal in in Ariadne 0.10. "
-                "Use ActiveMessage.message_chain instead.",
-            )
-            warn(warning, stacklevel=2)
-            logger.opt(depth=2).warning("".join(format_exception_only(type(warning), warning)).strip())
-
-            return self.message_chain
+        mixin = [MessageChainDispatcher, SourceDispatcher, QuoteDispatcher, SubjectDispatcher]
 
 
 class ActiveFriendMessage(ActiveMessage):
     """主动好友消息"""
 
     type: str = "ActiveFriendMessage"
 
@@ -257,15 +231,15 @@
     """消息链"""
 
     subject: Stranger
     """消息接收者"""
 
 
 class SyncMessage(MiraiEvent):
-    """同步消息: 从其他客户端同步的主动消息"""
+    """同步消息：从其他客户端同步的主动消息"""
 
     sync = True
 
 
 class FriendSyncMessage(SyncMessage, ActiveFriendMessage):
     """好友同步消息"""
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/event/mirai.py` & `graia-ariadne-0.9.9/src/graia/ariadne/event/mirai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Mirai 的各种事件"""
 
-from datetime import datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
-
-from graia.broadcast.entities.dispatcher import BaseDispatcher as AbstractDispatcher
-from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from pydantic import Field, root_validator
-from typing_extensions import Literal
-
-from ..connection.util import CallMethod
-from ..dispatcher import (
-    BaseDispatcher,
-    FriendDispatcher,
-    GroupDispatcher,
-    MemberDispatcher,
-    NoneDispatcher,
-    OperatorDispatcher,
-    OperatorMemberDispatcher,
-)
-from ..message.chain import MessageChain
-from ..message.element import Element
-from ..model import Client, Friend, Group, Member, MemberPerm
-from ..typing import generic_issubclass
-from . import MiraiEvent
+from datetime import datetime
+from enum import Enum
+from typing import Any, Dict, List, Optional
+from typing_extensions import Literal
+
+from pydantic import Field, root_validator
+
+from graia.broadcast.entities.dispatcher import BaseDispatcher as AbstractDispatcher
+from graia.broadcast.interfaces.dispatcher import DispatcherInterface
+
+from ..connection.util import CallMethod
+from ..dispatcher import (
+    BaseDispatcher,
+    FriendDispatcher,
+    GroupDispatcher,
+    MemberDispatcher,
+    OperatorDispatcher,
+    OperatorMemberDispatcher,
+)
+from ..message.chain import MessageChain
+from ..message.element import Element
+from ..model import Client, Friend, Group, Member, MemberPerm
+from ..typing import generic_issubclass
+from . import MiraiEvent
 
 
 class BotEvent(MiraiEvent):
     """指示有关 Bot 本身的事件."""
 
 
 class FriendEvent(MiraiEvent):
@@ -311,15 +311,15 @@
 
     提供的额外注解支持:
         - Ariadne (annotation): 发布事件的应用实例
         - Group (annotation): 发生该事件的群组
         - Member (annotation): 操作者, 一定是群主.
     """
 
-    type: str = "BotLeaveEventKick"
+    type: str = "BotLeaveEventDisband"
 
     group: Group
     """Bot 退出的群的信息"""
 
     operator: Optional[Member]
     """操作员, 为群主"""
 
@@ -642,18 +642,15 @@
 
     class Dispatcher(AbstractDispatcher):
         mixin = [MemberDispatcher]
 
         @staticmethod
         async def catch(interface: DispatcherInterface["MemberJoinEvent"]):
             if interface.name == "inviter" and generic_issubclass(Member, interface.annotation):
-                if inviter := interface.event.inviter:
-                    return inviter
-                elif result := await NoneDispatcher.catch(interface):
-                    return result
+                return interface.event.inviter
 
 
 class MemberLeaveEventKick(GroupEvent):
     """有一群组成员被管理员/群主从群组中删除, 当 `operator` 为 `None` 时, 执行者为 Bot 账号.
 
     Tip:
         当监听该事件或该类事件时, 请优先考虑使用原始事件类作为类型注解, 以此获得事件类实例, 便于获取更多的信息!
@@ -915,15 +912,15 @@
         1. 同意请求: `await event.accept()`, 具体查看该方法所附带的说明.
         2. 拒绝请求: `await event.reject()`, 具体查看该方法所附带的说明.
         3. 拒绝并不再接受来自对方的请求: `await event.rejectAndBlock()`, 具体查看该方法所附带的说明.
     """
 
     type = "NewFriendRequestEvent"
 
-    requestId: int = Field(..., alias="eventId")
+    request_id: int = Field(..., alias="eventId")
     """事件标识，响应该事件时的标识"""
 
     supplicant: int = Field(..., alias="fromId")
     """申请人QQ号"""
 
     nickname: str = Field(..., alias="nick")
     """申请人的昵称或群名片"""
@@ -997,15 +994,15 @@
         3. 忽略请求: `await event.ignore()`, 具体查看该方法所附带的说明.
         4. 拒绝并不再接受来自对方的请求: `await event.rejectAndBlock()`, 具体查看该方法所附带的说明.
         5. 忽略并不再接受来自对方的请求: `await event.ignoreAndBlock()`, 具体查看该方法所附带的说明.
     """
 
     type = "MemberJoinRequestEvent"
 
-    requestId: int = Field(..., alias="eventId")
+    request_id: int = Field(..., alias="eventId")
     """事件标识，响应该事件时的标识"""
 
     supplicant: int = Field(..., alias="fromId")
     """申请人QQ号"""
 
     nickname: str = Field(..., alias="nick")
     """申请人的昵称或群名片"""
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/exception.py` & `graia-ariadne-0.9.9/src/graia/ariadne/exception.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/chain.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/chain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Ariadne 消息链的实现"""
 import re
-import warnings
 from copy import deepcopy
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
@@ -12,21 +11,21 @@
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     overload,
 )
+from typing_extensions import Self
 
 from graia.amnesia.json import Json
 from graia.amnesia.message import MessageChain as BaseMessageChain
-from typing_extensions import Self
 
 from ..model import AriadneBaseModel
-from ..util import deprecated, gen_subclass, unescape_bracket
+from ..util import gen_subclass, unescape_bracket
 from .element import (
     At,
     AtAll,
     Element,
     Face,
     File,
     Image,
@@ -139,29 +138,14 @@
                 self,
                 __root__=self.build_chain((__root__, *elements)),
             )
         else:
             AriadneBaseModel.__init__(self, __root__=[])
             self.__root__ = __root__  # type: ignore
 
-    @deprecated("0.10.0")
-    def unzip(self) -> List[Union[str, Element]]:
-        """解压消息链为元素/单字符列表.
-
-        Return:
-            List[Union[str, Element]]: 解压后的元素/字符列表.
-        """
-        unzipped: List[Union[str, Element]] = []
-        for e in self.content:
-            if isinstance(e, Plain):
-                unzipped.extend(e.text)
-            else:
-                unzipped.append(e)
-        return unzipped
-
     def __repr_args__(self) -> "ReprArgs":
         return [(None, list(self.content))]
 
     @overload
     def __getitem__(self, item: Tuple[Type[Element_T], int]) -> List[Element_T]:
         ...
 
@@ -190,62 +174,41 @@
         Args:
             item (Union[Tuple[Type[Element], int], Type[Element], int, slice]): 索引项
         Returns:
             Union[List[Element], Element, MessageChain]: 索引结果.
         """
         if isinstance(item, tuple):
             return self.get(*item)
-        if isinstance(item, (int, slice)):
-            warnings.warn(
-                "Indexing MessageChain with int will change behaviour in 0.10.0!\n"
-                "See https://github.com/GraiaProject/Ariadne/blob/dev/CHANGELOG.md#095",
-                DeprecationWarning,
-            )
         return super().__getitem__(item)
 
-    @deprecated("0.10.0", "Use `index_sub` instead")
-    def find_sub_chain(self, subchain: MessageContainer) -> List[int]:
-        """判断消息链是否含有子链. 使用 KMP 算法.
-
-        Args:
-            subchain (Union[MessageChain, List[Element]]): 要判断的子链.
-
-        Returns:
-            List[int]: 所有找到的下标.
-        """
-        sub: MessageChain = MessageChain(subchain)
-
-        return super().index_sub(sub)
-
     def as_sendable(self) -> Self:
-        """将消息链转换为可发送形式 (去除 Source, Quote, File)
+        """将消息链转换为可发送形式 (去除 File)
 
         Returns:
             MessageChain: 转换后的消息链.
         """
-        return self.exclude(Source, Quote, File)
+        return self.exclude(File)
 
     def get(self, element_class: Type[Element_T], count: int = -1) -> List[Element_T]:
         res = super().get(element_class, count)
         if isinstance(res, (Quote, Source)):
-            warnings.warn(
-                "MessageChain.get(Quote/Source) is deprecated. And will be removed in 0.10.0.\n"
+            raise IndexError(
+                "MessageChain.get(Quote/Source) is removed in 0.10.0.\n"
                 "See https://github.com/GraiaProject/Ariadne/blob/dev/CHANGELOG.md#095",
-                DeprecationWarning,
             )
         return res
 
     def __eq__(self, other: Union[MessageContainer, Self]) -> bool:
         if id(self) == id(other):
             return True
         if not isinstance(other, (MessageChain, list)):
             return False
         if not isinstance(other, MessageChain):
             other = MessageChain(other)
-        return other.as_sendable().content == self.as_sendable().content
+        return other.content == self.content
 
     def __mul__(self, time: int) -> Self:
         result = []
         for _ in range(time):
             result.extend(deepcopy(self.content))
         return MessageChain(result, inline=True)
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/commander/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/commander/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,26 @@
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
+from typing_extensions import Self
+
+from pydantic import BaseConfig, BaseModel
+from pydantic.class_validators import Validator
+from pydantic.fields import ModelField
 
 from graia.broadcast import Broadcast, Listener
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.exectarget import ExecTarget
 from graia.broadcast.exceptions import PropagationCancelled
 from graia.broadcast.typing import T_Dispatcher
 from graia.broadcast.utilles import dispatcher_mixin_handler
-from pydantic import BaseConfig, BaseModel
-from pydantic.class_validators import Validator
-from pydantic.fields import ModelField
-from typing_extensions import Self
 
 from ...context import event_ctx
 from ...dispatcher import ContextDispatcher
 from ...event.message import MessageEvent
 from ...model.util import AriadneBaseModel
 from ...typing import DictStrAny, MaybeFlag, Sentinel, Wrapper
 from ...util import constant, gen_subclass, resolve_dispatchers_mixin, type_repr
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/commander/creart.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/commander/creart.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/commander/saya.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/commander/saya.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/commander/util.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/commander/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 from __future__ import annotations
 
 import abc
 import functools
 import inspect
 import re
 from contextvars import ContextVar
-from typing import (
-    Any,
-    Dict,
-    FrozenSet,
-    Generic,
-    Iterable,
-    List,
-    MutableMapping,
-    Optional,
-    Set,
-    TypeVar,
-    Union,
-)
+from typing import Any, Generic, Iterable, List, MutableMapping, TypeVar, Union
+from typing_extensions import Self
 from weakref import WeakKeyDictionary, WeakSet
 
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.dispatcher import BaseDispatcher
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from typing_extensions import Self
 
 from ...typing import MaybeFlag, Sentinel, T
 from ..chain import MessageChain
 from ..element import Element, Plain, Quote, Source
 
 L_PAREN = ("{", "[")
 R_PAREN = ("}", "]")
@@ -69,47 +57,47 @@
     for k, v in R_ESCAPE.items():
         string = string.replace(k, v)
     return string.strip()
 
 
 class Text:
     __slots__ = "choice"
-    choice: FrozenSet[str]
+    choice: frozenset[str]
 
-    def __init__(self, choice: Union[Iterable[str], str]) -> None:
+    def __init__(self, choice: Iterable[str] | str) -> None:
         self.choice = frozenset((choice,)) if isinstance(choice, str) else frozenset(choice)
 
     def __repr__(self) -> str:
         return f"Text({self.choice!r})"
 
 
 class Param:
     __slots__ = ("names",)
-    names: FrozenSet[str]
+    names: frozenset[str]
 
     def __init__(self, names: Iterable[str]) -> None:
         self.names = frozenset(names)
 
     def __repr__(self) -> str:
         return f"Param({self.names!r})"
 
 
 class AnnotatedParam:
     __slots__ = ("name", "annotation", "default", "wildcard")
     name: str
-    annotation: Optional[str]
-    default: Optional[str]
+    annotation: str | None
+    default: str | None
     wildcard: bool
 
     def __init__(
         self,
         name: str,
         wildcard: bool = False,
-        annotation: Optional[str] = None,
-        default: Optional[str] = None,
+        annotation: str | None = None,
+        default: str | None = None,
     ) -> None:
         self.name = name
         self.annotation = annotation
         self.default = default
         self.wildcard = wildcard
 
     def __repr__(self) -> str:
@@ -122,51 +110,51 @@
 
 
 U_Token = Union[Text, Param, AnnotatedParam]
 
 ann_assign = re.compile(r"(?P<name>[^:=]+)(?P<annotation>:[^=]+)?(?P<default>=.+)?")
 
 
-def parse_param(param_str: str) -> Union[Param, AnnotatedParam]:
+def parse_param(param_str: str) -> Param | AnnotatedParam:
     wildcard: bool = param_str.startswith("...")
     if wildcard:
         param_str = param_str[3:]
     match = ann_assign.match(param_str)
     assert match, f"Invalid param: {param_str}"
     names, *extra = match.groups()
     names = [unescape(name).strip() for name in names.split("|")]
     if not wildcard and not any(extra):
         return Param(names)
     assert len(names) == 1, f"Invalid param: {param_str}"
     return AnnotatedParam(
-        names[0], wildcard, *map(lambda s: unescape(s).strip().lstrip(":=").strip() if s else None, extra)
+        names[0], wildcard, *(unescape(s).strip().lstrip(":=").strip() if s else None for s in extra)
     )
 
 
-def _pop(char_stk: List[str]) -> str:
+def _pop(char_stk: list[str]) -> str:
     piece = "".join(char_stk)
     char_stk.clear()
     return piece
 
 
-def tokenize(string: str) -> List[U_Token]:
+def tokenize(string: str) -> list[U_Token]:
     """将字符串转义化, 并处理为 Text,  Param 两种 token
 
     Args:
         string (str): 要处理的字符串
 
     Returns:
         List[Tuple[CommandToken, List[int, str]]]: 处理后的 Token
     """
 
     string = escape(string)
 
     paren: str = ""
-    char_stk: List[str] = []
-    token: List[U_Token] = []
+    char_stk: list[str] = []
+    token: list[U_Token] = []
     pop = functools.partial(_pop, char_stk)
 
     for index, char in enumerate(string):
         if char in L_PAREN + R_PAREN:
             if char in L_PAREN:
                 assert not paren, (
                     f"""Duplicated parenthesis character "{char}" @ {index} !"""
@@ -192,30 +180,30 @@
     if char_stk:
         token.append(Text(pop()))
 
     return token
 
 
 class MatchEntry:
-    def __init__(self, tokens: List[U_Token]) -> None:
-        self.nodes: List[MaybeFlag[FrozenSet[str]]] = [
+    def __init__(self, tokens: list[U_Token]) -> None:
+        self.nodes: list[MaybeFlag[frozenset[str]]] = [
             token.choice if isinstance(token, Text) else Sentinel for token in tokens
         ]
-        self.tokens: List[Union[Text, Param]] = [
+        self.tokens: list[Text | Param] = [
             token.to_param() if isinstance(token, AnnotatedParam) else token for token in tokens
         ]
-        self.params: List[Param] = [token for token in self.tokens if isinstance(token, Param)]
+        self.params: list[Param] = [token for token in self.tokens if isinstance(token, Param)]
 
 
 T_MatchEntry = TypeVar("T_MatchEntry", bound=MatchEntry)
 
 
 class MatchNode(Generic[T_MatchEntry]):
     __slots__ = ("next", "entries")
-    next: Dict[MaybeFlag[str], MatchNode[T_MatchEntry]]
+    next: dict[MaybeFlag[str], MatchNode[T_MatchEntry]]
     entries: WeakSet[T_MatchEntry]
 
     def __init__(self) -> None:
         self.next = {}
         self.entries = WeakSet()
 
     def copy(self) -> Self:
@@ -224,20 +212,20 @@
         new_obj.entries = self.entries.copy()
         return new_obj
 
     def push(self, entry: T_MatchEntry, index: int = 0) -> None:
         if index >= len(entry.nodes):
             self.entries.add(entry)
             return
-        current: MaybeFlag[FrozenSet[str]] = entry.nodes[index]
+        current: MaybeFlag[frozenset[str]] = entry.nodes[index]
         if current is Sentinel:
             self.next.setdefault(current, MatchNode()).push(entry, index + 1)
         else:
-            target_nodes: List[MatchNode[T_MatchEntry]] = []
-            conflicts: Dict[MatchNode[T_MatchEntry], Set[str]] = {}
+            target_nodes: list[MatchNode[T_MatchEntry]] = []
+            conflicts: dict[MatchNode[T_MatchEntry], set[str]] = {}
             for piece, node in {piece: self.next[piece] for piece in current if piece in self.next}.items():
                 conflicts.setdefault(node, set()).add(piece)
             for old_node, conflict_fields in conflicts.items():
                 new_node = old_node.copy()
                 target_nodes.append(new_node)
                 for field in conflict_fields:
                     self.next[field] = new_node
@@ -247,15 +235,15 @@
                 new_node = MatchNode()
                 new_node.push(entry, index + 1)
                 for field in current:
                     self.next[field] = new_node
 
     def _inspect(self, fwd=""):
         if not self.next:
-            print(fwd)
+            pass
         for k, node in self.next.items():
             node._inspect(f"{fwd}{'<PARAM>' if k is Sentinel else k} ")
 
 
 class raw(abc.ABC):  # wildcard annotation object
     ...
 
@@ -270,15 +258,15 @@
         return Sentinel
     return obj
 
 
 class ContextVarDispatcher(BaseDispatcher):
     """分发常量给指定名称的参数"""
 
-    def __init__(self, data_ctx: ContextVar[Dict[str, Any]]) -> None:
+    def __init__(self, data_ctx: ContextVar[dict[str, Any]]) -> None:
         self.data_ctx = data_ctx
 
     async def catch(self, interface: DispatcherInterface):
         return self.data_ctx.get().get(interface.name)
 
 
 ChainContent = List[Union[str, Element]]
@@ -286,15 +274,15 @@
 ChainContentList = List[ChainContent]
 
 split_cache: MutableMapping[MessageChain, ChainContentList] = WeakKeyDictionary()
 
 quote_pairs = {"'": "'", '"': '"', "‘": "’", "“": "”"}
 
 
-def extract_str(buf: ChainContent) -> Optional[str]:
+def extract_str(buf: ChainContent) -> str | None:
     if len(buf) == 1 and isinstance(buf[0], str):
         return buf[0]
 
 
 def split(chain: MessageChain) -> ChainContentList:
     if chain in split_cache:
         return split_cache[chain]
@@ -304,15 +292,15 @@
 
     for elem in chain.__root__:
         if elem.__class__ in (Quote, Source):
             continue
         if not isinstance(elem, Plain):
             buffer.append(elem)
             continue
-        cache: List[str] = []
+        cache: list[str] = []
         skipping: bool = False
         for char in elem.text:
             if char == "\\" or skipping:
                 skipping = not skipping
                 continue
             if char in quote_pairs and not quote:
                 quote = quote_pairs[char]
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/element.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from base64 import b64decode, b64encode
 from datetime import datetime
 from enum import Enum
 from io import BytesIO
 from json import dumps as j_dump
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, List, Optional, Union, overload
+from typing_extensions import Self
+
+from pydantic.fields import Field
 
 from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
 from graia.amnesia.message import Element as BaseElement
 from graia.amnesia.message import Text as BaseText
-from pydantic import validator
-from pydantic.fields import Field
-from typing_extensions import Self
 
 from ..connection.util import UploadMethod
 from ..model import AriadneBaseModel, Friend, Member, Stranger
 from ..util import escape_bracket, internal_cls
+from . import Quote as Quote  # noqa: F401
+from . import Source as Source  # noqa: F401
 
 if TYPE_CHECKING:
     from ..event.message import MessageEvent
     from ..typing import ReprArgs
     from .chain import MessageChain
 
 
@@ -116,74 +118,14 @@
     def as_persistent_string(self) -> str:
         return self.text
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, (Plain, BaseText)) and self.text == other.text
 
 
-@internal_cls()
-class Source(Element):
-    """表示消息在一个特定聊天区域内的唯一标识"""
-
-    type: str = "Source"
-
-    id: int
-    """消息 ID"""
-
-    time: datetime
-    """发送时间"""
-
-    def __int__(self):
-        return self.id
-
-    def as_persistent_string(self) -> str:
-        return ""
-
-    async def fetch_original(self) -> "MessageChain":
-        """尝试从本标记恢复原本的消息链, 有可能失败.
-
-        Returns:
-            MessageChain: 原来的消息链.
-        """
-        from ..app import Ariadne
-
-        return (await Ariadne.current().get_message_from_id(self.id)).message_chain
-
-
-@internal_cls()
-class Quote(Element):
-    """表示消息中回复其他消息/用户的部分, 通常包含一个完整的消息链(`origin` 属性)"""
-
-    type: str = "Quote"
-
-    id: int
-    """引用的消息 ID"""
-
-    group_id: int = Field(..., alias="groupId")
-    """引用消息所在群号 (好友消息为 0)"""
-
-    sender_id: int = Field(..., alias="senderId")
-    """发送者 QQ 号"""
-
-    target_id: int = Field(..., alias="targetId")
-    """原消息的接收者QQ号 (或群号) """
-
-    origin: "MessageChain"
-    """原来的消息链"""
-
-    @validator("origin", pre=True, allow_reuse=True)
-    def _(cls, v):
-        from .chain import MessageChain
-
-        return MessageChain(v)  # no need to parse objects, they are universal!
-
-    def as_persistent_string(self) -> str:
-        return ""
-
-
 class At(Element):
     """该消息元素用于承载消息中用于提醒/呼唤特定用户的部分."""
 
     type: str = "At"
 
     target: int
     """At 的目标 QQ 号"""
@@ -555,19 +497,15 @@
         if nodes:
             node_list: List[ForwardNode] = []
             for i in nodes:
                 if isinstance(i, ForwardNode):
                     node_list.append(i)
                 elif isinstance(i, MessageEvent):
                     if not isinstance(i.sender, Client):
-                        node_list.append(
-                            ForwardNode(
-                                i.sender, time=i.message_chain.get_first(Source).time, message=i.message_chain
-                            )
-                        )
+                        node_list.append(ForwardNode(i.sender, time=i.source.time, message=i.message_chain))
                 else:
                     node_list.extend(i)
             data.update(nodeList=node_list)
         super().__init__(**data)
 
     def __str__(self) -> str:
         return f"[合并转发:共{len(self.node_list)}条]"
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/formatter.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """基于 format string 的消息链格式化器"""
 from __future__ import annotations
 
 import string
-from typing import Any, Literal, Union
+from typing import Any, Literal
 
 from .chain import MessageChain
 from .element import Element, Plain
 
 _global_formatter = string.Formatter()
 
 
@@ -48,16 +48,16 @@
         elif isinstance(obj, (Element, str)):
             return [Plain(obj) if isinstance(obj, str) else obj]
         else:
             return [Plain(str(obj))]
 
     def format(
         self,
-        *args: Union[Element, MessageChain, str, Any],
-        **kwargs: Union[Element, MessageChain, str, Any],
+        *args: Element | MessageChain | str | Any,
+        **kwargs: Element | MessageChain | str | Any,
     ) -> MessageChain:
         """通过初始化时传入的格式字符串 格式化消息链
 
         Args:
             *args (Union[Element, MessageChain, str, Any]): 格式化时传入的位置参数
             **kwargs (Union[Element, MessageChain, str, Any]): 格式化时传入的关键字参数
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/parser/base.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/parser/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 """Ariadne 基础的 parser, 包括 DetectPrefix 与 DetectSuffix"""
 import abc
 import difflib
 import fnmatch
 import re
 import weakref
-from typing import (
-    ClassVar,
-    DefaultDict,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-)
+from collections import defaultdict
+from typing import ClassVar, DefaultDict, Dict, Iterable, List, Optional, Tuple, Type, Union
+from typing_extensions import get_args
 
 from graia.broadcast.builtin.derive import Derive
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.dispatcher import BaseDispatcher
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.decorator import DecoratorInterface
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from typing_extensions import get_args
 
 from ...app import Ariadne
 from ...event.message import GroupMessage, MessageEvent
 from ...typing import Unions, generic_issubclass, get_origin
 from ..chain import MessageChain
-from ..element import At, Element, Plain, Quote, Source
+from ..element import At, Element, Plain
 
 
 class ChainDecorator(abc.ABC, Decorator, Derive[MessageChain]):
     pre = True
 
     @abc.abstractmethod
     async def __call__(self, chain: MessageChain, interface: DispatcherInterface) -> Optional[MessageChain]:
@@ -53,46 +44,37 @@
 
         Args:
             prefix (Union[str, Iterable[str]]): 要匹配的前缀
         """
         self.prefix: List[str] = [prefix] if isinstance(prefix, str) else list(prefix)
 
     async def __call__(self, chain: MessageChain, _) -> Optional[MessageChain]:
-        header = chain.include(Quote, Source)
-        rest: MessageChain = chain.exclude(Quote, Source)
         for prefix in self.prefix:
-            if rest.startswith(prefix):
-                result = rest.removeprefix(prefix).removeprefix(" ")
-                break
-        else:
-            raise ExecutionStop
-        return header + result
+            if chain.startswith(prefix):
+                return chain.removeprefix(prefix).removeprefix(" ")
+
+        raise ExecutionStop
 
 
 class DetectSuffix(ChainDecorator):
     """后缀检测器"""
 
     def __init__(self, suffix: Union[str, Iterable[str]]) -> None:
         """初始化后缀检测器.
 
         Args:
             suffix (Union[str, Iterable[str]]): 要匹配的后缀
         """
         self.suffix: List[str] = [suffix] if isinstance(suffix, str) else list(suffix)
 
     async def __call__(self, chain: MessageChain, _) -> Optional[MessageChain]:
-        header = chain.include(Quote, Source)
-        rest: MessageChain = chain.exclude(Quote, Source)
         for suffix in self.suffix:
-            if rest.endswith(suffix):
-                result = rest.removesuffix(suffix).removesuffix(" ")
-                break
-        else:
-            raise ExecutionStop
-        return header + result
+            if chain.endswith(suffix):
+                return chain.removesuffix(suffix).removesuffix(" ")
+        raise ExecutionStop
 
 
 class MentionMe(ChainDecorator):
     """At 账号或者提到账号群昵称"""
 
     def __init__(self, name: Union[bool, str] = True) -> None:
         """
@@ -106,57 +88,46 @@
         ariadne = Ariadne.current()
         name: Optional[str] = self.name if isinstance(self.name, str) else None
         if self.name is True:
             if isinstance(interface.event, GroupMessage):
                 name = (await ariadne.get_member(interface.event.sender.group, ariadne.account)).name
             else:
                 name = (await ariadne.get_bot_profile()).nickname
-        header = chain.include(Quote, Source)
-        rest: MessageChain = chain.exclude(Quote, Source)
-        first: Element = rest[0]
-        result: Optional[MessageChain] = None
-        if isinstance(name, str) and rest and isinstance(first, Plain) and str(first).startswith(name):
-            result = header + rest.removeprefix(name).removeprefix(" ")
-        if rest and isinstance(first, At) and first.target == ariadne.account:
-            result = header + MessageChain(rest.__root__[1:], inline=True).removeprefix(" ")
-
-        if result is None:
-            raise ExecutionStop
-        return result
+        first: Element = chain[0]
+        if isinstance(name, str) and isinstance(first, Plain) and str(first).startswith(name):
+            return chain.removeprefix(name).removeprefix(" ")
+        if isinstance(first, At) and first.target == ariadne.account:
+            return MessageChain(chain.__root__[1:], inline=True).removeprefix(" ")
+        raise ExecutionStop
 
 
 class Mention(ChainDecorator):
     """At 或提到指定账号/名称"""
 
     def __init__(self, target: Union[int, str]) -> None:
         """
         Args:
             target (Union[int, str]): 要提到的账号或者名称, \
             如果是 int 则是账号, 如果是 str 则是名称
         """
         self.person: Union[int, str] = target
 
     async def __call__(self, chain: MessageChain, _) -> Optional[MessageChain]:
-        header = chain.include(Quote, Source)
-        rest: MessageChain = chain.exclude(Quote, Source)
-        first: Element = rest[0]
-        result: Optional[MessageChain] = None
+        first: Element = chain[0]
         if (
-            rest
+            chain
             and isinstance(first, Plain)
             and isinstance(self.person, str)
             and str(first).startswith(self.person)
         ):
-            result = header + rest.removeprefix(self.person).removeprefix(" ")
-        if rest and isinstance(first, At) and isinstance(self.person, int) and first.target == self.person:
-            result = header + MessageChain(rest.__root__[1:], inline=True).removeprefix(" ")
+            return chain.removeprefix(self.person).removeprefix(" ")
+        if isinstance(first, At) and isinstance(self.person, int) and first.target == self.person:
+            return MessageChain(chain.__root__[1:], inline=True).removeprefix(" ")
 
-        if result is None:
-            raise ExecutionStop
-        return result
+        raise ExecutionStop
 
 
 class ContainKeyword(ChainDecorator):
     """消息中含有指定关键字"""
 
     def __init__(self, keyword: str) -> None:
         """初始化
@@ -348,15 +319,15 @@
     async def __call__(self, chain: MessageChain, _) -> Optional[MessageChain]:
         if not self.match(chain):
             raise ExecutionStop
         return chain
 
 
 class FuzzyDispatcher(BaseDispatcher):
-    scope_map: ClassVar[DefaultDict[str, List[str]]] = DefaultDict(list)
+    scope_map: ClassVar[DefaultDict[str, List[str]]] = defaultdict(list)
     event_ref: ClassVar["Dict[int, Dict[str, Tuple[str, float]]]"] = {}
 
     def __init__(self, template: str, min_rate: float = 0.6, scope: str = "") -> None:
         """初始化
 
         Args:
             template (str): 模板字符串
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/parser/twilight.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/parser/twilight.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,31 +22,25 @@
     TypedDict,
     TypeVar,
     Union,
     cast,
     final,
     overload,
 )
+from typing_extensions import Self
+
+from pydantic.utils import Representation
 
 from graia.broadcast.builtin.derive import Derive, DeriveDispatcher
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.dispatcher import BaseDispatcher
 from graia.broadcast.interfaces.decorator import DecoratorInterface
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from pydantic.utils import Representation
-from typing_extensions import Self
 
-from ...typing import (
-    AnnotatedType,
-    Sentinel,
-    T,
-    generic_isinstance,
-    generic_issubclass,
-    get_origin,
-)
+from ...typing import AnnotatedType, Sentinel, T, generic_isinstance, generic_issubclass, get_origin
 from ..chain import MessageChain
 from ..commander.util import Param as ParamToken
 from ..commander.util import Text as TextToken
 from ..commander.util import tokenize
 from ..element import Element
 from .base import ChainDecorator
 from .util import (
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/message/parser/util.py` & `graia-ariadne-0.9.9/src/graia/ariadne/message/parser/util.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/model/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/model/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Ariadne 各种 model 存放的位置"""
 import functools
 from datetime import datetime
 from typing import TYPE_CHECKING, Awaitable, Callable, Dict, Optional, Type, Union
+from typing_extensions import Literal
 
 from loguru import logger
 from pydantic import Field, validator
-from typing_extensions import Literal
 
 from ..util import gen_subclass, internal_cls
 
 if TYPE_CHECKING:
     from ..app import Ariadne
     from ..event import MiraiEvent
 
@@ -189,35 +189,14 @@
     sign: str
     """个性签名"""
 
     sex: Literal["UNKNOWN", "MALE", "FEMALE"]
     """性别"""
 
 
-if not TYPE_CHECKING:
-
-    def __getattr__(name):
-        if name == "BotMessage":
-            from traceback import format_exception_only
-            from warnings import warn
-
-            from ..event.message import ActiveMessage
-
-            warning = DeprecationWarning(  # FIXME: deprecated
-                "BotMessage is deprecated since Ariadne 0.9, "
-                "and scheduled for removal in Ariadne 0.10. "
-                "Use ActiveMessage instead"
-            )
-            warn(warning, stacklevel=2)
-            logger.opt(depth=1).warning("".join(format_exception_only(type(warning), warning)).strip())
-
-            globals()["BotMessage"] = ActiveMessage
-            return ActiveMessage
-
-
 __all__ = [
     "Client",
     "Friend",
     "Group",
     "GroupConfig",
     "Member",
     "MemberInfo",
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/model/relationship.py` & `graia-ariadne-0.9.9/src/graia/ariadne/model/relationship.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/model/util.py` & `graia-ariadne-0.9.9/src/graia/ariadne/model/util.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """用于 Ariadne 数据模型的工具类."""
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Literal, Union
+from typing_extensions import NotRequired, TypedDict
 
 from pydantic import BaseConfig, BaseModel, Extra
-from typing_extensions import NotRequired, TypedDict
 
 from ..util import snake_to_camel
 
 if TYPE_CHECKING:
     from ..typing import AbstractSetIntStr, DictStrAny, MappingIntStrAny
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/service.py` & `graia-ariadne-0.9.9/src/graia/ariadne/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,84 @@
 """Ariadne 的 launart 服务相关"""
 import asyncio
 import importlib.metadata
 import json
+import re
 from typing import Coroutine, Dict, Iterable, List, Tuple, Type, overload
 
 from aiohttp import ClientSession
-from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
-from graia.broadcast import Broadcast
 from launart import Launart, Service
 from loguru import logger
 
-from .connection import (
-    CONFIG_MAP,
-    ConnectionInterface,
-    ConnectionMixin,
-    HttpClientConnection,
-)
+from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
+from graia.broadcast import Broadcast
+
+from .connection import CONFIG_MAP, ConnectionInterface, ConnectionMixin, HttpClientConnection
 from .connection._info import HttpClientInfo, U_Info
-from .dispatcher import ContextDispatcher, NoneDispatcher
+from .dispatcher import ContextDispatcher, LaunartInterfaceDispatcher, NoneDispatcher
 from .exception import AriadneConfigurationError
 
 ARIADNE_ASCII_LOGO = r"""
     _         _           _
    / \   _ __(_) __ _  __| |_ __   ___
   / _ \ | '__| |/ _` |/ _` | '_ \ / _ \
  / ___ \| |  | | (_| | (_| | | | |  __/
 /_/   \_\_|  |_|\__,_|\__,_|_| |_|\___|"""
 
 monitored_prefix = ("kayaku", "statv", "launart", "luma", "graia", "avilla")
 
+VERSION_PATTERN = re.compile(
+    r"""
+    v?
+    (?:
+        (?:(?P<epoch>[0-9]+)!)?                           # epoch
+        (?P<release>[0-9]+(?:\.[0-9]+)*)                  # release segment
+        (?P<pre>                                          # pre-release
+            [-_\.]?
+            (?P<pre_l>(a|b|c|rc|alpha|beta|pre|preview))
+            [-_\.]?
+            (?P<pre_n>[0-9]+)?
+        )?
+        (?P<post>                                         # post release
+            (?:-(?P<post_n1>[0-9]+))
+            |
+            (?:
+                [-_\.]?
+                (?P<post_l>post|rev|r)
+                [-_\.]?
+                (?P<post_n2>[0-9]+)?
+            )
+        )?
+        (?P<dev>                                          # dev release
+            [-_\.]?
+            (?P<dev_l>dev)
+            [-_\.]?
+            (?P<dev_n>[0-9]+)?
+        )?
+    )
+    (?:\+(?P<local>[a-z0-9]+(?:[-_\.][a-z0-9]+)*))?       # local version
+""",
+    re.VERBOSE | re.IGNORECASE,
+)
+
 
 async def check_update(session: ClientSession, name: str, current: str, output: List[str]) -> None:
     """在线检查更新"""
     result: str = current
+    if match := VERSION_PATTERN.fullmatch(current):
+        current = match.group("release")
     try:
         async with session.get(f"http://mirrors.aliyun.com/pypi/web/json/{name}") as resp:
             data = await resp.text()
             result: str = json.loads(data)["info"]["version"]
+            if match := VERSION_PATTERN.fullmatch(result):
+                result = match.group("release")
     except Exception as e:
         logger.warning(f"Failed to retrieve latest version of {name}: {e}")
-    if result > current:
+    if tuple(map(int, str.split(result, "."))) > tuple(map(int, str.split(current, "."))):
         output.append(
             " ".join(
                 [
                     f"[cyan]{name}[/]:" if name.startswith("graiax-") else f"[magenta]{name}[/]:",
                     f"[green]{current}[/]",
                     f"-> [yellow]{result}[/]",
                 ]
@@ -76,14 +111,16 @@
         import creart
 
         self.connections = {}
         self.broadcast = creart.it(Broadcast)
 
         if ContextDispatcher not in self.broadcast.prelude_dispatchers:
             self.broadcast.prelude_dispatchers.append(ContextDispatcher)
+        if LaunartInterfaceDispatcher not in self.broadcast.prelude_dispatchers:
+            self.broadcast.prelude_dispatchers.append(LaunartInterfaceDispatcher)
         if NoneDispatcher not in self.broadcast.finale_dispatchers:
             self.broadcast.finale_dispatchers.append(NoneDispatcher)
 
         super().__init__()
 
     @staticmethod
     def base_telemetry() -> None:
@@ -161,29 +198,19 @@
             raise ValueError(f"Connection {self.connections[account]} conflicts with {connection}")
         return connection
 
     async def launch(self, mgr: Launart):
         """Launart 启动点"""
         from .app import Ariadne
         from .context import enter_context
-        from .event.lifecycle import (
-            AccountLaunch,
-            AccountShutdown,
-            ApplicationLaunch,
-            ApplicationShutdown,
-        )
+        from .event.lifecycle import AccountLaunch, AccountShutdown, ApplicationLaunch, ApplicationShutdown
 
         self.base_telemetry()
         async with self.stage("preparing"):
             self.http_interface = mgr.get_interface(AiohttpClientInterface)
-            if self.broadcast:
-                if asyncio.get_running_loop() is not self.loop:
-                    raise AriadneConfigurationError("Broadcast is attached to a different loop")
-            else:
-                self.broadcast = Broadcast(loop=self.loop)
             if "default_account" in Ariadne.options:
                 app = Ariadne.current()
                 with enter_context(app=app):
                     self.broadcast.postEvent(ApplicationLaunch(app))
             for conn in self.connections.values():
                 app = Ariadne.current(conn.info.account)
                 with enter_context(app=app):
@@ -205,17 +232,14 @@
             for task in asyncio.all_tasks():
                 if task.done():
                     continue
                 coro: Coroutine = task.get_coro()  # type: ignore
                 if coro.__qualname__ == "Broadcast.Executor":
                     task.cancel()
                     logger.debug(f"Cancelled {task.get_name()} (Broadcast.Executor)")
-                elif coro.cr_frame.f_globals["__name__"].startswith("graia.scheduler"):
-                    task.cancel()
-                    logger.debug(f"Cancelled {task.get_name()} (Scheduler Task)")
 
             logger.info("Checking for updates...", alt="[cyan]Checking for updates...[/]")
             await self.check_update()
 
     @property
     def client_session(self) -> ClientSession:
         """获取 aiohttp 的 ClientSession
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/typing.py` & `graia-ariadne-0.9.9/src/graia/ariadne/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Ariadne 的类型标注"""
 
 
-import builtins
 import contextlib
 import enum
 import sys
 import types
-from types import MethodType, TracebackType
+import typing_extensions
+from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
     Dict,
     Generic,
@@ -20,24 +20,15 @@
     Sequence,
     Tuple,
     Type,
     TypedDict,
     TypeVar,
     Union,
 )
-
-import typing_extensions
-from typing_extensions import (
-    Annotated,
-    ParamSpec,
-    Protocol,
-    TypeAlias,
-    get_args,
-    runtime_checkable,
-)
+from typing_extensions import Annotated, ParamSpec, Protocol, TypeAlias, get_args, runtime_checkable
 
 if TYPE_CHECKING:
     from .event.message import ActiveMessage
     from .message.chain import MessageChain
     from .model import Friend, Group, Member
 
 P = ParamSpec("P")
@@ -203,23 +194,18 @@
 
 Wrapper: TypeAlias = Callable[[T_Callable], T_Callable]
 
 AnnotatedType = type(Annotated[int, lambda x: x > 0])
 
 ExceptionHook: TypeAlias = Callable[[Type[BaseException], BaseException, Optional[TracebackType]], Any]
 
-if sys.version_info >= (3, 9):
-    classmethod = builtins.classmethod
-else:
 
-    class classmethod:
-        "Emulate PyClassMethod_Type()"
+class class_property(Generic[T]):
+    """Class-level property.
+    Link: https://stackoverflow.com/a/13624858/1280629
+    """
 
-        def __init__(self, f):
-            self.f = f
+    def __init__(self, fget: Callable[[Any], T]):
+        self.fget = fget
 
-        def __get__(self, obj, cls=None):
-            if cls is None:
-                cls = type(obj)
-            if hasattr(type(self.f), "__get__"):
-                return self.f.__get__(cls, cls)
-            return MethodType(self.f, cls)
+    def __get__(self, _, owner_cls) -> T:
+        return self.fget(owner_cls)
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/util/__init__.py` & `graia-ariadne-0.9.9/src/graia/ariadne/util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,27 +21,24 @@
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
+from loguru import logger
+
 from graia.broadcast import Broadcast
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.event import Dispatchable
 from graia.broadcast.entities.listener import Listener
 from graia.broadcast.entities.namespace import Namespace
-from graia.broadcast.exceptions import (
-    ExecutionStop,
-    PropagationCancelled,
-    RequirementCrashed,
-)
+from graia.broadcast.exceptions import ExecutionStop, PropagationCancelled, RequirementCrashed
 from graia.broadcast.typing import T_Dispatcher
 from graia.broadcast.utilles import dispatcher_mixin_handler
-from loguru import logger
 
 from ..typing import ExceptionHook, P, R, T, Wrapper
 
 if TYPE_CHECKING:
     from datetime import datetime
 
     from rich.console import Console
@@ -169,14 +166,15 @@
                 events,
                 inline_dispatchers=inline_dispatchers or [],
                 decorators=decorators or [],
                 priority=priority,
             )
 
     import creart
+
     import graia.broadcast.entities.listener
 
     graia.broadcast.entities.listener.Listener = BypassListener  # type: ignore
     graia.broadcast.Listener = BypassListener  # type: ignore
 
     if creart.exists_module("graia.saya"):
         import graia.saya.builtins.broadcast.schema
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/util/async_exec.py` & `graia-ariadne-0.9.9/src/graia/ariadne/util/async_exec.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/util/interrupt.py` & `graia-ariadne-0.9.9/src/graia/ariadne/util/interrupt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Broadcast Interrupt 相关的工具"""
 import asyncio
 from typing import Awaitable, Callable, Generic, List, Optional, Type, TypeVar, cast
+from typing_extensions import overload
 
 from creart import it
+
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.event import Dispatchable
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.interrupt import InterruptControl, Waiter
 from graia.broadcast.typing import T_Dispatcher
-from typing_extensions import overload
 
 from ..typing import T
 
 T_E = TypeVar("T_E", bound=Dispatchable)
 
 
 class _ExtendedWaiter(Waiter, Generic[T, T_E]):
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/util/saya.py` & `graia-ariadne-0.9.9/src/graia/ariadne/util/saya.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Saya 相关的工具"""
 from __future__ import annotations
 
 import inspect
-from typing import Callable, Dict, List, Optional, Type, Union, overload
+from typing import Callable, overload
 
 from graia.broadcast.entities.decorator import Decorator
 from graia.broadcast.entities.event import Dispatchable
 from graia.broadcast.typing import T_Dispatcher
 from graia.saya import Channel
 from graia.saya.builtins.broadcast.schema import ListenerSchema
 from graia.saya.cube import Cube
@@ -74,15 +74,15 @@
     Returns:
         Callable[[T_Callable], T_Callable]: 装饰器
     """
     ...
 
 
 @overload
-def decorate(map: Dict[str, Decorator], /) -> Wrapper:
+def decorate(map: dict[str, Decorator], /) -> Wrapper:
     """给指定参数名称附加装饰器
 
     Args:
         map (Dict[str, Decorator]): 参数名称与装饰器的映射
 
     Returns:
         Callable[[T_Callable], T_Callable]: 装饰器
@@ -96,15 +96,15 @@
     Args:
         name (str | Dict[str, Decorator]): 参数名称或与装饰器的映射
         decorator (Decorator): 装饰器
 
     Returns:
         Callable[[T_Callable], T_Callable]: 装饰器
     """
-    arg: Union[Dict[str, Decorator], List[Decorator]]
+    arg: dict[str, Decorator] | list[Decorator]
     if isinstance(args[0], str):
         name: str = args[0]
         decorator: Decorator = args[1]
         arg = {name: decorator}
     elif isinstance(args[0], dict):
         arg = args[0]
     else:
@@ -122,47 +122,47 @@
                     setattr(param, "_default", arg[param.name])
             func.__signature__ = sig
         return func
 
     return wrapper
 
 
-def listen(*event: Union[Type[Dispatchable], str]) -> Wrapper:
+def listen(*event: type[Dispatchable] | str) -> Wrapper:
     """在当前 Saya Channel 中监听指定事件
 
     Args:
         *event (Union[Type[Dispatchable], str]): 事件类型或事件名称
 
     Returns:
         Callable[[T_Callable], T_Callable]: 装饰器
     """
-    EVENTS: Dict[str, Type[Dispatchable]] = {e.__name__: e for e in gen_subclass(Dispatchable)}
-    events: List[Type[Dispatchable]] = [e if isinstance(e, type) else EVENTS[e] for e in event]
+    EVENTS: dict[str, type[Dispatchable]] = {e.__name__: e for e in gen_subclass(Dispatchable)}
+    events: list[type[Dispatchable]] = [e if isinstance(e, type) else EVENTS[e] for e in event]
 
     def wrapper(func: T_Callable) -> T_Callable:
         cube = ensure_cube_as_listener(func)
         cube.metaclass.listening_events.extend(events)
         return func
 
     return wrapper
 
 
-def priority(priority: int, *events: Type[Dispatchable]) -> Wrapper:
+def priority(priority: int, *events: type[Dispatchable]) -> Wrapper:
     """设置事件优先级
 
     Args:
         priority (int): 事件优先级
         *events (Type[Dispatchable]): 提供时则会设置这些事件的优先级, 否则设置全局优先级
 
     Returns:
         Callable[[T_Callable], T_Callable]: 装饰器
     """
 
     def wrapper(func: T_Callable) -> T_Callable:
         cube = ensure_cube_as_listener(func)
         cube.metaclass.priority = priority
         if events:
-            extra: Dict[Optional[Type[Dispatchable]], int] = getattr(cube.metaclass, "extra_priorities", {})
+            extra: dict[type[Dispatchable] | None, int] = getattr(cube.metaclass, "extra_priorities", {})
             extra.update((e, priority) for e in events)
         return func
 
     return wrapper
```

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/util/send.py` & `graia-ariadne-0.9.9/src/graia/ariadne/util/send.py`

 * *Files identical despite different names*

### Comparing `graia-ariadne-0.9.8/src/graia/ariadne/util/validator.py` & `graia-ariadne-0.9.9/src/graia/ariadne/util/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,36 +101,31 @@
 class Quoting(Decorator):
     """需要回复指定的消息"""
 
     pre = True
 
     msg_ids: Set[int]
 
-    def __init__(self, message: SequenceOrInstance[Union[int, ActiveMessage, MessageChain, Source]]):
+    def __init__(self, message: SequenceOrInstance[Union[int, ActiveMessage, Source]]):
         """
         Args:
-            message (SequenceOrInstance[Union[int, ActiveMessage, MessageChain, Source]]): 要回复的指定信息
+            message (SequenceOrInstance[Union[int, ActiveMessage, Source]]): 要回复的指定信息
         """
         if not isinstance(message, Sequence):
             message = [message]
         self.msg_ids = set()
         for msg in message:
-            if isinstance(msg, ActiveMessage):
-                self.msg_ids.add(msg.id)
-            elif isinstance(msg, MessageChain):
-                self.msg_ids.add(msg.get_first(Quote).id)
-            elif isinstance(msg, Source):
+            if isinstance(msg, (ActiveMessage, Source)):
                 self.msg_ids.add(msg.id)
             else:
                 self.msg_ids.add(msg)
 
     async def target(self, i: DecoratorInterface):
         try:
-            msg_chain: MessageChain = await i.dispatcher_interface.lookup_param(
-                "__decorator_parameter__", MessageChain, None
+            quote: Union[Quote, None] = await i.dispatcher_interface.lookup_param(
+                "__decorator_parameter_quote__", Union[Quote, None], None
             )
-            quotes = msg_chain.get(Quote)
-            if not quotes or quotes[0].id not in self.msg_ids:
+            if not quote or quote.id not in self.msg_ids:
                 raise RequirementCrashed
         except RequirementCrashed as e:
             raise ExecutionStop from e
-        return msg_chain
+        return await i.dispatcher_interface.lookup_param("__decorator_parameter__", MessageChain, None)
```

### Comparing `graia-ariadne-0.9.8/PKG-INFO` & `graia-ariadne-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graia-ariadne
-Version: 0.9.8
+Version: 0.9.9
 Summary: Another elegant Python QQ Bot framework for mirai and mirai-api-http v2.
 Keywords: graia,bot,qq,framework,mirai,ariadne
 Author-email: BlueGlassBlock <blueglassblock@outlook.com>,GreyElaina <GreyElaina@outlook.com>
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Robot Framework :: Library
```

