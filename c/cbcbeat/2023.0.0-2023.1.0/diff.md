# Comparing `tmp/cbcbeat-2023.0.0.tar.gz` & `tmp/cbcbeat-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcbeat-2023.0.0.tar", last modified: Fri Mar 31 12:16:28 2023, max compression
+gzip compressed data, was "cbcbeat-2023.1.0.tar", last modified: Mon May  8 13:19:36 2023, max compression
```

## Comparing `cbcbeat-2023.0.0.tar` & `cbcbeat-2023.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:16:28.409381 cbcbeat-2023.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-31 12:16:28.409381 cbcbeat-2023.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:16:28.405381 cbcbeat-2023.0.0/cbcbeat/
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/bidomainsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cardiacmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:16:28.409381 cbcbeat-2023.0.0/cbcbeat/cellmodels/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/beeler_reuter_1977.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/cardiaccellmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/fenton_karma_1998_BR_altered.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/fenton_karma_1998_MLR1_altered.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/fitzhughnagumo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/fitzhughnagumo_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    38860 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/grandi_pasqualini_bers_2010.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/nocellmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/rogers_mcculloch_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_2004_mcell.py
--rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_2004_mcell_cont.py
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_2004_mcell_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21299 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_M_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_epi_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    23190 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/cellsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/dolfinimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/gossplittingsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/gotran2cellmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/markerwisefield.py
--rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/monodomainsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/splittingsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/cbcbeat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:16:28.405381 cbcbeat-2023.0.0/cbcbeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-31 12:16:28.000000 cbcbeat-2023.0.0/cbcbeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-31 12:16:28.000000 cbcbeat-2023.0.0/cbcbeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:16:28.000000 cbcbeat-2023.0.0/cbcbeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 12:16:28.000000 cbcbeat-2023.0.0/cbcbeat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-31 12:16:28.000000 cbcbeat-2023.0.0/cbcbeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 12:16:28.000000 cbcbeat-2023.0.0/cbcbeat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-31 12:16:14.000000 cbcbeat-2023.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 12:16:28.409381 cbcbeat-2023.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:36.531530 cbcbeat-2023.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-08 13:19:36.531530 cbcbeat-2023.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:36.527530 cbcbeat-2023.1.0/cbcbeat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/bidomainsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cardiacmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:36.527530 cbcbeat-2023.1.0/cbcbeat/cellmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/beeler_reuter_1977.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/cardiaccellmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/fenton_karma_1998_BR_altered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/fenton_karma_1998_MLR1_altered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/fitzhughnagumo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/fitzhughnagumo_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38860 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/grandi_pasqualini_bers_2010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/nocellmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/rogers_mcculloch_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_2004_mcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_2004_mcell_cont.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_2004_mcell_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21299 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_M_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_epi_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/cellsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/dolfinimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/gossplittingsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/gotran2cellmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/markerwisefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/monodomainsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/splittingsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-08 13:19:12.000000 cbcbeat-2023.1.0/cbcbeat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:19:36.527530 cbcbeat-2023.1.0/cbcbeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-08 13:19:36.000000 cbcbeat-2023.1.0/cbcbeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 13:19:36.000000 cbcbeat-2023.1.0/cbcbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:19:36.000000 cbcbeat-2023.1.0/cbcbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 13:19:36.000000 cbcbeat-2023.1.0/cbcbeat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 13:19:36.000000 cbcbeat-2023.1.0/cbcbeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 13:19:36.000000 cbcbeat-2023.1.0/cbcbeat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-08 13:19:13.000000 cbcbeat-2023.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:19:36.531530 cbcbeat-2023.1.0/setup.cfg
```

### Comparing `cbcbeat-2023.0.0/COPYING` & `cbcbeat-2023.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/PKG-INFO` & `cbcbeat-2023.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcbeat
-Version: 2023.0.0
+Version: 2023.1.0
 Summary: An adjoint-enabled framework for computational cardiac electrophysiology
 Author: J.E hake, P.E Farrel, S. W. Funke
 Author-email: "M. E. Rognes" <meg@simula.no>
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: goss
 Provides-Extra: gotran
```

### Comparing `cbcbeat-2023.0.0/README.md` & `cbcbeat-2023.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/__init__.py` & `cbcbeat-2023.1.0/cbcbeat/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/bidomainsolver.py` & `cbcbeat-2023.1.0/cbcbeat/bidomainsolver.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cardiacmodels.py` & `cbcbeat-2023.1.0/cbcbeat/cardiacmodels.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/__init__.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/beeler_reuter_1977.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/beeler_reuter_1977.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/cardiaccellmodel.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/cardiaccellmodel.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/fenton_karma_1998_BR_altered.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/fenton_karma_1998_BR_altered.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/fenton_karma_1998_MLR1_altered.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/fenton_karma_1998_MLR1_altered.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/fitzhughnagumo.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/fitzhughnagumo.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/fitzhughnagumo_manual.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/fitzhughnagumo_manual.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/grandi_pasqualini_bers_2010.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/grandi_pasqualini_bers_2010.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/nocellmodel.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/nocellmodel.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/rogers_mcculloch_manual.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/rogers_mcculloch_manual.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_2004_mcell.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_2004_mcell.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_2004_mcell_cont.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_2004_mcell_cont.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_2004_mcell_disc.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_2004_mcell_disc.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_M_cell.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_M_cell.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_epi_cell.py` & `cbcbeat-2023.1.0/cbcbeat/cellmodels/tentusscher_panfilov_2006_epi_cell.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/cellsolver.py` & `cbcbeat-2023.1.0/cbcbeat/cellsolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,18 @@
         # Initialize and update parameters if given
         self.parameters = self.default_parameters()
         if params is not None:
             self.parameters.update(params)
 
         # Create (vector) function space for potential + states
         self.VS = dolfin.VectorFunctionSpace(
-            self._mesh, "CG", 1, dim=self._num_states + 1
+            self._mesh,
+            "CG",
+            self.parameters["polynomial_degree"],
+            dim=self._num_states + 1,
         )
 
         # Initialize solution field
         self.vs_ = backend.Function(self.VS, name="vs_")
         self.vs = backend.Function(self.VS, name="vs")
 
         # Initialize scheme
@@ -488,14 +491,15 @@
         """Initialize and return a set of default parameters
 
         *Returns*
           A set of parameters (:py:class:`dolfin.Parameters`)
         """
         params = dolfin.Parameters("CardiacODESolver")
         params.add("scheme", "BackwardEuler")
+        params.add("polynomial_degree", 1)
         params.add(point_integral_solver_default_parameters())
         params.add("enable_adjoint", True)
 
         return params
 
     def solution_fields(self):
         """
```

### Comparing `cbcbeat-2023.0.0/cbcbeat/gossplittingsolver.py` & `cbcbeat-2023.1.0/cbcbeat/gossplittingsolver.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/gotran2cellmodel.py` & `cbcbeat-2023.1.0/cbcbeat/gotran2cellmodel.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/markerwisefield.py` & `cbcbeat-2023.1.0/cbcbeat/markerwisefield.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/monodomainsolver.py` & `cbcbeat-2023.1.0/cbcbeat/monodomainsolver.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/splittingsolver.py` & `cbcbeat-2023.1.0/cbcbeat/splittingsolver.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat/utils.py` & `cbcbeat-2023.1.0/cbcbeat/utils.py`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/cbcbeat.egg-info/PKG-INFO` & `cbcbeat-2023.1.0/cbcbeat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcbeat
-Version: 2023.0.0
+Version: 2023.1.0
 Summary: An adjoint-enabled framework for computational cardiac electrophysiology
 Author: J.E hake, P.E Farrel, S. W. Funke
 Author-email: "M. E. Rognes" <meg@simula.no>
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: goss
 Provides-Extra: gotran
```

### Comparing `cbcbeat-2023.0.0/cbcbeat.egg-info/SOURCES.txt` & `cbcbeat-2023.1.0/cbcbeat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcbeat-2023.0.0/pyproject.toml` & `cbcbeat-2023.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "cbcbeat"
-version = "2023.0.0"
+version = "2023.1.0"
 description = "An adjoint-enabled framework for computational cardiac electrophysiology"
 authors = [{name = "M. E. Rognes", email = "meg@simula.no"}, {name = "J.E hake"}, {name = "P.E Farrel"}, {name = "S. W. Funke"}]
 license = {file = "COPYING.LESSSER"}
 readme = "README.md"
 dependencies = [
     "fenics-dolfin",
     "numpy",
```

