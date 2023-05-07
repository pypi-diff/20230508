# Comparing `tmp/bismarkplot-0.2.5.tar.gz` & `tmp/bismarkplot-1.0.tar.gz`

## Comparing `bismarkplot-0.2.5.tar` & `bismarkplot-1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.github/workflows/main.yaml
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/BismarkPlot.iml
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/dbnavigator.xml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/vcs.xml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/.nojekyll
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/Makefile
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/conf.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/index.rst
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/make.bat
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/requirements.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/_templates/module.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/BarPlot.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/Bismark.py
--rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/BismarkFiles.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/BoxPlot.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/HeatMap.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/LinePlot.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/__init__.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/read_bismark.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/src/bismarkplot/read_genome.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/README.md
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    43438 2020-02-02 00:00:00.000000 bismarkplot-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bismarkplot-1.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bismarkplot-1.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/BismarkPlot.iml
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/dbnavigator.xml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/.nojekyll
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/Makefile
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/conf.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/index.rst
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/make.bat
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/requirements.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/_templates/module.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/BarPlot.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/Bismark.py
+-rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/BismarkFiles.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/BoxPlot.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/HeatMap.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/LinePlot.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/__init__.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/read_bismark.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/read_genome.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 bismarkplot-1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 bismarkplot-1.0/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 bismarkplot-1.0/pyproject.toml
+-rw-r--r--   0        0        0    43599 2020-02-02 00:00:00.000000 bismarkplot-1.0/PKG-INFO
```

### Comparing `bismarkplot-0.2.5/.github/workflows/publish.yaml` & `bismarkplot-1.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/.idea/dbnavigator.xml` & `bismarkplot-1.0/.idea/dbnavigator.xml`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/.idea/inspectionProfiles/Project_Default.xml` & `bismarkplot-1.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/docs/Makefile` & `bismarkplot-1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/docs/conf.py` & `bismarkplot-1.0/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 project = 'BismarkPlot'
 copyright = '2023, shitohana'
 author = 'shitohana'
-release = '0.2.5'
+release = '1.0'
 import os
 import sys
 sys.path.insert(0, os.path.abspath('../src'))
 sys.path.append(os.path.abspath('.'))
 
 
 extensions = [
```

### Comparing `bismarkplot-0.2.5/docs/make.bat` & `bismarkplot-1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/BarPlot.py` & `bismarkplot-1.0/src/bismarkplot/BarPlot.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/Bismark.py` & `bismarkplot-1.0/src/bismarkplot/Bismark.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/BismarkFiles.py` & `bismarkplot-1.0/src/bismarkplot/BismarkFiles.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/BoxPlot.py` & `bismarkplot-1.0/src/bismarkplot/BoxPlot.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/HeatMap.py` & `bismarkplot-1.0/src/bismarkplot/HeatMap.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/LinePlot.py` & `bismarkplot-1.0/src/bismarkplot/LinePlot.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/read_bismark.py` & `bismarkplot-1.0/src/bismarkplot/read_bismark.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/src/bismarkplot/read_genome.py` & `bismarkplot-1.0/src/bismarkplot/read_genome.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/LICENSE.txt` & `bismarkplot-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bismarkplot-0.2.5/README.md` & `bismarkplot-1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # BismarkPlot
 A small library to plot Bismark ``methylation_exctractor`` reports.
 
 See the docs: https://shitohana.github.io/BismarkPlot
 
 Right now only ``coverage2cytosine`` input is supported, but support for ``bismark2bedGraph`` will be added soon.
 
+## Installation
+
+```commandline
+pip install bismarkplot
+```
+
 ## Example
 
 First we need to initialize ``genome`` and ``BismarkFiles``. ``genome`` is .gff or .bed file with gene coordinates. ``BismarkFiles`` is a class, which calculates data for all plots, so their types need to be specified when it is initialized.
 ```python
 import bismarkplot
 
 file = 'path/to/genome.gff'
@@ -39,32 +45,32 @@
     context='CG',
     strand='+',
     smooth=.05,
     labels = ['exp1', 'exp2'],
     title = 'Plot for CG+'
 ) 
 ```
-Result:
-![Plot for CG+](https://user-images.githubusercontent.com/43905117/236703691-023818e9-fb0d-47e6-a328-a712c9285928.png)
+
+<img alt="Plot for CG+" src="https://user-images.githubusercontent.com/43905117/236703691-023818e9-fb0d-47e6-a328-a712c9285928.png" width="" height="400"/>
+
 
 For heat maps use (or ``draw_heat_maps_all`` for all contexts)
 ```python
 bismark.draw_heat_maps_filtered(
     context='CG',
     strand='+',
     resolution=100,
     labels = ['exp1', 'exp2'],
     title = 'Heatmap for CG+'
 )   
 ```
 
-Result:
-![Heatmap for CG+](https://user-images.githubusercontent.com/43905117/236703690-b46c7579-3068-4e98-82f0-9a6435c7808b.png)
+<img alt="Heatmap for CG+" height="300" src="https://user-images.githubusercontent.com/43905117/236703690-b46c7579-3068-4e98-82f0-9a6435c7808b.png"/>
+
+
 For box plot or bar plot use
 ```python
 bismark.draw_box_plot(strand_specific=True, labels=['exp1', 'exp2'])
 bismark.draw_bar_plot(labels=['exp1', 'exp2'])
 ```
-
-Result
-![box_05_07_23:54.png](https://user-images.githubusercontent.com/43905117/236703689-9eaaa28a-1a98-4300-a0d0-83039ed9a541.png)
-![bar_05_07_23:54.png](https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png
+<img alt="box_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703689-9eaaa28a-1a98-4300-a0d0-83039ed9a541.png"/>
+<img alt="bar_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png"/>
```

### Comparing `bismarkplot-0.2.5/pyproject.toml` & `bismarkplot-1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bismarkplot"
-version = "0.2.5"
+version = "1.0"
 authors = [
   { name="shitohana", email="kyudytskiy@gmail.com" },
 ]
 keywords = ['bismark', 'methylation', 'plot']
 license = {file = "LICENSE.txt"}
 dependencies = [
     "matplotlib>=3.7.1",
```

### Comparing `bismarkplot-0.2.5/PKG-INFO` & `bismarkplot-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bismarkplot
-Version: 0.2.5
+Version: 1.0
 Summary: A small library to plot Bismark methylation_exctractor reports.
 Project-URL: Homepage, https://github.com/shitohana/BismarkPlot
 Project-URL: Documentation, https://shitohana.github.io/BismarkPlot/
 Project-URL: Bug Tracker, https://github.com/shitohana/BismarkPlot/issues
 Author-email: shitohana <kyudytskiy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -696,14 +696,20 @@
 # BismarkPlot
 A small library to plot Bismark ``methylation_exctractor`` reports.
 
 See the docs: https://shitohana.github.io/BismarkPlot
 
 Right now only ``coverage2cytosine`` input is supported, but support for ``bismark2bedGraph`` will be added soon.
 
+## Installation
+
+```commandline
+pip install bismarkplot
+```
+
 ## Example
 
 First we need to initialize ``genome`` and ``BismarkFiles``. ``genome`` is .gff or .bed file with gene coordinates. ``BismarkFiles`` is a class, which calculates data for all plots, so their types need to be specified when it is initialized.
 ```python
 import bismarkplot
 
 file = 'path/to/genome.gff'
@@ -734,32 +740,32 @@
     context='CG',
     strand='+',
     smooth=.05,
     labels = ['exp1', 'exp2'],
     title = 'Plot for CG+'
 ) 
 ```
-Result:
-![Plot for CG+](https://user-images.githubusercontent.com/43905117/236703691-023818e9-fb0d-47e6-a328-a712c9285928.png)
+
+<img alt="Plot for CG+" src="https://user-images.githubusercontent.com/43905117/236703691-023818e9-fb0d-47e6-a328-a712c9285928.png" width="" height="400"/>
+
 
 For heat maps use (or ``draw_heat_maps_all`` for all contexts)
 ```python
 bismark.draw_heat_maps_filtered(
     context='CG',
     strand='+',
     resolution=100,
     labels = ['exp1', 'exp2'],
     title = 'Heatmap for CG+'
 )   
 ```
 
-Result:
-![Heatmap for CG+](https://user-images.githubusercontent.com/43905117/236703690-b46c7579-3068-4e98-82f0-9a6435c7808b.png)
+<img alt="Heatmap for CG+" height="300" src="https://user-images.githubusercontent.com/43905117/236703690-b46c7579-3068-4e98-82f0-9a6435c7808b.png"/>
+
+
 For box plot or bar plot use
 ```python
 bismark.draw_box_plot(strand_specific=True, labels=['exp1', 'exp2'])
 bismark.draw_bar_plot(labels=['exp1', 'exp2'])
 ```
-
-Result
-![box_05_07_23:54.png](https://user-images.githubusercontent.com/43905117/236703689-9eaaa28a-1a98-4300-a0d0-83039ed9a541.png)
-![bar_05_07_23:54.png](https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png
+<img alt="box_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703689-9eaaa28a-1a98-4300-a0d0-83039ed9a541.png"/>
+<img alt="bar_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png"/>
```

