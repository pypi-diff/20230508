# Comparing `tmp/moped-1.9.9.tar.gz` & `tmp/moped-1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moped-1.9.9.tar", max compression
+gzip compressed data, was "dist/moped-1rc1.tar", last modified: Mon Apr 27 09:12:17 2020, max compression
```

## Comparing `moped-1.9.9.tar` & `moped-1rc1.tar`

### file list

```diff
@@ -1,23 +1,50 @@
--rw-r--r--   0        0        0    35079 2022-02-21 13:21:48.474458 moped-1.9.9/LICENSE
--rw-r--r--   0        0        0     2203 2022-02-21 13:21:48.474458 moped-1.9.9/README.md
--rw-r--r--   0        0        0     3227 2022-02-21 13:21:48.479458 moped-1.9.9/pyproject.toml
--rw-r--r--   0        0        0      716 2022-02-21 13:21:48.479458 moped-1.9.9/src/moped/__init__.py
--rw-r--r--   0        0        0        0 2022-02-21 13:21:48.479458 moped-1.9.9/src/moped/core/__init__.py
--rw-r--r--   0        0        0     1123 2022-02-21 13:21:48.479458 moped-1.9.9/src/moped/core/compound.py
--rw-r--r--   0        0        0     1230 2022-02-21 13:21:48.479458 moped-1.9.9/src/moped/core/constants.py
--rw-r--r--   0        0        0      329 2022-02-21 13:21:48.479458 moped-1.9.9/src/moped/core/kinetic_data.py
--rw-r--r--   0        0        0    95922 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/core/model.py
--rw-r--r--   0        0        0      264 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/core/monomer.py
--rw-r--r--   0        0        0     4011 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/core/reaction.py
--rw-r--r--   0        0        0        0 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/py.typed
--rw-r--r--   0        0        0      409 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/topological/__init__.py
--rw-r--r--   0        0        0    10449 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/topological/blast.py
--rw-r--r--   0        0        0     7125 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/topological/gapfilling.py
--rw-r--r--   0        0        0     7092 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/topological/scope.py
--rw-r--r--   0        0        0     4344 2022-02-21 13:21:48.480458 moped-1.9.9/src/moped/topological/treesearch.py
--rw-r--r--   0        0        0      573 2022-02-21 13:21:48.481459 moped-1.9.9/src/moped/utils/__init__.py
--rw-r--r--   0        0        0     5124 2022-02-21 13:21:48.481459 moped-1.9.9/src/moped/utils/comparison.py
--rw-r--r--   0        0        0    15145 2022-02-21 13:21:48.481459 moped-1.9.9/src/moped/utils/sbml.py
--rw-r--r--   0        0        0     1801 2022-02-21 13:21:48.481459 moped-1.9.9/src/moped/utils/serialize.py
--rw-r--r--   0        0        0     3331 2022-02-21 13:22:24.378719 moped-1.9.9/setup.py
--rw-r--r--   0        0        0     4000 2022-02-21 13:22:24.379191 moped-1.9.9/PKG-INFO
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     2697 2020-04-27 09:12:17.000000 moped-1rc1/PKG-INFO
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     1627 2020-04-27 08:56:15.000000 moped-1rc1/README.md
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/moped/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)      175 2020-02-20 12:43:30.000000 moped-1rc1/moped/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/moped/core/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        1 2020-02-20 12:32:45.000000 moped-1rc1/moped/core/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     5285 2020-04-12 07:45:41.000000 moped-1rc1/moped/core/compound.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     1161 2020-02-12 09:59:48.000000 moped-1rc1/moped/core/constants.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    93795 2020-04-15 08:34:24.000000 moped-1rc1/moped/core/model.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     7353 2020-03-12 11:18:26.000000 moped-1rc1/moped/core/reaction.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/moped/databases/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)       21 2020-01-30 08:25:21.000000 moped-1rc1/moped/databases/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    52051 2020-03-12 12:12:49.000000 moped-1rc1/moped/databases/cyc.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/moped/topological/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)      171 2020-02-20 12:31:29.000000 moped-1rc1/moped/topological/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     7310 2020-04-13 11:42:22.000000 moped-1rc1/moped/topological/blast.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     6697 2020-04-12 11:13:58.000000 moped-1rc1/moped/topological/gapfilling.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     6360 2020-04-12 08:31:02.000000 moped-1rc1/moped/topological/scope.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     3489 2020-03-04 07:47:04.000000 moped-1rc1/moped/topological/treesearch.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/moped/utils/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       43 2020-03-02 08:00:48.000000 moped-1rc1/moped/utils/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)      425 2020-04-12 08:25:42.000000 moped-1rc1/moped/utils/utils.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/moped.egg-info/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     2697 2020-04-27 09:12:17.000000 moped-1rc1/moped.egg-info/PKG-INFO
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)      991 2020-04-27 09:12:17.000000 moped-1rc1/moped.egg-info/SOURCES.txt
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        1 2020-04-27 09:12:17.000000 moped-1rc1/moped.egg-info/dependency_links.txt
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        1 2019-11-14 09:01:52.000000 moped-1rc1/moped.egg-info/not-zip-safe
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)      102 2020-04-27 09:12:17.000000 moped-1rc1/moped.egg-info/requires.txt
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)       12 2020-04-27 09:12:17.000000 moped-1rc1/moped.egg-info/top_level.txt
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       38 2020-04-27 09:12:17.000000 moped-1rc1/setup.cfg
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     1774 2020-04-02 12:33:43.000000 moped-1rc1/setup.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/tests/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        0 2020-01-30 08:25:21.000000 moped-1rc1/tests/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/tests/core/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        0 2020-01-30 08:25:21.000000 moped-1rc1/tests/core/__init__.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     8308 2020-03-04 07:58:30.000000 moped-1rc1/tests/core/test_cobra_interface.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     4940 2020-04-12 07:58:45.000000 moped-1rc1/tests/core/test_compound.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)   116959 2020-03-04 08:17:06.000000 moped-1rc1/tests/core/test_model.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)    10425 2020-04-12 10:46:37.000000 moped-1rc1/tests/core/test_reaction.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/tests/databases/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        0 2020-01-30 08:25:21.000000 moped-1rc1/tests/databases/__init__.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)   102880 2020-03-12 12:14:27.000000 moped-1rc1/tests/databases/test_cycparser.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    58164 2020-02-20 09:36:27.000000 moped-1rc1/tests/databases/test_cycparser_full.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-04-27 09:12:17.000000 moped-1rc1/tests/topological/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        0 2020-01-30 08:25:21.000000 moped-1rc1/tests/topological/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    18521 2020-04-15 08:16:48.000000 moped-1rc1/tests/topological/test_blast.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)    16338 2020-04-12 11:20:46.000000 moped-1rc1/tests/topological/test_gapfilling.py
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     6655 2020-04-12 08:30:46.000000 moped-1rc1/tests/topological/test_scope.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-04-12 15:18:33.000000 moped-1rc1/tests/topological/test_treesearch.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `moped-1.9.9/src/moped/core/constants.py` & `moped-1rc1/moped/core/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """File containts constants for modelling purposes.
 
 This might be reworked in future versions, as it feels
 rather archaic. But so far it does its job.
 """
 
-from __future__ import annotations
-
-__all__ = ["BIOMASS_TEMPLATES"]
-
 BIOMASS_TEMPLATES = {
     "ecoli": {
         "TRP_c": -0.055234,
         "GLT_c": -0.255712,
         "MALONYL-COA_c": -3.1e-05,
         "GTP_c": -0.209121,
         "NADP_c": -0.000112,
```

### Comparing `moped-1.9.9/src/moped/core/model.py` & `moped-1rc1/moped/core/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,302 +1,186 @@
 """The main model class, with which users are supposed to interface."""
-from __future__ import annotations
-
-__all__ = ["Model"]
 
 import copy
-import dataclasses
-import json
-import pickle
-import re
-import warnings
-from collections import defaultdict
-from pathlib import Path
-from typing import (
-    Any,
-    DefaultDict,
-    Dict,
-    Iterable,
-    List,
-    Pattern,
-    Set,
-    Tuple,
-    Union,
-    cast,
-)
-
 import cobra
-import cycparser
-import libsbml
 import numpy as np
 import pandas as pd
-import yaml
+import pathlib
+import re
+import warnings
+from collections import defaultdict
 
 from .. import topological
-from ..utils import get_temporary_directory
-from ..utils.sbml import export_model as _export_model
-from .compound import Compound
 from .constants import BIOMASS_TEMPLATES
-from .kinetic_data import KineticData
-from .monomer import Monomer
+from .compound import Compound
 from .reaction import Reaction
+from ..databases import Cyc
+from ..utils import get_temporary_directory
+
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import modelbase.ode as ode
     from modelbase.ode import ratelaws as rl
 
 
-@dataclasses.dataclass
-class SearchResult:
-    reactions: List[str]
-    compounds: List[str]
-
-
 class Model:
     """The main model class."""
 
     def __init__(
         self,
-        compounds: Iterable[Compound] | None = None,
-        reactions: Iterable[Reaction] | None = None,
-        compartments: Dict[str, str] | None = None,
-        objective: Dict[str, float] | None = None,
-        minimal_seed: Set[str] | None = None,
-        cofactor_pairs: Dict[str, str] | None = None,
-        monomers: Dict[str, Monomer] | None = None,
-        # gpr_annotations: Dict[str, List[Set[str]]] | None = None,
-        # kinetic_data: Dict[str, Dict[str, KineticData]] | None = None,
-        name: str | None = None,
-    ) -> None:
-        self.name: str = name if name is not None else "Model"
-        self.compartments: Dict[str, str] = {}
-        self.compounds: Dict[str, Compound] = {}
-        self.base_compounds: Dict[str, Set[str]] = {}
-        self.reactions: Dict[str, Reaction] = {}
-        self.base_reactions: Dict[str, Set[str]] = {}
-        self.variant_reactions: Dict[str, Set[str]] = {}
-        self.pathways: Dict[str, Set[str]] = {}
-        self.objective: Dict[str, float] = {}
-        self.cofactor_pairs: Dict[str, str] = {}
-        self.minimal_seed = set() if minimal_seed is None else minimal_seed
-        self.monomers: Dict[str, Monomer] = {}
-        # self.kinetic_data: Dict[str, Dict[str, KineticData]] = {}
-        # self.gpr_annotations: Dict[str, List[Set[str]]] = {}
-
-        # Filled by routines
-        self._compound_types: Dict[str, Set[str]] = {}
-        self._reaction_types: Dict[str, Set[str]] = {}
-        self._base_cofactor_pairs: Dict[str, str] = {}
-        # Temporary containers
-        self._duplicate_reactions: Set[str] = set()
+        compounds=None,
+        reactions=None,
+        compartments=None,
+        objective=None,
+        name=None,
+    ):
+        """Initialize a model object.
 
+        Parameters
+        ----------
+        compounds: iterable, optional
+            Iterable of moped.Compound objects
+        reactions: iterable, optional
+            Iterable of moped.Reaction objects
+        compartments: dict, optional
+            compartment_id: suffix mapping
+        objective: dict(str: float), optional
+            Mapping of reaction ids to objective coefficient
+        name: str, optional
+        """
+        self.name = name if name is not None else "Model"
+        self.compartments = {}
+        self.compounds = {}
+        self.base_compounds = {}
+        self._compound_types = {}
+        self.reactions = {}
+        self._reaction_types = {}
+        self.base_reactions = {}
+        self.variant_reactions = {}
+        self._duplicate_reactions = set()
+        self.pathways = {}
+        self.objective = {}
+        self._monomers = {}
         if compartments is not None:
             self.add_compartments(compartments=compartments)
         if compounds is not None:
             self.add_compounds(compounds=compounds)
-        if cofactor_pairs is not None:
-            for strong, weak in cofactor_pairs.items():
-                self.add_cofactor_pair(strong, weak)
         if reactions is not None:
             self.add_reactions(reactions=reactions)
         if objective is not None:
             self.set_objective(objective=objective)
-        if monomers is not None:
-            self.add_monomers(monomers)
-        # if gpr_annotations is not None:
-        #     self.add_gpr_annotations(gpr_annotations)
-        # if kinetic_data is not None:
-        #     self.add_kinetic_data(kinetic_data)
+        self.cofactor_pairs = {}
+        self.minimal_seed = set()
 
-    def __repr__(self) -> str:
-        s = f"Model: {self.name}\n"
+    def __repr__(self):
+        """Return model representation."""
+        if self.name is not None:
+            s = f"Model: {self.name}\n"
+        else:
+            s = f"Model:\n"
         s += f"    compounds: {len(self.compounds)}\n"
         s += f"    reactions: {len(self.reactions)}\n"
         return s
 
-    def __str__(self) -> str:
+    def __str__(self):
+        """Return model string representation."""
         s = f"Model: {self.name}\n"
         s += f"    compounds: {len(self.compounds)}\n"
         s += f"    reactions: {len(self.reactions)}\n"
         return s
 
-    def __enter__(self) -> "Model":
+    def __enter__(self):
         """Return and save a copy for context manager."""
         self._copy = self.copy()
         return self.copy()
 
-    def __exit__(
-        self,
-        exception_type: Any,
-        exception_value: Any,
-        exception_traceback: Any,
-    ) -> None:
+    def __exit__(self, exception_type, exception_value, exception_traceback):
         """Restore any changes made to the model."""
         self.__dict__ = self._copy.__dict__
 
-    def __add__(self, other: object) -> "Model":
-        if not isinstance(other, Model):
-            return NotImplemented
-        m1 = self.copy()
-        m1.add_compartments(other.compartments)
-        m1.add_compounds(other.compounds.values())
-        m1.add_reactions(other.reactions.values())
-        return m1
-
-    def __iadd__(self, other: object) -> "Model":
-        if not isinstance(other, Model):
-            return NotImplemented
-        self.add_compartments(other.compartments)
-        self.add_compounds(other.compounds.values())
-        self.add_reactions(other.reactions.values())
-        return self
-
-    def __sub__(self, other: object) -> "Model":
-        if not isinstance(other, Model):
-            return NotImplemented
-        m = self.copy()
-        m.remove_compartments([k for k in self.compartments.keys() if k in other.compartments])
-        m.remove_compounds([k for k in self.compounds.keys() if k in other.compounds])
-        m.remove_reactions([k for k in self.reactions.keys() if k in other.reactions])
-        return m
-
-    def __isub__(self, other: object) -> "Model":
-        if not isinstance(other, Model):
-            return NotImplemented
-        self.remove_compartments([k for k in self.compartments.keys() if k in other.compartments])
-        self.remove_compounds([k for k in self.compounds.keys() if k in other.compounds])
-        self.remove_reactions([k for k in self.reactions.keys() if k in other.reactions])
-        return self
-
-    def __and__(self, other: object) -> "Model":
-        if not isinstance(other, Model):
-            return NotImplemented
-        m = self.copy()
-        m.add_compartments({k: v for k, v in self.compartments.items() if k in other.compartments})
-        m.add_compounds([v for k, v in self.compounds.items() if k in other.compounds])
-        m.add_reactions([v for k, v in self.reactions.items() if k in other.reactions])
-        return m
-
-    def __or__(self, other: object) -> "Model":
-        if not isinstance(other, Model):
-            return NotImplemented
-        return self + other
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, Model):
-            return NotImplemented
-        return all(getattr(self, i) == getattr(other, i) for i in self.__dict__)
-
-    def copy(self) -> "Model":
+    def copy(self):
         """Create a deepcopy of the reaction.
 
         While this is more costly than shallow copies, it takes away
         the hassle of always keeping track if a shallow copy is what
         you want at the moment. So it's mostly for me not getting
         confused ;)
 
         Returns
         -------
         self: moped.Model
         """
         return copy.deepcopy(self)
 
-    def add_compartment(self, compartment_id: str, compartment_suffix: str) -> None:
+    def add_compartment(self, compartment_id, compartment_suffix):
         """Add a compartment to the model.
 
+        compartment_id: str
+            Name of the compartment, e.g. cytosol
+        compartment_suffix: str
+            Suffix of the compartment, e.g. c. Should not include the underscore.
+
         Examples
         --------
         model.add_compartment(compartment_id='cytosol', compartment_suffix='c')
         """
         self.compartments[compartment_id] = compartment_suffix
 
-    def add_compartments(self, compartments: Dict[str, str]) -> None:
+    def add_compartments(self, compartments):
         """Add multiple compartments to the model.
 
+        compartments: dict(str: str)
+            compartment_id: compartment_suffix
+
         Examples
         --------
         model.add_compartments(compartments={'cytosol': 'c'})
         """
         for compartment_id, compartment_suffix in compartments.items():
             self.add_compartment(
-                compartment_id=compartment_id,
-                compartment_suffix=compartment_suffix,
+                compartment_id=compartment_id, compartment_suffix=compartment_suffix
             )
 
-    def remove_compartment(self, compartment: str) -> None:
-        del self.compartments[compartment]
-
-    def remove_compartments(self, compartments: Iterable[str]) -> None:
-        for i in compartments:
-            self.remove_compartment(compartment=i)
-
-    def add_monomers(self, monomers: Dict[str, Monomer]) -> None:
-        self.monomers.update(monomers)
-
-    # def add_gpr_annotations(self, annotations: Dict[str, List[Set[str]]]) -> None:
-    #     self.gpr_annotations.update(annotations)
-
-    # def add_kinetic_data(self, kinetic_data: Dict[str, Dict[str, KineticData]]) -> None:
-    #     for rxn, d in kinetic_data.items():
-    #         for enzyme, data in d.items():
-    #             self.kinetic_data.setdefault(rxn, {}).setdefault(enzyme, data)
-
     ##########################################################################
     # Utils
     ##########################################################################
 
-    def _add_compartment_suffix(self, object_id: str, compartment_id: str) -> str:
+    def _add_compartment_suffix(self, object_id, compartment_id):
         """Add a compartment suffix (e.g. _e for extracellular) to the id.
 
         Raises
         ------
         KeyError
             If compartment does not exist
         """
         suffix = self.compartments[compartment_id]
         if suffix != "":
             return object_id + f"_{suffix}"
         return object_id
 
-    @staticmethod
-    def _strip_compartment_suffix(object_id: str, compartment_pattern: Pattern[str]) -> str:
-        """Split the compartment string from an object_id."""
+    def _strip_compartment_suffix(self, object_id, compartment_pattern):
+        """Split the compartment string from an object_id.
+
+        Parameters
+        ----------
+        object_id : str
+
+        Returns
+        -------
+        object_id : str
+            Object id without the compartment suffix, e.g. _e
+        """
         return re.sub(compartment_pattern, "", object_id)
 
     ##########################################################################
     # Creation routines
     ##########################################################################
 
-    def _fix_light_reaction_mass_balance(self) -> None:
-        """This one is really weird.
-        Memote requires us to give light a mass and then add another compound,
-        such that we can mass-balance the reactions. Yes.
-        """
-        if (cpd := self.compounds.get("Light_c")) is not None:
-            if "EXTRACELLULAR" not in self.compartments:  # can happen in rare cases
-                self.compartments["EXTRACELLULAR"] = "e"
-            cpd.formula = {"Photon": 1}
-            self.add_compound(
-                Compound(
-                    base_id="Light_used",
-                    compartment="EXTRACELLULAR",
-                    id="Light_used_e",
-                    charge=0,
-                    formula={"Photon": 1},
-                )
-            )
-            self.add_efflux("Light_used_e", "EXTRACELLULAR")
-            # for rxn_id in self.pathways.get("PWY-101", set()):
-            # reaction = self.reactions[rxn_id]
-            for reaction in self.reactions.values():
-                if "Light_c" in reaction.stoichiometries:
-                    reaction.stoichiometries["Light_used_e"] = -1 * reaction.stoichiometries["Light_c"]
-
-    def _fix_periplasm_proton_gradient(self) -> None:
+    def _fix_periplasm_proton_gradient(self):
         """Set reactions that do not match proton gradient criteria to irreversible.
 
         The criteria are the following:
         - All reactions of the following types are always kept
             TR-13 (Transport Energized by Phosphoanhydride-Bond Hydrolysis)
             TR-15 (Transport Energized by Decarboxylation)
             Membrane-Protein-Modification-Reactions
@@ -306,112 +190,114 @@
             TR-12 (Transport Energized by the Membrane Electrochemical Gradient)
         Keeping those reactions leads to thermodynamically infeasible loops, therefore
         they are reverted to a way that they only transport protons to the cytosol
         and are irreversible.
         """
         if "PERIPLASM" in self.get_model_compartment_ids():
             periplasm_recs = [
-                self.reactions[i] for i in self.get_transport_reactions(compartment_id="PERIPLASM")
+                self.reactions[i]
+                for i in self.get_transport_reactions(compartment_id="PERIPLASM")
             ]
-            proton_translocators = {i.id for i in periplasm_recs if "PROTON_p" in i.stoichiometries}
+            proton_translocators = {
+                i.id for i in periplasm_recs if "PROTON_p" in i.stoichiometries
+            }
             try:
                 tr13 = self.get_reactions_of_type(reaction_type="TR-13")
             except KeyError:
                 tr13 = set()
             try:
                 tr15 = self.get_reactions_of_type(reaction_type="TR-15")
             except KeyError:
                 tr15 = set()
             try:
-                mpmr = self.get_reactions_of_type(reaction_type="Membrane-Protein-Modification-Reactions")
+                mpmr = self.get_reactions_of_type(
+                    reaction_type="Membrane-Protein-Modification-Reactions"
+                )
             except KeyError:
                 mpmr = set()
             try:
-                etr = self.get_reactions_of_type(reaction_type="Electron-Transfer-Reactions")
+                etr = self.get_reactions_of_type(
+                    reaction_type="Electron-Transfer-Reactions"
+                )
             except KeyError:
                 etr = set()
             to_fix = proton_translocators.difference(tr13 | tr15 | etr | mpmr)
             for reaction_id in to_fix:
                 reaction = self.reactions[reaction_id]
                 if reaction.stoichiometries["PROTON_p"] > 0:
                     reaction.reverse_stoichiometry()
                 reaction.make_irreversible()
 
-    def _move_electron_transport_cofactors_to_cytosol(self) -> None:
+    def _move_electron_transport_cofactors_to_cytosol(self):
         """Move all periplasmatic electron transport cofactors into cytosol.
 
         This is done to keep the connectivity of the network.
         """
-        cofactors = {
+        cofactor_dict = {
             "Reduced-ferredoxins_p": "Reduced-ferredoxins_c",
             "Oxidized-ferredoxins_p": "Oxidized-ferredoxins_c",
             "Cytochromes-C-Reduced_p": "Cytochromes-C-Reduced_c",
             "Cytochromes-C-Oxidized_p": "Cytochromes-C-Oxidized_c",
             "NADPH_p": "NADPH_c",
             "NADP_p": "NADP_c",
             "NAD_p": "NAD_c",
             "ATP_p": "ATP_c",
             "ADP_p": "ADP_c",
         }
 
         try:
-            etr_reactions = self.get_reactions_of_type(reaction_type="Electron-Transfer-Reactions")
+            etr_reactions = self.get_reactions_of_type(
+                reaction_type="Electron-Transfer-Reactions"
+            )
         except KeyError:
             pass
         else:
             for reaction_id in tuple(etr_reactions):
-                reaction = copy.deepcopy(self.reactions[reaction_id])
-                if "PERIPLASM" in cast(str, reaction.compartment):
+                reaction = self.reactions[reaction_id].copy()
+                if "PERIPLASM" in reaction.compartment:
                     changed_cpds = False
                     for compound_id in tuple(reaction.stoichiometries):
-                        if compound_id in cofactors:
-                            reaction.stoichiometries[cofactors[compound_id]] = reaction.stoichiometries.pop(
-                                compound_id
-                            )
+                        if compound_id in cofactor_dict:
+                            reaction.stoichiometries[
+                                cofactor_dict[compound_id]
+                            ] = reaction.stoichiometries.pop(compound_id)
                             changed_cpds = True
                     if changed_cpds:
                         self.remove_reaction(
-                            reaction_id=reaction_id,
-                            remove_empty_references=False,
+                            reaction_id=reaction_id, remove_empty_references=False
                         )
-                        self._move_reaction_to_other_compartment(reaction)
-
-    def _move_reaction_to_other_compartment(self, reaction: Reaction) -> None:
-        reaction.id = cast(str, reaction.base_id)
-        if (count := reaction._var) is not None:
-            reaction.id += f"__var__{count}"
-        new_compartments = tuple(
-            sorted({cast(str, self.compounds[i].compartment) for i in reaction.stoichiometries})
-        )
-        if len(new_compartments) == 1:
-            compartment = new_compartments[0]
-            reaction.compartment = compartment
-            reaction.transmembrane = False
-            reaction.id += self._add_compartment_suffix(object_id="", compartment_id=compartment)
-        else:
-            reaction.compartment = new_compartments
-            reaction.transmembrane = True
-            for compartment_id in reaction.compartment:
-                reaction.id += self._add_compartment_suffix(object_id="", compartment_id=compartment_id)
-        self.add_reaction(reaction=reaction)
+                        reaction.id = reaction.base_id
+                        new_compartments = {
+                            self.compounds[i].compartment
+                            for i in reaction.stoichiometries
+                        }
+                        reaction.compartment = tuple(sorted(new_compartments))
+                        if len(reaction.compartment) > 1:
+                            reaction.transmembrane = True
+                        else:
+                            reaction.transmembrane = False
+                        for compartment_id in reaction.compartment:
+                            reaction.id += self._add_compartment_suffix(
+                                object_id="", compartment_id=compartment_id
+                            )
+                        self.add_reaction(reaction=reaction)
 
-    def _repair_photosynthesis_reactions(self) -> None:
+    def _repair_photosynthesis_reactions(self):
         """Switch the photosynthesis reactions proton compartments.
 
-        The way the photosynthesis reactions are currently annotated and parsed,
+        The way the photosynthesis reactions are currenlty annotated and parsed,
         they will transport protons out of the periplasm, while they are
         actually doing the opposite.
         """
         try:
-            for reaction_id in list(self.pathways["PWY-101"]):
-                reaction = copy.deepcopy(self.reactions[reaction_id])
+            for reaction_id in self.pathways["PWY-101"]:
+                reaction = self.reactions[reaction_id]
                 if reaction.transmembrane:
-                    self.remove_reaction(reaction_id, remove_empty_references=False)
                     st = reaction.stoichiometries
-                    in_compartment, out_compartment = cast(Tuple[str, str], reaction.compartment)
+                    in_compartment, out_compartment = reaction.compartment
                     in_proton_name = self._add_compartment_suffix(
                         object_id="PROTON", compartment_id=in_compartment
                     )
                     out_proton_name = self._add_compartment_suffix(
                         object_id="PROTON", compartment_id=out_compartment
                     )
                     try:
@@ -421,96 +307,91 @@
                         in_error = True
                     try:
                         out_protons = st.pop(out_proton_name)
                         out_error = False
                     except KeyError:
                         out_error = True
                     if not in_error:
-                        st[out_proton_name] = in_protons  # type: ignore
+                        st[out_proton_name] = in_protons
                     if not out_error:
-                        st[in_proton_name] = out_protons  # type: ignore
-                    self._move_reaction_to_other_compartment(reaction)
+                        st[in_proton_name] = out_protons
         except KeyError:
             pass
 
     def read_from_pgdb(
         self,
-        pgdb_path: Union[str, Path],
-        move_electron_transport_cofactors_to_cytosol: bool = True,
-        repair_photosynthesis_reactions: bool = True,
-        fix_periplasm_proton_gradient: bool = True,
-        fix_light_reaction_mass_balance: bool = True,
-        remove_unused_compounds: bool = True,
-        compartment_map: Dict[str, str] | None = None,
-        compartment_suffixes: Dict[str, str] | None = None,
-        type_map: Dict[str, str] | None = None,
-    ) -> None:
-        if not (path := Path(pgdb_path)).exists():
-            raise FileNotFoundError(f"Could not find metacyc at path {str(path)}")
-        parse_results = cycparser.parse_and_repair_pgdb(
-            path,
-            compartment_map=compartment_map,
-            type_map=type_map,
-            manual_additions=None,
-            compartment_suffixes=compartment_suffixes,
-        )
-        parse_compounds = parse_results.compounds
-        parse_reactions = parse_results.reactions
-        parse_compartments = parse_results.compartments
-        parse_gpr_annotations = parse_results.gpr_annotations
-        parse_kinetic_data = parse_results.kinetic_data
-        parse_monomers = parse_results.monomers
-
-        moped_kinetic_data = {
-            k: {k2: KineticData(v2.km, v2.kcat, v2.vmax)}
-            for k, v in parse_kinetic_data.items()
-            for k2, v2 in v.items()
-        }
+        pgdb_path,
+        parse_sequences=True,
+        apply_fba_fixes={
+            "move_electron_transport_cofactors_to_cytosol": True,
+            "repair_photosynthesis_reactions": True,
+            "fix_periplasm_proton_gradient": True,
+        },
+        compartment_map={
+            "CYTOSOL": "CYTOSOL",
+            "IN": "CYTOSOL",
+            "UNKNOWN-SPACE": "CYTOSOL",
+            "SIDE-1": "CYTOSOL",
+            "SIDE-2": "EXTRACELLULAR",
+            "EXTRACELLULAR": "EXTRACELLULAR",
+            "CHL-THY-MEM": "PERIPLASM",
+            "CHLOR-STR": "CYTOSOL",
+            "CHROM-STR": "CYTOSOL",
+            "GOLGI-LUM": "CYTOSOL",
+            "LYS-LUM": "CYTOSOL",
+            "MIT-IM-SPC": "CYTOSOL",
+            "MIT-IMEM": "PERIPLASM",
+            "MIT-LUM": "CYTOSOL",
+            "OUTER-MEM": "PERIPLASM",
+            "PERI-BAC": "PERIPLASM",
+            "PERI-BAC-GN": "PERIPLASM",
+            "PERIPLASM": "PERIPLASM",
+            "PEROX-LUM": "CYTOSOL",
+            "PLASMA-MEM": "PERIPLASM",
+            "PLAST-IMEM": "PERIPLASM",
+            "PLASTID-STR": "PERIPLASM",
+            "PM-ANIMAL": "PERIPLASM",
+            "PM-BAC-ACT": "PERIPLASM",
+            "PM-BAC-NEG": "PERIPLASM",
+            "PM-BAC-POS": "PERIPLASM",
+            "RGH-ER-LUM": "CYTOSOL",
+            "RGH-ER-MEM": "PERIPLASM",
+            "THY-LUM-CYA": "CYTOSOL",
+            "VAC-LUM": "CYTOSOL",
+            "VAC-MEM": "PERIPLASM",
+            "VESICLE": "PERIPLASM",
+            "OUT": "PERIPLASM",
+        },
+        remove_unused_compounds=True,
+    ):
+        """Parse the model from a given pdgb, e.g. MetaCyc.
 
-        moped_compounds = [
-            Compound(
-                base_id=v.base_id,
-                compartment=v.compartment,
-                formula=v.formula,
-                charge=v.charge,
-                name=v.name,
-                gibbs0=v.gibbs0,
-                smiles=v.smiles,
-                database_links=v.database_links,
-                types=v.types,
-                id=v.id,
-            )
-            for v in parse_compounds.values()
-        ]
-        moped_reactions = [
-            Reaction(
-                base_id=v.base_id,
-                id=v.id,
-                stoichiometries=v.stoichiometries,
-                compartment=v.compartment,
-                name=v.name,
-                bounds=v.bounds,
-                gibbs0=v.gibbs0,
-                ec=v.ec,
-                types=v.types,
-                pathways=v.pathways,
-                database_links=v.database_links,
-                transmembrane=v.transmembrane,
-                kinetic_data=moped_kinetic_data.get(v.base_id, {}),
-                gpr_annotation=parse_gpr_annotations.get(v.base_id, []),
-                _var=v._var,
-            )
-            for v in parse_reactions.values()
-        ]
-        moped_monomers = {
-            k: Monomer(id=k, sequence=v.sequence, database_links=v.database_links)
-            for k, v in parse_monomers.items()
-        }
-        self.compartments = parse_compartments
-        self.add_compounds(moped_compounds)
+        Parameters
+        ----------
+        pgdb_path: str or pathlib.Path
+            This is expected to lead to the data directory of the pgdb
+            so e.g. metacyc/23.0/data
+        parse_sequences: bool
+            Whether to parse the protein sequences of the model.
+            If they are not needed, set this to false to make the parsing
+            faster.
+        apply_fba-fixes: dict(str: bool)
+            Whether to apply certain common fixes after parsing
+        compartment_map: dict(str: str)
+
+        """
+        pgdb_path = pathlib.Path(pgdb_path)
+        compounds, reactions, compartments = Cyc(
+            pgdb_path=pgdb_path,
+            parse_sequences=parse_sequences,
+            compartment_map=compartment_map,
+        ).parse()
+        self.compartments = compartments
+        self.add_compounds(compounds=compounds)
+        self.add_reactions(reactions=reactions)
 
         for strong_cofactor_base_id, weak_cofactor_base_id in {
             "ATP": "ADP",
             "GTP": "GDP",
             "NADH": "NAD",
             "NADPH": "NADP",
             "10-FORMYL-THF": "THF",
@@ -527,16 +408,14 @@
             "CPD-12829": "PLASTOQUINONE-9",
         }.items():
             self.add_cofactor_pair(
                 strong_cofactor_base_id=strong_cofactor_base_id,
                 weak_cofactor_base_id=weak_cofactor_base_id,
             )
 
-        self.add_reactions(moped_reactions)
-
         self.add_minimal_seed(
             compound_ids={
                 "WATER_c",
                 "PROTON_c",
                 "OXYGEN-MOLECULE_c",
                 "CARBON-DIOXIDE_c",
                 "Pi_c",
@@ -544,132 +423,102 @@
                 "ZN+2_c",
                 "CU+2_c",
                 "CA+2_c",
                 "SULFATE_c",
                 "AMMONIA_c",
             }
         )
-
-        # self.add_gpr_annotations(parse_gpr_annotations)
-        # self.add_kinetic_data(moped_kinetic_data)
-        self.add_monomers(moped_monomers)
-
-        if move_electron_transport_cofactors_to_cytosol:
+        if apply_fba_fixes["move_electron_transport_cofactors_to_cytosol"]:
             self._move_electron_transport_cofactors_to_cytosol()
 
-        if repair_photosynthesis_reactions:
+        if apply_fba_fixes["repair_photosynthesis_reactions"]:
             self._repair_photosynthesis_reactions()
 
-        if fix_periplasm_proton_gradient:
+        if apply_fba_fixes["fix_periplasm_proton_gradient"]:
             self._fix_periplasm_proton_gradient()
 
         if remove_unused_compounds:
             self.remove_unused_compounds()
 
-        if fix_light_reaction_mass_balance:
-            self._fix_light_reaction_mass_balance()
+    def read_from_cobra(self, cobra_model):
+        """Import a cobra model into this model.
 
-    def _read_cobra_annotation(self, annotations: dict[str, str | list[str]]) -> dict[str, set[str]]:
-        if "sbo" in annotations:
-            annotations.pop("sbo")
-        return {k: set(v) if isinstance(v, list) else set([v]) for k, v in annotations.items()}
+        Parameters
+        ----------
+        cobra_model: cobra.Model
+            Mapping of model compartments to moped compartments
+        """
+        compartment_map = cobra_model.compartments
+        self.compartments.update({v: k for k, v in compartment_map.items()})
+        compartment_suffixes = re.compile(
+            "|".join(set([f"(_{i}$)" for i in compartment_map.keys()]))
+        )
 
-    def _read_cobra_compounds(
-        self,
-        cobra_model: cobra.Model,
-        compartment_map: dict[str, str],
-        compartment_suffixes: re.Pattern,
-    ) -> None:
+        objective = {}
         for metabolite in cobra_model.metabolites:
             base_id = self._strip_compartment_suffix(
-                object_id=metabolite.id,
-                compartment_pattern=compartment_suffixes,
+                object_id=metabolite.id, compartment_pattern=compartment_suffixes
             )
-            compartment = compartment_map[metabolite.compartment]
-            database_links = self._read_cobra_annotation(metabolite.annotation)
+            try:
+                compartment = compartment_map[metabolite.compartment]
+            except KeyError:
+                raise KeyError(
+                    f"Compartment {metabolite.compartment} missing in compartment map."
+                )
             self.add_compound(
                 Compound(
                     base_id=base_id,
-                    compartment=compartment,
                     id=metabolite.id,
+                    name=metabolite.name,
+                    compartment=compartment,
                     formula=metabolite.elements,
                     charge=metabolite.charge,
-                    name=metabolite.name,
                     gibbs0=None,
-                    smiles=None,
-                    database_links=database_links,
-                    types=list(),
-                    in_reaction=set(),
+                    types=None,
                 )
             )
-
-    def _read_cobra_rxn_genes(self, rxn: cobra.Reaction) -> dict[str, Monomer]:
-        monomers = {}
-        for gene in rxn.genes:
-            database_links = self._read_cobra_annotation(gene.annotation)
-            gene_id = cast(str, gene.id)
-            monomers[gene_id] = Monomer(id=gene_id, sequence=None, database_links=database_links)
-        return monomers
-
-    def _read_cobra_rxn_gpr_annotation(self, rxn: cobra.Reaction) -> list[set[str]]:
-        return [set(rxn.gene_reaction_rule.split(" and"))]
-
-    def _read_cobra_reactions_and_objective(
-        self,
-        cobra_model: cobra.Model,
-        compartment_map: dict[str, str],
-        compartment_suffixes: re.Pattern,
-    ) -> None:
-        objective = {}
         for reaction in cobra_model.reactions:
             obj_coef = reaction.objective_coefficient
             if obj_coef != 0:
                 objective[reaction.id] = obj_coef
 
-            compartment: Union[str, Tuple[str, ...]]
-            if len(reaction.compartments) == 1:
-                compartment = compartment_map[next(iter(reaction.compartments))]
-            else:
-                compartment = tuple(compartment_map[i] for i in reaction.compartments)
-            database_links = self._read_cobra_annotation(reaction.annotation)
-            self.add_monomers(self._read_cobra_rxn_genes(reaction))
-            gpr_annotation = self._read_cobra_rxn_gpr_annotation(reaction)
             self.add_reaction(
                 Reaction(
+                    base_id=self._strip_compartment_suffix(
+                        object_id=reaction.id, compartment_pattern=compartment_suffixes
+                    ),
                     id=reaction.id,
-                    compartment=compartment,
                     stoichiometries={k.id: v for k, v in reaction.metabolites.items()},
                     bounds=reaction.bounds,
-                    database_links=database_links,
-                    name=reaction.name if len(reaction.name) > 0 else None,
-                    base_id=self._strip_compartment_suffix(
-                        object_id=reaction.id,
-                        compartment_pattern=compartment_suffixes,
-                    ),
-                    gpr_annotation=gpr_annotation,
-                    _gpa=0 if len(gpr_annotation) > 0 else None,
+                    reversible=reaction.reversibility,
+                    gibbs0=None,
+                    ec=None,
+                    pathways=None,
+                    name=reaction.name,
                 )
             )
         self.set_objective(objective=objective)
 
-    def read_from_cobra(self, cobra_model: cobra.Model) -> None:
-        """Import a cobra model into this model."""
-        compartment_map = cobra_model.compartments
-        self.compartments.update({v: k for k, v in compartment_map.items()})
-        compartment_suffixes = re.compile("|".join(set([f"(_{i}$)" for i in compartment_map.keys()])))
-        self._read_cobra_compounds(cobra_model, compartment_map, compartment_suffixes)
-        self._read_cobra_reactions_and_objective(cobra_model, compartment_map, compartment_suffixes)
-
-    def read_from_sbml(self, sbml_file: Union[str, Path]) -> None:
-        """Import an sbml model into this model."""
-        cobra_model = cobra.io.read_sbml_model(filename=str(sbml_file))
+    def read_from_sbml(self, sbml_file):
+        """Import an sbml model into this model.
+
+        Parameters
+        ----------
+        sbml_file: str or pathlib.Path
+        """
+        cobra_model = cobra.io.read_sbml_model(filename=sbml_file)
         self.read_from_cobra(cobra_model=cobra_model)
 
-    def read_from_bigg(self, bigg_sbml_file: Union[str, Path]) -> None:
-        """Import a bigg sbml model into this model."""
+    def read_from_bigg(self, bigg_sbml_file):
+        """Import a bigg sbml model into this model.
+
+        Parameters
+        ----------
+        bigg_sbml_file: str or pathlib.Path
+        """
         self.read_from_sbml(sbml_file=bigg_sbml_file)
 
         for strong_cofactor_base_id, weak_cofactor_base_id in {
             "atp": "adp",
             "gtp": "gdp",
             "nadh": "nad",
             "nadph": "nadp",
@@ -686,137 +535,153 @@
                 weak_cofactor_base_id=weak_cofactor_base_id,
             )
 
     ##########################################################################
     # Universal functions
     ##########################################################################
 
-    def create_submodel(self, reaction_ids: Iterable[str], name: str | None = None) -> "Model":
-        """Create a subset of the model, containing the given reactions and their compounds."""
+    def create_submodel(self, reaction_ids, name=None):
+        """Create a subset of the model, containing the given reactions and their compounds.
+
+        Parameters
+        ----------
+        reactions: Iterable(str)
+            Iterable of reaction_ids
+
+        Returns
+        -------
+        submodel: moped.Model
+        """
         reactions = [self.reactions[i] for i in sorted(reaction_ids)]
         compounds = set()
         for rec in reactions:
-            for cpd_name in rec.stoichiometries:
-                cpd = copy.deepcopy(self.compounds[cpd_name])
+            for cpd in rec.stoichiometries:
+                cpd = self.compounds[cpd].copy()
                 cpd.in_reaction = set()
                 compounds.add(cpd)
         if name is None:
             name = self.name + " submodel"
 
         submodel = Model(
             compounds=compounds,
             reactions=reactions,
             name=name,
-            compartments=self.compartments.copy(),
-            objective=self.objective.copy(),
-            minimal_seed=self.minimal_seed.copy(),
-        )
-
-        # submodel.cofactor_pairs = self.cofactor_pairs.copy()
-        # This is wrong, submodel must not necessarily have the same cofactor pairs
-
-        # Collect base cofactor pairs
-        base_cofactor_pairs = {}
-        for strong, weak in self.cofactor_pairs.items():
-            strong_base_cpd = self.compounds[strong].base_id
-            weak_base_cpd = self.compounds[weak].base_id
-            base_cofactor_pairs[strong_base_cpd] = weak_base_cpd
-
-        # Only add cofactor pairs to submodel that actually exist in there
-        for strong, weak in base_cofactor_pairs.items():
-            submodel.add_cofactor_pair(
-                strong_cofactor_base_id=strong,
-                weak_cofactor_base_id=weak,
-            )
-
-        # Only export monomers that are actually used
-        monomers = {}
-        for reaction in self.reactions.values():
-            for enzyme in reaction.gpr_annotation:
-                for monomer in enzyme:
-                    if monomer in self.monomers:
-                        monomers[monomer] = self.monomers[monomer]
-        submodel.monomers = monomers
+            compartments=self.compartments,
+        )
+        submodel.cofactor_pairs = self.cofactor_pairs.copy()
         return submodel
 
-    def add_cofactor_pair(self, strong_cofactor_base_id: str, weak_cofactor_base_id: str) -> None:
+    def add_cofactor_pair(self, strong_cofactor_base_id, weak_cofactor_base_id):
         """Add a cofactor pair.
 
-        This automatically adds all compartment variants of the given base ids.
+        E.g. ATP as a strong cofactor and ADP as its weak pair.
 
-        Examples
-        --------
-        >>> model.add_cofactor_pair("ATP", "ADP")
+        Parameters
+        ----------
+        strong_cofactor: str
+        weak_cofactor: str
         """
         try:
-            self._base_cofactor_pairs[strong_cofactor_base_id] = weak_cofactor_base_id
             for strong_cpd_id in self.base_compounds[strong_cofactor_base_id]:
                 for weak_cpd_id in self.base_compounds[weak_cofactor_base_id]:
-                    if self.compounds[strong_cpd_id].compartment == self.compounds[weak_cpd_id].compartment:
+                    if (
+                        self.compounds[strong_cpd_id].compartment
+                        == self.compounds[weak_cpd_id].compartment
+                    ):
                         self.cofactor_pairs[strong_cpd_id] = weak_cpd_id
         except KeyError:
             pass
 
-    def get_weak_cofactors(self) -> List[str]:
-        """Get ids of weak cofactors."""
+    def get_weak_cofactors(self):
+        """Get ids of weak cofactors.
+
+        Returns
+        -------
+        cofactors: list(str)
+            List of cofactor ids
+        """
         return list(set([i for i in self.cofactor_pairs.values()]))
 
-    def get_weak_cofactor_duplications(self) -> List[str]:
+    def get_weak_cofactor_duplications(self):
         """Get ids of weak cofactors including the __cof__ tag.
 
         This function is useful for structural analyses, in which these
         tagged cofactors are used.
+
+        Returns
+        -------
+        cofactors: list(str)
+            List of cofactor ids
         """
         return list(set([i + "__cof__" for i in self.cofactor_pairs.values()]))
 
-    def get_strong_cofactors(self) -> List[str]:
-        """Get ids of strong cofactors."""
+    def get_strong_cofactors(self):
+        """Get ids of strong cofactors.
+
+        Returns
+        -------
+        cofactors: list(str)
+            List of cofactor ids
+        """
         return list(set([i for i in self.cofactor_pairs.keys()]))
 
-    def get_strong_cofactor_duplications(self) -> List[str]:
+    def get_strong_cofactor_duplications(self):
         """Get ids of strong cofactors including the __cof__ tag.
 
         This function is useful for structural analyses, in which these
-        tagged cofactors are used."""
+        tagged cofactors are used.
+
+        Returns
+        -------
+        cofactors: list(str)
+            List of cofactor ids
+        """
         return list(set([i + "__cof__" for i in self.cofactor_pairs.keys()]))
 
-    def update_from_reference(
-        self, reference_model: "Model", verbose: bool = False
-    ) -> Tuple[List[str], Set[str]]:
+    def update_from_reference(self, reference_model, verbose=False):
         """Update a model from a reference Model.
 
+        Parameters
+        ----------
+        reference_model: moped.Model
+        verbose: bool, optional
+
         Returns
         -------
-        unmapped_reactions
-            Reactions that could not be found in the reference database
-        unmapped_compounds
-            Compounds that could not be found in the reference database
+        unmapped_reactions: list(str)
+            List of reactions that could not be found in the reference database
+        unmapped_compounds: list(str)
+            List of compounds that could not be found in the reference database
         """
         mapped_compounds = set(self.compounds).intersection(reference_model.compounds)
         unmapped_compounds = set(self.compounds).difference(reference_model.compounds)
 
         old_base_reactions = set(self.base_reactions)
         old_variant_reactions = set(self.variant_reactions)
 
         new_base_reactions = set(reference_model.base_reactions)
         new_variant_reactions = set(reference_model.variant_reactions)
 
         unmapped_base_reactions = [
-            j for i in old_base_reactions.difference(new_base_reactions) for j in self.base_reactions[i]
+            j
+            for i in old_base_reactions.difference(new_base_reactions)
+            for j in self.base_reactions[i]
         ]
         unmapped_variant_reactions = [
             j
             for i in old_variant_reactions.difference(new_variant_reactions)
             for j in self.variant_reactions[i]
         ]
         unmapped_reactions = unmapped_base_reactions + unmapped_variant_reactions
 
         # Update all existing compounds
         for compound_id in mapped_compounds:
-            self.add_compound_from_reference(reference_model=reference_model, compound_id=compound_id)
+            self.add_compound_from_reference(
+                reference_model=reference_model, compound_id=compound_id
+            )
 
         # Update all existing base reactions
         for base_reaction_id in old_base_reactions.intersection(
             new_base_reactions
         ) | old_variant_reactions.intersection(new_variant_reactions):
             self.add_reaction_from_reference(
                 reference_model=reference_model,
@@ -831,247 +696,441 @@
             if not self.check_mass_balance(reaction_id=reaction_id):
                 self.remove_reaction(reaction_id=reaction_id)
                 continue
             if not self.check_charge_balance(reaction_id=reaction_id):
                 self.remove_reaction(reaction_id=reaction_id)
         if verbose:
             print(
-                f"Could not map {len(unmapped_base_reactions) + len(unmapped_variant_reactions)} reactions "
-                + f"and {len(unmapped_compounds)} compounds"
+                f"Could not map {len(unmapped_base_reactions) + len(unmapped_variant_reactions)} reactions and {len(unmapped_compounds)} compounds"
             )
-        return unmapped_reactions, unmapped_compounds
+            return unmapped_reactions, unmapped_compounds
 
     ##########################################################################
     # Compound functions
     ##########################################################################
 
-    def add_compound(self, compound: Compound) -> None:
-        """Add a compound to the model. Overwrites existing compounds."""
+    def add_compound(self, compound):
+        """Add a compound to the model. Overwrites existing compounds.
+
+        Parameters
+        ----------
+        compound: moped.Compound
+            The compound object
+
+        Raises
+        ------
+        TypeError
+            If compound is not of type moped.Compound
+        """
         if isinstance(compound, Compound):
             if not bool(compound.id):
                 compound.id = self._add_compartment_suffix(
-                    object_id=compound.base_id,
-                    compartment_id=cast(str, compound.compartment),
+                    object_id=compound.base_id, compartment_id=compound.compartment
                 )
-            cpd_id = cast(str, compound.id)
-            self.compounds[cpd_id] = copy.deepcopy(compound)
-            self.base_compounds.setdefault(compound.base_id, set()).add(cpd_id)
+            self.compounds[compound.id] = compound.copy()
+            self.base_compounds.setdefault(compound.base_id, set()).add(compound.id)
             for compound_type in compound.types:
-                self._compound_types.setdefault(compound_type, set()).add(cpd_id)
+                self._compound_types.setdefault(compound_type, set()).add(compound.id)
         else:
             raise TypeError("Compound has to be of type moped.model.Compound")
 
-    def add_compounds(self, compounds: Iterable[Compound]) -> None:
-        """Add multiple compounds to the model. Overwrites existing compounds."""
+    def add_compounds(self, compounds):
+        """Add multiple compounds to the model. Overwrites existing compounds.
+
+        Parameters
+        ----------
+        compounds: iterable(moped.Compound)
+            The compound objects
+
+        Raises
+        ------
+        TypeError
+            If compound is not of type moped.Compound
+        """
         for compound in compounds:
             self.add_compound(compound=compound)
 
-    def add_compound_from_reference(self, reference_model: "Model", compound_id: str) -> None:
-        """Overwrite local data from reference database or adds new one if it does not exist already."""
-        new_cpd = copy.deepcopy(reference_model.compounds[compound_id])
+    def add_compound_from_reference(self, reference_model, compound_id):
+        """Overwrite local data from reference database or adds new one if it does not exist already.
+
+        Parameters
+        ----------
+        reference_model: moped.Model
+        compound_id: str
+        """
+        new_cpd = reference_model.compounds[compound_id].copy()
         try:
             old_cpd = self.compounds.pop(compound_id)
             new_cpd.in_reaction = old_cpd.in_reaction
         except KeyError:
             new_cpd.in_reaction = set()
         self.compounds[compound_id] = new_cpd
 
-    def _create_compartment_variant(self, old_compound: Compound, compartment_id: str) -> Compound:
+    def _create_compartment_variant(self, old_compound, compartment_id):
         """Create a variant of the compound in another compartment.
 
         This empties the in_reaction set, as the compound is only known
         to be part of the reactions in the previous compartment and
         we cannot know whether those reactions are also available
         in the new compartment.
+
+        Parametersy
+        ----------
+        compartment: str
+            Name of the new compartment. Must be in utils.COMPARTMENT_SUFFIXES
+
+        Returns
+        -------
+        new_cpd: Compound
         """
-        new_compound = copy.deepcopy(old_compound)
+        new_compound = old_compound.copy()
         new_compound.id = self._add_compartment_suffix(
             object_id=old_compound.base_id, compartment_id=compartment_id
         )
         new_compound.compartment = compartment_id
         new_compound.in_reaction = set()
         self.add_compound(compound=new_compound)
         return new_compound
 
-    def add_compartment_compound_variant(self, compound_id: str, compartment_id: str) -> Compound:
-        """Add a copy of the compound in the respective compartment."""
+    def add_compartment_compound_variant(self, compound_id, compartment_id):
+        """Add a copy of the compound in the respective compartment.
+
+        Clears the in_reaction attribute. The compartments are named
+        according to the metacyc database
+
+        Parameters
+        ----------
+        compound_id: str
+        compartment: str
+
+        Raises
+        ------
+        TypeError
+            If compound_id is not a string
+        KeyError
+            If compound is not in the model
+        KeyError
+            If the compartment does not exist
+
+        Returns
+        -------
+        compartment_compound: moped.Compound
+        """
         try:
             old_compound = self.compounds[compound_id]
         except KeyError:
             try:
                 compound_variants = self.base_compounds[compound_id]
                 old_compound = self.compounds[next(iter(compound_variants))]
             except KeyError:
-                raise KeyError(f"Compound {compound_id} has to be in the model to create an external variant")
+                raise KeyError(
+                    f"Compound {compound_id} has to be in the model to create an external variant"
+                )
         new_compound_id = self._add_compartment_suffix(
             object_id=old_compound.base_id, compartment_id=compartment_id
         )
         try:
             new_compound = self.compounds[new_compound_id]
         except KeyError:
             new_compound = self._create_compartment_variant(
                 old_compound=old_compound, compartment_id=compartment_id
             )
         return new_compound
 
-    def set_compound_property(self, compound_id: str, property_dict: Dict[str, Any]) -> None:
-        """Set one or multiple properties of a compound."""
+    def set_compound_property(self, compound_id, property_dict):
+        """Set one or multiple properties of a compound.
+
+        Parameters
+        ----------
+        compound_id: str
+        property_dict: dict
+
+        Raises
+        ------
+        KeyError
+            If Compound does not have an attribute specified in property_dict
+        """
         for k, v in property_dict.items():
-            cpd = self.compounds[compound_id]
-            slots = dataclasses.asdict(cpd).keys()
-            if k not in slots:
-                raise KeyError(f"Compound does not have key '{k}', can only be one of {slots}")
-            setattr(cpd, k, v)
+            try:
+                setattr(self.compounds[compound_id], k, v)
+            except AttributeError:
+                raise KeyError(
+                    f"Compound does not have key '{k}', can only be one of {Compound.__slots__}"
+                )
+
+    def remove_compound(self, compound_id):
+        """Remove a compound from the model.
 
-    def remove_compound(self, compound_id: str) -> None:
-        """Remove a compound from the model."""
+        Parameters
+        ----------
+        compound_id: str
+        """
         compound = self.compounds.pop(compound_id)
 
         # Also remove from base compounds
-        self.base_compounds[compound.base_id].remove(compound_id)
+        self.base_compounds[compound.base_id].remove(compound.id)
         if not bool(self.base_compounds[compound.base_id]):
             del self.base_compounds[compound.base_id]
 
         # Also remove from compound types
         for compound_type in compound.types:
-            self._compound_types[compound_type].remove(compound_id)
+            self._compound_types[compound_type].remove(compound.id)
             if not bool(self._compound_types[compound_type]):
                 del self._compound_types[compound_type]
 
-        if compound_id in self.cofactor_pairs:
-            del self.cofactor_pairs[compound_id]
-        elif compound_id in self.get_weak_cofactors():
-            weak_cofactors = self.get_weak_cofactors()
-            strong_cofactors = self.get_strong_cofactors()
-            weak_to_strong = dict(zip(weak_cofactors, strong_cofactors))
-            del self.cofactor_pairs[weak_to_strong[compound_id]]
+    def remove_compounds(self, compound_ids):
+        """Remove multiple compounds from the model.
 
-    def remove_compounds(self, compound_ids: Iterable[str]) -> None:
-        """Remove multiple compounds from the model."""
+        Parameters
+        ----------
+        compound_ids: iterable(str)
+        """
         for compound_id in compound_ids:
             self.remove_compound(compound_id=compound_id)
 
-    def remove_unused_compounds(self) -> None:
+    def remove_unused_compounds(self):
         """Remove compounds from the model that are in no reaction."""
         all_compounds = set(self.compounds)
         used_compounds = set()
         for reaction in self.reactions.values():
             used_compounds.update(set(reaction.stoichiometries))
         unused = all_compounds.difference(used_compounds)
         self.remove_compounds(compound_ids=unused)
 
-    def get_compound_base_id(self, compound_id: str) -> str:
-        """Get the database links of a given compound."""
+    def get_compound_base_id(self, compound_id):
+        """Get the database links for a given compound.
+
+        Parameters
+        ----------
+        compound_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.compounds[compound_id].base_id
 
-    def get_compound_compartment_variants(self, compound_base_id: str) -> Set[str]:
+    def get_compound_compartment_variants(self, compound_base_id):
         """Get compound ids for all respective compartments the compound is in.
 
         The compound_base_id for ATP_c for example would be ATP.
+
+        Parameters
+        ----------
+        compound_base_id : str
+
+        Returns
+        -------
+        compound_ids : set
         """
         return self.base_compounds[compound_base_id]
 
-    def get_compound_compartment(self, compound_id: str) -> str | None:
-        """Get compartment of a given compound compound."""
+    def get_compound_compartment(self, compound_id):
+        """Get the database links for a given compound.
+
+        Parameters
+        ----------
+        compound_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.compounds[compound_id].compartment
 
-    def get_compound_formula(self, compound_id: str) -> Dict[str, float] | None:
-        """Get the charge of a given compound."""
+    def get_compound_formula(self, compound_id):
+        """Get the database links for a given compound.
+
+        Parameters
+        ----------
+        compound_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.compounds[compound_id].formula
 
-    def get_compound_charge(self, compound_id: str) -> float | None:
-        """Get the charge of a given compound."""
+    def get_compound_charge(self, compound_id):
+        """Get the database links for a given compound.
+
+        Parameters
+        ----------
+        compound_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.compounds[compound_id].charge
 
-    def get_compound_gibbs0(self, compound_id: str) -> float | None:
-        """Get the gibbs energy (free enthalpy) of the given compound."""
-        return self.compounds[compound_id].gibbs0
+    def get_reactions_of_compound(self, compound_id):
+        """Get all reactions of a compound.
 
-    def get_reactions_of_compound(self, compound_id: str) -> Set[str]:
-        """Get all reactions of a compound."""
+        Parameters
+        ----------
+        compound_id: str
+
+        Returns
+        -------
+        in_reaction: set(str)
+            Set of reaction ids of which the compound is part
+        """
         return self.compounds[compound_id].in_reaction
 
-    def get_compound_database_links(self, compound_id: str) -> Dict[str, Set[str]]:
-        """Get the database links of a given compound."""
+    def get_compound_database_links(self, compound_id):
+        """Get the database links for a given compound.
+
+        Parameters
+        ----------
+        compound_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.compounds[compound_id].database_links
 
-    def get_base_compound_ids(self) -> Set[str]:
-        """Get base IDs of all compounds."""
+    def get_base_compound_ids(self):
+        """Get base IDs of all compounds.
+
+        Returns
+        -------
+        base_compound_ids: set
+        """
         return set(i.base_id for i in self.compounds.values())
 
-    def get_compound_type_ids(self) -> Set[str]:
-        """Get all available compound types."""
+    def get_compound_type_ids(self):
+        """Get all available reaction types."""
         return set(self._compound_types)
 
-    def get_model_compartment_ids(self) -> Set[str]:
-        """Get all ids for compartments used in the model."""
+    def get_model_compartment_ids(self):
+        """Get all ids for compartments used in the model.
+
+        Returns
+        -------
+        compartment_ids : set
+        """
         return set(self.compartments)
 
-    def get_compounds_of_compartment(self, compartment_id: str) -> List[str]:
+    def get_compounds_of_compartment(self, compartment_id):
         """Get all compounds from the respective compartment.
 
         To look up the available compartments, see model.get_model_compartment_ids
 
+        Parameters
+        ----------
+        compartment: str
+
+        Returns
+        -------
+        compounds_of_compartment: list(str)
+
         See Also
         --------
         model.get_model_compartment_ids
             To get all available compartments
         """
         if compartment_id not in self.get_model_compartment_ids():
-            raise KeyError(
+            raise ValueError(
                 f"Unknown compartment {compartment_id}, did you mean any of {self.get_model_compartment_ids()}?"
             )
         return [k for k, v in self.compounds.items() if v.compartment == compartment_id]
 
-    def get_compounds_of_type(self, compound_type: str) -> Set[str]:
-        """Get all compound ids of a given compound_type."""
+    def get_compounds_of_type(self, compound_type):
+        """Get all compound ids of a given compound_type.
+
+        Parameters
+        ----------
+        compound_type : str
+
+        Returns
+        -------
+        compound_type : set
+        """
         return self._compound_types[compound_type]
 
     ##########################################################################
     # Reaction functions
     ##########################################################################
 
-    def add_reaction(self, reaction: Reaction) -> None:
-        """Add a reaction to the model."""
+    def add_reaction(self, reaction):
+        """Add a reaction to the model.
+
+        Also adds this reaction to each compounds in-reaction attribute,
+        pathways and monomers
+
+        Parameters
+        ----------
+        reaction: moped.Reaction
+
+        Raises
+        ------
+        KeyError
+            If any of the reaction compounds is not in the model
+        TypeError
+            If reaction is not of type moped.Reaction
+        """
         if not isinstance(reaction, Reaction):
             raise TypeError("Reaction has to be of type moped.model.Reaction")
         reaction_id = reaction.id
-        if reaction._var is not None:
-            self.variant_reactions.setdefault(cast(str, reaction.base_id), set()).add(reaction_id)
+        if "__var__" in reaction.id:
+            self.variant_reactions.setdefault(reaction.base_id, set()).add(reaction_id)
         else:
-            self.base_reactions.setdefault(cast(str, reaction.base_id), set()).add(reaction_id)
-        self.reactions[reaction_id] = copy.deepcopy(reaction)
+            self.base_reactions.setdefault(reaction.base_id, set()).add(reaction_id)
+        self.reactions[reaction_id] = reaction.copy()
         for compound in reaction.stoichiometries:
             self.compounds[compound].in_reaction.add(reaction_id)
         for type_ in reaction.types:
             self._reaction_types.setdefault(type_, set()).add(reaction.id)
         for pathway in reaction.pathways:
             self.add_reaction_to_pathway(pathway_id=pathway, reaction_id=reaction_id)
+        for monomer in reaction.sequences:
+            self._monomers.setdefault(monomer, set()).add(reaction.id)
+
+    def add_reactions(self, reactions):
+        """Add multiple reactions to the model.
+
+        Parameters
+        ----------
+        reactions: iterable(moped.Reaction)
 
-    def add_reactions(self, reactions: Iterable[Reaction]) -> None:
-        """Add multiple reactions to the model."""
+        Raises
+        ------
+        KeyError
+            If any of the reaction compounds is not in the model
+        TypeError
+            If reaction is not of type moped.Reaction
+        """
         for reaction in reactions:
             self.add_reaction(reaction=reaction)
 
     def add_reaction_from_reference(
-        self,
-        reference_model: "Model",
-        reaction_id: str,
-        update_compounds: bool = True,
-    ) -> None:
+        self, reference_model, reaction_id, update_compounds=True
+    ):
         """Add a reaction from a reference model.
 
         Always adds reversibiliy and cofactor duplicates as well. In this case all
         existing reaction variants are kept if they are not overwritten.
         Adds all variants of a reaction if the base_id of a variant reaction is given.
         In this case all other existing reaction variants are removed.
+
+        Parameters
+        ----------
+        reference_model: moped.model
+        reaction_id: str
+
+        Raises
+        ------
+        KeyError
+            If reaction_id cannot be found in the reference
         """
         try:
             reaction = self.reactions[reaction_id]
-            base_id = cast(str, reaction.base_id)
+            base_id = reaction.base_id
         except KeyError:
             base_id = reaction_id
         if base_id in reference_model.variant_reactions:
             try:
                 for reaction_id in tuple(self.variant_reactions[base_id]):
                     self.remove_reaction(reaction_id)
             except KeyError:
@@ -1079,15 +1138,17 @@
             new_reactions = [
                 reference_model.reactions[reaction_id]
                 for reaction_id in reference_model.variant_reactions[base_id]
             ]
             if update_compounds:
                 new_compound_ids = {j for i in new_reactions for j in i.stoichiometries}
                 for compound_id in new_compound_ids:
-                    self.add_compound_from_reference(reference_model=reference_model, compound_id=compound_id)
+                    self.add_compound_from_reference(
+                        reference_model=reference_model, compound_id=compound_id
+                    )
             for reaction in new_reactions:
                 self.add_reaction(reaction=reaction)
                 if reaction.id in reference_model._duplicate_reactions:
                     self._duplicate_reactions.add(reaction.id)
         elif base_id in reference_model.base_reactions:
             try:
                 for reaction_id in tuple(self.base_reactions[base_id]):
@@ -1097,565 +1158,876 @@
             new_reactions = [
                 reference_model.reactions[reaction_id]
                 for reaction_id in reference_model.base_reactions[base_id]
             ]
             if update_compounds:
                 new_compound_ids = {j for i in new_reactions for j in i.stoichiometries}
                 for compound_id in new_compound_ids:
-                    self.add_compound_from_reference(reference_model=reference_model, compound_id=compound_id)
+                    self.add_compound_from_reference(
+                        reference_model=reference_model, compound_id=compound_id
+                    )
             for reaction in new_reactions:
                 self.add_reaction(reaction=reaction)
                 if reaction.id in reference_model._duplicate_reactions:
                     self._duplicate_reactions.add(reaction.id)
         elif base_id in reference_model.reactions:
             self.add_reaction_from_reference(
                 reference_model=reference_model,
-                reaction_id=cast(str, reference_model.reactions[reaction_id].base_id),
+                reaction_id=reference_model.reactions[reaction_id].base_id,
             )
         else:
             raise KeyError(f"Could not find {reaction_id} in the reference_model")
 
     def add_reactions_from_reference(
-        self,
-        reference_model: "Model",
-        reaction_ids: Iterable[str],
-        update_compounds: bool = True,
-    ) -> None:
-        """Add reactions from a reference model, overwriting existing reactions."""
+        self, reference_model, reaction_ids, update_compounds=True
+    ):
+        """Add reactions from a reference model, overwriting existing reactions.
+
+        Parameters
+        ----------
+        reference_model : moped.Model
+        reaction_ids : Iterable(str)
+        update_compounds : bool
+            Whether to update all compounds that take place in the reaction as well
+        """
         for reaction_id in reaction_ids:
             self.add_reaction_from_reference(
                 reference_model=reference_model,
                 reaction_id=reaction_id,
                 update_compounds=update_compounds,
             )
 
-    def set_reaction_property(self, reaction_id: str, property_dict: Dict[str, Any]) -> None:
-        """Set one or multiple properties of a reaction."""
+    def set_reaction_property(self, reaction_id, property_dict):
+        """Set one or multiple properties of a reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+        property_dict
+            Dictionary containing attribute: value pairs
+
+        Raises
+        ------
+        KeyError
+            If Reaction does not have one of the keys of property_dict
+        """
         for k, v in property_dict.items():
-            reaction = self.reactions[reaction_id]
-            if k in reaction.__dict__:
+            try:
                 setattr(self.reactions[reaction_id], k, v)
-            else:
-                raise KeyError(f"Reaction does not have key '{k}', can only be one of {Reaction.__dict__}")
+            except AttributeError:
+                raise KeyError(
+                    f"Reaction does not have key '{k}', can only be one of {Reaction.__slots__}"
+                )
+
+    def remove_reaction(self, reaction_id, remove_empty_references=True):
+        """Remove a reaction from the model.
+
+        This also removes the reaction from reaction_variants, pathways
+        and its compounds in_reaction attribute if applicable.
+        If the compound in_reaction attribute is empty it also removes the compound
+
+        Parameters
+        ----------
+        reaction_id: str
 
-    def remove_reaction(self, reaction_id: str, remove_empty_references: bool = True) -> None:
-        """Remove a reaction from the model."""
+        Raises
+        ------
+        KeyError
+            If reaction is not in the model
+        """
         reaction = self.reactions[reaction_id]
-        base_id = cast(str, reaction.base_id)
-        if reaction._var is not None:
-            self.variant_reactions[base_id].remove(reaction_id)
+        if "__var__" in reaction_id:
+            self.variant_reactions[reaction.base_id].remove(reaction_id)
             if remove_empty_references:
-                if not bool(self.variant_reactions[base_id]):
-                    del self.variant_reactions[base_id]
+                if not bool(self.variant_reactions[reaction.base_id]):
+                    del self.variant_reactions[reaction.base_id]
         else:
-            self.base_reactions[base_id].remove(reaction_id)
+            self.base_reactions[reaction.base_id].remove(reaction_id)
             if remove_empty_references:
-                if not bool(self.base_reactions[base_id]):
-                    del self.base_reactions[base_id]
+                if not bool(self.base_reactions[reaction.base_id]):
+                    del self.base_reactions[reaction.base_id]
         for pathway in tuple(reaction.pathways):
-            self.remove_reaction_from_pathway(pathway_id=pathway, reaction_id=reaction_id)
+            self.remove_reaction_from_pathway(
+                pathway_id=pathway, reaction_id=reaction_id
+            )
         for compound in reaction.stoichiometries:
             self.compounds[compound].in_reaction.remove(reaction_id)
             if remove_empty_references:
                 if not bool(self.compounds[compound].in_reaction):
                     del self.compounds[compound]
-        for type_ in reaction.types:
-            self._reaction_types[type_].remove(reaction_id)
-            if remove_empty_references:
-                if not bool(self._reaction_types[type_]):
-                    del self._reaction_types[type_]
         del self.reactions[reaction_id]
 
-    def remove_reactions(self, reaction_ids: Iterable[str]) -> None:
-        """Remove multiple reactions from the model."""
+    def remove_reactions(self, reaction_ids):
+        """Remove multiple reactions from the model.
+
+        Parameters
+        ----------
+        reaction_ids: iterable(str)
+
+        Raises
+        ------
+        KeyError
+            If reaction is not in the model
+        """
         for reaction_id in reaction_ids:
             self.remove_reaction(reaction_id=reaction_id)
 
-    def get_reaction_base_id(self, reaction_id: str) -> str | None:
-        """Get the base id of a given reaction."""
+    def get_reaction_base_id(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].base_id
 
-    def get_reaction_compartment_variants(self, reaction_base_id: str) -> Set[str]:
-        """Get the ids of the reaction in all compartments it takes place in."""
+    def get_reaction_compartment_variants(self, reaction_base_id):
+        """Get the ids of the reaction in all compartments it takes place in.
+
+        Parameters
+        ----------
+        reaction_base_id : str
+
+        Returns
+        -------
+        reaction_ids : set
+        """
         return self.base_reactions[reaction_base_id]
 
-    def get_reaction_compartment(self, reaction_id: str) -> str | Tuple[str, ...] | None:
-        """Get the compartment of a given reaction."""
+    def get_reaction_compartment(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].compartment
 
-    def get_reaction_gibbs0(self, reaction_id: str) -> float | None:
-        """Get the database links of a given reaction."""
+    def get_reaction_gibbs0(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].gibbs0
 
-    def get_reaction_bounds(self, reaction_id: str) -> Tuple[float, float] | None:
-        """Get the bounds of a given reaction."""
+    def get_reaction_bounds(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].bounds
 
-    def get_reaction_reversibility(self, reaction_id: str) -> bool | None:
-        """Get whether a reaction is reversible."""
+    def get_reaction_reversibility(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].reversible
 
-    def get_reaction_pathways(self, reaction_id: str) -> Set[str]:
-        """Get the pathways of a given reaction."""
+    def get_reaction_pathways(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].pathways
 
-    def get_reaction_sequences(self, reaction_id: str) -> Dict[str, str]:
-        """Get the protein sequences of a given reaction."""
-        sequences = {}
-        reaction = self.reactions[reaction_id]
-        for enzyme in reaction.gpr_annotation:
-            for mon_id in enzyme:
-                if (mon := self.monomers.get(mon_id)) is not None:
-                    if (seq := mon.sequence) is not None:
-                        sequences[mon_id] = seq
-        return sequences
+    def get_reaction_sequences(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
 
-    def get_reaction_types(self, reaction_id: str) -> List[str]:
-        """Get the types of a given reaction."""
+        Returns
+        -------
+        database_links: dict
+        """
+        return self.reactions[reaction_id].sequences
+
+    def get_reaction_types(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].types
 
-    def get_reaction_database_links(self, reaction_id: str) -> Dict[str, Set[str]]:
-        """Get the database links of a given reaction."""
+    def get_reaction_database_links(self, reaction_id):
+        """Get the database links for a given reaction.
+
+        Parameters
+        ----------
+        reaction_id: str
+
+        Returns
+        -------
+        database_links: dict
+        """
         return self.reactions[reaction_id].database_links
 
-    def get_base_reaction_ids(self) -> Set[str]:
-        """Get base IDs of all reactions."""
+    def get_base_reaction_ids(self):
+        """Get base IDs of all reactions.
+
+        Returns
+        -------
+        base_compound_ids: set
+        """
         return set(self.base_reactions)
 
-    def get_reaction_type_ids(self) -> Set[str]:
+    def get_reaction_type_ids(self):
         """Get all available reaction types."""
         return set(self._reaction_types)
 
-    def get_reactions_of_type(self, reaction_type: str) -> Set[str]:
-        """Get all reaction ids of a given type."""
+    def get_reactions_of_type(self, reaction_type):
+        """Get all reaction ids of a given type.
+
+        Parameters
+        ----------
+        reaction_type : str
+
+        Returns
+        -------
+        reaction_ids : str
+        """
         return self._reaction_types[reaction_type]
 
-    def get_reaction_variants(self, base_reaction_id: str) -> Set[str]:
-        """Get all reaction variants."""
+    def get_reaction_variants(self, base_reaction_id):
+        """Get all reaction variants.
+
+        Parameters
+        ----------
+        base_reaction_id: str
+            So e.g. rxn1, if the variants are rxn1__var__0 etc
+        """
         return self.variant_reactions[base_reaction_id]
 
-    def get_reversible_reactions(self) -> List[str]:
-        """Get all reactions marked as reversible."""
+    def get_reversible_reactions(self):
+        """Get all reactions marked as reversible.
+
+        Returns
+        -------
+        reactions: list(str)
+            List of reaction ids
+        """
         return [k for k, v in self.reactions.items() if v.reversible]
 
-    def get_irreversible_reactions(self) -> List[str]:
-        """Get all reactions marked as irreversible."""
+    def get_irreversible_reactions(self):
+        """Get all reactions marked as irreversible.
+
+        Returns
+        -------
+        reactions: list(str)
+            List of reaction ids
+        """
         return [k for k, v in self.reactions.items() if not v.reversible]
 
-    def get_transmembrane_reactions(self) -> List[str]:
-        """Get reaction ids for reactions with compounds in two compartments."""
+    def get_transmembrane_reactions(self):
+        """Get reaction ids for reactions with compounds in two compartments.
+
+        Returns
+        -------
+        transmembrane_reactions : list(str)
+        """
         return [k for k, v in self.reactions.items() if v.transmembrane]
 
-    def get_reactions_of_compartment(
-        self, compartment_id: str, include_transporters: bool = True
-    ) -> Set[str]:
-        """Reaction reaction ids for reactions that occur in a given compartment."""
+    def get_reactions_of_compartment(self, compartment_id, include_transporters=True):
+        """Reaction reaction ids for reactions that occur in a given compartment.
+
+        Parameters
+        ----------
+        compartment : str
+        include_transporters : bool
+            Whether to include transmembrane reactions that transport anything in/out
+            of the compartment
+
+        Returns
+        -------
+        compartment_reactions : set(str)
+        """
         reaction_ids = {
             reaction_id
-            for compound_id in self.get_compounds_of_compartment(compartment_id=compartment_id)
+            for compound_id in self.get_compounds_of_compartment(
+                compartment_id=compartment_id
+            )
             for reaction_id in self.compounds[compound_id].in_reaction
         }
         if include_transporters:
             return reaction_ids
         return reaction_ids.difference(self.get_transmembrane_reactions())
 
-    def get_transport_reactions(self, compartment_id: str) -> Set[str]:
-        """Get reactions that transport something in/out of a given compartment."""
+    def get_transport_reactions(self, compartment_id):
+        """Get reactions that transport something in/out of a given compartment.
+
+        Parameters
+        ----------
+        into_compartment : str
+
+        Returns
+        -------
+        transport_reactions : set(str)
+        """
         compartment_reactions = self.get_reactions_of_compartment(
             compartment_id=compartment_id, include_transporters=True
         )
         transmembrane_reactions = self.get_transmembrane_reactions()
         return set(transmembrane_reactions).intersection(compartment_reactions)
 
     ##########################################################################
     # Pathway functions
     ##########################################################################
 
-    def add_pathway(self, pathway_id: str, pathway_reactions: Iterable[str]) -> None:
-        """Add a pathway to the model."""
+    def add_pathway(self, pathway_id, pathway_reactions):
+        """Add a pathway to the model.
+
+        This also adds the pathway to all reaction objects
+
+        Parameters
+        ----------
+        pathway_id: str
+        pathway_reactions: list(str)
+        """
         for reaction_id in pathway_reactions:
             self.reactions[reaction_id].pathways.add(pathway_id)
         self.pathways.setdefault(pathway_id, set()).update(pathway_reactions)
 
-    def add_reaction_to_pathway(self, pathway_id: str, reaction_id: str) -> None:
-        """Add a reaction to a pathway."""
+    def add_reaction_to_pathway(self, pathway_id, reaction_id):
+        """Add a reaction to a pathway.
+
+        This also adds the pathway to the reaction object
+
+        Parameters
+        ----------
+        pathway_id: str
+        reaction_id: str
+        """
         self.reactions[reaction_id].pathways.add(pathway_id)
         self.pathways.setdefault(pathway_id, set()).add(reaction_id)
 
-    def remove_pathway(self, pathway_id: str) -> None:
-        """Remove a pathway from the model."""
+    def remove_pathway(self, pathway_id):
+        """Remove a pathway from the model.
+
+        This also removes the pathway from all the reactions
+
+        Parameters
+        ----------
+        pathway_id: str
+        """
         reactions = self.pathways.pop(pathway_id)
         for reaction in reactions:
             self.reactions[reaction].pathways.remove(pathway_id)
 
-    def remove_reaction_from_pathway(self, pathway_id: str, reaction_id: str) -> None:
-        """Remove a reaction from a pathway."""
+    def remove_reaction_from_pathway(self, pathway_id, reaction_id):
+        """Remove a reaction from a pathway.
+
+        This also removes the pathway from the reaction object
+
+        Parameters
+        ----------
+        pathway_id: str
+        reaction_id: str
+        """
         self.pathways[pathway_id].remove(reaction_id)
         self.reactions[reaction_id].pathways.remove(pathway_id)
         # Remove pathway completely if it is empty
         if self.pathways[pathway_id] == set():
             self.remove_pathway(pathway_id=pathway_id)
 
-    def get_reactions_of_pathway(self, pathway_id: str) -> Set[str]:
-        """Get all reactions that are part of a pathway."""
+    def get_reactions_of_pathway(self, pathway_id):
+        """Get all reactions that are part of a pathway.
+
+        Parameters
+        ----------
+        pathway_id: str
+            Name of the pathway
+
+        Returns
+        -------
+        pathways: set(str)
+            Set of all reaction ids
+        """
         return self.pathways[pathway_id]
 
-    def get_pathway_ids(self) -> list[str]:
-        """Get all pathway ids."""
-        return list(self.pathways.keys())
+    def get_pathway_ids(self):
+        """Get all pathway ids.
+
+        Returns
+        -------
+        pathway_ids: tuple(str)
+        """
+        return tuple(self.pathways.keys())
 
     ##########################################################################
     # Medium, biomass and objective functions
     ##########################################################################
 
-    def add_transport_reaction(
-        self,
-        compound_id: str,
-        compartment_id: str,
-        bounds: Tuple[float, float] = (-1000, 1000),
-    ) -> None:
-        """Add a transport reaction into another compartment."""
-        orig_compartment = self.compounds[compound_id].compartment
+    def add_transport_reaction(self, compound_id, compartment_id, bounds=(-1000, 1000)):
+        """Add a transport reaction into another compartment.
+
+        Parameters
+        ----------
+        compound_id: str
+        compartment_id: str
+            The compartment into which the compound is transported
+        bounds: tuple(int, int)
+        """
         into_cpd = self.add_compartment_compound_variant(
             compound_id=compound_id, compartment_id=compartment_id
         )
-        into_suffix = self._add_compartment_suffix(object_id="", compartment_id=compartment_id)
+        into_suffix = self._add_compartment_suffix(
+            object_id="", compartment_id=compartment_id
+        )
+        if bounds[0] < 0 and bounds[1] > 0:
+            reversible = True
+        else:
+            reversible = False
         self.add_reaction(
             Reaction(
                 id=f"TR_{compound_id}{into_suffix}",
                 base_id=f"TR_{compound_id}",
-                stoichiometries={compound_id: -1, cast(str, into_cpd.id): 1},
+                stoichiometries={compound_id: -1, into_cpd.id: 1},
                 bounds=bounds,
+                reversible=reversible,
                 transmembrane=True,
-                compartment=(orig_compartment, compartment_id),
             )
         )
 
-    def add_influx(self, compound_id: str, extracellular_compartment_id: str) -> None:
-        """Add an influx of a compound to the model."""
+    def add_influx(self, compound_id, extracellular_compartment_id):
+        """Add an influx of a compound to the model.
+
+        Parameters
+        ----------
+        compound_id: str
+        add_tranporters: bool
+            If transport reactions into the cytosol should be added
+        """
         # Add influx
-        orig_compartment = self.compounds[compound_id].compartment
         ex_met = self.add_compartment_compound_variant(
             compound_id=compound_id, compartment_id=extracellular_compartment_id
         )
         self.add_reaction(
             Reaction(
                 id=f"EX_{ex_met.base_id}_e",
                 base_id=f"EX_{ex_met.base_id}",
-                stoichiometries={cast(str, ex_met.id): -1},
+                stoichiometries={ex_met.id: -1},
                 bounds=(-1000, 0),
-                compartment=(orig_compartment, extracellular_compartment_id),
             )
         )
 
-    def remove_influx(self, compound_id: str) -> None:
-        """Remove the influx of a given compound."""
-        try:
-            compound = self.compounds[compound_id]
-            base_compound_id = compound.base_id
-        except KeyError:
-            if compound_id not in self.base_compounds:
-                raise KeyError(f"Compound {compound_id} neither found in compounds nor base compounds")
-            base_compound_id = compound_id
-        self.remove_reaction(reaction_id=f"EX_{base_compound_id}_e")
+    def remove_influx(self, compound_id):
+        """Remove the influx of a given compound.
 
-    def add_efflux(self, compound_id: str, extracellular_compartment_id: str) -> None:
-        """Add an efflux of a compound to the model."""
+        Parameters
+        ----------
+        compound_id : str
+        """
+        compound = self.compounds[compound_id]
+        self.remove_reaction(reaction_id=f"EX_{compound.base_id}_e")
+
+    def add_efflux(self, compound_id, extracellular_compartment_id):
+        """Add an efflux of a compound to the model.
+
+        Parameters
+        ----------
+        compound_id: str
+        add_tranporters: bool
+            If transport reactions out of the cytosol should be added
+        """
         # Add efflux
-        orig_compartment = self.compounds[compound_id].compartment
         ex_met = self.add_compartment_compound_variant(
             compound_id=compound_id, compartment_id=extracellular_compartment_id
         )
         self.add_reaction(
             Reaction(
                 id=f"EX_{ex_met.base_id}_e",
                 base_id=f"EX_{ex_met.base_id}",
-                stoichiometries={cast(str, ex_met.id): -1},
+                stoichiometries={ex_met.id: -1},
                 bounds=(0, 1000),
-                compartment=(orig_compartment, extracellular_compartment_id),
+                reversible=False,
             )
         )
 
-    def remove_efflux(self, compound_id: str) -> None:
-        """Remove the efflux of a given compound."""
-        try:
-            compound = self.compounds[compound_id]
-            base_compound_id = compound.base_id
-        except KeyError:
-            if compound_id not in self.base_compounds:
-                raise KeyError(f"Compound {compound_id} neither found in compounds nor base compounds")
-            base_compound_id = compound_id
-        self.remove_reaction(reaction_id=f"EX_{base_compound_id}_e")
+    def remove_efflux(self, compound_id):
+        """Remove the efflux of a given compound.
+
+        Parameters
+        ----------
+        compound_id : str
+        """
+        compound = self.compounds[compound_id]
+        self.remove_reaction(reaction_id=f"EX_{compound.base_id}_e")
+
+    def add_medium_component(self, compound_id, extracellular_compartment_id):
+        """Add a compound as a medium component.
 
-    def add_medium_component(self, compound_id: str, extracellular_compartment_id: str) -> None:
-        """Add a compound as a medium component."""
+        Parameters
+        ----------
+        compound_id: str
+        add_tranporters: bool
+            If transport reactions in and out of the cytosol should be added
+        """
         # Add medium influx/efflux
-        orig_compartment = self.compounds[compound_id].compartment
         ex_met = self.add_compartment_compound_variant(
             compound_id=compound_id, compartment_id=extracellular_compartment_id
         )
         self.add_reaction(
             Reaction(
                 id=f"EX_{ex_met.base_id}_e",
                 base_id=f"EX_{ex_met.base_id}",
-                stoichiometries={cast(str, ex_met.id): -1},
+                stoichiometries={ex_met.id: -1},
                 bounds=(-1000, 1000),
-                compartment=(orig_compartment, extracellular_compartment_id),
+                reversible=True,
             )
         )
 
-    def remove_medium_component(self, compound_id: str) -> None:
-        """Remove influx and outflux of a given compound."""
-        try:
-            compound = self.compounds[compound_id]
-            base_compound_id = compound.base_id
-        except KeyError:
-            if compound_id not in self.base_compounds:
-                raise KeyError(f"Compound {compound_id} neither found in compounds nor base compounds")
-            base_compound_id = compound_id
-        self.remove_reaction(reaction_id=f"EX_{base_compound_id}_e")
+    def remove_medium_component(self, compound_id):
+        """Remove influx and outflux of a given compound.
+
+        Parameters
+        ----------
+        compound_id : str
+        """
+        compound = self.compounds[compound_id]
+        self.remove_reaction(reaction_id=f"EX_{compound.base_id}_e")
+
+    def get_biomass_template(self, organism="ecoli"):
+        """Return an organism specific biomass composition.
+
+        Parameters
+        ----------
+        organism: str
 
-    def get_biomass_template(self, organism: str = "ecoli") -> Dict[str, float]:
-        """Return an organism specific biomass composition."""
+        Returns
+        -------
+        biomass_template: dict(str: float)
+            Biomass composition of the organism
+        """
         try:
             return BIOMASS_TEMPLATES[organism]
         except KeyError:
             raise KeyError(
-                f"Could not find template for organism {organism}. "
-                + f"Currenly supported organisms are {tuple(BIOMASS_TEMPLATES)}"
+                f"Could not find template for organism {organism}. Currenly supported organisms are {tuple(BIOMASS_TEMPLATES)}"
             )
 
-    def set_objective(self, objective: Dict[str, float]) -> None:
-        """Set the objective function(s)."""
-        for reaction_id in objective:
-            if reaction_id not in self.reactions:
-                raise KeyError(f"Objective reaction {reaction_id} is not in the model")
+    def set_objective(self, objective):
+        """Set the objective function(s).
+
+        Parameters
+        ----------
+        objective_dictionary: dict(str: float)
+            Dictionary containing reaction_id:coefficient pairings
+        """
         self.objective = dict(objective)
 
     ##########################################################################
     # Quality control interface
     ##########################################################################
 
-    def check_charge_balance(self, reaction_id: str, verbose: bool = False) -> bool:
-        """Check the charge balance of a reaction."""
-        substrate_charge = 0.0
-        product_charge = 0.0
+    def check_charge_balance(self, reaction_id, verbose=False):
+        """Check the charge balance of a reaction.
+
+        Parameter
+        ---------
+        reaction_id: str
+        verbose: bool
+
+        Returns
+        -------
+        balanced: bool
+            Whether the reaction is balanced or not
+        """
+        substrate_charge = 0
+        product_charge = 0
         for k, v in self.reactions[reaction_id].stoichiometries.items():
-            charge = self.compounds[k].charge
-            if charge is None:
-                return False
             if v < 0:
-                substrate_charge -= charge * v
+                substrate_charge -= self.compounds[k].charge * v
             else:
-                product_charge += charge * v
+                product_charge += self.compounds[k].charge * v
         if verbose:
             print(f"Substrate charge: {substrate_charge}")
             print(f"Product charge: {product_charge}")
         if substrate_charge - product_charge == 0:
             return True
         return False
 
-    def check_mass_balance(self, reaction_id: str, verbose: bool = False) -> bool:
-        """Check the mass balance of a reaction."""
-        lhs_atoms: DefaultDict[str, float] = defaultdict(int)
-        rhs_atoms: DefaultDict[str, float] = defaultdict(int)
+    def check_mass_balance(self, reaction_id, verbose=False):
+        """Check the mass balance of a reaction.
+
+        Parameter
+        ---------
+        reaction_id: str
+        verbose: bool
+
+        Returns
+        -------
+        balanced: bool
+            Whether the reaction is balanced or not
+        """
+        lhs_atoms = defaultdict(lambda: 0)
+        rhs_atoms = defaultdict(lambda: 0)
         for k, v in self.reactions[reaction_id].stoichiometries.items():
             formula = self.compounds[k].formula
             if not bool(formula):
                 return False
             if v < 0:
                 for atom, stoich in formula.items():
                     lhs_atoms[atom] -= stoich * v
             else:
                 for atom, stoich in formula.items():
                     rhs_atoms[atom] += stoich * v
         if verbose:
             print(dict(lhs_atoms))
             print(dict(rhs_atoms))
+        diffs = {}
         for k in set((*lhs_atoms, *rhs_atoms)):
-            diff = lhs_atoms[k] - rhs_atoms[k]
-            if diff != 0:
+            try:
+                diff = lhs_atoms[k] - rhs_atoms[k]
+            except KeyError:
                 return False
+            if diff != 0:
+                diffs[k] = diff
+        if bool(diffs):
+            return False
         return True
 
     ###########################################################################
     # Stoichiometric functions
     ###########################################################################
 
-    def get_stoichiometric_matrix(self) -> np.ndarray:
-        """Return the stoichiometric matrix."""
+    def get_stoichiometric_matrix(self):
+        """Return the stoichiometric matrix.
+
+        Returns
+        -------
+        N: numpy.array
+        """
         cpd_mapper = dict(zip(self.compounds, range(len(self.compounds))))
         N = np.zeros((len(self.compounds), len(self.reactions)))
         for i, rxn in enumerate(self.reactions.values()):
             for cpd, val in rxn.stoichiometries.items():
                 N[cpd_mapper[cpd], i] = val
         return N
 
-    def get_stoichiometric_df(self) -> pd.DataFrame:
-        """Return the stoichiometric matrix as an annotated pandas dataframe."""
+    def get_stoichiometric_df(self):
+        """Return the stoichiometric matrix as an annotated pandas dataframe.
+
+        Returns
+        -------
+        N: pandas.DataFrame
+        """
         return pd.DataFrame(
             self.get_stoichiometric_matrix(),
-            index=cast(list, self.compounds),  # actually keys(), but doesn't matter
-            columns=cast(list, self.reactions),  # actually keys(), but doesn't matter
+            index=self.compounds,
+            columns=self.reactions,
         )
 
     ##########################################################################
     # Structural functions
     ##########################################################################
 
-    def add_minimal_seed(self, compound_ids: Iterable[str]) -> None:
-        """Add compounds that make up a minimal seed for the given organism."""
+    def add_minimal_seed(self, compound_ids):
+        """Add compounds that make up a minimal seed for the given organism.
+
+        Parameters
+        ----------
+        compound_ids : Iterable(str)
+        """
         for compound in compound_ids:
             self.minimal_seed.add(compound)
 
-    def get_minimal_seed(self, carbon_source_id: str) -> Set[str]:
-        """Get a minimal seed for most organisms."""
+    def get_minimal_seed(self, carbon_source_id):
+        """Get a minimal seed for most organisms.
+
+        Parameters
+        ----------
+        carbon_source: str
+            compound_id of the carbon source
+
+        Returns
+        -------
+        minimal_medium: list(str)
+        """
         if not bool(self.minimal_seed):
             raise ValueError(
                 "No minimal seed defined for this database. You can define one with Model.add_minimal_seed"
             )
-        seed = self.minimal_seed.copy()
-        seed.add(carbon_source_id)
-        return seed
+        else:
+            seed = self.minimal_seed.copy()
+            seed.add(carbon_source_id)
+            return seed
 
-    def reversibility_duplication(self) -> None:
+    def reversibility_duplication(self):
         """Add additional reverse reactions for all reactions that are reversible.
 
         Useful for structural analyses as scope and gapfilling
 
         Adds the __rev__ tag to those reactions.
         """
         for reaction_id in self.get_reversible_reactions():
-            rev_reaction = copy.deepcopy(self.reactions[reaction_id])
+            rev_reaction = self.reactions[reaction_id].copy()
             rev_reaction.id += "__rev__"
             rev_reaction.reverse_stoichiometry()
+            rev_reaction.reversible = False
             self.add_reaction(reaction=rev_reaction)
             self._duplicate_reactions.add(rev_reaction.id)
 
-    def remove_reversibility_duplication(self) -> None:
+    def remove_reversibility_duplication(self):
         """Remove the additional reverse reactions introduced.
 
         by model.reversibility_duplication
         """
         for reaction_id in tuple(self._duplicate_reactions):
             if "__rev__" in reaction_id:
                 self.remove_reaction(reaction_id=reaction_id)
                 self._duplicate_reactions.remove(reaction_id)
         self._duplicate_reactions = set()
 
-    def cofactor_duplication(self) -> None:
+    def cofactor_duplication(self):
         """Add additional reactions for reactions carrying cofactor pairs.
 
         Adds a __cof__ tag for every reaction that contains one of the cofactor pairs in model.cofactor_pairs.
 
         Useful for structural analyses as scope and gapfilling
         """
         # Add all cofacor metabolites, if they are in the model
         for k, v in self.cofactor_pairs.items():
             if k in self.compounds:
-                cof_cpd = copy.deepcopy(self.compounds[k])
-                cof_cpd.id = cast(str, cof_cpd.id) + "__cof__"
-                cof_cpd.in_reaction = set()
+                cof_cpd = self.compounds[k].copy()
+                cof_cpd.id = cof_cpd.id + "__cof__"
                 self.add_compound(compound=cof_cpd)
 
-                pair_cpd = copy.deepcopy(self.compounds[v])
-                pair_cpd.id = cast(str, pair_cpd.id) + "__cof__"
-                pair_cpd.in_reaction = set()
+                pair_cpd = self.compounds[v].copy()
+                pair_cpd.id = pair_cpd.id + "__cof__"
                 self.add_compound(compound=pair_cpd)
 
         for reaction in tuple(self.reactions.values()):
             reaction_cofactors = []
             for cof, pair in self.cofactor_pairs.items():
                 if cof in reaction.stoichiometries:
                     if pair in reaction.stoichiometries:
-                        if reaction.stoichiometries[cof] == -reaction.stoichiometries[pair]:
+                        if (
+                            reaction.stoichiometries[cof]
+                            == -reaction.stoichiometries[pair]
+                        ):
                             reaction_cofactors.append((cof, pair))
             if len(reaction_cofactors) > 0:
-                cofactor_reaction = copy.deepcopy(self.reactions[reaction.id])
+                cofactor_reaction = self.reactions[reaction.id].copy()
                 cofactor_reaction.id += "__cof__"
                 for (cof, pair) in reaction_cofactors:
-                    cofactor_reaction.replace_compound(old_compound=cof, new_compound=cof + "__cof__")
-                    cofactor_reaction.replace_compound(old_compound=pair, new_compound=pair + "__cof__")
+                    cofactor_reaction.replace_compound(
+                        old_compound=cof, new_compound=cof + "__cof__"
+                    )
+                    cofactor_reaction.replace_compound(
+                        old_compound=pair, new_compound=pair + "__cof__"
+                    )
                 self.add_reaction(reaction=cofactor_reaction)
                 self._duplicate_reactions.add(cofactor_reaction.id)
 
-    def remove_cofactor_duplication(self) -> None:
+    def remove_cofactor_duplication(self):
         """Remove the additional reverse reactions introduced by model.cofactor_duplication."""
         for reaction_id in tuple(self._duplicate_reactions):
             if "__cof__" in reaction_id:
                 self.remove_reaction(reaction_id)
                 self._duplicate_reactions.remove(reaction_id)
+        for i in tuple(self.compounds):
+            if "__cof__" in i:
+                del self.compounds[i]
 
     def breadth_first_search(
         self,
-        start_compound_id: str,
-        end_compound_id: str,
-        max_iterations: int = 50,
-        ignored_reaction_ids: Iterable[str] | None = None,
-        ignored_compound_ids: Iterable[str] | None = None,
-    ) -> SearchResult:
+        start_compound_id,
+        end_compound_id,
+        max_iterations=50,
+        ignored_reaction_ids=None,
+        ignored_compound_ids=None,
+    ):
         """Breadth-first search to find shortest path connecting two metabolites."""
-        metabolites, reactions = topological.metabolite_tree_search(
+        return topological.metabolite_tree_search(
             model=self,
             start_compound_id=start_compound_id,
             end_compound_id=end_compound_id,
             max_iterations=max_iterations,
             ignored_reaction_ids=ignored_reaction_ids,
             ignored_compound_ids=ignored_compound_ids,
             search_type="breadth-first",
         )
-        return SearchResult(reactions=reactions, compounds=metabolites)
 
     def depth_first_search(
         self,
-        start_compound_id: str,
-        end_compound_id: str,
-        max_iterations: int = 50,
-        ignored_reaction_ids: Iterable[str] | None = None,
-        ignored_compound_ids: Iterable[str] | None = None,
-    ) -> SearchResult:
-        """Depth-first search to find shortest path connecting two metabolites.
-
-        Parameters
-        ----------
-        start_compound_id: str
-        end_compound_id: str
-        max_iterations: int
-        ignored_reaction_ids: iterable(str)
-        ignored_compound_ids: iterable(str)
-
-        Returns
-        -------
-        metabolites: list(str)
-        reactions: list(str)"""
-        metabolites, reactions = topological.metabolite_tree_search(
+        start_compound_id,
+        end_compound_id,
+        max_iterations=50,
+        ignored_reaction_ids=None,
+        ignored_compound_ids=None,
+    ):
+        """Depth-first search to find shortest path connecting two metabolites."""
+        return topological.metabolite_tree_search(
             model=self,
             start_compound_id=start_compound_id,
             end_compound_id=end_compound_id,
             max_iterations=max_iterations,
             ignored_reaction_ids=ignored_reaction_ids,
             ignored_compound_ids=ignored_compound_ids,
             search_type="depth-first",
         )
-        return SearchResult(reactions=reactions, compounds=metabolites)
 
-    def scope(
-        self,
-        seed: Iterable[str],
-        include_weak_cofactors: bool = False,
-        return_lumped_results: bool = True,
-    ) -> Tuple[Set[str], Set[str]] | Tuple[list[Set[str]], list[Set[str]]]:
+    def scope(self, seed, include_weak_cofactors=False, return_lumped_results=True):
         """Run the scope algorithm for a single seed.
 
+        Parameters
+        ----------
+        seed: iterable
+        include_weak_cofactors: bool
+            Whether to include the weak cofactor duplications in the seed
+        return_lumped_results: bool
+            Whether to return the results as two sets or two lists of multiple sets
+            for each iteration
+
         Returns
         -------
-        scope_reactions
+        scope_reactions: set
             Can be turned into a list of sets for the respective iteration with
             return_lumped_results=False
-        scope_compounds
+        scope_compounds: set
             Can be turned into a list of sets for the respective iteration with
             return_lumped_results=False
 
 
         See Also
         --------
         model.multiple_scopes
@@ -1665,27 +2037,36 @@
             seed=seed,
             include_weak_cofactors=include_weak_cofactors,
             return_lumped_results=return_lumped_results,
         )
 
     def multiple_scopes(
         self,
-        seeds: Iterable[Iterable[str]],
-        include_weak_cofactors: bool = False,
-        return_lumped_results: bool = True,
-        multiprocessing: bool = False,
-    ) -> Dict[tuple, Tuple[Set[str], Set[str]] | Tuple[list[Set[str]], list[Set[str]]]]:
+        seeds,
+        include_weak_cofactors=False,
+        return_lumped_results=True,
+        multiprocessing=False,
+    ):
         """Run the scope algorithm for multiple seeds.
 
+        Parameters
+        ----------
+        seeds: iterable(iterable)
+        include_weak_cofactors: bool
+            Whether to include the weak cofactor duplications in the seed
+        return_lumped_results: bool
+            Whether to return the results as two sets or two lists of multiple sets
+            for each iteration
+
         Returns
         -------
-        scope_reactions
+        scope_reactions: set
             Can be turned into a list of sets for the respective iteration with
             return_lumped_results=False
-        scope_compounds
+        scope_compounds: set
             Can be turned into a list of sets for the respective iteration with
             return_lumped_results=False
 
 
         See Also
         --------
         model.scope
@@ -1696,40 +2077,73 @@
             include_weak_cofactors=include_weak_cofactors,
             return_lumped_results=return_lumped_results,
             multiprocessing=multiprocessing,
         )
 
     def get_gapfilling_reactions(
         self,
-        reference_model: "Model",
-        seed: Iterable[str],
-        targets: Iterable[str],
-        include_weak_cofactors: bool = False,
-        verbose: bool = False,
-    ) -> List[str]:
-        """Find reactions out of a reference model necessary to produce
-        all given targets from a given seed"""
+        reference_model,
+        seed,
+        targets,
+        include_weak_cofactors=False,
+        verbose=False,
+    ):
+        """Run the gapfilling algorithm.
+
+        To find reactions out of a reference model
+        necessary to produce all given targets from a given seed
+
+        Parameters
+        ----------
+        reference_model: moped.Model
+        seed: iterable(str)
+            Seed compound ids
+        targets: iterable(str)
+            Target compound ids
+
+        Returns
+        -------
+        gapfilled_reactions: list(str)
+            List of reaction ids which are necessary to produce all targets
+        """
         return topological.gapfilling(
             model=self,
             reference_model=reference_model,
             seed=seed,
             targets=targets,
             include_weak_cofactors=include_weak_cofactors,
             verbose=verbose,
         )
 
     def gapfilling(
         self,
-        reference_model: "Model",
-        seed: Iterable[str],
-        targets: Iterable[str],
-        include_weak_cofactors: bool = False,
-        verbose: bool = False,
-    ) -> None:
-        """Run the gapfilling algorithm and add the results to the model."""
+        reference_model,
+        seed,
+        targets,
+        include_weak_cofactors=False,
+        verbose=False,
+    ):
+        """Run the gapfilling algorithm and add the results to the model.
+
+        To find reactions out of a reference model
+        necessary to produce all given targets from a given seed
+
+        Parameters
+        ----------
+        reference_model: moped.Model
+        seed: iterable(str)
+            Seed compound ids
+        targets: iterable(str)
+            Target compound ids
+
+        Returns
+        -------
+        gapfilled_reactions: list(str)
+            List of reaction ids which are necessary to produce all targets
+        """
         gapfilling_reactions = self.get_gapfilling_reactions(
             reference_model=reference_model,
             seed=seed,
             targets=targets,
             include_weak_cofactors=include_weak_cofactors,
             verbose=verbose,
         )
@@ -1741,586 +2155,609 @@
             update_compounds=True,
         )
 
     ##########################################################################
     # Export functions
     ##########################################################################
 
-    def to_cobra(self) -> cobra.Model:
-        """Export the model into a cobra model to do FBA topological."""
+    def to_cobra(self):
+        """Export the model into a cobra model to do FBA topological.
+
+        Returns
+        -------
+        cobra_model: cobra.Model
+        """
         model = cobra.Model(self.name)
         model.compartments = {v: k for k, v in self.compartments.items()}
         model.add_metabolites(
             [
                 cobra.Metabolite(
                     id=cpd.id,
                     formula=cpd.formula_to_string(),
                     charge=cpd.charge,
-                    compartment=self.compartments[cast(str, cpd.compartment)],
+                    compartment=self.compartments[cpd.compartment],
                 )
                 for cpd in self.compounds.values()
             ]
         )
 
         for rxn in self.reactions.values():
             c_rxn = cobra.Reaction(id=rxn.id)
             model.add_reaction(c_rxn)
             c_rxn.bounds = rxn.bounds if rxn.bounds else (0, 1000)
             c_rxn.add_metabolites(rxn.stoichiometries)
 
         if self.objective is not None:
-            model.objective = {model.reactions.get_by_id(k): v for k, v in self.objective.items()}
+            model.objective = {
+                model.reactions.get_by_id(k): v for k, v in self.objective.items()
+            }
         return model
 
     ##########################################################################
     # Cobra interface
     ##########################################################################
 
-    def get_influx_reactions(
-        self,
-        cobra_solution: cobra.Solution | pd.Series,
-        sort_result: bool = False,
-    ) -> pd.DataFrame:
-        """Get influxes from a cobra simulation."""
+    def get_influx_reactions(self, cobra_solution, sort_result=False):
+        """Get influxes from a cobra simulation.
+
+        Parameters
+        ----------
+        cobra_solution
+        sort_result : bool
+            Whether to sort the results ascendingly
+
+        Returns
+        -------
+        influx_reactions: pandas.DataFrame
+        """
         exchange_reactions = {i for i in self.reactions if i.startswith("EX_")}
-        exchange_fluxes = cobra_solution[list(exchange_reactions)]  # type: ignore
-        result = -exchange_fluxes[exchange_fluxes < 0]
+        exchange_fluxes = cobra_solution.to_frame().loc[exchange_reactions, "fluxes"]
+        result = exchange_fluxes[exchange_fluxes > 0]
         if sort_result:
             return result.sort_values(ascending=False)
         return result
 
-    def get_efflux_reactions(
-        self,
-        cobra_solution: cobra.Solution | pd.Series,
-        sort_result: bool = False,
-    ) -> pd.DataFrame:
-        """Get effluxes from a cobra simulation."""
+    def get_efflux_reactions(self, cobra_solution, sort_result=False):
+        """Get effluxes from a cobra simulation.
+
+        Parameters
+        ----------
+        cobra_solution
+        sort_result : bool
+            Whether to sort the results ascendingly
+
+        Returns
+        -------
+        influx_reactions: pandas.DataFrame
+        """
         exchange_reactions = {i for i in self.reactions if i.startswith("EX_")}
-        exchange_fluxes = cobra_solution[list(exchange_reactions)]  # type: ignore
-        result = exchange_fluxes[exchange_fluxes > 0]
+        exchange_fluxes = cobra_solution.to_frame().loc[exchange_reactions, "fluxes"]
+        result = exchange_fluxes[exchange_fluxes < 0]
         if sort_result:
-            return result.sort_values(ascending=False)
+            return result.sort_values(ascending=True)
         return result
 
-    def get_producing_reactions(
-        self,
-        cobra_solution: cobra.Solution | pd.Series,
-        compound_id: str,
-        cutoff: float = 0,
-    ) -> dict[str, float]:
-        """Get reactions that produce the compound in the cobra simulation."""
+    def get_producing_reactions(self, cobra_solution, compound_id, cutoff=0):
+        """Get reactions that produce the compound in the cobra simulation.
+
+        Parameters
+        ----------
+        cobra_model: cobra.Model
+        compound_id: str
+
+        Returns
+        -------
+        reactions: dict(str: float)
+            Dictionary mapping the reation_id to the respective simulation flux
+        """
         producing = {}
         for reaction_id in self.compounds[compound_id].in_reaction:
-            flux = cobra_solution[reaction_id] * self.reactions[reaction_id].stoichiometries[compound_id]
+            flux = (
+                cobra_solution[reaction_id]
+                * self.reactions[reaction_id].stoichiometries[compound_id]
+            )
             if flux > cutoff:
                 producing[reaction_id] = flux
         return producing
 
-    def get_consuming_reactions(
-        self,
-        cobra_solution: cobra.Solution | pd.Series,
-        compound_id: str,
-        cutoff: float = 0,
-    ) -> dict[str, float]:
-        """Get reactions that consume the compound in the cobra simulation."""
+    def get_consuming_reactions(self, cobra_solution, compound_id, cutoff=0):
+        """Get reactions that consume the compound in the cobra simulation.
+
+        Parameters
+        ----------
+        cobra_model: cobra.Model
+        compound_id: str
+
+        Returns
+        -------
+        reactions: dict(str: float)
+            Dictionary mapping the reation_id to the respective simulation flux
+        """
         consuming = {}
         for reaction_id in self.compounds[compound_id].in_reaction:
-            flux = -cobra_solution[reaction_id] * self.reactions[reaction_id].stoichiometries[compound_id]
+            flux = (
+                -cobra_solution[reaction_id]
+                * self.reactions[reaction_id].stoichiometries[compound_id]
+            )
             if flux > cutoff:
                 consuming[reaction_id] = flux
         return consuming
 
     ##########################################################################
     # modelbase interface
     ##########################################################################
 
     @staticmethod
-    def _add_modelbase_influx_reaction(
-        mod: ode.Model,
-        rxn_id: str,
-        metabolite: List[str],
-        ratelaw: str = "constant",
-        suffix: str | None = None,
-    ) -> None:
+    def _add_modelbase_influx_reaction(mod, rxn_id, metabolite, ratelaw="constant"):
         if ratelaw == "constant":
             k_in = f"k_in_{rxn_id}"
             mod.add_parameters({k_in: 1})
-            if suffix is not None:
-                rxn_id += f"_{suffix}"
             mod.add_reaction_from_ratelaw(
-                rate_name=rxn_id,
-                ratelaw=rl.Constant(product=metabolite[0], k=k_in),
+                rate_name=rxn_id, ratelaw=rl.Constant(product=metabolite[0], k=k_in)
             )
         else:
             raise NotImplementedError
 
     @staticmethod
-    def _add_modelbase_efflux_reaction(
-        mod: ode.Model,
-        rxn_id: str,
-        metabolite: List[str],
-        ratelaw: str = "mass-action",
-        suffix: str | None = None,
-    ) -> None:
+    def _add_modelbase_efflux_reaction(mod, rxn_id, metabolite, ratelaw="mass-action"):
         if ratelaw == "mass-action":
             k_out = f"k_out_{rxn_id}"
             mod.add_parameters({k_out: 1})
-            if suffix is not None:
-                rxn_id += f"_{suffix}"
             mod.add_reaction_from_ratelaw(
                 rate_name=rxn_id,
                 ratelaw=rl.MassAction(substrates=metabolite, products=[], k_fwd=k_out),
             )
         else:
             raise NotImplementedError
 
     def _add_modelbase_medium_reaction(
         self,
-        mod: ode.Model,
-        rxn_id: str,
-        metabolite: List[str],
-        influx_ratelaw: str = "constant",
-        efflux_ratelaw: str = "mass-action",
-    ) -> None:
+        mod,
+        rxn_id,
+        metabolite,
+        influx_ratelaw="constant",
+        efflux_ratelaw="mass-action",
+    ):
         self._add_modelbase_influx_reaction(
             mod=mod,
-            rxn_id=rxn_id,
+            rxn_id=rxn_id + "_in",
             metabolite=metabolite,
             ratelaw=influx_ratelaw,
-            suffix="in",
         )
         self._add_modelbase_efflux_reaction(
             mod=mod,
-            rxn_id=rxn_id,
+            rxn_id=rxn_id + "_out",
             metabolite=metabolite,
             ratelaw=efflux_ratelaw,
-            suffix="out",
         )
 
     @staticmethod
     def _add_modelbase_irreversible_reaction(
-        mod: ode.Model,
-        rxn_id: str,
-        substrates: List[str],
-        products: List[str],
-        ratelaw: str = "mass-action",
-    ) -> None:
-        if ratelaw == "mass-action":
-            k_fwd = f"k_{rxn_id}"
-            mod.add_parameters({k_fwd: 1})
-            mod.add_reaction_from_ratelaw(
-                rate_name=rxn_id,
-                ratelaw=rl.MassAction(substrates=substrates, products=products, k_fwd=k_fwd),
-            )
-        else:
-            raise NotImplementedError
+        mod, rxn_id, substrates, products, ratelaw="mass-action"
+    ):
+        k_fwd = f"k_{rxn_id}"
+        mod.add_parameters({k_fwd: 1})
+        mod.add_reaction_from_ratelaw(
+            rate_name=rxn_id,
+            ratelaw=rl.MassAction(
+                substrates=substrates, products=products, k_fwd=k_fwd
+            ),
+        )
 
     @staticmethod
     def _add_modelbase_reversible_reaction(
-        mod: ode.Model,
-        rxn_id: str,
-        substrates: List[str],
-        products: List[str],
-        ratelaw: str = "mass-action",
-    ) -> None:
-        if ratelaw == "mass-action":
-            k_fwd = f"kf_{rxn_id}"
-            k_bwd = f"kr_{rxn_id}"
-            mod.add_parameters({k_fwd: 1, k_bwd: 1})
-            mod.add_reaction_from_ratelaw(
-                rate_name=rxn_id,
-                ratelaw=rl.ReversibleMassAction(
-                    substrates=substrates,
-                    products=products,
-                    k_fwd=k_fwd,
-                    k_bwd=k_bwd,
-                ),
-            )
-        else:
-            raise NotImplementedError
+        mod, rxn_id, substrates, products, ratelaw="mass-action"
+    ):
+        k_fwd = f"kf_{rxn_id}"
+        k_bwd = f"kr_{rxn_id}"
+        mod.add_parameters({k_fwd: 1, k_bwd: 1})
+        mod.add_reaction_from_ratelaw(
+            rate_name=rxn_id,
+            ratelaw=rl.ReversibleMassAction(
+                substrates=substrates, products=products, k_fwd=k_fwd, k_bwd=k_bwd
+            ),
+        )
 
     @staticmethod
-    def _stoich_dict_to_list(stoich_dict: Dict[str, float], reaction: str) -> List[str]:
+    def _stoich_dict_to_list(stoich_dict, reaction):
         stoich_list = []
         for cpd, stoich in stoich_dict.items():
             if not stoich == int(stoich):
-                warnings.warn(f"Check stoichiometries for reaction {reaction}, possible integer rounddown.")
-            stoich_list.extend([cpd] * max(int(abs(stoich)), 1))
+                warnings.warn(
+                    f"Check stoichiometries for reaction {reaction}, possible integer rounddown."
+                )
+            stoich_list.extend([cpd] * int(abs(stoich)))
         return stoich_list
 
     def to_kinetic_model(
         self,
-        reaction_ratelaw: str = "mass-action",
-        influx_ratelaw: str = "constant",
-        efflux_ratelaw: str = "mass-action",
-    ) -> ode.Model:
-        """Convert the model into a kinetic modelbase model."""
+        reaction_ratelaw="mass-action",
+        influx_ratelaw="constant",
+        efflux_ratelaw="mass-action",
+    ):
+        """Convert the model into a kinetic modelbase model.
+
+        Returns
+        -------
+        modelbase.ode.Model
+        """
         mod = ode.Model()
         mod.add_compounds(sorted(self.compounds))
 
-        for rxn_id, reaction in sorted(self.reactions.items()):
-            _substrates, _products = reaction.split_stoichiometries()
-            substrates = self._stoich_dict_to_list(_substrates, reaction=rxn_id)
-            products = self._stoich_dict_to_list(_products, reaction=rxn_id)
-
-            if len(reaction.stoichiometries) == 1:
-                if reaction.reversible:
-                    self._add_modelbase_medium_reaction(
-                        mod=mod,
-                        rxn_id=rxn_id,
-                        metabolite=substrates,
-                        influx_ratelaw=influx_ratelaw,
-                        efflux_ratelaw=efflux_ratelaw,
-                    )
-                else:
-                    if reaction.bounds is not None and reaction.bounds[0] < 0:
-                        self._add_modelbase_influx_reaction(
+        for reaction in sorted(self.reactions.values()):
+            rxn_id = reaction.id
+            substrates, products = reaction._split_stoichiometries()
+            substrates = self._stoich_dict_to_list(substrates, reaction=rxn_id)
+            products = self._stoich_dict_to_list(products, reaction=rxn_id)
+
+            try:
+                if len(reaction.stoichiometries) == 1:
+                    if reaction.reversible:
+                        self._add_modelbase_medium_reaction(
                             mod=mod,
                             rxn_id=rxn_id,
                             metabolite=substrates,
-                            ratelaw=influx_ratelaw,
+                            influx_ratelaw=influx_ratelaw,
+                            efflux_ratelaw=efflux_ratelaw,
                         )
                     else:
-                        self._add_modelbase_efflux_reaction(
+                        if reaction.bounds[0] < 0:
+                            self._add_modelbase_influx_reaction(
+                                mod=mod,
+                                rxn_id=rxn_id,
+                                metabolite=substrates,
+                                ratelaw=influx_ratelaw,
+                            )
+                        else:
+                            self._add_modelbase_efflux_reaction(
+                                mod=mod,
+                                rxn_id=rxn_id,
+                                metabolite=substrates,
+                                ratelaw=efflux_ratelaw,
+                            )
+                else:
+                    if reaction.reversible:
+                        self._add_modelbase_reversible_reaction(
                             mod=mod,
                             rxn_id=rxn_id,
-                            metabolite=substrates,
-                            ratelaw=efflux_ratelaw,
+                            substrates=substrates,
+                            products=products,
+                            ratelaw=reaction_ratelaw,
                         )
-            else:
-                if reaction.reversible:
-                    self._add_modelbase_reversible_reaction(
-                        mod=mod,
-                        rxn_id=rxn_id,
-                        substrates=substrates,
-                        products=products,
-                        ratelaw=reaction_ratelaw,
-                    )
-                else:
-                    self._add_modelbase_irreversible_reaction(
-                        mod=mod,
-                        rxn_id=rxn_id,
-                        substrates=substrates,
-                        products=products,
-                        ratelaw=reaction_ratelaw,
-                    )
+                    else:
+                        self._add_modelbase_irreversible_reaction(
+                            mod=mod,
+                            rxn_id=rxn_id,
+                            substrates=substrates,
+                            products=products,
+                            ratelaw=reaction_ratelaw,
+                        )
+            except AttributeError:
+                warnings.warn(
+                    f"Could not find a suitable rate function for {rxn_id}. Skipping."
+                )
         return mod
 
-    def to_kinetic_model_source_code(
-        self,
-        reaction_ratelaw: str = "mass-action",
-        influx_ratelaw: str = "constant",
-        efflux_ratelaw: str = "mass-action",
-    ) -> str:
-        """Convert the model into modelbase model soure code."""
-        mod = self.to_kinetic_model(
-            reaction_ratelaw=reaction_ratelaw,
-            influx_ratelaw=influx_ratelaw,
-            efflux_ratelaw=efflux_ratelaw,
-        )
-        return mod.generate_model_source_code()  # type: ignore
+    def to_kinetic_model_source_code(self):
+        """Convert the model into modelbase model soure code.
+
+        Returns
+        -------
+        modelbase.ode.Model
+        """
+        mod = self.to_kinetic_model()
+        return mod.generate_model_source_code()
+
+    ##########################################################################
+    # SBML interface
+    ##########################################################################
+
+    def to_sbml(self, filename="model.sbml"):
+        """Export the model to sbml.
+
+        Parameters
+        ----------
+        filename : str
+        """
+        cobra_model = self.to_cobra()
+        for metabolite in cobra_model.metabolites:
+            metabolite.charge = int(metabolite.charge)
+        cobra.io.write_sbml_model(cobra_model=cobra_model, filename=filename)
 
     ##########################################################################
     # Blast interface
     ##########################################################################
 
-    def get_monomer_sequences(self, reaction_ids: Iterable[str]) -> Set[str]:
-        """Get monomer sequences from the given reaction_ids."""
+    def get_monomer_sequences(self, reaction_ids):
+        """Get all monomer sequences from the given reaction_ids.
+
+        Parameters
+        ----------
+        reaction_ids: Iterable(str)
+
+        Returns
+        -------
+        sequences: set
+            Sequences
+        """
         sequences = set()
         for reaction_id in reaction_ids:
-            for name, sequence in self.get_reaction_sequences(reaction_id).items():
+            reaction = self.reactions[reaction_id]
+            for name, sequence in reaction.sequences.items():
                 sequences.add(f">gnl|META|{name}\n{sequence}")
         return sequences
 
-    def get_all_monomer_sequences(self) -> Set[str]:
-        """Get monomer sequences of all reactions."""
-        return self.get_monomer_sequences(self.reactions.keys())
-
-    def blast_sequences_against_genome(
-        self, sequences: Iterable[str], genome_file: str | Path
-    ) -> pd.DataFrame:
-        genome_file = Path(genome_file)
+    def get_all_monomer_sequences(self):
+        """Get all monomer sequences for all Model reactions.
+
+        Returns
+        -------
+        sequences: set
+            Sequences
+        """
+        sequences = set()
+        for reaction in self.reactions.values():
+            for name, sequence in reaction.sequences.items():
+                sequences.add(f">gnl|META|{name}\n{sequence}")
+        return sequences
+
+    def blast_sequences(self, sequences, genome_file):
+        """Blast all given sequences against a given nucleotide genome.
+
+        Parameters
+        ----------
+        genome_file: str or pathlib.Path
+            A nucleotide fasta file containing the genome of the organism
+
+        Returns
+        -------
+        blast_monomers: pandas.DataFrame
+            Results of the blast algorithm
+        """
+        genome_file = pathlib.Path(genome_file)
         if not genome_file.is_file():
             raise FileNotFoundError(f"genome_file '{genome_file}' does not exist.")
-        return topological.tblastn_pipeline(sequences=sequences, genome_file=genome_file)
+        return topological.blast(sequences=sequences, genome_file=genome_file)
 
-    def blast_sequences_against_proteome(
-        self, sequences: Iterable[str], proteome_file: str | Path
-    ) -> pd.DataFrame:
-        proteome_file = Path(proteome_file)
-        if not proteome_file.is_file():
-            raise FileNotFoundError(f"proteome_file '{proteome_file}' does not exist.")
-        return topological.blastp_pipeline(sequences=sequences, proteome_file=proteome_file)
-
-    def blast_reactions_against_genome(
-        self, reaction_ids: Iterable[str], genome_file: str | Path
-    ) -> pd.DataFrame:
-        sequences = self.get_monomer_sequences(reaction_ids=reaction_ids)
-        return self.blast_sequences_against_genome(sequences=sequences, genome_file=genome_file)
+    def blast_reactions(self, reaction_ids, genome_file):
+        """Blast all given reactions against a given nucleotide genome.
 
-    def blast_reactions_against_proteome(
-        self, reaction_ids: Iterable[str], proteome_file: str | Path
-    ) -> pd.DataFrame:
+        Parameters
+        ----------
+        genome_file: str or pathlib.Path
+            A nucleotide fasta file containing the genome of the organism
+
+        Returns
+        -------
+        blast_monomers: pandas.DataFrame
+            Results of the blast algorithm
+        """
         sequences = self.get_monomer_sequences(reaction_ids=reaction_ids)
-        return self.blast_sequences_against_proteome(sequences=sequences, proteome_file=proteome_file)
+        return self.blast_sequences(sequences=sequences, genome_file=genome_file)
 
-    def blast_all_reactions_against_genome(self, genome_file: str | Path) -> pd.DataFrame:
-        sequences = self.get_all_monomer_sequences()
-        return self.blast_sequences_against_genome(sequences=sequences, genome_file=genome_file)
+    def blast_all_reactions(self, genome_file):
+        """Blast all reactions of the model against a given nucleotide genome.
+
+        Parameters
+        ----------
+        genome_file: str or pathlib.Path
+            A nucleotide fasta file containing the genome of the organism
 
-    def blast_all_reactions_against_proteome(self, proteome_file: str | Path) -> pd.DataFrame:
+        Returns
+        -------
+        blast_monomers: pandas.DataFrame
+            Results of the blast algorithm
+        """
         sequences = self.get_all_monomer_sequences()
-        return self.blast_sequences_against_proteome(sequences=sequences, proteome_file=proteome_file)
+        return self.blast_sequences(sequences=sequences, genome_file=genome_file)
 
-    ##########################################################################
-    # Build submodels from blast results
-    ##########################################################################
+    def _get_reactions_from_blast_results(
+        self, filtered_blast_monomers, require_all_complex_monomers
+    ):
+        """Get all model reactions from the filtered_blast_monomers.
+
+        Parameters
+        ----------
+        filtered_blast_monomers: set
+            Ids of the filtered blast monomers
+        require_all_complex_monomers: bool
+            Whether to require, that all monomers of an enzyme reaction
+            have to be found in order for that reaction to be encluded
+            in the new model
+
+        Returns
+        -------
+        blast_reactions: set
+            All the reaction_ids of the reactions that were found.
+        """
+        if require_all_complex_monomers:
+            blast_reactions = set()
+            for reaction in self.reactions.values():
+                for monomers in reaction.monomers.values():
+                    if monomers.issubset(filtered_blast_monomers):
+                        blast_reactions.add(reaction.id)
+            return blast_reactions
+        else:
+            blast_reactions = set()
+            for monomer in filtered_blast_monomers:
+                for reaction in self._monomers[monomer]:
+                    blast_reactions.add(reaction)
+            return blast_reactions
 
     def create_submodel_from_blast_monomers(
         self,
-        blast_monomers: pd.DataFrame,
-        name: str | None = None,
-        max_evalue: float = 1e-6,
-        min_coverage: float = 85,
-        min_pident: float = 85,
-        prefix_remove: str = r"gnl\|.*?\|",
-        suffix_remove: str | None = None,
-    ) -> "Model":
-        """Create a submodel from given blast results."""
-        filtered_blast_monomers = topological.filter_blast_results(
+        blast_monomers,
+        name=None,
+        max_evalue=1e-6,
+        min_coverage=85,
+        min_pident=85,
+        require_all_complex_monomers=True,
+        prefix_remove=r"gnl\|.*?\|",
+        suffix_remove=None,
+    ):
+        """Create a submodel from given blast results.
+
+        This reads in blast monomers as obtained by blast_sequences
+        or blast_reactions and filters them according to the
+        given quality criteria.
+
+        Parameters
+        ----------
+        genome_file: str or pathlib.Path
+            A nucleotide fasta file containing the genome of the organism
+        max_evalue: float
+            Upper boundary for accepted Expect value
+        min_coverage: float
+            Lower boundary for accepted Query Coverage Per Subject
+        min_pident: float
+            Lower boundary for accepted Percentage of identical matches
+        prefix_remove: raw_string
+            Regular expression for a prefix to be removed ('^' is added automatically)
+        suffix_remove: raw_string
+            Regular expression for a suffix to be removed ('$' is added automatically)
+
+        For a deeper explanation of the quality criteria
+        (evalue, converage and pident) please consult the NCBI blast manual.
+
+        Returns
+        -------
+        submodel: moped.Model
+        """
+        blast_monomers = topological.filter_blast_results(
             blast_monomers=blast_monomers,
             max_evalue=max_evalue,
             min_coverage=min_coverage,
             min_pident=min_pident,
             prefix_remove=prefix_remove,
             suffix_remove=suffix_remove,
         )
-        blast_reactions: Dict[str, int] = dict()
-        for reaction in self.reactions.values():
-            for i, monomers in enumerate(reaction.gpr_annotation):
-                if monomers.issubset(filtered_blast_monomers):
-                    blast_reactions[reaction.id] = i
-                    break
-        submodel = self.create_submodel(reaction_ids=blast_reactions, name=name)
-        for rxn_id, enzrxn in blast_reactions.items():
-            submodel.reactions[rxn_id]._gpa = enzrxn
-        return submodel
+        blast_reactions = self._get_reactions_from_blast_results(
+            filtered_blast_monomers=blast_monomers,
+            require_all_complex_monomers=require_all_complex_monomers,
+        )
+        return self.create_submodel(reaction_ids=blast_reactions, name=name)
+
+    def create_submodel_from_sequences(
+        self,
+        sequences,
+        genome_file,
+        name=None,
+        max_evalue=1e-6,
+        min_coverage=85,
+        min_pident=85,
+        require_all_complex_monomers=True,
+        prefix_remove=r"gnl\|.*?\|",
+        suffix_remove=None,
+        cache_blast_results=False,
+    ):
+        """Create a submodel from given protein monomer sequences and a nucleotide genome.
+
+        This blasts all given protein monomer sequences against
+        the nucleotide database and then checks which reactions
+        can be found in that genome. The subset that can be found
+        will be returned as a new model.
 
-    def create_submodel_from_sequences_and_genome(
-        self,
-        sequences: Iterable[str],
-        genome_file: str | Path,
-        name: str | None = None,
-        max_evalue: float = 1e-6,
-        min_coverage: float = 85,
-        min_pident: float = 85,
-        prefix_remove: str = r"gnl\|.*?\|",
-        suffix_remove: str = None,
-        cache_blast_results: bool = False,
-    ) -> "Model":
+        Parameters
+        ----------
+        genome_file: str or pathlib.Path
+            A nucleotide fasta file containing the genome of the organism
+        max_evalue: float
+            Upper boundary for accepted Expect value
+        min_coverage: float
+            Lower boundary for accepted Query Coverage Per Subject
+        min_pident: float
+            Lower boundary for accepted Percentage of identical matches
+        prefix_remove: raw_string
+            Regular expression for a prefix to be removed ('^' is added automatically)
+        suffix_remove: raw_string
+            Regular expression for a suffix to be removed ('$' is added automatically)
+
+        For a deeper explanation of the quality criteria
+        (evalue, converage and pident) please consult the NCBI blast manual.
+
+        Returns
+        -------
+        submodel: moped.Model
+        """
         if cache_blast_results:
             if name is None:
                 raise ValueError("Name has to be given in order to cache results")
-            blast_file = get_temporary_directory(subdirectory="blast") / f"blast_genome_monomers_{name}.csv"
+            blast_file = (
+                get_temporary_directory(subdirectory="blast")
+                / f"blast_monomers_{name}.csv"
+            )
             if blast_file.is_file():
                 blast_monomers = pd.read_csv(blast_file, index_col=0)
             else:
-                print(f"Caching results to {blast_file}")
-                blast_monomers = self.blast_sequences_against_genome(
+                blast_monomers = self.blast_sequences(
                     sequences=sequences, genome_file=genome_file
                 )
                 blast_monomers.to_csv(blast_file)
         else:
-            blast_monomers = self.blast_sequences_against_genome(sequences=sequences, genome_file=genome_file)
+            blast_monomers = self.blast_sequences(
+                sequences=sequences, genome_file=genome_file
+            )
         return self.create_submodel_from_blast_monomers(
             blast_monomers=blast_monomers,
             name=name,
             max_evalue=max_evalue,
             min_coverage=min_coverage,
             min_pident=min_pident,
+            require_all_complex_monomers=require_all_complex_monomers,
             prefix_remove=prefix_remove,
             suffix_remove=suffix_remove,
         )
 
     def create_submodel_from_genome(
         self,
-        genome_file: str | Path,
-        name: str | None = None,
-        max_evalue: float = 1e-6,
-        min_coverage: float = 85,
-        min_pident: float = 85,
-        prefix_remove: str = r"gnl\|.*?\|",
-        suffix_remove: str = None,
-        cache_blast_results: bool = False,
-    ) -> "Model":
-        return self.create_submodel_from_sequences_and_genome(
-            self.get_all_monomer_sequences(),
-            genome_file=genome_file,
-            name=name,
-            max_evalue=max_evalue,
-            min_coverage=min_coverage,
-            min_pident=min_pident,
-            prefix_remove=prefix_remove,
-            suffix_remove=suffix_remove,
-            cache_blast_results=cache_blast_results,
-        )
+        genome_file,
+        name=None,
+        max_evalue=1e-6,
+        min_coverage=85,
+        min_pident=85,
+        require_all_complex_monomers=True,
+        prefix_remove=r"gnl\|.*?\|",
+        suffix_remove=None,
+        cache_blast_results=False,
+    ):
+        """Create a submodel from a given nucleotide genome.
+
+        This blasts all protein monomers of the model against
+        the nucleotide database and then checks which reactions
+        can be found in that genome. The subset that can be found
+        will be returned as a new model.
 
-    def create_submodel_from_sequences_and_proteome(
-        self,
-        sequences: Iterable[str],
-        proteome_file: str | Path,
-        name: str | None = None,
-        max_evalue: float = 1e-6,
-        min_coverage: float = 85,
-        min_pident: float = 85,
-        prefix_remove: str = r"gnl\|.*?\|",
-        suffix_remove: str = None,
-        cache_blast_results: bool = False,
-    ) -> "Model":
-        if cache_blast_results:
-            if name is None:
-                raise ValueError("Name has to be given in order to cache results")
-            blast_file = get_temporary_directory(subdirectory="blast") / f"blast_proteome_monomers_{name}.csv"
-            if blast_file.is_file():
-                blast_monomers = pd.read_csv(blast_file, index_col=0)
-            else:
-                print(f"Caching results to {blast_file}")
-                blast_monomers = self.blast_sequences_against_proteome(
-                    sequences=sequences, proteome_file=proteome_file
-                )
-                blast_monomers.to_csv(blast_file)
-        else:
-            blast_monomers = self.blast_sequences_against_proteome(
-                sequences=sequences, proteome_file=proteome_file
-            )
-        return self.create_submodel_from_blast_monomers(
-            blast_monomers=blast_monomers,
-            name=name,
-            max_evalue=max_evalue,
-            min_coverage=min_coverage,
-            min_pident=min_pident,
-            prefix_remove=prefix_remove,
-            suffix_remove=suffix_remove,
-        )
+        Parameters
+        ----------
+        genome_file: str or pathlib.Path
+            A nucleotide fasta file containing the genome of the organism
+        max_evalue: float
+            Upper boundary for accepted Expect value
+        min_coverage: float
+            Lower boundary for accepted Query Coverage Per Subject
+        min_pident: float
+            Lower boundary for accepted Percentage of identical matches
+        prefix_remove: raw_string
+            Regular expression for a prefix to be removed ('^' is added automatically)
+        suffix_remove: raw_string
+            Regular expression for a suffix to be removed ('$' is added automatically)
 
-    def create_submodel_from_proteome(
-        self,
-        proteome_file: str | Path,
-        name: str | None = None,
-        max_evalue: float = 1e-6,
-        min_coverage: float = 85,
-        min_pident: float = 85,
-        prefix_remove: str = r"gnl\|.*?\|",
-        suffix_remove: str = None,
-        cache_blast_results: bool = False,
-    ) -> "Model":
-        return self.create_submodel_from_sequences_and_proteome(
-            self.get_all_monomer_sequences(),
-            proteome_file=proteome_file,
+        For a deeper explanation of the quality criteria
+        (evalue, converage and pident) please consult the NCBI blast manual.
+
+        Returns
+        -------
+        submodel: moped.Model
+        """
+        sequences = self.get_all_monomer_sequences()
+        return self.create_submodel_from_sequences(
+            sequences=sequences,
+            genome_file=genome_file,
             name=name,
             max_evalue=max_evalue,
             min_coverage=min_coverage,
             min_pident=min_pident,
+            require_all_complex_monomers=require_all_complex_monomers,
             prefix_remove=prefix_remove,
             suffix_remove=suffix_remove,
             cache_blast_results=cache_blast_results,
         )
-
-    ##########################################################################
-    # Serde
-    ##########################################################################
-
-    def to_sbml(self, filename: str | Path = "model.sbml") -> None:
-        """Export the model to sbml."""
-        doc = _export_model(model=self)
-        libsbml.writeSBMLToFile(doc, filename=str(filename))
-
-    def to_pickle(self, filename: str | Path) -> None:
-        with open(filename, "wb") as file:
-            pickle.dump(self, file)
-
-    def to_json(self, filename: str | Path) -> None:
-        from ..utils.serialize import serialize
-
-        with open(filename, "w") as file:
-            json.dump(serialize(self), file, indent=2)
-
-    def to_yaml(self, filename: str | Path) -> None:
-        from ..utils.serialize import serialize
-
-        with open(filename, "w") as file:
-            yaml.dump(serialize(self), file)
-
-    @staticmethod
-    def load_from_pickle(filename: str | Path) -> "Model":
-        with open(filename, "rb") as file:
-            model = pickle.load(file)
-        if isinstance(model, Model):
-            return model
-        raise NotImplementedError("Pickled object is not a Model")
-
-    @staticmethod
-    def load_from_json(filename: str | Path) -> "Model":
-        with open(filename, "r") as file:
-            obj = json.load(file)
-        return _deserialize(obj)
-
-    @staticmethod
-    def load_from_yaml(filename: str | Path) -> "Model":
-        with open(filename, "r") as file:
-            obj = yaml.safe_load(file)
-        return _deserialize(obj)
-
-
-def _deserialize_compounds(obj: Dict[str, Any]) -> list[Compound]:
-    return [
-        Compound(
-            base_id=str(i["base_id"]),
-            id=str(i["id"]),
-            name=str(i["name"]),
-            compartment=str(i["compartment"]),
-            smiles=str(i["smiles"]),
-            formula={str(k): float(v) for k, v in i["formula"].items()},
-            charge=int(charge) if (charge := i["charge"]) is not None else None,
-            gibbs0=float(gibbs0) if (gibbs0 := i["gibbs0"]) is not None else None,
-            database_links={str(k): set(v) for k, v in i["database_links"].items()},
-            types=list(i["types"]),
-            in_reaction=set(i["in_reaction"]),
-        )
-        for i in obj["compounds"]
-    ]
-
-
-def _deserialize_reactions(obj: Dict[str, Any]) -> list[Reaction]:
-    return [
-        Reaction(
-            base_id=str(i["base_id"]),
-            id=str(i["id"]),
-            name=str(name) if (name := i["name"]) is not None else None,
-            compartment=str(comp)
-            if isinstance(comp := i["compartment"], str)
-            else tuple(str(x) for x in comp),
-            bounds=(float(i["bounds"][0]), float(i["bounds"][1])),
-            gibbs0=float(gibbs0) if (gibbs0 := i["gibbs0"]) is not None else None,
-            ec=i["ec"],
-            transmembrane=i["transmembrane"] == "True",
-            types=list(i["types"]),
-            pathways=set(i["pathways"]),
-            stoichiometries={k: float(v) for k, v in i["stoichiometries"].items()},
-            gpr_annotation=[set(v) for v in i["gpr_annotation"]],
-            kinetic_data={k: KineticData(**v) for k, v in i["kinetic_data"].items()},
-            database_links={k: set(v) for k, v in i["database_links"].items()},
-        )
-        for i in obj["reactions"]
-    ]
-
-
-def _deserialize(obj: Dict[str, Any]) -> Model:
-    return Model(
-        compounds=_deserialize_compounds(obj),
-        reactions=_deserialize_reactions(obj),
-        compartments=obj["compartments"],
-        objective=obj["objective"],
-        minimal_seed=set(obj["minimal_seed"]),
-        name=obj["name"],
-        cofactor_pairs=obj["base_cofactor_pairs"],
-    )
```

### Comparing `moped-1.9.9/src/moped/topological/blast.py` & `moped-1rc1/moped/topological/blast.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,88 @@
-from __future__ import annotations
+"""NCBI Blast interface."""
+
 
-import functools
-import io
-import multiprocessing
 import subprocess
+import pathlib
+import pandas as pd
+import multiprocessing
+import io
 import sys
+import functools
 from collections.abc import Iterable
-from pathlib import Path
-from typing import Set
-
-import pandas as pd
 
 from ..utils import get_temporary_directory
 
-__all__ = [
-    "tblastn_pipeline",
-    "blastp_pipeline",
-    "filter_blast_results",
-]
-
 TEMP_DIR = get_temporary_directory(subdirectory="blast")
 
 
-def _generate_blast_genome_database(genome_file: Path) -> None:
+def _generate_blast_database(genome_file):
     """Generate a blast database from a given nucleotide fasta file.
 
     The generates files are stored in a temporary directory.
+
+    Attributes
+    ----------
+    genome_file: fasta file
+        Nucleotide fasta file
     """
     subprocess.run(
         [
             "makeblastdb",
             "-in",
             genome_file,
             "-parse_seqids",
             "-blastdb_version",
             "5",
             "-dbtype",
             "nucl",
             "-out",
-            TEMP_DIR / f"{genome_file.stem}",
+            TEMP_DIR / genome_file.stem,
         ]
     )
 
 
-def _generate_blast_proteome_database(proteome_file: Path) -> None:
-    """Generate a blast database from a given proteome fasta file.
-
-    The generates files are stored in a temporary directory.
-    """
-    subprocess.run(
-        [
-            "makeblastdb",
-            "-in",
-            proteome_file,
-            "-parse_seqids",
-            "-blastdb_version",
-            "5",
-            "-dbtype",
-            "prot",
-            "-out",
-            TEMP_DIR / f"{proteome_file.stem}",
-        ]
-    )
-
-
-def _unify_inputs(sequences: str | Path | Iterable[str], tempfiles: list[Path]) -> Path:
+def _unify_inputs(sequences, tempfiles):
     """Unify the different inputs for the blast method.
 
     Will create temporary files, if sequences is not a file
 
     Attributes
     ----------
     sequences: str, Iterable(str), file_path
         Inputs
     tempfiles: list
         list to keep track of all created files
 
     Returns
     -------
-    file: Path
+    file: pathlib.Path
     """
-    file: Path
     if isinstance(sequences, str):
         if sequences.startswith(">"):
             file = TEMP_DIR / "blast_input.fasta"
             with open(file, "w+") as f:
                 f.write(sequences)
             tempfiles.append(file)
         else:
-            file = Path(sequences)
+            file = pathlib.Path(sequences)
     elif isinstance(sequences, Iterable):
         file = TEMP_DIR / "blast_input.fasta"
         with open(file, "w+") as f:
             for sequence in sequences:
                 f.write(sequence + "\n")
         tempfiles.append(file)
-    elif isinstance(sequences, Path):
+    elif isinstance(sequences, pathlib.Path):
         file = sequences
     else:
         raise TypeError(f"Unsupported type {type(sequences)}")
     return file
 
 
-def _split_input_files(file_path: Path, n_cores: int, temporary_files: list[Path]) -> list[Path]:
+def _split_input_files(file_path, n_cores, temporary_files):
     """Split the input file into multiple files to enable multiprocessing with blast.
 
     Attributes
     ----------
     file_path
         Path to the input file
     n_cores: int
@@ -137,21 +113,20 @@
                         )
                     ]
                 )
             )
     return files
 
 
-def _run_tblastn(query_file_path: str | Path, database_name: str) -> str:
-    """Protein Query-Translated Subject BLAST (aligns proteins with
-    translated DNA)
+def _run_blast_process(query_file_path, database_name):
+    """Run blast software (helper function).
 
     Attributes
     ----------
-    query_file_path: str or Path
+    query_file_path: str or pathlib.Path
         Path of the query file
 
     Returns
     -------
     matches: str
         Outputs the matches in a tsv table format as a multiline-string
     """
@@ -169,113 +144,31 @@
         stderr=subprocess.PIPE,
     )
     if out.returncode != 0:
         raise ValueError(f"Process failed: {out.stderr.decode('utf-8')}")
     return out.stdout.decode("utf-8")
 
 
-def _run_blastp(query_file_path: str | Path, database_name: str) -> str:
-    """Search protein database using a protein query
-
-    Attributes
-    ----------
-    query_file_path: str or Path
-        Path of the query file
-
-    Returns
-    -------
-    matches: str
-        Outputs the matches in a tsv table format as a multiline-string
-    """
-    out = subprocess.run(
-        [
-            "blastp",
-            "-db",
-            TEMP_DIR / database_name,
-            "-query",
-            query_file_path,
-            "-outfmt",
-            "6 qseqid sseqid evalue pident qcovs",
-        ],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-    )
-    if out.returncode != 0:
-        raise ValueError(f"Process failed: {out.stderr.decode('utf-8')}")
-    return out.stdout.decode("utf-8")
-
-
-def _read_blast_results(results: str) -> pd.DataFrame:
+def _read_blast_results(results):
     """Transform blast csv result to pandas df."""
-    df = (
-        pd.read_csv(
-            io.StringIO(results),
-            sep="\t",
-            header=None,  # type: ignore
-            names=["Monomer", "qseqid", "evalue", "pident", "qcovs"],
-        )
-        .sort_values(by=["Monomer", "evalue"])
-        .set_index("Monomer", drop=True)
+    results = pd.read_csv(
+        io.StringIO(results),
+        sep="\t",
+        header=None,
+        names=["Monomer", "qseqid", "evalue", "pident", "qcovs"],
     )
-    return df[~df.index.duplicated(keep="first")]
-
-
-def tblastn_pipeline(
-    sequences: str | Path | Iterable[str],
-    genome_file: Path,
-    multiple_cores: bool = True,
-) -> pd.DataFrame:
-    """Blast protein sequences against a genome.
-
-    If multiple matches for a monomer are found, only the one
-    with the lowest e-value is returned.
-
-    Attributes
-    ----------
-    sequences: str, Iterable(str), file_path
-        Input protein sequences
-    genome_file: file
-        Nucleotide fasta file
-    multiple_cores: bool
-        Whether to utilize multiprocessing. On Windows this is always disabled
-
-    Returns
-    -------
-    matches: pandas.DataFrame
-        The matches sorted by their monomer ID
-    """
-    temporary_files: list[Path] = []
-    genome_fp = Path(genome_file)
-
-    _generate_blast_genome_database(genome_file=genome_file)
-    file_path = _unify_inputs(sequences, temporary_files)
-    partial_blast = functools.partial(_run_tblastn, **{"database_name": genome_fp.stem})
-
-    if not multiple_cores or sys.platform in ["win32", "cygwin"]:
-        results = partial_blast(file_path)
-    else:
-        n_cores = multiprocessing.cpu_count()
-        files = _split_input_files(file_path, n_cores, temporary_files)
-        pool = multiprocessing.Pool(n_cores)
-        results = "\n".join(pool.map(partial_blast, files))
-        pool.close()
-    results = _read_blast_results(results=results)
-
-    # Delete temporary files
-    for file in temporary_files:
-        file.unlink()
+    # Only keep results with lowest e-value
+    results = results.sort_values(by=["Monomer", "evalue"])
+    results = results.set_index("Monomer", drop=True)
+    results = results[~results.index.duplicated(keep="first")]
     return results
 
 
-def blastp_pipeline(
-    sequences: str | Path | Iterable[str],
-    proteome_file: Path,
-    multiple_cores: bool = True,
-) -> pd.DataFrame:
-    """Blast protein sequences against a proteome.
+def blast(sequences, genome_file, multiple_cores=True):
+    """Blast protein sequences against a genome.
 
     If multiple matches for a monomer are found, only the one
     with the lowest e-value is returned.
 
     Attributes
     ----------
     sequences: str, Iterable(str), file_path
@@ -286,20 +179,22 @@
         Whether to utilize multiprocessing. On Windows this is always disabled
 
     Returns
     -------
     matches: pandas.DataFrame
         The matches sorted by their monomer ID
     """
-    temporary_files: list[Path] = []
-    proteome_filepath = Path(proteome_file)
+    temporary_files = []
+    genome_file = pathlib.Path(genome_file)
 
-    _generate_blast_proteome_database(proteome_file=proteome_file)
+    _generate_blast_database(genome_file=genome_file)
     file_path = _unify_inputs(sequences, temporary_files)
-    partial_blast = functools.partial(_run_blastp, **{"database_name": proteome_filepath.stem})
+    partial_blast = functools.partial(
+        _run_blast_process, **{"database_name": genome_file.stem}
+    )
 
     if not multiple_cores or sys.platform in ["win32", "cygwin"]:
         results = partial_blast(file_path)
     else:
         n_cores = multiprocessing.cpu_count()
         files = _split_input_files(file_path, n_cores, temporary_files)
         pool = multiprocessing.Pool(n_cores)
@@ -310,21 +205,16 @@
     # Delete temporary files
     for file in temporary_files:
         file.unlink()
     return results
 
 
 def filter_blast_results(
-    blast_monomers: pd.DataFrame,
-    max_evalue: float,
-    min_coverage: float,
-    min_pident: float,
-    prefix_remove: str | None,
-    suffix_remove: str | None,
-) -> Set[str]:
+    blast_monomers, max_evalue, min_coverage, min_pident, prefix_remove, suffix_remove,
+):
     """Filter the blast results to remove matches that do not match the quality criteria.
 
     Also optionally removes a prefix and suffix (given as regular expressions).
 
     For explanations for the quality criteria please consult the NCBI blast
     manual.
```

### Comparing `moped-1.9.9/src/moped/topological/gapfilling.py` & `moped-1rc1/moped/topological/gapfilling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 """Gapfilling functions. Mostly a meneco interface."""
-from __future__ import annotations
 
+import pyasp
 import warnings
-from typing import TYPE_CHECKING, Iterable, List, cast
+from collections.abc import Iterable
 
-import pyasp
 from __meneco__ import query, utils
 
-if TYPE_CHECKING:
-    from ..core.model import Model
-
-__all__ = ["gapfilling"]
 
-
-def model_to_termset(model: "Model", model_name: str) -> pyasp.TermSet:
+def model_to_termset(model, model_name):
     """Convert a moped model into a meneco termset.
 
     Parameters
     ----------
     model: moped.Model
     model_name: str
 
     Returns
     -------
     model_terms: pyasp.term.TermSet
         Converted model
     """
     model_terms = pyasp.TermSet()
     for reaction in model.reactions.values():
-        model_terms.add(pyasp.Term("reaction", ['"' + reaction.id + '"', '"' + model_name + '"']))
-        substrates, products = reaction.split_stoichiometries()
+        model_terms.add(
+            pyasp.Term("reaction", ['"' + reaction.id + '"', '"' + model_name + '"'])
+        )
+        substrates, products = reaction._split_stoichiometries()
         for substrate in substrates:
             model_terms.add(
                 pyasp.Term(
                     "reactant",
                     [
                         '"' + substrate + '"',
                         '"' + reaction.id + '"',
@@ -51,15 +47,15 @@
                         '"' + model_name + '"',
                     ],
                 )
             )
     return model_terms
 
 
-def compound_id_to_term(compound_type: str, compound_id: str) -> pyasp.Term:
+def compound_id_to_term(compound_type, compound_id):
     """Convert a moped compound into a meneco termset.
 
     Parameters
     ----------
     compound_type: str
         E.g. reactant, product, target
     compound_id: str
@@ -68,15 +64,15 @@
     -------
     compound_term: pyasp.Term
         Converted compound
     """
     return pyasp.Term(compound_type, ['"' + compound_id + '"'])
 
 
-def compound_list_to_termset(compound_type: str, compound_iterable: Iterable[str]) -> pyasp.TermSet:
+def compound_list_to_termset(compound_type, compound_iterable):
     """Convert a moped compound list into a meneco termset.
 
     Parameters
     ----------
     compound_type: str
         E.g. reactant, product, target
     compound_iterable: Iterable(str)
@@ -88,45 +84,38 @@
     """
     terms = pyasp.TermSet()
     for compound_id in compound_iterable:
         terms.add(compound_id_to_term(compound_type, compound_id))
     return terms
 
 
-def get_unproducible_compounds(
-    model: pyasp.TermSet, targets: Iterable[str], seed: Iterable[str]
-) -> pyasp.TermSet:
+def get_unproducible_compounds(model, targets, seed):
     """Get compounds that are not producible given the model and seed compounds.
 
     Parameters
     ----------
     model: pyasp.term.TermSet
     targets: Iterable(str)
         Compounds to be produced
     seed: Iterable(str)
         Compounds with which the algorithm starts
 
     Returns
     -------
     unproducible_compounds: pyasp.TermSet
     """
-    return pyasp.TermSet(
+    return pyasp.term.TermSet(
         [
             compound_id_to_term("target", i.arg(0).strip('"'))
             for i in query.get_unproducible(model, targets, seed)
         ]
     )
 
 
-def get_essential_reactions(
-    model: pyasp.TermSet,
-    database: pyasp.TermSet,
-    seed: Iterable[str],
-    producible: Iterable[str],
-) -> pyasp.TermSet:
+def get_essential_reactions(model, database, seed, producible):
     """Get essential reactions to produce the producible reactions.
 
     Parameters
     ----------
     model: pyasp.term.TermSet
     database: pyasp.term.TermSet
         All possible reactions
@@ -136,45 +125,42 @@
         Compounds that can be produced in the database
 
     Returns
     -------
     essential_reactions: pyasp.TermSet
         All reactions that are essential to produce the producible reactions
     """
-    essential_reactions: pyasp.TermSet = pyasp.TermSet()
+    essential_reactions = pyasp.TermSet()
     for target in producible:
         single_target = pyasp.TermSet()
         single_target.add(target)
-        essentials = query.get_intersection_of_completions(model, database, seed, single_target)
-        essential_reactions = cast(pyasp.TermSet, essential_reactions.union(essentials))
+        essentials = query.get_intersection_of_completions(
+            model, database, seed, single_target
+        )
+        essential_reactions = essential_reactions.union(essentials)
     return essential_reactions
 
 
-def term_to_str(term: pyasp.Term) -> str:
+def term_to_str(term):
     """Convert a pyasp term to a Python string.
 
     Parameters
     ----------
     term: pyasp.Term
 
     Returns
     -------
     term_str: str
     """
-    return term.arg(0).strip('"')  # type: ignore
+    return term.arg(0).strip('"')
 
 
 def gapfilling(
-    model: "Model",
-    reference_model: "Model",
-    seed: Iterable[str],
-    targets: Iterable[str],
-    include_weak_cofactors: bool = False,
-    verbose: bool = False,
-) -> List[str]:
+    model, reference_model, seed, targets, include_weak_cofactors=False, verbose=False
+):
     """Gap-filling using the meneco package.
 
     Parameters
     ----------
     model: moped.Model
     reference_model: moped.Model
     seed: List[str]
@@ -208,30 +194,38 @@
     db_terms = model_to_termset(reference_model, "repair")
 
     seed = compound_list_to_termset("seed", seed)
     targets = compound_list_to_termset("target", targets)
 
     unproducible_model = get_unproducible_compounds(model_terms, targets, seed)
     if verbose:
-        print(f"Searching for {[term_to_str(p) for p in unproducible_model]} in reference database")
+        print(
+            f"Searching for {[term_to_str(p) for p in unproducible_model]} in reference database"
+        )
     unproducible_database = get_unproducible_compounds(db_terms, targets, seed)
     producible = unproducible_model.difference(unproducible_database)
 
     if len(unproducible_database) > 0:
         warnings.warn(
             f"Could not produce {[term_to_str(p) for p in unproducible_database]} in reference database"
         )
         if verbose:
-            print(f"Could produce {[term_to_str(p) for p in producible]} in reference database")
+            print(
+                f"Could produce {[term_to_str(p) for p in producible]} in reference database"
+            )
     else:
         if verbose:
             print("Could produce all compounds in reference database")
 
-    essential_reactions = get_essential_reactions(model_terms, db_terms, seed, producible)
+    essential_reactions = get_essential_reactions(
+        model_terms, db_terms, seed, producible
+    )
     if verbose:
         print(f"Found {len(essential_reactions)} essential reaction(s)")
     filled_model = pyasp.TermSet(model_terms.union(essential_reactions))
     utils.clean_up()
 
     # Get minimal solution
-    min_models = query.get_minimal_completion_size(filled_model, db_terms, seed, producible)
+    min_models = query.get_minimal_completion_size(
+        filled_model, db_terms, seed, producible
+    )
     return [term_to_str(term) for term in min_models[0]]
```

### Comparing `moped-1.9.9/src/moped/topological/scope.py` & `moped-1rc1/moped/topological/scope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 """Scope algorithm interace."""
-from __future__ import annotations
 
-import itertools
 import sys
-from collections.abc import Iterable
-from functools import partial
-from multiprocessing import Pool, cpu_count
-from typing import TYPE_CHECKING, Dict, Set, Tuple
+import itertools
 
-if TYPE_CHECKING:
-    from ..core.model import Model
+from multiprocessing import Pool, cpu_count
 
-__all__ = [
-    "scope",
-    "multiple_scopes",
-]
+# from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from functools import partial
+from collections.abc import Iterable
 
 
-def split_stoichiometries(
-    model: Model,
-) -> Dict[str, Dict[str, Dict[str, float]]]:
+def _split_stoichiometries(model):
     """Split reaction stoichiometries into substrates and products.
 
     This is done to have the sets of either substrates and products
     to run the scope algorithm smoothly, e.g. comparing if substrates
     are a subset of the seed.
 
     Parameters
@@ -36,23 +27,20 @@
         Mapping of reaction ids to their substrates and products
     """
     reactions = {}
     for reaction_id, rxn in model.reactions.items():
         # Exclude medium reactions
         if len(rxn.stoichiometries) == 1:
             continue
-        substrates, products = rxn.split_stoichiometries()
-        reactions[reaction_id] = {
-            "substrates": substrates,
-            "products": products,
-        }
+        substrates, products = rxn._split_stoichiometries()
+        reactions[reaction_id] = {"substrates": substrates, "products": products}
     return reactions
 
 
-def _create_seed_set(seed: str | Iterable[str], model: Model, include_weak_cofactors: bool) -> Set[str]:
+def _create_seed_set(seed, model, include_weak_cofactors):
     """Check the user seed input and unify it to be a set.
 
     Parameters
     ----------
     seed: str, Iterable(str)
     model: moped.Model
     include_weak_cofactors: bool
@@ -68,21 +56,15 @@
         raise TypeError("Initial seed has to be str or Iterable[str]")
     seed = set(seed)
     if include_weak_cofactors:
         seed = seed.union(set(model.get_weak_cofactor_duplications()))
     return seed
 
 
-def _scope(
-    seed: str | Iterable[str],
-    model: Model,
-    reactions: Dict[str, Dict[str, Dict[str, float]]],
-    include_weak_cofactors: bool,
-    return_lumped_results: bool,
-) -> Tuple[Set[str], Set[str]] | Tuple[list[Set[str]], list[Set[str]]]:
+def _scope(seed, model, reactions, include_weak_cofactors, return_lumped_results):
     """Run the scope algorithm.
 
     This function is called by both scope and multiple_scopes to actually run
     the algorithm.
 
     Parameters
     ----------
@@ -98,28 +80,32 @@
         round or whether all the rounds should be lumped together.
 
     Returns
     -------
     scope_reactions: list(set) or set
     scope_compounds: list(set) or set
     """
-    seed = _create_seed_set(seed=seed, model=model, include_weak_cofactors=include_weak_cofactors)
+    seed = _create_seed_set(
+        seed=seed, model=model, include_weak_cofactors=include_weak_cofactors
+    )
     all_compounds = seed.copy()
     scope_reactions = []
     scope_compounds = []
     possible_reactions = set(reactions)
     while True:
-        new_reactions: Set[str] = set()
-        new_compounds: Set[str] = set()
+        new_reactions = set()
+        new_compounds = set()
         reactions_to_remove = set()
         for reaction in possible_reactions:
             if set(reactions[reaction]["substrates"]).issubset(all_compounds):
                 reactions_to_remove.add(reaction)
                 new_reactions.add(reaction)
-                new_compounds = new_compounds.union(set(reactions[reaction]["products"]))
+                new_compounds = new_compounds.union(
+                    set(reactions[reaction]["products"])
+                )
         if len(new_reactions) > 0:
             # Remove duplicate compounds
             new_compounds = new_compounds.difference(all_compounds)
             scope_reactions.append(new_reactions)
             scope_compounds.append(new_compounds)
             # Update iterables
             all_compounds = all_compounds.union(new_compounds)
@@ -129,20 +115,15 @@
                 return (
                     set(itertools.chain.from_iterable(scope_reactions)),
                     set(itertools.chain.from_iterable(scope_compounds)),
                 )
             return scope_reactions, scope_compounds
 
 
-def scope(
-    model: Model,
-    seed: Iterable[str],
-    include_weak_cofactors: bool,
-    return_lumped_results: bool,
-) -> Tuple[Set[str], Set[str]] | Tuple[list[Set[str]], list[Set[str]]]:
+def scope(model, seed, include_weak_cofactors, return_lumped_results):
     """Run the scope algorithm.
 
     Parameters
     ----------
     seed: set
     model: moped.Model
     include_weak_cofactors: bool
@@ -151,32 +132,28 @@
     return_lumped_results: bool
         Whether to return the results separated by the simulation
         round or whether all the rounds should be lumped together.
 
     Raises
     ------
     ValueError
-        If initial_seed is not str or List[str]
+        If initial_seed is not str or list[str]
     """
     return _scope(
         seed=seed,
         model=model,
-        reactions=split_stoichiometries(model),
+        reactions=_split_stoichiometries(model),
         include_weak_cofactors=include_weak_cofactors,
         return_lumped_results=return_lumped_results,
     )
 
 
 def multiple_scopes(
-    model: Model,
-    seeds: Iterable[Iterable[str]],
-    include_weak_cofactors: bool,
-    return_lumped_results: bool,
-    multiprocessing: bool,
-) -> Dict[tuple, Tuple[Set[str], Set[str]] | Tuple[list[Set[str]], list[Set[str]]]]:
+    model, seeds, include_weak_cofactors, return_lumped_results, multiprocessing
+):
     """Run the scope algorithm for multiple seeds.
 
     Parameters
     ----------
     seed: set
     model: moped.Model
     include_weak_cofactors: bool
@@ -189,31 +166,29 @@
         Whether to utilize multiple processes for the calculation.
         This is always disabled for Windows os, as the multiprocessing
         tends to misbehave in those cases
 
     Raises
     ------
     ValueError
-        If initial_seed is not str or List[str]
+        If initial_seed is not str or list[str]
 
     Returns
     -------
     seeds: dict
         Dict mapping the seeds against the results. See return_lumped_results
         for the exact output format.
     """
-    seeds_normalized = [tuple(i) for i in seeds]
-    reactions = split_stoichiometries(model)
+    seeds = [tuple(i) for i in seeds]
+    reactions = _split_stoichiometries(model)
     partial_scope = partial(
         _scope,
         model=model,
         reactions=reactions,
         include_weak_cofactors=include_weak_cofactors,
         return_lumped_results=return_lumped_results,
     )
     if not multiprocessing or sys.platform in ["win32", "cygwin"]:
-        return dict(zip(seeds_normalized, map(partial_scope, seeds)))
+        return dict(zip(seeds, map(partial_scope, seeds)))
     else:
         pool = Pool(processes=cpu_count())
-        res = dict(zip(seeds_normalized, pool.map(partial_scope, seeds)))
-        pool.close()
-        return res
+        return dict(zip(seeds, pool.map(partial_scope, seeds)))
```

### Comparing `moped-1.9.9/src/moped/topological/treesearch.py` & `moped-1rc1/moped/topological/treesearch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 """Interface to tree search algorithms."""
-from __future__ import annotations
 
-from queue import LifoQueue, Queue
-from typing import TYPE_CHECKING, Dict, Iterable, List, Tuple, cast
+from queue import Queue
+from queue import LifoQueue
 
-from typing_extensions import Literal
 
-if TYPE_CHECKING:
-    from ..core.model import Model
-
-__all__ = ["metabolite_tree_search"]
-
-
-def _deconstruct_path(
-    end: str, parents: Dict[str, Tuple[str | None, str | None]]
-) -> Tuple[List[str], List[str]]:
+def _deconstruct_path(start, end, parents):
     """Deconstruct the path taken."""
     met, rec = parents[end]
     mets = [met]
     recs = [rec]
     while True:
-        met, rec = parents[cast(str, met)]
+        met, rec = parents[met]
         if met is not None:
             recs.append(rec)
             mets.append(met)
         else:
-            return cast(List[str], mets[::-1] + [end]), cast(List[str], recs[::-1])
+            return mets[::-1] + [end], recs[::-1]
 
 
-def split_stoichiometries(
-    model: Model,
-) -> Dict[str, Dict[str, Dict[str, float]]]:
+def _split_stoichiometries(model):
     """Split reaction stoichiometries into substrates and products.
 
     This is done to have the sets of either substrates and products
     to run the scope algorithm smoothly, e.g. comparing if substrates
     are a subset of the seed.
 
     Parameters
@@ -47,86 +35,79 @@
         Mapping of reaction ids to their substrates and products
     """
     reactions = {}
     for reaction_id, rxn in model.reactions.items():
         # Exclude medium reactions
         if len(rxn.stoichiometries) == 1:
             continue
-        substrates, products = rxn.split_stoichiometries()
-        reactions[reaction_id] = {
-            "substrates": substrates,
-            "products": products,
-        }
+        substrates, products = rxn._split_stoichiometries()
+        reactions[reaction_id] = {"substrates": substrates, "products": products}
     return reactions
 
 
-def _add_metabolite(
-    child_metabolite: str,
-    parent_metabolite: str,
-    reaction_id: str,
-    parents: Dict[str, Tuple[str | None, str | None]],
-    Q: LifoQueue | Queue,
-) -> None:
-    if child_metabolite not in parents:
-        parents[child_metabolite] = parent_metabolite, reaction_id
-        Q.put(child_metabolite)
-
-
 def metabolite_tree_search(
-    model: Model,
-    start_compound_id: str,
-    end_compound_id: str,
-    max_iterations: int,
-    ignored_reaction_ids: Iterable[str] | None,
-    ignored_compound_ids: Iterable[str] | None,
-    search_type: Literal["breadth-first", "depth-first"],
-) -> Tuple[List[str], List[str]]:
+    model,
+    start_compound_id,
+    end_compound_id,
+    max_iterations,
+    ignored_reaction_ids,
+    ignored_compound_ids,
+    search_type,
+):
     """Do a tree search to find the shortest connection between two compounds.
 
     Parameters
     ----------
     start_compound_id : str
     end_compound_id : str
     max_iterations : int
     ignored_reaction_ids : iterable
     ignored_compound_ids : iterable
     search_type : str, {breadth-first, depth-first}
     """
-    model = model.copy()
-    for i in [start_compound_id, end_compound_id]:
-        if i not in model.compounds:
-            raise KeyError(f"Could not find compound {i}")
-    ignored_reaction_ids = set() if ignored_reaction_ids is None else set(ignored_reaction_ids)
-    ignored_compound_ids = set() if ignored_compound_ids is None else set(ignored_compound_ids)
+    ignored_reaction_ids = (
+        set() if ignored_reaction_ids is None else set(ignored_reaction_ids)
+    )
+    ignored_compound_ids = (
+        set() if ignored_compound_ids is None else set(ignored_compound_ids)
+    )
     cofactors = set(model.get_weak_cofactors()) ^ set(model.get_strong_cofactors())
 
-    reactions = split_stoichiometries(model)
+    reactions = _split_stoichiometries(model)
     for i in ignored_reaction_ids:
-        model.remove_reaction(reaction_id=i)
+        del reactions[i]
 
     if search_type == "breadth-first":
-        Q: Queue | LifoQueue = Queue()  # FIFO Queue
+        Q = Queue()  # FIFO Queue
     elif search_type == "depth-first":
         Q = LifoQueue()
     else:
-        raise ValueError("Unknown search type, choose from {breadth-first, depth-first}")
+        raise ValueError(
+            "Unknown search type, choose from {breadth-first, depth-first}"
+        )
     Q.put(start_compound_id)
-    parents: Dict[str, Tuple[str | None, str | None]] = {
-        k: (None, None) for k in (cofactors ^ {start_compound_id} ^ ignored_compound_ids)
+    parents = {
+        k: (None, None)
+        for k in (cofactors ^ {start_compound_id} ^ ignored_compound_ids)
     }  # Parent metabolites and reactions of discovered metabolites
     n = 0
 
+    def add_metabolite(child_metabolite, parent_metabolite, reaction_id):
+        if child_metabolite not in parents:
+            parents[child_metabolite] = parent_metabolite, reaction_id
+            Q.put(child_metabolite)
+
     while not Q.empty():
         substrate_id = Q.get()
         if substrate_id == end_compound_id:
-            return _deconstruct_path(end_compound_id, parents)
+            return _deconstruct_path(start_compound_id, end_compound_id, parents)
 
         for reaction_id in model.compounds[substrate_id].in_reaction:
             reaction = reactions[reaction_id]
             if substrate_id in reaction["substrates"]:
                 for product_id in reaction["products"]:
-                    _add_metabolite(product_id, substrate_id, reaction_id, parents, Q)
+                    add_metabolite(product_id, substrate_id, reaction_id)
         n += 1
         if n == max_iterations:
             raise ValueError("Exceeded max iterations")
     else:
         raise ValueError("Could not find a solution")
```

