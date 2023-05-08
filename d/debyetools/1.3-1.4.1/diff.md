# Comparing `tmp/debyetools-1.3.tar.gz` & `tmp/debyetools-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/debyetools-1.3.tar", last modified: Tue Mar  7 19:21:38 2023, max compression
+gzip compressed data, was "dist/debyetools-1.4.1.tar", last modified: Mon May  8 19:48:26 2023, max compression
```

## Comparing `debyetools-1.3.tar` & `debyetools-1.4.1.tar`

### file list

```diff
@@ -1,36 +1,50 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-07 19:21:38.274836 debyetools-1.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2023-03-07 19:20:39.000000 debyetools-1.3/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2687 2023-03-07 19:21:38.274836 debyetools-1.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2023-03-07 19:20:39.000000 debyetools-1.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-07 19:21:38.270838 debyetools-1.3/debyetools/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11745 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/anharmonicity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/aux_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1844 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/debfunct.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8033 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/defects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3456 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/electronic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/fs_compound_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9911 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/layout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11113 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/ndeb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4175 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/pairanalysis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1909 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/poisson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160930 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/potentials.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-07 19:21:38.274836 debyetools-1.3/debyetools/tpropsgui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3017 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34346 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13857 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/functions0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42578 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10074 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/layout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/plotter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4349 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/plotter_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/tpropsgui/toolbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24920 2023-03-07 19:20:39.000000 debyetools-1.3/debyetools/vibrational.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-07 19:21:38.270838 debyetools-1.3/debyetools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2687 2023-03-07 19:21:38.000000 debyetools-1.3/debyetools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      809 2023-03-07 19:21:38.000000 debyetools-1.3/debyetools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-07 19:21:38.000000 debyetools-1.3/debyetools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2023-03-07 19:21:38.000000 debyetools-1.3/debyetools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-03-07 19:21:38.000000 debyetools-1.3/debyetools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-03-07 19:21:38.274836 debyetools-1.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2023-03-07 19:20:39.000000 debyetools-1.3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.363857 debyetools-1.4.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2023-05-08 19:47:31.000000 debyetools-1.4.1/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2642 2023-05-08 19:48:26.363857 debyetools-1.4.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2023-05-08 19:47:31.000000 debyetools-1.4.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.359857 debyetools-1.4.1/debyetools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11745 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/anharmonicity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6335 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/aux_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1844 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/debfunct.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8033 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/defects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3717 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/electronic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1436 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/fs_compound_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9911 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/layout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11113 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/ndeb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4926 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/pairanalysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3496 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/poisson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   161578 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/potentials.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4698 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/potentials_2.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.363857 debyetools-1.4.1/debyetools/tpropsgui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11483 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/atomtools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      268 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/dialog_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34356 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/functions0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/get_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42948 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/layout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8849 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/plot_EV.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/plotter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/plotter_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      883 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/toolbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16226 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_heatcapacitywindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18970 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_interatomic_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22118 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/window_cp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/window_interatomicparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24920 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/vibrational.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.359857 debyetools-1.4.1/debyetools.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2642 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1341 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       35 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-08 19:48:26.363857 debyetools-1.4.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2023-05-08 19:47:31.000000 debyetools-1.4.1/setup.py
```

### Comparing `debyetools-1.3/LICENSE.md` & `debyetools-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/PKG-INFO` & `debyetools-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 1.3
+Version: 1.4.1
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # debyetools
 
 Implementation of a tool for calculating self-consistent thermodynamic properties that can take into account all kinds of contributions to the free energy inluding explicit anharmonicity. The software presented here is based in the Debye approximation within the QHA using the crystal internal energetics parametrized at ground-state to project the thermodynamics properties at high temperatures.
```

### Comparing `debyetools-1.3/README.md` & `debyetools-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/anharmonicity.py` & `debyetools-1.4.1/debyetools/anharmonicity.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/aux_functions.py` & `debyetools-1.4.1/debyetools/aux_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     :param array center: The position in space where the system of reference is
 
     """
 
     cell_coords = np.array(list((it.product(np.arange(size[0]),
                                             np.arange(size[1]),
                                             np.arange(size[2])))))
+
     cell_coords_centered = cell_coords + center
     cell_coords_centered = np.dot(cell_coords_centered, primitive_cell)
 
     return cell_coords_centered
 
 def gen_Ts(Ti,Tf,nTs):
     """
@@ -50,39 +51,43 @@
     :param float Ti: Initial temperature. (Try not to use the value 0. Use 0.1 instead.)
     :param float Tf: Final temperature.
     :param int nTs: Number of values. This does not include room temperature, which is included anyways.
 
     :retun list_of_floats: Values of temperatures between Ti and Tf, inclusive, plus room temperature.
     """
     minF_step = (Tf - Ti)/(nTs - 1.)
-    Ts = np.arange(Ti, Tf+1, minF_step)
+    Ts = np.arange(Ti, Tf+minF_step, minF_step)
     Ts = np.r_[Ts, [298.15]]
     Ts.sort()
     return Ts
 def gen_Ps(Ti,Tf,nTs):
     """
     Function to generate a range of temperatures.
 
     :param float Ti: Initial temperature. (Try not to use the value 0. Use 0.1 instead.)
     :param float Tf: Final temperature.
     :param int nTs: Number of values. This does not include room temperature, which is included anyways.
 
     :retun list_of_floats: Values of temperatures between Ti and Tf, inclusive, plus room temperature.
     """
+    if nTs <= 1: return np.array([Ti])
     minF_step = (Tf - Ti)/(nTs - 1.)
     Ts = np.arange(Ti, Tf+1, minF_step)
-    Ts.sort()
+
     return Ts
 
-def load_doscar(filename_sufix):
+def load_doscar(filename_sufix, list_filetags = ['-0.10', '-0.09','-0.08','-0.07','-0.06','-0.05','-0.04','-0.03',
+                                                 '-0.02','-0.01','-0.00','0.01','0.02','0.03','0.04','0.05','0.06',
+                                                 '0.07','0.08','0.09','0.10']):
+    list_filetags = [str(li) for li in list_filetags]
     E = []
     N = []
     Ef = []
     nat = 0
-    for dosfile in ['-0.10', '-0.09','-0.08','-0.07','-0.06','-0.05','-0.04','-0.03','-0.02','-0.01','-0.00','0.01','0.02','0.03','0.04','0.05','0.06','0.07','0.08','0.09','0.10']:
+    for dosfile in list_filetags:
         countline = 0
         EN = []
 
         filename = filename_sufix+dosfile
         with open(filename) as infile:
                 for line in infile:
                     if countline == 0:
@@ -90,14 +95,15 @@
                     if countline == 5:
                         Ef.append(float(line.split()[3]))
                     if countline > 5:
                         EN.append(line.split()[0:2])
 
                     countline +=1
         ENAl = np.array(EN)
+        # print(dosfile, EN)
         E.append([float(s) for s in list(ENAl[:,0])])
         N.append([float(s)/nat for s in list(ENAl[:,1])])
 
     return E,N,Ef
 
 def load_V_E(energy_dir,energy_dir_contcar, units='eV/atom'):
     with open(energy_dir_contcar,'r') as f_poscar:
@@ -136,15 +142,15 @@
 
 def load_EM(filename_outcar_eps):
     EM = []
 
     with open(filename_outcar_eps) as f:
         lines = f.readlines()
         for i, line in enumerate(lines):
-            if line.startswith(' TOTAL ELASTIC MODULI (kBar)'):
+            if line.startswith('  SYMMETRIZED ELASTIC MODULI (kBar)'):
                 j = i + 3
                 data = lines[j:j+6]
                 break
 
     for line in data:
         EM += [[float(x) for x in line.split()[1:]]]
     EM = np.array(EM)
```

### Comparing `debyetools-1.3/debyetools/debfunct.py` & `debyetools-1.4.1/debyetools/debfunct.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/defects.py` & `debyetools-1.4.1/debyetools/defects.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/electronic.py` & `debyetools-1.4.1/debyetools/electronic.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,40 +60,45 @@
     def d2FdVdT(self,T,V):
         return -2*np.pi**2*NAv*self.r*kB**2*T*self.dNfVdV_T(V)*(1/6)/(0.160218e-18)
     def d3FdV2dT(self,T,V):
         return -2*np.pi**2*NAv*self.r*kB**2*T*self.d2NfVdV2_T(V)*(1/6)/(0.160218e-18)
     def d3FdVdT2(self,T,V):
         return -2*np.pi**2*NAv*self.r*kB**2*self.dNfVdV_T(V)*(1/6)/(0.160218e-18)
 
-def fit_electronic(Vs, p_el,E,N,Ef):
+def fit_electronic(Vs, p_el,E,N,Ef, ixss=8, ixse=-1):
     """
     Fitting procedure for the N(Ef)(V) function.
 
     :param list_of_floats Vs: Volumes.
     :param list_of_floats p_el: Initial parameters.
     :param list_of_lists_of_floats E: Matrix with energies at each level for each volume.
     :param list_of_lists_of_floats N: Matrix with densities of state at each level for each volume.
     :param list_of_floats Ef: Fermi levels as function of temperature.
 
     :retun list_of_floats: optimized parameters.
     """
 
     V = np.array(Vs)
-    ix_V0=10
+    ix_V0=4
     EfV0 = float(Ef[ix_V0])
     ixs=[i for i,x in enumerate(E[ix_V0]) if x>=Ef[ix_V0]]
     E1 = float(E[ix_V0][ixs[0]-1])
     E2 = float(E[ix_V0][ixs[0]])
     N1 = float(N[ix_V0][ixs[0]-1])
     N2 = float(N[ix_V0][ixs[0]])
     NfV0 = (EfV0 - E1)*(N2 - N1)/(E2 - E1) + N1
-    NfV = np.array([NfV0*np.sqrt(ef/EfV0) for ef in Ef][8:-1])
-    P2 = leastsq(NfV2m, p_el, args=(V[8:-1], NfV),maxfev=1000)
+    NfV = np.array([NfV0*np.sqrt(ef/EfV0) for ef in Ef][ixss:ixse])
+    P2 = leastsq(NfV2m, p_el, args=(V[ixss:ixse], NfV),maxfev=1000)
+
     P2 = P2[0]
 
+    NfVcalc = [NfV_poly_fun(Vi, P2[0], P2[1], P2[2], P2[3]) for Vi in V[ixss:ixse]]
+    print('#V NfVdata NfVcalc')
+    for Vi, Ndatai, Ncalci in zip(V[ixss:ixse], NfV, NfVcalc):
+        print('%.5e %.5e %.5e' % (Vi, Ndatai, Ncalci))
     return P2
 
 def NfV_poly_fun(V, _A, _B, _C, _D):
     return _A + _B*V + _C*V**2 + _D*V**3
 
 def NfV2m(P, Vdata, NfVdata):
     NfVcalc = [NfV_poly_fun(Vi, P[0], P[1], P[2], P[3]) for Vi in Vdata]
```

### Comparing `debyetools-1.3/debyetools/fs_compound_db.py` & `debyetools-1.4.1/debyetools/fs_compound_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import numpy as np
 from scipy.optimize import curve_fit
 
-Cp2fit = lambda T, P0, P1, P2, P3, P4, P5: P0*T**0 + P1*T**1 + P2*T**(-2) + P3*T**2 + P4*T**(-.5) + P5*T**(-3)
+Cp2fit = lambda T, P0, P1, P2, P3: P0*T**0 + P1*T**1 + P2*T**(-2) + P3*T**2# + P4*T**(-.5) + P5*T**(-3)
 alpha2fit = lambda T, Q0, Q1, Q2, Q3: Q0*T**0 + Q1*T**1 + Q2*T**(-1) + Q3*T**(-2)
 Ksinv2fit = lambda T, R0, R1, R2, R3: R0*T**0 + R1*T**1 + R2*T**2 + R3*T**3
 Ksp2fit = lambda T, S0, S1: S0 + S1*(T-298.15)*np.log(T/298.15)
 
 def fit_FS(tprops, T_from, T_to):
     """
     Procedure for the fitting of FS compound database parametes to thermodynamic properties.
```

### Comparing `debyetools-1.3/debyetools/layout.py` & `debyetools-1.4.1/debyetools/layout.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/ndeb.py` & `debyetools-1.4.1/debyetools/ndeb.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/pairanalysis.py` & `debyetools-1.4.1/debyetools/pairanalysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,95 @@
 import numpy as np
 import itertools as it
 import debyetools.aux_functions as afn
 
 
 
-def neighbor_list(size, cutoff, center, basis_vectors, primitive_cell):
+def neighbor_list(size, max_distance, center, basis_vectors, primitive_cell, ncells=True):
     """ calculate a list i, j, dij where i and j are a pair of atoms of
     indexes i and j, respectively, and dij is the distance between them.
 
     :param array size: Number of times we are replicating the primitive cel
-    :param int cutoff: Number of times we are replicating the supercell up to which we are considering for the calculation (uses pbc)
+    :param int max_distance: Number of times we are replicating the supercell up to which we are considering for the calculation (uses pbc)
     :param array center: The position in space where the system of reference is
     :param array basis_vectors: atoms position within a single primitive cell
     :param array primitive_cell: the primitive cell
     :return: D, I , J
     """
 
     basis_vectors = np.dot(basis_vectors,primitive_cell)
-    size_g = size + 2*cutoff  #to do: change cutoff for some other word and add a cutoff distance.
-                              # new_co= int(min(cutoff,....))
+    size_g = size + 2*max_distance  #to do: change max_distance for some other word and add a max_distance distance.
+                              # new_co= int(min(max_distance,....))
 
     cell_coords_centered = afn.generate_cells_coordinates(size, primitive_cell, center)
-    cell_coords_centered_g = afn.generate_cells_coordinates(size_g, primitive_cell, center-cutoff)
+    cell_coords_centered_g = afn.generate_cells_coordinates(size_g, primitive_cell, center-max_distance)
+    # print(size_g)
 
     XCs = []
     Is = []
     Js = []
+    CIXs = []
+
 
     ixs = np.arange(len(basis_vectors))
     jxs = np.arange(len(basis_vectors))
 
-    for icell, cell_coords_i in enumerate(cell_coords_centered):
-        ix_neighbor = np.where(np.all(abs(cell_coords_centered_g-cell_coords_i)<=cutoff, axis=1))[0]
+    for cell_coords_i in cell_coords_centered:
+        ix_neighbor = np.where(np.all(abs(cell_coords_centered_g-cell_coords_i)<=max_distance, axis=1))[0]
         Xs = np.array([cell_coords_i,]*len(basis_vectors))+basis_vectors
 
-        for cell_coords_i_g in cell_coords_centered_g[ix_neighbor]:
+        for ixx, cell_coords_i_g in enumerate(cell_coords_centered_g[ix_neighbor]):
             Xsg = np.array([cell_coords_i_g,]*len(basis_vectors))+basis_vectors
             for x, xg in it.product(Xs, Xsg):
                 XCs.append((x-xg)**2)
             for i, j in it.product(ixs, jxs):
                 Is.append(i)
                 Js.append(j)
+                CIXs.append(ix_neighbor[ixx])
+
 
     XCs = np.array(XCs)
     Is = np.array(Is)
     Js = np.array(Js)
-    CX = np.sum(XCs/cutoff**2, axis=1)
+    CIXs = np.array(CIXs)
+
+    CX = np.sum(XCs/max_distance**2, axis=1)
 
     ix = np.where(np.all([CX<=1, CX>0], axis=0))[0]
     distances = np.sqrt(np.sum(XCs[ix], axis=1))
 
-    return distances, Is[ix], Js[ix]
+    res = distances, Is[ix], Js[ix], cell_coords_centered_g, CIXs[ix]
 
-def pair_analysis(atom_types, size, cutoff, center, basis_vectors, primitive_cell):
+    return res
+
+def pair_analysis(atom_types, size, max_distance, center, basis_vectors, primitive_cell, prec=10, full=False, cutoff=None):
     """
     run a pair analysis of a crystal structure of almost any type of symmetry.
 
     :param list_of_str atom_types: the types of each atom in the primitive cell in the same order as the basis vectors.
     :param array size: Number of times we are replicating the primitive cel
-    :param int cutoff: Number of times we are replicating the supercell up to which we are considering for the calculation (uses pbc)
+    :param int max_distance: Number of times we are replicating the supercell up to which we are considering for the calculation (uses pbc)
     :param array center: The position in space where the system of reference is
     :param array basis_vectors: atoms position within a single primitive cell
     :param array primitive_cell: the primitive cell
     :return:  pair distance, pair number, pair types
     """
-    cutoff = np.array([int(cutoff), int(cutoff), int(cutoff)]) ##<--- fix_here
-    dAxBy, iAxBy, jAxBy  = neighbor_list(size, cutoff, center, basis_vectors, primitive_cell)
-
+    max_distance = np.array([int(max_distance), int(max_distance), int(max_distance)]) ##<--- fix_here
+    dAxBy, iAxBy, jAxBy, cells_cohordniates, ij_ccix  = neighbor_list(size, max_distance, center, basis_vectors, primitive_cell)
+    if cutoff is not None:
+        maxdjx = np.where(dAxBy <= cutoff)
+        dAxBy, iAxBy, jAxBy, ij_ccix = dAxBy[maxdjx], iAxBy[maxdjx], jAxBy[maxdjx], ij_ccix[maxdjx]
+    dAxBy = np.array([np.round(d,prec) for d in dAxBy])
+    res_2 = dAxBy, iAxBy, jAxBy
     nat = np.prod(size)*len(basis_vectors)
 
     combs_types,types_all = afn.c_types(atom_types)
 
-    dAxBy = np.array([float('%0.10e'%(d)) for d in dAxBy])
-    bins_dAxBy =list(set([li for li in list(set(np.append(dAxBy, [max(cutoff)])))]))
+    # dAxBy = np.array([float('%0.10e'%(d)) for d in dAxBy])
+    bins_dAxBy =list(set([li for li in list(set(np.append(dAxBy, [max(max_distance)])))]))
     bins_dAxBy.sort()
     distances = bins_dAxBy[:-1]
 
     ptlst = []
     for i,j,d in zip(iAxBy,jAxBy,dAxBy):
         for ii in range(len(combs_types)):
             if (types_all[i]+'-'+types_all[j] == combs_types[ii]) or (types_all[j]+'-'+types_all[i] == combs_types[ii]):
@@ -90,8 +103,12 @@
         ds[i] = np.array([d for d in dAxBy[np.where(ptlst==i)[0]]])
     hs = ['' for x in range(len(combs_types))]
     bs = ['' for x in range(len(combs_types))]
     for i in range(len(combs_types)):
         hs[i], bs[i] = np.histogram(ds[i], bins=bins_dAxBy)
     tot_num_bonds_per_molecule = np.array(hs).T
     num_bonds_per_formula = tot_num_bonds_per_molecule/nat
-    return np.array(distances), num_bonds_per_formula, combs_types
+
+    if full:
+        return np.array(distances), num_bonds_per_formula, combs_types, res_2[0], res_2[1], res_2[2], cells_cohordniates, ij_ccix
+    else:
+        return np.array(distances), num_bonds_per_formula, combs_types
```

### Comparing `debyetools-1.3/debyetools/poisson.py` & `debyetools-1.4.1/debyetools/poisson.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-def poisson_ratio(EM):
+def poisson_ratio(EM, quiet=False):
     """
     Calculation of the Poisson's ratio from elastic moduli matrix.
 
     :param list_of_lists_of_floats EM: Elastic moduli matrix.
 
     :return float: Poisson's ratio.
     """
+    if quiet:
+        return quiet_pa(EM)
+
     C11, C12, C13 = EM[0,0]*1e-1, EM[0,1]*1e-1, EM[0,2]*1e-1
     C22, C23 = EM[1,1]*1e-1, EM[1,2]*1e-1
     C33 = EM[2,2]*1e-1
     C44 = EM[3,3]*1e-1
     C55 = EM[4,4]*1e-1
     C66 = EM[5,5]*1e-1
 
-    if EM[0,4]*1e-1>0:
+    if EM[0,4]**2*1e-1>0:
         C15 = EM[0,4]*1e-1
         C25 = EM[1,4]*1e-1
         C35 = EM[2,4]*1e-1
         C46 = EM[3,5]*1e-1
     else:
         C15 = EM[0,5]*1e-1
         C25 = EM[1,5]*1e-1
@@ -37,11 +40,51 @@
     Sr=GR
     Sv=GV
     B = (BR+BV)/2
     S = (GR+GV)/2
     Y = (9.*B*S)/(3.*B+S)
     nu = (3.*B-Y)/(6.*B)
     AU = 5*Sv/Sr+Bv/Br-6
-    print('Sv/Sr',Sv/Sr, 'Sv/Sr', Bv/Br)
+    print('Sv/Sr',Sv/Sr, 'Bv/Br', Bv/Br)
     print('C11, C12, C13, C15, C22, C23, C25, C33, C35, C44, C46, C55, C66, B, Y, S, AU, nu','\n',C11, C12, C13, C15, C22, C23, C25, C33, C35, C44, C46, C55, C66, B, Y, S, AU, nu)
 
     return nu
+
+def quiet_pa(EM):
+    C11, C12, C13 = EM[0,0]*1e-1, EM[0,1]*1e-1, EM[0,2]*1e-1
+    C22, C23 = EM[1,1]*1e-1, EM[1,2]*1e-1
+    C33 = EM[2,2]*1e-1
+    C44 = EM[3,3]*1e-1
+    C55 = EM[4,4]*1e-1
+    C66 = EM[5,5]*1e-1
+
+    if EM[0,4]*1e-1>0:
+        C15 = EM[0,4]*1e-1
+        C25 = EM[1,4]*1e-1
+        C35 = EM[2,4]*1e-1
+        C46 = EM[3,5]*1e-1
+    else:
+        C15 = EM[0,5]*1e-1
+        C25 = EM[1,5]*1e-1
+        C35 = EM[2,5]*1e-1
+        C46 = EM[3,4]*1e-1
+
+    f = C11*(C22*C55-C25**2)-C12*(C12*C55-C15*C25)+C15*(C12*C25-C15*C22)+C25*(C23*C35-C25*C33)
+    g = C11*C22*C33-C11*C23**2-C22*C13**2-C33*C12**2+2*C12*C13*C23
+    Omega=2*(C15*C25*(C33*C12-C13*C23)+C15*C35*(C22*C13-C12*C23)+C25*C35*(C11*C23-C12*C13)) -(C15**2*(C22*C33-C23**2)+C25**2*(C11*C33-C13**2)+C35**2*(C11*C22-C12**2))+g*C55
+    GV = 1/15*(C11+C22+C33+3*(C44+C55+C66)-(C12+C13+C23))
+    GR = 15*(4*((C33*C55-C35**2)*(C11+C22+C12) + (C23*C55-C25*C35)*(C11-C12-C23) + (C13*C35-C15*C33)*(C15+C25) + (C13*C55-C15*C35)*(C22-C12-C23-C13) + (C13*C25-C15*C23)*(C15-C25) + f)/Omega+3*(g/Omega+(C44+C66)/(C44*C66-C46**2)))**(-1)
+    BV = (C11+C22+C33+2*(C12+C13+C23))/9
+    BR = Omega*((C33*C55-C35**2)*(C11+C22-2*C12)+(C23*C55-C25*C35)*(2*C12-2*C11-C23) + (C13*C35-C15*C33)*(C15-2*C25)+(C13*C55-C15*C35)*(2*C12+2*C23-C13-2*C22)+2*(C13*C25-C15*C23)*(C25-C15)+f)**(-1)
+
+    Br=BR
+    Bv=BV
+    Sr=GR
+    Sv=GV
+    B = (BR+BV)/2
+    S = (GR+GV)/2
+    Y = (9.*B*S)/(3.*B+S)
+    nu = (3.*B-Y)/(6.*B)
+    AU = 5*Sv/Sr+Bv/Br-6
+
+    return BR, BV, B, GR, GV, S, AU, nu
+
```

### Comparing `debyetools-1.3/debyetools/potentials.py` & `debyetools-1.4.1/debyetools/potentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,25 +527,28 @@
     """
     Morse potential and derivatives.
 
     :param list args: formula, primitive_cell, basis_vectors, cutoff, number_of_neighbor_levels.
     :param list_of_floats parameters: Morse potential parameters.
     """
 
-    def __init__(self, *args, units='J/mol', parameters=''):
+    def __init__(self, *args, units='J/mol', parameters='', prec=10):
         formula, primitive_cell, basis_vectors, cutoff, number_of_neighbor_levels = args
         # formula,    primitive_cell,    basis_vectors    = pair_analysis.ReadPOSCAR(ins_atoms_positions_filename)
+        self.formula, self.primitive_cell, self.basis_vectors = formula, primitive_cell, basis_vectors
+
         size = np.array([1, 1, 1])
         center = np.array([0, 0, 0])
         atom_types = formula * np.prod(size)
         neigbor_distances_at_Vstar, number_of_pairs_per_distance, comb_types = pairanalysis.pair_analysis(atom_types,
                                                                                                           size, cutoff,
                                                                                                           center,
                                                                                                           basis_vectors,
-                                                                                                          primitive_cell)
+                                                                                                          primitive_cell,
+                                                                                                          prec=prec)
 
         neigbor_distances_at_Vstar, number_of_pairs_per_distance = neigbor_distances_at_Vstar[
                                                                    :number_of_neighbor_levels], number_of_pairs_per_distance[
                                                                                                 :number_of_neighbor_levels,
                                                                                                 :]
 
         self.comb_types = comb_types
@@ -576,20 +579,25 @@
         :param list_of_floats Edata: Target data.
         :param list_of_floats initial_parameters: initial_parameters.
 
         :return list_of_floats: Optimal parameters.
         """
         if fit:
             pEOS = initial_parameters
-            popt = least_squares(self.error2min, pEOS, args=(Vdata, Edata))['x']
+            lstsq_sol = least_squares(self.error2min, pEOS, args=(Vdata, Edata), bounds=(0, np.inf))
+            popt = lstsq_sol['x']
             self.pEOS = popt
+            self.eos_residuals = lstsq_sol['fun']
         if not fit:
             self.pEOS = initial_parameters
 
-        mV = minimize(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata), max(Vdata))], tol=1e-10)
+            #        for i in range(-20, 21):
+            #            print(Vdata[0]*(1+i/100) , self.E0(Vdata[0]*(1+i/100)))
+        mV = minimize(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata) * .9, max(Vdata) * 1.1)], tol=1e-10)
+        # mV2 = self.minimize_bruteforce(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata)*.9, max(Vdata)*1.1)], tol=1e-10)
         self.V0 = mV['x'][0]
 
         return self.pEOS
 
     def E04min(self, V, pEOS):
         if type(V) == np.ndarray:
             return np.array([self.E04min(Vi, pEOS) for Vi in V])
@@ -834,15 +842,15 @@
         :param list_of_floats Edata: Target data.
         :param list_of_floats initial_parameters: initial_parameters.
 
         :return list_of_floats: Optimal parameters.
         """
         if fit:
             pEOS = initial_parameters[:4]
-            popt = least_squares(self.error2min, pEOS, args=(Vdata, Edata))['x']
+            popt = least_squares(self.error2min, pEOS, args=(Vdata, Edata),bounds=([-np.inf, 0, 0, 0], [0, np.inf,np.inf,np.inf]))['x']
             self.pEOS = popt
         if not fit:
             self.pEOS = initial_parameters[:4]
 
         mV = minimize(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata), max(Vdata))], tol=1e-10)
         self.V0 = mV['x'][0]
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/elements.py` & `debyetools-1.4.1/debyetools/tpropsgui/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def Chk(txt,key,disabled=False):
     return dChk(txt,key,False,disabled=disabled)
 
 def collapse(layout, key):
     return sg.pin(sg.Column(layout, key='||Col_'+key,visible=False, vertical_alignment='top'))
 
 def Bc(txt,key,colors,right_click_menu=None):
-    print('||B_'+key)
+    # print('||B_'+key)
     return sg.Button(txt,key='||B_'+key,disabled=True,font=("Helvetica", 10),right_click_menu=right_click_menu,pad=(1,1))
 
 def Be(txt,key,colors,right_click_menu=None):
     return sg.Button(txt,key='||B_'+key,disabled=False,font=("Helvetica", 10),right_click_menu=right_click_menu,pad=(1,1))
 
 def VS():
     return sg.VSeperator()
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/events.py` & `debyetools-1.4.1/debyetools/tpropsgui/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 #
 def eos_write_params(window,EOSStr,pEOS):
         window['--I_params_'+EOSStr].update(', '.join(['%.9e' for i in pEOS])%tuple(pEOS))
         pEOS2=pEOS
         # if EOSStr not in ['EAM', 'MP']:
         #     pEOS2[0]=pEOS2[0]/(0.160218e-18 * 6.02214e23)
         #     pEOS2[1] = pEOS2[1] / (1e-30 * 6.02e23)
-        print(EOSStr,':',', '.join(['%.9e' for i in pEOS])%tuple(pEOS))
+        # print(EOSStr,':',', '.join(['%.9e' for i in pEOS])%tuple(pEOS))
 ##
 def chk_el(window,event):
     window['--I_p_el'].update(disabled= not bool(window[event].get()))
     window['||B_calc_el'].update(disabled= not bool(window[event].get()))
 #
 def chk_def(window,event):
     window['--I_p_evac'].update(disabled= not bool(window[event].get()))
@@ -201,22 +201,22 @@
     window['--I_fs_Tfrom'].update(disabled=False)
     window['--I_fs_Tto'].update(disabled=False)
     window['||B_eval_anh'].update(disabled=False)
     window['--Tab_'].update(visible=False)
 #
 def plot_EvV(window, eosobj_dict, opened_EOS_dict,jx):
     pots_str_lst = [k for k in opened_EOS_dict if opened_EOS_dict[k]]
-    print(pots_str_lst)
+    # print(pots_str_lst)
     V_DFT = eosobj_dict['V_DFT']
     E_DFT = eosobj_dict['E_DFT']
     tab3_str='#V          DFT         '+'          '.join(['%s' for i in pots_str_lst])%tuple(pots_str_lst)+'\n'
     for Vi, Ei in zip(V_DFT, E_DFT):
         Emi = [eosobj_dict[k].E0(Vi) for k in pots_str_lst]
         tab3_str= tab3_str + '%.10e   %.10e  '%(Vi,Ei) + '  '.join(['%.10e' for i in Emi])%tuple(Emi)+'\n'
-    print(tab3_str)
+    # print(tab3_str)
     initial_tabs_multilinetxt = {'t0':{'multiline':tab3_str}}
     initial_lines_settings = {
                               'l0': {'plot':True,'label':0,'linestyle':'None','color':'mediumpurple',  'marker':'o',   'markerfacecolor':'black', 'markeredgecolor':'mediumpurple',  'linewidth':2,'markersize':10},
                               'l1': {'plot':True,'label':0,'linestyle':'None','color':'purple',        'marker':'+',   'markerfacecolor':'None', 'markeredgecolor':'purple',         'linewidth':2,'markersize':10},
                               'l2': {'plot':True,'label':0,'linestyle':'None','color':'gray',          'marker':'x',   'markerfacecolor':'None', 'markeredgecolor':'gray',           'linewidth':2,'markersize':10},
                               'l3': {'plot':True,'label':0,'linestyle':'None','color':'orchid',        'marker':'s',   'markerfacecolor':'None', 'markeredgecolor':'orchid',         'linewidth':2,'markersize':10},
                               'l4': {'plot':True,'label':0,'linestyle':'None','color':'deepskyblue',   'marker':'^',   'markerfacecolor':'None', 'markeredgecolor':'deepskyblue',    'linewidth':2,'markersize':10},
@@ -239,22 +239,22 @@
 
     data4plot = plot.pop_window(initial_tabs_multilinetxt,initial_lines_settings,initial_fig_settings,jx)
 
     return data4plot
 
 def plot_EvV_full(window, eosobj_dict, opened_EOS_dict,jx):
     pots_str_lst = [k for k in opened_EOS_dict if opened_EOS_dict[k]]
-    print(pots_str_lst)
+    # print(pots_str_lst)
     V_DFT = eosobj_dict['V_DFT']
     E_DFT = eosobj_dict['E_DFT']
     tab3_str='#V          DFT         '+'          '.join(['%s' for i in pots_str_lst])%tuple(pots_str_lst)+'\n'
     for Vi, Ei in zip(V_DFT, E_DFT):
         Emi = [eosobj_dict[k].E0(Vi) for k in pots_str_lst]
         tab3_str= tab3_str + '%.10e   %.10e  '%(Vi,Ei) + '  '.join(['%.10e' for i in Emi])%tuple(Emi)+'\n'
-    print(tab3_str)
+    # print(tab3_str)
     initial_tabs_multilinetxt = {'t0':{'multiline':tab3_str}}
     initial_lines_settings = {
                               'l0': {'plot':True,'label':0,'linestyle':'None','color':'mediumpurple',  'marker':'o',   'markerfacecolor':'black', 'markeredgecolor':'mediumpurple',  'linewidth':2,'markersize':10},
                               'l1': {'plot':True,'label':0,'linestyle':'None','color':'purple',        'marker':'+',   'markerfacecolor':'None', 'markeredgecolor':'purple',         'linewidth':2,'markersize':10},
                               'l2': {'plot':True,'label':0,'linestyle':'None','color':'gray',          'marker':'x',   'markerfacecolor':'None', 'markeredgecolor':'gray',           'linewidth':2,'markersize':10},
                               'l3': {'plot':True,'label':0,'linestyle':'None','color':'orchid',        'marker':'s',   'markerfacecolor':'None', 'markeredgecolor':'orchid',         'linewidth':2,'markersize':10},
                               'l4': {'plot':True,'label':0,'linestyle':'None','color':'deepskyblue',   'marker':'^',   'markerfacecolor':'None', 'markeredgecolor':'deepskyblue',    'linewidth':2,'markersize':10},
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/functions0.py` & `debyetools-1.4.1/debyetools/tpropsgui/functions0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import PySimpleGUI as sg
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-#
+plt.switch_backend('TkAgg')
 import numpy as np
 # import addcopyfighandler
 #
 legend_loc_list = ['best','upper right','upper left','lower left','lower right','right','center left','center right','lower center','upper center','center']
 line_styles_list = ['-','--','-.',':','None']
 colors_list = ['mediumpurple','purple','gray','orchid','deepskyblue', 'pink', 'darkkhaki', 'aqua','cornflowerblue','blue','green','red','C0','C1','C2','C3','C4']
 markers_list=['.','o','+','x','1', '2', '3', '4','s','h','^', 'v','>', '<','*', '8', 'd', 'P', 'p', 'H','None']
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/gui.py` & `debyetools-1.4.1/debyetools/tpropsgui/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,25 @@
-def gui() -> object:
+import sys
+from PySide6.QtWidgets import QApplication
+
+from debyetools.tpropsgui.mainwindow import mainWindow
+def interface():
+    app = QApplication(sys.argv)
+
+    widget = mainWindow(app=app)
+    # widget.app = app
+    widget.show()
+    sys.exit(app.exec())
+
+
+def gui():
+    from warnings import warn
+
+    warn('This is deprecated', DeprecationWarning, stacklevel=2)
+
     import PySimpleGUI as sg
     from debyetools.tpropsgui.layout import layout
     import debyetools.tpropsgui.events as events
     # import debyetools.tpropsgui.toolbox as tbox
     from debyetools.aux_functions import load_doscar, load_V_E, load_EM, load_cell
     import debyetools.potentials as potentials
     import traceback
@@ -33,15 +50,15 @@
     EOS2plot_dict = {str_i:'' for str_i in EOS_str_lst}
     mws_dict = {'Al3Ca_D022': 0.030255624999999998, 'H': 0.0010079, 'He': 0.0040026, 'Li': 0.006941, 'Be': 0.0090122, 'B': 0.010811, 'C': 0.0120107, 'N': 0.0140067, 'O': 0.0159994, 'F': 0.0189984, 'Ne': 0.020179700000000002, 'Na': 0.0229897, 'Mg': 0.024305, 'Al': 0.026981500000000002, 'Si': 0.0280855, 'P': 0.0309738, 'S': 0.032064999999999996, 'Cl': 0.035453000000000005, 'K': 0.0390983, 'Ar': 0.039948, 'Ca': 0.040078, 'Sc': 0.0449559, 'Ti': 0.047867, 'V': 0.0509415, 'Cr': 0.051996099999999996, 'Mn': 0.054938, 'Fe': 0.055845, 'Ni': 0.0586934, 'Co': 0.0589332, 'Cu': 0.063546, 'Zn': 0.06539, 'Ga': 0.069723, 'Ge': 0.07264, 'As': 0.0749216, 'Se': 0.07895999999999999, 'Br': 0.079904, 'Kr': 0.0838, 'Rb': 0.0854678, 'Sr': 0.08762, 'Y': 0.0889059, 'Zr': 0.091224, 'Nb': 0.0929064, 'Mo': 0.09594, 'Tc': 0.098, 'Ru': 0.10107, 'Rh': 0.1029055, 'Pd': 0.10642, 'Ag': 0.1078682, 'Cd': 0.112411, 'In': 0.114818, 'Sn': 0.11871, 'Sb': 0.12176000000000001, 'I': 0.1269045, 'Te': 0.1276, 'Xe': 0.131293, 'Cs': 0.13290549999999998, 'Ba': 0.137327, 'La': 0.1389055, 'Ce': 0.14011600000000002, 'Pr': 0.1409077, 'Nd': 0.14424, 'Pm': 0.145, 'Sm': 0.15036000000000002, 'Eu': 0.151964, 'Gd': 0.15725, 'Tb': 0.1589253, 'Dy': 0.1625, 'Ho': 0.1649303, 'Er': 0.167259, 'Tm': 0.1689342, 'Yb': 0.17304, 'Lu': 0.174967, 'Hf': 0.17849, 'Ta': 0.1809479, 'W': 0.18384, 'Re': 0.18620699999999998, 'Os': 0.19022999999999998, 'Ir': 0.19221700000000003, 'Pt': 0.195078, 'Au': 0.1969665, 'Hg': 0.20059, 'Tl': 0.2043833, 'Pb': 0.2072, 'Bi': 0.2089804, 'Po': 0.209, 'At': 0.21, 'Rn': 0.222, 'Fr': 0.223, 'Ra': 0.226, 'Ac': 0.227, 'Pa': 0.2310359, 'Th': 0.2320381, 'Np': 0.237, 'U': 0.2380289, 'Am': 0.243, 'Pu': 0.244, 'Cm': 0.247, 'Bk': 0.247, 'Cf': 0.251, 'Es': 0.252, 'Fm': 0.257, 'Md': 0.258, 'No': 0.259, 'Rf': 0.261, 'Lr': 0.262, 'Db': 0.262, 'Bh': 0.264, 'Sg': 0.266, 'Mt': 0.268, 'Rg': 0.272, 'Hs': 0.277}
 
     #### Window layout
     layout = layout(EOS_str_lst)
 
     #### Window creation
-    window1, window2, window3,window4,window5, window7 = sg.Window('ThermoProps V1.1', layout=layout, finalize=True), None, None, None, None, None
+    window1, window2, window3,window4,window5, window7 = sg.Window('tProps V1.0.3', layout=layout, finalize=True), None, None, None, None, None
 
     #### loop to wait for user action
     all_props={}
     tprops_dict_all = {}
     p_el_initial = [3.8027342892e-01, -1.8875015171e-02,
                     5.3071034596e-04, -7.0100707467e-06]
     FS_db_params = {}
@@ -50,20 +67,20 @@
     window5_counter = 0
     windows_ix = ''
     bool_anh = False
     while True:
         window,event, values = sg.read_all_windows()
         # pr0nt(window,event)
         # pr0nt(window1, window2, window3,window4,window5)
-        print(event)
+        # print(event)
         try:
             ips = event.index('ix')
             ips2 = event[ips:].index('-')
             windows_ix = event[ips+2:ips+ips2]
-            print(windows_ix)
+            # print(windows_ix)
         except:
             print(False)
 
         # #close window
         if event == sg.WIN_CLOSED or event == '--B_close':
             window.close()
             if window == window2:       # if closing win 2, mark as closed
@@ -180,15 +197,15 @@
                             else:
                                 pass
 
                         if checked_EOS_dict[k]:
                             # print(verb,'7')
                             initial_parameters = np.array(initial_parameters,dtype=object)
                             EOS2params.fitEOS(V_DFT, E_DFT, initial_parameters=initial_parameters)
-                            print(k, 'fitted')
+                            # print(k, 'fitted')
                         else:
                             initial_parameters = np.array([float(pi) for pi in window['--I_params_'+k].get().split(', ')])
                             # pr0nt(initial_parameters)
                             EOS2params.fitEOS(V_DFT, E_DFT, initial_parameters=initial_parameters, fit=False)
                             print(k, 'not fitted')
                             #EOS2params.pEOS = np.array([float(pi) for pi in window['--I_params_'+k].get().split(', ')])
                             #EOS2params.V0=1e-5
@@ -304,15 +321,15 @@
                 E, N, Ef = load_doscar(str_folderbrowser+'/DOSCAR.EvV.')
                 p_electronic = fit_electronic(V_DFT, p_el_initial,E,N,Ef)
 
                 window['--I_p_el'].update(', '.join(['%.5e' for _ in p_electronic]) % tuple(p_electronic))
             except FileNotFoundError:
                 sg.popup_ok("DOSCAR files not found.\n\nIf you don't have any, try using your own parameter values or just without electronic contribution.")
             except Exception as e:
-                print(e.__class__)
+                # print(e.__class__)
                 sg.popup_ok(traceback.format_exc())
 
         elif event == '||B_run_minF':
             # mode=''
             try:
                 for k in EOS_str_lst:
                     window['--M_tprop_'+k].update('')
@@ -377,15 +394,15 @@
                 Pressure = float(Pressure)
 
 
                 T = gen_Ts(T_initial, T_final, number_Temps)
 
                 for k in opened_EOS_dict.keys():
                     if opened_EOS_dict[k]:
-                        print(window['--I_formula'].get(), nu, m, p_intanh, EOS2plot_dict[k], p_electronic,p_defects, p_anh, mode)
+                        # print(window['--I_formula'].get(), nu, m, p_intanh, EOS2plot_dict[k], p_electronic,p_defects, p_anh, mode)
                         nDebs_dict[k]['ndeb'] = nDeb(nu, m, p_intanh, EOS2plot_dict[k], p_electronic,
                                              p_defects, p_anh, mode=mode)
                         Tmin, Vmin = nDebs_dict[k]['ndeb'].min_G(T,EOS2plot_dict[k].V0,Pressure)
                         #Tmin, Vmin = nDebs_dict[k]['ndeb'].min_G(T,nDebs_dict[k]['ndeb'].EOS.V0,Pressure, Vmin[0], a_DM, b_DM)
                         nDebs_dict[k]['T'] = np.array(Tmin)
                         nDebs_dict[k]['V'] = Vmin
                 txt2VT = '#T'
@@ -417,15 +434,15 @@
                 sg.popup_ok(traceback.format_exc())
 
 
         elif event == '||B_eval_tprops':
             try:
                 for o in opened_EOS_dict:
                     if opened_EOS_dict[o]:
-                        print('Results for:',o)
+                        # print('Results for:',o)
                         tprops_dict_all[o] = nDebs_dict[o]['ndeb'].eval_props(nDebs_dict[o]['T'],nDebs_dict[o]['V'],Pressure)
 
                         window['--Tab_'+o].update(visible=True)
                         #window['--Tab_'+o].select()
                         keys_TPs = tprops_dict_all[o].keys()
                         tprops_str = '#T          '+' '.join([(j+'            ') for j in list(keys_TPs)[1:]])+'\n'
                         TPs_arr = np.c_[tuple([tprops_dict_all[o][j] for j in keys_TPs])]
@@ -470,15 +487,15 @@
                 sg.popup_ok('Please add the Murnaghan EOS to the calculation.')
             elif len([o for o in opened_EOS_dict if opened_EOS_dict[o] == True])<2:
                 sg.popup_ok('Please add at least one EOS different from Murnaghan to evaluate its anharmonicity contribution.')
 
             else:
                 anh_arr_MU = np.c_[tuple([tprops_dict_all['MU'][j] for j in keys_TPs])]
                 import debyetools.tpropsgui.elements as elmt
-                print('XXXXXXXXXXXXXXXXXXXXXXXXX')
+                # print('XXXXXXXXXXXXXXXXXXXXXXXXX')
                 lo_tabs_anh = [[elmt.Tab(eos_str,[[elmt.sCol([[elmt.M('','anh_'+eos_str,1000,7)]], 'anh_'+eos_str, 470, 80)]],'anh_'+eos_str,False) for eos_str in ['','MP','BM','RV','MG','TB','MU','PT','BM4','MU2','EAM','*MP','*BM','*RV','*MG','*TB','*MU','*PT','*BM4','*MU2','*EAM']]]
 
                 lo_anh = [[elmt.TG(lo_tabs_anh, 'tabs_anh')],
                           [elmt.T('select property to plot:', 'anh2plt'),
                            elmt.ICombo(['       ', '       ', '       ', '       '], 'anh2plt', 10, 1),
                            elmt.Bc('Plot', 'plotter_anh', ('white', elmt.theme_background_color()))]]
 
@@ -504,15 +521,15 @@
                         window7['--Tab_anh_' + o].update(visible=True)
 
 
 
                         # pr0nt(anh_arr-anh_arr_MU)
                 window7['--Tab_anh_'].update(visible=False)
                 bool_anh = True
-                print('bool_anh', bool_anh)
+                # print('bool_anh', bool_anh)
 
         elif event == '||B_plotter_tprops':
             try:
                 keys_EOS = []
                 for o in opened_EOS_dict:
                     if opened_EOS_dict[o]:
                         keys_EOS.append(o)
@@ -597,15 +614,15 @@
                             #window['--I_fsK_P'+str(0)+o].update(' '.join(['%.7e' for i in FS_db_params[o]['1/Ks']])%tuple(FS_db_params[o]['1/Ks']))
 
                         for i in range(len(FS_db_params[o]['Ksp'])):
                             window['--I_fsKp_P'+str(i)+o].update(disabled=False)
                             window['--I_fsKp_P'+str(i)+o].update('%.4e'%(FS_db_params[o]['Ksp'][i]))
                             #window['--I_fsKp_P'+str(0)+o].update(' '.join(['%.7e' for i in FS_db_params[o]['Ksp']])%tuple(FS_db_params[o]['Ksp']))
 
-                        print('xxxxx', window['--I_formula'].get(), window['--I_strkt'].get(),o,mode,H298,S298,' '.join(['%.7e' for i in FS_db_params[o]['Cp']])%tuple(FS_db_params[o]['Cp']), ' '.join(['%.7e' for i in FS_db_params[o]['a']])%tuple(FS_db_params[o]['a']), ' '.join(['%.7e' for i in FS_db_params[o]['1/Ks']])%tuple(FS_db_params[o]['1/Ks']), ' '.join(['%.7e' for i in FS_db_params[o]['Ksp']])%tuple(FS_db_params[o]['Ksp']))
+                        # print('xxxxx', window['--I_formula'].get(), window['--I_strkt'].get(),o,mode,H298,S298,' '.join(['%.7e' for i in FS_db_params[o]['Cp']])%tuple(FS_db_params[o]['Cp']), ' '.join(['%.7e' for i in FS_db_params[o]['a']])%tuple(FS_db_params[o]['a']), ' '.join(['%.7e' for i in FS_db_params[o]['1/Ks']])%tuple(FS_db_params[o]['1/Ks']), ' '.join(['%.7e' for i in FS_db_params[o]['Ksp']])%tuple(FS_db_params[o]['Ksp']))
 
 
                 window['--Tab_fs_'].update(visible=False)
             except Exception as e:
                 sg.popup_ok(traceback.format_exc())
 
         elif '||B_plotter_fsprop2plt' in event:
@@ -631,15 +648,15 @@
             #     for stri in ['DM', 'Sl', 'VZ', 'mfv']:
             #         window['--Chk_mode_'+stri].update(disabled=False)
 
             if window[event].get():
                 mode = event.replace('--Chk_mode_','')
             else:
                 mode = 'xx'
-            print(mode)
+            # print(mode)
 
 
         elif event in ['--B_ix'+windows_ix+'-figwidth_UP', '--B_ix'+windows_ix+'-figheight_UP', '--B_ix'+windows_ix+'-figwidth_DN', '--B_ix'+windows_ix+'-figheight_DN']:
             data4plot_dict[windows_ix].increment_b_updn(event, values,0.1,1)
             data4plot_dict[windows_ix].update_formats()
             data4plot_dict[windows_ix].update_canvas(show=False)
         elif event in ['--B_ix'+windows_ix+'-titlesize_UP','--B_ix'+windows_ix+'-labelxsize_UP','--B_ix'+windows_ix+'-labelysize_UP','--B_ix'+windows_ix+'-titlesize_DN','--B_ix'+windows_ix+'-labelxsize_DN','--B_ix'+windows_ix+'-labelysize_DN','--B_ix'+windows_ix+'-legendncol_UP','--B_ix'+windows_ix+'-legendncol_DN','--B_ix'+windows_ix+'-legendfontsize_UP','--B_ix'+windows_ix+'-legendfontsize_DN']:
@@ -749,17 +766,17 @@
                     f.write('|<\n')
 
         elif '--B_ix'+windows_ix+'-editdata' == event:
             data4plot_dict[windows_ix].create_popupwindow()
 
             while True:
                 event2, values2 = data4plot_dict[windows_ix].popup_window.read()
-                print(event2)
+                # print(event2)
                 if event2 in ('--B_ok_w2',sg.WIN_CLOSED):
-                    print('ok')
+                    # print('ok')
                     break
 
                 if event2 == '--B_addtab_w2':
                     data4plot_dict[windows_ix].copy_multiline2dic(add=True)
                     data4plot_dict[windows_ix].popup_window.close()
                     data4plot_dict[windows_ix].create_popupwindow()
                     data4plot_dict[windows_ix].popup_window['--Tab_data_'+data4plot_dict[windows_ix] .tabs.keys()[-1]].select()
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/layout.py` & `debyetools-1.4.1/debyetools/tpropsgui/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     lo_def = [[elmt.Chk('','def',disabled=True),elmt.T('Evac:','p_evac'),elmt.dI('','p_evac',3),elmt.T('Svac:','p_svac'),elmt.dI('','p_svac',3),elmt.T('Tm:','Tm'),elmt.dI('','Tm',7)]]
 
     lo_anhxc = [[elmt.Chk('parameters:','anhxc',disabled=True),elmt.dI('','p_anhxc',10)]]
 
     lo_intanh = [[elmt.Chk('parameters:','intanh',disabled=True),elmt.dI('','p_intanh',10)]]
 
-    lo_left = [[elmt.T('compound:','compound'),
+    lo_left = [[elmt.T('path for input files:','compound'),
                 elmt.dI('','compound',30),
                 elmt.dI(txt='', key='FILEBROWSE_', w=0, disabled=False,enable_events=True,visible=False),
                 elmt.Br('compound')],
                [elmt.T('formula:','formula'),elmt.dI('','formula',6),elmt.T('structure:','strkt'),elmt.dI('','strkt',4)],
                [elmt.T('mass: (Kg/mol-at)','mass'),elmt.dI('','mass',7),elmt.T('r:','r',visible=False),elmt.dI('1','r',5,visible=False)],
                [elmt.F('EOS parametrization',lo_EOS,'EOS', right_click_menu=['',['More Info...::EOS','Go to code...::GoToEOS',]])],
                [elmt.F("Poisson's ratio", lo_poisson,'poisson', right_click_menu=['',['More Info...::Poisson','Go to code...::GoToPoisson',]])],
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/plotter.py` & `debyetools-1.4.1/debyetools/tpropsgui/plotter.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/tpropsgui/plotter_class.py` & `debyetools-1.4.1/debyetools/tpropsgui/plotter_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             try:
                 getattr(self.lines,k)['settings'] =line_settings[k]
             except:
                 getattr(self.lines,k)['settings'] = {'plot':True,'label':0,'linestyle':'-','color':'gray','marker':'x','markerfacecolor':'gray','markeredgecolor':'cornflowerblue','linewidth':2,'markersize':8,'scalex':1,'scaley':1}
 
     def create_window(self,simple=False):
         if simple == True:
-            print('simple_layout')
+            # print('simple_layout')
             layout = fn.simple_layout(self.lines)
         else:
             layout = fn.general_layout(self.lines,self.jx)
         window = sg.Window('Plotting stuff...', layout, finalize=True)
         self.window = window
 
     def create_popupwindow(self):
@@ -57,25 +57,25 @@
 
     def update_window(self, fig_settings):
         self.fig_settings=fig_settings
         for k in fig_settings.keys():
             self.window['ix'+str(self.jx)+'-'+k].update(fig_settings[k])
 
     def create_canvas(self,show=False):
-        print('create_canvas show',show)
+        # print('create_canvas show',show)
 
         self.fig = fn.plot_fig(self.fig_settings,self.lines,show=show)
         self.figure_canvas_agg = fn.draw_figure(self.window['--CANVAS2-'].TKCanvas, self.fig)
 
     def delete_fig_agg(self):
         self.figure_canvas_agg.get_tk_widget().forget()
         plt.close('all')
 
     def update_canvas(self,show=False):
-        print('update_canvas show',show)
+        # print('update_canvas show',show)
 
         self.delete_fig_agg()
         self.create_canvas(show=show)
 
     def increment_b_updn(self,event, values, incr, rdval):
         udstr = '_'+event.replace('_',' ').split()[-1]
         if udstr=='_UP':posneg=1
@@ -92,18 +92,18 @@
     def update_lines_settings(self):
         for l in list(self.window.key_dict.keys()):
             ix_inx = l.find('ix')
             newl = l[ix_inx:]
             ix_inx2 = newl.find('-')
             newl2 = newl[ix_inx2+1:]
             #l=newl2
-            print('AAAAA',l,l.replace('++',' ').split(),ix_inx,ix_inx==0,newl2[:2]=='++')
+            # print('AAAAA',l,l.replace('++',' ').split(),ix_inx,ix_inx==0,newl2[:2]=='++')
             if ix_inx==0 and newl2[:2]=='++':#l[:2]=='++': #ix_inx==0:#
                 prp = newl2.replace('++',' ').split()
-                print(self.lines.keys())
+                # print(self.lines.keys())
                 li = getattr(self.lines,prp[-1])['settings']
                 li[prp[0]]=self.window[l].get()
 
     def copy_multiline2dic(self,add=False):
         for l in list(self.popup_window.key_dict.keys()):
             if l[:2]=='||':
                 prp = l.replace('||',' ').split()
```

### Comparing `debyetools-1.3/debyetools/tpropsgui/toolbox.py` & `debyetools-1.4.1/debyetools/tpropsgui/toolbox.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools/vibrational.py` & `debyetools-1.4.1/debyetools/vibrational.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.3/debyetools.egg-info/PKG-INFO` & `debyetools-1.4.1/debyetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 1.3
+Version: 1.4.1
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # debyetools
 
 Implementation of a tool for calculating self-consistent thermodynamic properties that can take into account all kinds of contributions to the free energy inluding explicit anharmonicity. The software presented here is based in the Debye approximation within the QHA using the crystal internal energetics parametrized at ground-state to project the thermodynamics properties at high temperatures.
```

### Comparing `debyetools-1.3/debyetools.egg-info/SOURCES.txt` & `debyetools-1.4.1/debyetools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,22 +9,36 @@
 debyetools/electronic.py
 debyetools/fs_compound_db.py
 debyetools/layout.py
 debyetools/ndeb.py
 debyetools/pairanalysis.py
 debyetools/poisson.py
 debyetools/potentials.py
+debyetools/potentials_2.py
 debyetools/vibrational.py
 debyetools.egg-info/PKG-INFO
 debyetools.egg-info/SOURCES.txt
 debyetools.egg-info/dependency_links.txt
 debyetools.egg-info/requires.txt
 debyetools.egg-info/top_level.txt
 debyetools/tpropsgui/__init__.py
+debyetools/tpropsgui/atomtools.py
+debyetools/tpropsgui/dialog_doscar.py
+debyetools/tpropsgui/dialog_warning.py
 debyetools/tpropsgui/elements.py
 debyetools/tpropsgui/events.py
 debyetools/tpropsgui/functions0.py
+debyetools/tpropsgui/get_functions.py
 debyetools/tpropsgui/gui.py
 debyetools/tpropsgui/layout.py
+debyetools/tpropsgui/mainwindow.py
+debyetools/tpropsgui/plot_EV.py
 debyetools/tpropsgui/plotter.py
 debyetools/tpropsgui/plotter_class.py
-debyetools/tpropsgui/toolbox.py
+debyetools/tpropsgui/toolbox.py
+debyetools/tpropsgui/ui_dialog_doscar.py
+debyetools/tpropsgui/ui_heatcapacitywindow.py
+debyetools/tpropsgui/ui_interatomic_params.py
+debyetools/tpropsgui/ui_mainwindow.py
+debyetools/tpropsgui/ui_warning.py
+debyetools/tpropsgui/window_cp.py
+debyetools/tpropsgui/window_interatomicparams.py
```

### Comparing `debyetools-1.3/setup.py` & `debyetools-1.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="debyetools",
-    version="1.3",
+    version="1.4.1",
     description="Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://debyetools.readthedocs.io/",
     author="Javier Jofre",
     author_email="javier.jofre@polymtl.ca",
     license="GPLv3",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
     packages=["debyetools", "debyetools.tpropsgui"],
     include_package_data=True,
     install_requires=["numpy", "pysimplegui", "scipy", "matplotlib"]
 )
```

