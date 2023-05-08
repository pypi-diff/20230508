# Comparing `tmp/batogram-1.0.6.tar.gz` & `tmp/batogram-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batogram-1.0.6.tar", last modified: Sun Apr 23 19:36:38 2023, max compression
+gzip compressed data, was "batogram-1.0.7.tar", last modified: Mon May  8 12:53:54 2023, max compression
```

## Comparing `batogram-1.0.6.tar` & `batogram-1.0.7.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.649627 batogram-1.0.6/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-04-22 20:32:02.000000 batogram-1.0.6/LICENSE
--rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-04-21 19:32:05.000000 batogram-1.0.6/MANIFEST.in
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6317 2023-04-23 19:36:38.648627 batogram-1.0.6/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4369 2023-04-23 19:35:13.000000 batogram-1.0.6/README.md
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.572626 batogram-1.0.6/batogram/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-04-23 19:25:54.000000 batogram-1.0.6/batogram/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/__main__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/about.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4634 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/amplitudegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2599 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/appsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5255 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/appsettingsmodal.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.580626 batogram-1.0.6/batogram/assets/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/3669170_home_ic_icon.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-left-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-left-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-right-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-right-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/batogram.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/download-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/drag-move-2-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/expand-left-right-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/expand-up-down-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/home-4-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/zoom-in-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7482 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/audiofileservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/breadcrumbservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7257 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/buttonframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/chunky_spectrogram.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.631627 batogram-1.0.6/batogram/colour_maps/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L01.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L03.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L05.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L06.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L07.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L08.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L09.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L16.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L17.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L18.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L19.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L20.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/black-body-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/inferno-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3593 2023-04-22 20:37:59.000000 batogram-1.0.6/batogram/colourmap.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1605 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/common.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1762 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/constants.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.636627 batogram-1.0.6/batogram/external/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/external/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/external/guano.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/external/tooltip.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/fileinfoframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2638 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/frames.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5298 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/graphsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/historianservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    27810 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/layouts.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1244 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/modalwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    28314 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/morebncframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    12392 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/moreframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/morerenderingframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6055 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/morescaleframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4486 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/profilegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/readoutframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    56511 2023-04-22 19:51:11.000000 batogram-1.0.6/batogram/rendering.py
--rwxr-xr-x   0 jmears    (1000) jmears    (1000)    34753 2023-04-22 19:51:11.000000 batogram-1.0.6/batogram/rootwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-04-22 20:48:37.000000 batogram-1.0.6/batogram/runner.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.647627 batogram-1.0.6/batogram/samples/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/samples/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    19066 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/spectrogramgraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    15524 2023-04-23 18:49:49.000000 batogram-1.0.6/batogram/spectrogrammouseservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/validatingwidgets.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    13433 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/wavfileparser.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.578626 batogram-1.0.6/batogram.egg-info/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6317 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2226 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/SOURCES.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/dependency_links.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/entry_points.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/requires.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/top_level.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1467 2023-04-23 19:26:27.000000 batogram-1.0.6/pyproject.toml
--rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-04-23 19:36:38.649627 batogram-1.0.6/setup.cfg
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.808996 batogram-1.0.7/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.0.7/LICENSE
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.0.7/MANIFEST.in
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6425 2023-05-08 12:53:54.808996 batogram-1.0.7/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4478 2023-05-08 11:32:46.000000 batogram-1.0.7/README.md
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.802996 batogram-1.0.7/batogram/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-05-08 12:45:47.000000 batogram-1.0.7/batogram/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/__main__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/about.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4634 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/amplitudegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6212 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/appsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/appsettingsmodal.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.804996 batogram-1.0.7/batogram/assets/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/3669170_home_ic_icon.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-left-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-left-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-right-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-right-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/batogram.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/download-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/drag-move-2-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/expand-left-right-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/expand-up-down-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/fullscreen-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/home-4-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/zoom-in-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7542 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/audiofileservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/breadcrumbservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/buttonframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/chunky_spectrogram.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.807996 batogram-1.0.7/batogram/colour_maps/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L01.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L03.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L05.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L06.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L07.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L08.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L09.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L16.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L17.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L18.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L19.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L20.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/black-body-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/inferno-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colourmap.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1605 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/common.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1762 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/constants.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.807996 batogram-1.0.7/batogram/external/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/external/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/external/guano.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/external/tooltip.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/fileinfoframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2638 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/frames.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5241 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/graphsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/historianservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30878 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/layouts.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1134 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/modalwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    28313 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/morebncframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    12442 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/moreframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/morerenderingframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6055 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/morescaleframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4596 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/profilegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/readoutframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    59357 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/rendering.py
+-rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35194 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/rootwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/runner.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.807996 batogram-1.0.7/batogram/samples/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/samples/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    18969 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/spectrogramgraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    15546 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/spectrogrammouseservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/validatingwidgets.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    13442 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/wavfileparser.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.802996 batogram-1.0.7/batogram.egg-info/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6425 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2262 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/SOURCES.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/dependency_links.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/entry_points.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/requires.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/top_level.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-05-08 12:46:12.000000 batogram-1.0.7/pyproject.toml
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-05-08 12:53:54.808996 batogram-1.0.7/setup.cfg
```

### Comparing `batogram-1.0.6/LICENSE` & `batogram-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/PKG-INFO` & `batogram-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.6
+Version: 1.0.7
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,21 +26,23 @@
 Keywords: bat,spectrogram,chiropterology,fourier,ultrasonic,ultrasound,echo,GUANO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-batogram
+Batogram
 ========
 
+![Screen Shot](docs/screenshot.png "Screen Shot")
+
 Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
@@ -54,30 +56,31 @@
 
 ### Windows
 
 There are currently two approaches to installing Batogram on Windows. The first and simplest
 method is as follows:
 
 * Download a Batogram executable for Windows from Github. Available releases are listed 
-[here](https://github.com/jmears63/batogram/releases).
+[here](https://github.com/jmears63/batogram/releases). You need the file named batogram.exe, listed
+under Assets.
 * Probably Windows Defender will warn you of the danger of downloading such files from unknown
 sources. Assess the risk and decide if you going ahead. Assuming you are, proceed to the
 next step.
 * Copy the downloaded executable to your Windows desktop, so that you can find it when you want it.
 * Double click it on the desktop to run it. The first time you run it, it will take a little longer to start 
 up than usual. You will notice a command window launched alongside Batogram - ignore it. This is to
 aid debugging, and will be removed in a future release.
 
 The second installation method is to install Python on your Windows computer, and then follow the 
 same steps as the Linux installation. If you take this route, I assume you know what you are doing.
 
 ### Linux
 
 On Linux, Batogram is currently installed from the command line using pip, as below.
-You need to have Python 3.10 as a minimum.  
+You need to have Python 3.9 as a minimum.  
 
     # Create a virtual environment at a convenient location in your home directory:
     mkdir ~/batogram
     cd batogram
     python3 -m venv venv
     source venv/bin/activate
```

### Comparing `batogram-1.0.6/README.md` & `batogram-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-batogram
+Batogram
 ========
 
+![Screen Shot](docs/screenshot.png "Screen Shot")
+
 Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
@@ -18,30 +20,31 @@
 
 ### Windows
 
 There are currently two approaches to installing Batogram on Windows. The first and simplest
 method is as follows:
 
 * Download a Batogram executable for Windows from Github. Available releases are listed 
-[here](https://github.com/jmears63/batogram/releases).
+[here](https://github.com/jmears63/batogram/releases). You need the file named batogram.exe, listed
+under Assets.
 * Probably Windows Defender will warn you of the danger of downloading such files from unknown
 sources. Assess the risk and decide if you going ahead. Assuming you are, proceed to the
 next step.
 * Copy the downloaded executable to your Windows desktop, so that you can find it when you want it.
 * Double click it on the desktop to run it. The first time you run it, it will take a little longer to start 
 up than usual. You will notice a command window launched alongside Batogram - ignore it. This is to
 aid debugging, and will be removed in a future release.
 
 The second installation method is to install Python on your Windows computer, and then follow the 
 same steps as the Linux installation. If you take this route, I assume you know what you are doing.
 
 ### Linux
 
 On Linux, Batogram is currently installed from the command line using pip, as below.
-You need to have Python 3.10 as a minimum.  
+You need to have Python 3.9 as a minimum.  
 
     # Create a virtual environment at a convenient location in your home directory:
     mkdir ~/batogram
     cd batogram
     python3 -m venv venv
     source venv/bin/activate
```

### Comparing `batogram-1.0.6/batogram/__main__.py` & `batogram-1.0.7/batogram/__main__.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/about.py` & `batogram-1.0.7/batogram/about.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/amplitudegraphframe.py` & `batogram-1.0.7/batogram/amplitudegraphframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/assets/batogram.png` & `batogram-1.0.7/batogram/assets/batogram.png`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/audiofileservice.py` & `batogram-1.0.7/batogram/audiofileservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import time
+from typing import Optional
+
 import numpy as np
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from numpy import ndarray
 from .common import AxisRange
 from .graphsettings import MAX_FFT_SAMPLES
@@ -75,21 +77,21 @@
         self._filepath = filepath
         self._sample_rate = None
         self._sample_count = None
         self._raw_data = None
         self._data_serial: int = 0  # Used for the pipeline to detect when the file data has changed.
         self._metadata = None
         self._guano_data = None
-        self._file_parser: WavFileParser | None = None
-        self._channels: int | None = None
-        self._bytes_per_value: int | None = None
+        self._file_parser: Optional[WavFileParser] = None
+        self._channels: Optional[int] = None
+        self._bytes_per_value: Optional[int] = None
 
     def open(self):
         self._file_parser = WavFileParser(self._filepath)
-        chunks = self._file_parser.open()
+        chunks: WavFileParser.Chunks = self._file_parser.open()
         sample_rate, data, guanodata = chunks.header.sample_rate_hz, chunks.data, chunks.guanodata
 
         channels = chunks.header.num_channels  # Avoid warnings.
         sample_count = chunks.data.actual_sample_count
         # print("Opened file {}: rate = {} channels = {} samples = {}".format(self._filepath, sample_rate, channels, sample_count))
 
         # Do some sanity checks:
```

### Comparing `batogram-1.0.6/batogram/breadcrumbservice.py` & `batogram-1.0.7/batogram/breadcrumbservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/buttonframe.py` & `batogram-1.0.7/batogram/buttonframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             col += 1
 
         left_space = tk.Label(self)
         left_space.grid(row=0, column=col)
         spacer1_index = col
         col += 1
 
-        self._home_image = self._load_image("home-4-line.png")
+        self._home_image = self._load_image("fullscreen-line.png")
         self._home_button = MyButton(self, self._home_image, command=home_command)
         self._home_button.grid(row=0, column=col, padx=0, ipadx=0, sticky="NSEW")
         ToolTip(self._home_button, msg="Reset axis ranges to match input data")
         col += 1
 
         self._previous_image = self._load_image("arrow-left-line.png")
         self._previous_button = MyButton(self, self._previous_image,
```

### Comparing `batogram-1.0.6/batogram/chunky_spectrogram.py` & `batogram-1.0.7/batogram/chunky_spectrogram.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L01.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L01.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L03.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L03.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L05.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L05.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L06.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L06.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L07.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L07.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L08.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L08.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L09.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L09.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L16.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L16.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L17.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L17.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L18.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L18.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L19.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L19.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/CET-L20.csv` & `batogram-1.0.7/batogram/colour_maps/CET-L20.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/black-body-table-byte-1024.csv` & `batogram-1.0.7/batogram/colour_maps/black-body-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv` & `batogram-1.0.7/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/inferno-table-byte-1024.csv` & `batogram-1.0.7/batogram/colour_maps/inferno-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colour_maps/kindlmann-table-byte-1024.csv` & `batogram-1.0.7/batogram/colour_maps/kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/colourmap.py` & `batogram-1.0.7/batogram/colourmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+from typing import Optional
 
 import numpy as np
 
 from . import get_colour_map_path
 from .appsettings import COLOUR_MAPS, DEFAULT_COLOUR_MAP
 
 
@@ -30,16 +31,16 @@
     def __init__(self, map_file: str):
         """
         Don't use this to create instances, instead access
         the single shared instance using get_instance().
         """
 
         self._cmap = None
-        self._num_steps: int | None = None
-        self._polyfilla_colour: str | None = None
+        self._num_steps: Optional[int] = None
+        self._polyfilla_colour: Optional[str] = None
 
         self.reload_map(map_file)
 
     def reload_map(self, map_file: str):
         """
             Read a colour map from a CSV with thee or four columns. The last three columns
             are RGB byte values.
```

### Comparing `batogram-1.0.6/batogram/common.py` & `batogram-1.0.7/batogram/common.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/constants.py` & `batogram-1.0.7/batogram/constants.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/external/guano.py` & `batogram-1.0.7/batogram/external/guano.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/external/tooltip.py` & `batogram-1.0.7/batogram/external/tooltip.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/fileinfoframe.py` & `batogram-1.0.7/batogram/fileinfoframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/frames.py` & `batogram-1.0.7/batogram/frames.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/graphsettings.py` & `batogram-1.0.7/batogram/graphsettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from dataclasses import dataclass
 from typing import Optional, NoReturn, Callable
 
-from .appsettings import DEFAULT_COLOUR_MAP, COLOUR_MAPS
 from .common import AxisRange
 from .frames import DrawableFrame
 
 borderwidth = 10
 
 SUPPORTED_FFT_SAMPLES = [64, 128, 256, 512, 1024, 2048, 4096, 8192]
 DEFAULT_FFT_SAMPLES_INDEX = 3
```

### Comparing `batogram-1.0.6/batogram/historianservice.py` & `batogram-1.0.7/batogram/historianservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/layouts.py` & `batogram-1.0.7/batogram/layouts.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,43 +114,46 @@
     """This class knows how to lay out and draw the components of a graph."""
 
     def __init__(self, font_height, canvas_width, canvas_height):
         super().__init__(font_height, canvas_width, canvas_height)
         self._margin = int(self._font_height * 2)
         self._data_ranges: Optional[Tuple[AxisRange, AxisRange]] = None
         self._data_area = None
-        self._x_axis: AxisLayout | None = None
-        self._y_axis: AxisLayout | None = None
+        self._x_axis: Optional[AxisLayout] = None
+        self._y_axis: Optional[AxisLayout] = None
 
     def get_data_ranges(self) -> Tuple[AxisRange, AxisRange]:
         return self._data_ranges
 
+    def calc_preferred_time_range(self, sign: int) -> AxisRange:
+        return self._x_axis.calc_preferred_range(sign)
+
     def _get_right_margin(self):
         return self._canvas_width - self._margin, 0, self._canvas_width - 1, self._canvas_height - 1
 
     def _get_top_margin(self):
         return 0, 0, self._canvas_width - 1, self._margin - 1
 
     def _get_left_margin(self, axis_size):
         return 0, 0, axis_size - 1, self._canvas_height - 1
 
     def _get_bottom_margin(self, axis_size):
         return 0, self._canvas_height - 1, self._canvas_width - 1, self._canvas_height - axis_size - 1
 
-    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid: bool):
+    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid: bool, zero_based_x_axis: bool):
         """Draw a graph including axes, image and grid. We do this in two phases:
         (1) The axes etc., which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
 
         self._data_ranges = x_range, y_range
 
     def rect_to_values(self, pixel_rect) \
-            -> Tuple[float, float, float, float] | None:
+            -> Optional[Tuple[float, float, float, float]]:
         """Scale the pixel rectangle supplied to real axis values."""
 
         l, t, r, b = pixel_rect
         if self._x_axis and self._y_axis:
             # if clamp:
             vl = self._x_axis.canvas_to_axis(l)
             vr = self._x_axis.canvas_to_axis(r)
@@ -172,21 +175,26 @@
         else:
             return None
 
     @staticmethod
     def _draw_graph_image(canvas, data_area, image):
         (il, it, ir, ib) = data_area
 
-        # There may be a right margin to fill, if we are zoomed right out:
+        # There may be a right margin to fill, if we are zoomed right out. And
+        # rounding errors may result in the image being one pixel short. So, we apply
+        # polyfilla around the right and bottom edge.
         image_height, image_width, _ = image.shape
-        data_area_width: int = ir - il
+        data_area_width, data_area_height = ir - il + 1, ib - it + 1
+        fill_colour: str = colourmap.instance.get_polyfilla_colour()
         if image_width < data_area_width:
             delta = data_area_width - image_width
-            fill_colour: str = colourmap.instance.get_polyfilla_colour()
-            canvas.create_rectangle(ir - delta, it, ir, it + image_height - 1, fill=fill_colour, outline=fill_colour)
+            canvas.create_rectangle(ir - delta, it, ir, ib, fill=fill_colour, outline=fill_colour)
+        if image_height < data_area_height:
+            delta = data_area_height - image_height
+            canvas.create_rectangle(il, ib - delta, ir, ib, fill=fill_colour, outline=fill_colour)
 
         inverted_image = Image.fromarray(np.uint8(image)).convert('RGB')
         pil_image = ImageOps.flip(inverted_image)
         image = ImageTk.PhotoImage(pil_image)
         canvas.my_image = image  # Hack to protect the image against garbage collection
         # (see https://web.archive.org/web/20201111190625id_/http://effbot.org/pyfaq/why-do-my-tkinter-images-not-appear.htm)
         canvas.create_image(il, it, image=image, anchor='nw')
@@ -251,15 +259,15 @@
         self._hide_text = hide_text
         self._font_name = "helvetica"
         self._layout()
         self._min_pixel = None
         self._max_pixel = None
         self._axis_range: Optional[AxisRange] = None
         self._units: List[AxisUnit] = sorted(units, key=lambda u: u.limit)  # Ascending.
-        self._units_to_use: AxisUnit | None = None
+        self._units_to_use: Optional[AxisUnit] = None
 
     def _layout(self):
         # These coordinates increase from 0 on the outside to maximum
         # next to the data area.
 
         unit = self._font_height  # Everything is relative to font size.
         half_unit = int(unit / 2 + 0.5)  # Avoid floating point.
@@ -354,19 +362,71 @@
         """Decide what units to use based on the axis range."""
 
         if len(self._units) == 1:
             return self._units[0]
         else:
             abs_max: float = max(abs(axis_range.min), abs(axis_range.max))
             # The possible units are already sorted in ascending order.
+            u = self._units[0]      # Avoid a warning.
             for u in self._units:
                 if abs_max < u.limit:
                     return u
             return u
 
+    _preferred_ms_per_100pixels = [1.0, 2.0, 5.0, 10.0, 20.0, 50.0, 100.0, 200.0, 500.0, 1000.0, 2000.0, 5000.0]
+
+    def calc_preferred_range(self, sign: int) -> AxisRange:
+        """Calculate a preset axis range that is next large (or smaller) than the current range."""
+
+        #
+        # We want the total time span to result in one of these peferred ranges.
+        #   1, 2, 5, 10, 20, 50 etc ms per 100 pixels.
+        # so (time range) / (data_width_pixels) = preset value
+        #
+        # The supplied sign tells us whether we are aiming to zoom in or out relative to the current.
+        # Positive sign increases the axis range.
+        #
+
+        current_range = self._axis_range
+        centre = (current_range.min + current_range.max) / 2
+        span = current_range.max - current_range.min
+        pixel_span = self._max_pixel - self._min_pixel
+
+        # Calculate the current scaling, that we went to round up or down to preferred:
+        ms_per_100pixels = span * 100.0 * 1000.0 / pixel_span
+        new_ms_per_100pixels = ms_per_100pixels     # Default - no change.
+
+        nudge_factor = 1.05     # Slight fudge in case the current range is a preferred range.
+        if sign > 0:
+            # We want to increase and round the range:
+            nudged_ms_per_100pixels = ms_per_100pixels * nudge_factor
+            for preferred in self._preferred_ms_per_100pixels:
+                if nudged_ms_per_100pixels < preferred:
+                    new_ms_per_100pixels = preferred
+                    break
+            # Otherwise, the range is already larger than the largest, no change.
+            pass
+        elif sign < 0:
+            # We want to decrease and round the range:
+            nudged_ms_per_100pixels = ms_per_100pixels / nudge_factor
+            for preferred in reversed(self._preferred_ms_per_100pixels):
+                if nudged_ms_per_100pixels > preferred:
+                    new_ms_per_100pixels = preferred
+                    break
+            # Otherwise, the range is already smaller than the smallest, no change.
+            pass
+
+        new_span = new_ms_per_100pixels * pixel_span / (100.0 * 1000.0)
+        # print("Prefered {} -> {}".format(span, new_span))
+
+        # The new span might go beyond the range of the actual data, but it will
+        # be clipped by the caller.
+
+        return AxisRange(centre - new_span / 2, centre + new_span / 2)
+
 
 class SpectrogramLayout(GraphLayout):
     """This Layout knows how to lay out and raw a spectrogram."""
 
     _x_axis_unit = [AxisUnit(scaler=1.0, units="s"),  # Default
                     AxisUnit(limit=0.5, scaler=1E-3, units="ms")
                     ]
@@ -388,15 +448,15 @@
         self._data_area = (
             self._y_axis_width, self._margin, self._canvas_width - self._margin - 1,
             self._canvas_height - self._x_axis_height - 1)
         self._dead_space = (
             0, self._canvas_height - self._x_axis_height, self._y_axis_width - 1, self._canvas_height - 1)
 
     def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid, zero_based_x_axis: bool):
-        super().draw(canvas, x_range, y_range, show_grid)
+        super().draw(canvas, x_range, y_range, show_grid, zero_based_x_axis)
 
         """Draw a graph including axes, image and grid. We do this in two phases:
         (1) The axes etc, which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
 
@@ -475,16 +535,16 @@
         self._x_axis_height = self._x_axis.get_size()
         self._y_axis_width = self._y_axis.get_size()
 
         # Calculate some *inclusive* zero based rectangle coords:
         self._data_area = (
             self._y_axis_width, 0, self._canvas_width - self._margin - 1, self._canvas_height)
 
-    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid):
-        super().draw(canvas, x_range, y_range, show_grid)
+    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid: bool, zero_based_x_axis: bool = False):
+        super().draw(canvas, x_range, y_range, show_grid, zero_based_x_axis)
 
         """Draw a graph including axes, image and grid. We do this in two phases:
         (1) The axes etc, which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
 
@@ -546,15 +606,15 @@
         self._data_area = (
             self._y_axis_width, self._margin, self._canvas_width - self._margin - 1,
             self._canvas_height - self._x_axis_height - 1)
         self._dead_space = (
             0, self._canvas_height - self._x_axis_height, self._y_axis_width - 1, self._canvas_height - 1)
 
     def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid: bool, zero_based_x_axis: bool):
-        super().draw(canvas, x_range, y_range, show_grid)
+        super().draw(canvas, x_range, y_range, show_grid, zero_based_x_axis)
 
         """Draw a graph including axes, image and grid. We do this in two phases:
         (1) The axes etc, which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
```

### Comparing `batogram-1.0.6/batogram/modalwindow.py` & `batogram-1.0.7/batogram/modalwindow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import tkinter as tk
 
 
 class ModalWindow(tk.Toplevel):
     def __init__(self, parent):
         super().__init__(parent)
-        self.transient(parent)  # Doesn't seem to do anything.
-        # self.attributes('-topmost', 'true')  # Keep in front of its parent.
+        self.transient(parent)
 
         # Find the highest level parent window we can:
         ancestor = parent
         while ancestor.master:
             ancestor = ancestor.master
 
         # Don't prescribe the size, let the window adjust to its contents:
```

### Comparing `batogram-1.0.6/batogram/morebncframe.py` & `batogram-1.0.7/batogram/morebncframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # SOFTWARE.
 import math
 import tkinter as tk
 import numpy as np
 
 from . import colourmap
 from abc import abstractmethod, ABC
-from typing import Any, List, Tuple
+from typing import Any, List, Tuple, Optional
 from .common import clip_to_range
 from .frames import DrawableFrame
 from .validatingwidgets import ValidatingMapOptionMenu, ValidatingFrameHelper, ValidatingRadiobutton, \
     DoubleValidatingEntry
 from .graphsettings import GraphSettings, BNC_MODES, borderwidth, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, \
     BNC_INTERACTIVE_MODE
 
@@ -159,15 +159,15 @@
 
 class ScaleCanvas(tk.Canvas):
     """A canvas the displays the colour scale for a spectrogram."""
 
     def __init__(self, parent):
         super().__init__(parent, bg="black", height=15, width=CANVAS_WIDTH)
 
-    def set_scale_pixels(self, prange: tuple[int, int] | None):
+    def set_scale_pixels(self, prange: Optional[tuple[int, int]]):
         """Draw a colour mapped scale."""
         width, height = self.winfo_width(), self.winfo_height()
 
         self.clear()
         if prange is not None:
             xmin, xmax = prange
             if xmin < xmax:
@@ -192,24 +192,24 @@
     _DRAG_CURSOR = "sb_h_double_arrow"
 
     def __init__(self, canvas: "HistogramCanvas", line: "BnCLine", which: int, tag_name: str):
         self._line = line
         self._canvas = canvas
         self._tag_name = tag_name
         self._which = which  # Which dragger are we? Maybe a subclass would be cleaner, but hey ho.
-        self._rectangle: int | None = None  # The rectangle drawn on the canvas, if any.
+        self._rectangle: Optional[int] = None  # The rectangle drawn on the canvas, if any.
         # _pos is the position we were originally drawn at:
-        self._pos: tuple[int, int] | None = None
+        self._pos: Optional[tuple[int, int]] = None
         # _moved is the position have been moved to, updated during a drag:
-        self._moved: tuple[int, int] | None = None
+        self._moved: Optional[tuple[int, int]] = None
 
-        self._start_event: Any | None = None  # If this is non None, we know we are currently dragging.
-        self._width: int | None = None
-        self._height: int | None = None
-        self._allowed_x_range: tuple[int, int] | None = None
+        self._start_event: Optional[Any] = None  # If this is non None, we know we are currently dragging.
+        self._width: Optional[int] = None
+        self._height: Optional[int] = None
+        self._allowed_x_range: Optional[tuple[int, int]] = None
 
         canvas.tag_bind(self._tag_name, "<Enter>", lambda event: self.mouse_enters_dragger(event))
         canvas.tag_bind(self._tag_name, "<Leave>", lambda event: self.mouse_leaves_dragger(event))
         canvas.tag_bind(self._tag_name, "<Button-1>", lambda event: self._on_click(event))
         canvas.tag_bind(self._tag_name, "<B1-Motion>", lambda event: self._on_move(event))
         canvas.tag_bind(self._tag_name, "<ButtonRelease-1>", lambda event: self._on_release(event))
 
@@ -318,19 +318,19 @@
         self._scale_canvas = scale_canvas  # We'll upate the scale whenever it changes.
 
         # The line always has a dragger at each end. We will show and hide them as required by the mode:
         self._min_dragger: Dragger = Dragger(self._histogram_canvas, self, self.MIN_DRAGGER, "min")
         self._max_dragger: Dragger = Dragger(self._histogram_canvas, self, self.MAX_DRAGGER, "max")
         self._draggers: List[Dragger] = [self._min_dragger, self._max_dragger]
 
-        self._line: int | None = None       # The line object in the canvas.
-        self._prange: tuple[int, int] | None = None     # The x pixel range spanned by the line.
+        self._line: Optional[int] = None       # The line object in the canvas.
+        self._prange: Optional[tuple[int, int]] = None     # The x pixel range spanned by the line.
 
-        self._width: int | None = None      # Cache the canvas size for convenience.
-        self._height: int | None = None
+        self._width: Optional[int] = None      # Cache the canvas size for convenience.
+        self._height: Optional[int] = None
 
     def show(self, prange: tuple[int, int], with_draggers: bool):
         """
         Draw or remove the BnC line, with or without draggers according to mode.
         """
 
         # Cache the canvas size for convenience:
@@ -386,22 +386,21 @@
             d.hide()
 
     def on_dragger_moved(self, which: int, x_resulting: int):
         """The draggers call this as notification that they have moved."""
 
         # Update our record of the dragger positions:
         pmin, pmax = self._prange
-        match which:
-            case self.MIN_DRAGGER:
-                pmin = x_resulting
-            case self.MAX_DRAGGER:
-                pmax = x_resulting
-            case _:
-                # Shouldn't get here.
-                pass
+        if which == self.MIN_DRAGGER:
+            pmin = x_resulting
+        elif which == self.MAX_DRAGGER:
+            pmax = x_resulting
+        else:
+            # Shouldn't get here.
+            pass
         self._prange = pmin, pmax
 
         # Redraw the line. The moving dragger has already been redrawn, the other is fine as it is.
         self._draw_line(self._prange)
 
     def on_dragger_released(self):
         min_x, _ = self._min_dragger.get_pos()
@@ -415,23 +414,22 @@
         self._histogram_canvas.on_bnc_interactive_change((min_x, max_x))
 
     def get_allowed_range(self, which_asking: int) -> tuple[int, int]:
         """A dragger calls this method to get the range of x values which we will
         allow it to have."""
         min_spacing = 5
         prange = 1, self._width - 1
-        match which_asking:
-            case BnCLine.MIN_DRAGGER:
-                # This dragger must be to the left of the max dragger:
-                x_pos, _ = self._max_dragger.get_pos()
-                prange = (1, x_pos - min_spacing)
-            case BnCLine.MAX_DRAGGER:
-                # This dragger must be to the right of the min dragger:
-                x_pos, _ = self._min_dragger.get_pos()
-                prange = (x_pos + min_spacing, self._width - 1)
+        if which_asking == BnCLine.MIN_DRAGGER:
+            # This dragger must be to the left of the max dragger:
+            x_pos, _ = self._max_dragger.get_pos()
+            prange = (1, x_pos - min_spacing)
+        elif which_asking == BnCLine.MAX_DRAGGER:
+            # This dragger must be to the right of the min dragger:
+            x_pos, _ = self._min_dragger.get_pos()
+            prange = (x_pos + min_spacing, self._width - 1)
 
         return prange
 
     def on_wheel_move(self, delta: int):
         # Adjust the lower line value as though dragged left:
         min_x, _ = self._min_dragger.get_pos()
         max_x, _ = self._max_dragger.get_pos()
@@ -483,15 +481,15 @@
         # For Windows:
         self.bind("<MouseWheel>", self._on_wheel)
 
         self._reset_histogram()
 
     def on_bnc_interactive_change(self, prange: tuple[int, int]):
         # Scale the pixels to values:
-        vrange: Tuple[float, float] | None = self._pixels_to_values(prange)
+        vrange: Optional[Tuple[float, float]] = self._pixels_to_values(prange)
         if vrange is not None:
             self._parent.on_bnc_interactive_change(vrange)
 
     def show_histogram(self, data: np.ndarray):
         """Called from the rendering pipeline to display the histogram,
         and optionally an auto BnC range."""
         width, height = self.winfo_width(), self.winfo_height()
@@ -546,15 +544,15 @@
         self._bin_edges = None
         self._auto_vrange = None
 
     def on_bnc_settings_changed(self):
         # Convert the value range provided to a pixel range. Pixels
         # correspond to bin edges:
         vrange = self._settings.bnc_manual_min, self._settings.bnc_manual_max
-        prange: tuple[int, int] | None = self._values_to_pixels(vrange)
+        prange: Optional[tuple[int, int]] = self._values_to_pixels(vrange)
         interactive_mode: bool = self._settings.bnc_adjust_type == BNC_INTERACTIVE_MODE
         self._is_interactive_mode = interactive_mode
         if prange is not None:
             self._bnc_line.show(prange, interactive_mode)
 
     def hide_bnc_line(self):
         self._is_interactive_mode = False
@@ -575,16 +573,16 @@
     def _on_wheel(self, event):
         if self._is_interactive_mode:
             if event.delta > 0:
                 self._bnc_line.on_wheel_move(self._WHEEL_DELTA)
             else:
                 self._bnc_line.on_wheel_move(-self._WHEEL_DELTA)
 
-    def _values_to_pixels(self, vrange: tuple[float, float]) -> Tuple[int, int] | None:
-        prange: Tuple[int, int] | None = None
+    def _values_to_pixels(self, vrange: tuple[float, float]) -> Optional[Tuple[int, int]]:
+        prange: Optional[Tuple[int, int]] = None
         if self._bin_edges is not None:
             vmin, vmax = vrange
             # Scale vmin and vmax to bin numbers (which correspond to the x coordinate).
             # We choose the bin whose centre is closest to the value - that means,
             # add half a bin width and then floor.
             bin_count = len(self._bin_edges) - 1  # n bins have n+1 boundaries.
             if bin_count > 0:
@@ -595,16 +593,16 @@
                     bin_max = math.floor((vmax - bin_lowest) * bin_count / bin_range + 0.5)
                     bin_min = clip_to_range(bin_min, 0, bin_count - 1)
                     bin_max = clip_to_range(bin_max, 1, bin_count)
                     prange = bin_min, bin_max
 
         return prange
 
-    def _pixels_to_values(self, prange: Tuple[int, int]) -> Tuple[float, float] | None:
-        vrange: Tuple[float, float] | None = None
+    def _pixels_to_values(self, prange: Tuple[int, int]) -> Optional[Tuple[float, float]]:
+        vrange: Optional[Tuple[float, float]] = None
         if self._bin_edges is not None:
             pmin, pmax = prange
 
             bin_count = len(self._bin_edges - 1)
             if bin_count > 0:
                 # Scale bin numbers (which correspond to the x coordinate) to vmin and vmax:
                 bin_lowest, bin_highest = self._bin_edges[0], self._bin_edges[-1]
```

### Comparing `batogram-1.0.6/batogram/moreframe.py` & `batogram-1.0.7/batogram/moreframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 import webbrowser
+from typing import Optional
+
 import numpy as np
 
 from .graphsettings import GraphSettings
 
 from tkinter import scrolledtext
 from tkinter import messagebox, ttk, font
 from .morebncframe import HistogramInterface, BrightnessContrastFrame
@@ -69,21 +71,21 @@
 
     # One day, avoid this assumption:
     _CLICKABLE_COLOUR = "blue"
     _NORMAL_COLOUR = "black"
 
     def __init__(self, parent, *args, **kwargs):
         super().__init__(parent, *args, **kwargs)
-        self._url: str | None = None
+        self._url: Optional[str] = None
         self._underlined_font = font.Font(self, self.cget("font"))
         self._underlined_font.configure(underline=True)
         self._normal_font = font.Font(self, self.cget("font"))
         self.bind('<Button-1>', self._on_click)
 
-    def set_url(self, url: str | None):
+    def set_url(self, url: Optional[str]):
         self._url = url
         if url is not None:
             self.config(fg=self._CLICKABLE_COLOUR)
             self.config(font=self._underlined_font)
             self.config(cursor="hand2")
         else:
             self.config(fg=self._NORMAL_COLOUR)
@@ -94,15 +96,15 @@
         if self._url is not None:
             webbrowser.open(self._url, new=0, autoraise=True)
 
 
 class GuanoValue(tk.Label):
     """A file metadata value from GUANO data."""
 
-    def __init__(self, parent: "GuanoFrame", label: UrlLabel, guano_name: str, units: str | None):
+    def __init__(self, parent: "GuanoFrame", label: UrlLabel, guano_name: str, units: Optional[str]):
         self._my_var = tk.StringVar()
         super().__init__(parent, textvariable=self._my_var, width=25, anchor="w")
         self._my_parent: "GuanoFrame" = parent
         self._guano_name = guano_name
         self._units = "" if units is None else " {}".format(units)
         self._my_parent.register_value_widget(self)
         self._label = label
@@ -117,21 +119,21 @@
             value = "{}{}".format(data[self._guano_name], self._units)
             self._my_var.set(value)
         else:
             self._my_var.set("")
 
 
 class LatLongGuanoValue(GuanoValue):
-    def __init__(self, parent: "GuanoFrame", label: UrlLabel, guano_name: str, units: str | None):
+    def __init__(self, parent: "GuanoFrame", label: UrlLabel, guano_name: str, units: Optional[str]):
         super().__init__(parent, label, guano_name, units)
 
     def notify_update(self, data: GuanoFile):
         super().notify_update(data)
 
-        url: str | None = None
+        url: Optional[str] = None
         if data is not None and self._guano_name in data:
             lat_long = data[self._guano_name]
             try:
                 latitude, longitude = lat_long
                 zoom = 10
                 url = "http://maps.google.com/maps?z={}&t=m&q=loc:{}+{}".format(zoom, latitude, longitude)
                 # print("url = {}", url)
@@ -168,15 +170,15 @@
         self.rowconfigure(1, weight=0)
         self.columnconfigure(0, weight=1)
 
 
 class GuanoFrame(tk.Frame):
     def __init__(self, parent, pad: int):
         super().__init__(parent)
-        self._guano_data: GuanoFile | None = None
+        self._guano_data: Optional[GuanoFile] = None
         self._value_widgets = []
         self._pad = pad
 
         def add_guano_value(class_to_use, row: int, column: int, guano_field: str, ui_name: str = None,
                             units: str = None):
             if ui_name is None:
                 ui_name = guano_field
@@ -303,9 +305,9 @@
         # Make sure the error is visible to the user:
         self._settings_notebook.select(container)
         messagebox.showerror('Value Error', message)
 
     def get_histogram_interface(self) -> HistogramInterface:
         return self._settings_notebook
 
-    def set_guano_data(self, data: GuanoFile | None):
+    def set_guano_data(self, data: Optional[GuanoFile]):
         self._settings_notebook.set_guano_data(data)
```

### Comparing `batogram-1.0.6/batogram/morerenderingframe.py` & `batogram-1.0.7/batogram/morerenderingframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/morescaleframe.py` & `batogram-1.0.7/batogram/morescaleframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/profilegraphframe.py` & `batogram-1.0.7/batogram/profilegraphframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 
 PROFILE_WIDTH = 90
 
 
 class ProfileGraphFrame(GraphFrame):
     """A Frame containing a profile graph for a spectrogram."""
 
-    def __init__(self, parent, root, pipeline, data_context, settings):
+    def __init__(self, parent, root, pipeline, data_context, settings, is_reference):
         super().__init__(parent, root, pipeline, data_context, settings)
 
         self._canvas = tk.Canvas(self, bg="black", height=1, width=PROFILE_WIDTH)
         self._canvas.grid(row=0, column=0, sticky='nesw')
         self.columnconfigure(0, weight=1)
         self.rowconfigure(0, weight=1)
         self._parent = parent
+        self._is_reference = is_reference
 
         self.bind("<Configure>", self._on_canvas_change)
         self.bind(MAIN_PROFILE_COMPLETER_EVENT, self._do_completer)
 
         # self._pipeline = None   # Temporary, remove this.
 
     def draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
@@ -67,26 +68,26 @@
         graph_completer, data_area = layout.draw(self._canvas, profile_range, frequency_range,
                                                  self._settings.show_grid, self._settings.zero_based_time)
         if af_data and self._pipeline:
             # Kick off the pipeline which will create a graph in another thread,
             # and complete by generating an event that will finish drawing the grph:
             self._completer = graph_completer
             screen_factors = self._parent.get_screen_factors()
-            request = self._get_pipeline_request(af_data, data_area, time_range, frequency_range, screen_factors,
+            request = self._get_pipeline_request(self._is_reference, af_data, data_area, time_range, frequency_range, screen_factors,
                                                  self._dc.get_afs())
             self._pipeline.submit(request,
                                   lambda: self.event_generate(MAIN_PROFILE_COMPLETER_EVENT),
                                   self._pipeline_error_handler)
         else:
             # No data, so we can complete drawing the graph right away:
             graph_completer()
 
     @staticmethod
-    def _get_pipeline_request(data, data_area, time_range, frequency_range, screen_factors: tuple[float, float], rdr: RawDataReader):
-        request = ProfilePipelineRequest(data_area, data, time_range, frequency_range, screen_factors, rdr)
+    def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range, screen_factors: tuple[float, float], rdr: RawDataReader):
+        request = ProfilePipelineRequest(is_reference, data_area, data, time_range, frequency_range, screen_factors, rdr)
         return request
 
     def _do_completer(self, _):
         # A bit of a hack because tkinter doesn't seem to allow data to be attached to an event:
         completer = self._completer
         if completer:
             memory_limit_hit, request, points, v_range = self._pipeline.get_completion_data()
```

### Comparing `batogram-1.0.6/batogram/readoutframe.py` & `batogram-1.0.7/batogram/readoutframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/rendering.py` & `batogram-1.0.7/batogram/rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,22 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+from __future__ import annotations
 
 import math
+from time import process_time
+
 import numpy as np
 import scipy
+from scipy.interpolate import CubicSpline
 
 from . import colourmap, appsettings
 from copy import deepcopy
 from dataclasses import dataclass
 from threading import Lock, Thread, Condition
 from typing import Type, Tuple, Optional, Any, Callable
 from scipy import ndimage
@@ -117,18 +121,17 @@
                 return
 
             if pending_request_tuple is None:  # I suppose this might happen if there is a race I haven't thought of.
                 continue
 
             request, on_completion, on_error = pending_request_tuple
 
-            self.do_processing(request)
             try:
                 # Derived classes must define this to contain work they want doing:
-                # self.do_processing(request)
+                self.do_processing(request)
                 pass
             except FailGracefullyException as _:
                 pass
             except BaseException as e:
                 if on_error:
                     on_error(e)
                 else:
@@ -166,40 +169,41 @@
         self._cached_settings = None
         self._settings = settings
         self._serial: int = 0
         self._cacheddata = None
         self._cachedparams = None
         self._lock = Lock()
 
-    def process_data(self, inputdata, params) -> (Any, int, bool):
+    def process_data(self, inputdata, params: Tuple) -> (Any, int, bool):
 
         # Hold a lock for this step as we do its calculation. This allows us to share
         # a step between different pipelines so that can do the calculation only once,
         # the first thread that gets there does the work; the other benefits from the
         # cached response. The step needs to be atomic for this to work.
 
         with self._lock:
+            caching_enabled: bool = True
             was_cached_used: bool = False
             outputdata = None
             # Get a hash of the settings that relate to this step, or None if nun:
             settings = deepcopy(self.get_relevant_settings())
             # See if we can use cached results:
             if self._cacheddata is not None:
-                if params == self._cachedparams:
+                if params == self._cachedparams and caching_enabled:
                     if settings is None or settings == self._cached_settings:
                         # We can use the cached value:
                         # print("Using cached data for {}".format(type(self)))
                         outputdata = self._cacheddata
                         was_cached_used = True
             if outputdata is None:
                 # print("Calculating data for {}".format(type(self)))
                 # The cache didn't work out, so we have to do the calculation.
-                # t1 = process_time()
+                t1 = process_time()
                 outputdata = self._implementation(inputdata, params)
-                # t2 = process_time()
+                t2 = process_time()
                 # print("{:.0f} ms for {}".format((t2 - t1) * 1000, type(self).__name__))
 
                 # Cache the result in case we need it again (quite likely):
                 self._cacheddata = outputdata
                 self._cachedparams = params
                 self._cached_settings = settings
                 self._serial += 1
@@ -217,22 +221,23 @@
         """Return the settings relevant to this calculation, or None if no settings are used."""
         # Subclasses whose calculation depends on any settings MUST implement this
         # so that caching properly.
         return None
 
 
 class SpectrogramPipelineRequest(RenderingRequest):
-    def __init__(self, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
-                 frequency_range: AxisRange,
-                 screen_factors: tuple[float, float], raw_data_reader: RawDataReader):
+    def __init__(self, is_reference: bool, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
+                 frequency_range: AxisRange, screen_factors: tuple[float, float],
+                 raw_data_reader: RawDataReader):
         super().__init__(data_area, file_data)
         self.axis_time_range: AxisRange = time_range
         self.axis_frequency_range: AxisRange = frequency_range
-        self.screen_factors = screen_factors
         self.raw_data_reader = raw_data_reader
+        self.screen_factors = screen_factors
+        self.is_reference = is_reference
 
     def __str__(self):
         return "SpectrogramPipelineRequest: {} etc".format(self.data_area)
 
 
 @dataclass
 class GraphParams:
@@ -320,36 +325,38 @@
 
         if settings.fft_overlap == ADAPTIVE_FFT_OVERLAP_PERCENT:
             self.actual_fft_overlap_percent = self._calculate_auto_fft_overlap(
                 sample_rate, self.actual_fft_samples, screen_factors)
         else:
             self.actual_fft_overlap_percent = settings.fft_overlap
 
+        # print("fft_samples = {}, fft_overlap = {}".format(self.actual_fft_samples, self.actual_fft_overlap_percent))
         self.actual_fft_overlap_samples = int(self.actual_fft_overlap_percent / 100.0 * self.actual_fft_samples)
         self.step_count: int = int(self.actual_fft_samples - self.actual_fft_overlap_samples)
         half_segment_offset: int = int(self.actual_fft_samples / 2)  # Ignore the rounding error, small.
         step_time: float = (self.actual_fft_samples - self.actual_fft_overlap_samples) / sample_rate
         time_points = file_data.sample_count
         # max_segment_count: int = int((time_points - half_segment_offset) / self.step_count) + 1  # Ignore any leftover time points.
-        max_segment_count: int = int((time_points - self.actual_fft_overlap_samples) / self.step_count)  # Ignore any leftover time points.
+        max_segment_count: int = int(
+            (time_points - self.actual_fft_overlap_samples) / self.step_count)  # Ignore any leftover time points.
         time_axis_min, time_axis_max = axis_time_range.get_tuple()
         freq_axis_min, freq_axis_max = axis_frequency_range.get_tuple()
 
         # ************** Calculations relating to the time axis **************
 
         def time_to_segment_index(t: float) -> int:
             """Get the segment number corresponding to the axis time. t=0 at the centre of
             the first segment, and offsets are constant between there and subsequent
             centres. We round down intentionally."""
             segment_index = int(t / step_time)  # This rounds *down* to the nearest step
             return segment_index
 
         def segment_index_to_time(i: int) -> float:
             """Get the axis time corresponding to a segment index - which is the time at the centre of the segment."""
-            t = i * step_time # - step_time / 2
+            t = i * step_time  # - step_time / 2
             return t
 
         def segment_index_to_time_index(segment_index: int):
             """Get the index of the FIRST time value that is part of the segment."""
             # Offset for the spacing of centres - a negative time range index may result.
             time_index = int(segment_index * self.step_count - half_segment_offset)
             return time_index
@@ -361,16 +368,16 @@
             return time_index
 
         # Convert the axis ranges supplied to data index ranges, rounding outwards.
         # t=0 is the centre of the first sfft segment, so it depends in the window size.
         # This convention avoids varying time offsets as different window sizes are selected.
 
         self.first_segment_index = time_to_segment_index(time_axis_min)
-        self.last_segment_index: int = self.first_segment_index + math.ceil(    # Round outwards.
-            (time_axis_max - time_axis_min) / step_time) + 1                    # Half open.
+        self.last_segment_index: int = self.first_segment_index + math.ceil(  # Round outwards.
+            (time_axis_max - time_axis_min) / step_time) + 1  # Half open.
 
         # Allow a left and right margin to hide any edge artifacts from zooming. The
         # result is data indexes that may be outside the range of available data:
         margin: int = 10
         self.first_segment_index -= margin
         self.last_segment_index += margin
 
@@ -380,15 +387,16 @@
 
         # Convert the segment index range to a time index range. We know the time indexes are sane,
         # because we clipped the segment indexes above. These time index ranges are the range needed
         # to calculate the segments - not the time range of the segments.
         self.first_time_index_for_segs = segment_index_to_time_index(self.first_segment_index)
         # Note: (1) the last_segment_index is half open so - 1. (2) include the full index range for the previous
         # segment so that it can be calculated.
-        self.last_time_index_for_segs = segment_index_to_time_index(self.last_segment_index - 1) + self.actual_fft_samples
+        self.last_time_index_for_segs = segment_index_to_time_index(
+            self.last_segment_index - 1) + self.actual_fft_samples
 
         # Reverse calculate to the time range we actually cover, which is the segment centres.
         self.actual_time_axis_min = segment_index_to_time(self.first_segment_index)
         self.actual_time_axis_max = segment_index_to_time(self.last_segment_index - 1)  # -1 because half open range
 
         # Calculate the time index range corresponding to the actual axis values:
         self.first_time_index_for_amp = time_to_time_index(self.actual_time_axis_min)
@@ -539,23 +547,22 @@
         self._graph_params = None
         self._histogram_interface = None
         self._spectrogram_step = spectrogram_step
         self._data_reader_step = data_reader_step
         self._zoom_step = SpectrogramZoomStep(settings)
         self._bnc_step = SpectrogramBNCStep(settings)
         self._apply_colour_map_step = SpectrogramApplyColourMapStep(settings)
-        self._calc_data: SpectrogramCalcData | None = None
 
         # Remember info about the last histogram data, so we know if there is any change to it:
         self._last_histogram_data_details: tuple[int, int] | None = None
 
     def get_completion_data(self):
         return self._completion_data
 
-    def get_graph_parameters(self) -> GraphParams | None:
+    def get_graph_parameters(self) -> Optional[GraphParams]:
         return self._graph_params
 
     def do_processing(self, request: SpectrogramPipelineRequest):
         # print("do_processing {}".format(request))
 
         self._completion_data = None
 
@@ -591,22 +598,28 @@
 
         if filedata is None:
             raise ValueError("There is no spectrum data")
 
         # Note that this step is shared with the profile pipeline, to avoid needless double calculation,
         # so we need to make sure we use the same settings in each pipeline.
 
-        params = filedata_serial, calc_data, request.raw_data_reader
+        # Include the settings serial number artificially so that any settings change
+        # results in a complete rerender:
+        params = filedata_serial, request.raw_data_reader, calc_data.first_time_index_for_segs, \
+            calc_data.last_time_index_for_segs, appsettings.instance.serial_number
         (rawdata, raw_data_offset), raw_data_serial, _ = self._data_reader_step.process_data(
             None, params)
 
         if rawdata.min() == rawdata.max():
             raise FailGracefullyException("Range of raw data values is zero")
 
-        params = raw_data_serial, sample_rate, sample_count, request.screen_factors, request.axis_time_range, calc_data
+        # Include the actual fft samples and overlap to force a cache miss when they change:
+        params = raw_data_serial, sample_rate, sample_count, request.axis_time_range, \
+            calc_data.actual_fft_samples, calc_data.actual_fft_overlap_samples, calc_data.actual_fft_overlap_percent, \
+            request.is_reference
         (specdata, self._graph_params), specdata_serial, _ = \
             self._spectrogram_step.process_data((rawdata, raw_data_offset), params)
 
         del rawdata  # Allow the gc to reclaim this memory.
 
         params = raw_data_serial, height, width, request.axis_time_range, request.axis_frequency_range, \
             file_time_range, file_frequency_range, calc_data
@@ -642,24 +655,34 @@
 
         return None
 
 
 class SpectrogramDataReaderStep(PipelineStep):
     """Get the raw data we need to render the spectrogram."""
 
+    @dataclass
+    class RelevantSettings:
+        time_range: Optional[AxisRange]
+
+        def __init__(self, settings: GraphSettings):
+            self.time_range = settings.time_range
+
+    def get_relevant_settings(self) -> RelevantSettings:
+        """Get the settings subset that is relevant to this step. We will use this as a basis
+        for cache invalidation."""
+        return SpectrogramDataReaderStep.RelevantSettings(self._settings)
+
     def __init__(self, settings: GraphSettings):
         super().__init__(settings)
 
     def _implementation(self, inputdata, params):
-        calc_data: SpectrogramCalcData
-        _, calc_data, raw_data_reader = params
+        _, raw_data_reader, time_min_index, time_max_index, _ = params
 
-        time_min_index, time_max_index = calc_data.first_time_index_for_segs, calc_data.last_time_index_for_segs
         raw_data, samples_read = raw_data_reader.read_raw_data((time_min_index, time_max_index))
-        return raw_data, calc_data.first_time_index_for_segs
+        return raw_data, time_min_index
 
 
 class SpectrogramFftStep(PipelineStep):
     """Calculate a spectrogram from the raw data"""
 
     def __init__(self, settings: GraphSettings):
         super().__init__(settings)
@@ -677,16 +700,16 @@
 
     def get_relevant_settings(self) -> RelevantSettings:
         """Get the settings subset that is relevant to this step. We will use this as a basis
         for cache invalidation."""
         return SpectrogramFftStep.RelevantSettings(self._settings)
 
     def _implementation(self, inputdata, params):
-        calc_data: SpectrogramCalcData
-        previous_serial, sample_rate, file_data_samples, screen_factors, axis_time_range, calc_data = params
+        previous_serial, sample_rate, file_data_samples, axis_time_range, actual_fft_samples, \
+            actual_fft_overlap_samples, actual_fft_overlap_percent, is_reference = params
         rs = self.get_relevant_settings()
 
         # Input data is a subset of raw data from the input file, chosen to include
         # the axis range required. It consists of the data itself, and the offset from the
         # start of the data file in samples:
         data_read, data_read_offset = inputdata
         _, data_sample_count = data_read.shape
@@ -694,16 +717,16 @@
 
         # We will calculate the spectogram corresponding of the somewhat enlarged actual axis range
         # in the SpectrogramCalcData. Later on, when we zoom the data to fit the display, we will discard
         # the excess data. That means we fft the range of data indexes in the SpectrogramCalcData.
 
         # print("calculating spectrogram: {}: {}", params, inputdata.shape)
 
-        combined_spectrogram = self._do_spectrogram(data_read, sample_rate, rs.window_type,
-                                                    calc_data.actual_fft_samples, calc_data.actual_fft_overlap_samples)
+        frequencies, combined_spectrogram = self._do_spectrogram(data_read, sample_rate, rs.window_type,
+                                                                 actual_fft_samples, actual_fft_overlap_samples)
 
         # print("delta_t = {}".format(delta_t))
 
         # We now have spectrogram data corresponding to *actual* axis range, ie spanning from the middle of the
         # first segment to the middle of the last segment.
 
         # Make sure there aren't any zero values that would make log10 below fail:
@@ -711,44 +734,75 @@
             # s = np.sort(combined_spectrogram)
             arbitrary_small_number = 1E-20  # TODO review this arbitrary small number.
             combined_spectrogram = np.where(combined_spectrogram <= 0, arbitrary_small_number, combined_spectrogram)
 
         # Convert the resulting spectrogram to dB.
         # Multiplier is 10, not 20, because _do_spectrogram has already squared it.
         db_spectrogram = 10 * np.log10(combined_spectrogram)
+
+        # Apply frequency response correction if required.
+        response_data = appsettings.instance.ref_mic_response_data if is_reference else appsettings.instance.main_mic_response_data
+        if response_data is not None:
+            frequency_response = self._calculate_frequency_response(frequencies, response_data)
+            # We need to change the shape of the frequency response so that it will "broadcast" over the spectrogram:
+            frequency_response = frequency_response.reshape(-1, 1)
+            db_spectrogram -= frequency_response
+
         return db_spectrogram, \
-            GraphParams(fft_samples=calc_data.actual_fft_samples, fft_overlap=calc_data.actual_fft_overlap_percent,
+            GraphParams(fft_samples=actual_fft_samples, fft_overlap=actual_fft_overlap_percent,
                         window_type=rs.window_type)
 
     @staticmethod
-    def _do_spectrogram(data: np.ndarray, sample_rate: int, window_type, actual_fft_samples: int, overlap: int):
+    def _calculate_frequency_response(frequencies: np.ndarray, mic_response_data: Tuple[CubicSpline, float, float, float, float])\
+            -> np.ndarray:
+        """Interpolate/extrapolate the microphones response to match the frequency buckets suppled."""
+
+        cs, f_min, f_max, r_min, r_max = mic_response_data
+        interpolated = cs(frequencies)
+        # Override the spline's extrapolation with constant extrapolation (much safer):
+        for i in range(len(frequencies)):
+            f = frequencies[i]
+            if f < f_min:
+                interpolated[i] = r_min
+            if f > f_max:
+                interpolated[i] = r_max
+
+        return interpolated
+
+    @staticmethod
+    def _do_spectrogram(data: np.ndarray, sample_rate: int, window_type, actual_fft_samples: int, overlap: int) \
+            -> Tuple[np.ndarray, np.ndarray]:
         """
         Calculate the spectrogram that is the scalar sum of powers from all channels - ie,
         ignoring phase.
         """
 
         # Create a spectrogram for each channel:
         spectrograms = []
+        frequencies = None
         for d in data:
             # print("spectrogram of {} points".format(len(d)))
             # t1 = process_time()
-            _, _, spectrum_data = chunky_spectrogram(
+            fbuckets, _, spectrum_data = chunky_spectrogram(
                 d, fs=sample_rate,
                 window=window_type,
                 nperseg=actual_fft_samples,
                 noverlap=overlap,
                 nfft=None,
                 # detrend=False, # Defaults to constant.
                 return_onesided=True,
                 scaling='density',
                 # So that power dB is independent of window size.
                 # Power per Hz.
                 axis=-1,
                 mode='psd')  # psd to square the data to get power.
 
+            if frequencies is None:
+                frequencies = fbuckets
+
             # t2 = process_time()
             # print("chunked_spectrogram time: {}".format(t2 - t1))
             # t1 = process_time()
 
             spectrograms.append(spectrum_data)
 
             # t2 = process_time()
@@ -772,15 +826,15 @@
             chunk_data_target = spectrograms[0][:, samples_done:samples_done + to_sum]
             np.sum(sub_spectrograms, axis=0, out=chunk_data_target)
             samples_done += to_sum
 
         # np.sum(spectrograms, axis=0, out=combined_spectrogram)  # Sum across all axes. Hungry on memory.
 
         # return combined_spectrogram
-        return spectrograms[0]
+        return frequencies, spectrograms[0]
 
 
 class SpectrogramZoomStep(PipelineStep):
     """Zoom the data in or out to match the number of pixels we went to fill in the display."""
 
     def __init__(self, settings: GraphSettings):
         super().__init__(settings)
@@ -794,15 +848,14 @@
 
     def get_relevant_settings(self) -> RelevantSettings:
         """Get the settings subset that is relevant to this step. We will use this as a basis
         for cache invalidation."""
         return SpectrogramZoomStep.RelevantSettings(self._settings)
 
     def _implementation(self, specdata, params):
-        calc_data: SpectrogramCalcData
         previous_serial, canvas_height, canvas_width, canvas_time_range, canvas_frequency_range, \
             file_time_range, file_frequency_range, calc_data = params
 
         rs = self.get_relevant_settings()
 
         # print("zoom input {},{}".format(inputdata.min(), inputdata.max()))
 
@@ -981,21 +1034,23 @@
         # print("Bytes needed: {:,}".format(bytes_needed))
 
         if bytes_needed > self._MAX_SPECTROGRAM_MEMORY_USAGE:
             # No, we aren't going ahead with a request that needs this much memory.
             self._completion_data = True, request, None
             return
 
-        params = filedata_serial, calc_data, request.raw_data_reader
+        params = filedata_serial, request.raw_data_reader, calc_data.first_time_index_for_segs, \
+            calc_data.last_time_index_for_segs, appsettings.instance.serial_number
         (rawdata, raw_data_offset), raw_data_serial, _ = self._data_reader_step.process_data(
             None, params)
 
         # For performance, reduce the data volume to be close to the target canvas width. The
         # resulting reduced data matches the time range wanted for the axis:
-        params = filedata_serial, width, axis_trange, axis_arange, filedata_trange, filedata_arange, filedata_sample_count, calc_data
+        params = filedata_serial, width, axis_trange, axis_arange, filedata_trange, filedata_arange, \
+            filedata_sample_count, calc_data.first_time_index_for_amp, calc_data.last_time_index_for_amp
         (reduced_data, reduction_ratio), reduce_serial, _ = self._reduce_step.process_data(
             (rawdata, raw_data_offset), params)
 
         # Draw the amplitude spans into a bitmap array:
         params = reduce_serial, sample_rate, height, width, axis_trange, axis_arange, filedata_trange, filedata_arange
         line_segments, ampdata_serial, _ = self._amplitude_image_step.process_data(
             reduced_data, params)
@@ -1012,24 +1067,25 @@
     expensive downstream calculations."""
 
     def __init__(self, settings: GraphSettings):
         super().__init__(settings)
 
     def _implementation(self, input_data, params):
         calc_data: SpectrogramCalcData
-        previous_serial, canvas_width, axis_trange, axis_arange, filedata_trange, filedata_arange, filedata_samples, calc_data = params
+        previous_serial, canvas_width, axis_trange, axis_arange, filedata_trange, filedata_arange, \
+            filedata_samples, first_time_index_for_amp, last_time_index_for_amp = params
         (rawdata, input_data_offset) = input_data
         del input_data
         channels, _ = rawdata.shape
         _, raw_samples = rawdata.shape
 
         # Map the required axis range back to raw data samples supplied:
         # The time axis range corresponds to the segment range:
-        min_input_index = calc_data.first_time_index_for_amp - input_data_offset
-        max_input_index = calc_data.last_time_index_for_amp - input_data_offset
+        min_input_index = first_time_index_for_amp - input_data_offset
+        max_input_index = last_time_index_for_amp - input_data_offset
 
         # Sanity:
         min_input_index = max(0, min_input_index)
         max_input_index = min(raw_samples, max_input_index)
 
         target_bucket_count = canvas_width * 2
         slicing_factor = int((max_input_index - min_input_index) / target_bucket_count)
@@ -1111,22 +1167,22 @@
                 segment_index += 1
             last_y = ymin, ymax
 
         return line_segments
 
 
 class ProfilePipelineRequest(RenderingRequest):
-    def __init__(self, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
-                 frequency_range: AxisRange,
-                 screen_factors: tuple[float, float], raw_data_reader: RawDataReader):
+    def __init__(self, is_reference: bool, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
+                 frequency_range: AxisRange, screen_factors, raw_data_reader: RawDataReader):
         super().__init__(data_area, file_data)
         self.axis_time_range = time_range
         self.axis_frequency_range = frequency_range
-        self.screen_factors = screen_factors
         self.raw_data_reader = raw_data_reader
+        self.screen_factors = screen_factors
+        self.is_reference = is_reference
 
     def __str__(self):
         return "ProfilePipelineRequest {} etc".format(self.data_area)
 
 
 class ProfilePipeline(RenderingPipeline, PipelineHelper):
     """All steps needed to render a profile graph."""
@@ -1137,15 +1193,14 @@
         PipelineHelper.__init__(self)
 
         self._spectrogram_step = spectrogram_step
         self._data_reader_step = data_reader_step
         self._zoom_step = SpectrogramZoomStep(settings)
         self._profile_line_segment_step = ProfileLineSegmentStep(settings)
         self._data_reader_step = data_reader_step
-        self._calc_data: SpectrogramCalcData | None = None
         self._completion_data = None
 
     def do_processing(self, request: ProfilePipelineRequest) -> None:
         # Unpack some parameters:
         l, t, r, b = request.data_area
         height, width = b - t + 1, r - l + 1
         file_time_range, file_frequency_range = request.file_data.time_range, request.file_data.frequency_range
@@ -1173,25 +1228,28 @@
             # No, we aren't going ahead with a request that needs this much memory.
             self._completion_data = True, request, None, None
             return
 
         # This step is shared with the main spectrogram pipeline step, to avoid needlessly
         # calculating it twice:
 
-        params = filedata_serial, calc_data, request.raw_data_reader
+        params = filedata_serial, request.raw_data_reader, calc_data.first_time_index_for_segs, \
+            calc_data.last_time_index_for_segs, appsettings.instance.serial_number
         (rawdata, raw_data_offset), raw_data_serial, _ = self._data_reader_step.process_data(
             None, params)
 
-        params = raw_data_serial, sample_rate, sample_count, request.screen_factors, request.axis_time_range, calc_data
+        params = raw_data_serial, sample_rate, sample_count, request.axis_time_range, \
+            calc_data.actual_fft_samples, calc_data.actual_fft_overlap_samples, calc_data.actual_fft_overlap_percent, \
+            request.is_reference
         (specdata, self._graph_params), specdata_serial, spectrogram_serial = \
             self._spectrogram_step.process_data((rawdata, raw_data_offset), params)
 
         del rawdata  # Allow the gc to reclaim this memory.
 
-        params = spectrogram_serial, height, width, request.axis_time_range, request.axis_frequency_range, \
+        params = raw_data_serial, height, width, request.axis_time_range, request.axis_frequency_range, \
             file_time_range, file_frequency_range, calc_data
         zoomed_specdata, zoomed_serial, _ = self._zoom_step.process_data(specdata, params)
 
         # Create a series of points for drawing the profile:
         params = zoomed_serial, height, width
         (profile_points, vmin, vmax), specdata_serial, _ = self._profile_line_segment_step.process_data(
             zoomed_specdata, params)
```

### Comparing `batogram-1.0.6/batogram/rootwindow.py` & `batogram-1.0.7/batogram/rootwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,17 +126,17 @@
             # We have to tell the parent frame to reduce size, it doesn't do this
             # automatically when we remove the settings frames sadly:
             self._parent.configure(height=0, width=100)  # Width has to be non zero for some reason.
 
 
 class GraphPipelines(NamedTuple):
     """A tuple of rendering pipelines relating to a set of graphs."""
-    amplitude: AmplitudePipeline | None
-    spectrogram: SpectrogramPipeline | None
-    profile: ProfilePipeline | None
+    amplitude: Optional[AmplitudePipeline]
+    spectrogram: Optional[SpectrogramPipeline]
+    profile: Optional[ProfilePipeline]
 
 
 class PanelFrame(tk.Frame):
     """This is a Frame which contains the set of graphs relating to the main or the reference data."""
 
     def __init__(self, parent, root, pipelines, data_context, settings, settings_frame, pad, is_reference):
         super().__init__(parent)
@@ -169,15 +169,15 @@
         self._spectrogram_frame.set_scroller_t(self._time_scroller)
         self._time_scroller.grid(row=4, column=col, sticky="ew", padx=pad)
 
         self._readout_frame = ReadoutFrame(self)
         self._readout_frame.grid(row=6, column=col, pady=pad, sticky='we')
 
         col = 1
-        self._profile_frame = ProfileGraphFrame(self, root, pipelines.profile, self._dc, self._settings)
+        self._profile_frame = ProfileGraphFrame(self, root, pipelines.profile, self._dc, self._settings, is_reference=is_reference)
         self._profile_frame.grid(row=3, column=col, sticky='ns')
 
         col = 2
         frequency_scroller = tk.Scrollbar(self, orient='vertical', jump=True, repeatdelay=0)
         frequency_scroller.grid(row=3, column=col, sticky="ns")
         self._spectrogram_frame.set_scroller_f(frequency_scroller)
 
@@ -261,15 +261,16 @@
                 if range_f.min + delta_f < freq_min:
                     delta_f = -(range_f.min - freq_min)
 
         limited_range_t = AxisRange(range_t.min + delta_t, range_t.max + delta_t)
         limited_range_f = AxisRange(range_f.min + delta_f, range_f.max + delta_f)
 
         self.on_rescale_handler(limited_range_t, limited_range_f,
-                                add_breadcrumb=add_breadcrumb, draw_scope=DrawableFrame.DRAW_ALL)
+                                add_breadcrumb=add_breadcrumb,
+                                draw_scope=DrawableFrame.DRAW_ALL)
 
     def draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
         # Update the settings to match the *actual* new axis ranges:
         self._settings.time_range = self._dc.time_range
         self._settings.frequency_range = self._dc.frequency_range
         self._settings.on_app_modified_settings()
 
@@ -382,49 +383,52 @@
 
     def on_page_down_key(self, event):
         self._spectrogram_frame.fview(tk.SCROLL, 1, tk.UNITS)
 
     def on_shift_page_down_key(self, event):
         self._spectrogram_frame.fview(tk.SCROLL, 1, tk.PAGES)
 
+    def on_home_key(self, event):
+        self.on_home_button()
+
 
 class DataContext:
     """This class contains data used by a graph pane, including raw file data and axis ranges."""
 
     DEFAULT_TIME_RANGE = AxisRange(rmin=0, rmax=30)
     DEFAULT_FREQUENCY_RANGE = AxisRange(rmin=0, rmax=192000)
     DEFAULT_AMPLITUDE_RANGE = AxisRange(rmin=-1, rmax=1)
 
     def __init__(self):
-        self.afs: AudioFileService | None = None
+        self.afs: Optional[AudioFileService] = None
         self.breadcrumb_service = BreadcrumbService()
         self.time_range: Optional[AxisRange] = None
         self.frequency_range: Optional[AxisRange] = None
         self.amplitude_range: Optional[AxisRange] = None
         self.reset()
 
     def reset(self):
         self._set_afs(None)
         self.time_range = self.DEFAULT_TIME_RANGE
         self.frequency_range = self.DEFAULT_FREQUENCY_RANGE
         self.amplitude_range = self.DEFAULT_AMPLITUDE_RANGE
 
-    def _set_afs(self, afs: AudioFileService | None):
+    def _set_afs(self, afs: Optional[AudioFileService]):
         # If we already have an afs, close it:
         if self.afs is not None:
             self.afs.close()
         self.afs = afs
 
     def get_ranges(self):
         return self.time_range, self.frequency_range, self.amplitude_range
 
-    def get_afs(self) -> AudioFileService | None:
+    def get_afs(self) -> Optional[AudioFileService]:
         return self.afs
 
-    def get_afs_data(self) -> AudioFileService.RenderingData | None:
+    def get_afs_data(self) -> Optional[AudioFileService.RenderingData]:
         return self.afs.get_rendering_data() if self.afs is not None else None
 
     def update_from_af(self, afs: AudioFileService):
         self._set_afs(afs)
         af_data = afs.get_rendering_data()
         self.amplitude_range = af_data.amplitude_range
         self.time_range = af_data.time_range
@@ -499,14 +503,15 @@
         self.bind('<Shift-Up>', self._main_pane.on_shift_up_key)
         self.bind('<Down>', self._main_pane.on_down_key)
         self.bind('<Shift-Down>', self._main_pane.on_shift_down_key)
         self.bind('<Prior>', self._main_pane.on_page_up_key)
         self.bind('<Shift-Prior>', self._main_pane.on_shift_page_up_key)
         self.bind('<Next>', self._main_pane.on_page_down_key)
         self.bind('<Shift-Next>', self._main_pane.on_shift_page_down_key)
+        self.bind('<Home>', self._main_pane.on_home_key)
 
         # Allow tk to work out the size of things before we try to draw any graphs:
         self.update_idletasks()
 
         self._main_pane.draw()
         self._ref_pane.draw()
 
@@ -583,40 +588,40 @@
     def _create_menus(self):
         # Set up the menus (see https://tkdocs.com/tutorial/menus.html):
         self.option_add('*tearOff', False)
         menubar = tk.Menu(self)
         self['menu'] = menubar
 
         self._menu_file = tk.Menu(menubar)
-        menubar.add_cascade(menu=self._menu_file, label=MENU_TEXT_FILE)
-        self._menu_file.add_command(label=MENU_TEXT_OPEN_MAIN, command=self._open_main_file)
+        menubar.add_cascade(menu=self._menu_file, label=MENU_TEXT_FILE, underline=0)
+        self._menu_file.add_command(label=MENU_TEXT_OPEN_MAIN, command=self._open_main_file, underline=0)
         self._menu_file.entryconfigure(MENU_TEXT_OPEN_MAIN, accelerator='Ctrl+O')
         self.bind("<Control-o>", self._open_main_file_event)
         self._menu_recent_main = tk.Menu(self._menu_file)
         self._menu_file.add_cascade(menu=self._menu_recent_main, label=MENU_TEXT_OPEN_RECENT_MAIN)
         self._populate_file_history(self._menu_recent_main, self._main_historian, self._do_open_main_file)
-        self._menu_file.add_command(label=MENU_TEXT_CLOSE_MAIN, command=self._close_main_file_event)
+        self._menu_file.add_command(label=MENU_TEXT_CLOSE_MAIN, command=self._close_main_file_event, underline=0)
         self._menu_file.add_separator()
 
-        self._menu_file.add_command(label=MENU_TEXT_OPEN_REF, command=self._open_ref_file)
+        self._menu_file.add_command(label=MENU_TEXT_OPEN_REF, command=self._open_ref_file, underline=5)
         self._menu_file.entryconfigure(MENU_TEXT_OPEN_REF, accelerator='Ctrl+R')
         self.bind("<Control-r>", self._open_ref_file_event)
         self._menu_recent_ref = tk.Menu(self._menu_file)
         self._menu_file.add_cascade(menu=self._menu_recent_ref, label=MENU_TEXT_OPEN_RECENT_REF)
         self._populate_file_history(self._menu_recent_ref, self._ref_historian, self._do_open_ref_file)
         self._menu_file.add_command(label=MENU_TEXT_CLOSE_REF, command=self.close_ref_file_event)
         self._menu_file.add_separator()
 
         # self._menu_file.add_command(label=MENU_TEXT_SAVE, command=self.save_files_as)
         # self._menu_file.add_separator()
-        self._menu_file.add_command(label=MENU_TEXT_EXIT, command=self.exit)
+        self._menu_file.add_command(label=MENU_TEXT_EXIT, command=self.exit, underline=1)
         self._menu_file.entryconfigure(MENU_TEXT_EXIT, accelerator='Ctrl+X')
         self.bind("<Control-x>", self.exit_event)
 
-        menubar.add_command(label=MENU_TEXT_SETTINGS, command=self._show_settings)
+        menubar.add_command(label=MENU_TEXT_SETTINGS, command=self._show_settings, underline=0)
 
         menubar.add_command(label=MENU_TEXT_ABOUT, command=self._show_about)
 
         self.enable_menu_items()
 
     @staticmethod
     def _populate_file_history(parent_menu_item, historian, method):
@@ -651,22 +656,24 @@
         ('audio files', '*.wav *.WAV'),
         ('All files', '*.*')
     )
 
     def _open_main_file_event(self, _):
         self._open_main_file()
 
-    def _open_file_dialog(self, title: str):
+    def _open_file_dialog(self, title: str) -> str:
         initialdir = None
         if self._first_file_open:
             self._first_file_open = False
+            # Only do this the first time a file is opened; thereafter, the dialog
+            # remembers where the user last navigated it to:
             initialdir = appsettings.instance.data_directory
 
-        filepath = tk.filedialog.askopenfilename(title=title, filetypes=self.filetypes,
-                                                 initialdir=initialdir)
+        filepath: str = tk.filedialog.askopenfilename(title=title, filetypes=self.filetypes,
+                                                      initialdir=initialdir)
         return filepath
 
     def _open_main_file(self):
         filepath = self._open_file_dialog("Open an audio file")
         if filepath:
             self._do_open_main_file(filepath)
```

### Comparing `batogram-1.0.6/batogram/spectrogramgraphframe.py` & `batogram-1.0.7/batogram/spectrogramgraphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
-from typing import Tuple
+from typing import Tuple, Optional
 
 from .constants import MAIN_SPECTROGAM_COMPLETER_EVENT, FONT_SIZE, MIN_F_RANGE, MIN_T_RANGE
 from . import layouts
 from .audiofileservice import RawDataReader, AudioFileService
 from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
 from .spectrogrammouseservice import SpectrogramMouseService, CursorMode
@@ -45,25 +45,25 @@
     def notify_draw_complete(self):
         self._mouse_service.notify_draw_complete()
 
 
 class SpectrogramGraphFrame(GraphFrame):
     """A graph frame containing a spectrogram."""
 
-    def __init__(self, parent: "PanelFrame", root, pipeline, data_context, settings, initial_cursor_mode, is_reference=False):
+    def __init__(self, parent: "PanelFrame", root, pipeline, data_context, settings, initial_cursor_mode, is_reference):
         super().__init__(parent, root, pipeline, data_context, settings)
 
         self._is_reference = is_reference
         self._canvas = SpectrogramCanvas(self, height=100, width=100, initial_cursor_mode=initial_cursor_mode)
         self._canvas.grid(row=0, column=0, sticky='nesw')
         self.columnconfigure(0, weight=1)
         self.rowconfigure(0, weight=1)
 
         self._layout = None
-        self._histogram_interface: HistogramInterface | None = None
+        self._histogram_interface: Optional[HistogramInterface] = None
 
         # Scrollers are (individually) optional:
         self._scroller_t = None
         self._scroller_f = None
 
         self._parent = parent
 
@@ -133,15 +133,15 @@
             self._update_frequency_scroller(frequency_range, afs_data.frequency_range)
             if self._pipeline:
                 # Kick off the pipeline which will create a spectrogram in another thread,
                 # and complete by generating an event that will finish drawing the graph in
                 # this thread.
                 self._completer = graph_completer
                 screen_factors = self._parent.get_screen_factors()
-                request = self._get_pipeline_request(afs_data, data_area, time_range, frequency_range, screen_factors,
+                request = self._get_pipeline_request(self._is_reference, afs_data, data_area, time_range, frequency_range, screen_factors,
                                                      self._dc.get_afs())
                 self._pipeline.submit(request,
                                       lambda: self.event_generate(MAIN_SPECTROGAM_COMPLETER_EVENT),
                                       self._pipeline_error_handler)
         else:
             # No data, make the sliders full length:
             self._update_time_scroller(AxisRange(0, 1), AxisRange(0, 1))
@@ -165,17 +165,17 @@
             self._canvas.config(cursor="fleur")
         else:
             self._canvas.config(cursor="")
 
         self._canvas.set_cursor_mode(mode)
 
     @staticmethod
-    def _get_pipeline_request(data, data_area, time_range, frequency_range, screen_factors: tuple[float, float],
+    def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range, screen_factors: tuple[float, float],
                               raw_data_reader: RawDataReader):
-        request = SpectrogramPipelineRequest(data_area, data, time_range, frequency_range, screen_factors, raw_data_reader)
+        request = SpectrogramPipelineRequest(is_reference, data_area, data, time_range, frequency_range, screen_factors, raw_data_reader)
         return request
 
     def _do_completer(self, _):
         # A bit of a hack because tkinter doesn't seem to allow data to be attached to an event:
         completer = self._completer
         if completer:
             memory_limit_hit, request, image, histogram, auto_vrange = self._pipeline.get_completion_data()  # Can be None.
@@ -377,31 +377,24 @@
         self._parent.on_scroll_handler(0, delta_f, range_t, range_f)
 
     def set_preset_time_range(self, sign: int):
         """Zoom the time range in or out, centered on the current range.
         Positive sign increases the axis range, ie zoom out.
         """
 
-        time_range, _ = self._layout.get_data_ranges()
-        centre = (time_range.min + time_range.max) / 2
-        span = time_range.max - time_range.min
+        new_time_range: AxisRange = self._layout.calc_preferred_time_range(sign)
 
-        if sign > 0:
-            span *= 1.2
-        else:
-            span *= 0.8
-
-        if span < MIN_T_RANGE:
+        if new_time_range.max - new_time_range.min < MIN_T_RANGE:
             # Allow them to zoom back out again, to avoid getting stuck.
             if sign < 0:
                 print("Ignoring insane zoom in.")
                 return False  # Insane zoom requested, ignore it.
 
         _, frequency_range = self._layout.get_data_ranges()
-        self._parent.on_rescale_handler(AxisRange(centre - span / 2, centre + span / 2), frequency_range)
+        self._parent.on_rescale_handler(new_time_range, frequency_range)
 
     def _update_time_scroller(self, axis_range, file_range):
         if self._scroller_t is None:
             return
 
         # Set the time scroller so that the bar represents the visible part of the data,
         # scaled to the range 0 to 1.0.
```

### Comparing `batogram-1.0.6/batogram/spectrogrammouseservice.py` & `batogram-1.0.7/batogram/spectrogrammouseservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 
 from enum import Enum
 from timeit import default_timer as timer
-from typing import Tuple
+from typing import Tuple, Optional
 
 # Grey, so its visible against black and white.
 DRAG_RECTANGLE_COLOUR = "grey"
 DRAG_LINE_COLOUR = "grey"
 ARROW_SHAPE = (16, 20, 6)
 
 
@@ -65,17 +65,17 @@
         self._state: MouseState = MouseState.START
         self._start_position = None
         self._rect = None
         self._line = None
         self._line1 = None
         self._line2 = None
         self._last_wheel_time = timer()
-        self._canvas_height: int | None = None
-        self._canvas_width: int | None = None
-        self._last_drag_mode: DragMode | None = None
+        self._canvas_height: Optional[int] = None
+        self._canvas_width: Optional[int] = None
+        self._last_drag_mode: Optional[DragMode] = None
 
         # Left mouse button:
         canvas.bind('<ButtonPress-1>', self._on_button1_press)
         canvas.bind('<Shift-ButtonPress-1>', self._on_button1_press)
         canvas.bind('<ButtonRelease-1>', self._on_button1_release)
         canvas.bind('<Shift-ButtonRelease-1>', self._on_shift_button1_release)
         canvas.bind('<B1-Motion>', self._on_button1_move)
@@ -355,15 +355,15 @@
         if self._line2 is not None:
             self._canvas.delete(self._line2)
             self._line2 = None
         if self._line is not None:
             self._canvas.delete(self._line)
             self._line = None
 
-    def _get_drag_mode(self, event, is_shift: bool) -> DragMode | None:
+    def _get_drag_mode(self, event, is_shift: bool) -> Optional[DragMode]:
         """
         Decide if frequency or time is clamped, depending on the current direction
         of the mouse offset.
         """
 
         # Holding down shift keeps to the current mode, if there is one:
         if is_shift and self._last_drag_mode is not None:
```

### Comparing `batogram-1.0.6/batogram/validatingwidgets.py` & `batogram-1.0.7/batogram/validatingwidgets.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.6/batogram/wavfileparser.py` & `batogram-1.0.7/batogram/wavfileparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import io
 import numpy as np
 
 from dataclasses import dataclass
-from typing import List, Callable, Any, Tuple
+from typing import List, Callable, Any, Tuple, Optional
 from .external.guano import GuanoFile
 
 
 class WavFileError(Exception):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, *kwargs)
 
@@ -55,27 +55,27 @@
         data: "WavFileParser.Data"
         guanodata: GuanoFile
 
     def __init__(self, filepath: str):
         self._filepath = filepath
         self._f = None
         self._start_of_data = None      # File offset to where data starts.
-        self._fmt_header: WavFileParser.Header | None = None
+        self._fmt_header: Optional[WavFileParser.Header] = None
 
-    def open(self) -> np.ndarray | None:
+    def open(self) -> Chunks:
         # Binary mode:
         self._f = open(self._filepath, "rb")
         return self._read_chunks()
 
     def close(self):
         if self._f is not None:
             self._f.close()
         self._f = None
 
-    def _read_chunks(self,) -> np.ndarray | None:
+    def _read_chunks(self,) -> Chunks:
         """Read all the metadata we can from the wav file. Call read_data() later to get the actual data."""
 
         # See http://soundfile.sapp.org/doc/WaveFormat/
         # See https://github.com/riggsd/guano-spec/blob/master/guano_specification.md
 
         self._f.seek(0, io.SEEK_END)
         file_len = self._f.tell()
@@ -158,15 +158,15 @@
         if excess_data > 0:
             print("Discarding {} excess bytes from the end of fmt".format(excess_data))
             self._f.read(excess_data)
 
         return WavFileParser.Header(num_channels=num_channels, sample_rate_hz=sample_rate_hz,
                                     bits_per_sample=bits_per_sample)
 
-    def _skim_data(self, header: Header) -> Data | None:
+    def _skim_data(self, header: Header) -> Optional[Data]:
         """Process the data chunk without storing any of the data."""
 
         data_byte_count = self._read_int32("ChunkSize")
 
         # Note where the data starts so we can come back for it later.
         self._start_of_data = self._f.tell()
 
@@ -203,15 +203,15 @@
         # to seek to the end of data chunk now to not confused the caller:
         self._f.seek(self._start_of_data + data_byte_count)
 
         return WavFileParser.Data(actual_sample_count=actual_sample_count,
                                   data_range=(min_value, max_value),
                                   data_byte_count=data_byte_count)
 
-    def read_data(self, index_range: tuple[int, int]) -> tuple[np.ndarray | None, int]:
+    def read_data(self, index_range: tuple[int, int]) -> tuple[Optional[np.ndarray], int]:
         """Read the request range of data (half open), and return the data and actual count read."""
 
         dt = None
         if self._fmt_header.bits_per_sample == 8:
             dt = np.dtype(np.uint8)
         elif self._fmt_header.bits_per_sample == 16:
             dt = np.dtype(np.int16)
@@ -244,15 +244,15 @@
 
         if self._fmt_header.num_channels > 1:
             actual_samples_read = int(actual_values_read / self._fmt_header.num_channels)
             data = data.reshape((actual_samples_read, self._fmt_header.num_channels))
 
         return data, actual_samples_read
 
-    def _read_guan(self) -> GuanoFile | None:
+    def _read_guan(self) -> Optional[GuanoFile]:
         # https://www.wildlifeacoustics.com/SCHEMA/GUANO.html
         # https://github.com/riggsd/guano-py/blob/master/guano.py
 
         chunk_size_bytes = self._read_int32("ChunkSize")
         metadata = self._f.read(chunk_size_bytes)
         gf = GuanoFile.from_string(metadata)
 
@@ -268,30 +268,30 @@
         self._f.seek(t + chunk_size)
 
     def _check_value(self, fieldname: str, value, check: Callable, text: str):
         if not check(value):
             raise WavFileError("Unexpected value for {} in {}: found {}: {}"
                                .format(fieldname, self._filepath, value, text))
 
-    def _read_int32(self, fieldname: str, expected: int | None = None) -> int:
+    def _read_int32(self, fieldname: str, expected: Optional[int] = None) -> int:
         b = self._f.read(4)
         n = int.from_bytes(b, byteorder='little')
         if expected is not None and n != expected:
             raise WavFileError("Unexpected value for {} in {}: found {}, expected {}"
                                .format(fieldname, self._filepath, n, expected))
         return n
 
-    def _read_int16(self, fieldname: str, expected: int | None = None) -> int:
+    def _read_int16(self, fieldname: str, expected: Optional[int] = None) -> int:
         b = self._f.read(2)
         n = int.from_bytes(b, byteorder='little')
         if expected is not None and n != expected:
             raise WavFileError("Unexpected value for {} in {}: found {}, expected {}"
                                .format(fieldname, self._filepath, n, expected))
         return n
 
-    def _read_text_bytes(self, length, fieldname, expected: bytes | None = None) -> List[bytes]:
+    def _read_text_bytes(self, length, fieldname, expected: Optional[bytes] = None) -> List[bytes]:
         b = self._f.read(length)
         if expected is not None and b != expected:
             raise WavFileError("Unexpected value for {} in {}: found {}, expected {}"
                                .format(fieldname, self._filepath, b, expected))
 
         return b
```

### Comparing `batogram-1.0.6/batogram.egg-info/PKG-INFO` & `batogram-1.0.7/batogram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.6
+Version: 1.0.7
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,21 +26,23 @@
 Keywords: bat,spectrogram,chiropterology,fourier,ultrasonic,ultrasound,echo,GUANO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-batogram
+Batogram
 ========
 
+![Screen Shot](docs/screenshot.png "Screen Shot")
+
 Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
@@ -54,30 +56,31 @@
 
 ### Windows
 
 There are currently two approaches to installing Batogram on Windows. The first and simplest
 method is as follows:
 
 * Download a Batogram executable for Windows from Github. Available releases are listed 
-[here](https://github.com/jmears63/batogram/releases).
+[here](https://github.com/jmears63/batogram/releases). You need the file named batogram.exe, listed
+under Assets.
 * Probably Windows Defender will warn you of the danger of downloading such files from unknown
 sources. Assess the risk and decide if you going ahead. Assuming you are, proceed to the
 next step.
 * Copy the downloaded executable to your Windows desktop, so that you can find it when you want it.
 * Double click it on the desktop to run it. The first time you run it, it will take a little longer to start 
 up than usual. You will notice a command window launched alongside Batogram - ignore it. This is to
 aid debugging, and will be removed in a future release.
 
 The second installation method is to install Python on your Windows computer, and then follow the 
 same steps as the Linux installation. If you take this route, I assume you know what you are doing.
 
 ### Linux
 
 On Linux, Batogram is currently installed from the command line using pip, as below.
-You need to have Python 3.10 as a minimum.  
+You need to have Python 3.9 as a minimum.  
 
     # Create a virtual environment at a convenient location in your home directory:
     mkdir ~/batogram
     cd batogram
     python3 -m venv venv
     source venv/bin/activate
```

### Comparing `batogram-1.0.6/batogram.egg-info/SOURCES.txt` & `batogram-1.0.7/batogram.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 batogram/assets/arrow-right-circle-line.png
 batogram/assets/arrow-right-line.png
 batogram/assets/batogram.png
 batogram/assets/download-line.png
 batogram/assets/drag-move-2-line.png
 batogram/assets/expand-left-right-fill.png
 batogram/assets/expand-up-down-fill.png
+batogram/assets/fullscreen-line.png
 batogram/assets/home-4-line.png
 batogram/assets/zoom-in-line.png
 batogram/colour_maps/CET-L01.csv
 batogram/colour_maps/CET-L03.csv
 batogram/colour_maps/CET-L05.csv
 batogram/colour_maps/CET-L06.csv
 batogram/colour_maps/CET-L07.csv
```

### Comparing `batogram-1.0.6/pyproject.toml` & `batogram-1.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "batogram"
-version = "1.0.6"
+version = "1.0.7"   # Set this to the version number during release, and revert to 0.0.0 between releases.
 authors = [
     {name = "John Mears", email = "john+batogram@themears.co.uk"},
 ]
 description = "Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls."
 readme = "README.md"
-requires-python = ">=3.10"      # To support | with type hints.
+requires-python = ">=3.9"
 keywords = ["bat", "spectrogram", "chiropterology", "fourier", "ultrasonic", "ultrasound", "echo", "GUANO"]
 license = {file = "LICENSE"}
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
```

