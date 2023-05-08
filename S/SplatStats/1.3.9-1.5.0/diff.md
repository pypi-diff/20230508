# Comparing `tmp/SplatStats-1.3.9.tar.gz` & `tmp/SplatStats-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-1.3.9.tar", last modified: Thu Mar 30 04:24:56 2023, max compression
+gzip compressed data, was "SplatStats-1.5.0.tar", last modified: Mon May  8 00:36:46 2023, max compression
```

## Comparing `SplatStats-1.3.9.tar` & `SplatStats-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-03-30 04:24:56.029718 SplatStats-1.3.9/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-09-17 20:12:28.000000 SplatStats-1.3.9/LICENSE
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-03-30 04:24:56.029718 SplatStats-1.3.9/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6368 2023-01-25 04:16:56.000000 SplatStats-1.3.9/README.md
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-03-30 04:24:56.025717 SplatStats-1.3.9/SplatStats/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10828 2023-03-14 03:30:29.000000 SplatStats-1.3.9/SplatStats/Battle.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10240 2022-11-24 03:14:30.000000 SplatStats-1.3.9/SplatStats/Player.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2744 2023-03-14 23:56:09.000000 SplatStats-1.3.9/SplatStats/StatInk.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2477 2022-11-01 00:29:50.000000 SplatStats-1.3.9/SplatStats/Team.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      896 2023-03-19 21:08:44.000000 SplatStats-1.3.9/SplatStats/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       21 2023-03-30 04:24:55.000000 SplatStats-1.3.9/SplatStats/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6148 2022-12-04 18:34:39.000000 SplatStats-1.3.9/SplatStats/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13883 2023-03-30 04:23:43.000000 SplatStats-1.3.9/SplatStats/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     5393 2023-02-27 04:39:12.000000 SplatStats-1.3.9/SplatStats/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4137 2023-03-14 03:19:39.000000 SplatStats-1.3.9/SplatStats/files.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8663 2023-02-17 22:36:56.000000 SplatStats-1.3.9/SplatStats/parsers.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    46277 2023-03-09 20:52:36.000000 SplatStats-1.3.9/SplatStats/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1428 2022-09-29 02:14:29.000000 SplatStats-1.3.9/SplatStats/plotsAux.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1709 2022-11-14 00:32:41.000000 SplatStats-1.3.9/SplatStats/plotsTeam.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9349 2023-03-22 00:31:54.000000 SplatStats-1.3.9/SplatStats/statInkConstants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     7047 2023-03-21 00:53:41.000000 SplatStats-1.3.9/SplatStats/statInkPlots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6574 2023-03-24 03:36:50.000000 SplatStats-1.3.9/SplatStats/statInkStats.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13623 2022-11-13 20:31:57.000000 SplatStats-1.3.9/SplatStats/stats.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-03-30 04:24:56.029718 SplatStats-1.3.9/SplatStats.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-03-30 04:24:55.000000 SplatStats-1.3.9/SplatStats.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      607 2023-03-30 04:24:55.000000 SplatStats-1.3.9/SplatStats.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-03-30 04:24:55.000000 SplatStats-1.3.9/SplatStats.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      159 2023-03-30 04:24:55.000000 SplatStats-1.3.9/SplatStats.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       11 2023-03-30 04:24:55.000000 SplatStats-1.3.9/SplatStats.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-03-30 04:24:56.029718 SplatStats-1.3.9/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1251 2023-02-19 19:16:43.000000 SplatStats-1.3.9/setup.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-08 00:36:46.681797 SplatStats-1.5.0/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-09-17 20:12:28.000000 SplatStats-1.5.0/LICENSE
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-08 00:36:46.681797 SplatStats-1.5.0/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6368 2023-01-25 04:16:56.000000 SplatStats-1.5.0/README.md
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-08 00:36:46.673797 SplatStats-1.5.0/SplatStats/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10828 2023-03-14 03:30:29.000000 SplatStats-1.5.0/SplatStats/Battle.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10240 2022-11-24 03:14:30.000000 SplatStats-1.5.0/SplatStats/Player.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2750 2023-04-05 03:12:55.000000 SplatStats-1.5.0/SplatStats/StatInk.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2477 2022-11-01 00:29:50.000000 SplatStats-1.5.0/SplatStats/Team.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      896 2023-03-19 21:08:44.000000 SplatStats-1.5.0/SplatStats/__init__.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       21 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats/_version.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6148 2022-12-04 18:34:39.000000 SplatStats-1.5.0/SplatStats/auxiliary.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13947 2023-05-08 00:35:21.000000 SplatStats-1.5.0/SplatStats/colors.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     5393 2023-02-27 04:39:12.000000 SplatStats-1.5.0/SplatStats/constants.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4137 2023-03-14 03:19:39.000000 SplatStats-1.5.0/SplatStats/files.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8663 2023-02-17 22:36:56.000000 SplatStats-1.5.0/SplatStats/parsers.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    46328 2023-04-06 00:24:58.000000 SplatStats-1.5.0/SplatStats/plots.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1428 2022-09-29 02:14:29.000000 SplatStats-1.5.0/SplatStats/plotsAux.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1709 2022-11-14 00:32:41.000000 SplatStats-1.5.0/SplatStats/plotsTeam.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10176 2023-04-06 04:24:33.000000 SplatStats-1.5.0/SplatStats/statInkConstants.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10543 2023-04-28 00:57:38.000000 SplatStats-1.5.0/SplatStats/statInkPlots.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8511 2023-04-06 03:09:35.000000 SplatStats-1.5.0/SplatStats/statInkStats.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13660 2023-04-13 18:00:01.000000 SplatStats-1.5.0/SplatStats/stats.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-08 00:36:46.681797 SplatStats-1.5.0/SplatStats.egg-info/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      607 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/SOURCES.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/dependency_links.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      159 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/requires.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       11 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/top_level.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-05-08 00:36:46.681797 SplatStats-1.5.0/setup.cfg
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1251 2023-02-19 19:16:43.000000 SplatStats-1.5.0/setup.py
```

### Comparing `SplatStats-1.3.9/LICENSE` & `SplatStats-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/PKG-INFO` & `SplatStats-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.3.9
+Version: 1.5.0
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.3.9/README.md` & `SplatStats-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/Battle.py` & `SplatStats-1.5.0/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/Player.py` & `SplatStats-1.5.0/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/StatInk.py` & `SplatStats-1.5.0/SplatStats/StatInk.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,8 +50,9 @@
         df['power'] = df['power'].fillna(naInt)
         df['win'] = [True if (i=='alpha') else False for i in df['win']]
         # Cleanup colors -----------------------------------------------------
         df['alpha-color'] = [f'#{c}' if type(c) is str else naColor for c in df['alpha-color']]
         df['bravo-color'] = [f'#{c}' if type(c) is str else naColor for c in df['bravo-color']]
         # Coherce into data types and return dataframe -----------------------
         df.astype(ink.SPLATSTATS_DTYPES, copy=False)
-        return df
+        return df
+
```

### Comparing `SplatStats-1.3.9/SplatStats/Team.py` & `SplatStats-1.5.0/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/__init__.py` & `SplatStats-1.5.0/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/auxiliary.py` & `SplatStats-1.5.0/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/colors.py` & `SplatStats-1.5.0/SplatStats/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 # Splatfest -------------------------------------------------------------------
 ROCK_PAPER_SCISSORS_S3      = ('#413BBA', '#BEB013', '#C03E3E', '#35BA49')
 GEAR_GRUB_FUN_S3            = ('#8A19F7', '#BE7118', '#28C05E', '#3F2CD2')
 GRASS_FIRE_WATER_S3         = ('#1BA974', '#DA4514', '#002AFF', '#FFFF00')
 SPICY_SWEET_SOUR_S3         = ('#AD5438', '#9A6FCC', '#A5B533', '#00A2E8')
 DARK_MILK_WHITE_S3          = ('#3D1F7A', '#995935', '#D6BF8F', '#FFFF00')
 NESSIE_ALIENS_BIGFOOT_S3    = ('#118F32', '#793199', '#A1482B', '#0935A6')
+POWER_WISDOM_COURAGE_S3     = ('#AB2A5C', '#488DB5', '#03A65F')
 # Return of the Mammalians ----------------------------------------------------
 ORANGE_V_BLUE_S3            = ('#EE8711', '#0943F0', '#81DE17')
 YELLOW_V_INDIGO_S3          = ('#DEC109', '#531BBA', '#C920B7')
 GREEN_V_BLUE_S3             = ('#51C71B', '#2120CC', '#C920B7')
 SODA_V_MAGENTA_S3           = ('#AEF4F0', '#DD0DD3', '#C6D314')
 LBLUE_V_BLUE_S3             = ('#14BBE7', '#285EEA', '#C920B7')
 BLUE_V_MAGENTA_S3           = ('#1B18D7', '#DD0DD3', '#C6D314')
```

### Comparing `SplatStats-1.3.9/SplatStats/constants.py` & `SplatStats-1.5.0/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/files.py` & `SplatStats-1.5.0/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/parsers.py` & `SplatStats-1.5.0/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/plots.py` & `SplatStats-1.5.0/SplatStats/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 
 import squarify
+import pandas as pd
 import numpy as np
 import seaborn as sns
 from pywaffle import Waffle
 import matplotlib.pyplot as plt
 from math import radians, log10
 from matplotlib.patches import Rectangle
 import SplatStats.constants as cst
@@ -806,15 +807,15 @@
         legendDict (dict, optional): Dictionary for labels (see pywaffle's docs). Defaults to { 'loc': 'upper left', 'bbox_to_anchor': (1, 1), 'ncol': 1, 'framealpha': 0, 'fontsize': 10 }.
 
     Returns:
         (fix, ax): Matplotlib's fig and ax objects.
     """    
     (fig, ax) = figAx
     # Aggregate ---------------------------------------------------------------
-    df = playerHistory.groupby(grouping).agg(function)
+    df = playerHistory[[grouping, stat]].groupby(grouping).agg(function)
     cols = [
         i+aux.alphaToHex(alpha) for i in colors[:len(df.index)]
     ]
     # Waffle ------------------------------------------------------------------
     Waffle.make_waffle(
         ax=ax,
         rows=rows, 
@@ -869,15 +870,15 @@
         xRange (tuple, optional): Values to map onto the rRange values. Defaults to (0, 10).
         colors (_type_, optional): List of hex colors for bars. Defaults to clr.ALL_COLORS.
 
     Returns:
         (fix, ax): Matplotlib's fig and ax objects.
     """
     # Gather data -------------------------------------------------------------
-    df = playerHistory.groupby(cat).agg(aggFun)
+    df = playerHistory[[cat, stat]].groupby(cat).agg(aggFun)
     df.sort_values(by=[stat], inplace=True)
     catVals = list(df[stat])
     # Generate chart ----------------------------------------------------------
     (fig, ax) = polarBarChart(
         xVals=list(df.index), yVals=catVals,
         figAx=figAx, logScale=logScale, ticksStep=ticksStep,
         rRange=rRange, yRange=yRange, colors=colors, labels=labels,
```

### Comparing `SplatStats-1.3.9/SplatStats/plotsAux.py` & `SplatStats-1.5.0/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/plotsTeam.py` & `SplatStats-1.5.0/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/SplatStats/statInkConstants.py` & `SplatStats-1.5.0/SplatStats/statInkConstants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
+import numpy as np
 # import json
+
 # with open('./InkStat/weapon.json', 'r') as f:
 #   WEAPONS = json.load(f)
 # wpnKeys = [i['key'] for i in WEAPONS]
 # wpnDict = {
 #   wpnKeys[ix]: WEAPONS[ix]['name']['en_US'] for ix in range(len(wpnKeys))
 # }
 
@@ -229,7 +231,34 @@
   'B4-death': 'Int8',      'B4-special': 'Int8',
   'B4-inked': 'Int16',     'A4-abilities': 'object',
   # Medals ------------------------------------------------------------------
   'medal1-name': 'string', 'medal1-grade': 'string',
   'medal2-name': 'string', 'medal2-grade': 'string',
   'medal3-name': 'string', 'medal3-grade': 'string'
 }
+
+
+INKSTATS_STYLE = {
+    'kill': {
+        'color': '#1A1AAEDD', 'range': (0, 15),
+        'scaler': lambda x: np.interp(x, [0, 0.125, 0.25], [0, .70, 0.95]),
+        'range': (0, 15)
+    },
+    'death': {
+        'color': '#801AB3DD', 'range': (0, 15),
+        'scaler': lambda x: np.interp(x, [0, 0.125, 0.25], [0, .70, 0.95]),
+        'range': (0, 15)
+    },
+    'assist': {
+        'color': '#C12D74DD', 'range': (0, 10),
+        'scaler': lambda x: np.interp(x, [0, 0.25, 0.65], [0, .70, 0.95]),
+        
+    },
+    'special': {
+        'color': '#1FAFE8DD', 'range': (0, 10),
+        'scaler': lambda x: np.interp(x, [0, 0.25, 0.65], [0, .70, 0.95]),
+    },
+    'paint': {
+        'color': '#35BA49DD', 'range': (0, 20),
+        'scaler': lambda x: np.interp(x, [0, 0.1, 0.2], [0, .70, 0.95]),
+    }
+}
```

### Comparing `SplatStats-1.3.9/SplatStats/statInkPlots.py` & `SplatStats-1.5.0/SplatStats/statInkPlots.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import matplotlib.pyplot as plt
+import matplotlib.colors as mcolors
+from matplotlib.patches import Rectangle
 import SplatStats.colors as clr
 import SplatStats.plots as pts
+import SplatStats.statInkConstants as cst
 
 
 def plotStackedBar(
         data, series_labels, labels=None, figAx=None, category_labels=None, 
         show_values=False, value_format="{}", y_label=None, 
         colors=None, textColor='#000000', fontsize=12,
         xTickOffset=5
@@ -180,40 +183,138 @@
         txt.set_text('{:.0f}k'.format(float(lab)/1e3))
     ax.set_xticklabels(xlabels, rotation=0, fontsize=fontSizes[0])
     return (fig, ax)
 
 
 def plotGaussianLobby(
         lbyDaily, lbyGaussDaily,
-        figAx=None,
+        figAx=None, ylim=(0, -1250), xticksDelta=30,
         gModesColors = ['#DE0B64FF', '#FDFF00FF', '#0D37C3FF', '#71DA0CFF', '#531BBAFF']
     ):
     gModes = list(lbyDaily.columns)
     if not figAx:
         (fig, ax) = (plt.figure(figsize=(20, 3)), plt.axes())
     else:
         (fig, ax) = figAx
     ax.stackplot(
         lbyGaussDaily[0][0], *[-y[1] for y in lbyGaussDaily], 
         labels=gModes, baseline='zero',
         colors=gModesColors
     )
     ax.legend(loc='upper left').remove()
     ax.set_xlim(0, lbyGaussDaily[0][0][-1])
-    ax.set_ylim(0, -1250)
-    xtickRan = np.arange(0, lbyGaussDaily[0][0][-1], 15)
-    ax.set_ylim(ax.get_ylim()[::-1])
+    ax.set_ylim(ylim[0], ylim[1])
+    xtickRan = np.arange(0, lbyGaussDaily[0][0][-1], xticksDelta)
+    # ax.set_ylim(ax.get_ylim()[::-1])
     ax.xaxis.tick_top()
     ax.set_xticks(
         xtickRan, 
         [
-            '{}/{}'.format(lbyDaily.index[i].month, lbyDaily.index[i].day)
+            '{}/{}'.format(
+                lbyDaily.index[int(i)].month, 
+                lbyDaily.index[int(i)].day
+            )
             for i in xtickRan
         ],
         ha='left', va='bottom', rotation=0, fontsize=12.5
     )
     ax.set_yticks([], [])
     ax.spines['top'].set_visible(False)
     ax.spines['bottom'].set_visible(False)
     ax.spines['left'].set_visible(False)
     ax.spines['right'].set_visible(False)
+    return (fig, ax)
+
+
+def plotWeaponsStrips(
+        weaponsHists, weaponsList, stat,
+        figAx=None,
+        weaponsSummary=None,
+        color='#1A1AAEDD', range=(0, 50),
+        cScaler=(lambda x: np.interp(x, [0, 0.125, 0.25], [0, .70, 1])),
+        binSize=1
+    ):
+    wpnList = weaponsList[::-1]
+    bCol = mcolors.ColorConverter().to_rgba(color)
+    if figAx:
+        (fig, ax) = figAx
+    else:
+        (fig, ax) = plt.subplots(figsize=(5, 20))
+    for (ix, wpn) in enumerate(wpnList):
+        wpnData = weaponsHists[wpn][stat]
+        for (x, k) in enumerate(wpnData):
+            alpha = cScaler(k)
+            ax.add_patch(
+                Rectangle(
+                    (x, ix), binSize, 1,
+                    facecolor=(bCol[0], bCol[1], bCol[2], alpha),
+                    edgecolor='#00000088',
+                )
+            )
+    if weaponsSummary:
+        for (ix, wpn) in enumerate(wpnList):
+            wpnData = weaponsSummary[wpn][stat] + binSize/2
+            ax.vlines(
+                wpnData, ix+0.25, ix+0.75,
+                colors='#000000AA',
+                lw=2.5, ls='-'
+            )
+    ax.set_ylim(0, len(wpnList))
+    ax.set_yticks(np.arange(0.5, len(wpnList), 1))
+    ax.set_yticklabels(wpnList)
+    ax.set_xlim(range[0], range[1]+binSize)
+    # ax.xaxis.tick_top()
+    ax.set_xticks(np.arange(range[0]+binSize/2, range[1]+binSize/2+1/2, 5))
+    ax.set_xticklabels(np.arange(range[0], range[1]+1, 5))
+    ax.set_title('{}'.format(stat), fontdict={'fontsize': 20})
+    return (fig, ax)
+
+
+
+def plotWeaponStrip(
+        weaponsHists, weaponName, wpnStats,
+        figAx=None,
+        weaponsSummary=None,
+        styleDictionary=cst.INKSTATS_STYLE,
+        binSize=1
+    ):
+    ranges = np.array([styleDictionary[c]['range'] for c in wpnStats]).T
+    range = (min(ranges[0]), max(ranges[1]))
+    bCols = [
+        mcolors.ColorConverter().to_rgba(styleDictionary[c]['color']) 
+        for c in wpnStats
+    ]
+    cScalers = [styleDictionary[c]['scaler'] for c in wpnStats]
+    if figAx:
+        (fig, ax) = figAx
+    else:
+        (fig, ax) = plt.subplots(figsize=(20, 2))
+    wpnFullData = weaponsHists[weaponName]
+    for (ix, stat) in enumerate(wpnStats):
+        wpnData = wpnFullData[stat]
+        for (x, k) in enumerate(wpnData):
+            alpha = cScalers[ix](k)
+            bCol = bCols[ix]
+            ax.add_patch(
+                Rectangle(
+                    (x, ix), binSize, 1,
+                    facecolor=(bCol[0], bCol[1], bCol[2], alpha),
+                    edgecolor='#00000088',
+                )
+            )
+    if weaponsSummary:
+        wpnFullSummary = weaponsSummary[weaponName]
+        for (ix, sta) in enumerate(wpnStats):
+            wpnData = wpnFullSummary[sta] + binSize/2
+            ax.vlines(
+                wpnData, ix+0.25, ix+0.75,
+                colors='#000000AA',
+                lw=2.5, ls='-'
+            )
+    ax.set_xticks(np.arange(range[0]+binSize/2, range[1]+binSize/2+1/2, 5))
+    ax.set_xticklabels(np.arange(range[0], range[1]+1, 5))
+    ax.set_xlim(range[0], range[1]+binSize)
+    ax.set_ylim(0, len(wpnStats))
+    ax.set_yticks(np.arange(0.5, len(wpnStats), 1))
+    ax.set_yticklabels(wpnStats)
+    ax.set_title('{}'.format(weaponName), fontdict={'fontsize': 20})
     return (fig, ax)
```

### Comparing `SplatStats-1.3.9/SplatStats/statInkStats.py` & `SplatStats-1.5.0/SplatStats/statInkStats.py`

 * *Files 20% similar despite different names*

```diff
@@ -178,7 +178,76 @@
     wpnRanks = zip(
         [i+1 for i in range(wpnsNum)], 
         wpnFreq.keys(),
         [wpnWinRatio[ix] for ix in freqSorting]
     )
     return list(wpnRanks)
 
+
+def getWeaponsDataframe(
+        battlesResults,
+        stats=['weapon', 'kill', 'assist', 'death', 'inked', 'special']
+    ):
+    dfs = []
+    for prepend in ['A1', 'A2', 'A3', 'A4', 'B1', 'B2', 'B3', 'B4']:
+        df = battlesResults[[prepend+'-{}'.format(c) for c in stats]]
+        df.columns = [c[3:] for c in df.columns]
+        dfs.append(df)
+    dfStats = pd.concat(dfs)
+    return dfStats
+
+
+def getWeaponStatsHistograms(
+        weaponDF, range,
+        stats=['kill', 'death', 'assist', 'special', 'inked'],
+        normalized=True, binSize=1
+    ):
+    wpnHists = {
+        stat: np.nan_to_num(
+            stt.calcBinnedFrequencies(
+                weaponDF[stat], range[0], range[1], 
+                normalized=normalized, binSize=binSize
+            ), 0
+        )
+        for stat in stats
+    }
+    return wpnHists
+
+
+def getWeaponStatsMean(
+        weaponDF,
+        stats=['kill', 'death', 'assist', 'special', 'inked'],
+        mFun=np.mean
+    ):
+    if weaponDF.shape[0] > 0:
+        wpnMeans = {stat: mFun(weaponDF[stat]) for stat in stats}
+    else:
+        wpnMeans = {stat: 0 for stat in stats}
+    return wpnMeans
+
+
+def getWeaponsStatsHistograms(
+        weaponsDF, weapons, range,
+        stats=['kill', 'death', 'assist', 'special', 'inked'],
+        normalized=True, binSize=1
+    ):
+    kFreqs = {}
+    for wpn in weapons:
+        wpnDF = weaponsDF[weaponsDF['weapon']==wpn]
+        kFreqs[wpn] = getWeaponStatsHistograms(
+            wpnDF, range, stats=stats, binSize=binSize, normalized=normalized
+        )
+    return kFreqs
+
+
+def getWeaponsStatsSummary(
+        weaponsDF, weapons, 
+        summaryFunction=np.mean,
+        stats=['kill', 'death', 'assist', 'special', 'inked']
+    ):
+    kMeans = {}
+    for wpn in weapons:
+        wpnDF = weaponsDF[weaponsDF['weapon']==wpn]
+        kMeans[wpn] = getWeaponStatsMean(
+            wpnDF, stats=stats, mFun=summaryFunction
+        )
+    return kMeans
```

### Comparing `SplatStats-1.3.9/SplatStats/stats.py` & `SplatStats-1.5.0/SplatStats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,21 +96,20 @@
         xMax (int): Highest possible value that will be counted.
         binSize (int, optional): Step size for the binning (from xMin to xMax in intervals of binSize). Defaults to 1.
         normalized (bool, optional): If true, the frequencies are divided by the total so that they sum to 1. Defaults to False.
 
     Returns:
         array: Frequencies of ocurrences in the defined ranges.
     """    
-    freqs = np.array([
-        frequencyInRange(array, i, i+binSize) for i in 
-        range(xMin, xMax, binSize)
-    ])
-    total = np.sum(freqs)
+    rans = np.arange(xMin, xMax+binSize, binSize)
+    sArray = sorted(np.copy(array))
+    sortedIxs = np.searchsorted(sArray, rans, side='left')
+    freqs = np.diff(sortedIxs)
     if normalized:
-        freqs = freqs/total
+        freqs = freqs/np.sum(freqs)
     return freqs
 
 
 def calcStatsByKey(bHist, key, sortBy='win ratio', ascending=False):
     """Given a battle history dataframe, this function calculates stats broken down by the supplied key (column).
 
     Args:
```

### Comparing `SplatStats-1.3.9/SplatStats.egg-info/PKG-INFO` & `SplatStats-1.5.0/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.3.9
+Version: 1.5.0
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.3.9/SplatStats.egg-info/SOURCES.txt` & `SplatStats-1.5.0/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-1.3.9/setup.py` & `SplatStats-1.5.0/setup.py`

 * *Files identical despite different names*

