# Comparing `tmp/solarkit-0.1.tar.gz` & `tmp/solarkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarkit-0.1.tar", last modified: Sun May  7 17:19:23 2023, max compression
+gzip compressed data, was "solarkit-0.1.1.tar", last modified: Mon May  8 17:31:06 2023, max compression
```

## Comparing `solarkit-0.1.tar` & `solarkit-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 17:19:23.821237 solarkit-0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.1/LICENSE
--rw-rw-rw-   0        0        0     1654 2023-05-07 17:19:23.820238 solarkit-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1055 2023-05-07 17:17:01.000000 solarkit-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 17:19:23.821237 solarkit-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-07 17:09:44.000000 solarkit-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:19:23.813240 solarkit-0.1/solarkit/
--rw-rw-rw-   0        0        0      117 2023-05-01 16:29:31.000000 solarkit-0.1/solarkit/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.1/solarkit/planet.py
--rw-rw-rw-   0        0        0     2867 2023-05-06 19:41:16.000000 solarkit-0.1/solarkit/solar_system.py
--rw-rw-rw-   0        0        0     2072 2023-05-07 16:25:21.000000 solarkit-0.1/solarkit/utils.py
--rw-rw-rw-   0        0        0    11888 2023-05-07 17:04:12.000000 solarkit-0.1/solarkit/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:19:23.819238 solarkit-0.1/solarkit.egg-info/
--rw-rw-rw-   0        0        0     1654 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:06.176398 solarkit-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2003 2023-05-08 17:31:06.175897 solarkit-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-05-08 17:28:30.000000 solarkit-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:31:06.176398 solarkit-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-08 17:30:45.000000 solarkit-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:06.168896 solarkit-0.1.1/solarkit/
+-rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-0.1.1/solarkit/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.1.1/solarkit/planet.py
+-rw-rw-rw-   0        0        0     2876 2023-05-08 17:27:06.000000 solarkit-0.1.1/solarkit/solar_system.py
+-rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-0.1.1/solarkit/utils.py
+-rw-rw-rw-   0        0        0    11976 2023-05-08 17:27:06.000000 solarkit-0.1.1/solarkit/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:06.173897 solarkit-0.1.1/solarkit.egg-info/
+-rw-rw-rw-   0        0        0     2003 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/top_level.txt
```

### Comparing `solarkit-0.1/LICENSE` & `solarkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solarkit-0.1/PKG-INFO` & `solarkit-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.1
+Version: 0.1.1
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -12,30 +12,33 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # solarkit - BPhO Computational challenge
-## A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations
 
+A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations.
 It was built as the first part of a two part subimission for the challenge. My idea is to create a website using django to allow anyone to use the simulation. Having this package will ensure clean, backend code that will do the work in just a couple of lines.
 
+* [Repo link](https://github.com/carlos-lorenzo/solarkit) (for PyPI)
+
 ### Challenges
 * Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
-1. pip install solarkit
-2. create .py file
-3. start experimenting! (follow example image for guidance)
+1. "pip install solarkit" or [download package files](https://github.com/carlos-lorenzo/solarkit/tree/main/Package) from repository and  install locally
+2. [Download](https://github.com/carlos-lorenzo/solarkit/blob/08a2d0ddc34b3abecce7789cbe7163d7d49cbd48/planet_data.csv) or create your own data
+3. Create .py file
+4. Start experimenting! (follow example image for guidance)
 
 ### Use example
 ![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
```

### Comparing `solarkit-0.1/README.md` & `solarkit-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # solarkit - BPhO Computational challenge
-## A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations
 
+A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations.
 It was built as the first part of a two part subimission for the challenge. My idea is to create a website using django to allow anyone to use the simulation. Having this package will ensure clean, backend code that will do the work in just a couple of lines.
 
+* [Repo link](https://github.com/carlos-lorenzo/solarkit) (for PyPI)
+
 ### Challenges
 * Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
-1. pip install solarkit
-2. create .py file
-3. start experimenting! (follow example image for guidance)
+1. "pip install solarkit" or [download package files](https://github.com/carlos-lorenzo/solarkit/tree/main/Package) from repository and  install locally
+2. [Download](https://github.com/carlos-lorenzo/solarkit/blob/08a2d0ddc34b3abecce7789cbe7163d7d49cbd48/planet_data.csv) or create your own data
+3. Create .py file
+4. Start experimenting! (follow example image for guidance)
 
 ### Use example
 ![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
```

### Comparing `solarkit-0.1/setup.py` & `solarkit-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1"
+VERSION = "0.1.1"
 DESCRIPTION = "Visualise a solar system and do cool stuff with it"
 
 # Setting up
 setup(
     name="solarkit",
     version=VERSION,
     author="Carlos Lorenzo",
```

### Comparing `solarkit-0.1/solarkit/planet.py` & `solarkit-0.1.1/solarkit/planet.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.1/solarkit/solar_system.py` & `solarkit-0.1.1/solarkit/solar_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 from typing import Dict, Optional
 
-from planet import Planet
+from solarkit.planet import Planet
 
 
 @dataclass
 class Solar_System:
     """
     Solar system class
```

### Comparing `solarkit-0.1/solarkit/utils.py` & `solarkit-0.1.1/solarkit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pickle
 
 import pandas as pd
 
-from planet import Planet
-from solar_system import Solar_System
+from solarkit.planet import Planet
+from solarkit.solar_system import Solar_System
 
 
 def create_planet(planet_data: pd.Series(object)) -> Planet:
     
     """
     Creates a planet from a pd.Series(object) containing the required data (reference Planet object parameters)
 
@@ -23,15 +23,15 @@
                                 R=planet_data["R"],
                                 trot=planet_data["trot"],
                                 P=planet_data["P"],
                                 colour=planet_data["colour"],)
     
     return new_planet
 
-def load_system(path: str):
+def load_system_from_csv(path: str):
     """
     Creates a system from a csv. Each row contains the required data (reference Planet object parameters)
 
     Args:
         path (str): The path to a .csv file
 
     Returns:
```

### Comparing `solarkit-0.1/solarkit/viewer.py` & `solarkit-0.1.1/solarkit/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from dataclasses import dataclass, field
 from typing import Optional, List, Dict
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from solar_system import Solar_System
-from planet import Planet
+from solarkit.solar_system import Solar_System
+from solarkit.planet import Planet
 
 
 @dataclass
 class Viewer:
     """
     Visualise (& more) a Solar_System object
 
     Args:
         system (Solar_System): A Solar_System object\n
         planets_to_use (List[str]): Select speficif planets (leave blank for all)\n
         compute_3D (bool): Show in 3D\n
         target_fps (int): Animation's fps\n
     """
+    
     system: Solar_System
     planets_to_use: List[str] = field(default_factory=list)
     compute_3D: Optional[bool] = field(default= False)
     target_fps: Optional[int] = field(default=30)
     
     orbit_data: Dict[str, Dict[str, List[float]]] = field(init=False, default_factory=dict)
     chosen_planets: List[Planet] = field(init=False, default=list)
@@ -108,26 +109,27 @@
     
     def show_plot(self):
         """
         Show drawn figure (calls plt.show())
         """
         plt.show()
     
-    def save_figure(self, filename: str) -> None:
+    def save_figure(self, path: str, filename: str) -> None:
         """_summary_
 
         Args:
-            filename (str): _description_
+            path (str): directory where the image will be stored
+            filename (str): name of image
         """
         
 
-        if not os.path.exists("figures"):
-            os.mkdir("figures")
+        if not os.path.exists(path):
+            os.mkdir(path)
         
-        plt.savefig(f"figures/{filename}", dpi=250)
+        plt.savefig(f"{path}/{filename}", dpi=250)
         
           
     def plot_orbit(self, orbit_data: Dict[str, List[float]]) -> None:
         """
         Plots the orbit of a planet
 
         Args:
```

### Comparing `solarkit-0.1/solarkit.egg-info/PKG-INFO` & `solarkit-0.1.1/solarkit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.1
+Version: 0.1.1
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -12,30 +12,33 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # solarkit - BPhO Computational challenge
-## A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations
 
+A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations.
 It was built as the first part of a two part subimission for the challenge. My idea is to create a website using django to allow anyone to use the simulation. Having this package will ensure clean, backend code that will do the work in just a couple of lines.
 
+* [Repo link](https://github.com/carlos-lorenzo/solarkit) (for PyPI)
+
 ### Challenges
 * Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
-1. pip install solarkit
-2. create .py file
-3. start experimenting! (follow example image for guidance)
+1. "pip install solarkit" or [download package files](https://github.com/carlos-lorenzo/solarkit/tree/main/Package) from repository and  install locally
+2. [Download](https://github.com/carlos-lorenzo/solarkit/blob/08a2d0ddc34b3abecce7789cbe7163d7d49cbd48/planet_data.csv) or create your own data
+3. Create .py file
+4. Start experimenting! (follow example image for guidance)
 
 ### Use example
 ![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
```

