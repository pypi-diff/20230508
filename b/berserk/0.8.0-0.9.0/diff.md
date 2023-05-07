# Comparing `tmp/berserk-0.8.0.tar.gz` & `tmp/berserk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/berserk-0.8.0.tar", last modified: Sun Mar  8 19:03:01 2020, max compression
+gzip compressed data, was "dist/berserk-0.9.0.tar", last modified: Wed Apr 15 05:37:41 2020, max compression
```

## Comparing `berserk-0.8.0.tar` & `berserk-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/
--rw-r--r--   0 rhgrant10   (501) staff       (20)      463 2020-01-21 00:14:44.000000 berserk-0.8.0/AUTHORS.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)     3512 2018-06-09 15:00:24.000000 berserk-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)     2893 2020-03-08 18:57:06.000000 berserk-0.8.0/HISTORY.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1548 2018-06-09 15:00:24.000000 berserk-0.8.0/LICENSE
--rw-r--r--   0 rhgrant10   (501) staff       (20)      289 2018-06-11 02:14:12.000000 berserk-0.8.0/MANIFEST.in
--rw-r--r--   0 rhgrant10   (501) staff       (20)     9025 2020-03-08 19:03:01.000000 berserk-0.8.0/PKG-INFO
--rw-r--r--   0 rhgrant10   (501) staff       (20)     3415 2020-01-26 11:43:40.000000 berserk-0.8.0/README.rst
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/berserk/
--rw-r--r--   0 rhgrant10   (501) staff       (20)      691 2020-03-08 19:02:14.000000 berserk-0.8.0/berserk/__init__.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)    32539 2020-03-08 18:58:02.000000 berserk-0.8.0/berserk/clients.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)    15873 2020-01-04 19:24:01.000000 berserk-0.8.0/berserk/enums.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1621 2020-01-21 00:14:44.000000 berserk-0.8.0/berserk/exceptions.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     4252 2020-01-19 22:23:42.000000 berserk-0.8.0/berserk/formats.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1833 2020-01-26 10:34:13.000000 berserk-0.8.0/berserk/models.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     2470 2020-01-22 07:20:13.000000 berserk-0.8.0/berserk/session.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     3523 2020-01-25 05:26:54.000000 berserk-0.8.0/berserk/utils.py
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/berserk.egg-info/
--rw-r--r--   0 rhgrant10   (501) staff       (20)     9025 2020-03-08 19:03:00.000000 berserk-0.8.0/berserk.egg-info/PKG-INFO
--rw-r--r--   0 rhgrant10   (501) staff       (20)      845 2020-03-08 19:03:00.000000 berserk-0.8.0/berserk.egg-info/SOURCES.txt
--rw-r--r--   0 rhgrant10   (501) staff       (20)        1 2020-03-08 19:03:00.000000 berserk-0.8.0/berserk.egg-info/dependency_links.txt
--rw-r--r--   0 rhgrant10   (501) staff       (20)       45 2020-03-08 19:03:00.000000 berserk-0.8.0/berserk.egg-info/requires.txt
--rw-r--r--   0 rhgrant10   (501) staff       (20)        8 2020-03-08 19:03:00.000000 berserk-0.8.0/berserk.egg-info/top_level.txt
--rw-r--r--   0 rhgrant10   (501) staff       (20)        1 2020-03-08 19:03:00.000000 berserk-0.8.0/berserk.egg-info/zip-safe
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/docs/
--rw-r--r--   0 rhgrant10   (501) staff       (20)      608 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/Makefile
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/docs/_build/
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/docs/_build/html/
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/docs/_build/html/_static/
--rw-r--r--   0 rhgrant10   (501) staff       (20)      286 2020-01-21 06:53:28.000000 berserk-0.8.0/docs/_build/html/_static/file.png
--rw-r--r--   0 rhgrant10   (501) staff       (20)       90 2020-01-21 06:53:28.000000 berserk-0.8.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 rhgrant10   (501) staff       (20)       90 2020-01-21 06:53:28.000000 berserk-0.8.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 rhgrant10   (501) staff       (20)     2047 2020-01-26 12:50:35.000000 berserk-0.8.0/docs/announcing.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)      629 2020-01-25 04:06:10.000000 berserk-0.8.0/docs/api.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)       28 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/authors.rst
--rwxr-xr-x   0 rhgrant10   (501) staff       (20)     5623 2020-01-21 00:14:44.000000 berserk-0.8.0/docs/conf.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)       33 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/contributing.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)       28 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/history.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1612 2020-01-21 00:14:44.000000 berserk-0.8.0/docs/index.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1118 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/installation.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)      769 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/make.bat
--rw-r--r--   0 rhgrant10   (501) staff       (20)       27 2018-06-09 15:00:24.000000 berserk-0.8.0/docs/readme.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)    15407 2020-01-21 00:14:44.000000 berserk-0.8.0/docs/usage.rst
--rw-r--r--   0 rhgrant10   (501) staff       (20)       44 2020-01-26 10:47:40.000000 berserk-0.8.0/requirements.txt
--rw-r--r--   0 rhgrant10   (501) staff       (20)      189 2020-01-04 19:14:38.000000 berserk-0.8.0/requirements_dev.txt
--rw-r--r--   0 rhgrant10   (501) staff       (20)      449 2020-03-08 19:03:01.000000 berserk-0.8.0/setup.cfg
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1415 2020-03-08 19:01:44.000000 berserk-0.8.0/setup.py
-drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-03-08 19:03:01.000000 berserk-0.8.0/tests/
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1644 2018-06-15 03:21:29.000000 berserk-0.8.0/tests/test_formats.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)      277 2018-12-23 18:51:09.000000 berserk-0.8.0/tests/test_models.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     1238 2018-12-23 18:51:09.000000 berserk-0.8.0/tests/test_session.py
--rw-r--r--   0 rhgrant10   (501) staff       (20)     2165 2020-01-21 00:30:15.000000 berserk-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     9592 2020-04-15 05:37:41.000000 berserk-0.9.0/PKG-INFO
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1548 2018-06-09 15:00:24.000000 berserk-0.9.0/LICENSE
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       44 2020-01-26 10:47:40.000000 berserk-0.9.0/requirements.txt
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     3499 2020-04-15 05:13:46.000000 berserk-0.9.0/CONTRIBUTING.rst
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     9592 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/PKG-INFO
+-rw-r--r--   0 rhgrant10   (501) staff       (20)        1 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/zip-safe
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      845 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/SOURCES.txt
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       45 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/requires.txt
+-rw-r--r--   0 rhgrant10   (501) staff       (20)        8 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/top_level.txt
+-rw-r--r--   0 rhgrant10   (501) staff       (20)        1 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk.egg-info/dependency_links.txt
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/tests/
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     2165 2020-01-21 00:30:15.000000 berserk-0.9.0/tests/test_utils.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1238 2018-12-23 18:51:09.000000 berserk-0.9.0/tests/test_session.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1644 2018-06-15 03:21:29.000000 berserk-0.9.0/tests/test_formats.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      277 2018-12-23 18:51:09.000000 berserk-0.9.0/tests/test_models.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      289 2018-06-11 02:14:12.000000 berserk-0.9.0/MANIFEST.in
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/docs/
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1015 2020-04-15 05:01:39.000000 berserk-0.9.0/docs/index.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       33 2018-06-09 15:00:24.000000 berserk-0.9.0/docs/contributing.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     2047 2020-04-14 16:07:22.000000 berserk-0.9.0/docs/announcing.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      608 2018-06-09 15:00:24.000000 berserk-0.9.0/docs/Makefile
+-rwxr-xr-x   0 rhgrant10   (501) staff       (20)     5624 2020-04-15 04:44:36.000000 berserk-0.9.0/docs/conf.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)    15407 2020-04-15 05:12:56.000000 berserk-0.9.0/docs/usage.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      769 2018-06-09 15:00:24.000000 berserk-0.9.0/docs/make.bat
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/docs/_build/
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/docs/_build/html/
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/docs/_build/html/_static/
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       90 2020-01-21 06:53:28.000000 berserk-0.9.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      286 2020-01-21 06:53:28.000000 berserk-0.9.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       90 2020-01-21 06:53:28.000000 berserk-0.9.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       28 2018-06-09 15:00:24.000000 berserk-0.9.0/docs/history.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1105 2020-04-15 05:12:34.000000 berserk-0.9.0/docs/installation.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       28 2018-06-09 15:00:24.000000 berserk-0.9.0/docs/authors.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)       27 2018-06-09 15:00:24.000000 berserk-0.9.0/docs/readme.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      661 2020-04-15 05:13:02.000000 berserk-0.9.0/docs/api.rst
+drwxr-xr-x   0 rhgrant10   (501) staff       (20)        0 2020-04-15 05:37:41.000000 berserk-0.9.0/berserk/
+-rw-r--r--   0 rhgrant10   (501) staff       (20)    15873 2020-01-04 19:24:01.000000 berserk-0.9.0/berserk/enums.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1833 2020-01-26 10:34:13.000000 berserk-0.9.0/berserk/models.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     2470 2020-01-22 07:20:13.000000 berserk-0.9.0/berserk/session.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      691 2020-04-15 05:35:10.000000 berserk-0.9.0/berserk/__init__.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     3523 2020-04-13 15:58:40.000000 berserk-0.9.0/berserk/utils.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     4539 2020-04-14 04:57:33.000000 berserk-0.9.0/berserk/formats.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)    35422 2020-04-14 15:55:15.000000 berserk-0.9.0/berserk/clients.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1612 2020-04-14 04:57:33.000000 berserk-0.9.0/berserk/exceptions.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     1415 2020-04-15 05:35:10.000000 berserk-0.9.0/setup.py
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     3082 2020-04-15 05:34:54.000000 berserk-0.9.0/HISTORY.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      180 2020-04-15 05:10:33.000000 berserk-0.9.0/AUTHORS.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      482 2020-04-15 05:37:41.000000 berserk-0.9.0/setup.cfg
+-rw-r--r--   0 rhgrant10   (501) staff       (20)     3713 2020-04-15 05:24:58.000000 berserk-0.9.0/README.rst
+-rw-r--r--   0 rhgrant10   (501) staff       (20)      224 2020-04-14 16:05:02.000000 berserk-0.9.0/requirements_dev.txt
```

### Comparing `berserk-0.8.0/CONTRIBUTING.rst` & `berserk-0.9.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .. highlight:: shell
 
-============
 Contributing
 ============
 
 Contributions are welcome, and they are greatly appreciated! Every little bit
 helps, and credit will always be given.
 
 You can contribute in many ways:
```

### Comparing `berserk-0.8.0/HISTORY.rst` & `berserk-0.9.0/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-=======
 History
 =======
 
+0.9.0 (2020-04-14)
+------------------
+
+* Add remaining ``Board`` endpoints: seek, handle_draw_offer, offer_draw, accept_draw, and decline_draw
+* Multiple doc updates/fixes
+* Add codecov reporting
+
 0.8.0 (2020-03-08)
-==================
+------------------
 
 * Add new ``Board`` client: stream_incoming_events, stream_game_state, make_move, post_message, abort_game, and resign_game
 
 0.7.0 (2020-01-26)
-==================
+------------------
 
 * Add simuls
 * Add studies export and export chapter
 * Add tournament results, games export, and list by creator
 * Add user followers, users following, rating history, and puzzle activity
 * Add new ``Teams`` client: join, get members, kick member, and leave
 * Updated documentation, including new docs for some useful utils
 * Fixed bugs in ``Tournaments.export_games``
 * Deprecated ``Users.get_by_team`` - use ``Teams.get_members`` instead
 
 
 0.6.1 (2020-01-20)
-==================
+------------------
 
 * Add py37 to the travis build
 * Update development status classifier to 4 - Beta
 * Fix py36 issue preventing successful build
 * Make updates to the Makefile
 
 
 0.6.0 (2020-01-20)
-==================
+------------------
 
 * Add logging to the ``berserk.session`` module
 * Fix exception message when no cause
 * Fix bug in ``Broadcasts.push_pgn_update``
 * Update documentation and tweak the theme
 
 
 0.5.0 (2020-01-20)
-==================
+------------------
 
 * Add ``ResponseError`` for 4xx and 5xx responses with status code, reason, and cause
 * Add ``ApiError`` for all other request errors
 * Fix test case broken by 0.4.0 release
 * Put all utils code under test
 
 
 0.4.0 (2020-01-19)
-==================
+------------------
 
 * Add support for the broadcast endpoints
 * Add a utility for easily converting API objects into update params
 * Fix multiple bugs with the tournament create endpoint
 * Improve the reusability of some conversion utilities
 * Improve many docstrings in the client classes
 
 
 0.3.2 (2020-01-04)
-==================
+------------------
 
 * Fix bug where options not passed for challenge creation
 * Convert requirements from pinned to sematically compatible
 * Bump all developer dependencies
 * Use pytest instead of the older py.test
 * Use py37 in tox
 
 
 0.3.1 (2018-12-23)
-==================
+------------------
 
 * Convert datetime string in tournament creation response into datetime object
 
 
 0.3.0 (2018-12-23)
-==================
+------------------
 
 * Convert all timestamps to datetime in all responses
 * Provide support for challenging other players to a game
 
 
 0.2.1 (2018-12-08)
-==================
+------------------
 
-* Bump requests dependency to >=2.20.0 (CVE-2018-18074)
+* Bump requests dependency to >-2.20.0 (CVE-2018-18074)
 
 
 0.2.0 (2018-12-08)
-==================
+------------------
 
 * Add `position` and `start_date` params to `Tournament.create`
 * Add `Position` enum
 
 
 0.1.2 (2018-07-14)
-==================
+------------------
 
 * Fix an asine bug in the docs
 
 
 0.1.1 (2018-07-14)
-==================
+------------------
 
 * Added tests for session and formats modules
 * Fixed mispelled PgnHandler class (!)
 * Fixed issue with trailing whitespace when splitting multiple PGN texts
 * Fixed the usage overview in the README
 * Fixed the versions for travis-ci
 * Made it easier to test the `JsonHandler` class
 * Salted the bumpversion config to taste
 
 
 0.1.0 (2018-07-10)
-==================
+------------------
 
 * First release on PyPI.
```

### Comparing `berserk-0.8.0/LICENSE` & `berserk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/PKG-INFO` & `berserk-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 Metadata-Version: 2.1
 Name: berserk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for the lichess API
 Home-page: https://github.com/rhgrant10/berserk
 Author: Robert Grant
 Author-email: rhgrant10@gmail.com
 License: GNU General Public License v3
 Description: =======
         berserk
         =======
         
         
         .. image:: https://img.shields.io/pypi/v/berserk.svg
                 :target: https://pypi.python.org/pypi/berserk
+                :alt: Available on PyPI
         
         .. image:: https://img.shields.io/travis/rhgrant10/berserk.svg
                 :target: https://travis-ci.org/rhgrant10/berserk
+                :alt: Continuous Integration
+        
+        .. image:: https://codecov.io/gh/rhgrant10/berserk/branch/master/graph/badge.svg
+                :target: https://codecov.io/gh/rhgrant10/berserk
+                :alt: Code Coverage
         
         .. image:: https://readthedocs.org/projects/berserk/badge/?version=latest
                 :target: https://berserk.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        Python client for the lichess API
+        Python client for the `Lichess API`_.
         
+        .. _Lichess API: https://lichess.org/api
         
         * Free software: GNU General Public License v3
         * Documentation: https://berserk.readthedocs.io.
         
         
         Features
         ========
         
         * handles JSON and PGN formats at user's discretion
-        * token auth support provided
+        * token auth session
         * easy integration with OAuth2
+        * automatically converts time values to datetimes
         
         Usage
         =====
         
         You can use any ``requests.Session``-like object as a session, including those
         from ``requests_oauth``. A simple token session is included, as shown below:
         
@@ -49,220 +57,222 @@
             session = berserk.TokenSession(API_TOKEN)
             client = berserk.Client(session=session)
         
         Most if not all of the API is available:
         
         .. code-block:: python
         
-                client.account.get
-                client.account.get_email
-                client.account.get_preferences
-                client.account.get_kid_mode
-                client.account.set_kid_mode
-                client.account.upgrade_to_bot
-        
-                client.users.get_puzzle_activity
-                client.users.get_realtime_statuses
-                client.users.get_all_top_10
-                client.users.get_leaderboard
-                client.users.get_public_data
-                client.users.get_activity_feed
-                client.users.get_by_id
-                client.users.get_live_streamers
-                client.users.get_users_followed
-                client.users.get_users_following
-                client.users.get_rating_history
-        
-                client.teams.get_members
-                client.teams.join
-                client.teams.leave
-                client.teams.kick_member
-        
-                client.games.export
-                client.games.export_by_player
-                client.games.export_multi
-                client.games.get_among_players
-                client.games.get_ongoing
-                client.games.get_tv_channels
-        
-                client.challenges.create
-                client.challenges.accept
-                client.challenges.decline
-        
-                client.bots.stream_incoming_events
-                client.bots.stream_game_state
-                client.bots.make_move
-                client.bots.post_message
-                client.bots.abort_game
-                client.bots.resign_game
-                client.bots.accept_challenge
-                client.bots.decline_challenge
-        
-                client.tournaments.get
-                client.tournaments.create
-                client.tournaments.export_games
-                client.tournaments.stream_results
-                client.tournaments.stream_by_creator
-        
-                client.broadcasts.create
-                client.broadcasts.get
-                client.broadcasts.update
-                client.broadcasts.push_pgn_update
+            client.account.get
+            client.account.get_email
+            client.account.get_preferences
+            client.account.get_kid_mode
+            client.account.set_kid_mode
+            client.account.upgrade_to_bot
+        
+            client.users.get_puzzle_activity
+            client.users.get_realtime_statuses
+            client.users.get_all_top_10
+            client.users.get_leaderboard
+            client.users.get_public_data
+            client.users.get_activity_feed
+            client.users.get_by_id
+            client.users.get_by_team
+            client.users.get_live_streamers
+            client.users.get_users_followed
+            client.users.get_users_following
+            client.users.get_rating_history
+        
+            client.teams.get_members
+            client.teams.join
+            client.teams.leave
+            client.teams.kick_member
+        
+            client.games.export
+            client.games.export_by_player
+            client.games.export_multi
+            client.games.get_among_players
+            client.games.get_ongoing
+            client.games.get_tv_channels
+        
+            client.challenges.create
+            client.challenges.accept
+            client.challenges.decline
+        
+            client.board.stream_incoming_events
+            client.board.seek
+            client.board.stream_game_state
+            client.board.make_move
+            client.board.post_message
+            client.board.abort_game
+            client.board.resign_game
+            client.board.handle_draw_offer
+            client.board.offer_draw
+            client.board.accept_draw
+            client.board.decline_draw
+        
+            client.bots.stream_incoming_events
+            client.bots.stream_game_state
+            client.bots.make_move
+            client.bots.post_message
+            client.bots.abort_game
+            client.bots.resign_game
+            client.bots.accept_challenge
+            client.bots.decline_challenge
+        
+            client.tournaments.get
+            client.tournaments.create
+            client.tournaments.export_games
+            client.tournaments.stream_results
+            client.tournaments.stream_by_creator
+        
+            client.broadcasts.create
+            client.broadcasts.get
+            client.broadcasts.update
+            client.broadcasts.push_pgn_update
         
-                client.simuls.get
+            client.simuls.get
         
-                client.studies.export_chapter
-                client.studies.export
+            client.studies.export_chapter
+            client.studies.export
         
         
         Details for each function can be found in the `full documentation <https://berserk.readthedocs.io>`_.
         
         
         Credits
         =======
         
-        Authors
-        -------
-        
-        Development Lead
-        ~~~~~~~~~~~~~~~~
-        
-        * Robert Grant <rhgrant10@gmail.com>
-        
-        Contributors
-        ~~~~~~~~~~~~
-        
-        * Robert Graham <rpgraham84@gmail.com>
-        
-        
-        Miscellaneous
-        -------------
-        
         This package was created with Cookiecutter_ and the
         `audreyr/cookiecutter-pypackage`_ project template.
         
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         
-        =======
         History
         =======
         
+        0.9.0 (2020-04-14)
+        ------------------
+        
+        * Add remaining ``Board`` endpoints: seek, handle_draw_offer, offer_draw, accept_draw, and decline_draw
+        * Multiple doc updates/fixes
+        * Add codecov reporting
+        
         0.8.0 (2020-03-08)
-        ==================
+        ------------------
         
         * Add new ``Board`` client: stream_incoming_events, stream_game_state, make_move, post_message, abort_game, and resign_game
         
         0.7.0 (2020-01-26)
-        ==================
+        ------------------
         
         * Add simuls
         * Add studies export and export chapter
         * Add tournament results, games export, and list by creator
         * Add user followers, users following, rating history, and puzzle activity
         * Add new ``Teams`` client: join, get members, kick member, and leave
         * Updated documentation, including new docs for some useful utils
         * Fixed bugs in ``Tournaments.export_games``
         * Deprecated ``Users.get_by_team`` - use ``Teams.get_members`` instead
         
         
         0.6.1 (2020-01-20)
-        ==================
+        ------------------
         
         * Add py37 to the travis build
         * Update development status classifier to 4 - Beta
         * Fix py36 issue preventing successful build
         * Make updates to the Makefile
         
         
         0.6.0 (2020-01-20)
-        ==================
+        ------------------
         
         * Add logging to the ``berserk.session`` module
         * Fix exception message when no cause
         * Fix bug in ``Broadcasts.push_pgn_update``
         * Update documentation and tweak the theme
         
         
         0.5.0 (2020-01-20)
-        ==================
+        ------------------
         
         * Add ``ResponseError`` for 4xx and 5xx responses with status code, reason, and cause
         * Add ``ApiError`` for all other request errors
         * Fix test case broken by 0.4.0 release
         * Put all utils code under test
         
         
         0.4.0 (2020-01-19)
-        ==================
+        ------------------
         
         * Add support for the broadcast endpoints
         * Add a utility for easily converting API objects into update params
         * Fix multiple bugs with the tournament create endpoint
         * Improve the reusability of some conversion utilities
         * Improve many docstrings in the client classes
         
         
         0.3.2 (2020-01-04)
-        ==================
+        ------------------
         
         * Fix bug where options not passed for challenge creation
         * Convert requirements from pinned to sematically compatible
         * Bump all developer dependencies
         * Use pytest instead of the older py.test
         * Use py37 in tox
         
         
         0.3.1 (2018-12-23)
-        ==================
+        ------------------
         
         * Convert datetime string in tournament creation response into datetime object
         
         
         0.3.0 (2018-12-23)
-        ==================
+        ------------------
         
         * Convert all timestamps to datetime in all responses
         * Provide support for challenging other players to a game
         
         
         0.2.1 (2018-12-08)
-        ==================
+        ------------------
         
-        * Bump requests dependency to >=2.20.0 (CVE-2018-18074)
+        * Bump requests dependency to >-2.20.0 (CVE-2018-18074)
         
         
         0.2.0 (2018-12-08)
-        ==================
+        ------------------
         
         * Add `position` and `start_date` params to `Tournament.create`
         * Add `Position` enum
         
         
         0.1.2 (2018-07-14)
-        ==================
+        ------------------
         
         * Fix an asine bug in the docs
         
         
         0.1.1 (2018-07-14)
-        ==================
+        ------------------
         
         * Added tests for session and formats modules
         * Fixed mispelled PgnHandler class (!)
         * Fixed issue with trailing whitespace when splitting multiple PGN texts
         * Fixed the usage overview in the README
         * Fixed the versions for travis-ci
         * Made it easier to test the `JsonHandler` class
         * Salted the bumpversion config to taste
         
         
         0.1.0 (2018-07-10)
-        ==================
+        ------------------
         
         * First release on PyPI.
         
 Keywords: berserk
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `berserk-0.8.0/README.rst` & `berserk-0.9.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 =======
 berserk
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/berserk.svg
         :target: https://pypi.python.org/pypi/berserk
+        :alt: Available on PyPI
 
 .. image:: https://img.shields.io/travis/rhgrant10/berserk.svg
         :target: https://travis-ci.org/rhgrant10/berserk
+        :alt: Continuous Integration
+
+.. image:: https://codecov.io/gh/rhgrant10/berserk/branch/master/graph/badge.svg
+        :target: https://codecov.io/gh/rhgrant10/berserk
+        :alt: Code Coverage
 
 .. image:: https://readthedocs.org/projects/berserk/badge/?version=latest
         :target: https://berserk.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
-Python client for the lichess API
+Python client for the `Lichess API`_.
 
+.. _Lichess API: https://lichess.org/api
 
 * Free software: GNU General Public License v3
 * Documentation: https://berserk.readthedocs.io.
 
 
 Features
 ========
 
 * handles JSON and PGN formats at user's discretion
-* token auth support provided
+* token auth session
 * easy integration with OAuth2
+* automatically converts time values to datetimes
 
 Usage
 =====
 
 You can use any ``requests.Session``-like object as a session, including those
 from ``requests_oauth``. A simple token session is included, as shown below:
 
@@ -41,96 +49,92 @@
     session = berserk.TokenSession(API_TOKEN)
     client = berserk.Client(session=session)
 
 Most if not all of the API is available:
 
 .. code-block:: python
 
-        client.account.get
-        client.account.get_email
-        client.account.get_preferences
-        client.account.get_kid_mode
-        client.account.set_kid_mode
-        client.account.upgrade_to_bot
-
-        client.users.get_puzzle_activity
-        client.users.get_realtime_statuses
-        client.users.get_all_top_10
-        client.users.get_leaderboard
-        client.users.get_public_data
-        client.users.get_activity_feed
-        client.users.get_by_id
-        client.users.get_live_streamers
-        client.users.get_users_followed
-        client.users.get_users_following
-        client.users.get_rating_history
-
-        client.teams.get_members
-        client.teams.join
-        client.teams.leave
-        client.teams.kick_member
-
-        client.games.export
-        client.games.export_by_player
-        client.games.export_multi
-        client.games.get_among_players
-        client.games.get_ongoing
-        client.games.get_tv_channels
-
-        client.challenges.create
-        client.challenges.accept
-        client.challenges.decline
-
-        client.bots.stream_incoming_events
-        client.bots.stream_game_state
-        client.bots.make_move
-        client.bots.post_message
-        client.bots.abort_game
-        client.bots.resign_game
-        client.bots.accept_challenge
-        client.bots.decline_challenge
-
-        client.tournaments.get
-        client.tournaments.create
-        client.tournaments.export_games
-        client.tournaments.stream_results
-        client.tournaments.stream_by_creator
-
-        client.broadcasts.create
-        client.broadcasts.get
-        client.broadcasts.update
-        client.broadcasts.push_pgn_update
+    client.account.get
+    client.account.get_email
+    client.account.get_preferences
+    client.account.get_kid_mode
+    client.account.set_kid_mode
+    client.account.upgrade_to_bot
+
+    client.users.get_puzzle_activity
+    client.users.get_realtime_statuses
+    client.users.get_all_top_10
+    client.users.get_leaderboard
+    client.users.get_public_data
+    client.users.get_activity_feed
+    client.users.get_by_id
+    client.users.get_by_team
+    client.users.get_live_streamers
+    client.users.get_users_followed
+    client.users.get_users_following
+    client.users.get_rating_history
+
+    client.teams.get_members
+    client.teams.join
+    client.teams.leave
+    client.teams.kick_member
+
+    client.games.export
+    client.games.export_by_player
+    client.games.export_multi
+    client.games.get_among_players
+    client.games.get_ongoing
+    client.games.get_tv_channels
+
+    client.challenges.create
+    client.challenges.accept
+    client.challenges.decline
+
+    client.board.stream_incoming_events
+    client.board.seek
+    client.board.stream_game_state
+    client.board.make_move
+    client.board.post_message
+    client.board.abort_game
+    client.board.resign_game
+    client.board.handle_draw_offer
+    client.board.offer_draw
+    client.board.accept_draw
+    client.board.decline_draw
+
+    client.bots.stream_incoming_events
+    client.bots.stream_game_state
+    client.bots.make_move
+    client.bots.post_message
+    client.bots.abort_game
+    client.bots.resign_game
+    client.bots.accept_challenge
+    client.bots.decline_challenge
+
+    client.tournaments.get
+    client.tournaments.create
+    client.tournaments.export_games
+    client.tournaments.stream_results
+    client.tournaments.stream_by_creator
+
+    client.broadcasts.create
+    client.broadcasts.get
+    client.broadcasts.update
+    client.broadcasts.push_pgn_update
 
-        client.simuls.get
+    client.simuls.get
 
-        client.studies.export_chapter
-        client.studies.export
+    client.studies.export_chapter
+    client.studies.export
 
 
 Details for each function can be found in the `full documentation <https://berserk.readthedocs.io>`_.
 
 
 Credits
 =======
 
-Authors
--------
-
-Development Lead
-~~~~~~~~~~~~~~~~
-
-* Robert Grant <rhgrant10@gmail.com>
-
-Contributors
-~~~~~~~~~~~~
-
-* Robert Graham <rpgraham84@gmail.com>
-
-
-Miscellaneous
--------------
-
 This package was created with Cookiecutter_ and the
 `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `berserk-0.8.0/berserk/__init__.py` & `berserk-0.9.0/berserk/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Top-level package for berserk."""
 
 
 __author__ = """Robert Grant"""
 __email__ = 'rhgrant10@gmail.com'
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 
 from .clients import Client  # noqa: F401
 from .session import TokenSession  # noqa: F401
 from .session import Requestor  # noqa: F401
 from .enums import PerfType  # noqa: F401
 from .enums import Variant  # noqa: F401
```

### Comparing `berserk-0.8.0/berserk/clients.py` & `berserk-0.9.0/berserk/clients.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
+from time import time as now
 import requests
 from deprecated import deprecated
 
 from .session import Requestor
-from .formats import JSON, LIJSON, PGN, NDJSON
+from .formats import JSON, LIJSON, PGN, NDJSON, TEXT
 from . import models
 
 
 __all__ = [
     'Client',
     'Account',
     'Board',
@@ -548,14 +549,51 @@
 
         :return: stream of incoming events
         :rtype: iterator over the stream of events
         """
         path = 'api/stream/event'
         yield from self._r.get(path, stream=True)
 
+    def seek(self, time, increment, rated=False, variant='standard',
+             color='random', rating_range=None):
+        """Create a public seek to start a game with a random opponent.
+
+        :param int time: intial clock time in minutes
+        :param int increment: clock increment in minutes
+        :param bool rated: whether the game is rated (impacts ratings)
+        :param str variant: game variant to use
+        :param str color: color to play
+        :param rating_range: range of opponent ratings
+        :return: duration of the seek
+        :rtype: float
+        """
+        if isinstance(rating_range, (list, tuple)):
+            low, high = rating_range
+            rating_range = f'{low}-{high}'
+
+        path = '/api/board/seek'
+        payload = {
+            'rated': str(bool(rated)).lower(),
+            'time': time,
+            'increment': increment,
+            'variant': variant,
+            'color': color,
+            'ratingRange': rating_range or '',
+        }
+
+        # we time the seek
+        start = now()
+
+        # just keep reading to keep the search going
+        for line in self._r.post(path, data=payload, fmt=TEXT, stream=True):
+            pass
+
+        # and return the time elapsed
+        return now() - start
+
     def stream_game_state(self, game_id):
         """Get the stream of events for a board game.
 
         :param str game_id: ID of a game
         :return: iterator over game states
         """
         path = f'api/board/game/stream/{game_id}'
@@ -603,14 +641,61 @@
         :param str game_id: ID of a game
         :return: success
         :rtype: bool
         """
         path = f'api/board/game/{game_id}/resign'
         return self._r.post(path)['ok']
 
+    def handle_draw_offer(self, game_id, accept):
+        """Create, accept, or decline a draw offer.
+
+        To offer a draw, pass ``accept=True`` and a game ID of an in-progress
+        game. To response to a draw offer, pass either ``accept=True`` or
+        ``accept=False`` and the ID of a game in which you have recieved a
+        draw offer.
+
+        Often, it's easier to call :func:`offer_draw`, :func:`accept_draw`, or
+        :func:`decline_draw`.
+
+        :param str game_id: ID of an in-progress game
+        :param bool accept: whether to accept
+        :return: True if successful
+        :rtype: bool
+        """
+        accept = "yes" if accept else "no"
+        path = f'/api/board/game/{game_id}/draw/{accept}'
+        return self._r.post(path)['ok']
+
+    def offer_draw(self, game_id):
+        """Offer a draw in the given game.
+
+        :param str game_id: ID of an in-progress game
+        :return: True if successful
+        :rtype: bool
+        """
+        return self.handle_draw_offer(game_id, True)
+
+    def accept_draw(self, game_id):
+        """Accept an already offered draw in the given game.
+
+        :param str game_id: ID of an in-progress game
+        :return: True if successful
+        :rtype: bool
+        """
+        return self.handle_draw_offer(game_id, True)
+
+    def decline_draw(self, game_id):
+        """Decline an already offered draw in the given game.
+
+        :param str game_id: ID of an in-progress game
+        :return: True if successful
+        :rtype: bool
+        """
+        return self.handle_draw_offer(game_id, False)
+
 
 class Bots(BaseClient):
     """Client for bot-related endpoints."""
 
     def stream_incoming_events(self):
         """Get your realtime stream of incoming events.
```

### Comparing `berserk-0.8.0/berserk/enums.py` & `berserk-0.9.0/berserk/enums.py`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/berserk/exceptions.py` & `berserk-0.9.0/berserk/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """HTTP status text of the response."""
         return self.response.reason
 
     @property
     def cause(self):
         if self._cause is ResponseError.__UNDEFINED:
             try:
-                self._cause = self.response.json()['error']
+                self._cause = self.response.json()
             except Exception:
                 self._cause = None
         return self._cause
 
     @staticmethod
     def _catch_exception(response):
         try:
```

### Comparing `berserk-0.8.0/berserk/formats.py` & `berserk-0.9.0/berserk/formats.py`

 * *Files 11% similar despite different names*

```diff
@@ -126,14 +126,29 @@
                 lines = []
             last_line = decoded_line
 
         if lines:
             yield '\n'.join(lines).strip()
 
 
+class TextHandler(FormatHandler):
+
+    def __init__(self):
+        super().__init__(mime_type='text/plain')
+
+    def parse(self, response):
+        return response.text
+
+    def parse_stream(self, response):
+        yield from response.iter_lines()
+
+
+#: Basic text
+TEXT = TextHandler()
+
 #: Handles vanilla JSON
 JSON = JsonHandler(mime_type='application/json')
 
 #: Handles oddball LiChess JSON (normal JSON, crazy MIME type)
 LIJSON = JsonHandler(mime_type='application/vnd.lichess.v3+json')
 
 #: Handles newline-delimited JSON
```

### Comparing `berserk-0.8.0/berserk/models.py` & `berserk-0.9.0/berserk/models.py`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/berserk/session.py` & `berserk-0.9.0/berserk/session.py`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/berserk/utils.py` & `berserk-0.9.0/berserk/utils.py`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/berserk.egg-info/PKG-INFO` & `berserk-0.9.0/berserk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 Metadata-Version: 2.1
 Name: berserk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for the lichess API
 Home-page: https://github.com/rhgrant10/berserk
 Author: Robert Grant
 Author-email: rhgrant10@gmail.com
 License: GNU General Public License v3
 Description: =======
         berserk
         =======
         
         
         .. image:: https://img.shields.io/pypi/v/berserk.svg
                 :target: https://pypi.python.org/pypi/berserk
+                :alt: Available on PyPI
         
         .. image:: https://img.shields.io/travis/rhgrant10/berserk.svg
                 :target: https://travis-ci.org/rhgrant10/berserk
+                :alt: Continuous Integration
+        
+        .. image:: https://codecov.io/gh/rhgrant10/berserk/branch/master/graph/badge.svg
+                :target: https://codecov.io/gh/rhgrant10/berserk
+                :alt: Code Coverage
         
         .. image:: https://readthedocs.org/projects/berserk/badge/?version=latest
                 :target: https://berserk.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        Python client for the lichess API
+        Python client for the `Lichess API`_.
         
+        .. _Lichess API: https://lichess.org/api
         
         * Free software: GNU General Public License v3
         * Documentation: https://berserk.readthedocs.io.
         
         
         Features
         ========
         
         * handles JSON and PGN formats at user's discretion
-        * token auth support provided
+        * token auth session
         * easy integration with OAuth2
+        * automatically converts time values to datetimes
         
         Usage
         =====
         
         You can use any ``requests.Session``-like object as a session, including those
         from ``requests_oauth``. A simple token session is included, as shown below:
         
@@ -49,220 +57,222 @@
             session = berserk.TokenSession(API_TOKEN)
             client = berserk.Client(session=session)
         
         Most if not all of the API is available:
         
         .. code-block:: python
         
-                client.account.get
-                client.account.get_email
-                client.account.get_preferences
-                client.account.get_kid_mode
-                client.account.set_kid_mode
-                client.account.upgrade_to_bot
-        
-                client.users.get_puzzle_activity
-                client.users.get_realtime_statuses
-                client.users.get_all_top_10
-                client.users.get_leaderboard
-                client.users.get_public_data
-                client.users.get_activity_feed
-                client.users.get_by_id
-                client.users.get_live_streamers
-                client.users.get_users_followed
-                client.users.get_users_following
-                client.users.get_rating_history
-        
-                client.teams.get_members
-                client.teams.join
-                client.teams.leave
-                client.teams.kick_member
-        
-                client.games.export
-                client.games.export_by_player
-                client.games.export_multi
-                client.games.get_among_players
-                client.games.get_ongoing
-                client.games.get_tv_channels
-        
-                client.challenges.create
-                client.challenges.accept
-                client.challenges.decline
-        
-                client.bots.stream_incoming_events
-                client.bots.stream_game_state
-                client.bots.make_move
-                client.bots.post_message
-                client.bots.abort_game
-                client.bots.resign_game
-                client.bots.accept_challenge
-                client.bots.decline_challenge
-        
-                client.tournaments.get
-                client.tournaments.create
-                client.tournaments.export_games
-                client.tournaments.stream_results
-                client.tournaments.stream_by_creator
-        
-                client.broadcasts.create
-                client.broadcasts.get
-                client.broadcasts.update
-                client.broadcasts.push_pgn_update
+            client.account.get
+            client.account.get_email
+            client.account.get_preferences
+            client.account.get_kid_mode
+            client.account.set_kid_mode
+            client.account.upgrade_to_bot
+        
+            client.users.get_puzzle_activity
+            client.users.get_realtime_statuses
+            client.users.get_all_top_10
+            client.users.get_leaderboard
+            client.users.get_public_data
+            client.users.get_activity_feed
+            client.users.get_by_id
+            client.users.get_by_team
+            client.users.get_live_streamers
+            client.users.get_users_followed
+            client.users.get_users_following
+            client.users.get_rating_history
+        
+            client.teams.get_members
+            client.teams.join
+            client.teams.leave
+            client.teams.kick_member
+        
+            client.games.export
+            client.games.export_by_player
+            client.games.export_multi
+            client.games.get_among_players
+            client.games.get_ongoing
+            client.games.get_tv_channels
+        
+            client.challenges.create
+            client.challenges.accept
+            client.challenges.decline
+        
+            client.board.stream_incoming_events
+            client.board.seek
+            client.board.stream_game_state
+            client.board.make_move
+            client.board.post_message
+            client.board.abort_game
+            client.board.resign_game
+            client.board.handle_draw_offer
+            client.board.offer_draw
+            client.board.accept_draw
+            client.board.decline_draw
+        
+            client.bots.stream_incoming_events
+            client.bots.stream_game_state
+            client.bots.make_move
+            client.bots.post_message
+            client.bots.abort_game
+            client.bots.resign_game
+            client.bots.accept_challenge
+            client.bots.decline_challenge
+        
+            client.tournaments.get
+            client.tournaments.create
+            client.tournaments.export_games
+            client.tournaments.stream_results
+            client.tournaments.stream_by_creator
+        
+            client.broadcasts.create
+            client.broadcasts.get
+            client.broadcasts.update
+            client.broadcasts.push_pgn_update
         
-                client.simuls.get
+            client.simuls.get
         
-                client.studies.export_chapter
-                client.studies.export
+            client.studies.export_chapter
+            client.studies.export
         
         
         Details for each function can be found in the `full documentation <https://berserk.readthedocs.io>`_.
         
         
         Credits
         =======
         
-        Authors
-        -------
-        
-        Development Lead
-        ~~~~~~~~~~~~~~~~
-        
-        * Robert Grant <rhgrant10@gmail.com>
-        
-        Contributors
-        ~~~~~~~~~~~~
-        
-        * Robert Graham <rpgraham84@gmail.com>
-        
-        
-        Miscellaneous
-        -------------
-        
         This package was created with Cookiecutter_ and the
         `audreyr/cookiecutter-pypackage`_ project template.
         
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         
-        =======
         History
         =======
         
+        0.9.0 (2020-04-14)
+        ------------------
+        
+        * Add remaining ``Board`` endpoints: seek, handle_draw_offer, offer_draw, accept_draw, and decline_draw
+        * Multiple doc updates/fixes
+        * Add codecov reporting
+        
         0.8.0 (2020-03-08)
-        ==================
+        ------------------
         
         * Add new ``Board`` client: stream_incoming_events, stream_game_state, make_move, post_message, abort_game, and resign_game
         
         0.7.0 (2020-01-26)
-        ==================
+        ------------------
         
         * Add simuls
         * Add studies export and export chapter
         * Add tournament results, games export, and list by creator
         * Add user followers, users following, rating history, and puzzle activity
         * Add new ``Teams`` client: join, get members, kick member, and leave
         * Updated documentation, including new docs for some useful utils
         * Fixed bugs in ``Tournaments.export_games``
         * Deprecated ``Users.get_by_team`` - use ``Teams.get_members`` instead
         
         
         0.6.1 (2020-01-20)
-        ==================
+        ------------------
         
         * Add py37 to the travis build
         * Update development status classifier to 4 - Beta
         * Fix py36 issue preventing successful build
         * Make updates to the Makefile
         
         
         0.6.0 (2020-01-20)
-        ==================
+        ------------------
         
         * Add logging to the ``berserk.session`` module
         * Fix exception message when no cause
         * Fix bug in ``Broadcasts.push_pgn_update``
         * Update documentation and tweak the theme
         
         
         0.5.0 (2020-01-20)
-        ==================
+        ------------------
         
         * Add ``ResponseError`` for 4xx and 5xx responses with status code, reason, and cause
         * Add ``ApiError`` for all other request errors
         * Fix test case broken by 0.4.0 release
         * Put all utils code under test
         
         
         0.4.0 (2020-01-19)
-        ==================
+        ------------------
         
         * Add support for the broadcast endpoints
         * Add a utility for easily converting API objects into update params
         * Fix multiple bugs with the tournament create endpoint
         * Improve the reusability of some conversion utilities
         * Improve many docstrings in the client classes
         
         
         0.3.2 (2020-01-04)
-        ==================
+        ------------------
         
         * Fix bug where options not passed for challenge creation
         * Convert requirements from pinned to sematically compatible
         * Bump all developer dependencies
         * Use pytest instead of the older py.test
         * Use py37 in tox
         
         
         0.3.1 (2018-12-23)
-        ==================
+        ------------------
         
         * Convert datetime string in tournament creation response into datetime object
         
         
         0.3.0 (2018-12-23)
-        ==================
+        ------------------
         
         * Convert all timestamps to datetime in all responses
         * Provide support for challenging other players to a game
         
         
         0.2.1 (2018-12-08)
-        ==================
+        ------------------
         
-        * Bump requests dependency to >=2.20.0 (CVE-2018-18074)
+        * Bump requests dependency to >-2.20.0 (CVE-2018-18074)
         
         
         0.2.0 (2018-12-08)
-        ==================
+        ------------------
         
         * Add `position` and `start_date` params to `Tournament.create`
         * Add `Position` enum
         
         
         0.1.2 (2018-07-14)
-        ==================
+        ------------------
         
         * Fix an asine bug in the docs
         
         
         0.1.1 (2018-07-14)
-        ==================
+        ------------------
         
         * Added tests for session and formats modules
         * Fixed mispelled PgnHandler class (!)
         * Fixed issue with trailing whitespace when splitting multiple PGN texts
         * Fixed the usage overview in the README
         * Fixed the versions for travis-ci
         * Made it easier to test the `JsonHandler` class
         * Salted the bumpversion config to taste
         
         
         0.1.0 (2018-07-10)
-        ==================
+        ------------------
         
         * First release on PyPI.
         
 Keywords: berserk
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `berserk-0.8.0/berserk.egg-info/SOURCES.txt` & `berserk-0.9.0/berserk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/docs/Makefile` & `berserk-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/docs/announcing.rst` & `berserk-0.9.0/docs/announcing.rst`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/docs/api.rst` & `berserk-0.9.0/docs/api.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-API
-===
+Developer Interface
+===================
 
 Clients
 -------
 
 .. automodule:: berserk.clients
     :members:
     :undoc-members:
```

### Comparing `berserk-0.8.0/docs/conf.py` & `berserk-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     # 'logo_only': False,
     'display_version': True,
     # 'prev_next_buttons_location': 'bottom',
     # 'style_external_links': False,
     # 'vcs_pageview_mode': '',
     # 'style_nav_header_background': 'white',
     # # Toc options
-    'collapse_navigation': True,
+    'collapse_navigation': False,
     # 'sticky_navigation': True,
     # 'navigation_depth': 4,
     # 'includehidden': True,
     # 'titles_only': False
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
@@ -181,9 +181,9 @@
      'Miscellaneous'),
 ]
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'http://docs.python.org/3/': None,
-    'http://docs.python-requests.org/en/latest/': None
+    'https://requests.readthedocs.io/en/master/': None
 }
```

### Comparing `berserk-0.8.0/docs/installation.rst` & `berserk-0.9.0/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .. highlight:: shell
 
-============
 Installation
 ============
 
 
 Stable release
 --------------
```

### Comparing `berserk-0.8.0/docs/make.bat` & `berserk-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/docs/usage.rst` & `berserk-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/setup.py` & `berserk-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     keywords='berserk',
     name='berserk',
     packages=find_packages(include=['berserk']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rhgrant10/berserk',
-    version='0.8.0',
+    version='0.9.0',
     zip_safe=True,
 )
```

### Comparing `berserk-0.8.0/tests/test_formats.py` & `berserk-0.9.0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/tests/test_session.py` & `berserk-0.9.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `berserk-0.8.0/tests/test_utils.py` & `berserk-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

