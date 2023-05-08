# Comparing `tmp/Subsearch-2.33.5.tar.gz` & `tmp/Subsearch-2.34.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.33.5.tar", last modified: Mon Apr 24 21:54:43 2023, max compression
+gzip compressed data, was "Subsearch-2.34.0rc1.tar", last modified: Mon May  8 15:46:32 2023, max compression
```

## Comparing `Subsearch-2.33.5.tar` & `Subsearch-2.34.0rc1.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 21:54:26.000000 Subsearch-2.33.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 21:54:26.000000 Subsearch-2.33.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-24 21:54:43.453870 Subsearch-2.33.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-24 21:54:26.000000 Subsearch-2.33.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 21:54:26.000000 Subsearch-2.33.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:54:43.453870 Subsearch-2.33.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-24 21:54:26.000000 Subsearch-2.33.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.441870 Subsearch-2.33.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/application_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/set_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.844054 Subsearch-2.34.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.848054 Subsearch-2.34.0rc1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.848054 Subsearch-2.34.0rc1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/application_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/subsearch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_trough_hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_trough_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/language_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/language_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/language_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/ttk_style.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/settings_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tkinter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/updates.py
```

### Comparing `Subsearch-2.33.5/LICENSE` & `Subsearch-2.34.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/PKG-INFO` & `Subsearch-2.34.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.33.5
+Version: 2.34.0rc1
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.33.5/README.md` & `Subsearch-2.34.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/pyproject.toml` & `Subsearch-2.34.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop"
 ]
-dependencies = ["selectolax==0.3.12", "cloudscraper==1.2.69", "num2words==0.5.12", "packaging==23.1", "requests==2.28.2"]
+dependencies = ["selectolax==0.3.13", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.30.0"]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/vagabondHustler/subsearch"
 
 [project.scripts]
 subsearch = "subsearch:main"
@@ -41,15 +41,15 @@
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
 optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.14.9", "mypy==1.2.0", "pipreqs==0.4.13"]
-dev = ["pytest==7.3.1", "pytest-cov==4.0.0", "tox==4.4.12"]
+dev = ["pytest==7.3.1", "pytest-cov==4.0.0", "tox==4.5.1"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
 log_cli = true
```

### Comparing `Subsearch-2.33.5/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.34.0rc1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.33.5
+Version: 2.34.0rc1
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.33.5/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.34.0rc1/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/Subsearch.egg-info/top_level.txt
 src/subsearch/__init__.py
 src/subsearch/__main__.py
 src/subsearch/core.py
 src/subsearch/data/__init__.py
 src/subsearch/data/application_config.json
 src/subsearch/data/data_objects.py
+src/subsearch/data/guid.py
 src/subsearch/data/languages.json
 src/subsearch/data/set_data.py
 src/subsearch/data/version.py
 src/subsearch/gui/__init__.py
 src/subsearch/gui/tab_manager.py
 src/subsearch/gui/tkinter_utils.py
 src/subsearch/gui/assets/dark.tcl
@@ -85,9 +86,10 @@
 src/subsearch/utils/__init__.py
 src/subsearch/utils/exceptions.py
 src/subsearch/utils/file_manager.py
 src/subsearch/utils/imdb_lookup.py
 src/subsearch/utils/io_json.py
 src/subsearch/utils/io_winreg.py
 src/subsearch/utils/log.py
+src/subsearch/utils/mutex_synchronizer.py
 src/subsearch/utils/string_parser.py
 src/subsearch/utils/updates.py
```

### Comparing `Subsearch-2.33.5/src/subsearch/__init__.py` & `Subsearch-2.34.0rc1/src/subsearch/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,153 @@
-import sys
-from pathlib import Path
-from threading import Thread
-
-from subsearch import core
-from subsearch.gui import tab_manager
-from subsearch.utils import io_json, io_winreg
-
-PACKAGEPATH = Path(__file__).resolve().parent.as_posix()
-HOMEPATH = Path(PACKAGEPATH).parent.as_posix()
-sys.path.append(HOMEPATH)
-sys.path.append(PACKAGEPATH)
-
-
-class Subsearch(core.AppSteps):
-    def __init__(self) -> None:
-        """
-        Setup and gather all available parameters
-        """
-        core.AppSteps.__init__(self)
-
-    def thread_executor(self, *args) -> None:
-        """
-        Search for subtitles with active providers concurrently.
-        """
-        provider_threads = {}
-        for provider in args:
-            provider_threads[provider] = Thread(target=provider)
-
-        for thread in provider_threads.values():
-            thread.start()
-
-        for thread in provider_threads.values():
-            thread.join()
-
-    def search_for_subtitles(self) -> None:
-        """
-        Runs a search with all active providers, either concurrently or separately.
-        """
-        if io_json.get_json_key("use_threading"):
-            self.thread_executor(
-                self._provider_subscene,
-                self._provider_opensubtitles,
-                self._provider_yifysubtitles,
-            )
-        else:
-            self._provider_subscene()
-            self._provider_opensubtitles()
-            self._provider_yifysubtitles()
-
-    def provider_opensubtitles(self) -> None:
-        """
-        Search for subtitles on opensubtitles
-        """
-        self._provider_opensubtitles()
-
-    def provider_subscene(self) -> None:
-        """
-        Search for subtitles on subscene
-        """
-        self._provider_subscene()
-
-    def provider_yifysubtitles(self) -> None:
-        """
-        Search for subtitles on yifysubtitles
-        """
-        self._provider_yifysubtitles()
-
-    def process_files(self) -> None:
-        """
-        Download zip files containing the .srt files, extract, rename and clean up tmp files
-        """
-        self._download_files()
-        self._not_downloaded()
-        self._extract_zip_files()
-        self._clean_up()
-
-    def pre_exit(self) -> None:
-        """
-        Stop pref counter, log elapsed time and keep the terminal open if show_terminal is True
-        """
-        self._pre_exit()
-
-
-def console() -> None:
-    r"""
-    Usages: subsearch [OPTIONS]
-
-    Options:
-        --settings [lang, search, app, dl]      Open the GUI settings menu
-                                                    ang: opens tab with available languages
-                                                    search: opens tab with settings such as available providers
-                                                    app: opens tab with app settings
-                                                    dl: opens tab for subtitles not downloaded
-
-        --registry-key [add, del]               Edit the registry
-                                                    add: adds the context menu  / replaces the context menu with default values
-                                                    del: deletes the context menu
-                                                    e.g: subsearch --registry-key add
-
-        --help                                  Prints usage information
-    """
-
-    for num, arg in enumerate(sys.argv[1:], 1):
-        if arg.startswith("--settings"):
-            if sys.argv[num + 1] == "lang":
-                sys.argv.pop(num), sys.argv.pop(num)  # pop arguments
-                tab_manager.open_tab("language")
-            elif sys.argv[num + 1] == "search":
-                sys.argv.pop(num), sys.argv.pop(num)  # pop arguments
-                tab_manager.open_tab("search")
-            elif sys.argv[num + 1] == "app":
-                sys.argv.pop(num), sys.argv.pop(num)  # pop arguments
-                tab_manager.open_tab("settings")
-            elif sys.argv[num + 1] == "dl":
-                sys.argv.pop(num), sys.argv.pop(num)  # pop arguments
-                tab_manager.open_tab("download")
-
-            break
-        elif arg.startswith("--registry-key") or arg.startswith("--add-key"):
-            if sys.argv[num + 1] == "add":
-                sys.argv.pop(num), sys.argv.pop(num)  # pop arguments
-                io_winreg.add_context_menu()
-                break
-            elif sys.argv[num + 1] == "del":
-                sys.argv.pop(num), sys.argv.pop(num)  # pop arguments
-                io_winreg.remove_context_menu()
-                break
-        elif arg.startswith("--help"):
-            sys.argv.pop(num)  # pop argument
-            print(console.__doc__)
-            break
-        elif len(sys.argv[1:]) == num:
-            print("Invalid argument")
-            print(console.__doc__)
-
-
-def main() -> None:
-    for i in sys.argv:
-        if i.startswith("--"):
-            console()
-            return None
-
-    app = Subsearch()
-    app.search_for_subtitles()
-    app.process_files()
-    app.pre_exit()
-
-
-if __name__ == "__main__":
-    main()
+import sys
+from pathlib import Path
+from threading import Thread
+
+from subsearch import core
+from subsearch.data import __guid__
+from subsearch.gui import tab_manager
+from subsearch.utils import io_json, io_winreg, mutex_synchronizer
+
+PACKAGEPATH = Path(__file__).resolve().parent.as_posix()
+HOMEPATH = Path(PACKAGEPATH).parent.as_posix()
+sys.path.append(HOMEPATH)
+sys.path.append(PACKAGEPATH)
+
+
+class Subsearch(core.AppSteps):
+    def __init__(self) -> None:
+        """
+        Setup and gather all available parameters
+        """
+        core.AppSteps.__init__(self)
+
+    def thread_executor(self, *args) -> None:
+        """
+        Search for subtitles with active providers concurrently.
+        """
+        provider_threads = {}
+        for provider in args:
+            provider_threads[provider] = Thread(target=provider)
+
+        for thread in provider_threads.values():
+            thread.start()
+
+        for thread in provider_threads.values():
+            thread.join()
+
+    def search_for_subtitles(self) -> None:
+        """
+        Runs a search with all active providers, either concurrently or separately.
+        """
+        if io_json.get_json_key("use_threading"):
+            self.thread_executor(
+                self._provider_subscene,
+                self._provider_opensubtitles,
+                self._provider_yifysubtitles,
+            )
+        else:
+            self._provider_subscene()
+            self._provider_opensubtitles()
+            self._provider_yifysubtitles()
+
+    def provider_opensubtitles(self) -> None:
+        """
+        Search for subtitles on opensubtitles
+        """
+        self._provider_opensubtitles()
+
+    def provider_subscene(self) -> None:
+        """
+        Search for subtitles on subscene
+        """
+        self._provider_subscene()
+
+    def provider_yifysubtitles(self) -> None:
+        """
+        Search for subtitles on yifysubtitles
+        """
+        self._provider_yifysubtitles()
+
+    def process_files(self) -> None:
+        """
+        Download zip files containing the .srt files, extract, rename and clean up tmp files
+        """
+        self._download_files()
+        self._not_downloaded()
+        self._extract_zip_files()
+        self._clean_up()
+
+    def pre_exit(self) -> None:
+        """
+        Stop pref counter, log elapsed time and keep the terminal open if show_terminal is True
+        """
+        self._pre_exit()
+
+
+def console() -> None:
+    r"""
+    Usages: subsearch [OPTIONS]
+
+    Options:
+        --settings [lang, search, app, dl]      Open the GUI settings menu
+                                                    ang: opens tab with available languages
+                                                    search: opens tab with settings such as available providers
+                                                    app: opens tab with app settings
+                                                    dl: opens tab for subtitles not downloaded
+
+        --registry-key [add, del]               Edit the registry
+                                                    add: adds the context menu  / replaces the context menu with default values
+                                                    del: deletes the context menu
+                                                    e.g: subsearch --registry-key add
+
+        --help                                  Prints usage information
+    """
+
+    for num, arg in enumerate(sys.argv[1:], 1):
+        if arg.startswith("--settings"):
+            if sys.argv[num + 1] == "lang":
+                sys.argv.pop(num), sys.argv.pop(num)
+                tab_manager.open_tab("language")
+            elif sys.argv[num + 1] == "search":
+                sys.argv.pop(num), sys.argv.pop(num)
+                tab_manager.open_tab("search")
+            elif sys.argv[num + 1] == "app":
+                sys.argv.pop(num), sys.argv.pop(num)
+                tab_manager.open_tab("settings")
+            elif sys.argv[num + 1] == "dl":
+                sys.argv.pop(num), sys.argv.pop(num)
+                tab_manager.open_tab("download")
+
+            break
+        elif arg.startswith("--registry-key") or arg.startswith("--add-key"):
+            if sys.argv[num + 1] == "add":
+                sys.argv.pop(num), sys.argv.pop(num)
+                io_winreg.add_context_menu()
+                break
+            elif sys.argv[num + 1] == "del":
+                sys.argv.pop(num), sys.argv.pop(num)
+                io_winreg.remove_context_menu()
+                break
+        elif arg.startswith("--help"):
+            sys.argv.pop(num)  # pop argument
+            print(console.__doc__)
+            break
+        elif len(sys.argv[1:]) == num:
+            print("Invalid argument")
+            print(console.__doc__)
+
+
+@mutex_synchronizer.synchronized(__guid__)
+def main() -> None:
+    for i in sys.argv:
+        if i.startswith("--"):
+            console()
+            return None
+
+    app = Subsearch()
+    app.search_for_subtitles()
+    app.process_files()
+    app.pre_exit()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `Subsearch-2.33.5/src/subsearch/core.py` & `Subsearch-2.34.0rc1/src/subsearch/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self) -> None:
         self.app_config = io_json.get_app_config()
         if video_data is not None:
             self.file_exist = True
             self.file_hash = file_manager.get_hash(video_data.file_path)
         else:
             self.file_exist = False
-            self.file_hash = "000000000000000000"
+            self.file_hash = ""
         self.results: dict[str, list[DownloadMetaData]] = {}
         self.skipped_downloads: dict[str, list[FormattedMetadata]] = {}
         self.skipped_combined: list[FormattedMetadata] = []
         self.downloads: dict[str, int] = {}
         self.language_data = io_json.get_language_data()
 
         for provider in self.app_config.providers.keys():
@@ -82,15 +82,15 @@
         log.output_header("Search started")
 
     def _provider_opensubtitles(self) -> None:
         if self.skip_step.opensubtitles():
             return None
         # log.output_header("Searching on opensubtitles")
         _opensubs = opensubtitles.OpenSubtitles(**self.search_kwargs)
-        if self.app_config.providers["opensubtitles_hash"] and self.file_hash != "000000000000000000":
+        if self.app_config.providers["opensubtitles_hash"] and self.file_hash != "":
             self.results["opensubtitles_hash"] = _opensubs.parse_hash_results()
         if self.app_config.providers["opensubtitles_site"]:
             self.results["opensubtitles_site"] = _opensubs.parse_site_results()
         self.skipped_downloads["opensubtitles_site"] = _opensubs._sorted_list()
 
     def _provider_subscene(self) -> None:
         if self.skip_step.subscene():
```

### Comparing `Subsearch-2.33.5/src/subsearch/data/application_config.json` & `Subsearch-2.34.0rc1/src/subsearch/data/application_config.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'multiple_app_instances'": 'False'}*

```diff
@@ -17,14 +17,15 @@
         ".swf": true,
         ".vob": true,
         ".wmv": true
     },
     "log_to_file": false,
     "manual_download_fail": true,
     "manual_download_mode": false,
+    "multiple_app_instances": false,
     "percentage_threshold": 90,
     "providers": {
         "opensubtitles_hash": true,
         "opensubtitles_site": true,
         "subscene_site": true,
         "yifysubtitles_site": true
     },
```

### Comparing `Subsearch-2.33.5/src/subsearch/data/data_objects.py` & `Subsearch-2.34.0rc1/src/subsearch/data/data_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     rename_best_match: bool
     context_menu: bool
     context_menu_icon: bool
     manual_download_fail: bool
     manual_download_mode: bool
     show_terminal: bool
     use_threading: bool
+    multiple_app_instances: bool
     log_to_file: bool
     file_extensions: dict[str, bool]
     providers: dict[str, bool]
     hearing_impaired: bool
     non_hearing_impaired: bool
```

### Comparing `Subsearch-2.33.5/src/subsearch/data/languages.json` & `Subsearch-2.34.0rc1/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/data/set_data.py` & `Subsearch-2.34.0rc1/src/subsearch/data/set_data.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/__init__.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/dark.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_disabled.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_hover.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_pressed.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_rest.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_hover.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_press.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_rest.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_hover.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_press.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_rest.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_hover.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_press.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_rest.png` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.34.0rc1/src/subsearch/gui/assets/ttk_style.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/tab_manager.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/tab_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         self.configure(bg=GUI_DATA.colors.dark_grey)
         settings_tab.FileExtensions(self).pack(anchor="center")
         tk.Frame(self, height=80, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
         settings_tab.ShowContextMenu(self).pack(anchor="center")
         settings_tab.ShowContextMenuIcon(self).pack(anchor="center")
         settings_tab.ShowDownloadWindow(self).pack(anchor="center")
         settings_tab.UseThreading(self).pack(anchor="center")
+        settings_tab.MultipleAppInstances(self).pack(anchor="center")
         settings_tab.LogToFile(self).pack(anchor="center")
         if file_manager.running_from_exe() is False:
             settings_tab.ShowTerminalOnSearch(self).pack(anchor="center")
         tk.Frame(self, height=20, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
         settings_tab.CheckForUpdates(self).pack(anchor="center")
```

### Comparing `Subsearch-2.33.5/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/language_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/search_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/settings_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,25 @@
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
         tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Use threading", "use_threading")
 
 
+class MultipleAppInstances(tkinter_utils.ToggleableFrameButton):
+    """
+    Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
+
+    Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
+    """
+
+    def __init__(self, parent) -> None:
+        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Multiple app instances", "multiple_app_instances")
+
+
 class CheckForUpdates(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
         self.string_var = tk.StringVar()
         self.string_var.set(f"")
         label = tk.Label(self, text=f"Version {__version__}")
```

### Comparing `Subsearch-2.33.5/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.34.0rc1/src/subsearch/gui/tkinter_utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/providers/generic.py` & `Subsearch-2.34.0rc1/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.34.0rc1/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/providers/subscene.py` & `Subsearch-2.34.0rc1/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.34.0rc1/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/utils/file_manager.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/file_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import shutil
 import struct
 import sys
 import zipfile
 from pathlib import Path
 
 from subsearch.data import video_data
@@ -53,21 +52,20 @@
         src (Path): Source path to extract files
         dst (Path): Destination path to extract files
         extension (str): Extension of files to be extracted
 
     Returns:
         None.
     """
-    for file in os.listdir(src):
-        if file.endswith(extension):
-            log.output(f"Extracting: {file} -> ..\\subs\\{file}")
-            filename = Path(src) / file
-            zip_ref = zipfile.ZipFile(filename)
-            zip_ref.extractall(dst)
-            zip_ref.close()
+    for file in Path(src).glob(f"*{extension}"):
+        filename = Path(src) / file
+        log.path_action("extract", file, dst)
+        zip_ref = zipfile.ZipFile(filename)
+        zip_ref.extractall(dst)
+        zip_ref.close()
 
 
 def rename_best_match(release_name: str, cwd: Path, extension: str) -> None:
     """
     Function renames and moves the best matching subtitle file, based on the release name, to the specified path. If no match is found nothing happens.
 
     Args:
@@ -76,70 +74,68 @@
         extension (str): The file type of the subtitles i.e ".srt".
 
     Returns:
         None.
     """
     if video_data is None:
         return None
-    higest_value = (0, "")
-    for file in os.listdir(video_data.subs_directory):
-        if file.endswith(extension):
-            value = string_parser.calculate_match(file, release_name)
-            if value >= higest_value[0]:
-                higest_value = value, file
-
-    file_to_rename = higest_value[1]
-    if file_to_rename.endswith(extension):
-        old_name_src = Path(video_data.subs_directory) / file_to_rename
-        new_name_dst = Path(video_data.subs_directory) / release_name
-        log.output(f"Renaming: {file_to_rename } -> {release_name}")
-        os.rename(old_name_src, new_name_dst)
-        move_src = new_name_dst
-        move_dst = Path(cwd) / release_name
-        log.output(f"Moving: {release_name} -> {cwd}")
-        shutil.move(move_src, move_dst)
+    best_match = (0, "")
+    for file in Path(video_data.subs_directory).glob(f"*{extension}"):
+        value = string_parser.calculate_match(file.name, release_name)
+        if value >= best_match[0]:
+            best_match = value, file
+    if not best_match[1]:
+        return None
+    file_to_rename = best_match[1]
+    old_name_src = Path(video_data.subs_directory) / file_to_rename
+    new_name_dst = Path(video_data.subs_directory) / release_name
+    log.path_action("rename", file_to_rename, new_name_dst)
+    old_name_src.rename(new_name_dst)
+    move_src = new_name_dst
+    move_dst = Path(cwd) / release_name
+    log.path_action("move", move_src, cwd)
+    if move_dst.exists():
+        move_dst.unlink()
+    shutil.move(move_src, move_dst)
 
 
 def clean_up_files(cwd: Path, extension: str) -> None:
     """
     Removes files with specific extensions in a given directory
 
     Args:
         cwd (pathlib.Path): The directory path where the files to be deleted reside.
         extension (str): The file extension of the files to be deleted.
 
     Returns:
         None
     """
 
-    for file in os.listdir(cwd):
-        if file.endswith(extension):
-            log.output(f"Removing: {file}")
-            file_path = Path(cwd) / file
-            file_path.unlink()
+    for file in Path(cwd).glob(f"*{extension}"):
+        log.path_action("remove", file)
+        file_path = Path(cwd) / file
+        file_path.unlink()
 
 
 def del_directory(directory: Path) -> None:
     """
     Remove a directory and its contents.
 
     Args:
         directory: A Path object representing the directory to be removed.
 
     Returns:
         None
     """
-    for file in os.listdir(directory):
-        log.output(f"Removing: {file}")
-    log.output(f"Removing: {directory}")
+    log.path_action("remove", directory)
     shutil.rmtree(directory)
 
 
 def directory_is_empty(directory: Path) -> bool:
-    if len(os.listdir(directory)) == 0:
+    if not any(directory.iterdir()):
         return True
     return False
 
 
 def make_necessary_directories() -> None:
     """
     Make necessary directories using video object info.
@@ -161,27 +157,28 @@
         file_path: A Path object indicating the location of the input file. If None, returns an all-zero string.
 
     Returns:
         A hexadecimal String indicating the unique hash value of the file. If the file cannot be read or its size is less than 131072 bytes, returns an all-zero string '000000000000000000'.
 
     Examples:
         get_hash(Path("my_folder/my_file.jpg")) returns "d020f52c464caedd"
-        get_hash(None) returns "000000000000000000"
+        get_hash(None) returns ""
     """
     if file_path is None:
-        return "000000000000000000"
+        return ""
     try:
         longlongformat = "<q"  # little-endian long long
         bytesize = struct.calcsize(longlongformat)
         with open(file_path, "rb") as f:
-            filesize = os.path.getsize(file_path)
+            # filesize = os.path.getsize(file_path)
+            filesize = file_path.stat().st_size
             hash = filesize
             if filesize < 65536 * 2:
                 log.output(f"SizeError: filesize is {filesize} bytes", False)
-                return "000000000000000000"
+                return ""
             n1 = 65536 // bytesize
             for _x in range(n1):
                 buffer = f.read(bytesize)
                 (l_value,) = struct.unpack(longlongformat, buffer)
                 hash += l_value
                 hash = hash & 0xFFFFFFFFFFFFFFFF  # to remain as 64bit number
             f.seek(max(0, filesize - 65536), 0)
@@ -192,8 +189,8 @@
                 hash += l_value
                 hash = hash & 0xFFFFFFFFFFFFFFFF
 
         returnedhash = "%016x" % hash
         return returnedhash
 
     except IOError:
-        return "000000000000000000"
+        return ""
```

### Comparing `Subsearch-2.33.5/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/utils/io_json.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/io_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     data["percentage_threshold"] = 90
     data["rename_best_match"] = True
     data["context_menu"] = True
     data["context_menu_icon"] = True
     data["manual_download_fail"] = True
     data["manual_download_mode"] = False
     data["use_threading"] = True
+    data["multiple_app_instances"] = False
     data["show_terminal"] = False
     data["log_to_file"] = False
     data["file_extensions"] = dict.fromkeys(data["file_extensions"], True)
     data["providers"] = dict.fromkeys(data["providers"], True)
     with open(APPLICATION_CONFIG_JSON, "r+", encoding="utf-8") as file:
         file.seek(0)
         json.dump(data, file, indent=4)
```

### Comparing `Subsearch-2.33.5/src/subsearch/utils/io_winreg.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/io_winreg.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import winreg
 from pathlib import Path
 
 from subsearch.data import app_paths
 from subsearch.utils import file_manager
 
 COMPUTER_NAME = socket.gethostname()
-CLASSES_PATH = "Software\\Classes"
-ASTERISK_PATH = "Software\\Classes\\*"
-SHELL_PATH = "Software\\Classes\\*\\shell"
-SUBSEARCH_PATH = "Software\\Classes\\*\\shell\\Subsearch"
-COMMAND_PATH = "Software\\Classes\\*\\shell\\Subsearch\\command"
+CLASSES_PATH = r"Software\Classes"
+ASTERISK_PATH = r"Software\Classes\*"
+SHELL_PATH = r"Software\Classes\*\shell"
+SUBSEARCH_PATH = r"Software\Classes\*\shell\Subsearch"
+COMMAND_PATH = r"Software\Classes\*\shell\Subsearch\command"
 
 
 def write_keys() -> None:
     """
     Writes keys to the windows registry.
     """
     key_paths = [(CLASSES_PATH, "*"), (ASTERISK_PATH, "shell"), (SHELL_PATH, "Subsearch"), (SUBSEARCH_PATH, "command")]
@@ -25,47 +25,42 @@
                 winreg.CreateKey(sk, sub_key)
 
 
 def write_all_valuex() -> None:
     """
     Write values to the registry for `subsearch`, `icon`, `appliesto` and `command`.
     """
-    write_valuex("subsearch")
-    write_valuex("icon")
-    write_valuex("appliesto")
-    write_valuex("command")
+    items = ["subsearch", "icon", "appliesto", "command"]
+    for i in items:
+        write_valuex(i)
 
 
 def write_valuex(key: str) -> None:
     """
     Write a value to registry key.
 
     Args:
         key: A string that represents the target registry key.
 
     Returns:
         None.
     """
-    if key == "subsearch":
-        key_type = SUBSEARCH_PATH
-        value_name = ""
-        value = "Subsearch"
-    if key.lower() == "icon":
-        key_type = SUBSEARCH_PATH
-        value_name = "Icon"
-        value = get_icon_value()
-    elif key.lower() == "appliesto":
-        key_type = SUBSEARCH_PATH
-        value_name = "AppliesTo"
-        value = get_appliesto_value()
-    elif key.lower() == "command":
-        key_type = COMMAND_PATH
-        value_name = ""
-        value = get_command_value()
-    open_write_valuex(key_type, value_name, value)
+    key_map = {
+        "subsearch": {"key_type": SUBSEARCH_PATH, "value_name": "", "value": "Subsearch"},
+        "icon": {"key_type": SUBSEARCH_PATH, "value_name": "Icon", "value": get_icon_value()},
+        "appliesto": {"key_type": SUBSEARCH_PATH, "value_name": "AppliesTo", "value": get_appliesto_value()},
+        "command": {"key_type": COMMAND_PATH, "value_name": "", "value": get_command_value()},
+    }
+
+    key = key.lower()
+    if key in key_map:
+        key_type = key_map[key]["key_type"]
+        value_name = key_map[key]["value_name"]
+        value = key_map[key]["value"]
+        open_write_valuex(key_type, value_name, value)
 
 
 def open_write_valuex(sub_key: str, value_name: str, value: str) -> None:
     """
     Writes a value to a specific key in the Windows registry.
 
     Args:
```

### Comparing `Subsearch-2.33.5/src/subsearch/utils/log.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,29 +35,28 @@
     file_handler.setFormatter(formatter)
     logger.addHandler(file_handler)
 
 
 def output(msg: str, terminal: bool = True, to_log: bool = True, level: str = "info"):
     def _to_log(msg: str, level: str) -> None:
         if video_data is None or LOG_TO_FILE is False:
-            return None
+            return
         if to_log is False:
-            return None
-        if level == "info":
-            logger.info(msg)
-        elif level == "warning":
-            logger.warning(msg)
-        elif level == "error":
-            logger.error(msg)
-        elif level == "critical":
-            logger.critical(msg)
+            return
+        log_methods = {
+            "info": logger.info,
+            "warning": logger.warning,
+            "error": logger.error,
+            "critical": logger.critical,
+        }
+        log_methods[level](msg)
 
     def _to_terminal(msg: str, to_terminal, level: str) -> None:
         if to_terminal is False:
-            return None
+            return
         if level == "info":
             lock = Lock()
             lock.acquire()
             print(msg)
             lock.release()
         else:
             print(f"{level.upper()} - {msg}")
@@ -88,54 +87,103 @@
 def output_done_with_tasks(end_new_line: bool = False) -> None:
     output("Done with tasks")
     if end_new_line:
         output("")
 
 
 def output_parameters() -> None:
-    output_header(f"User data")
-    output(f"Language:                         {language_data.name}, {language_data.alpha_1}, {language_data.alpha_2b}")
-    output(f"Use HI subtitle:                  {app_config.hearing_impaired}")
-    output(f"Use non-HI subtitle:              {app_config.non_hearing_impaired}")
-    output(f"Match threshold:                  {app_config.percentage_threshold}%")
-    output(f"Use site subscene:                {app_config.providers['subscene_site']}")
-    output(f"Use site opensubtitles:           {app_config.providers['opensubtitles_site']}")
-    output(f"Use hash opensubtitles:           {app_config.providers['opensubtitles_hash']}")
-    output(f"Use site yifysubtitles:           {app_config.providers['yifysubtitles_site']}")
-    output("")
-    output_header(f"File data")
-    output(f"Filename:                         {video_data.filename}")
-    output(f"Directory:                        {video_data.directory_path}")
-    output("")
-    output_header(f"Release data")
-    output(f"Title:                            {release_data.title}")
-    output(f"Year:                             {release_data.year}")
-    output(f"Season:                           {release_data.season}, {release_data.season_ordinal}")
-    output(f"Episode:                          {release_data.episode}, {release_data.episode_ordinal}")
-    output(f"Series:                           {release_data.tvseries}")
-    output(f"Release:                          {release_data.release}")
-    output(f"Group:                            {release_data.group}")
-    output(f"File hash:                        {release_data.file_hash}")
-    output("")
-    output_header(f"Provider url data")
-    output(f"subscene_site:                    {provider_urls.subscene}")
-    output(f"opensubtitles_site:               {provider_urls.opensubtitles}")
-    output(f"opensubtitles_hash:               {provider_urls.opensubtitles_hash}")
-    output(f"yifysubtitles_site:               {provider_urls.yifysubtitles}")
+    """
+    Logs the parameters used by the application.
 
-    output("")
+    Args:
+        data: A dictionary containing the header and the data.
+
+    Returns:
+        None
+    """
+    data = {
+        "User data": [
+            {"Language": f"{language_data.name}, {language_data.alpha_1}, {language_data.alpha_2b}"},
+            {"Use HI subtitle": app_config.hearing_impaired},
+            {"Use non-HI subtitle": app_config.non_hearing_impaired},
+            {"Match threshold": f"{app_config.percentage_threshold}%"},
+            {"Use site subscene": app_config.providers["subscene_site"]},
+            {"Use site opensubtitles": app_config.providers["opensubtitles_site"]},
+            {"Use hash opensubtitles": app_config.providers["opensubtitles_hash"]},
+            {"Use site yifysubtitles": app_config.providers["yifysubtitles_site"]},
+        ],
+        "File data": [{"Filename": video_data.filename}, {"Directory": video_data.directory_path}],
+        "Release data": [
+            {"Title": release_data.title},
+            {"Year": release_data.year},
+            {"Season": f"{release_data.season}, {release_data.season_ordinal}"},
+            {"Episode": f"{release_data.episode}, {release_data.episode_ordinal}"},
+            {"Series": release_data.tvseries},
+            {"Release": release_data.release},
+            {"Group": release_data.group},
+            {"File hash": release_data.file_hash},
+        ],
+        "Provider url data": [
+            {"subscene_site": provider_urls.subscene},
+            {"opensubtitles_site": provider_urls.opensubtitles},
+            {"opensubtitles_hash": provider_urls.opensubtitles_hash},
+            {"yifysubtitles_site": provider_urls.yifysubtitles},
+        ],
+    }
+    for header, header_data in data.items():
+        output_header(header)
+        for item in header_data:
+            key, value = list(item.items())[0]
+            padding = " " * (30 - len(key))
+            output(f"{key}:{padding}{value}")
+        output("")
 
 
 def output_match(provider: str, pct_result: int, key: str, to_log_: bool = False) -> None:
     if pct_result >= app_config.percentage_threshold:
         output(f"> {provider:<14}{pct_result:>3}% {key}", to_log=to_log_)
     else:
         output(f"  {provider:<14}{pct_result:>3}% {key}", to_log=to_log_)
 
 
+def path_action(action_type: str, src_: Path, dst_: Path | None = None) -> None:
+    """
+    Logs a message indicating the removal, renaming, moving, or extraction of a file or directory.
+
+    Args:
+        action_type (str): A string representing the type of action being performed (e.g. "remove", "rename", "move", "extract").
+        src_ (Path): A Path object representing the file or directory being acted upon.
+        dst_ (Path, optional): An optional Path object representing the new location or name of the file or directory (used for renaming, moving and extracting actions). Defaults to None.
+
+    Returns:
+        None
+    """
+    if src_.is_file():
+        type = "file"
+    elif src_.is_dir():
+        type = "directory"
+
+    src = src_.relative_to(src_.parent.parent) if src_ else None
+    dst = dst_.relative_to(dst_.parent.parent) if dst_ else None
+
+    action_messages: dict[str, str] = {
+        "remove": rf"Removing {type}: ...\{src}",
+        "rename": rf"Renaming {type}: ...\{src} -> ...\{dst}",
+        "move": rf"Moving {type}: ...\{src} -> ...\{dst}",
+        "extract": rf"Extracting archive: ...\{src} -> ...\{dst}",
+    }
+
+    message = action_messages.get(action_type)
+
+    if not message:
+        raise ValueError("Invalid action type")
+
+    output(message)
+
+
 def set_logger_data(**kwargs) -> None:
     global release_data, app_config, provider_urls, language_data
     release_data = kwargs["release_data"]
     app_config = kwargs["app_config"]
     provider_urls = kwargs["provider_urls"]
     language_data = kwargs["language_data"]
```

### Comparing `Subsearch-2.33.5/src/subsearch/utils/string_parser.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.5/src/subsearch/utils/updates.py` & `Subsearch-2.34.0rc1/src/subsearch/utils/updates.py`

 * *Files identical despite different names*

