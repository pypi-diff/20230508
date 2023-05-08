# Comparing `tmp/csoundengine-1.9.0.tar.gz` & `tmp/csoundengine-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csoundengine-1.9.0.tar", last modified: Sun Mar  6 23:53:44 2022, max compression
+gzip compressed data, was "csoundengine-1.9.1.tar", last modified: Mon Mar  7 00:02:18 2022, max compression
```

## Comparing `csoundengine-1.9.0.tar` & `csoundengine-1.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.241629 csoundengine-1.9.0/
--rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-1.9.0/LICENSE.txt
--rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-1.9.0/MANIFEST.in
--rw-rw-r--   0 em        (1000) em        (1000)     7289 2022-03-06 23:53:44.241629 csoundengine-1.9.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     5398 2022-02-28 10:54:24.000000 csoundengine-1.9.0/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.213630 csoundengine-1.9.0/csoundengine/
--rw-rw-r--   0 em        (1000) em        (1000)     3953 2022-02-28 23:31:28.000000 csoundengine-1.9.0/csoundengine/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     6464 2022-03-04 16:43:40.000000 csoundengine-1.9.0/csoundengine/config.py
--rwxrwxr-x   0 em        (1000) em        (1000)   100685 2022-03-06 23:34:58.000000 csoundengine-1.9.0/csoundengine/csoundlib.py
--rw-rw-r--   0 em        (1000) em        (1000)    11236 2022-03-01 09:27:40.000000 csoundengine-1.9.0/csoundengine/dependencies.py
--rwxrwxr-x   0 em        (1000) em        (1000)   122493 2022-03-06 23:46:09.000000 csoundengine-1.9.0/csoundengine/engine.py
--rw-rw-r--   0 em        (1000) em        (1000)    19539 2022-03-04 14:03:11.000000 csoundengine-1.9.0/csoundengine/engineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)      106 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/errors.py
--rw-rw-r--   0 em        (1000) em        (1000)    30487 2022-03-06 18:11:17.000000 csoundengine-1.9.0/csoundengine/instr.py
--rw-rw-r--   0 em        (1000) em        (1000)     7513 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/interact.py
--rw-rw-r--   0 em        (1000) em        (1000)     8167 2022-03-03 11:25:53.000000 csoundengine-1.9.0/csoundengine/internalTools.py
--rw-rw-r--   0 em        (1000) em        (1000)     4485 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/jacktools.py
--rw-rw-r--   0 em        (1000) em        (1000)     1047 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/jupytertools.py
--rw-rw-r--   0 em        (1000) em        (1000)     2351 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/linuxaudio.py
--rw-rw-r--   0 em        (1000) em        (1000)     5769 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/magic.py
--rw-rw-r--   0 em        (1000) em        (1000)    32829 2022-03-06 22:54:44.000000 csoundengine-1.9.0/csoundengine/offline.py
--rw-rw-r--   0 em        (1000) em        (1000)     6021 2022-02-22 09:48:28.000000 csoundengine-1.9.0/csoundengine/paramtable.py
--rwxrwxr-x   0 em        (1000) em        (1000)     6994 2022-03-04 17:51:43.000000 csoundengine-1.9.0/csoundengine/plotting.py
--rw-rw-r--   0 em        (1000) em        (1000)    43404 2022-03-06 18:41:17.000000 csoundengine-1.9.0/csoundengine/session.py
--rw-rw-r--   0 em        (1000) em        (1000)     3003 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/sessioninstrs.py
--rw-rw-r--   0 em        (1000) em        (1000)     1589 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/state.py
--rw-rw-r--   0 em        (1000) em        (1000)    30596 2022-03-06 23:11:01.000000 csoundengine-1.9.0/csoundengine/synth.py
--rw-rw-r--   0 em        (1000) em        (1000)     4482 2022-03-06 22:33:39.000000 csoundengine-1.9.0/csoundengine/tableproxy.py
--rw-rw-r--   0 em        (1000) em        (1000)      306 2022-03-04 15:37:02.000000 csoundengine-1.9.0/csoundengine/termui.py
--rw-rw-r--   0 em        (1000) em        (1000)     1630 2021-11-13 21:37:59.000000 csoundengine-1.9.0/csoundengine/tools.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.215629 csoundengine-1.9.0/csoundengine.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     7289 2022-03-06 23:53:44.000000 csoundengine-1.9.0/csoundengine.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     1541 2022-03-06 23:53:44.000000 csoundengine-1.9.0/csoundengine.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-03-06 23:53:44.000000 csoundengine-1.9.0/csoundengine.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-1.9.0/csoundengine.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      199 2022-03-06 23:53:44.000000 csoundengine-1.9.0/csoundengine.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2022-03-06 23:53:44.000000 csoundengine-1.9.0/csoundengine.egg-info/top_level.txt
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.205630 csoundengine-1.9.0/data/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.206630 csoundengine-1.9.0/data/plugins/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.223629 csoundengine-1.9.0/data/plugins/linux/
--rw-rw-r--   0 em        (1000) em        (1000)    31328 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   104096 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108688 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31392 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2022-02-23 23:23:30.000000 csoundengine-1.9.0/data/plugins/linux/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.234629 csoundengine-1.9.0/data/plugins/macos/
--rw-rw-r--   0 em        (1000) em        (1000)    66496 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   104744 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103640 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    66816 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2022-02-23 23:23:31.000000 csoundengine-1.9.0/data/plugins/macos/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-06 23:53:44.240629 csoundengine-1.9.0/data/plugins/windows/
--rw-rw-r--   0 em        (1000) em        (1000)    45056 2022-02-23 23:23:32.000000 csoundengine-1.9.0/data/plugins/windows/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    71168 2022-02-23 23:23:32.000000 csoundengine-1.9.0/data/plugins/windows/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2022-02-23 23:23:32.000000 csoundengine-1.9.0/data/plugins/windows/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2022-02-23 23:23:32.000000 csoundengine-1.9.0/data/plugins/windows/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    23552 2022-02-23 23:23:32.000000 csoundengine-1.9.0/data/plugins/windows/poly.dll
--rw-rw-r--   0 em        (1000) em        (1000)       38 2022-03-06 23:53:44.241629 csoundengine-1.9.0/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     1350 2022-03-06 23:53:35.000000 csoundengine-1.9.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.545212 csoundengine-1.9.1/
+-rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-1.9.1/LICENSE.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-1.9.1/MANIFEST.in
+-rw-rw-r--   0 em        (1000) em        (1000)     7289 2022-03-07 00:02:18.544212 csoundengine-1.9.1/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5398 2022-02-28 10:54:24.000000 csoundengine-1.9.1/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.534213 csoundengine-1.9.1/csoundengine/
+-rw-rw-r--   0 em        (1000) em        (1000)     3953 2022-02-28 23:31:28.000000 csoundengine-1.9.1/csoundengine/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6464 2022-03-04 16:43:40.000000 csoundengine-1.9.1/csoundengine/config.py
+-rwxrwxr-x   0 em        (1000) em        (1000)   100685 2022-03-06 23:34:58.000000 csoundengine-1.9.1/csoundengine/csoundlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)    11236 2022-03-01 09:27:40.000000 csoundengine-1.9.1/csoundengine/dependencies.py
+-rwxrwxr-x   0 em        (1000) em        (1000)   122493 2022-03-06 23:46:09.000000 csoundengine-1.9.1/csoundengine/engine.py
+-rw-rw-r--   0 em        (1000) em        (1000)    19539 2022-03-04 14:03:11.000000 csoundengine-1.9.1/csoundengine/engineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)      106 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/errors.py
+-rw-rw-r--   0 em        (1000) em        (1000)    30487 2022-03-06 18:11:17.000000 csoundengine-1.9.1/csoundengine/instr.py
+-rw-rw-r--   0 em        (1000) em        (1000)     7513 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/interact.py
+-rw-rw-r--   0 em        (1000) em        (1000)     8167 2022-03-03 11:25:53.000000 csoundengine-1.9.1/csoundengine/internalTools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4485 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/jacktools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1047 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/jupytertools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2351 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/linuxaudio.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5769 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/magic.py
+-rw-rw-r--   0 em        (1000) em        (1000)    32829 2022-03-06 22:54:44.000000 csoundengine-1.9.1/csoundengine/offline.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6021 2022-02-22 09:48:28.000000 csoundengine-1.9.1/csoundengine/paramtable.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     6994 2022-03-04 17:51:43.000000 csoundengine-1.9.1/csoundengine/plotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)    43404 2022-03-06 18:41:17.000000 csoundengine-1.9.1/csoundengine/session.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3003 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/sessioninstrs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1589 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/state.py
+-rw-rw-r--   0 em        (1000) em        (1000)    30596 2022-03-06 23:11:01.000000 csoundengine-1.9.1/csoundengine/synth.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4482 2022-03-06 22:33:39.000000 csoundengine-1.9.1/csoundengine/tableproxy.py
+-rw-rw-r--   0 em        (1000) em        (1000)      306 2022-03-04 15:37:02.000000 csoundengine-1.9.1/csoundengine/termui.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1630 2021-11-13 21:37:59.000000 csoundengine-1.9.1/csoundengine/tools.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.535213 csoundengine-1.9.1/csoundengine.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     7289 2022-03-07 00:02:18.000000 csoundengine-1.9.1/csoundengine.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     1541 2022-03-07 00:02:18.000000 csoundengine-1.9.1/csoundengine.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-03-07 00:02:18.000000 csoundengine-1.9.1/csoundengine.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-1.9.1/csoundengine.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      199 2022-03-07 00:02:18.000000 csoundengine-1.9.1/csoundengine.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2022-03-07 00:02:18.000000 csoundengine-1.9.1/csoundengine.egg-info/top_level.txt
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.529213 csoundengine-1.9.1/data/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.530213 csoundengine-1.9.1/data/plugins/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.539213 csoundengine-1.9.1/data/plugins/linux/
+-rw-rw-r--   0 em        (1000) em        (1000)    31328 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   104096 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108688 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31392 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2022-02-23 23:23:30.000000 csoundengine-1.9.1/data/plugins/linux/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.542213 csoundengine-1.9.1/data/plugins/macos/
+-rw-rw-r--   0 em        (1000) em        (1000)    66496 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   104744 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103640 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    66816 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2022-02-23 23:23:31.000000 csoundengine-1.9.1/data/plugins/macos/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-03-07 00:02:18.544212 csoundengine-1.9.1/data/plugins/windows/
+-rw-rw-r--   0 em        (1000) em        (1000)    45056 2022-02-23 23:23:32.000000 csoundengine-1.9.1/data/plugins/windows/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    71168 2022-02-23 23:23:32.000000 csoundengine-1.9.1/data/plugins/windows/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2022-02-23 23:23:32.000000 csoundengine-1.9.1/data/plugins/windows/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2022-02-23 23:23:32.000000 csoundengine-1.9.1/data/plugins/windows/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    23552 2022-02-23 23:23:32.000000 csoundengine-1.9.1/data/plugins/windows/poly.dll
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2022-03-07 00:02:18.545212 csoundengine-1.9.1/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)     1350 2022-03-07 00:02:15.000000 csoundengine-1.9.1/setup.py
```

### Comparing `csoundengine-1.9.0/LICENSE.txt` & `csoundengine-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/PKG-INFO` & `csoundengine-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: csoundengine
-Version: 1.9.0
+Version: 1.9.1
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Description: csoundengine
         ============
```

### Comparing `csoundengine-1.9.0/README.rst` & `csoundengine-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/__init__.py` & `csoundengine-1.9.1/csoundengine/__init__.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/config.py` & `csoundengine-1.9.1/csoundengine/config.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/csoundlib.py` & `csoundengine-1.9.1/csoundengine/csoundlib.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/dependencies.py` & `csoundengine-1.9.1/csoundengine/dependencies.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/engine.py` & `csoundengine-1.9.1/csoundengine/engine.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/engineorc.py` & `csoundengine-1.9.1/csoundengine/engineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/instr.py` & `csoundengine-1.9.1/csoundengine/instr.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/interact.py` & `csoundengine-1.9.1/csoundengine/interact.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/internalTools.py` & `csoundengine-1.9.1/csoundengine/internalTools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/jacktools.py` & `csoundengine-1.9.1/csoundengine/jacktools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/jupytertools.py` & `csoundengine-1.9.1/csoundengine/jupytertools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/linuxaudio.py` & `csoundengine-1.9.1/csoundengine/linuxaudio.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/magic.py` & `csoundengine-1.9.1/csoundengine/magic.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/offline.py` & `csoundengine-1.9.1/csoundengine/offline.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/paramtable.py` & `csoundengine-1.9.1/csoundengine/paramtable.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/plotting.py` & `csoundengine-1.9.1/csoundengine/plotting.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/session.py` & `csoundengine-1.9.1/csoundengine/session.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/sessioninstrs.py` & `csoundengine-1.9.1/csoundengine/sessioninstrs.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/state.py` & `csoundengine-1.9.1/csoundengine/state.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/synth.py` & `csoundengine-1.9.1/csoundengine/synth.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/tableproxy.py` & `csoundengine-1.9.1/csoundengine/tableproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine/tools.py` & `csoundengine-1.9.1/csoundengine/tools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/csoundengine.egg-info/PKG-INFO` & `csoundengine-1.9.1/csoundengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: csoundengine
-Version: 1.9.0
+Version: 1.9.1
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Description: csoundengine
         ============
```

### Comparing `csoundengine-1.9.0/csoundengine.egg-info/SOURCES.txt` & `csoundengine-1.9.1/csoundengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libbeosc.so` & `csoundengine-1.9.1/data/plugins/linux/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libelse.so` & `csoundengine-1.9.1/data/plugins/linux/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libjsfx.so` & `csoundengine-1.9.1/data/plugins/linux/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libklib.so` & `csoundengine-1.9.1/data/plugins/linux/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libpathtools.so` & `csoundengine-1.9.1/data/plugins/linux/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libpoly.so` & `csoundengine-1.9.1/data/plugins/linux/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/librisset.so` & `csoundengine-1.9.1/data/plugins/linux/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/linux/libsndmeta.so` & `csoundengine-1.9.1/data/plugins/linux/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libbeosc.dylib` & `csoundengine-1.9.1/data/plugins/macos/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libelse.dylib` & `csoundengine-1.9.1/data/plugins/macos/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libjsfx.dylib` & `csoundengine-1.9.1/data/plugins/macos/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libklib.dylib` & `csoundengine-1.9.1/data/plugins/macos/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libpathtools.dylib` & `csoundengine-1.9.1/data/plugins/macos/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libpoly.dylib` & `csoundengine-1.9.1/data/plugins/macos/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/librisset.dylib` & `csoundengine-1.9.1/data/plugins/macos/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/macos/libsndmeta.dylib` & `csoundengine-1.9.1/data/plugins/macos/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/windows/beosc.dll` & `csoundengine-1.9.1/data/plugins/windows/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/windows/else.dll` & `csoundengine-1.9.1/data/plugins/windows/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/windows/klib.dll` & `csoundengine-1.9.1/data/plugins/windows/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/windows/pathtools.dll` & `csoundengine-1.9.1/data/plugins/windows/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/data/plugins/windows/poly.dll` & `csoundengine-1.9.1/data/plugins/windows/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-1.9.0/setup.py` & `csoundengine-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
-version = (1, 9, 0)
+version = (1, 9, 1)
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 
@@ -26,15 +26,15 @@
     install_requires=[
         "numpy",
         "scipy",
         "matplotlib",
         "JACK-client",
         "ctcsound",
         "sndfileio>=1.8.1",
-        "emlib>=1.3.1",
+        "emlib>=1.3.3",
         "cachetools",
         "configdict>=0.8",
         "bpf4",
         "numpyx>=0.5",
         "pitchtools>=1.1",
         "appdirs",
         "pygments",
```

