# Comparing `tmp/emmet-builders-0.9.2.tar.gz` & `tmp/emmet-builders-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emmet-builders-0.9.2.tar", last modified: Thu Aug  5 00:57:49 2021, max compression
+gzip compressed data, was "dist/emmet-builders-0.9.3.tar", last modified: Thu Aug  5 01:31:11 2021, max compression
```

## Comparing `emmet-builders-0.9.2.tar` & `emmet-builders-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet/builders/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet/builders/feff/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/feff/xas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet/builders/materials/
--rw-r--r--   0 runner    (1001) docker     (121)    15593 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/electrodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    22553 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/electronic_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/optimade.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/oxidation_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     8561 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/provenance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/robocrys.py
--rw-r--r--   0 runner    (1001) docker     (121)     5997 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/substrates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5803 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/materials/summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet/builders/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10879 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/vasp/materials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/vasp/task_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12004 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/emmet/builders/vasp/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/emmet_builders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-05 00:57:49.000000 emmet-builders-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      740 2021-08-05 00:57:42.000000 emmet-builders-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet/builders/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet/builders/feff/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/feff/xas.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet/builders/materials/
+-rw-r--r--   0 runner    (1001) docker     (121)    15593 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/electrodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22553 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/electronic_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/optimade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/oxidation_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8560 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/robocrys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5997 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/substrates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5803 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/materials/summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2345 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet/builders/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10879 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/vasp/materials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/vasp/task_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12004 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/emmet/builders/vasp/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/emmet_builders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-05 01:31:11.000000 emmet-builders-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2021-08-05 01:31:07.000000 emmet-builders-0.9.3/setup.py
```

### Comparing `emmet-builders-0.9.2/emmet/builders/feff/xas.py` & `emmet-builders-0.9.3/emmet/builders/feff/xas.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/electrodes.py` & `emmet-builders-0.9.3/emmet/builders/materials/electrodes.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/electronic_structure.py` & `emmet-builders-0.9.3/emmet/builders/materials/electronic_structure.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/optimade.py` & `emmet-builders-0.9.3/emmet/builders/materials/optimade.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/oxidation_states.py` & `emmet-builders-0.9.3/emmet/builders/materials/oxidation_states.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/provenance.py` & `emmet-builders-0.9.3/emmet/builders/materials/provenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                     material_id=mat["material_id"], snls=matched_snls
                 )
 
                 doc.authors.append(self.settings.DEFAULT_AUTHOR)
                 doc.history.append(self.settings.DEFAULT_HISTORY)
                 doc.references.append(self.settings.DEFAULT_REFERENCE)
 
-                snl_docs.append(doc.dict(exclude_unset=True))
+                snl_docs.append(doc.dict(exclude_none=True))
 
         return snl_docs
 
     def match(self, snls, mat):
         """
         Finds a material doc that matches with the given snl
         Args:
```

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/robocrys.py` & `emmet-builders-0.9.3/emmet/builders/materials/robocrys.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/substrates.py` & `emmet-builders-0.9.3/emmet/builders/materials/substrates.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/materials/summary.py` & `emmet-builders-0.9.3/emmet/builders/materials/summary.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/settings.py` & `emmet-builders-0.9.3/emmet/builders/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/utils.py` & `emmet-builders-0.9.3/emmet/builders/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/vasp/materials.py` & `emmet-builders-0.9.3/emmet/builders/vasp/materials.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/vasp/task_validator.py` & `emmet-builders-0.9.3/emmet/builders/vasp/task_validator.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet/builders/vasp/thermo.py` & `emmet-builders-0.9.3/emmet/builders/vasp/thermo.py`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/emmet_builders.egg-info/SOURCES.txt` & `emmet-builders-0.9.3/emmet_builders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-builders-0.9.2/setup.py` & `emmet-builders-0.9.3/setup.py`

 * *Files identical despite different names*

