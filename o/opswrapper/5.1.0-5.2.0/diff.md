# Comparing `tmp/opswrapper-5.1.0.tar.gz` & `tmp/opswrapper-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opswrapper-5.1.0.tar", last modified: Thu Oct 13 20:52:15 2022, max compression
+gzip compressed data, was "opswrapper-5.2.0.tar", last modified: Mon May  8 18:21:58 2023, max compression
```

## Comparing `opswrapper-5.1.0.tar` & `opswrapper-5.2.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2022-10-13 20:52:15.736178 opswrapper-5.1.0/
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1069 2022-10-13 20:52:15.000000 opswrapper-5.1.0/LICENSE.txt
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2618 2022-10-13 20:52:15.736178 opswrapper-5.1.0/PKG-INFO
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2110 2022-10-13 20:52:15.000000 opswrapper-5.1.0/README.rst
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      111 2022-10-13 20:52:15.000000 opswrapper-5.1.0/pyproject.toml
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      704 2022-10-13 20:52:15.736178 opswrapper-5.1.0/setup.cfg
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)       38 2022-10-13 20:52:15.000000 opswrapper-5.1.0/setup.py
-drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2022-10-13 20:52:15.726179 opswrapper-5.1.0/src/
-drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2022-10-13 20:52:15.726179 opswrapper-5.1.0/src/opswrapper/
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      562 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/__init__.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)        5 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/__version__
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     9926 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/algorithm.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     7086 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/analysis.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     6834 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/base.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3502 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/config.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2873 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/constraints.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8275 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/element.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3919 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/formatting.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3705 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/integration.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8937 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/integrator.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)    12437 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/material.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1576 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/model.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     7904 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/output.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8519 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/section.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     9100 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/test.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     6860 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/uniaxialmaterialanalysis.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     6316 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper/utils.py
-drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2022-10-13 20:52:15.726179 opswrapper-5.1.0/src/opswrapper.egg-info/
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2618 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper.egg-info/PKG-INFO
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      953 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper.egg-info/SOURCES.txt
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)        1 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper.egg-info/dependency_links.txt
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)       19 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper.egg-info/requires.txt
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)       11 2022-10-13 20:52:15.000000 opswrapper-5.1.0/src/opswrapper.egg-info/top_level.txt
-drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2022-10-13 20:52:15.736178 opswrapper-5.1.0/test/
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1472 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_algorithm.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      907 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_constraints.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      805 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_element.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1235 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_integrator.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3085 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_material.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      604 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_model.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     5883 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_recorders.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1255 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_section.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      879 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_test.py
--rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      145 2022-10-13 20:52:15.000000 opswrapper-5.1.0/test/test_utils.py
+drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2023-05-08 18:21:58.268831 opswrapper-5.2.0/
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1069 2023-05-08 18:21:57.000000 opswrapper-5.2.0/LICENSE.txt
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2618 2023-05-08 18:21:58.268831 opswrapper-5.2.0/PKG-INFO
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2110 2023-05-08 18:21:57.000000 opswrapper-5.2.0/README.rst
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      111 2023-05-08 18:21:57.000000 opswrapper-5.2.0/pyproject.toml
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      704 2023-05-08 18:21:58.268831 opswrapper-5.2.0/setup.cfg
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)       38 2023-05-08 18:21:57.000000 opswrapper-5.2.0/setup.py
+drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2023-05-08 18:21:58.258831 opswrapper-5.2.0/src/
+drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2023-05-08 18:21:58.268831 opswrapper-5.2.0/src/opswrapper/
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      562 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/__init__.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)        5 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/__version__
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     9850 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/algorithm.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     7117 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/analysis.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     6835 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/base.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3567 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/config.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2877 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/constraints.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8583 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/element.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3943 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/formatting.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     7092 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/integration.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8900 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/integrator.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)    12399 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/material.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1738 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/model.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8024 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/output.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     8998 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/section.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     9097 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/test.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     6888 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/uniaxialmaterialanalysis.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     6372 2023-05-08 18:21:57.000000 opswrapper-5.2.0/src/opswrapper/utils.py
+drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2023-05-08 18:21:58.268831 opswrapper-5.2.0/src/opswrapper.egg-info/
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     2618 2023-05-08 18:21:58.000000 opswrapper-5.2.0/src/opswrapper.egg-info/PKG-INFO
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      978 2023-05-08 18:21:58.000000 opswrapper-5.2.0/src/opswrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)        1 2023-05-08 18:21:58.000000 opswrapper-5.2.0/src/opswrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)       19 2023-05-08 18:21:58.000000 opswrapper-5.2.0/src/opswrapper.egg-info/requires.txt
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)       11 2023-05-08 18:21:58.000000 opswrapper-5.2.0/src/opswrapper.egg-info/top_level.txt
+drwxr-xr-x   0 ptalley2  (1000) ptalley2  (1000)        0 2023-05-08 18:21:58.268831 opswrapper-5.2.0/test/
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1496 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_algorithm.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      915 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_constraints.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      789 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_element.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      506 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_integration.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1235 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_integrator.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     3167 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_material.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      604 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_model.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     5915 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_recorders.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)     1269 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_section.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      879 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_test.py
+-rw-r--r--   0 ptalley2  (1000) ptalley2  (1000)      169 2023-05-08 18:21:57.000000 opswrapper-5.2.0/test/test_utils.py
```

### Comparing `opswrapper-5.1.0/LICENSE.txt` & `opswrapper-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opswrapper-5.1.0/PKG-INFO` & `opswrapper-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswrapper
-Version: 5.1.0
+Version: 5.2.0
 Summary: Python helpers for writing OpenSees scripts.
 Home-page: https://github.com/otaithleigh/opswrapper
 Author: Peter Talley
 Author-email: ptalley2@vols.utk.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opswrapper-5.1.0/README.rst` & `opswrapper-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `opswrapper-5.1.0/setup.cfg` & `opswrapper-5.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `opswrapper-5.1.0/src/opswrapper/__init__.py` & `opswrapper-5.2.0/src/opswrapper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from . import test
 from . import uniaxialmaterialanalysis
 from . import utils
 from .base import *
 from .formatting import *
 from .model import *
 
-__version__ = importlib.resources.read_text(__name__, '__version__')
+__version__ = importlib.resources.read_text(__name__, "__version__")
```

### Comparing `opswrapper-5.1.0/src/opswrapper/algorithm.py` & `opswrapper-5.2.0/src/opswrapper/algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,129 +1,134 @@
 import dataclasses
 import typing as t
 
 from .base import OpenSeesObject
 from .utils import ValueTypeDispatch
 
 __all__ = [
-    'Algorithm',
-    'BFGS',
-    'Broyden',
-    'KrylovNewton',
-    'Linear',
-    'ModifiedNewton',
-    'Newton',
-    'NewtonLineSearch',
-    'SecantNewton',
+    "Algorithm",
+    "BFGS",
+    "Broyden",
+    "KrylovNewton",
+    "Linear",
+    "ModifiedNewton",
+    "Newton",
+    "NewtonLineSearch",
+    "SecantNewton",
 ]
 
 
 class Algorithm(OpenSeesObject):
     _tangent_flag_dispatch: t.ClassVar[ValueTypeDispatch[str, t.Union[str, None]]]
 
-    def __init_subclass__(cls, tangent_dispatch: t.Optional[dict] = None, **kwargs) -> None:
+    def __init_subclass__(
+        cls, tangent_dispatch: t.Optional[dict] = None, **kwargs
+    ) -> None:
         super().__init_subclass__(**kwargs)
         if tangent_dispatch is not None:
-            cls._tangent_flag_dispatch = ValueTypeDispatch('tangent', tangent_dispatch)
+            cls._tangent_flag_dispatch = ValueTypeDispatch("tangent", tangent_dispatch)
 
     def tcl_code(self, formats=None) -> str:
-        return ' '.join(['algorithm', *self.tcl_args(formats)])
+        return " ".join(["algorithm", *self.tcl_args(formats)])
 
     # The only option to most algorithm commands is the tangent type, handled
     # here by `_tangent_flag_dispatch`. Since these are just str, they don't
     # need to go through `format_objects`.
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [self.__class__.__name__]
         tangent_flag = self._tangent_flag_dispatch[self.tangent]
         if tangent_flag is not None:
             args.append(tangent_flag)
 
         return args
 
 
-#===================================================================================================
+# ======================================================================================
 # Classical methods
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class Linear(
     Algorithm,
     tangent_dispatch={
-        'current': None,
-        'initial': '-initial',
-        'secant': '-secant',
+        "current": None,
+        "initial": "-initial",
+        "secant": "-secant",
     },
 ):
     """Linear algorithm which takes one iteration to solve the system of
     equations::
 
         ΔU = K^-1 R(U)
 
     Parameters
     ----------
     tangent : {'current', 'initial', 'secant'}
         Which stiffness to use for iterating. (default: 'current')
     factor_once : bool, optional
         If True, only set up and factor the matrix once. (default: False)
     """
-    tangent: str = 'current'
+
+    tangent: str = "current"
     factor_once: bool = False
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = super().tcl_args(formats)
         if self.factor_once:
-            args.append('-factorOnce')
+            args.append("-factorOnce")
         return args
 
 
 @dataclasses.dataclass
 class Newton(
     Algorithm,
     tangent_dispatch={
-        'current': None,
-        'initial': '-initial',
-        'initialThenCurrent': '-intialThenCurrent',  # Not a typo
-        'secant': '-secant',
-        'hall': '-hall',
+        "current": None,
+        "initial": "-initial",
+        "initialThenCurrent": "-intialThenCurrent",  # Not a typo
+        "secant": "-secant",
+        "hall": "-hall",
     },
 ):
     """Newton-Raphson method for solving the nonlinear residual equation.
 
     Parameters
     ----------
     tangent : {'current', 'initial', 'initialThenCurrent', 'secant', 'hall'}
         Which stiffness to use for iterating. (default: 'current')
     """
-    tangent: str = 'current'
+
+    tangent: str = "current"
 
 
 @dataclasses.dataclass
 class ModifiedNewton(
     Algorithm,
     tangent_dispatch={
-        'current': None,
-        'initial': '-initial',
-        'secant': '-secant',
-        'hall': '-hall',
+        "current": None,
+        "initial": "-initial",
+        "secant": "-secant",
+        "hall": "-hall",
     },
 ):
     """Modified Newton-Raphson method for solving the nonlinear residual
     equation.
 
     Parameters
     ----------
     tangent : {'current', 'initial', 'secant', 'hall'}
         Which stiffness to use for iterating. (default: 'current')
     """
-    tangent: str = 'current'
+
+    tangent: str = "current"
 
 
-#===================================================================================================
+# ======================================================================================
 # Line search methods
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class NewtonLineSearch(Algorithm):
     """Newton-Raphson algorithm with line search, which increases the
     effectiveness when convergence is slow due to roughness of the residual.
 
     Parameters
     ----------
@@ -153,83 +158,85 @@
         U_n1 = U_n + η ΔU
 
     The different line search algorithms use different root finding algorithms
     to obtain η, a root to the function s(η) defined as::
 
         s(η) = ΔU R(U_n + η ΔU)
     """
-    type_search: str = 'InitialInterpolated'
+
+    type_search: str = "InitialInterpolated"
     tol: float = 0.8
     max_iters: int = 10
     min_eta: float = 0.1
     max_eta: float = 10.0
 
     _line_search_type_dispatch = ValueTypeDispatch(
-        'line search',
+        "line search",
         {
-            'Bisection': 'Bisection',
-            'Secant': 'Secant',
-            'RegulaFalsi': 'RegulaFalsi',
-            'InitialInterpolated': 'InitialInterpolated'
+            "Bisection": "Bisection",
+            "Secant": "Secant",
+            "RegulaFalsi": "RegulaFalsi",
+            "InitialInterpolated": "InitialInterpolated",
         },
     )
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [
-            'NewtonLineSearch',
-            '-typeSearch',
+            "NewtonLineSearch",
+            "-typeSearch",
             self._line_search_type_dispatch[self.type_search],
-            '-tol',
+            "-tol",
             self.tol,
-            '-maxIter',
+            "-maxIter",
             self.max_iters,
-            '-minEta',
+            "-minEta",
             self.min_eta,
-            '-maxEta',
+            "-maxEta",
             self.max_eta,
         ]
         return self.format_objects(args, formats)
 
 
-#===================================================================================================
+# ======================================================================================
 # Accelerated Newton methods
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class _AcceleratedNewton(
     Algorithm,
     tangent_dispatch={
-        'current': 'current',
-        'initial': 'initial',
-        'noTangent': 'noTangent',
+        "current": "current",
+        "initial": "initial",
+        "noTangent": "noTangent",
     },
 ):
     """Modified Newton method with accelerator.
 
     Parameters
     ----------
     iterate : {'current', 'initial', 'noTangent'}, optional
         Tangent to iterate on. (default: 'current')
     increment : {'current', 'initial', 'noTangent'}, optional
         Tangent to increment on. (default: 'current')
     max_dim: int, optional
         Maximum number of iterations until the tangent is reformed and the
         acceleration restarts. (default: 3)
     """
-    iterate: str = 'current'
-    increment: str = 'current'
+
+    iterate: str = "current"
+    increment: str = "current"
     max_dim: int = 3
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [self.__class__.__name__]
         tangent_iter = self._tangent_flag_dispatch[self.iterate]
         tangent_incr = self._tangent_flag_dispatch[self.increment]
 
-        args.extend(['-iterate', tangent_iter])
-        args.extend(['-increment', tangent_incr])
-        args.extend(['-maxDim', *self.format_objects([self.max_dim], formats)])
+        args.extend(["-iterate", tangent_iter])
+        args.extend(["-increment", tangent_incr])
+        args.extend(["-maxDim", *self.format_objects([self.max_dim], formats)])
 
         return args
 
 
 @dataclasses.dataclass
 class KrylovNewton(_AcceleratedNewton):
     """Modified Newton method with Krylov subspace accelerator.
@@ -275,32 +282,32 @@
 #
 #
 # @dataclasses.dataclass
 # class PeriodicNewton(_AcceleratedNewton):
 #     pass
 
 
-#===================================================================================================
+# ======================================================================================
 # Broyden-type algorithms
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class _Broyden(
     Algorithm,
     tangent_dispatch={
-        'current': None,
-        'initial': '-initial',
-        'secant': '-secant',
+        "current": None,
+        "initial": "-initial",
+        "secant": "-secant",
     },
 ):
-    tangent: str = 'current'
+    tangent: str = "current"
     count: int = 10
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = super().tcl_args(formats)
-        args.extend(self.format_objects(['-count', self.count], formats))
+        args.extend(self.format_objects(["-count", self.count], formats))
         return args
 
 
 @dataclasses.dataclass
 class Broyden(_Broyden):
     """Broyden algorithm for general unsymmetric systems.
```

### Comparing `opswrapper-5.1.0/src/opswrapper/analysis.py` & `opswrapper-5.2.0/src/opswrapper/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     return str(uuid.uuid4())
 
 
 def _get_default_scratch_path():
     return config.path_of.scratch
 
 
-class ScratchFile():
+class ScratchFile:
     """Create a scratch file path generator.
 
     Parameters
     ----------
     analysis_type : str
         Type of the analysis, e.g. 'SectionAnalysis'.
     analysis_id : optional
@@ -39,36 +39,37 @@
 
     Example
     -------
     >>> scratch_file = scratch_file_factory('TestoPresto', 0)
     >>> scratch_file('disp', '.dat')
     PosixPath('/tmp/TestoPresto_0_disp.dat')
     """
+
     def __init__(
         self,
         analysis_type: str,
         analysis_id: Optional[str] = None,
-        scratch_path: Optional[Path] = None
+        scratch_path: Optional[Path] = None,
     ):
         if analysis_id is None:
             analysis_id = _get_str_uuid4()
         if scratch_path is None:
             scratch_path = _get_default_scratch_path()
 
         self.analysis_type = str(analysis_type)
         self.analysis_id = str(analysis_id)
         self.scratch_path = Path(scratch_path).resolve()
 
     def __repr__(self) -> str:
         analysis_type = self.analysis_type
         analysis_id = self.analysis_id
         scratch_path = self.scratch_path
-        return f'ScratchFile({analysis_type=}, {analysis_id=}, {scratch_path=})'
+        return f"ScratchFile({analysis_type=}, {analysis_id=}, {scratch_path=})"
 
-    def __call__(self, name: str, suffix: str = '') -> Path:
+    def __call__(self, name: str, suffix: str = "") -> Path:
         """
         Parameters
         ----------
         name : str
             Name of the scratch file, e.g. 'displacement'.
         suffix : str, optional
             Suffix to use for the scratch file. (default: '')
@@ -79,41 +80,44 @@
             Path to the scratch file.
         """
         components = []
         if self.analysis_type:
             components.append(self.analysis_type)
         if self.analysis_id:
             components.append(self.analysis_id)
-        components.append(f'{name}{suffix}')
-        filename = '_'.join(components)
+        components.append(f"{name}{suffix}")
+        filename = "_".join(components)
 
-        return self.scratch_path/filename
+        return self.scratch_path / filename
 
 
 def scratch_file_factory(*args, **kwargs):
-    warnings.warn('opswrapper.analysis.scratch_file_factory is deprecated.'
-                  'Use opswrapper.analysis.ScratchFile instead.')
+    warnings.warn(
+        "opswrapper.analysis.scratch_file_factory is deprecated."
+        "Use opswrapper.analysis.ScratchFile instead."
+    )
     return ScratchFile(*args, **kwargs)
 
 
 class AnalysisResults(NamedTuple):
     """Results from an OpenSees analysis.
 
     Parameters
     ----------
     returncode : int
         The return code from OpenSees.
     stdout : str
         Captured console output from OpenSees.
     """
+
     returncode: int
     stdout: str
 
 
-class OpenSeesAnalysis():
+class OpenSeesAnalysis:
     """Wrapper for an OpenSees analysis.
 
     Parameters
     ----------
     name : str, optional
         Descriptive name for the analysis object. Defaults to the class name.
     echo_output : bool, optional
@@ -123,14 +127,15 @@
     opensees_path : Path, optional
         Path to the OpenSees binary to use. If None, uses the value from the
         global configuration. (default: None)
     scratch_path : Path, optional
         Path to the directory for storing temporary files. If None, uses the
         value from the global configuration. (default: None)
     """
+
     def __init__(
         self,
         name: str = None,
         echo_output: bool = False,
         delete_files: bool = True,
         opensees_path: Path = None,
         scratch_path: Path = None,
@@ -141,16 +146,16 @@
         self.name = name
         self.echo_output = echo_output
         self.delete_files = delete_files
         self.opensees_path = opensees_path
         self.scratch_path = scratch_path
 
     def __repr__(self):
-        clsname = self.__class__.__module__ + '.' + self.__class__.__name__
-        return f'<{clsname} {self.name!r} at {id(self):#x}>'
+        clsname = self.__class__.__module__ + "." + self.__class__.__name__
+        return f"<{clsname} {self.name!r} at {id(self):#x}>"
 
     @property
     def opensees_path(self):
         """Path to the OpenSees binary to use.
 
         If None, looks for 'OpenSees' on the system PATH.
         """
@@ -217,21 +222,26 @@
         """
         if echo is None:
             echo = self.echo_output
 
         cmd = [str(self.opensees_path), str(inputfile)]
         stdout = []
         if echo:
+
             def handle_stdout(line):
-                print(line, end='')
+                print(line, end="")
                 stdout.append(line)
+
         else:
+
             def handle_stdout(line):
                 stdout.append(line)
 
-        with sub.Popen(cmd, bufsize=1, stdout=sub.PIPE, stderr=sub.STDOUT, text=True) as p:
+        with sub.Popen(
+            cmd, bufsize=1, stdout=sub.PIPE, stderr=sub.STDOUT, text=True
+        ) as p:
             for line in p.stdout:
                 handle_stdout(line)
 
-        stdout = ''.join(stdout)
+        stdout = "".join(stdout)
 
         return AnalysisResults(p.returncode, stdout)
```

### Comparing `opswrapper-5.1.0/src/opswrapper/base.py` & `opswrapper-5.2.0/src/opswrapper/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import dataclasses
 import typing
 
 from .formatting import MultiFormatSpec, SpecLike, _GLOBAL_FORMAT_SPEC
 from .utils import coerce_numeric
 
 __all__ = [
-    'OpenSeesObject',
+    "OpenSeesObject",
 ]
 
 
 class OpenSeesObject(abc.ABC):
     """Base class for wrapping OpenSees Tcl objects/commands.
 
     Formatting
@@ -42,14 +42,15 @@
         >>> section.Elastic2D.set_class_format_spec({float: '#.3g'})
         >>> s = section.Elastic2D(...)
         >>> s.set_format_spec({float: '#.3g'})
 
     Each of these methods return the previously-set modifiers if you wish to restore
     them later.
     """
+
     _format_spec: MultiFormatSpec = _GLOBAL_FORMAT_SPEC
 
     def __post_init__(self):
         # Gently attempt to coerce numeric types. Not guarding against TypeError
         # from dataclasses.fields since __post_init__ only gets called on
         # dataclasses.
         for field in dataclasses.fields(self):
```

### Comparing `opswrapper-5.1.0/src/opswrapper/config.py` & `opswrapper-5.2.0/src/opswrapper/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import warnings
 from pathlib import Path
 from typing import Union
 
 import tomli
 
-_CONFIG_FILE_NAME = '.path_of.toml'
+_CONFIG_FILE_NAME = ".path_of.toml"
 
 
-class PathOf():
+class PathOf:
     """Paths to important files and directories.
 
     Works by looking for `.path_of.toml` files, starting from the current
     working directory and working back to the root, with the root having the
     lowest priority and the CWD the highest. Any time the CWD changes, the
     configuration is re-calculated.
 
@@ -25,53 +25,58 @@
     Configured paths may be accessed using either key (`path_of['opensees']`)
     or attribute (`path_of.opensees`) access.
 
     Temporary overrides may be set using key-value syntax
     (`path_of['opensees'] = '/path/to/OpenSees'`), but will be overridden if the
     CWD changes and the configuration recalculates.
     """
+
     _default = {
-        'opensees': Path('OpenSees'),
-        'scratch': Path.home()/'Scratch',
+        "opensees": Path("OpenSees"),
+        "scratch": Path.home() / "Scratch",
     }
 
     def __init__(self):
         self._cwd = Path.cwd()
         self._config: dict[str, Path] = {}
         self._build_config()
 
     def _build_config(self):
         """Starting from the CWD, walk up to root, accumulating .path_of.toml
         files, then apply them starting from root.
         """
         config_files = []
-        if (p := self._cwd/_CONFIG_FILE_NAME).exists():
+        if (p := self._cwd / _CONFIG_FILE_NAME).exists():
             config_files.append(p)
 
         for parent in self._cwd.parents:
-            if (p := parent/_CONFIG_FILE_NAME).exists():
+            if (p := parent / _CONFIG_FILE_NAME).exists():
                 config_files.append(p)
 
         for file in reversed(config_files):
             self._apply_config(file)
 
     def _apply_config(self, filename):
         try:
-            with open(filename, 'rb') as f:
+            with open(filename, "rb") as f:
                 config = tomli.load(f)
         except Exception as exc:
-            warnings.warn(f'Could not load config file {filename} due to exception: {exc}')
+            warnings.warn(
+                f"Could not load config file {filename} due to exception: {exc}"
+            )
             return
 
         config_bak = self._config.copy()
         pathed_config = zip(config.keys(), map(Path, config.values()))
         try:
             self._config.update(pathed_config)
         except Exception as exc:
-            warnings.warn(f'Failed to apply config file {filename} due to exception: {exc}')
+            warnings.warn(
+                f"Failed to apply config file {filename} due to exception: {exc}"
+            )
             self._config = config_bak
 
     def __setitem__(self, key: str, value: Union[str, Path]):
         self.set(key, value)
 
     def __getitem__(self, key: str) -> Path:
         return self.get(key)
@@ -97,15 +102,15 @@
             self._cwd = cwd
             self._build_config()
         value = self._config.get(key)
         if value is None:
             try:
                 return self._default[key]
             except KeyError as exc:
-                raise KeyError(f'{key!r} is unset and no default is provided') from exc
+                raise KeyError(f"{key!r} is unset and no default is provided") from exc
         else:
             return value
 
     def set(self, key: str, value: Union[str, Path]):
         self._config[key] = Path(value)
```

### Comparing `opswrapper-5.1.0/src/opswrapper/constraints.py` & `opswrapper-5.2.0/src/opswrapper/constraints.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import typing as t
 
 from .base import OpenSeesObject
 
 
 class Constraints(OpenSeesObject):
     def tcl_code(self, formats=None) -> str:
-        return ' '.join(['constraints', *self.tcl_args(formats=formats)])
+        return " ".join(["constraints", *self.tcl_args(formats=formats)])
 
 
 @dataclasses.dataclass
 class Plain(Constraints):
     """Plain constraint handler.
 
     Only supports constraints applied using the 'fix' and 'equalDOF' commands.
     """
+
     def tcl_args(self, formats=None) -> t.List[str]:
-        return ['Plain']
+        return ["Plain"]
 
 
 @dataclasses.dataclass
 class Transformation(Constraints):
     """Constraints enforcement by the transformation method.
 
     Notes
@@ -34,16 +35,17 @@
     transformation method does not follow constraints:
 
     1. If a node is fixed, constrain it with the 'fix' command and 'equalDOF' or
        other type of constraint.
     2. If multiple nodes are constrained, make sure that the retained node is
        not constrained in any other constraint.
     """
+
     def tcl_args(self, formats=None) -> t.List[str]:
-        return ['Transformation']
+        return ["Transformation"]
 
 
 @dataclasses.dataclass
 class Lagrange(Constraints):
     """Constraints enforcement using Lagrange multipliers.
 
     Parameters
@@ -56,19 +58,20 @@
     Notes
     -----
     The Lagrange multiplier method introduces new unknowns to the system of
     equations. The diagonal part of the system corresponding to these new
     unknowns is 0.0. This ensures that the system IS NOT symmetric positive
     definite.
     """
+
     alpha_s: float
     alpha_m: float
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['Lagrange', self.alpha_s, self.alpha_m]
+        args = ["Lagrange", self.alpha_s, self.alpha_m]
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class Penalty(Constraints):
     """Constraints enforcement using the penalty method.
 
@@ -82,13 +85,14 @@
     Notes
     -----
     The degree to which the constraints are enforced is dependent on the penalty
     values chosen. Problems can arise if these values are too small (constraint
     not enforced strongly enough) or too large (problems associated with
     conditioning of the system of equations).
     """
+
     alpha_s: float
     alpha_m: float
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['Penalty', self.alpha_s, self.alpha_m]
+        args = ["Penalty", self.alpha_s, self.alpha_m]
         return self.format_objects(args, formats)
```

### Comparing `opswrapper-5.1.0/src/opswrapper/element.py` & `opswrapper-5.2.0/src/opswrapper/element.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclasses.dataclass
 class Element(base.OpenSeesObject):
     tag: int
     inode: int
     jnode: int
 
     def tcl_code(self, formats=None) -> str:
-        return 'element ' + ' '.join(self.tcl_args(formats))
+        return "element " + " ".join(self.tcl_args(formats))
 
 
 @dataclasses.dataclass
 class ElasticBeamColumn2D(Element):
     """Elastic beam column element for 2D analysis.
 
     Does not include shear deformations.
@@ -39,30 +39,37 @@
         Tag of the geometric transformation to use.
     mass : float, optional
         Mass-per-length of the element. (default: None)
     cmass : bool, optional
         If True, use a consistent mass matrix instead of a lumped mass matrix.
         (default: False)
     """
+
     A: float
     E: float
     Iz: float
     transf: int
     mass: float = None
     cmass: bool = False
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [
-            'elasticBeamColumn', self.tag, self.inode, self.jnode, self.A, self.E, self.Iz,
-            self.transf
+            "elasticBeamColumn",
+            self.tag,
+            self.inode,
+            self.jnode,
+            self.A,
+            self.E,
+            self.Iz,
+            self.transf,
         ]
         if self.mass is not None:
-            args.extend(['-mass', self.mass])
+            args.extend(["-mass", self.mass])
         if self.cmass:
-            args.append('-cMass')
+            args.append("-cMass")
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class ElasticBeamColumn3D(Element):
     A: float
     E: float
@@ -72,21 +79,30 @@
     Iz: float
     transf: int
     mass: float = None
     cmass: bool = False
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [
-            'elasticBeamColumn', self.tag, self.inode, self.jnode, self.A, self.E, self.G, self.J,
-            self.Iy, self.Iz, self.transf
+            "elasticBeamColumn",
+            self.tag,
+            self.inode,
+            self.jnode,
+            self.A,
+            self.E,
+            self.G,
+            self.J,
+            self.Iy,
+            self.Iz,
+            self.transf,
         ]
         if self.mass is not None:
-            args.extend(['-mass', self.mass])
+            args.extend(["-mass", self.mass])
         if self.cmass:
-            args.append('-cMass')
+            args.append("-cMass")
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class ForceBeamColumn(Element):
     """Force-based beam column element.
 
@@ -107,27 +123,35 @@
     iterative : bool, optional
         If True, use the iterative form of the element solution. (default: False)
     maxiters : int, optional
         Maximum iterations for the iterative form. (default: 10)
     itertol : float, optional
         Tolerance for the iterative form. (default: 1e-12)
     """
+
     transf: int
     integration: t.Union[str, integration.Integration]
     mass: float = None
     iterative: bool = False
     maxiters: int = 10
     itertol: float = 1e-12
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['forceBeamColumn', self.tag, self.inode, self.jnode, self.transf, self.integration]
+        args = [
+            "forceBeamColumn",
+            self.tag,
+            self.inode,
+            self.jnode,
+            self.transf,
+            self.integration,
+        ]
         if self.mass is not None:
-            args.extend(['-mass', self.mass])
+            args.extend(["-mass", self.mass])
         if self.iterative:
-            args.extend(['-iter', self.maxiters, self.itertol])
+            args.extend(["-iter", self.maxiters, self.itertol])
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class DispBeamColumn(Element):
     """Displacement-based beam column element.
 
@@ -150,45 +174,48 @@
     cmass : bool, optional
         If True, use a consistent mass matrix instead of a lumped mass matrix.
         (default: False)
     integration : str, optional
         Integration method to use: 'Lobotto', 'Legendre', 'Radau', 'NewtonCotes',
         or 'Trapezoidal'. (default: 'Legendre')
     """
+
     npoints: int
     section: int
     transf: int
     mass: float = None
     cmass: bool = False
-    integration: str = 'Legendre'
+    integration: str = "Legendre"
 
     def tcl_args(self, formats=None) -> t.List[str]:
         try:
             nsections = len(self.section)
             if nsections != self.npoints and nsections != 1:
-                raise ValueError("DispBeamColumn: number of sections must be 1 or npoints")
+                raise ValueError(
+                    "DispBeamColumn: number of sections must be 1 or npoints"
+                )
             sections = self.section
         except TypeError:
             nsections = 1
             sections = [self.section]
 
-        args = ['dispBeamColumn', self.tag, self.inode, self.jnode, self.npoints]
+        args = ["dispBeamColumn", self.tag, self.inode, self.jnode, self.npoints]
         if nsections == 1:
             args.append(self.section)
             args.append(self.transf)
         else:
-            args.append('-sections')
+            args.append("-sections")
             args.extend(sections)
             args.append(self.transf)
         if self.mass is not None:
-            args.extend(['-mass', self.mass])
+            args.extend(["-mass", self.mass])
         if self.cmass:
-            args.append('-cMass')
-        if self.integration != 'Legendre':
-            args.extend('-integration', self.integration)
+            args.append("-cMass")
+        if self.integration != "Legendre":
+            args.extend("-integration", self.integration)
 
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class Truss(Element):
     """Truss element.
@@ -210,30 +237,31 @@
     cmass : bool, optional
         If True, use a consistent mass matrix instead of lumped mass. (default: False)
     do_rayleigh : bool, optional
         If True, include Rayleigh damping for this element. (default: False)
     corot : bool, optional
         If True, construct a corotTruss instead of a truss. (default: False)
     """
+
     A: float
     mat: int
     rho: float = None
     cmass: bool = False
     do_rayleigh: bool = False
     corot: bool = False
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        element = 'corotTruss' if self.corot else 'truss'
+        element = "corotTruss" if self.corot else "truss"
         args = [element, self.tag, self.inode, self.jnode, self.A, self.mat]
         if self.rho is not None:
-            args.extend(['-rho', self.rho])
+            args.extend(["-rho", self.rho])
         if self.cmass:
-            args.extend(['-cMass', self.cmass])
+            args.extend(["-cMass", self.cmass])
         if self.do_rayleigh:
-            args.extend(['-doRayleigh', self.do_rayleigh])
+            args.extend(["-doRayleigh", self.do_rayleigh])
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class TrussSection(Element):
     """Truss element specified by a section.
 
@@ -252,23 +280,24 @@
     cmass : bool, optional
         If True, use a consistent mass matrix instead of lumped mass. (default: False)
     do_rayleigh : bool, optional
         If True, include Rayleigh damping for this element. (default: False)
     corot : bool, optional
         If True, construct a corotTruss instead of a truss. (default: False)
     """
+
     section: int
     rho: float = None
     cmass: bool = False
     do_rayleigh: bool = False
     corot: bool = False
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        element = 'corotTrussSection' if self.corot else 'trussSection'
+        element = "corotTrussSection" if self.corot else "trussSection"
         args = [element, self.tag, self.inode, self.jnode, self.section]
         if self.rho is not None:
-            args.extend(['-rho', self.rho])
+            args.extend(["-rho", self.rho])
         if self.cmass:
-            args.extend(['-cMass', self.cmass])
+            args.extend(["-cMass", self.cmass])
         if self.do_rayleigh:
-            args.extend(['-doRayleigh', self.do_rayleigh])
+            args.extend(["-doRayleigh", self.do_rayleigh])
         return self.format_objects(args, formats)
```

### Comparing `opswrapper-5.1.0/src/opswrapper/formatting.py` & `opswrapper-5.2.0/src/opswrapper/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from __future__ import annotations
 
 import dataclasses
 from typing import Dict, Union
 
 __all__ = [
-    'MultiFormatSpec',
-    'set_global_format_spec',
+    "MultiFormatSpec",
+    "set_global_format_spec",
 ]
 
 
 @dataclasses.dataclass
-class MultiFormatSpec():
+class MultiFormatSpec:
     """Specifiers for formatting of different types."""
+
     _spec: SpecDict = dataclasses.field(default_factory=dict)
 
     # Properties for temporary backwards compatibility
     @property
     def int(self):
         return self.get_format(1)
 
     @property
     def float(self):
         return self.get_format(1.0)
 
     def __repr__(self) -> str:
         clsname = self.__class__.__name__
-        specs = ', '.join([f'{cls.__name__}={fmt!r}' for cls, fmt in self._spec.items()])
-        return f'{clsname}({specs})'
+        specs = ", ".join(
+            [f"{cls.__name__}={fmt!r}" for cls, fmt in self._spec.items()]
+        )
+        return f"{clsname}({specs})"
 
     def copy(self):
         """Return a copy of the object."""
         the_copy = self.__class__()
         the_copy.update(self)
         return the_copy
 
@@ -76,41 +79,41 @@
         try:
             fmt = self._spec[obj.__class__]
         except KeyError:
             for type, fmt in self._spec.items():
                 if isinstance(obj, type):
                     break
             else:
-                fmt = ''
+                fmt = ""
         return fmt
 
     def register_format(self, cls: type, fmt: str):
         """Register a format string for a given type.
 
         Parameters
         ----------
         cls : Type
             The type to register.
         fmt : str
             The format string to register.
         """
         if not isinstance(cls, type):
-            raise TypeError(f'cls must be a type, not a {cls.__class__!r}')
+            raise TypeError(f"cls must be a type, not a {cls.__class__!r}")
 
         self._spec[cls] = fmt
 
 
 SpecDict = Dict[type, str]
 SpecLike = Union[SpecDict, MultiFormatSpec]
 
 _GLOBAL_FORMAT_SPEC = MultiFormatSpec()
-_GLOBAL_FORMAT_SPEC.register_format(bool, 'd')
-_GLOBAL_FORMAT_SPEC.register_format(int, 'd')
-_GLOBAL_FORMAT_SPEC.register_format(float, 'g')
-_GLOBAL_FORMAT_SPEC.register_format(str, '')
+_GLOBAL_FORMAT_SPEC.register_format(bool, "d")
+_GLOBAL_FORMAT_SPEC.register_format(int, "d")
+_GLOBAL_FORMAT_SPEC.register_format(float, ".12g")
+_GLOBAL_FORMAT_SPEC.register_format(str, "")
 
 
 def set_global_format_spec(formats: SpecDict):
     """Set the global default format specifiers.
 
     Parameters
     ----------
```

### Comparing `opswrapper-5.1.0/src/opswrapper/integrator.py` & `opswrapper-5.2.0/src/opswrapper/integrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import dataclasses
 import typing as t
 
 from .base import OpenSeesObject
 
 __all__ = [
-    'ArcLength',
-    'CentralDifference',
-    'DisplacementControl',
-    'HHT',
-    'Integrator',
-    'LoadControl',
-    'MinUnbalDispNorm',
-    'Newmark',
-    'StaticIntegrator',
-    'TransientIntegrator',
+    "ArcLength",
+    "CentralDifference",
+    "DisplacementControl",
+    "HHT",
+    "Integrator",
+    "LoadControl",
+    "MinUnbalDispNorm",
+    "Newmark",
+    "StaticIntegrator",
+    "TransientIntegrator",
 ]
 
 
 class Integrator(OpenSeesObject):
     def tcl_code(self, formats=None) -> str:
-        return ' '.join(['integrator', *self.tcl_args(formats)])
+        return " ".join(["integrator", *self.tcl_args(formats)])
 
 
-#===================================================================================================
+# ======================================================================================
 # Static integrators
-#===================================================================================================
+# ======================================================================================
 class StaticIntegrator(Integrator):
     pass
 
 
 @dataclasses.dataclass
 class LoadControl(StaticIntegrator):
     """
@@ -51,23 +51,24 @@
        the load patterns. If the only active loads acting on the domain are in
        load patterns with a Linear time series with a factor of 1.0, this
        integrator is the same as the classical load control method.
     2. The optional arguments are supplied to speed up the step size in cases
        where convergence is too fast and slow down the step size in cases where
        convergence is too slow.
     """
+
     incr: float
     num_iters: int = 1
     min_incr: float = None
     max_incr: float = None
 
     def tcl_args(self, formats=None) -> t.List[str]:
         min_incr = self.incr if self.min_incr is None else self.min_incr
         max_incr = self.incr if self.max_incr is None else self.max_incr
-        args = ['LoadControl', self.incr, self.num_iters, min_incr, max_incr]
+        args = ["LoadControl", self.incr, self.num_iters, min_incr, max_incr]
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class DisplacementControl(StaticIntegrator):
     """
     Parameters
@@ -83,26 +84,27 @@
         The number of iterations the user would like to occur in the solution
         algorithm. (default: 1)
     min_incr : float, optional
         The minimum step size to allow. (default: `incr`)
     max_incr : float, optional
         The maximum step size to allow. (default: `incr`)
     """
+
     node: int
     dof: int
     incr: float
     num_iters: int = 1
     min_incr: float = None
     max_incr: float = None
 
     def tcl_args(self, formats=None) -> t.List[str]:
         min_incr = self.incr if self.min_incr is None else self.min_incr
         max_incr = self.incr if self.max_incr is None else self.max_incr
         args = [
-            'DisplacementControl',
+            "DisplacementControl",
             self.node,
             self.dof,
             self.incr,
             self.num_iters,
             min_incr,
             max_incr,
         ]
@@ -127,23 +129,24 @@
         Factor relating first load increment at subsequent time steps.
         (default: 1.0)
     min_incr : float, optional
         Minimum load increment. (default: `incr`)
     max_incr : float, optional
         Maximum load increment. (default: `incr`)
     """
+
     incr: float
     Jd: float = 1.0
     min_incr: float = None
     max_incr: float = None
 
     def tcl_args(self, formats=None) -> t.List[str]:
         min_incr = self.incr if self.min_incr is None else self.min_incr
         max_incr = self.incr if self.max_incr is None else self.max_incr
-        args = ['MinUnbalDispNorm', self.incr, self.Jd, min_incr, max_incr]
+        args = ["MinUnbalDispNorm", self.incr, self.Jd, min_incr, max_incr]
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
 class ArcLength(StaticIntegrator):
     """Static integrator using the arc length scheme.
 
@@ -157,24 +160,25 @@
     Parameters
     ----------
     s : float
         Arc length.
     alpha : float
         Scaling factor on the reference loads.
     """
+
     s: float
     alpha: float
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        return self.format_objects(['ArcLength', self.s, self.alpha], formats)
+        return self.format_objects(["ArcLength", self.s, self.alpha], formats)
 
 
-#===================================================================================================
+# ======================================================================================
 # Transient integrators
-#===================================================================================================
+# ======================================================================================
 class TransientIntegrator(Integrator):
     pass
 
 
 @dataclasses.dataclass
 class CentralDifference(TransientIntegrator):
     """Explicit integration by the central difference method.
@@ -183,16 +187,17 @@
     -----
     1. As an explicit integration method, the calculation of U_(t + Δt) is based
        on the equilibrium equation at time t.
     2. If there is no Rayleigh damping and the C matrix is 0, for a diagonal
        mass matrix a diagonal solver can (and should) be used.
     3. For stability, Δt/Tn < 1/π.
     """
+
     def tcl_args(self, formats) -> t.List[str]:
-        return ['CentralDifference']
+        return ["CentralDifference"]
 
 
 @dataclasses.dataclass
 class Newmark(TransientIntegrator):
     """Newmark integration.
 
     Parameters
@@ -211,19 +216,20 @@
     2. Two common sets of choices are
        - Average Acceleration Method (γ = 1/2, β = 1/4)
        - Linear Acceleration Method (γ = 1/2, β = 1/6)
     3. γ > 1/2 results in numerical damping proportional to γ - 1/2
     4. The method is second order accurate if and only if γ = 1/2
     5. The method is conditionally stable for β >= γ/2 >= 1/4
     """
+
     gamma: float
     beta: float
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        return self.format_objects(['Newmark', self.gamma, self.beta], formats)
+        return self.format_objects(["Newmark", self.gamma, self.beta], formats)
 
 
 @dataclasses.dataclass
 class HHT(TransientIntegrator):
     """Hilber-Hughes-Taylor integrator.
 
     HHT is a one-step implicit method that allows for energy dissipation and
@@ -245,27 +251,28 @@
     -----
     1. α = 1.0 corresponds to the Newmark method.
     2. α should be between 2/3 and 1.0. The smaller the α, the greater the
        numerical damping.
     3. The default values for γ and β ensure the method is second-order accurate
        and unconditionally stable when α is between 2/3 and 1.
     """
+
     alpha: float
     gamma: float = None
     beta: float = None
 
     @property
     def default_gamma(self):
-        return 0.25*(2 - self.alpha)**2
+        return 0.25 * (2 - self.alpha) ** 2
 
     @property
     def default_beta(self):
         return 1.5 - self.alpha
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['HHT', self.alpha]
+        args = ["HHT", self.alpha]
         if self.gamma is not None or self.beta is not None:
             # OpenSees wants gamma and beta both specified if either is not default
             args.append(self.gamma if self.gamma is not None else self.default_gamma)
             args.append(self.beta if self.beta is not None else self.default_beta)
 
         return self.format_objects(args, formats)
```

### Comparing `opswrapper-5.1.0/src/opswrapper/material.py` & `opswrapper-5.2.0/src/opswrapper/material.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 @dataclasses.dataclass
 class UniaxialMaterial(base.OpenSeesObject):
     tag: int
 
     def tcl_code(self, formats=None) -> str:
-        return 'uniaxialMaterial ' + ' '.join(self.tcl_args(formats))
+        return "uniaxialMaterial " + " ".join(self.tcl_args(formats))
 
 
-#===================================================================================================
+# ======================================================================================
 # Elastic-ish materials
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class Elastic(UniaxialMaterial):
     """Elastic uniaxial material.
 
     Wraps the OpenSees Tcl command Elastic:
 
         uniaxialMaterial Elastic $matTag $E <$eta> <$Eneg>
@@ -32,20 +32,21 @@
     E : float
         Tangent/modulus of elasticity
     eta : float, optional
         Damping tangent (default = 0.0)
     Eneg : float, optional
         Tangent in compression (default = E)
     """
+
     E: float
     eta: float = 0.0
     Eneg: float = None
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['Elastic', self.tag, self.E]
+        args = ["Elastic", self.tag, self.E]
         if self.Eneg is not None:
             args.append(self.eta)
             args.append(self.Eneg)
         elif self.eta != 0.0:
             args.append(self.eta)
 
         return self.format_objects(args, formats)
@@ -69,21 +70,22 @@
         Strain/deformation at which the material reaches plastic state in tension.
     eps_yN : float, optional
         Strain/deformation at which the material reaches plastic state in compression.
         (default = eps_y)
     eps0 : float, optional
         Initial strain/deformation. (default = 0.0)
     """
+
     E: float
     eps_y: float
     eps_yN: float = None
     eps0: float = 0.0
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['ElasticPP', self.tag, self.E, self.eps_y]
+        args = ["ElasticPP", self.tag, self.E, self.eps_y]
         eps_yN = self.eps_yN if self.eps_yN is not None else self.eps_y
         if self.eps0 != 0.0:
             args.append(eps_yN)
             args.append(self.eps0)
         elif self.eps_yN is not None:
             args.append(eps_yN)
 
@@ -109,38 +111,39 @@
     h_iso : float
         Isotropic hardening modulus.
     h_kin : float
         Kinematic hardening modulus.
     eta : float, optional
         Visco-plastic coefficient. (default = 0.0)
     """
+
     E: float
     sigma_y: float
     h_iso: float
     h_kin: float
     eta: float = 0.0
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [
-            'Hardening',
+            "Hardening",
             self.tag,
             self.E,
             self.sigma_y,
             self.h_iso,
             self.h_kin,
         ]
         if self.eta != 0.0:
             args.append(self.eta)
 
         return self.format_objects(args, formats)
 
 
-#===================================================================================================
+# ======================================================================================
 # Steels
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class Steel01(UniaxialMaterial):
     """Bilinear steel model with optional isotropic hardening.
 
     Wraps the OpenSees Tcl command Steel01:
 
         uniaxialMaterial Steel01 $matTag $Fy $E0 $b <$a1 $a2 $a3 $a4>
@@ -162,14 +165,15 @@
         Isotropic hardening parameter; see `a1`.
     a3 : float, optional
         Isotropic hardening parameter; increase of tension yield envelope as
         proportion of yield strength after a plastic strain of a4*Fy/E0.
     a4 : float, optional
         Isotropic hardening parameter; see `a3`.
     """
+
     Fy: float
     E: float
     b: float
     a1: float = None
     a2: float = None
     a3: float = None
     a4: float = None
@@ -177,19 +181,21 @@
     def _num_iso_params_defined(self):
         return sum([a is not None for a in (self.a1, self.a2, self.a3, self.a4)])
 
     def __post_init__(self):
         super().__post_init__()
         nparams = self._num_iso_params_defined()
         if nparams not in [0, 4]:
-            raise ValueError('Steel01: isometric hardening definition incomplete '
-                             f'(expected 4 params, got {nparams})')
+            raise ValueError(
+                "Steel01: isometric hardening definition incomplete "
+                f"(expected 4 params, got {nparams})"
+            )
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['Steel01', self.tag, self.Fy, self.E, self.b]
+        args = ["Steel01", self.tag, self.Fy, self.E, self.b]
         if self._num_iso_params_defined() == 4:
             args.extend([self.a1, self.a2, self.a3, self.a4])
 
         return self.format_objects(args, formats)
 
 
 @dataclasses.dataclass
@@ -231,14 +237,15 @@
         (default: 0.0)
     a4 : float, optional
         Isotropic hardening parameter; see `a3`. (default: 1.0)
     sigma_i : float, optional
         Initial stress. Initial strain is not zero; it is calculated from
         sigma_i/E. (default: 0.0)
     """
+
     Fy: float
     E: float
     b: float
     R0: float = 20
     cR1: float = 0.925
     cR2: float = 0.15
     a1: float = None
@@ -248,15 +255,15 @@
     sigma_i: float = None
 
     def _num_iso_params_defined(self):
         return sum([a is not None for a in (self.a1, self.a2, self.a3, self.a4)])
 
     def tcl_args(self, formats=None) -> t.List[str]:
         args = [
-            'Steel02',
+            "Steel02",
             self.tag,
             self.Fy,
             self.E,
             self.b,
             self.R0,
             self.cR1,
             self.cR2,
@@ -270,17 +277,17 @@
                 args.extend([self.a1, self.a2, self.a3, self.a4, self.sigma_i])
         elif n_iso_params == 4:
             args.extend([self.a1, self.a2, self.a3, self.a4])
 
         return self.format_objects(args, formats)
 
 
-#===================================================================================================
+# ======================================================================================
 # Deterioration models
-#===================================================================================================
+# ======================================================================================
 @dataclasses.dataclass
 class Bilin(UniaxialMaterial):
     """Deterioration model with bilinear hysteretic response.
 
     Parameters
     ----------
     tag : int
@@ -340,14 +347,15 @@
         Rate of cyclic deterioration in the negative loading direction. This
         parameter is used to create asymmetric hysteretic behavior in the case
         of a composite beam. For symmetric hysteretic response use 1.0.
     nfactor : float, optional
         Elastic stiffness amplification factor, mainly for use with concentrated
         plastic hinge elements. (default: 0.0)
     """
+
     K0: float
     as_plus: float
     as_neg: float
     My_plus: float
     My_neg: float
     lambda_s: float
     lambda_c: float
@@ -366,16 +374,17 @@
     theta_u_plus: float
     theta_u_neg: float
     D_plus: float = 1.0
     D_neg: float = 1.0
     nfactor: float = None
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        args = ['Bilin']
+        args = ["Bilin"]
         args += [
-            getattr(self, field.name) for field in dataclasses.fields(self)
-            if field.name not in ('nfactor', )
+            getattr(self, field.name)
+            for field in dataclasses.fields(self)
+            if field.name not in ("nfactor",)
         ]
         if self.nfactor is not None:
             args.append(self.nfactor)
 
         return self.format_objects(args, formats)
```

### Comparing `opswrapper-5.1.0/src/opswrapper/model.py` & `opswrapper-5.2.0/src/opswrapper/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Basic OpenSees modeling commands."""
 
 import dataclasses
+from typing import Iterable, Optional, Union
 
 import numpy as np
 
 from . import base
 from .utils import coerce_numeric
 
 __all__ = [
@@ -12,55 +13,62 @@
     "Node",
 ]
 
 
 @dataclasses.dataclass
 class Model(base.OpenSeesObject):
     """Model constructor.
-    
+
     Parameters
     ----------
     ndm: int
         Number of dimensions.
     ndf: int
         Number of degrees-of-freedom per node.
     """
+
     ndm: int
     ndf: int
 
     def tcl_code(self, formats=None) -> str:
-        args = ['model', 'basic', '-ndm', self.ndm, '-ndf', self.ndf]
-        return ' '.join(self.format_objects(args, formats))
+        args = ["model", "basic", "-ndm", self.ndm, "-ndf", self.ndf]
+        return " ".join(self.format_objects(args, formats))
 
 
 @dataclasses.dataclass(init=False)
 class Node(base.OpenSeesObject):
     """Node in the model.
-    
+
     Parameters
     ----------
     tag : int
         Integer tag identifying the node.
     *coords : float
         NDM coordinates of the node.
     mass : tuple, optional
         NDF-length tuple of nodal masses.
     """
+
     tag: int
-    coords: tuple
-    mass: tuple = None
+    coords: np.ndarray
+    mass: Optional[np.ndarray] = None
 
-    def __init__(self, tag, *coords, mass=None):
+    def __init__(
+        self,
+        tag: int,
+        *coords: Union[float, Iterable[float]],
+        mass: Optional[Iterable[float]] = None
+    ):
         super().__init__()
         self.tag = tag
         self.coords = np.array(coords).flatten()
         if mass is not None:
             mass = np.array(mass).flatten()
         self.mass = mass
 
     def tcl_code(self, formats=None) -> str:
-        args = ['node', self.tag]
+        args = ["node", self.tag]
         args.extend([coerce_numeric(c, float) for c in self.coords])
         if self.mass is not None:
-            args.append('-mass')
+            args.append("-mass")
             args.extend([coerce_numeric(m, float) for m in self.mass])
-        return ' '.join(self.format_objects(args, formats))
+        return " ".join(self.format_objects(args, formats))
```

### Comparing `opswrapper-5.1.0/src/opswrapper/output.py` & `opswrapper-5.2.0/src/opswrapper/output.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,54 +40,58 @@
     Example
     -------
     >>> ElementRecorder(file='/path/to/file', elements=1, dofs=[1, 2],
     ... response='localForce').tcl_code()
     'recorder Element -file {/path/to/file} -ele 1 -dof 1 2 localForce'
     """
     file: Optional[Union[str, Path]] = None
-    fileformat: str = 'file'
+    fileformat: str = "file"
     precision: int = None
     elements: np.ndarray = None
     region: int = None
     dofs: np.ndarray = None
     response: str = None
 
     def __post_init__(self):
-        if self.fileformat not in ['file', 'xml', 'binary']:
+        if self.fileformat not in ["file", "xml", "binary"]:
             raise ValueError(
                 "ElementRecorder: given file format is not recognized "
                 f"(expected one of 'file', 'xml', 'binary'; got {self.fileformat!r}"
             )
 
     def tcl_code(self, formats=None) -> str:
-        args = ['recorder Element', f'-{self.fileformat}']
+        args = ["recorder Element", f"-{self.fileformat}"]
 
         file_arg, tcl_list_expansion = _format_file_arg(self.file)
         args.append(file_arg)
 
-        if str(self.elements) == 'all':
-            args.append(f'-ele {tcl_list_expansion}[getEleTags]')
+        if str(self.elements) == "all":
+            args.append(f"-ele {tcl_list_expansion}[getEleTags]")
         elif self.elements is not None:
-            args.append('-ele')
-            args.extend(utils.coerce_numeric(tag, int) for tag in np.asarray(self.elements).flat)
+            args.append("-ele")
+            args.extend(
+                utils.coerce_numeric(tag, int) for tag in np.asarray(self.elements).flat
+            )
 
         if self.region is not None:
-            args.append('-region')
+            args.append("-region")
             args.append(self.region)
 
         if self.precision is not None:
-            args.append('-precision')
+            args.append("-precision")
             args.append(self.precision)
 
         if self.dofs is not None:
-            args.append('-dof')
-            args.extend(utils.coerce_numeric(dof, int) for dof in np.asarray(self.dofs).flat)
+            args.append("-dof")
+            args.extend(
+                utils.coerce_numeric(dof, int) for dof in np.asarray(self.dofs).flat
+            )
 
         args.append(self.response)
-        return ' '.join(self.format_objects(args, formats))
+        return " ".join(self.format_objects(args, formats))
 
 
 @dataclasses.dataclass
 class NodeRecorder(base.OpenSeesObject):
     R"""Node recorder.
 
     Parameters
@@ -139,76 +143,80 @@
 
     Example
     -------
     >>> NodeRecorder(file='/path/to/file', nodes=1, dofs=[1, 2], response='disp').tcl_code()
     'recorder Node -file {/path/to/file} -node 1 -dof 1 2 disp'
     """
     file: Optional[Union[str, Path]] = None
-    fileformat: str = 'file'
+    fileformat: str = "file"
     precision: int = None
     time_series: int = None
     time: bool = False
     nodes: np.ndarray = None
     node_range: np.ndarray = None
     region: int = None
     dofs: np.ndarray = None
     response: str = None
 
     def __post_init__(self):
-        if self.fileformat not in ['file', 'xml', 'binary']:
+        if self.fileformat not in ["file", "xml", "binary"]:
             raise ValueError(
                 "NodeRecorder: given file format is not recognized "
                 f"(expected one of 'file', 'xml', 'binary'; got {self.fileformat!r}"
             )
 
     def tcl_code(self, formats=None) -> str:
-        args = ['recorder Node', f'-{self.fileformat}']
+        args = ["recorder Node", f"-{self.fileformat}"]
 
         file_arg, tcl_list_expansion = _format_file_arg(self.file)
         args.append(file_arg)
 
         if self.precision is not None:
-            args.append('-precision')
+            args.append("-precision")
             args.append(self.precision)
 
         if self.time_series is not None:
-            args.append('-timeSeries')
+            args.append("-timeSeries")
             args.append(self.time_series)
 
         if self.time:
-            args.append('-time')
+            args.append("-time")
 
-        if str(self.nodes) == 'all':
-            args.append(f'-node {tcl_list_expansion}[getNodeTags]')
+        if str(self.nodes) == "all":
+            args.append(f"-node {tcl_list_expansion}[getNodeTags]")
         elif self.nodes is not None:
-            args.append('-node')
-            args.extend(utils.coerce_numeric(tag, int) for tag in np.asarray(self.nodes).flat)
+            args.append("-node")
+            args.extend(
+                utils.coerce_numeric(tag, int) for tag in np.asarray(self.nodes).flat
+            )
 
         if self.node_range is not None:
-            args.append('-nodeRange')
+            args.append("-nodeRange")
             args.extend(self.node_range)
 
         if self.region is not None:
-            args.append('-region')
+            args.append("-region")
             args.append(self.region)
 
         if self.dofs is not None:
-            args.append('-dof')
-            args.extend(utils.coerce_numeric(dof, int) for dof in np.asarray(self.dofs).flat)
+            args.append("-dof")
+            args.extend(
+                utils.coerce_numeric(dof, int) for dof in np.asarray(self.dofs).flat
+            )
 
         args.append(self.response)
-        return ' '.join(self.format_objects(args, formats))
+        return " ".join(self.format_objects(args, formats))
 
 
 def _format_file_arg(file: Union[str, Path] = None) -> Tuple[str, str]:
     if file is None:
         # Escape enclosing brackets for a total of three brackets on either side
-        file_arg = '{{{file}}}'
+        file_arg = "{{{file}}}"
         # If the returned string is being returned with '{file}' in it to be formatted later,
         # need to escape the brackets in the list expansion operator. Otherwise, a completely
         # baffling KeyError will be raised when calling '.format'.
-        tcl_list_expansion = '{{*}}'
+        tcl_list_expansion = "{{*}}"
     else:
         file = utils.path_for_tcl(file)
-        file_arg = '{%s}' % file
-        tcl_list_expansion = '{*}'
+        file_arg = "{%s}" % file
+        tcl_list_expansion = "{*}"
     return file_arg, tcl_list_expansion
```

### Comparing `opswrapper-5.1.0/src/opswrapper/section.py` & `opswrapper-5.2.0/src/opswrapper/section.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 @dataclasses.dataclass
 class Section(base.OpenSeesObject):
     tag: int
 
     def tcl_code(self, formats=None) -> str:
-        return 'section ' + ' '.join(self.tcl_args(formats))
+        return "section " + " ".join(self.tcl_args(formats))
 
 
 @dataclasses.dataclass
 class Elastic2D(Section):
     """Elastic section for 2D analysis.
 
     Shear deformations may be included by specifying `G` and `alphaY`.
@@ -31,26 +31,27 @@
     G : float, optional
         Shear modulus of the section. Both `G` and `alphaY` must be set to
         create a section with shear deformations. (default: None)
     alphaY : float, optional
         Shear shape factor. Both `G` and `alphaY` must be set to create a
         section with shear deformations. (default: None)
     """
+
     E: float
     A: float
     Iz: float
     G: float = None
     alphaY: float = None
 
     def tcl_code(self, formats=None) -> str:
         fmt = self.get_format_spec(formats)
         i, f = fmt.int, fmt.float
-        code = f'section Elastic {self.tag:{i}} {self.E:{f}} {self.A:{f}} {self.Iz:{f}}'
+        code = f"section Elastic {self.tag:{i}} {self.E:{f}} {self.A:{f}} {self.Iz:{f}}"
         if self.G is not None and self.alphaY is not None:
-            code += f' {self.G:{f}} {self.alphaY:{f}}'
+            code += f" {self.G:{f}} {self.alphaY:{f}}"
         return code
 
 
 @dataclasses.dataclass
 class Elastic3D(Section):
     """Elastic section for 3D analysis.
 
@@ -75,52 +76,55 @@
     alphaY : float, optional
         Shear shape factor along the local y-axis. Both `alphaY` and `alphaZ`
         must be set to create a section with shear deformations. (default: None)
     alphaZ : float, optional
         Shear shape factor along the local z-axis. Both `alphaY` and `alphaZ`
         must be set to create a section with shear deformations. (default: None)
     """
+
     E: float
     A: float
     Iz: float
     Iy: float
     G: float
     J: float
     alphaY: float = None
     alphaZ: float = None
 
     def tcl_code(self, formats=None) -> str:
         fmt = self.get_format_spec(formats)
         i, f = fmt.int, fmt.float
         code = (
-            f'section Elastic {self.tag:{i}} {self.E:{f}} {self.A:{f}}'
-            f' {self.Iz:{f}} {self.Iy:{f}} {self.G:{f}} {self.J:{f}}'
+            f"section Elastic {self.tag:{i}} {self.E:{f}} {self.A:{f}}"
+            f" {self.Iz:{f}} {self.Iy:{f}} {self.G:{f}} {self.J:{f}}"
         )
         if self.alphaY is not None and self.alphaZ is not None:
-            code += f' {self.alphaY:{f}} {self.alphaZ:{f}}'
+            code += f" {self.alphaY:{f}} {self.alphaZ:{f}}"
         return code
 
 
-#===================================================================================================
+# ======================================================================================
 # Fiber section
-#===================================================================================================
+# ======================================================================================
 class FiberSectionCommand(base.OpenSeesObject):
     def tcl_code(self, formats=None) -> str:
-        return ' '.join(self.tcl_args(formats))
+        return " ".join(self.tcl_args(formats))
 
 
 @dataclasses.dataclass
 class fiber(FiberSectionCommand):
     y: float
     z: float
     A: float
     mat: int
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        return self.format_objects(['    fiber', self.y, self.z, self.A, self.mat], formats)
+        return self.format_objects(
+            ["    fiber", self.y, self.z, self.A, self.mat], formats
+        )
 
 
 @dataclasses.dataclass
 class patch_quad(FiberSectionCommand):
     mat: int
     nfIJ: int
     nfJK: int
@@ -130,34 +134,59 @@
     zJ: float
     yK: float
     zK: float
     yL: float
     zL: float
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        return self.format_objects([
-            '    patch', 'quad', self.mat, self.nfIJ, self.nfJK, self.yI, self.zI, self.yJ, self.zJ,
-            self.yK, self.zK, self.yL, self.zL
-        ], formats)
+        return self.format_objects(
+            [
+                "    patch",
+                "quad",
+                self.mat,
+                self.nfIJ,
+                self.nfJK,
+                self.yI,
+                self.zI,
+                self.yJ,
+                self.zJ,
+                self.yK,
+                self.zK,
+                self.yL,
+                self.zL,
+            ],
+            formats,
+        )
 
 
 @dataclasses.dataclass
 class patch_rect(FiberSectionCommand):
     mat: int
     nfY: int
     nfZ: int
     yI: float
     zI: float
     yJ: float
     zJ: float
 
     def tcl_args(self, formats=None) -> t.List[str]:
-        return self.format_objects([
-            '    patch', 'rect', self.mat, self.nfY, self.nfZ, self.yI, self.zI, self.yJ, self.zJ
-        ], formats)
+        return self.format_objects(
+            [
+                "    patch",
+                "rect",
+                self.mat,
+                self.nfY,
+                self.nfZ,
+                self.yI,
+                self.zI,
+                self.yJ,
+                self.zJ,
+            ],
+            formats,
+        )
 
 
 @dataclasses.dataclass
 class Fiber(Section):
     """Fiber-based section.
 
     Commands that define the fibers can be passed in at construction or created
@@ -173,14 +202,15 @@
         List of commands that make up the section. (default: [])
 
     Example
     -------
     >>> ops.section.Fiber(1).fiber(0, 1, 1.0, 2).fiber(0, -1, 1.0, 2)
     Fiber(tag=1, GJ=None, commands=[fiber(y=0, z=1, A=1.0, mat=2), fiber(y=0, z=-1, A=1.0, mat=2)])
     """
+
     GJ: float = None
     commands: t.List[FiberSectionCommand] = dataclasses.field(default_factory=list)
 
     def fiber(self, y, z, A, mat):
         """Add a single fiber.
 
         Returns `self` to allow chained commands.
@@ -226,17 +256,21 @@
             yI, zI = coords[0]
             yJ, zJ = coords[1]
             yK, zK = coords[2]
             yL, zL = coords[3]
         elif len(coords) == 8:
             yI, zI, yJ, zJ, yK, zK, yL, zL = coords
         else:
-            raise ValueError("patch_quad: coords must either be 4 2-tuples or 8 coordinates")
+            raise ValueError(
+                "patch_quad: coords must either be 4 2-tuples or 8 coordinates"
+            )
 
-        self.commands.append(patch_quad(mat, nfIJ, nfJK, yI, zI, yJ, zJ, yK, zK, yL, zL))
+        self.commands.append(
+            patch_quad(mat, nfIJ, nfJK, yI, zI, yJ, zJ, yK, zK, yL, zL)
+        )
         return self
 
     def patch_rect(self, mat, nfY, nfZ, *coords):
         """Add a rectangular patch of fibers.
 
         The patch is defined by the vertices I and J which define the lower left
         and upper right corners, respectively.
@@ -259,26 +293,28 @@
         """
         if len(coords) == 2:
             yI, zI = coords[0]
             yJ, zJ = coords[1]
         elif len(coords) == 4:
             yI, zI, yJ, zJ = coords
         else:
-            raise ValueError("patch_rect: coords must either be 2 2-tuples or 4 coordinates")
+            raise ValueError(
+                "patch_rect: coords must either be 2 2-tuples or 4 coordinates"
+            )
 
         self.commands.append(patch_rect(mat, nfY, nfZ, yI, zI, yJ, zJ))
         return self
 
     def tcl_code(self, formats=None) -> str:
-        args = ['section', 'Fiber', self.tag]
+        args = ["section", "Fiber", self.tag]
         if self.GJ is not None:
-            args.append('-GJ')
+            args.append("-GJ")
             args.append(self.GJ)
-        args.append('{')
-        section_command = ' '.join(self.format_objects(args, formats))
+        args.append("{")
+        section_command = " ".join(self.format_objects(args, formats))
 
         code = [
             section_command,
             *self.commands,
-            '}',
+            "}",
         ]
-        return '\n'.join(self.format_objects(code, formats))
+        return "\n".join(self.format_objects(code, formats))
```

### Comparing `opswrapper-5.1.0/src/opswrapper/test.py` & `opswrapper-5.2.0/src/opswrapper/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,26 @@
              BUT RETURN A SUCCESSFUL TEST.
     norm_type : int, optional
         Type of norm. 0 = max-norm, 1 = 1-norm, 2 = 2-norm, etc. (default: 2)"""
 
 
 class PrintFlag(IntEnum):
     """Print flag for convergence tests.
-    
+
     Options
     -------
     - 0: print nothing
     - 1: print information on norms each time `test()` is invoked
     - 2: print information on norms and number of iterations at end of
          successful test
     - 4: print norms at each step and also the ΔU and R(U) vectors.
     - 5: if test fails to converge after `max_iters`, print an error message
          BUT RETURN A SUCCESSFUL TEST.
     """
+
     NOTHING = 0
     NORMS = 1
     NORMS_AND_ITERS = 2
     NORMS_AND_VECS = 4
     IGNORE_ERROR = 5
 
 
@@ -50,15 +51,15 @@
 class Test(OpenSeesObject):
     tolerance: float
     max_iters: int
     print_flag: int = PrintFlag.NOTHING
     norm_type: int = 2
 
     def tcl_code(self, formats=None) -> str:
-        return ' '.join(['test', *self.tcl_args(formats=formats)])
+        return " ".join(["test", *self.tcl_args(formats=formats)])
 
     def tcl_args(self, formats=None) -> t.List[str]:
         method = self.__class__.__name__
         print_flag = PrintFlag(self.print_flag)
         args = [method, self.tolerance, self.max_iters, print_flag, self.norm_type]
         return self.format_objects(args, formats)
 
@@ -278,8 +279,8 @@
     This integrator is testing::
 
         [ΔUi * R(Ui)] / [ΔU0 * R(U0)] < tol
     """
 
 
 for subclass in Test.__subclasses__():
-    subclass.__doc__ %= {'parameters': _standard_test_parameters}
+    subclass.__doc__ %= {"parameters": _standard_test_parameters}
```

### Comparing `opswrapper-5.1.0/src/opswrapper/uniaxialmaterialanalysis.py` & `opswrapper-5.2.0/src/opswrapper/uniaxialmaterialanalysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,28 +29,29 @@
     opensees_path : pathlib.Path, optional
         Path to the OpenSees binary to use. If None, uses the value from the
         global configuration. (default: None)
     scratch_path : pathlib.Path, optional
         Path to the directory for storing temporary files. If None, uses the
         value from the global configuration. (default: None)
     """
+
     def __init__(
         self,
         material,
         tag=1,
         echo_output=False,
         delete_files=True,
         opensees_path=None,
-        scratch_path=None
+        scratch_path=None,
     ):
         super().__init__(
             echo_output=echo_output,
             delete_files=delete_files,
             opensees_path=opensees_path,
-            scratch_path=scratch_path
+            scratch_path=scratch_path,
         )
         self.material = material
         self.tag = tag
 
     def _process_material_definition(self):
         """Sanitize the given material definition into a list of str."""
         try:
@@ -62,15 +63,15 @@
 
     def run_analysis(
         self,
         peak_points,
         rate_type: str = None,
         rate_value: float = None,
         echo: bool = None,
-        analysis_id: str = None
+        analysis_id: str = None,
     ):
         """
         Parameters
         ----------
         peak_points : array_like
             Peak displacements (strains) to cycle between.
         rate_type : {'StrainRate', 'Steps', None}, default None
@@ -94,82 +95,84 @@
         """
         peak_points = np.array(peak_points)
         results = xr.Dataset()
 
         # Filenames
         scratch_file = self.create_scratch_filer(analysis_id)
         files = utils.Namespace()
-        files.input = scratch_file('input', '.tcl')
-        files.pattern = scratch_file('pattern', '.dat')
-        files.output_force = scratch_file('output_force', '.dat')
-        files.output_disp = scratch_file('output_disp', '.dat')
-        files.output_stiff = scratch_file('output_stiff', '.dat')
+        files.input = scratch_file("input", ".tcl")
+        files.pattern = scratch_file("pattern", ".dat")
+        files.output_force = scratch_file("output_force", ".dat")
+        files.output_disp = scratch_file("output_disp", ".dat")
+        files.output_stiff = scratch_file("output_stiff", ".dat")
 
-        numbers = self._generate_imposed_displacement(peak_points, rate_type, rate_value)
+        numbers = self._generate_imposed_displacement(
+            peak_points, rate_type, rate_value
+        )
         numsteps = numbers.size - 2
 
-        pattern_filepath = '{' + utils.path_for_tcl(files.pattern) + '}'
+        pattern_filepath = "{" + utils.path_for_tcl(files.pattern) + "}"
         new_recorder = functools.partial(ElementRecorder, precision=10, elements=1)
         material_definition = self._process_material_definition()
         model = [
             Model(ndm=1, ndf=1),
             Node(1, 0.0),
             Node(2, 1.0),
-            'fix 1 1',
+            "fix 1 1",
             *material_definition,
             element.Truss(1, 1, 2, 1.0, mat=self.tag),
             f'pattern Plain 1 "Series -dt 1.0 -filePath {pattern_filepath} -factor 1.0" {{',
-            '    sp 2 1 1.0',
-            '}',
-            new_recorder(file=files.output_force, response='force'),
-            new_recorder(file=files.output_disp, response='deformations'),
-            new_recorder(file=files.output_stiff, response='stiff'),
-            'system UmfPack',
+            "    sp 2 1 1.0",
+            "}",
+            new_recorder(file=files.output_force, response="force"),
+            new_recorder(file=files.output_disp, response="deformations"),
+            new_recorder(file=files.output_stiff, response="stiff"),
+            "system UmfPack",
             constraints.Transformation(),
             test.NormDispIncr(tolerance=1e-8, max_iters=10, print_flag=0),
-            'algorithm Newton',
-            'numberer RCM',
-            'integrator LoadControl 1.0',
-            'analysis Static',
-            f'set ok [analyze {numsteps:d}]',
-            'if {$ok != 0} {exit 2}',
-            'exit 1',
+            "algorithm Newton",
+            "numberer RCM",
+            "integrator LoadControl 1.0",
+            "analysis Static",
+            f"set ok [analyze {numsteps:d}]",
+            "if {$ok != 0} {exit 2}",
+            "exit 1",
         ]
 
         # Write files to disk
         np.savetxt(files.pattern, numbers)
         utils.print_model(model, file=files.input)
 
         # Run the analysis
         process = self.run_opensees(files.input, echo=echo)
         if process.returncode == 1:
-            status = 'Analysis successful'
+            status = "Analysis successful"
         elif process.returncode == 2:
-            status = 'Analysis failed'
+            status = "Analysis failed"
             warnings.warn("UniaxialMaterialAnalysis.run_analysis: analysis failed")
         else:
             raise RuntimeError(
                 f"Analysis ended in an unknown manner, exit code: {process.returncode}"
             )
 
         # Read results
         disp = np.loadtxt(files.output_disp)
-        results['disp'] = xr.DataArray(disp, dims='time')
+        results["disp"] = xr.DataArray(disp, dims="time")
 
         force = np.loadtxt(files.output_force)
-        results['force'] = xr.DataArray(force[:, 1], dims='time')
+        results["force"] = xr.DataArray(force[:, 1], dims="time")
 
         with warnings.catch_warnings() as cw:
-            warnings.simplefilter('ignore')
+            warnings.simplefilter("ignore")
             stiff = np.loadtxt(files.output_stiff)
         if len(stiff) != 0:
-            results['stiff'] = xr.DataArray(stiff, dims='time')
+            results["stiff"] = xr.DataArray(stiff, dims="time")
 
-        results.attrs['status'] = status
-        results.attrs['stdout'] = process.stdout
+        results.attrs["status"] = status
+        results.attrs["stdout"] = process.stdout
 
         # Cleanup
         if self.delete_files:
             for _, file in files:
                 try:
                     file.unlink()
                 except FileNotFoundError:
@@ -179,14 +182,14 @@
 
     @staticmethod
     def _generate_imposed_displacement(peak_points, rate_type=None, rate_value=None):
         if rate_type is not None and rate_value is None:
             raise TypeError("rate_value must be specified if rate_type is not None")
 
         rate = {
-            'StrainRate': lambda: rate_value,
-            'Steps': lambda: np.sum(np.abs(np.diff(peak_points)))/rate_value,
+            "StrainRate": lambda: rate_value,
+            "Steps": lambda: np.sum(np.abs(np.diff(peak_points))) / rate_value,
             None: lambda: np.max(np.abs(np.diff(peak_points))),
         }[rate_type]()
 
         numbers = utils.fill_out_numbers(peak_points, rate).flatten()
         return np.array([numbers[0], *numbers, numbers[-1]])
```

### Comparing `opswrapper-5.1.0/src/opswrapper/utils.py` & `opswrapper-5.2.0/src/opswrapper/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,29 +45,30 @@
 
     >>> files['input']
     'input.tcl'
     >>> files['output'] = 'output.csv'
     >>> files.output
     'output.csv'
     """
+
     def __iter__(self):
         return iter(self.__dict__.items())
 
     def __getitem__(self, key):
         return getattr(self, key)
 
     def __setitem__(self, key, value):
         setattr(self, key, value)
 
     def __delitem__(self, key):
         delattr(self, key)
 
 
 def path_for_tcl(path) -> str:
-    return str(path).replace('\\', '/')
+    return str(path).replace("\\", "/")
 
 
 def print_model(model: List[str], file=None):
     """Print a model definition to a file.
 
     Parameters
     ----------
@@ -80,38 +81,38 @@
     """
     try:
         file = Path(file)
         file_is_descriptor = False
     except TypeError:
         file_is_descriptor = True
 
-    modeltext = '\n'.join([str(line) for line in model])
+    modeltext = "\n".join([str(line) for line in model])
     if file_is_descriptor:
         print(modeltext, file=file)
     else:
-        with open(file, 'w') as f:
+        with open(file, "w") as f:
             print(modeltext, file=f)
 
 
 def tcllist(l: list) -> str:
     """Translate a Python list to the equivalent Tcl command.
 
     All elements in the list are quoted using brackets and will not support
     variable substitution. Do that on the Python side.
 
     Example:
     >>> tcllist([1.0, 2, "sam's the best!"])
     "[list {1.0} {2} {sam's the best!}]"
     """
-    list_items = ['{' + str(i) + '}' for i in l]
-    list_str = ' '.join(list_items)
-    return f'[list {list_str}]'
+    list_items = ["{" + str(i) + "}" for i in l]
+    list_str = " ".join(list_items)
+    return f"[list {list_str}]"
 
 
-def list_dataclass_fields(name, object, pad='', end='\n', exclude=None) -> str:
+def list_dataclass_fields(name, object, pad="", end="\n", exclude=None) -> str:
     """Represent the fields of a dataclass object.
 
     Parameters
     ----------
     name : str
         The name to use for the object in the representation.
     object : dataclass
@@ -128,21 +129,23 @@
     >>> print(list_dataclass_fields('gravity_columns', self.gravity_columns, pad=' '*8))
             gravity_columns.include          : True
             gravity_columns.num_points       : 4
             gravity_columns.material_model   : Steel01
             gravity_columns.strain_hardening : 0.01
     """
     fields = dataclasses.fields(object)
-    lenname = lambda f: len(getattr(f, 'name'))
+    lenname = lambda f: len(getattr(f, "name"))
     max_key_len = max(map(lenname, fields))
     l = []
     for field in fields:
         if exclude is not None and field.name in exclude:
             continue
-        l.append(f'{pad}{name}.{field.name.ljust(max_key_len)} : {getattr(object, field.name)!r}')
+        l.append(
+            f"{pad}{name}.{field.name.ljust(max_key_len)} : {getattr(object, field.name)!r}"
+        )
 
     return end.join(l)
 
 
 def fill_out_numbers(peaks, rate):
     """Fill in numbers between peaks.
 
@@ -176,27 +179,27 @@
         peaks = peaks.T
 
     numpeaks = peaks.shape[0]
     numbers = [peaks[0, :]]
 
     for i in range(numpeaks - 1):
         diff = peaks[i + 1, :] - peaks[i, :]
-        numsteps = int(np.maximum(2, 1 + np.ceil(np.max(np.abs(diff/rate)))))
+        numsteps = int(np.maximum(2, 1 + np.ceil(np.max(np.abs(diff / rate)))))
         numbers_to_add = np.linspace(peaks[i, :], peaks[i + 1, :], numsteps)
         numbers.append(numbers_to_add[1:, :])
 
     numbers = np.vstack(numbers)
     if 1 in numbers.shape:
         numbers = numbers.flatten()
 
     return numbers
 
 
-KT = TypeVar('KT')
-VT = TypeVar('VT')
+KT = TypeVar("KT")
+VT = TypeVar("VT")
 
 
 @dataclasses.dataclass
 class ValueTypeDispatch(Generic[KT, VT]):
     """Dispatch helper that raises TypeError.
 
     Parameters
@@ -213,17 +216,20 @@
     ...                                       'initial': '-initial'})
     >>> tangent_dispatch['initial']
     '-initial'
     >>> tangent_dispatch['not_a_tangent']
     <Traceback>
     TypeError: Invalid tangent 'not_a_tangent'; must be one of ['current', 'initial']
     """
+
     name: str
     dispatch: Mapping[KT, VT]
 
     def __getitem__(self, key: KT) -> VT:
         try:
             value = self.dispatch[key]
         except KeyError as exc:
             valid = list(self.dispatch)
-            raise TypeError(f'Invalid {self.name} {key!r}; must be one of {valid!r}') from exc
+            raise TypeError(
+                f"Invalid {self.name} {key!r}; must be one of {valid!r}"
+            ) from exc
         return value
```

### Comparing `opswrapper-5.1.0/src/opswrapper.egg-info/PKG-INFO` & `opswrapper-5.2.0/src/opswrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswrapper
-Version: 5.1.0
+Version: 5.2.0
 Summary: Python helpers for writing OpenSees scripts.
 Home-page: https://github.com/otaithleigh/opswrapper
 Author: Peter Talley
 Author-email: ptalley2@vols.utk.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opswrapper-5.1.0/src/opswrapper.egg-info/SOURCES.txt` & `opswrapper-5.2.0/src/opswrapper.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/opswrapper.egg-info/SOURCES.txt
 src/opswrapper.egg-info/dependency_links.txt
 src/opswrapper.egg-info/requires.txt
 src/opswrapper.egg-info/top_level.txt
 test/test_algorithm.py
 test/test_constraints.py
 test/test_element.py
+test/test_integration.py
 test/test_integrator.py
 test/test_material.py
 test/test_model.py
 test/test_recorders.py
 test/test_section.py
 test/test_test.py
 test/test_utils.py
```

### Comparing `opswrapper-5.1.0/test/test_algorithm.py` & `opswrapper-5.2.0/test/test_algorithm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from pytest import raises
 
 from opswrapper import algorithm
 
 
 def test_Linear():
     generated = algorithm.Linear().tcl_code()
-    assert generated == 'algorithm Linear'
+    assert generated == "algorithm Linear"
 
 
 def test_Linear_with_tangent():
-    generated = algorithm.Linear('secant').tcl_code()
-    assert generated == 'algorithm Linear -secant'
+    generated = algorithm.Linear("secant").tcl_code()
+    assert generated == "algorithm Linear -secant"
 
 
 def test_Linear_factor_once():
     generated = algorithm.Linear(factor_once=True).tcl_code()
-    assert generated == 'algorithm Linear -factorOnce'
+    assert generated == "algorithm Linear -factorOnce"
 
 
 def test_Linear_bad_tangent():
     with raises(TypeError):
-        algorithm.Linear('not_a_valid_tangent').tcl_code()
+        algorithm.Linear("not_a_valid_tangent").tcl_code()
 
 
 def test_Newton():
     generated = algorithm.Newton().tcl_code()
-    assert generated == 'algorithm Newton'
+    assert generated == "algorithm Newton"
 
 
 def test_Newton_tangent():
-    generated = algorithm.Newton('hall').tcl_code()
-    assert generated == 'algorithm Newton -hall'
+    generated = algorithm.Newton("hall").tcl_code()
+    assert generated == "algorithm Newton -hall"
 
 
 def test_Newton_weird_tangent():
-    generated = algorithm.Newton('initialThenCurrent').tcl_code()
+    generated = algorithm.Newton("initialThenCurrent").tcl_code()
     # No, this is not a typo.
-    assert generated == 'algorithm Newton -intialThenCurrent'
+    assert generated == "algorithm Newton -intialThenCurrent"
 
 
 def test_KrylovNewton_default():
     generated = algorithm.KrylovNewton().tcl_code()
-    assert generated == 'algorithm KrylovNewton -iterate current -increment current -maxDim 3'
+    assert (
+        generated
+        == "algorithm KrylovNewton -iterate current -increment current -maxDim 3"
+    )
 
 
 def test_Broyden_default():
     generated = algorithm.Broyden().tcl_code()
-    assert generated == 'algorithm Broyden -count 10'
+    assert generated == "algorithm Broyden -count 10"
 
 
 def test_Broyden_tangent():
-    generated = algorithm.Broyden('secant').tcl_code()
-    assert generated == 'algorithm Broyden -secant -count 10'
+    generated = algorithm.Broyden("secant").tcl_code()
+    assert generated == "algorithm Broyden -secant -count 10"
```

### Comparing `opswrapper-5.1.0/test/test_constraints.py` & `opswrapper-5.2.0/test/test_constraints.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from opswrapper import constraints
 
 
 def test_Plain():
     generated = constraints.Plain().tcl_code()
-    assert generated == 'constraints Plain'
+    assert generated == "constraints Plain"
 
 
 def test_Transformation():
     generated = constraints.Transformation().tcl_code()
-    assert generated == 'constraints Transformation'
+    assert generated == "constraints Transformation"
 
 
 def test_Lagrange():
     generated = constraints.Lagrange(1e6, 1e6).tcl_code()
-    assert generated == 'constraints Lagrange 1e+06 1e+06'
+    assert generated == "constraints Lagrange 1000000 1000000"
 
 
 def test_Lagrange_other_format():
-    generated = constraints.Lagrange(1e6, 1e6).tcl_code({float: '.0f'})
-    assert generated == 'constraints Lagrange 1000000 1000000'
+    generated = constraints.Lagrange(1e6, 1e6).tcl_code({float: ".1f"})
+    assert generated == "constraints Lagrange 1000000.0 1000000.0"
 
 
 def test_Penalty():
     generated = constraints.Penalty(1e12, 1e12).tcl_code()
-    assert generated == 'constraints Penalty 1e+12 1e+12'
+    assert generated == "constraints Penalty 1e+12 1e+12"
 
 
 def test_Penalty_other_format():
-    generated = constraints.Penalty(1e12, 1e12).tcl_code({float: '+.1e'})
-    assert generated == 'constraints Penalty +1.0e+12 +1.0e+12'
+    generated = constraints.Penalty(1e12, 1e12).tcl_code({float: "+.1e"})
+    assert generated == "constraints Penalty +1.0e+12 +1.0e+12"
```

### Comparing `opswrapper-5.1.0/test/test_element.py` & `opswrapper-5.2.0/test/test_element.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from opswrapper import element
 from opswrapper import integration
 
 
 def test_ElasticBeamColumn2D():
     generated = element.ElasticBeamColumn2D(1, 0, 1, 10.0, 29000.0, 144.0, 1).tcl_code()
-    expected = 'element elasticBeamColumn 1 0 1 10 29000 144 1'
+    expected = "element elasticBeamColumn 1 0 1 10 29000 144 1"
     assert generated == expected
 
 
 def test_ElasticBeamColumn3D():
-    generated = element.ElasticBeamColumn3D(1, 0, 1, 10.0, 29000.0, 11000.0, 0.402, 14.1, 144.0,
-                                            1).tcl_code()
-    expected = 'element elasticBeamColumn 1 0 1 10 29000 11000 0.402 14.1 144 1'
+    generated = element.ElasticBeamColumn3D(
+        1, 0, 1, 10.0, 29000.0, 11000.0, 0.402, 14.1, 144.0, 1
+    ).tcl_code()
+    expected = "element elasticBeamColumn 1 0 1 10 29000 11000 0.402 14.1 144 1"
     assert generated == expected
 
 
 def test_ForceBeamColumn():
-    generated = element.ForceBeamColumn(2, 0, 1, 1, integration.Lobatto(1, 5)).tcl_code()
+    generated = element.ForceBeamColumn(
+        2, 0, 1, 1, integration.Lobatto(1, 5)
+    ).tcl_code()
     expected = 'element forceBeamColumn 2 0 1 1 "Lobatto 1 5"'
     assert generated == expected
```

### Comparing `opswrapper-5.1.0/test/test_integrator.py` & `opswrapper-5.2.0/test/test_integrator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from opswrapper import integrator
 
 
 def test_LoadControl_default():
     generated = integrator.LoadControl(0.1).tcl_code()
-    assert generated == 'integrator LoadControl 0.1 1 0.1 0.1'
+    assert generated == "integrator LoadControl 0.1 1 0.1 0.1"
 
 
 def test_DisplacementControl_default():
     generated = integrator.DisplacementControl(1, 1, 0.1).tcl_code()
-    assert generated == 'integrator DisplacementControl 1 1 0.1 1 0.1 0.1'
+    assert generated == "integrator DisplacementControl 1 1 0.1 1 0.1 0.1"
 
 
 def test_MinUnbalDispNorm_default():
     generated = integrator.MinUnbalDispNorm(0.1).tcl_code()
-    assert generated == 'integrator MinUnbalDispNorm 0.1 1 0.1 0.1'
+    assert generated == "integrator MinUnbalDispNorm 0.1 1 0.1 0.1"
 
 
 def test_ArcLength():
-    generated = integrator.ArcLength(1.0, 0.1).tcl_code({float: '#g'})
-    assert generated == 'integrator ArcLength 1.00000 0.100000'
+    generated = integrator.ArcLength(1.0, 0.1).tcl_code({float: "#g"})
+    assert generated == "integrator ArcLength 1.00000 0.100000"
 
 
 def test_CentralDifference():
     generated = integrator.CentralDifference().tcl_code()
-    assert generated == 'integrator CentralDifference'
+    assert generated == "integrator CentralDifference"
 
 
 def test_Newmark():
     generated = integrator.Newmark(0.5, 0.25).tcl_code()
-    assert generated == 'integrator Newmark 0.5 0.25'
+    assert generated == "integrator Newmark 0.5 0.25"
 
 
 def test_HHT_default():
     generated = integrator.HHT(0.9).tcl_code()
-    assert generated == 'integrator HHT 0.9'
+    assert generated == "integrator HHT 0.9"
 
 
 def test_HHT_non_default():
     generated = integrator.HHT(0.9, 0.3025).tcl_code()
-    assert generated == 'integrator HHT 0.9 0.3025 0.6'
+    assert generated == "integrator HHT 0.9 0.3025 0.6"
```

### Comparing `opswrapper-5.1.0/test/test_material.py` & `opswrapper-5.2.0/test/test_material.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,92 @@
 from opswrapper import material
 
 
 def test_elastic():
-    assert material.Elastic(1, 29000).tcl_code() == 'uniaxialMaterial Elastic 1 29000'
+    assert material.Elastic(1, 29000).tcl_code() == "uniaxialMaterial Elastic 1 29000"
 
 
 def test_elastic_special_format():
-    assert material.Elastic(1, 29000).tcl_code({float: '.2e'}) == 'uniaxialMaterial Elastic 1 2.90e+04'
+    assert (
+        material.Elastic(1, 29000).tcl_code({float: ".2e"})
+        == "uniaxialMaterial Elastic 1 2.90e+04"
+    )
 
 
 def test_elastic_Eneg_but_no_eta():
     generated_code = material.Elastic(1, 29000, Eneg=10000).tcl_code()
-    expected_code = 'uniaxialMaterial Elastic 1 29000 0 10000'
+    expected_code = "uniaxialMaterial Elastic 1 29000 0 10000"
     assert generated_code == expected_code
 
 
 def test_elastic_Eneg_and_eta():
     generated_code = material.Elastic(1, 29000, 12.0, 10000).tcl_code()
-    expected_code = 'uniaxialMaterial Elastic 1 29000 12 10000'
+    expected_code = "uniaxialMaterial Elastic 1 29000 12 10000"
     assert generated_code == expected_code
 
 
 def test_elastic_pp():
     generated_code = material.ElasticPP(1, 29000, 0.00207).tcl_code()
-    expected_code = 'uniaxialMaterial ElasticPP 1 29000 0.00207'
+    expected_code = "uniaxialMaterial ElasticPP 1 29000 0.00207"
     assert generated_code == expected_code
 
 
 def test_elastic_pp_eps0_but_no_eps_yN():
     generated_code = material.ElasticPP(1, 29000, 0.00207, eps0=0.001).tcl_code()
-    expected_code = 'uniaxialMaterial ElasticPP 1 29000 0.00207 0.00207 0.001'
+    expected_code = "uniaxialMaterial ElasticPP 1 29000 0.00207 0.00207 0.001"
     assert generated_code == expected_code
 
 
 def test_Steel01():
     generated_code = material.Steel01(1, 50, 29000, 0.003).tcl_code()
-    expected_code = 'uniaxialMaterial Steel01 1 50 29000 0.003'
+    expected_code = "uniaxialMaterial Steel01 1 50 29000 0.003"
     assert generated_code == expected_code
 
 
 def test_Steel01_special_format():
-    generated_code = material.Steel01(1, 50, 29000, 0.003).tcl_code({float: '.2e'})
-    expected_code = 'uniaxialMaterial Steel01 1 5.00e+01 2.90e+04 3.00e-03'
+    generated_code = material.Steel01(1, 50, 29000, 0.003).tcl_code({float: ".2e"})
+    expected_code = "uniaxialMaterial Steel01 1 5.00e+01 2.90e+04 3.00e-03"
     assert generated_code == expected_code
 
 
 def test_Steel01_iso_hardening():
-    generated_code = material.Steel01(1, 50, 29000, 0.003, 0.01, 0.02, 0.03, 0.04).tcl_code()
-    expected_code = 'uniaxialMaterial Steel01 1 50 29000 0.003 0.01 0.02 0.03 0.04'
+    generated_code = material.Steel01(
+        1, 50, 29000, 0.003, 0.01, 0.02, 0.03, 0.04
+    ).tcl_code()
+    expected_code = "uniaxialMaterial Steel01 1 50 29000 0.003 0.01 0.02 0.03 0.04"
     assert generated_code == expected_code
 
 
 def test_Steel02():
     generated_code = material.Steel02(1, 50, 29000, 0.003).tcl_code()
-    expected_code = 'uniaxialMaterial Steel02 1 50 29000 0.003 20 0.925 0.15'
+    expected_code = "uniaxialMaterial Steel02 1 50 29000 0.003 20 0.925 0.15"
     assert generated_code == expected_code
 
 
 def test_Steel02_special_format():
-    generated_code = material.Steel02(1, 50, 29000, 0.003).tcl_code({int: '4d'})
-    expected_code = 'uniaxialMaterial Steel02    1 50 29000 0.003 20 0.925 0.15'
+    generated_code = material.Steel02(1, 50, 29000, 0.003).tcl_code({int: "4d"})
+    expected_code = "uniaxialMaterial Steel02    1 50 29000 0.003 20 0.925 0.15"
     assert generated_code == expected_code
 
 
 def test_Steel02_non_default_R():
-    generated_code = material.Steel02(1, 50, 29000, 0.003, R0=15, cR1=0.9, cR2=0.20).tcl_code()
-    expected_code = 'uniaxialMaterial Steel02 1 50 29000 0.003 15 0.9 0.2'
+    generated_code = material.Steel02(
+        1, 50, 29000, 0.003, R0=15, cR1=0.9, cR2=0.20
+    ).tcl_code()
+    expected_code = "uniaxialMaterial Steel02 1 50 29000 0.003 15 0.9 0.2"
     assert generated_code == expected_code
 
 
 def test_Steel02_iso_hardening():
-    generated_code = material.Steel02(1, 50, 29000, 0.003, a1=0.5, a2=1.0, a3=0.5, a4=1.0).tcl_code()
-    expected_code = 'uniaxialMaterial Steel02 1 50 29000 0.003 20 0.925 0.15 0.5 1 0.5 1'
+    generated_code = material.Steel02(
+        1, 50, 29000, 0.003, a1=0.5, a2=1.0, a3=0.5, a4=1.0
+    ).tcl_code()
+    expected_code = (
+        "uniaxialMaterial Steel02 1 50 29000 0.003 20 0.925 0.15 0.5 1 0.5 1"
+    )
     assert generated_code == expected_code
 
 
 def test_Steel02_initial_stress():
     generated_code = material.Steel02(1, 50, 29000, 0.003, sigma_i=15).tcl_code()
-    expected_code = 'uniaxialMaterial Steel02 1 50 29000 0.003 20 0.925 0.15 0 1 0 1 15'
+    expected_code = "uniaxialMaterial Steel02 1 50 29000 0.003 20 0.925 0.15 0 1 0 1 15"
     assert generated_code == expected_code
```

### Comparing `opswrapper-5.1.0/test/test_model.py` & `opswrapper-5.2.0/test/test_model.py`

 * *Files identical despite different names*

### Comparing `opswrapper-5.1.0/test/test_recorders.py` & `opswrapper-5.2.0/test/test_recorders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,181 +1,185 @@
 import numpy as np
 
 from opswrapper.output import NodeRecorder, ElementRecorder
 
 
 def test_node_recorder():
     recorder = NodeRecorder(
-        file='/path/to/file',
+        file="/path/to/file",
         nodes=1,
         dofs=[1, 2],
-        response='disp',
+        response="disp",
     )
     generated = recorder.tcl_code()
-    expected = 'recorder Node -file {/path/to/file} -node 1 -dof 1 2 disp'
+    expected = "recorder Node -file {/path/to/file} -node 1 -dof 1 2 disp"
     assert generated == expected
 
 
 def test_node_recorder_pass_array():
     recorder = NodeRecorder(
-        file=R'C:\Scratch\displacement.dat',
+        file=R"C:\Scratch\displacement.dat",
         nodes=np.array([1, 2, 3, 4, 5]),
         dofs=np.array([1, 2, 3, 4, 5, 6]),
-        response='disp',
+        response="disp",
     )
     generated = recorder.tcl_code()
     expected = (
-        'recorder Node -file {C:/Scratch/displacement.dat} '
-        '-node 1 2 3 4 5 -dof 1 2 3 4 5 6 disp'
+        "recorder Node -file {C:/Scratch/displacement.dat} "
+        "-node 1 2 3 4 5 -dof 1 2 3 4 5 6 disp"
     )
     assert generated == expected
 
 
 def test_node_recorder_windows_path():
     recorder = NodeRecorder(
-        file=R'C:\Scratch\displacement.dat',
+        file=R"C:\Scratch\displacement.dat",
         nodes=[1, 2, 3, 4, 5],
         dofs=[1, 2, 3, 4, 5, 6],
-        response='disp',
+        response="disp",
     )
     generated = recorder.tcl_code()
     expected = (
-        'recorder Node -file {C:/Scratch/displacement.dat} '
-        '-node 1 2 3 4 5 -dof 1 2 3 4 5 6 disp'
+        "recorder Node -file {C:/Scratch/displacement.dat} "
+        "-node 1 2 3 4 5 -dof 1 2 3 4 5 6 disp"
     )
     assert generated == expected
 
 
 def test_node_recorder_delayed_file():
-    recorder = NodeRecorder(nodes=1, dofs=1, response='accel')
+    recorder = NodeRecorder(nodes=1, dofs=1, response="accel")
     generated = recorder.tcl_code()
-    expected = 'recorder Node -file {{{file}}} -node 1 -dof 1 accel'
+    expected = "recorder Node -file {{{file}}} -node 1 -dof 1 accel"
     assert generated == expected
 
 
 def test_node_recorder_delayed_file_then_format():
-    recorder = NodeRecorder(nodes=1, dofs=1, response='accel')
-    generated = recorder.tcl_code().format(file='/path/to/file')
-    expected = 'recorder Node -file {/path/to/file} -node 1 -dof 1 accel'
+    recorder = NodeRecorder(nodes=1, dofs=1, response="accel")
+    generated = recorder.tcl_code().format(file="/path/to/file")
+    expected = "recorder Node -file {/path/to/file} -node 1 -dof 1 accel"
     assert generated == expected
 
 
 def test_node_recorder_region():
-    recorder = NodeRecorder(file='/path/to/file', region=1, response='vel')
+    recorder = NodeRecorder(file="/path/to/file", region=1, response="vel")
     generated = recorder.tcl_code()
-    expected = 'recorder Node -file {/path/to/file} -region 1 vel'
+    expected = "recorder Node -file {/path/to/file} -region 1 vel"
     assert generated == expected
 
 
 def test_node_recorder_all_nodes():
     recorder = NodeRecorder(
-        file='/path/to/file',
-        nodes='all',
+        file="/path/to/file",
+        nodes="all",
         dofs=[1, 2, 3],
-        response='vel',
+        response="vel",
     )
     generated = recorder.tcl_code()
-    expected = 'recorder Node -file {/path/to/file} -node {*}[getNodeTags] -dof 1 2 3 vel'
+    expected = (
+        "recorder Node -file {/path/to/file} -node {*}[getNodeTags] -dof 1 2 3 vel"
+    )
     assert generated == expected
 
 
 def test_node_recorder_all_nodes_delayed_file():
-    recorder = NodeRecorder(nodes='all', dofs=1, response='accel')
+    recorder = NodeRecorder(nodes="all", dofs=1, response="accel")
     generated = recorder.tcl_code()
-    expected = 'recorder Node -file {{{file}}} -node {{*}}[getNodeTags] -dof 1 accel'
+    expected = "recorder Node -file {{{file}}} -node {{*}}[getNodeTags] -dof 1 accel"
     assert generated == expected
 
 
 def test_node_recorder_all_nodes_delayed_file_then_format():
-    recorder = NodeRecorder(nodes='all', dofs=1, response='accel')
-    generated = recorder.tcl_code().format(file='/path/to/file')
-    expected = 'recorder Node -file {/path/to/file} -node {*}[getNodeTags] -dof 1 accel'
+    recorder = NodeRecorder(nodes="all", dofs=1, response="accel")
+    generated = recorder.tcl_code().format(file="/path/to/file")
+    expected = "recorder Node -file {/path/to/file} -node {*}[getNodeTags] -dof 1 accel"
     assert generated == expected
 
 
 def test_element_recorder():
     recorder = ElementRecorder(
-        file='/path/to/file',
+        file="/path/to/file",
         elements=1,
         dofs=[1, 2],
-        response='localForce',
+        response="localForce",
     )
     generated = recorder.tcl_code()
-    expected = 'recorder Element -file {/path/to/file} -ele 1 -dof 1 2 localForce'
+    expected = "recorder Element -file {/path/to/file} -ele 1 -dof 1 2 localForce"
     assert generated == expected
 
 
 def test_element_recorder_pass_array():
     recorder = ElementRecorder(
-        file=R'C:\Scratch\forces.dat',
+        file=R"C:\Scratch\forces.dat",
         elements=np.array([1, 2, 3, 4, 5]),
         dofs=np.array([1, 2, 3, 4, 5, 6]),
-        response='force',
+        response="force",
     )
     generated = recorder.tcl_code()
     expected = (
-        'recorder Element -file {C:/Scratch/forces.dat} '
-        '-ele 1 2 3 4 5 -dof 1 2 3 4 5 6 force'
+        "recorder Element -file {C:/Scratch/forces.dat} "
+        "-ele 1 2 3 4 5 -dof 1 2 3 4 5 6 force"
     )
     assert generated == expected
 
 
 def test_element_recorder_windows_path():
     recorder = ElementRecorder(
-        file=R'C:\Scratch\forces.dat',
+        file=R"C:\Scratch\forces.dat",
         elements=[1, 2, 3, 4, 5],
         dofs=[1, 2, 3, 4, 5, 6],
-        response='force',
+        response="force",
     )
     generated = recorder.tcl_code()
     expected = (
-        'recorder Element -file {C:/Scratch/forces.dat} '
-        '-ele 1 2 3 4 5 -dof 1 2 3 4 5 6 force'
+        "recorder Element -file {C:/Scratch/forces.dat} "
+        "-ele 1 2 3 4 5 -dof 1 2 3 4 5 6 force"
     )
     assert generated == expected
 
 
 def test_element_recorder_delayed_file():
-    recorder = ElementRecorder(elements=1, dofs=1, response='force')
+    recorder = ElementRecorder(elements=1, dofs=1, response="force")
     generated = recorder.tcl_code()
-    expected = 'recorder Element -file {{{file}}} -ele 1 -dof 1 force'
+    expected = "recorder Element -file {{{file}}} -ele 1 -dof 1 force"
     assert generated == expected
 
 
 def test_element_recorder_delayed_file_then_format():
-    recorder = ElementRecorder(elements=1, dofs=1, response='force')
-    generated = recorder.tcl_code().format(file='/path/to/file')
-    expected = 'recorder Element -file {/path/to/file} -ele 1 -dof 1 force'
+    recorder = ElementRecorder(elements=1, dofs=1, response="force")
+    generated = recorder.tcl_code().format(file="/path/to/file")
+    expected = "recorder Element -file {/path/to/file} -ele 1 -dof 1 force"
     assert generated == expected
 
 
 def test_element_recorder_region():
-    recorder = ElementRecorder(file='/path/to/file', region=1, response='axialForce')
+    recorder = ElementRecorder(file="/path/to/file", region=1, response="axialForce")
     generated = recorder.tcl_code()
-    expected = 'recorder Element -file {/path/to/file} -region 1 axialForce'
+    expected = "recorder Element -file {/path/to/file} -region 1 axialForce"
     assert generated == expected
 
 
 def test_element_recorder_all_elements():
     recorder = ElementRecorder(
-        file='/path/to/file',
-        elements='all',
+        file="/path/to/file",
+        elements="all",
         dofs=[1, 2, 3],
-        response='globalForce',
+        response="globalForce",
     )
     generated = recorder.tcl_code()
-    expected = 'recorder Element -file {/path/to/file} -ele {*}[getEleTags] -dof 1 2 3 globalForce'
+    expected = "recorder Element -file {/path/to/file} -ele {*}[getEleTags] -dof 1 2 3 globalForce"
     assert generated == expected
 
 
 def test_element_recorder_all_elements_delayed_file():
-    recorder = ElementRecorder(elements='all', dofs=1, response='force')
+    recorder = ElementRecorder(elements="all", dofs=1, response="force")
     generated = recorder.tcl_code()
-    expected = 'recorder Element -file {{{file}}} -ele {{*}}[getEleTags] -dof 1 force'
+    expected = "recorder Element -file {{{file}}} -ele {{*}}[getEleTags] -dof 1 force"
     assert generated == expected
 
 
 def test_element_recorder_all_elements_delayed_file_then_format():
-    recorder = ElementRecorder(elements='all', dofs=1, response='force')
-    generated = recorder.tcl_code().format(file='/path/to/file')
-    expected = 'recorder Element -file {/path/to/file} -ele {*}[getEleTags] -dof 1 force'
+    recorder = ElementRecorder(elements="all", dofs=1, response="force")
+    generated = recorder.tcl_code().format(file="/path/to/file")
+    expected = (
+        "recorder Element -file {/path/to/file} -ele {*}[getEleTags] -dof 1 force"
+    )
     assert generated == expected
```

### Comparing `opswrapper-5.1.0/test/test_section.py` & `opswrapper-5.2.0/test/test_section.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from opswrapper import section
 
 
 def test_Elastic2D():
     generated = section.Elastic2D(1, 29000, 10, 144).tcl_code()
-    expected = 'section Elastic 1 29000 10 144'
+    expected = "section Elastic 1 29000 10 144"
     assert generated == expected
 
 
 def test_Elastic2D_special_format():
-    generated = section.Elastic2D(1, 29000, 10, 144).tcl_code({float: '#.3g'})
-    expected = 'section Elastic 1 2.90e+04 10.0 144.'
+    generated = section.Elastic2D(1, 29000, 10, 144).tcl_code({float: "#.3g"})
+    expected = "section Elastic 1 2.90e+04 10.0 144."
     assert generated == expected
 
 
 def test_Elastic2D_shear():
     generated = section.Elastic2D(1, 29000, 10, 144, 11000, 1.0).tcl_code()
-    expected = 'section Elastic 1 29000 10 144 11000 1'
+    expected = "section Elastic 1 29000 10 144 11000 1"
     assert generated == expected
 
 
 def test_Elastic3D():
     generated = section.Elastic3D(1, 29000, 10, 144, 14.1, 11000, 0.402).tcl_code()
-    expected = 'section Elastic 1 29000 10 144 14.1 11000 0.402'
+    expected = "section Elastic 1 29000 10 144 14.1 11000 0.402"
     assert generated == expected
 
 
 def test_Elastic3D_shear():
-    generated = section.Elastic3D(1, 29000, 10, 144, 14.1, 11000, 0.402, 1.0, 1.0).tcl_code()
-    expected = 'section Elastic 1 29000 10 144 14.1 11000 0.402 1 1'
+    generated = section.Elastic3D(
+        1, 29000, 10, 144, 14.1, 11000, 0.402, 1.0, 1.0
+    ).tcl_code()
+    expected = "section Elastic 1 29000 10 144 14.1 11000 0.402 1 1"
     assert generated == expected
 
 
 def test_Fiber_section():
     generated = section.Fiber(1).fiber(0, -1, 1.0, 2).fiber(0, 1, 1.0, 2).tcl_code()
-    expected = 'section Fiber 1 {\n    fiber 0 -1 1 2\n    fiber 0 1 1 2\n}'
+    expected = "section Fiber 1 {\n    fiber 0 -1 1 2\n    fiber 0 1 1 2\n}"
     assert generated == expected
```

### Comparing `opswrapper-5.1.0/test/test_test.py` & `opswrapper-5.2.0/test/test_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from pytest import raises
 
 from opswrapper import test
 
 
 def test_standard():
     generated = test.NormUnbalance(1e-8, 50).tcl_code()
-    expected = 'test NormUnbalance 1e-08 50 0 2'
+    expected = "test NormUnbalance 1e-08 50 0 2"
     assert generated == expected
 
 
 def test_with_flags():
     generated = test.NormUnbalance(1e-8, 50, 2, 2).tcl_code()
-    expected = 'test NormUnbalance 1e-08 50 2 2'
+    expected = "test NormUnbalance 1e-08 50 2 2"
     assert generated == expected
 
 
 def test_with_str_field():
-    generated = test.NormDispIncr('$tol', 50, 2, 2).tcl_code()
-    expected = 'test NormDispIncr $tol 50 2 2'
+    generated = test.NormDispIncr("$tol", 50, 2, 2).tcl_code()
+    expected = "test NormDispIncr $tol 50 2 2"
     assert generated == expected
 
 
 def test_alternate_format():
-    generated = test.NormUnbalance(1e-8, 50, 2, 2).tcl_code({float: '.2e'})
-    expected = 'test NormUnbalance 1.00e-08 50 2 2'
+    generated = test.NormUnbalance(1e-8, 50, 2, 2).tcl_code({float: ".2e"})
+    expected = "test NormUnbalance 1.00e-08 50 2 2"
     assert generated == expected
 
 
 def test_bad_print_flag():
     the_test = test.EnergyIncr(1e-4, 50, 8)
     with raises(ValueError):
         the_test.tcl_code()
```

