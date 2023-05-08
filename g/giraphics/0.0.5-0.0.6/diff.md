# Comparing `tmp/giraphics-0.0.5.tar.gz` & `tmp/giraphics-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/giraphics-0.0.5.tar", last modified: Thu Mar 18 11:17:58 2021, max compression
+gzip compressed data, was "giraphics-0.0.6.tar", last modified: Mon May  8 07:08:50 2023, max compression
```

## Comparing `giraphics-0.0.5.tar` & `giraphics-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,48 @@
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.859381 giraphics-0.0.5/
--rw-r--r--   0 girirajhira   (501) staff       (20)      773 2021-03-18 11:17:58.859624 giraphics-0.0.5/PKG-INFO
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.848034 giraphics-0.0.5/giraphics/
--rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-02-05 12:08:00.599220 giraphics-0.0.5/giraphics/__init__.py
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.849286 giraphics-0.0.5/giraphics/animate/
--rw-r--r--   0 girirajhira   (501) staff       (20)     1572 2021-02-22 12:00:52.573955 giraphics-0.0.5/giraphics/animate/animation.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     7689 2021-02-09 13:52:08.202458 giraphics-0.0.5/giraphics/animate/animator.py
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.851863 giraphics-0.0.5/giraphics/graphing/
--rw-r--r--   0 girirajhira   (501) staff       (20)     1252 2021-02-09 13:52:08.251799 giraphics-0.0.5/giraphics/graphing/Scenic.py
--rw-r--r--   0 girirajhira   (501) staff       (20)    11737 2021-02-09 13:52:08.230076 giraphics-0.0.5/giraphics/graphing/fancygraphs.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     5032 2021-02-09 13:52:08.303331 giraphics-0.0.5/giraphics/graphing/figure.py
--rw-r--r--   0 girirajhira   (501) staff       (20)    20344 2021-02-22 11:42:17.973703 giraphics-0.0.5/giraphics/graphing/graph.py
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.853738 giraphics-0.0.5/giraphics/graphing3d/
--rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-01-17 13:54:27.963000 giraphics-0.0.5/giraphics/graphing3d/__init__.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     1710 2021-02-09 13:51:32.936471 giraphics-0.0.5/giraphics/graphing3d/graph3d.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     4654 2021-02-09 13:52:08.158131 giraphics-0.0.5/giraphics/graphing3d/graph3d2.py
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.854997 giraphics-0.0.5/giraphics/svg/
--rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-02-09 13:56:09.733430 giraphics-0.0.5/giraphics/svg/__init__.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     7878 2021-02-20 13:40:16.995236 giraphics-0.0.5/giraphics/svg/svgkit.py
-drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2021-03-18 11:17:58.859220 giraphics-0.0.5/giraphics/utilities/
--rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-01-17 14:15:29.739649 giraphics-0.0.5/giraphics/utilities/__init__.py
--rw-r--r--   0 girirajhira   (501) staff       (20)      790 2020-03-24 15:14:58.971366 giraphics-0.0.5/giraphics/utilities/colour.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     4853 2021-02-22 12:03:14.697063 giraphics-0.0.5/giraphics/utilities/convert.py
--rw-r--r--   0 girirajhira   (501) staff       (20)      835 2020-07-08 02:05:00.286990 giraphics-0.0.5/giraphics/utilities/latext.py
--rw-r--r--   0 girirajhira   (501) staff       (20)      236 2020-08-14 14:28:42.486834 giraphics-0.0.5/giraphics/utilities/mathtext.py
--rw-r--r--   0 girirajhira   (501) staff       (20)      400 2020-07-08 02:05:00.266059 giraphics-0.0.5/giraphics/utilities/timer.py
--rw-r--r--   0 girirajhira   (501) staff       (20)     2071 2020-08-13 15:23:59.013719 giraphics-0.0.5/giraphics/utilities/utils.py
--rw-r--r--   0 girirajhira   (501) staff       (20)      974 2021-02-09 14:13:24.551113 giraphics-0.0.5/setup.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.354240 giraphics-0.0.6/
+-rw-r--r--   0 girirajhira   (501) staff       (20)     1082 2021-10-28 15:33:11.000000 giraphics-0.0.6/LICENSE.md
+-rw-r--r--   0 girirajhira   (501) staff       (20)      759 2023-05-08 07:08:50.354022 giraphics-0.0.6/PKG-INFO
+-rw-r--r--   0 girirajhira   (501) staff       (20)     5055 2023-05-08 06:58:23.000000 giraphics-0.0.6/README.md
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.345309 giraphics-0.0.6/giraphics/
+-rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-10-28 15:33:11.000000 giraphics-0.0.6/giraphics/__init__.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.347233 giraphics-0.0.6/giraphics/animate/
+-rw-r--r--   0 girirajhira   (501) staff       (20)     1856 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/animate/animation.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     7681 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/animate/animator.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      794 2022-11-07 09:04:34.000000 giraphics-0.0.6/giraphics/animate/morphing_animation_test.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     2525 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/animate/movements.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.348722 giraphics-0.0.6/giraphics/graphing/
+-rw-r--r--   0 girirajhira   (501) staff       (20)     1249 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing/Scenic.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)    18984 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing/fancygraph.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     6118 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing/figure.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)    26209 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing/graph.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)        0 2022-07-17 14:05:07.000000 giraphics-0.0.6/giraphics/graphing/scenic2.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.349672 giraphics-0.0.6/giraphics/graphing3d/
+-rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-10-28 15:33:11.000000 giraphics-0.0.6/giraphics/graphing3d/__init__.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     1709 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing3d/graph3d.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     4702 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing3d/graph3d2.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      220 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/graphing3d/grapher3.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.350480 giraphics-0.0.6/giraphics/svg/
+-rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-10-28 15:33:11.000000 giraphics-0.0.6/giraphics/svg/__init__.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)    11292 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/svg/morph.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)    10656 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/svg/morph2.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)    11222 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/svg/svgkit.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.353709 giraphics-0.0.6/giraphics/utilities/
+-rw-r--r--   0 girirajhira   (501) staff       (20)        0 2021-10-28 15:33:11.000000 giraphics-0.0.6/giraphics/utilities/__init__.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     2311 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/utilities/caching_functions.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     2423 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/utilities/colour.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     5516 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/utilities/convert.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     2579 2022-07-17 14:14:21.000000 giraphics-0.0.6/giraphics/utilities/latex2.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)        0 2022-07-17 14:05:07.000000 giraphics-0.0.6/giraphics/utilities/latex_converter.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      427 2022-07-17 14:14:39.000000 giraphics-0.0.6/giraphics/utilities/latex_svg_decoder.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      835 2022-07-17 14:05:07.000000 giraphics-0.0.6/giraphics/utilities/latext.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      236 2022-07-17 14:05:07.000000 giraphics-0.0.6/giraphics/utilities/mathtext.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      560 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/utilities/parametrisations.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)      400 2021-10-28 15:33:11.000000 giraphics-0.0.6/giraphics/utilities/timer.py
+-rw-r--r--   0 girirajhira   (501) staff       (20)     2484 2023-05-08 06:58:24.000000 giraphics-0.0.6/giraphics/utilities/utils.py
+drwxr-xr-x   0 girirajhira   (501) staff       (20)        0 2023-05-08 07:08:50.345959 giraphics-0.0.6/giraphics.egg-info/
+-rw-r--r--   0 girirajhira   (501) staff       (20)      759 2023-05-08 07:08:50.000000 giraphics-0.0.6/giraphics.egg-info/PKG-INFO
+-rw-r--r--   0 girirajhira   (501) staff       (20)     1133 2023-05-08 07:08:50.000000 giraphics-0.0.6/giraphics.egg-info/SOURCES.txt
+-rw-r--r--   0 girirajhira   (501) staff       (20)        1 2023-05-08 07:08:50.000000 giraphics-0.0.6/giraphics.egg-info/dependency_links.txt
+-rw-r--r--   0 girirajhira   (501) staff       (20)       14 2023-05-08 07:08:50.000000 giraphics-0.0.6/giraphics.egg-info/requires.txt
+-rw-r--r--   0 girirajhira   (501) staff       (20)       10 2023-05-08 07:08:50.000000 giraphics-0.0.6/giraphics.egg-info/top_level.txt
+-rw-r--r--   0 girirajhira   (501) staff       (20)       38 2023-05-08 07:08:50.354313 giraphics-0.0.6/setup.cfg
+-rw-r--r--   0 girirajhira   (501) staff       (20)      995 2023-05-08 06:58:24.000000 giraphics-0.0.6/setup.py
```

### Comparing `giraphics-0.0.5/PKG-INFO` & `giraphics-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: giraphics
-Version: 0.0.5
+Version: 0.0.6
 Summary: Lightweight graphing and animations
 Home-page: https://github.com/tghira/giraphics
 Author: T. G. Hiranandani
 Author-email: giraphics@protonmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: graphs,animations,graphics,vector-graphics
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE.md
```

### Comparing `giraphics-0.0.5/giraphics/animate/animation.py` & `giraphics-0.0.6/giraphics/animate/animation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from giraphics.utilities.convert import *
-from giraphics.graphing.fancygraphs import *
-from os import getcwd
+from giraphics.graphing.fancygraph import *
 from IPython.display import Image, SVG, Video
 
 
-class Frame_graphic(FancyGraphs):
+class FrameGraphic(FancyGraph):
     def __init__(self, width, height, xlim, ylim, name, origin=[0.0, 0.0], theme="dark",
                  transform="none", grouped=False):
-        FancyGraphs.__init__(self, width, height, xlim, ylim, name, origin=[0.0, 0.0], theme="dark",
-                 transform="none", grouped=False)
+        FancyGraph.__init__(self, width, height, xlim, ylim, name, origin=[0.0, 0.0], theme="dark",
+                            transform=transform, grouped=False)
         self.frame_index = 0
+        self.last_frame = ''
 
     def press(self):
         self.svg.path = "vectors/g" + namer(self.frame_index) + ".svg"
         self.frame_index += 1
-        FancyGraphs.save(self)
-        self.svg.__init__(self.svg.path, self.width, self.height, transform="none", grouped=False)
+        self.last_frame = self.svg.canvas
+        FancyGraph.save(self, clear=False)
+        self.svg.canvas = self.svg.preamble
 
 
 class Animation:
-    def __init__(self, name, frames, width, height, xlim, ylim, framerate=60, origin=[0, 0]):
+    def __init__(self, name, width, height, xlim, ylim, framerate=60, origin=[0, 0], pauses=True):
         create_directory("vectors", warnings=False)
         create_directory("rasters", warnings=False)
-        self.frames = frames
+        self.frames = 0
         self.name = name
         self.width = width
         self.framerate = framerate
         self.height = height
         self.xlim = xlim
         self.ylim = ylim
-        self.plate = Frame_graphic(width, height, xlim, ylim, '', origin=origin)
+        self.pauses = pauses
+        self.plate = FrameGraphic(width, height, xlim, ylim, '', origin=origin)
 
-    def develop(self, cleanup=True, warnings=True):
+    def pause(self, frames):
+        if self.pauses:
+            for i in range(frames):
+                self.plate.svg.canvas = self.plate.last_frame
+                self.plate.press()
+
+    def develop(self, cleanup=True, warnings=True, workers=2):
         # Creating
-        create_raster_batch("vectors", 'g', 'p', "rasters", self.frames)
-        create_mpeg(self.name, 'p', self.frames, "rasters", framerate=self.framerate, warnings=warnings)
+        create_raster_batch("vectors", 'g', 'p', "rasters", self.plate.frame_index)
+        create_mpeg(self.name, 'p', "rasters", framerate=self.framerate, warnings=warnings)
         if cleanup:
             clean_up('vectors', 'rasters')
 
-
+    def show(self):
+        Video(self.name)
```

### Comparing `giraphics-0.0.5/giraphics/animate/animator.py` & `giraphics-0.0.6/giraphics/animate/animator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import multiprocessing
 import os
 from giraphics.utilities.utils import listlike
 from giraphics.utilities import convert
 import sys
-from giraphics.graphing.fancygraphs import FancyGraphs
+from giraphics.graphing.fancygraph import FancyGraph
 from giraphics.utilities.timer import Timer
 
 '''
 TODO: Fix grid issue, too bold
     : Quality control
     : Create work spaces
     : Do an eigen vector example
@@ -40,77 +40,77 @@
     def epsf(self, i):
         return (i) ** 3
 
     def create_frame(self, name, func, i, axes=True, label=True, expr="", grid=True, axestroke=2, axescolour="white",
                      strokewidths=[2], colours=["yellow"], bg="black", grid_colour="yellow", grindint=10, scale=0.8,
                      grids=[10, 10], s=1, opac=1, display=False):
         if self.type == "complex":
-            G = FancyGraphs(self.height, self.width, self.xlim, self.ylim, name)
+            G = FancyGraph(self.height, self.width, self.xlim, self.ylim, name)
             G.bg(bg)
             if axes:
                 G.axes(colour=axescolour, strokewidth=axestroke)
             if grid:
                 G.grid(colour=grid_colour)
             for i in range(len(func)):
                 G.ComplexPlot(func[i], strokewidth=strokewidths[i])
             G.save()
             if display:
                 G.display()
         elif self.type == "cart":
-            G = FancyGraphs(self.height, self.width, self.xlim, self.ylim, name)
+            G = FancyGraph(self.height, self.width, self.xlim, self.ylim, name)
             G.bg(bg)
             if axes:
                 G.axes(colour=axescolour, strokewidth=axestroke)
             if grid:
                 G.grid(colour=grid_colour)
             if label:
                 G.embed_latex_anim(expr % (i, i), self.xlim - 2, self.ylim - 2)
             for i in range(len(func)):
                 G.plot(func[i], strokewidth=strokewidths[i], colour=colours[i], opac=opac)
             G.save()
             if display:
                 G.display()
         elif self.type == "lineartrans":
-            G = FancyGraphs(self.height, self.width, self.xlim, self.ylim, name)
+            G = FancyGraph(self.height, self.width, self.xlim, self.ylim, name)
             G.bg(bg)
             if axes:
                 G.axes(colour=axescolour, strokewidth=axestroke)
             if grid:
                 G.grid(colour=grid_colour)
             for i in range(len(func)):
                 G.LinearTranforms(func, strokewidths=strokewidths)
             G.save()
             if display:
                 G.display()
         elif self.type == "scatter":
-            G = FancyGraphs(self.height, self.width, self.xlim, self.ylim, name)
+            G = FancyGraph(self.height, self.width, self.xlim, self.ylim, name)
             G.bg(bg)
             if axes:
                 G.axes(colour=axescolour, strokewidth=axestroke)
             if grid:
                 G.grid(colour=grid_colour)
             for i in range(len(func)):
                 G.scatter(func[i], strokewidth=strokewidths[i])
             G.save()
             if display:
                 G.display()
         elif self.type == "vectorfield":
-            G = FancyGraphs(self.height, self.width, self.xlim, self.ylim, name)
+            G = FancyGraph(self.height, self.width, self.xlim, self.ylim, name)
             G.bg(bg)
             if axes:
                 G.axes(colour=axescolour, strokewidth=axestroke)
             if grid:
                 G.grid(colour=grid_colour)
             for i in range(len(func)):
                 G.VectorField(func[i], strokewidth=strokewidths[i], stroke=colours[i], gridint=grindint, scale=scale,constcolour=False)
             G.save()
             if display:
                 G.display()
         elif self.type == "complexscatter":
-            G = FancyGraphs(self.height, self.width, self.xlim, self.ylim, name)
+            G = FancyGraph(self.height, self.width, self.xlim, self.ylim, name)
             G.bg(bg)
             if axes:
                 G.axes(colour=axescolour, strokewidth=axestroke)
             if grid:
                 G.grid(colour=grid_colour)
             for i in range(len(func)):
                 G.ComplexPlotScatter(func[i], s=s, colour=colours[i], grids=grids)
```

### Comparing `giraphics-0.0.5/giraphics/graphing/Scenic.py` & `giraphics-0.0.6/giraphics/graphing/Scenic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from giraphics.graphing.fancygraphs import *
+from giraphics.graphing.fancygraph import *
 
 
-class Widget(FancyGraphs):
+class Widget(FancyGraph):
     def __init__(self, xlim, ylim, Scene, scale=[0.25,0.25], pos=[0, 0], origin=[0.0, 0.0], border=True,
                 bcol="white", bstroke=2.5):
         #Translations
         absx, absy = Scene.tranx(pos[0]) - Scene.width * scale[0]/2, Scene.trany(pos[1]) - Scene.height * scale[1]/2
         Graph.__init__(self,Scene.width * scale[0], Scene.height * scale[1], xlim, ylim, " ", origin=origin,
                            transform="translate(" + str(absx) + " " + str(absy) + ")", grouped=True)
         #Borders
         Scene.svg.draw_rect(Scene.tranx(pos[0]), Scene.trany(pos[1]), Scene.width * scale[0], Scene.height * scale[1], 'none', stroke=bcol,
                                strokewidth=bstroke)
     def save(self):
         self.svg.save(write_out=False)
 
 
-class Scene(FancyGraphs):
+class Scene(FancyGraph):
     def commitWidget(self, widget):
         widget.save()
         self.svg.canvas += widget.svg.canvas
 
 # A = Scene(2560, 1440, 16, 9, 'Ascene.svg')
 # A.bg(colour="black")
 # A.axes()
```

### Comparing `giraphics-0.0.5/giraphics/graphing/figure.py` & `giraphics-0.0.6/giraphics/graphing/figure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from giraphics.graphing.graph import Graph
+import numpy as np
 
+from giraphics.graphing.graph import Graph
+from math import pi
 
 class Figure(Graph):
     def __init__(self, width, height, xlim, ylim, name, origin=[0.0, 0.0], theme="dark",
                  border_width=0.12, bg="white"):
         Graph.__init__(self, width, height, xlim, ylim, name, theme=theme)
         self.bw = 1 - border_width
         self.border_width = border_width
@@ -71,41 +73,69 @@
                               str((round((i - self.ylim - self.origin[1]) * oy, 2))),
                               fontsize=fontsize, colour=stroke, opac=0.6)
 
     # Todo: Constructions #
 
     # Features
 
-    def xlabel(self, label="x", fontsize=13):
-        x = self.origin[0]
-        y = -self.ylim*self.bw - (1-self.bw)*self.ylim/2
-        self.text(x, y, text=label, colour="black", fontsize=fontsize)
-
-    def ylabel(self, label="y", fontsize=13):
-        y = self.origin[1]
-        x = -self.xlim*self.bw - (1-self.bw)*self.xlim/2
-        self.text(x, y, text=label, colour="black", fontsize=fontsize, rotation="-90")
-
-    def title(self, title_label, fontsize = 26):
-        x = self.origin[0]
-        y = self.ylim*self.bw + (1-self.bw)*self.ylim/3
-        self.text(x, y, title_label, colour="black", fontsize=fontsize)
+    def xlabel(self, label="x", fontsize=13, use_latex=False, scale=2):
+        if use_latex:
+            x = self.origin[0]
+            y = -self.ylim * self.bw - (1 - self.bw) * self.ylim / 2
+            self.add_latex(label, x, y, scale=scale)
+        else:
+            x = self.origin[0]
+            y = -self.ylim*self.bw - (1-self.bw)*self.ylim/2
+            self.text(x, y, text=label, colour="black", fontsize=fontsize)
+
+    def ylabel(self, label="f(x)", fontsize=13, use_latex=False,scale=2):
+        if use_latex:
+            y = self.origin[1]
+            x = -self.xlim * self.bw - (1 - self.bw) * self.xlim/2
+            self.add_latex(label, x, y, scale=2, rotation=pi/2)
+        else:
+            y = self.origin[1]
+            x = -self.xlim*self.bw - (1-self.bw)*self.xlim/2
+            self.text(x, y, text=label, colour="black", fontsize=fontsize, rotation="-90")
+
+    def title(self, title_label, fontsize = 26, use_latex=False):
+        if use_latex:
+            x = self.origin[0]
+            y = self.ylim * self.bw + (1 - self.bw) * self.ylim / 3
+            self.add_latex(title_label,x,y)
+        else:
+            x = self.origin[0]
+            y = self.ylim*self.bw + (1-self.bw)*self.ylim/3
+            self.text(x, y, title_label, colour="black", fontsize=fontsize)
+
+
+    def legend(self, data, loc = 'upper right'):
+        for i in range(0,1)
+
 
     def save(self):
-        self.svg.canvas += self.inner_graph.svg.canvas + "\n </svg>\n </g>\n"
+        self.svg.canvas += self.inner_graph.svg.canvas + "\n </svg>\n </g>\n </g>\n"
         self.draw_rect(0, 0, 2 * self.xlim * self.bw, 2 * self.ylim * self.bw, fill="none", colour="black",
                        strokewidth=1.2)
         Graph.save(self)
 
-# def func(x):
-#     return 0.04 * x ** 2 * math.sin(6 * x) - 5
-#
-# f = Figure(600, 450, 15, 10, "fig.svg", origin=[-5,-5])
-# f.plot(func, colour="red")
-# f.grid()
-# # f.grid2(colour="blue")
-# # f.ticks(markers=True)
-# f.xlabel(label="f(x)")
-# f.ylabel()
-# f.title("Title")
-# f.save()
-# f.display()
+
+import math
+def func(x):
+    return 0.04 * x ** 2 * math.sin(6 * x) - 5
+
+
+f = Figure(600, 450, 15, 10, "fig2.svg", origin=[0,0])
+f.plot(func, colour="red")
+f.plot_points(np.linspace(-15,15, 100),np.linspace(-15,15, 100)**2, colour='blue')
+f.grid()
+# f.grid2(colour="blue")
+# f.ticks(markers=True)
+# f.xlabel(label="$f(x)$", use_latex=True)
+# f.ylabel(use_latex=True)
+f.inner_graph.axes(colour='black')
+f.xlabel(label ='$x$', use_latex=True)
+f.ylabel(label ='$y$', use_latex=True)
+f.add_latex('$f(x)$', 0, 0, scale=3, rotation=0)
+# f.title("Title", use_latex=True)
+f.save()
+f.display()
```

### Comparing `giraphics-0.0.5/giraphics/graphing/graph.py` & `giraphics-0.0.6/giraphics/graphing/graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from giraphics.svg.svgkit import *
-from giraphics.utilities.latext import *
-from giraphics.utilities.mathtext import *
+# from giraphics.utilities.latext import *
+# from giraphics.utilities.mathtext import *
+from giraphics.svg.morph2 import *
+from giraphics.utilities.latex2 import latex_expression
 from giraphics.utilities.convert import *
+from giraphics.utilities.latex_svg_decoder import *
 from IPython.display import SVG as IPSVG
 from IPython.display import Image
 import numpy as np
+from math import sqrt
 import webbrowser
 import os
 import platform
-# from numba import njit, jit
 
 
 class Graph:
     def __init__(self, width, height, xlim, ylim, name, origin=[0.0, 0.0], theme="dark",
                  transform="none", grouped=False):
         """
         Initial
@@ -31,51 +34,53 @@
         :param transform: bool
             sets transformation rules for the svg
         :param grouped: bool
             whether the svg should be grouped
         """
         self.svg = SVG(name, width, height, transform=transform, grouped=grouped)
         self.name = name
-        self.eps = xlim / 2000
         self.height = height
         self.width = width
         self.xlim = xlim
+        self.transform = transform
         self.ylim = ylim
         self.origin = np.array(origin)
         self.xscale = width / (2 * xlim)
         self.yscale = height / (2 * ylim)
-        self.TexLoader = []
+        self.nscale = sqrt(self.xscale ** 2 + self.yscale ** 2) / sqrt(2) / 30
+        self.insets = []
+        self.latex_history = {}
         if theme == "dark":
             self.theme = {
                 'background': 'black',
                 'primary': 'yellow',
                 'secondary': 'white'
             }
         else:
             self.theme = {
                 'background': 'white',
                 'primary': 'black',
                 'secondary': 'black'
             }
 
-    
     def tranx(self, x):
         """
         converts the x coordinate to svg coordinate
         :param x: float
             x coordinate in standard units
         :returns: float
             return the x coordinate in y
         """
         if x is not None:
             return + round((self.width / (2 * self.xlim)) * (x + self.origin[0]) + self.width / 2, 2)
             return - round((self.height / (2 * self.ylim)) * (y + self.origin[1]) + self.height / 2, 2)
 
         else:
             return None
+
     def trany(self, y):
         """
         converts the y coordinate to svg coordinate
         :param y:
         :return: svg coordinate
         """
         if y is not None:
@@ -99,14 +104,15 @@
             colour of the axes
         :param strokewidth: float
             thickness of the axes
         :param arrows: bool
             whether arrows are to required
         :return: None
         """
+        strokewidth = strokewidth * self.nscale
         ox = self.origin[0]
         oy = self.origin[1]
         scale = strokewidth * self.height * 0.001 / 2
 
         self.svg.draw_line(self.tranx(-self.xlim - ox), self.trany(0), self.tranx(self.xlim - ox), self.trany(0),
                            stroke=colour,
                            strokewidth=strokewidth)
@@ -119,29 +125,28 @@
             self.svg.draw_arrowhead2(self.tranx(0), self.trany(self.ylim - oy) + 3 * scale, scale, 0,
                                      colour=colour)  # N
             self.svg.draw_arrowhead2(self.tranx(0), self.trany(-self.ylim - oy) - 3 * scale, scale, math.pi,
                                      colour=colour)  # S
             self.svg.draw_arrowhead2(self.tranx(-self.xlim - ox) + 3 * scale, self.trany(0), scale, - math.pi / 2,
                                      colour=colour)  # W
 
-    # Todo: Fix Grid, origin changes
-
     def grid(self, grid_int=None, colour="#A7A7A7", grid_multiplier=1, strokewidth=0.7, opac=0.5):
         """
         Creates a grid
         :param grids: list (length 2)
         the number of gridlines horizontally and vertically
         :param colour: string
             set the colour of the grid
         :param strokewidth: float
             sets the thickness of the grid
         :param opac: float (0-1)
             sets the opacity of the grid
         :return: None
         """
+        strokewidth = strokewidth * self.nscale
         if grid_int is None:
             grid_int = []
             if self.xlim < 5:
                 grid_int.append(round(2 * self.xlim * grid_multiplier))
             else:
                 grid_int.append(2 * self.xlim)
             if self.ylim < 5:
@@ -161,16 +166,15 @@
                                stroke=colour, strokewidth=strokewidth, opacity=opac)
 
     # def text(self, x, y, text, fontsize=20, colour="white", rotation=0,
     #          font="14", opac=1):
     #     self.svg.canvas += '<text x="%s" y="%s"  style=" font-family:Arial" fill="%s" font-size="%s" opacity="%s"  transform="rotate(%s)"> %s </text>' % (
     #     self.tranx(x), self.trany(y), colour, fontsize, opac, rotation, text)
 
-    def text(self, x, y, text, fontsize=20, colour="white", rotation=0,
-             font="14", opac=1):
+    def text(self, x, y, text, fontsize=12, colour="white", rotation=0, opac=1, fontfamily='sans-serif'):
         """
         Draws specified text at the given coordinates (in standard units)
         :param x: float
             x coordinate
         :param y: float
             y coordinate
         :param text: string
@@ -182,44 +186,46 @@
         :param rotation: float
             specifies the how the text should be rotated
         :param font: string
             specifies the font to be used
         :param opac: float (0-1)
         :return: None
         """
-        self.svg.canvas += '<text x="%s" y="%s"  font-family="Recursive" fill="%s" font-size="%s" alignment-baseline="middle" text-anchor="middle" opacity="%s"  transform="rotate(%s,%s,%s)"> %s </text>\n' % (
-            self.tranx(x), self.trany(y), colour, fontsize, opac, rotation, self.tranx(x), self.trany(y), text)
-
-    def math_text(self, expression, x, y, colour="White", scale=4):
-        math_to_svg(expression, os.getcwd() + "/temp.txt")
-        with open("temp.txt", 'r') as file:
-            code = file.read()
-        os.remove(os.getcwd() + "/temp.txt")
-        dx = len(expression) * scale
-        dy = 9 * scale
-        self.svg.canvas += '\n <g transform-origin="bottome" transform="translate(' + str(
-            self.tranx(x) - dx) + ' ' + str(self.trany(y) - dy) + '),' + 'scale(' + str(scale) + ',' + str(
-            scale) + ')' + ' ">'
-        self.svg.canvas += code.replace('currentColor', colour).replace('8.781ex', str(scale))
-        self.svg.canvas += '</g> \n'
+        fontsize *= self.nscale
+        self.svg.canvas += f'<text x="{self.tranx(x)}" y="{self.trany(y)}"  font-family="{fontfamily}" fill="{colour}" font-size="{fontsize}" alignment-baseline="middle" text-anchor="middle" color="{colour}" opacity="{opac}"  transform="rotate({rotation},{self.tranx(x)},{self.trany(y)})"> {text} </text>\n'
 
-    def add_math_text(self, expr, x, y, colour="white", scale=4):
-        self.TexLoader.append([expr, x, y, colour, scale])
+    # def math_text(self, expression, x, y, colour="White", scale=4):
+    #     math_to_svg(expression, os.getcwd() + "/temp.txt")
+    #     with open("temp.txt", 'r') as file:
+    #         code = file.read()
+    #     os.remove(os.getcwd() + "/temp.txt")
+    #     dx = len(expression) * scale
+    #     dy = 9 * scale
+    #     self.svg.canvas += '\n <g transform-origin="bottome" transform="translate(' + str(
+    #         self.tranx(x) - dx) + ' ' + str(self.trany(y) - dy) + '),' + 'scale(' + str(scale) + ',' + str(
+    #         scale) + ')' + ' ">'
+    #     self.svg.canvas += code.replace('currentColor', colour).replace('8.781ex', str(scale))
+    #     self.svg.canvas += '</g> \n'
+    #
+    # def add_math_text(self, expr, x, y, colour="white", scale=4):
+    #     self.TexLoader.append([expr, x, y, colour, scale])
 
-    def ticks(self, colour="yellow", strokewidth=1, markers=False, fontsize=8):
+    def ticks(self, colour="yellow", strokewidth=1, markers=False, fontsize=4):
         """
         Adds ticks to x and y axes
         :param colour: string
         :param strokewidth: float
         :param tick: int
             the number of ticks
         :param markers: bool
         :param fontsize: float
         :return: None
         """
+        strokewidth = strokewidth * self.nscale
+        fontsize = fontsize * self.nscale
         tickx, ticky = round(2 * self.xlim), round(2 * self.ylim)
         dx = self.width / tickx
         dy = self.height / ticky
         ox = self.xlim * 2 / tickx
         oy = self.ylim * 2 / ticky
         # x axis
         for i in range(1, tickx):
@@ -238,15 +244,15 @@
                                strokewidth=strokewidth)
             if markers:
                 if i - self.ylim != self.origin[1]:
                     self.text(fontsize / dx, (i - self.ylim - self.origin[1]) * oy,
                               str((round((i - self.ylim - self.origin[1]) * oy, 2))),
                               fontsize=fontsize, colour=colour, opac=0.6)
 
-    def arrow(self, x1, y1, x2, y2, scale, colour, strokewidth):
+    def arrow(self, x1, y1, x2, y2, scale=1, colour='white', strokewidth=2):
         """
         Draws a line from (x1, y1) to (x2, y2)
         :param x1: float
             Start x coordinate
         :param y1: float
             Start y coordinate
         :param x2: float
@@ -257,17 +263,18 @@
             Size of the arrow
         :param : string
             Colour of the arrow
         :param strokewidth: float
             Width of arrow tail
         :return: None
         """
+        strokewidth = strokewidth * self.nscale
+        scale = scale * self.nscale
         self.svg.draw_arrow(x1, y1, x2, y2, scale, stroke=colour, strokewidth=strokewidth)
 
-
     def plot(self, func, colour="red", strokewidth=1.5, opac=1, n=500):
         """
         Graphs the given function
         :param func: function
             function to be plotted
         :param colour: string
             colour of the curve
@@ -275,14 +282,15 @@
             width of curve
         :param opac: string
             opacity of the curve
         :param n: int
             Number of points used in the curve
         :return: None
         """
+        strokewidth = strokewidth * self.nscale
         eps = self.xlim / n
         X = [self.tranx(i * eps - self.origin[0]) for i in range(-n, n + 1)]
         Y = [self.trany(func(i * eps - self.origin[0])) for i in range(-n, n + 1)]
         self.svg.draw_polyline(X, Y, colour=colour, strokewidth=strokewidth, opac=opac)
 
     def graph_polar(self, func, colour="red", strokewidth=1.5, opac=1, n=500):
         """
@@ -295,21 +303,22 @@
             width of curve
         :param opac: string
             opacity of the curve
         :param n: int
             Number of points used in the curve
         :return: None
         """
-
+        strokewidth = strokewidth * self.nscale
         eps = self.xlim / n
         X = [self.tranx(i * eps - self.origin[0]) for i in range(-n, n + 1)]
         Y = [self.trany(func(i * eps - self.origin[0])) for i in range(-n, n + 1)]
         self.svg.draw_polyline(X, Y, colour=colour, strokewidth=strokewidth, opac=opac)
 
     def area(self, func, limits, colour="red", area_colour="orange", strokewidth=0, opac=1, n=500):
+        strokewidth = self.nscale * strokewidth
         eps = (limits[1] - limits[0]) / n
         X = [self.tranx(i * eps + limits[0]) for i in range(n + 1)]
         X.append(self.tranx(limits[1]))  # Ensure uniform area
         Y = [self.trany(func(i * eps + limits[0])) for i in range(n + 1)]
         Y.append(self.trany(func(limits[0])))  # Ensure uniform area
         self.svg.draw_polyline(X, Y, colour=colour, strokewidth=strokewidth, opac=opac, fill=area_colour)
 
@@ -324,223 +333,286 @@
                width of curve
            :param opac: string
                opacity of the curve
            :param n: int
                Number of points used in the curve
            :return: None
            """
+        strokewidth = self.nscale * strokewidth
         eps = self.xlim / n
         X = [self.tranx(i * eps - self.origin[0]) if i % 15 > 7 else None for i in range(-n, n + 1)]
         Y = [self.trany(func(i * eps - self.origin[0])) for i in range(-n, n + 1)]
         self.svg.draw_polyline(X, Y, colour=colour, strokewidth=strokewidth, opac=opac)
 
-    def plot_points(self, X, Y, colour="red", strokewidth=1, opac=1):
+    def plot_points(self, X, Y, colour="red", strokewidth=1, opac=1, style='none', fill='none', fill_opacity = 1):
         """
         Graphs the inputted points
         :param X:
         :param Y:
         :param colour:
         :param strokewidth:
         :param opac:
         :return:
         """
+        strokewidth = strokewidth * self.nscale
         X1 = [self.tranx(x) for x in X]
         Y1 = [self.trany(y) for y in Y]
-        self.svg.draw_polyline(X1, Y1, colour=colour, strokewidth=strokewidth, opac=opac)
+        self.svg.draw_polyline(X1, Y1, colour=colour, strokewidth=strokewidth, opac=opac, fill=fill, fill_opacity=fill_opacity)
 
     def scatter(self, X, Y, s=1, colour="white", opac=1):
         """
         Scatter plots the points X,Y
         :param X: list
         :param Y: list
         :param s: float
         :param colour: string
         :param opac: float (0-1)
         :return: None
         """
+        s = s * self.nscale
         if len(X) != len(Y):
             print("Data sets are misaligned!")
         for i in range(len(X)):
             self.svg.draw_circ(self.tranx(-X[i]), self.trany(Y[i]), s, fill=colour, stroke=colour,
                                strokewidth=0, opac=opac)
 
-    def param_label(self, x, y, label, s, stroke="white", strokewidth=12):
-        text = "%s = %s" % (label, s)
-        self.text(x, y, text, strokewidth=strokewidth, stroke=stroke)
-
-    def embed_latex(self, expr, x, y, width=200, height=200, colour="white", size=45):
-        A = LaText("expr.png", 0.5, 0.5, expr, colour=colour, size=size)
-        A.save()
-        self.svg.embed_image(self.tranx(x) - width / 2, self.trany(y) - height / 2, width=width,
-                             height=height, href=os.getcwd() + "/expr.png")
-
-    def embed_latex_anim(self, expr, x, y, width=200, height=200, colour="white", size=45):
-        A = LaText(os.getcwd() + "/Plots/expr.png", 0.5, 0.5, expr, colour=colour, size=size)
-        A.save()
-        self.svg.embed_image(self.tranx(x) - width / 2, self.trany(y) - height / 2, width=width,
-                             height=height, href=os.getcwd() + "/Plots/expr.png")
+    def add_latex(self, expr, x0, y0, scale=1, rotation=0, centre_align=True, colour=None, preamble=None,
+                  usepackages=None, cleanup=True, opacity=1, background=False, bg_colour='black', bg_opacity=.4,
+                  box=False, boxcolour='white', boxwidth=2, boxmult=1.6):
+        scale = scale * self.nscale
+        if expr in self.latex_history:
+            tex_info = self.latex_history[expr]
+            expr_code, w_expr, h_expr = tex_info[0].replace('fill-opacity:1', f'fill-opacity:{round(opacity, 3)}'), \
+                                        tex_info[1], tex_info[2]
+        else:
+            expr_code, w_expr, h_expr = latex_expression(expr, colour=colour, preamble=preamble,
+                                                         usepackages=usepackages,
+                                                         cleanup=cleanup)
+            # Data processing
+            index = len(self.latex_history)
+            symbols = get_svg_symbol_ids(expr_code)
+            clips = get_svg_clip_ids(expr_code)
+            for symb in symbols:
+                expr_code = expr_code.replace(symb, symb + f'-{index}')
+            for clip in clips:
+                expr_code = expr_code.replace(clip, clip + f'-{index}')
+
+            self.latex_history[expr] = [expr_code, w_expr, h_expr, colour]
+
+            expr_code = expr_code.replace('fill-opacity:1', f'fill-opacity:{round(opacity, 3)}')
+
+        mata = scale * np.cos(rotation)
+        matc = scale * np.sin(rotation)
+        matb = -scale * np.sin(rotation)
+        matd = scale * np.cos(rotation)
+        if centre_align:
+            mate = self.width / 2 + x0 * self.xscale - scale * (
+                    np.cos(rotation) * w_expr + np.sin(rotation) * h_expr) / 2
+            matf = self.height / 2 - y0 * self.yscale - scale * (
+                    -np.sin(rotation) * w_expr + np.cos(rotation) * h_expr) / 2
+        else:
+            mate = self.width / 2 + x0 * self.xscale
+            matf = self.height / 2 - y0 * self.yscale
+
+        if background:
+            self.svg.draw_rect(mate + scale * w_expr / 2, matf + scale * h_expr / 2, w_expr * scale, h_expr * scale,
+                               fill=bg_colour, opacity=bg_opacity,
+                               strokewidth=0)
+
+        if box:
+            self.svg.draw_rect(mate + scale * w_expr / 2, matf + scale * h_expr / 2, w_expr * scale * boxmult,
+                               h_expr * scale * boxmult, 'None', strokewidth=boxwidth,
+                               stroke=boxcolour)
+
+        self.svg.canvas += f'<g transform="matrix({mata}, {matb},{matc}, {matd}, {mate}, {matf})">\n'
+        self.svg.canvas += expr_code
+        self.svg.canvas += '</g>\n'
 
-    # Construction
+    # Constructions
 
     def draw_arrow(self, x1, y1, x2, y2, scale=1, colour="black", strokewidth=1):
+        strokewidth = strokewidth * self.nscale
+        scale = scale * self.nscale
         self.svg.draw_arrow(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), scale, stroke=colour,
                             strokewidth=strokewidth)
 
+    def draw_arrow2(self, x1, y1, x2, y2, scale=1, colour="black", strokewidth=1):
+        strokewidth = strokewidth * self.nscale
+        scale = scale * self.nscale
+        self.svg.draw_arrow2(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), scale, stroke=colour,
+                             strokewidth=strokewidth)
+
     def draw_double_arrow(self, x1, y1, x2, y2, scale=1, colour="black", strokewidth=1):
+        strokewidth = strokewidth * self.nscale
+        scale = scale * self.nscale
         self.svg.draw_arrow(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), scale, stroke=colour,
                             strokewidth=strokewidth)
         self.svg.draw_arrow(self.tranx(x2), self.trany(y2), self.tranx(x1), self.trany(y1), scale, stroke=colour,
                             strokewidth=strokewidth)
 
+    def draw_polygon(self, X, Y, fill="none", colour="black", strokewidth=1, fill_opacity=1):
+        strokewidth = strokewidth * self.nscale
+        X1 = [self.tranx(x) for x in X]
+        Y1 = [self.trany(y) for y in Y]
+        self.svg.draw_polygon(X1, Y1, fill=fill, stroke=colour, strokewidth=strokewidth, opacity=fill_opacity)
 
-    def draw_circle(self, x, y, r, fill="none", colour="black", strokewidth=1):
+    def draw_circle(self, x, y, r, fill="none", colour="black", strokewidth=1, fill_opacity=1):
+        strokewidth = strokewidth * self.nscale
         self.svg.draw_circ(self.tranx(x), self.trany(y), self.xscale * r, fill=fill, stroke=colour,
-                           strokewidth=strokewidth)
+                           strokewidth=strokewidth, fill_opacity=fill_opacity)
 
-    def draw_line(self, x1, y1, x2, y2, colour="black", strokewidth=1, opacity=1, cap="butt"):
-        self.svg.draw_line(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), stroke=colour,
-                           strokewidth=strokewidth, opacity=opacity, cap=cap)
-
-    def draw_rect(self, x, y, width, height, fill, colour="black", strokewidth=1, opac=1):
+    def draw_rect(self, x, y, width, height, fill, colour="black", strokewidth=1, opac=1, fill_opacity=1):
+        strokewidth = strokewidth * self.nscale
         self.svg.draw_rect(self.tranx(x), self.trany(y), abs(self.xscale * (width)),
-                           self.yscale * height, fill, stroke=colour, strokewidth=strokewidth, opacity=opac)
+                           self.yscale * height, fill, stroke=colour, strokewidth=strokewidth, opacity=opac,
+                           fill_opacity=fill_opacity)
+
+    def draw_ellipse(self, x, y, rx, ry, fill="none", fill_opacity=1, colour="black", strokewidth=1):
+        strokewidth = strokewidth * self.nscale
+        self.svg.draw_ellipse(self.tranx(x), self.trany(y), self.nscale * rx, self.nscale * ry, fill=fill,
+                              stroke=colour,
+                              strokewidth=strokewidth, fill_opacity=fill_opacity)
+
+    def cubic_bezier(self, path, colour="red", strokewidth=2, opacity=1, fill="none"):
+        pathstr = f'M {self.tranx(path[0, 0])} {self.trany(path[0, 1])} C '
+        strokewidth = strokewidth * self.nscale
+        for i in range(1, 4):
+            pathstr += f'{self.tranx(path[i, 0])} {self.trany(path[i, 1])},'
+
+        self.svg.draw_path(pathstr[:-1], colour=colour, strokewidth=strokewidth, opac=opacity, fill=fill)
+
+
+    def quadratic_bezier(self, path, colour="red", strokewidth=2, opacity=1, fill="none"):
+        pathstr = f'M {self.tranx(path[0, 0])} {self.trany(path[0, 1])} Q '
+        strokewidth = strokewidth * self.nscale
+        for i in range(1, 3):
+            pathstr += f'{self.tranx(path[i, 0])} {self.trany(path[i, 1])},'
+
+        self.svg.draw_path(pathstr[:-1], colour=colour, strokewidth=strokewidth, opac=opacity, fill=fill)
+
+    def draw_path(self, path, colour="red", strokewidth=2, opacity=1, fill="none", fill_opacity = 0):
+        strokewidth = strokewidth * self.nscale
+        pobj = parse_path(path)
+        print('rr', (pobj))
+        translated_pobj = convert_points2giraphics2(pobj, self.tranx, self.trany)
+        print('ll', len(translated_pobj))
+        cc = path2svg(translated_pobj)
+        self.svg.draw_path(cc, colour=colour, strokewidth=strokewidth, opac=opacity, fill=fill, fill_opacity = fill_opacity)
 
     def draw_line(self, x1, y1, x2, y2, marker="*", colour="black", strokewidth=1, opacity=1, cap="butt",
-                  segments=20, dotted=False):
-        if not dotted:
-            self.svg.draw_line(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), stroke=colour,
-                               strokewidth=strokewidth, opacity=opacity, cap=cap)
-        else:
-            self.svg.draw_dotted_line(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), marker=marker,
-                                      stroke=colour,
-                                      strokewidth=strokewidth, opacity=opacity, cap=cap, segments=segments)
-
-    def point(self, x, y, s=1, colour="white"):
-        self.draw_circle(x, y, 15 * s / self.width, fill=colour, strokewidth=0)
-
-    def save(self):
-        if len(self.TexLoader) != 0:
-            for t in self.TexLoader:
-                self.math_text(t[0], t[1], t[2], colour=t[3], scale=t[4])
-        """
-        Saves the plot and clears the svg.canvas
-        """
+                  segments=20, style=None):
+        strokewidth = strokewidth * self.nscale
+        self.svg.draw_line(self.tranx(x1), self.trany(y1), self.tranx(x2), self.trany(y2), stroke=colour,
+                           strokewidth=strokewidth, opacity=opacity, cap=cap, style=style)
+
+    def draw_arc(self, x, y, r, start, stop, colour="red", strokewidth=2, opac=1, fill="none", fixflag=False):
+        strokewidth = strokewidth * self.nscale
+        self.svg.draw_arc(self.tranx(x), self.trany(y), r * self.xscale, start, stop, colour=colour,
+                          strokewidth=strokewidth, opac=opac, fill=fill, fixflag=fixflag)
+
+    def point(self, x, y, s=1, colour="white", opacity=1):
+        s = s * self.nscale
+        self.draw_circle(x, y, 15 * s / self.width, fill=colour, strokewidth=0, fill_opacity=opacity)
+
+    def update_properties(self, width=None, height=None, xlim=None, ylim=None, transform=None):
+        if width is not None:
+            self.width = width
+        if height is not None:
+            self.height = height
+        if xlim is not None:
+            self.xlim = xlim
+        if ylim is not None:
+            self.ylim = ylim
+        if transform is not None:
+            self.transform = transform
+        self.__init__(self.width, self.height, self.xlim, self.ylim, self.name, origin=self.origin,
+                      transform=self.transform)
+
+    def save(self, clear=False):
         self.svg.save()
-        self.svg.canvas = ""
+
+        if clear:
+            self.svg.canvas = ""
+
+    # def save(self, clear=False):
+    #     if len(self.TexLoader) != 0:
+    #         for t in self.TexLoader:
+    #             self.math_text(t[0], t[1], t[2], colour=t[3], scale=t[4])
+    #     """
+    #     Saves the plot and clears the svg.canvas
+    #     """
+    #     self.svg.save()
+    #     if clear:
+    #         self.svg.canvas = ""
 
     def jupyter_display(self, raster=False):
         self.save()
         print(os.getcwd())
         if not raster:
-            return IPSVG(filename=os.getcwd()+'/'+self.name)
+            return IPSVG(filename=os.getcwd() + '/' + self.name)
         else:
-            convert_image(self.name+'.svg', self.name+'.png')
-            return Image(filename=self.name+'.png')
+            convert_image(self.name + '.svg', self.name + '.png')
+            return Image(filename=self.name + '.png')
 
     def display(self):
         """
         Displays the plot in a webbrowser
         """
         if platform.system() == "Darwin":
             webbrowser.get("open -a /Applications/Google\ Chrome.app %s").open(os.getcwd() + "/" + self.name)
         elif platform.system() == "Windows":
             webbrowser.get('chrome').open('file://' + os.getcwd() + "/" + self.name)
         else:
             print("OS error, your os is ", platform.system())
 
-
-"""
-def func(x):
-    return 0.04 * x ** 2 * math.sin(6 * x) + 5
-
-def sq(x):
-    return x * x
-
-f = Figure(600, 500, 15, 10, "fig.svg", origin=[-0, -0])
-f.plot(func)
-f.axes(colour="black")
-f.scatter([0.1 * i for i in range(-1500, 1500)], [sq(0.1 * i) for i in range(-1500, 1500)], colour="black")
-f.save()
-f.display()
-"""
-''' 
-
-def g(s):
-    def f(x):
-        return x**4 + s
-    return f
-g1 = g(0)
-g2 = g(1)
-g3 = g(2)
-g4 = g(3)
-
-g = Graph(800, 800, 5, 5, "50sd.svg", origin=[-2.,-2.])
-g.bg("black")
-g.axes(colour="white")
-g.ticks(markers=True)
-#g.grid(grids=[10,10], colour="white", stroke_width=0.5, opac=0.5)
-#g.ticks(markers=True, tick=5)
-
-#g.plot(f, "blue")
-# g.embed_latex("$x^2+y^2=1$", 0, 0)
-#dt = math.pi * 2 / 100
-#g.svg.draw_arrow(23, 200, 34, 44, stroke="white")m
-g.plot(g1)
-g.plot(g2)
-g.save()
-
-
-'''
-'''
-def f(s):
-    def k(x):
-        return math.sin(x) + s -5
-    return k
-
-if __name__ == "__main__":
-    A = Graph(1000,1000,5,5,"c1.svg", origin=[0,0])
-    A.bg(colour="black")
-    A.axes(colour="yellow")
-    for i in range(12):
-        A.plot(f(i))
-    A.grid(colour="white")
-    A.save()
-    A.display()
-
-'''
-
-#
 # def f(x):
 #     return x
 #
 #
 # def g(x):
 #     return x * x
-#
-#
-# A = Graph(400, 400, 5, 5, 'svg.svg', origin=[-5, -5])
-# A.bg()
+# # #
+# # #
+# A = Graph(400, 400, 5, 5, 'svg2.svg', origin=[0, 0])
+# A.bg(colour='black')
 # A.axes()
-# A.grid()
+# x, y = 3, 3
+# A.draw_arrow2(1, 0, 3, 3, scale=2, colour='white')
+# # A.point(x, y, s = .4, colour='red')
+# A.ticks()
+# A.draw_polygon([0,2,1], [0,0,1], colour='white', fill='white',fill_opacity=.2)
+# A.grid([5,5])
 # A.ticks(markers=True)
-# A.plot(f)
-# A.plot(g)
-#
-# A.draw_dotted_line(0, 0, 6, 7, stroke="white", marker=".")
+# # A.svg.draw_arrowhead2(200, 200, 10, 2,colour='white')
 # A.save()
 # A.display()
-#
-#
-# g = Graph(1000,1000,3,3,'giraphics.svg')
-# g.bg(colour="black")
-# g.math_text('GiraFix', 0,0)
-# g.save()
-# # g.display()
-# G = Graph(1000,1000,10,10,'ss')
-#
-# from giraphics.utilities.timer import Timer
-#
-#
-# t = Timer()
-# t.start()
-# G.tranx1(100)
-# t.stop()
+
+# # #
+# from giraphics.utilities.utils import getAngle
+# a,b = getAngle(0,0, 1,1)
+# print(a+b, a-b)
+
+# A.ticks(markers=True)
+# A.text(0,0,'hello', colour='white')
+# # A.plot(f)
+# # A.plot(g)
+# # A.add_latex('$x_1$', 0, 0, background=False, colour='white', scale=4, centre_align=False,
+# #             box=True,boxcolour='white', boxwidth=2, opacity=1)
+# #
+# # A.add_latex2('a', 0, 0, scale=6, rotation=0*np.pi/2, colour=[0,0,0])
+# #
+# # A.add_latex2('b', 2, 3, scale=6, rotation=0*np.pi/2, colour=[0,0,0])
+# #
+# # # # A.draw_dotted_line(0, 0, 6, 7, stroke="white", marker=".")
+# # A.add_inset(2,2,2,2,position=[3,3])
+# # A.bg(colour='blue')
+# # A.grid()
+# # # A.draw_arrow(0,0, 4,4,colour='white')
+# # A.axes()
+# # # A.draw_rect(0,0,8,8,'none', colour='white')
+# # # A.draw_arrow2(0,0, -4,-4, colour='white')
+# # A.draw_line(0,0, 4, 0, colour='white')
+# # A.draw_line(0,0, 4, 4, colour='white', style='dotted')
+# # A.draw_arc(0,0, 3, 0, -np.pi/4)
+# A.save()
+# #
+# # # A.display()
```

### Comparing `giraphics-0.0.5/giraphics/graphing3d/graph3d.py` & `giraphics-0.0.6/giraphics/graphing3d/graph3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from giraphics.utilities.convert import *
-from giraphics.graphing.fancygraphs import *
+from giraphics.graphing.fancygraph import *
 import numpy as np
 from math import cos, sin
 
 
 def lorentz(x0,y0,z0,N, a = 1 , s= 1, b =1 , eps = 0.01):
     X, Y, Z = [x0], [y0], [z0]
     x, y, z = 0,0,0
```

### Comparing `giraphics-0.0.5/giraphics/graphing3d/graph3d2.py` & `giraphics-0.0.6/giraphics/graphing3d/graph3d2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from giraphics.utilities.convert import *
-from giraphics.graphing.fancygraphs import *
+from giraphics.graphing.fancygraph import *
 import numpy as np
 from math import pi
 from numpy import sin, cos
 
 
 def Rz(theta, r=1):
     return np.array([[cos(theta), -sin(theta), 0], [sin(theta), cos(theta), 0], [0, 0, 1]])
@@ -44,15 +44,15 @@
     A.save()
 print('l')
 create_raster_batch("Plotsr", 'g', 'p', 'plotsrast', frames)
 create_mpeg('LiveLorent3.mp4', 'p', frames, dir=os.getcwd() + "/plotsrast")
 
 '''
 
-class Graph3d(FancyGraphs):
+class Graph3d(FancyGraph):
     def surface(self, func, rotator, yn = 60, xn = 60):
         mesh = np.mgrid[-5:5.1:0.5, -5:5.1:0.5]
         X = np.linspace(-self.xlim, self.xlim, xn)
         Y = np.linspace(-self.ylim, self.ylim, yn)
         Z = func(X, Y)
         P = np.matmul(rotator, np.column_stack((X,Y,Z)).T)
         for i in range(yn):
@@ -79,15 +79,15 @@
             for i in range(density):
                 X = r * sin(theta) * cos(phi[i]) + cx
                 Y = r * sin(theta) * sin(phi[i]) + cy
                 Z = r * cos(theta) + cz
                 P = np.matmul(rotator, np.column_stack((X, Y, Z)).T)
                 self.plot_points(P[0], P[1], colour=colour)
 
-    def axes_3d(self, rotator):
+    def axes3d(self, rotator):
         vecspos = np.array([[1,0,0], [0,1,0], [0,0,1]])*self.xlim
         vecsneg = -np.array([[1,0,0], [0,1,0], [0,0,1]])*self.xlim
         V1 = np.matmul(rotator, vecspos)
         V2 = np.matmul(rotator, vecsneg)
         self.svg.draw_arrow(self.tranx(V2[0][0]),self.trany(V2[0][1]), self.tranx(V1[0][0]), self.trany(V1[0][1]),stroke="white")
         self.svg.draw_arrow(self.tranx(V2[1][0]),self.trany(V2[1][1]),self.tranx(V1[1][0]), self.trany(V1[1][1]),stroke="white")
         self.svg.draw_arrow(self.tranx(V2[2][0]),self.trany(V2[2][1]),self.tranx(V1[2][0]), self.trany(V1[2][1]),stroke="white")
@@ -97,26 +97,27 @@
 
     def Rx(self,theta, r=1):
         return np.array([ [0, 0, 1],[cos(theta), -sin(theta), 0], [sin(theta), cos(theta), 0]])
 
     def Ry(self,theta, r=1):
         return np.array([[cos(theta), 0, sin(theta)], [0, 1, 0], [-sin(theta), 0, cos(theta)]])
 
-frames = 200
-create_directory("Plotsr")
-create_directory("plotsrast")
-
-def rtr(t, w = 0.02):
-    return np.matmul(Rz(0.33), Ry(w*t))
-def funx(x,y):
-    return -0.3*(x**2 + sin(y))
-
-for i in range(frames):
-    A = Graph3d(1000, 1000, 30, 30, "Plotsr/g" + namer(i) + ".svg")
-    A.bg("black")
-    A.surface(funx, rtr(i))
-    A.axes_3d(rtr(i))
-   # A.mesh_sphere(6, 0, 0, 0, rotator=rtr(i))
-    A.save()
-
-create_raster_batch("Plotsr", 'g', 'p', 'plotsrast', frames)
-create_mpeg('../../sample_projects/Videos/surf1.mp4', 'p', frames, dir=os.getcwd() + "/plotsrast")
+# frames = 200
+# create_directory("Plotsr")
+# create_directory("plotsrast")
+#
+# def rtr(t, w = 0.02):
+#     return np.matmul(Rz(0.33), Ry(w*t))
+# def funx(x,y):
+#     return -0.3*(x**2 + sin(y))
+#
+# for i in range(frames):
+#     A = Graph3d(1000, 1000, 30, 30, "Plotsr/g" + namer(i) + ".svg")
+#     A.bg("black")
+#     A.surface(funx, rtr(i))
+#     A.axes_3d(rtr(i))
+#    # A.mesh_sphere(6, 0, 0, 0, rotator=rtr(i))
+#     A.save()
+#
+# create_raster_batch("Plotsr", 'g', 'p', 'plotsrast', frames)
+# create_mpeg('../../sample_projects/Videos/surf1.mp4', 'p', frames, dir=os.getcwd() + "/plotsrast")
+class Animation
```

### Comparing `giraphics-0.0.5/giraphics/utilities/convert.py` & `giraphics-0.0.6/giraphics/utilities/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,16 +94,37 @@
         p.start()
 
 def create_raster_batch(dir, filename, savename, savedir, num):
     for i in range(num):
         command = ("rsvg-convert {}/{}/{}{}.svg -o {}/{}/{}{}.png").format(os.getcwd(), dir, filename, namer(i), os.getcwd(), savedir, savename, namer(i))
         os.system(command)
 
+def crb_wrap(dir, filename, savename, savedir):
+    cwd = os.getcwd()
+    def inner(i):
+        command = ("rsvg-convert {}/{}/{}{}.svg -o {}/{}/{}{}.png").format(cwd, dir, filename, f'{i:04}',
+                                                                           cwd, savedir, savename, f'{i:04}')
+        print(command)
+        os.system(command)
+    return inner
+
+
+def create_raster_parallel(dir, filename, savename, savedir, num, pools=2):
+    if pools == 'all':
+        pools = multiprocessing.cpu_count()
+    f = crb_wrap(dir,filename,savename, savedir)
+    print(f)
+    p = multiprocessing.Pool(pools)
+    p.map(f, range(num))
+    p.close()
+    p.join()
+
+
 # create_raster_batch("ftp", 'g', 'p', 'ftprast', 1)
-def create_mpeg(filename, batchname, num, dir, framerate='60', warnings=True, overwrite=True):
+def create_mpeg(filename, batchname, dir, framerate='60', warnings=True, overwrite=True):
     if warnings:
         w = '-loglevel warning'
     else:
         w = ''
     if overwrite:
         y = '-y'
     else:
```

### Comparing `giraphics-0.0.5/giraphics/utilities/latext.py` & `giraphics-0.0.6/giraphics/utilities/latext.py`

 * *Files identical despite different names*

### Comparing `giraphics-0.0.5/giraphics/utilities/utils.py` & `giraphics-0.0.6/giraphics/utilities/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,89 @@
 import numpy as np
-from math import cos, sin
+from math import cos, sin, atan, pi, atan2
+
 import time
 
+
 class Timer:
     """
     Times code between the start() and stop()
     """
+
     def __init__(self, text="Elapsed time: {:0.4f} seconds", logger=print):
         self._start_time = None
         self.text = text
         self.logger = logger
+
     def start(self, label="task"):
         """
         Starts the timer when run
         :param label: Label of the timer
         """
         self.label = label
         self.t1 = time.time()
+
     def stop(self):
         """
         Stops the timer when run and prints the time taken to complete the task
         :return:
         """
         self.t2 = time.time()
-        print("Time lapsed for %s: %s" % (self.label, self.t2-self.t1))
+        print("Time lapsed for %s: %s" % (self.label, self.t2 - self.t1))
+
 
 def listlike(var):
     """
     Takes a variable and returns the variable in a list if it is not already a list
     :param var: variable
     :return: List
     """
     if isinstance(var, list):
         return var
     else:
         return [var]
 
 
+def getAngle(x1, y1, x2, y2):
+    if x1 - x2 != 0:
+        if x1 - x2 < 0:
+            ang = atan((y2 - y1) / (x2 - x1)) + pi / 2
+        else:
+            ang = atan((y2 - y1) / (x2 - x1)) - pi / 2
+    else:
+        if y2 - y1 < 0:
+            ang = 0
+        else:
+            ang = pi
+    return ang
+
+
 def max2d(arr):
-    m,n = 0, 0
+    m, n = 0, 0
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             if arr[i][j] >= arr[m][n]:
                 m, n = i, j
-    return arr[m,n]
+    return arr[m, n]
+
 
 def min2d(arr):
-    m,n = 0, 0
+    m, n = 0, 0
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             if arr[i][j] <= arr[m][n]:
                 m, n = i, j
-    return arr[m,n]
+    return arr[m, n]
 
 
 # Velocity Distribution
 def identity(t):
     return t
 
+
 def TopHeavy(i, k=4):
     return i ** k
 
 
 def BottomHeavy(i, k=0.25):
     return i ** k
 
@@ -85,14 +107,21 @@
 def norm(x):
     t = 0
     for v in x:
         t += v ** 2
     return t ** (0.5)
 
 
+def parity(x):
+    if x >= 0:
+        return 1
+    else:
+        return -1
+
+
 # Rotations 3D
 def Rx(theta, r=1):
     return np.array([[cos(theta), -sin(theta), 0], [sin(theta), cos(theta), 0], [0, 0, 1]])
     pass
 
 
 def Rz(theta, r=1):
```

### Comparing `giraphics-0.0.5/setup.py` & `giraphics-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from distutils.core import setup
 setup(
   name = 'giraphics',
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   packages=['giraphics', 'giraphics.graphing', 'giraphics.animate', 'giraphics.svg', 'giraphics.graphing3d',
             'giraphics.utilities'],
   description = 'Lightweight graphing and animations',
   author = 'T. G. Hiranandani',
   author_email = 'giraphics@protonmail.com',
   url = 'https://github.com/tghira/giraphics',
   keywords = ['graphs', 'animations', 'graphics', 'vector-graphics'],
   install_requires=[
           'numpy',
+          'IPython',
       ],
 
   classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

