# Comparing `tmp/emmet-core-0.9.2.tar.gz` & `tmp/emmet-core-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emmet-core-0.9.2.tar", last modified: Thu Aug  5 00:57:52 2021, max compression
+gzip compressed data, was "dist/emmet-core-0.9.3.tar", last modified: Thu Aug  5 01:31:08 2021, max compression
```

## Comparing `emmet-core-0.9.2.tar` & `emmet-core-0.9.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-08-05 00:57:52.000000 emmet-core-0.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet/core/
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8460 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/electrode.py
--rw-r--r--   0 runner    (1001) docker     (121)    14973 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/electronic_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet/core/feff/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/feff/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/material.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/material_property.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/mpid.py
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/optimade.py
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/oxidation_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/polar.py
--rw-r--r--   0 runner    (1001) docker     (121)     6580 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/provenance.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/robocrys.py
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     9123 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/structure_group.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet/core/substrates/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   377842 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/substrates/structures.json
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/substrates/substrates.py
--rw-r--r--   0 runner    (1001) docker     (121)    12267 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/thermo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5572 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet/core/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet/core/vasp/calc_types/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/calc_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/calc_types/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/calc_types/run_types.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/calc_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7730 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/material.py
--rw-r--r--   0 runner    (1001) docker     (121)     6358 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     8610 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/vasp/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/xas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2021-08-05 00:57:45.000000 emmet-core-0.9.2/emmet/core/xrd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-05 00:57:52.000000 emmet-core-0.9.2/emmet_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-08-05 00:57:45.000000 emmet-core-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-05 00:57:52.000000 emmet-core-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-08-05 00:57:45.000000 emmet-core-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-08-05 01:31:08.000000 emmet-core-0.9.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8460 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/electrode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14940 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/electronic_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet/core/feff/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/feff/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2958 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/material.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/material_property.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3044 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/mpid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4321 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/optimade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/oxidation_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/polar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6555 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/robocrys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4391 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9123 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/structure_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet/core/substrates/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   377842 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/substrates/structures.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4434 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/substrates/substrates.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12298 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4942 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5572 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet/core/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet/core/vasp/calc_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/calc_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/calc_types/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/calc_types/run_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3741 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/calc_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7730 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/material.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6333 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8610 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/vasp/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9019 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/xas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3375 2021-08-05 01:31:04.000000 emmet-core-0.9.3/emmet/core/xrd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-05 01:31:08.000000 emmet-core-0.9.3/emmet_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2021-08-05 01:31:04.000000 emmet-core-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-05 01:31:08.000000 emmet-core-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2021-08-05 01:31:04.000000 emmet-core-0.9.3/setup.py
```

### Comparing `emmet-core-0.9.2/emmet/core/base.py` & `emmet-core-0.9.3/emmet/core/base.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/electrode.py` & `emmet-core-0.9.3/emmet/core/electrode.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/electronic_structure.py` & `emmet-core-0.9.3/emmet/core/electronic_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Core definition of an Electronic Structure """
 from __future__ import annotations
 
 from collections import defaultdict
 from datetime import datetime
 from math import isnan
 from typing import Dict, Type, TypeVar, Union
-import numpy as np
 
+import numpy as np
 from pydantic import BaseModel, Field
 from pymatgen.analysis.magnetism.analyzer import (
     CollinearMagneticStructureAnalyzer,
     Ordering,
 )
 from pymatgen.core import Structure
 from pymatgen.core.periodic_table import Element
@@ -117,14 +117,16 @@
 
 
 class ElectronicStructureDoc(PropertyDoc, ElectronicStructureSummary):
     """
     Definition for a core Electronic Structure Document
     """
 
+    property_name = "electronc_structure"
+
     bandstructure: BandstructureData = Field(
         None, description="Band structure data for the material."
     )
 
     dos: DosData = Field(None, description="Density of states data for the material.")
 
     last_updated: datetime = Field(
@@ -370,24 +372,20 @@
         dos_cbm, dos_vbm = dos_obj.get_cbm_vbm()
         dos_gap = max(dos_cbm - dos_vbm, 0.0)
 
         if bs_gap is not None and bs_gap <= dos_gap + 0.2:
             summary_task = bs_entry.setyawan_curtarolo.task_id
             summary_band_gap = bs_gap
             summary_cbm = (
-                bs_entry.setyawan_curtarolo.cbm.get(  # type: ignore
-                    "energy", None
-                )
+                bs_entry.setyawan_curtarolo.cbm.get("energy", None)  # type: ignore
                 if bs_entry.setyawan_curtarolo.cbm is not None
                 else None
             )
             summary_vbm = (
-                bs_entry.setyawan_curtarolo.vbm.get(  # type: ignore
-                    "energy", None
-                )
+                bs_entry.setyawan_curtarolo.vbm.get("energy", None)  # type: ignore
                 if bs_entry.setyawan_curtarolo.cbm is not None
                 else None
             )  # type: ignore
             summary_efermi = bs_entry.setyawan_curtarolo.efermi
             is_gap_direct = bs_entry.setyawan_curtarolo.is_gap_direct
             is_metal = bs_entry.setyawan_curtarolo.is_metal
             summary_magnetic_ordering = bs_entry.setyawan_curtarolo.magnetic_ordering
```

### Comparing `emmet-core-0.9.2/emmet/core/feff/task.py` & `emmet-core-0.9.3/emmet/core/feff/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Core definition of a VASP Task Document """
-from typing import Any, ClassVar, Dict, List
+from typing import Any, Dict, List
 
 from pydantic import Field
 from pymatgen.analysis.xas.spectrum import XAS
 from pymatgen.core import Structure
 from pymatgen.core.periodic_table import Element
 
 from emmet.core.structure import StructureMetadata
@@ -23,15 +23,15 @@
     EXAFS = "EXAFS"
     XAFS = "XAFS"
 
 
 class TaskDocument(BaseTaskDocument, StructureMetadata):
     """Task Document for a FEFF XAS Calculation. Doesn't support EELS for now"""
 
-    calc_code: ClassVar[str] = "FEFF"
+    calc_code = "FEFF"
 
     structure: Structure
     input_parameters: Dict[str, Any] = Field(
         {}, description="Input parameters for the FEFF calculation"
     )
     spectrum: List[List[float]] = Field(
         [[]], description="Raw spectrum data from FEFF xmu.dat or eels.dat"
```

### Comparing `emmet-core-0.9.2/emmet/core/material.py` & `emmet-core-0.9.3/emmet/core/material.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/material_property.py` & `emmet-core-0.9.3/emmet/core/material_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Core definition of a Materials Document """
 from __future__ import annotations
 
 from datetime import datetime
-from typing import ClassVar, Sequence, Type, TypeVar
+from typing import Sequence, Type, TypeVar
 
 from pydantic import Field
 from pymatgen.core import Structure
 
 from emmet.core.material import PropertyOrigin
 from emmet.core.mpid import MPID
 from emmet.core.structure import StructureMetadata
@@ -17,15 +17,15 @@
 class PropertyDoc(StructureMetadata):
     """
     Base model definition for any singular materials property. This may contain any amount
     of structure metadata for the purpose of search
     This is intended to be inherited and extended not used directly
     """
 
-    property_name: ClassVar[str]
+    property_name: str
     material_id: MPID = Field(
         ...,
         description="The ID of the material, used as a universal reference across proeprty documents."
         "This comes in the form of an MPID or int",
     )
 
     last_updated: datetime = Field(
```

### Comparing `emmet-core-0.9.2/emmet/core/mpid.py` & `emmet-core-0.9.3/emmet/core/mpid.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/optimade.py` & `emmet-core-0.9.3/emmet/core/optimade.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/oxidation_states.py` & `emmet-core-0.9.3/emmet/core/oxidation_states.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from emmet.core.material_property import PropertyDoc
 from emmet.core.mpid import MPID
 
 
 class OxidationStateDoc(PropertyDoc):
     """Oxidation states computed from the structure"""
 
+    property_name = "oxidation"
+
     possible_species: List[str] = Field(
         description="Possible charged species in this material"
     )
     possible_valences: List[float] = Field(
         description="List of valences for each site in this material"
     )
     average_oxidation_states: Dict[str, float] = Field(
```

### Comparing `emmet-core-0.9.2/emmet/core/polar.py` & `emmet-core-0.9.3/emmet/core/polar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Core definition for Polar property Document """
-from typing import ClassVar, Tuple
+from typing import Tuple
 
 import numpy as np
 from pydantic import Field
 from pymatgen.analysis.piezo import PiezoTensor as BasePiezoTensor
 
 from emmet.core import SETTINGS
 from emmet.core.material_property import PropertyDoc
@@ -15,15 +15,15 @@
 
 
 class Dielectric(PropertyDoc):
     """
     A dielectric property block
     """
 
-    property_name: ClassVar[str] = "dielectric"
+    property_name = "dielectric"
 
     total: Matrix3D = Field(description="Total dielectric response")
     ionic: Matrix3D = Field(
         description="Dielectric response due to atomic rearrangement"
     )
     electronic: Matrix3D = Field(
         description="Dielectric response due to electron rearrangement"
@@ -58,15 +58,15 @@
 
 
 class Piezoelectric(PropertyDoc):
     """
     A dielectric package block
     """
 
-    property_name: ClassVar[str] = "piezoelectric"
+    property_name = "piezoelectric"
 
     total: PiezoTensor = Field(None, description="")
     ionic: PiezoTensor = Field(None, description="")
     electronic: PiezoTensor = Field(None, description="")
 
     e_ij_max: float = Field(None, description="")
     max_direction: Tuple[int, int, int] = Field(
```

### Comparing `emmet-core-0.9.2/emmet/core/provenance.py` & `emmet-core-0.9.3/emmet/core/provenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Core definition of a Provenance Document """
 import warnings
 from datetime import datetime
-from typing import ClassVar, Dict, List, Optional
+from typing import Dict, List, Optional
 
 from pybtex.database import BibliographyData, parse_string
 from pybtex.errors import set_strict_mode
 from pydantic import BaseModel, Field, root_validator, validator
 
 from emmet.core.material_property import PropertyDoc
 from emmet.core.mpid import MPID
@@ -100,15 +100,15 @@
 
 
 class ProvenanceDoc(PropertyDoc):
     """
     A provenance property block
     """
 
-    property_name: ClassVar[str] = "provenance"
+    property_name = "provenance"
 
     created_at: datetime = Field(
         ...,
         description="creation date for the first structure corresponding to this material",
     )
 
     references: List[str] = Field(
```

### Comparing `emmet-core-0.9.2/emmet/core/robocrys.py` & `emmet-core-0.9.3/emmet/core/robocrys.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,19 @@
 
 
 class RobocrystallogapherDoc(PropertyDoc):
     """
     This document contains the descriptive data from robocrystallographer
     for a material:
         Structural features, mineral prototypes, dimensionality, ...
+
     """
 
+    property_name = "robocrys"
+
     description: str = Field(
         description="Decription text from robocrytallographer.",
     )
 
     condensed_structure: CondensedStructureData = Field(
         description="Condensed structure data from robocrytallographer.",
     )
```

### Comparing `emmet-core-0.9.2/emmet/core/settings.py` & `emmet-core-0.9.3/emmet/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/spectrum.py` & `emmet-core-0.9.3/emmet/core/spectrum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ Core definition of Spectrum document """
 from datetime import datetime
-from typing import ClassVar, List
+from typing import List
 
 from pydantic import Field
 
 from emmet.core.mpid import MPID
 from emmet.core.structure import StructureMetadata
 
 
 class SpectrumDoc(StructureMetadata):
     """
     Base model definition for any spectra document. This should contain
     metadata on the structure the spectra pertains to
     """
 
-    spectrum_name: ClassVar[str]
+    spectrum_name: str
 
     material_id: MPID = Field(
         ...,
         description="The ID of the material, used as a universal reference across proeprty documents."
         "This comes in the form: mp-******",
     )
```

### Comparing `emmet-core-0.9.2/emmet/core/structure.py` & `emmet-core-0.9.3/emmet/core/structure.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/structure_group.py` & `emmet-core-0.9.3/emmet/core/structure_group.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/stubs.py` & `emmet-core-0.9.3/emmet/core/stubs.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/substrates/structures.json` & `emmet-core-0.9.3/emmet/core/substrates/structures.json`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/substrates/substrates.py` & `emmet-core-0.9.3/emmet/core/substrates/substrates.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,16 @@
                 strain=match.strain,
             )
 
 
 class SubstratesDoc(PropertyDoc):
     """Substrate matches computed for the material"""
 
+    property_name = "substrates"
+
     substrates: List[SubstrateMatch] = Field(
         description="The list of matches for all given substrates"
     )
 
     @classmethod
     def from_structure(  # type: ignore[override]
         cls,
```

### Comparing `emmet-core-0.9.2/emmet/core/summary.py` & `emmet-core-0.9.3/emmet/core/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,16 @@
 
 class SummaryDoc(PropertyDoc):
     """
     Summary information about materials and their properties, useful for materials
     screening studies and searching.
     """
 
+    property_name = "summary"
+
     # Materials
 
     deprecated: bool = Field(
         ..., description="Whether the material is tagged as deprecated"
     )
     structure: Structure = Field(
         ..., description="The lowest energy structure for this material"
```

### Comparing `emmet-core-0.9.2/emmet/core/symmetry.py` & `emmet-core-0.9.3/emmet/core/symmetry.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/task.py` & `emmet-core-0.9.3/emmet/core/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """ Core definition of a Task Document which represents a calculation from some program"""
 from datetime import datetime
-from typing import ClassVar, List
+from typing import List
 
 from pydantic import Field
 
 from emmet.core.base import EmmetBaseModel
 from emmet.core.mpid import MPID
 
 
 class TaskDocument(EmmetBaseModel):
     """
     Definition of Task Document
     """
 
-    calc_code: ClassVar[str] = Field(
-        ..., description="The calculation code used to compute this task"
-    )
+    calc_code: str = Field(description="The calculation code used to compute this task")
     version: str = Field(None, description="The version of the calculation code")
     dir_name: str = Field(None, description="The directory for this task")
     task_id: MPID = Field(None, description="the Task ID For this document")
 
     completed: bool = Field(False, description="Whether this calcuation completed")
     completed_at: datetime = Field(
         None, description="Timestamp for when this task was completed"
```

### Comparing `emmet-core-0.9.2/emmet/core/thermo.py` & `emmet-core-0.9.3/emmet/core/thermo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Core definition of a Thermo Document """
 from collections import defaultdict
-from typing import ClassVar, Dict, List, Union
+from typing import Dict, List, Union
 
 from pydantic import BaseModel, Field
 from pymatgen.analysis.phase_diagram import PhaseDiagram
 from pymatgen.entries.computed_entries import ComputedEntry, ComputedStructureEntry
 
 from emmet.core.material_property import PropertyDoc
 from emmet.core.mpid import MPID
@@ -29,17 +29,15 @@
 
 
 class ThermoDoc(PropertyDoc):
     """
     A thermo entry document
     """
 
-    property_name: ClassVar[str] = Field(
-        "thermo", description="The subfield name for this property"
-    )
+    property_name = "thermo"
 
     uncorrected_energy_per_atom: float = Field(
         ..., description="The total DFT energy of this material per atom in eV/atom"
     )
 
     energy_per_atom: float = Field(
         ...,
```

### Comparing `emmet-core-0.9.2/emmet/core/utils.py` & `emmet-core-0.9.3/emmet/core/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/vasp/calc_types/generate.py` & `emmet-core-0.9.3/emmet/core/vasp/calc_types/generate.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/vasp/calc_types/run_types.yaml` & `emmet-core-0.9.3/emmet/core/vasp/calc_types/run_types.yaml`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/vasp/calc_types/utils.py` & `emmet-core-0.9.3/emmet/core/vasp/calc_types/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/vasp/material.py` & `emmet-core-0.9.3/emmet/core/vasp/material.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/vasp/task.py` & `emmet-core-0.9.3/emmet/core/vasp/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Core definition of a VASP Task Document """
-from typing import Any, ClassVar, Dict, List, Union
+from typing import Any, Dict, List, Union
 
 from pydantic import BaseModel, Field
 from pymatgen.analysis.structure_analyzer import oxide_type
 from pymatgen.core import Structure
 from pymatgen.entries.computed_entries import ComputedEntry, ComputedStructureEntry
 
 from emmet.core.math import Matrix3D, Vector3D
@@ -88,15 +88,15 @@
 
 
 class TaskDocument(BaseTaskDocument, StructureMetadata):
     """
     Definition of VASP Task Document
     """
 
-    calc_code: ClassVar[str] = "VASP"
+    calc_code = "VASP"
     run_stats: Dict[str, RunStatistics] = Field(
         {},
         description="Summary of runtime statisitics for each calcualtion in this task",
     )
 
     is_valid: bool = Field(
         True, description="Whether this task document passed validation or not"
```

### Comparing `emmet-core-0.9.2/emmet/core/vasp/validation.py` & `emmet-core-0.9.3/emmet/core/vasp/validation.py`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/emmet/core/xas.py` & `emmet-core-0.9.3/emmet/core/xas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from itertools import groupby
-from typing import ClassVar, List
+from typing import List
 
 import numpy as np
 from pydantic import Field
 from pymatgen.analysis.xas.spectrum import XAS, site_weighted_spectrum
 from pymatgen.core.periodic_table import Element
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
@@ -44,15 +44,15 @@
 
 
 class XASDoc(SpectrumDoc):
     """
     Document describing a XAS Spectrum.
     """
 
-    spectrum_name: ClassVar[str] = "XAS"
+    spectrum_name = "XAS"
 
     spectrum: XAS
 
     task_ids: List[str] = Field(
         ...,
         title="Calculation IDs",
         description="List of Calculations IDs used to make this XAS spectrum.",
@@ -62,15 +62,18 @@
     spectrum_type: Type = Field(..., title="XAS Spectrum Type")
     edge: Edge = Field(
         ..., title="Absorption Edge", description="The interaction edge for XAS"
     )
 
     @classmethod
     def from_spectrum(
-        cls, xas_spectrum: XAS, material_id: MPID, **kwargs,
+        cls,
+        xas_spectrum: XAS,
+        material_id: MPID,
+        **kwargs,
     ):
         spectrum_type = xas_spectrum.spectrum_type
         el = xas_spectrum.absorbing_element
         edge = xas_spectrum.edge
         xas_id = f"{material_id}-{spectrum_type}-{el}-{edge}"
 
         if xas_spectrum.absorbing_index is not None:
@@ -123,23 +126,27 @@
             ),
         )
 
         # Generate Merged Spectra
         # Dictionary of all site to spectra mapping
         sites_to_spectra = {
             index: list(group)
-            for index, group in groupby(all_spectra, key=lambda x: x.absorbing_index,)
+            for index, group in groupby(
+                all_spectra,
+                key=lambda x: x.absorbing_index,
+            )
         }
 
         # perform spectra merging
         for site, spectra in sites_to_spectra.items():
             type_to_spectra = {
                 index: list(group)
                 for index, group in groupby(
-                    spectra, key=lambda x: (x.edge, x.spectrum_type),
+                    spectra,
+                    key=lambda x: (x.edge, x.spectrum_type),
                 )
             }
             # Make K-edge XAFS spectra by merging XANES + EXAFS
             if ("K", "XANES") in type_to_spectra and ("K", "EXAFS") in type_to_spectra:
                 xanes = type_to_spectra[("K", "XANES")][-1]
                 exafs = type_to_spectra[("K", "EXAFS")][-1]
                 try:
```

### Comparing `emmet-core-0.9.2/emmet/core/xrd.py` & `emmet-core-0.9.3/emmet/core/xrd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import ClassVar, Dict
+from typing import Dict
 
 import numpy as np
 from pydantic import Field, root_validator
 from pymatgen.analysis.diffraction.xrd import (
     WAVELENGTHS,
     DiffractionPattern,
     XRDCalculator,
@@ -25,15 +25,15 @@
 
 
 class XRDDoc(SpectrumDoc):
     """
     Document describing a XRD Diffraction Pattern
     """
 
-    spectrum_name: ClassVar[str] = "XRD"
+    spectrum_name = "XRD"
 
     spectrum: DiffractionPattern
     min_two_theta: float
     max_two_theta: float
     wavelength: float = Field(..., description="Wavelength for the diffraction source")
     target: Element = Field(
         None, description="Target element for the diffraction source"
```

### Comparing `emmet-core-0.9.2/emmet_core.egg-info/SOURCES.txt` & `emmet-core-0.9.3/emmet_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-core-0.9.2/setup.py` & `emmet-core-0.9.3/setup.py`

 * *Files identical despite different names*

