# Comparing `tmp/cavcalc-1.1.0.tar.gz` & `tmp/cavcalc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cavcalc-1.1.0.tar", max compression
+gzip compressed data, was "cavcalc-1.2.0.tar", max compression
```

## Comparing `cavcalc-1.1.0.tar` & `cavcalc-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0    35129 2023-04-12 16:38:17.667410 cavcalc-1.1.0/LICENSE
--rw-r--r--   0        0        0    12397 2023-04-12 16:38:17.667410 cavcalc-1.1.0/README.md
--rw-r--r--   0        0        0     1782 2023-04-12 16:38:17.676410 cavcalc-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3921 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/__init__.py
--rw-r--r--   0        0        0      409 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/__main__.py
--rw-r--r--   0        0        0      168 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/__version__.py
--rw-r--r--   0        0        0        0 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/__init__.py
--rw-r--r--   0        0        0     9474 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/_container.py
--rw-r--r--   0        0        0     5348 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/_groups.py
--rw-r--r--   0        0        0     3960 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/_types.py
--rw-r--r--   0        0        0      748 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_default.mplstyle
--rw-r--r--   0        0        0      403 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_exiters.py
--rw-r--r--   0        0        0    10537 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_handler.py
--rw-r--r--   0        0        0     3230 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_main.py
--rw-r--r--   0        0        0     1462 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_session.py
--rw-r--r--   0        0        0     9254 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/calculate.py
--rw-r--r--   0        0        0     1536 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/cavcalc.ini
--rw-r--r--   0        0        0     3856 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/env.py
--rw-r--r--   0        0        0      256 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/errors.py
--rw-r--r--   0        0        0      709 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/__init__.py
--rw-r--r--   0        0        0     5193 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/_maps.py
--rw-r--r--   0        0        0     1105 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/_utils.py
--rw-r--r--   0        0        0     7331 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/asymmetric.py
--rw-r--r--   0        0        0     3541 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/resonance.py
--rw-r--r--   0        0        0     6007 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/symmetric.py
--rw-r--r--   0        0        0    22169 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/output.py
--rw-r--r--   0        0        0      443 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/__init__.py
--rw-r--r--   0        0        0     5330 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/_maps.py
--rw-r--r--   0        0        0     1126 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/enums.py
--rw-r--r--   0        0        0     6339 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/parameter.py
--rw-r--r--   0        0        0     3839 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/tools.py
--rw-r--r--   0        0        0       78 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/testing.py
--rw-r--r--   0        0        0    13686 1970-01-01 00:00:00.000000 cavcalc-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-05-08 13:58:05.906346 cavcalc-1.2.0/LICENSE
+-rw-r--r--   0        0        0    12700 2023-05-08 13:58:05.906346 cavcalc-1.2.0/README.md
+-rw-r--r--   0        0        0     1782 2023-05-08 13:58:05.915346 cavcalc-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3921 2023-05-08 13:58:05.916347 cavcalc-1.2.0/src/cavcalc/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-08 13:58:05.916347 cavcalc-1.2.0/src/cavcalc/__main__.py
+-rw-r--r--   0        0        0      168 2023-05-08 13:58:05.916347 cavcalc-1.2.0/src/cavcalc/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:58:05.916347 cavcalc-1.2.0/src/cavcalc/_arguments/__init__.py
+-rw-r--r--   0        0        0    10566 2023-05-08 13:58:05.916347 cavcalc-1.2.0/src/cavcalc/_arguments/_container.py
+-rw-r--r--   0        0        0     5348 2023-05-08 13:58:05.916347 cavcalc-1.2.0/src/cavcalc/_arguments/_groups.py
+-rw-r--r--   0        0        0     4476 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_arguments/_types.py
+-rw-r--r--   0        0        0      105 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_arguments/_utils.py
+-rw-r--r--   0        0        0      748 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_default.mplstyle
+-rw-r--r--   0        0        0      403 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_exiters.py
+-rw-r--r--   0        0        0    11237 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_handler.py
+-rw-r--r--   0        0        0     3230 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_main.py
+-rw-r--r--   0        0        0     1462 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/_session.py
+-rw-r--r--   0        0        0    10537 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/calculate.py
+-rw-r--r--   0        0        0     1536 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/cavcalc.ini
+-rw-r--r--   0        0        0     4190 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/env.py
+-rw-r--r--   0        0        0      256 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/errors.py
+-rw-r--r--   0        0        0      709 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/functions/__init__.py
+-rw-r--r--   0        0        0     5629 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/functions/_maps.py
+-rw-r--r--   0        0        0     1105 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/functions/_utils.py
+-rw-r--r--   0        0        0     7331 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/functions/asymmetric.py
+-rw-r--r--   0        0        0     4717 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/functions/resonance.py
+-rw-r--r--   0        0        0     6007 2023-05-08 13:58:05.917347 cavcalc-1.2.0/src/cavcalc/functions/symmetric.py
+-rw-r--r--   0        0        0    22211 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/output.py
+-rw-r--r--   0        0        0      454 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/parameters/__init__.py
+-rw-r--r--   0        0        0     6129 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/parameters/_maps.py
+-rw-r--r--   0        0        0     1235 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/parameters/enums.py
+-rw-r--r--   0        0        0     5837 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/parameters/parameter.py
+-rw-r--r--   0        0        0     4893 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/parameters/tools.py
+-rw-r--r--   0        0        0       78 2023-05-08 13:58:05.918347 cavcalc-1.2.0/src/cavcalc/testing.py
+-rw-r--r--   0        0        0    13989 1970-01-01 00:00:00.000000 cavcalc-1.2.0/PKG-INFO
```

### Comparing `cavcalc-1.1.0/LICENSE` & `cavcalc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/README.md` & `cavcalc-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```bash
 cavcalc --version
 ```
 
 if you see something along the lines of
 
 ```
-cavcalc v1.1.0
+cavcalc v1.2.0
 ```
 
 then you should be ready to start using `cavcalc`!
 
 **Note**: As is often recommended with the installation of Python packages (especially those with dependencies
 on packages such as `numpy` and `matplotlib`, as is the case here), you should prefer to install `cavcalc` in
 a suitable virtual environment. See [the official documentation on Python virtual environments](https://docs.python.org/3/tutorial/venv.html)
@@ -87,15 +87,15 @@
 
 ### Computing all available parameters
 
 A compute target of `all` is the default choice which is used to calculate all parameters which can be determined
 from the arguments specified. For example, using approximate values of the Advanced LIGO arm cavity parameters,
 
 ```bash
-cavcalc -L 4km -Rc1 1934 -Rc2 2245 -T1 0.014 -L1 37.5e-6 -T2 5e-6 -L2 37.5e-6
+cavcalc -L 4km -Rc1 1934 -Rc2 2245 -T1 0.014 -L1 37.5e-6 -T2 5e-6 -L2 L1
 ```
 
 gives the following output:
 
 ```
 Given:
 	Loss of first mirror = 3.75e-05
@@ -115,14 +115,17 @@
 	FWHM = 84.56921734107604 Hz
 	Mode separation frequency = 4988.072188176178 Hz
 	Pole frequency = 42.28460867053802 Hz
 
 	Finesse = 443.11699254426594
 	Reflectivity of first mirror = 0.9859625
 	Reflectivity of second mirror = 0.9999574999999999
+	Internal resonance enhancement factor = 20036.317877295227
+	External resonance enhancement factor = 281.2598122025325
+	Fractional transmission intensity = 0.011953542018623487
 
 	Position of beam waist (from first mirror) = 1837.2153886417168 m
 
 	Radius of beam at first mirror = 53.421066433049255 mm
 	Radius of beam at second mirror = 62.448079883230896 mm
 	Radius of beam at waist = 11.950538458990879 mm
 
@@ -208,19 +211,22 @@
 
 ![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_w_vs_L_gouy.png)
 
 A matplotlib compliant colour-map can be specified when making an image plot using the `--cmap <name>` option. For example,
 the following command gives the plot shown below.
 
 ```bash
-cavcalc gouy -L 12um -g1 "-2 2 499" -g2 "-2 2 499" --mesh true --plot --cmap Spectral_r
+cavcalc gouy -g1 "-2 2 499" -g2 g1 --mesh true --plot --cmap Spectral_r
 ```
 
 ![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/asymmcav_w0_vs_g1g2.png)
 
+**Note** that here we also used the parameter-referencing feature of `cavcalc`, introduced in v1.2.0, to set
+the values of `g1` to those of `g2`.
+
 ## A note on g-factors
 
 Stability (g) factors are split into four different parameters for implementation purposes and to
 hopefully make it clearer as to which argument is being used and whether the resulting cavity
 computations are for a symmetric or asymmetric cavity. These arguments are detailed here:
 
 - `-gs` : The symmetric, singular stability factor. This represents the individual g-factors of **both**
```

### Comparing `cavcalc-1.1.0/pyproject.toml` & `cavcalc-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cavcalc"
-version = "1.1.0"
+version = "1.2.0"
 description = "A program for computing Fabry-Perot optical cavity parameters."
 authors = ["Samuel Rowlinson <samueljrowlinson@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://cavcalc.readthedocs.io/en/latest/"
 repository = "https://gitlab.com/sjrowlinson/cavcalc"
 documentation = "https://cavcalc.readthedocs.io/en/latest/"
```

### Comparing `cavcalc-1.1.0/src/cavcalc/__init__.py` & `cavcalc-1.2.0/src/cavcalc/__init__.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/_arguments/_container.py` & `cavcalc-1.2.0/src/cavcalc/_arguments/_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import numpy as np
 from typing import Any, Union
 import warnings
 
+from ._utils import _ReferencedQuantity
 from .. import Q_
-from .._exiters import quit_print
+from .._exiters import bug, quit_print
 from ..parameters import ArgParameter, ParameterType
 
 
-# TODO (sjr) Should probably add a decorator to enable freezing of instances of
-#            this, and set it to frozen in _CavCalcSession.parse_args after
-#            parsing the arguments into it.
 class _Arguments:
     def __init__(self):
         self.__physical_args = {}
 
     @property
     def physical_args(self) -> dict[ParameterType, ArgParameter]:
         return self.__physical_args
@@ -31,14 +29,37 @@
 
     def has(self, argname: str) -> bool:
         """Checks that `argname` was specified as one of the arguments, and so
         is held by this namespace-like object."""
         return getattr(self, argname, None) is not None
 
     def process(self, arg_orders: dict[str, int]):
+        # Resolve cross-referenced arguments
+        for name, v in vars(self).copy().items():
+            if isinstance(v, _ReferencedQuantity):
+                if name == v.ref_name:
+                    quit_print(f"Argument '{name}' references itself!")
+
+                q = getattr(self, v.ref_name)
+                ref_chain = set([name, v.ref_name])
+                while isinstance(q, _ReferencedQuantity):
+                    if q.ref_name in ref_chain:
+                        quit_print(
+                            "Encountered a reference loop whilst trying to "
+                            f"resolve the parameter '{name}'."
+                        )
+                    q = getattr(self, q.ref_name)
+
+                if q is None:
+                    quit_print(f"Argument '{name}' references a parameter which was not given.")
+                elif not isinstance(q, Q_):
+                    bug(f"Argument '{name}' references a parameter which is not a quantity.")
+
+                setattr(self, name, q)
+
         filter_phys_args = lambda: {name: v for name, v in vars(self).items() if isinstance(v, Q_)}
         phys_args = filter_phys_args()
 
         # Construct mesh-grids from these parameters in the order specified
         axis_orders = {}
         if self.mesh:
             if isinstance(self.mesh, bool):
@@ -102,15 +123,15 @@
                 self.__physical_args[Lm.ptype] = Lm
 
     def verify(self):
         """Checks that the arguments held by this namespace-like object make sense
         and are consistent with one another."""
         if self.has("units"):
             if self.is_all_target:
-                quit_print(
+                warnings.warn(
                     "Specifying output units is only supported in single target mode. Use "
                     "a 'cavcalc.ini' config file to override units in multi target mode, or "
                     "interact with cavcalc via the Python API for tasks requiring more "
                     "customisation."
                 )
 
         if self.has("loadfile") and self.physical_args:
@@ -189,14 +210,20 @@
                 msg = (
                     "Incorrect usage! Cavity g-factor and symmetric mirror g-factors "
                     "cannot be specified simultaneously."
                 )
 
             quit_print(msg + "\n\n" + instruct)
 
+        if has_gs and (has_g1 or has_g2):
+            quit_print(
+                "Incorrect usage! Individual mirror g-factors and symmetric "
+                "mirror g-factor cannot be specified simultaneously."
+            )
+
         # ... and same goes for combinations of RoCs...
         if self.has("Rc") and (self.has("Rc1") or self.has("Rc2")):
             quit_print(
                 "Incorrect usage! Symmetric curvature, 'Rc', and individual (non-symmetric), 'Rc1' and 'Rc2', "
                 "curvatures cannot be specified simultaneously.\n\nTo specify a non-symmetric cavity "
                 "please use both 'Rc1' and 'Rc2', do not give a value for 'Rc'. To specify a symmetric "
                 "cavity please use just 'Rc'."
@@ -206,11 +233,11 @@
         if self.has("w") and (self.has("w1") or self.has("w2")):
             quit_print(
                 "Incorrect usage! Symmetric beam-size, 'w', and individual (non-symmetric), 'w1' and 'w2', "
                 "beam-sizes cannot be specified simultaneously.\n\nTo specify a non-symmetric cavity "
                 "please use both 'w1' and 'w2', do not give a value for 'w'. To specify a symmetric "
                 "cavity please use just 'w'."
             )
-        for p in "w", "w1", "w2", "w0":
+        for p in "w", "w1", "w2":
             if P := self[p]:
                 if np.any(P.value.m < 0):
                     quit_print(f"{p} is invalid. Beam sizes must be non-negative.")
```

### Comparing `cavcalc-1.1.0/src/cavcalc/_arguments/_groups.py` & `cavcalc-1.2.0/src/cavcalc/_arguments/_groups.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/_arguments/_types.py` & `cavcalc-1.2.0/src/cavcalc/_arguments/_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Functions to convert strings, passed as CLI arguments, to
 appropriate quantities for these argument types."""
 
 import numpy as np
 import os
 from pint.errors import UndefinedUnitError
 
+from ._utils import _ReferencedQuantity
 from .. import Q_
 from .._exiters import quit_print
+from ..parameters import valid_arguments
 
 
 def _parse_data_range(*args):
     nargs = len(args)
     if nargs < 3 or nargs > 4:
         quit_print(
             f'Expected data range in format "<start> <stop> <num> [<units>]" ' f"but got: {args}"
@@ -18,14 +20,21 @@
 
     if nargs == 3:
         start, stop, num = args
         units = ""
     else:
         start, stop, num, units = args
 
+    for x in start, stop, num:
+        xc = x.casefold()
+        if "inf" in xc:
+            quit_print("Encountered 'inf' in a data range. Values must be real and finite.")
+        if "nan" in xc:
+            quit_print("Encountered 'NaN' in a data range. Values must be real and finite.")
+
     try:
         start = float(start)
     except ValueError:
         quit_print(
             f"Could not convert data range start value '{start}' to a floating point number."
         )
 
@@ -62,14 +71,18 @@
             else:  # load from text/csv file
                 data = np.loadtxt(string)
         except:
             quit_print(f"Unable to parse file {string}")
 
         return Q_(data)
 
+    # ... then check if it's a reference to another parameter...
+    if string in valid_arguments:
+        return _ReferencedQuantity(string)
+
     # ... then try parsing as a range...
     args = string.split()
     if len(args) > 1:
         return _parse_data_range(*args)
 
     # ... if that fails then just attempt to convert
     # the argument to a floating point number
```

### Comparing `cavcalc-1.1.0/src/cavcalc/_default.mplstyle` & `cavcalc-1.2.0/src/cavcalc/_default.mplstyle`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/_handler.py` & `cavcalc-1.2.0/src/cavcalc/_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pint.errors import DimensionalityError, UndefinedUnitError
 
 from . import _CONFIG, Q_
 from ._arguments._container import _Arguments
+from .errors import CavCalcError
 from ._exiters import quit_print, bug
 from .functions._maps import (
     RESONANCE_TARGETS_FUNC_MAP as _RES_TARGETS_MAP,
     SYMMETRIC_TARGETS_FUNC_MAP as _SYMM_TARGETS_MAP,
     ASYMMETRIC_TARGETS_FUNC_MAP as _ASYMM_TARGETS_MAP,
 )
 from .output import SingleOutput, MultiOutput
@@ -115,14 +116,17 @@
                     chained_reqd, _ = self.func_dep_map[chained_func]
                     chained_func_args = tuple(
                         self.args.physical_args.get(p) or self.chained.get(p) for p in chained_reqd
                     )
                     # ... storing them as chained ArgParameter instances, for
                     # easy use when calculating self.target_function later on
                     self.chained[pd] = ArgParameter(pd, compute(chained_func, *chained_func_args))
+
+                    for arg in chained_func_args:
+                        arg._used = True
             else:
                 msg = f"Incorrect usage. To compute {self.args.compute} I require one of: "
                 all_maps = _RES_TARGETS_MAP | _SYMM_TARGETS_MAP | _ASYMM_TARGETS_MAP
                 for reqd_params, ret_param in all_maps.values():
                     if ret_param == self.target_parameter.ptype:
                         msg += "\n\t"
                         msg += " AND ".join(
@@ -141,20 +145,28 @@
     def run(self):
         reqd_params, _ = self.func_dep_map[self.target_function]
         func_args = tuple(
             self.args.physical_args.get(p) or self.chained.get(p) for p in reqd_params
         )
 
         result = compute(self.target_function, *func_args)
+        units = self.args["units"] or _CONFIG["units"].get(self.target_parameter.name)
         if not self.target_parameter.is_unitless:
-            units = self.args["units"] or _CONFIG["units"].get(self.target_parameter.name)
             try:
                 result = result.to(units)
             except (DimensionalityError, UndefinedUnitError, ValueError) as ex:
                 quit_print(str(ex))
+        else:
+            if units:
+                quit_print(
+                    f"Units '{units}' given for dimensionless target '{self.target_parameter.name}'"
+                )
+
+        for arg in func_args:
+            arg._used = True
 
         self.target_parameter = TargetParameter(self.target_parameter.name, result)
         return SingleOutput(self.target_parameter, tuple(self.args.physical_args.values()))
 
 
 class _AllTargetHandler(_Handler):
     def __init__(self, args):
@@ -175,20 +187,28 @@
                 )
                 for p in reqd_params
             )
 
             target_param = TargetParameter(ret_param)
 
             result = compute(func, *func_args)
+            units = _CONFIG["units"].get(target_param.name)
             if not target_param.is_unitless:
-                units = self.args["units"] or _CONFIG["units"].get(target_param.name)
                 try:
                     result = result.to(units)
                 except (DimensionalityError, UndefinedUnitError, ValueError) as ex:
                     quit_print(str(ex))
+            else:
+                if units:
+                    quit_print(
+                        f"Units '{units}' given for dimensionless target '{target_param.name}'"
+                    )
+
+            for arg in filter(lambda p: isinstance(p, ArgParameter), func_args):
+                arg._used = True
 
             target_param = TargetParameter(ret_param, result)
             computed_targets[target_param] = reqd_params
 
         to_update = {}
         for tgt_p, reqd_params in computed_targets.items():
             for rp in reqd_params:
@@ -220,21 +240,24 @@
         return MultiOutput(computed_targets, tuple(self.args.physical_args.values()))
 
 
 def compute(func, *args) -> Q_:
     try:
         return func(*(arg_p.value for arg_p in args))
     except Exception as ex:
+        if isinstance(ex, CavCalcError):
+            raise
+
         if isinstance(ex, ValueError) and "operands could not be broadcast" in str(ex):
             shapes = (str(getattr(arg_p.value.m, "shape", 1)) for arg_p in args)
             quit_print(
                 f"Encountered inconsistent parameter shapes when calling {func.__name__}. "
                 f"Parameters: {{{', '.join(arg_p.name for arg_p in args)}}}, with shapes: "
                 f"{{{', '.join(shapes)}}}, could not be broadcast together."
             )
         else:
             bug(
                 "The following error occurred:\n\n"
                 f"\t{ex}\n\n"
                 f"when calling {func.__name__} with arguments:\n\n"
-                + "\n\t".join(arg_p.compact_str for arg_p in args)
+                + "\n\t".join(str(arg_p) for arg_p in args)
             )
```

### Comparing `cavcalc-1.1.0/src/cavcalc/_main.py` & `cavcalc-1.2.0/src/cavcalc/_main.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/_session.py` & `cavcalc-1.2.0/src/cavcalc/_session.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/calculate.py` & `cavcalc-1.2.0/src/cavcalc/calculate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 A module holding the primary function for interacting with ``cavcalc``
 via the API.
 """
 
 import numpy as np
+import os
+from tempfile import NamedTemporaryFile
 
 from . import _SESSION, Q_
 from .errors import CavCalcError
 from ._handler import make_handler as _make_handler
-from .parameters import ArgParameter, ParameterType, valid_arguments, valid_targets
+from .parameters import ArgParameter, Parameter, ParameterType, valid_arguments, valid_targets
 from .parameters.tools import get_name
 
 
 def calculate(target=None, meshes=None, **kwargs):
     """Calculates a target parameter from an arbitrary number of physical arguments.
 
     If no `target` is specified then the default behaviour is to calculate all computable
@@ -71,14 +73,15 @@
 
         Each kwarg value can be specified as:
 
         * A single value, or an array of values. The units of this value will correspond to
           those of the associated parameter, or parameter category, in the config file being used.
         * A ``cavcalc.ureg.Quantity`` instance. See the Pint documentation for details on
           instantiating ``Quantity`` objects.
+        * A :class:`.Parameter` object: i.e. an entry from an existing :class:`.BaseOutput` instance.
         * Or any value which can be converted into a ``Quantity`` instance; e.g. a string
           (such as ``"10cm"``) or a tuple (such as ``(310, "deg")``).
 
     Parameters
     ----------
     target : str | :class:`.ParameterType`, optional
         The target parameter to compute, can be specified as a string (see drop-down box above) or
@@ -156,14 +159,20 @@
 
         out = cc.calculate(L="3cm", w1="100um", w2="120um")
 
         # .value is the pint.Quantity object
         print(f"Rc1 = {out.get('Rc1').value.to('mm'):~}")
         print(f"Rc2 = {out.get('Rc2').value.to('mm'):~}")
 
+    Compute the fractional transmission intensity over a grid of the mirror reflectivities:
+
+    .. jupyter-execute::
+
+        out = cc.calculate("Atrn", R1=np.linspace(0, 1, 250), R2="R1", meshes=True).plot(cmap="hot");
+
     Plot the radius of the beam at the waist position, as a function of the beam radii
     on the mirrors; whilst using :func:`.configure` to temporarily override the default
     units (loaded from the config files) for beam-size type parameters:
 
     .. jupyter-execute::
 
         w_arr = np.linspace(80, 150, 499)
@@ -178,44 +187,66 @@
         else:
             target = get_name(target)
             if target not in valid_targets:
                 raise CavCalcError(f"Invalid target '{target}'")
     else:
         target = "all"
 
+    tmp_files = []
     command = [target]
     for arg, value in kwargs.items():
         if arg not in valid_arguments:
             raise CavCalcError(f"Unrecognised / invalid argument '{arg}'")
 
-        if isinstance(value, tuple):
+        if isinstance(value, str) and value in valid_arguments:  # parameter reference
+            command.extend([f"-{arg}", value])
+            continue
+
+        if isinstance(value, Parameter):
+            value = value.value
+        elif isinstance(value, tuple):
             if len(value) != 2:
                 raise CavCalcError(f"Expected tuple of length 2 for argument '{arg}'")
             value = Q_(*value)
         else:
             value = Q_(value)
 
         arg_param = ArgParameter(arg, value)
 
         command.append(arg_param.cli_form)
         units_str = str(arg_param.value.units)
         if arg_param.is_array:
-            start = np.min(arg_param.value.m)
-            stop = np.max(arg_param.value.m)
-            size = arg_param.value.m.size
+            # If the array is irregularly spaced, then we need to save it to a
+            # tmp file for loading later on in the parser (as the data-range
+            # syntax only allows for linearly spaced array args).
+            if np.any(np.abs(np.diff(arg_param.value.m, n=2)) > 1e-15):
+                with NamedTemporaryFile(suffix=".npy", delete=False) as f:
+                    np.save(f, arg_param.value.m)
+                    command.append(f.name)
+                    tmp_files.append(f.name)
+            else:
+                start = np.min(arg_param.value.m)
+                stop = np.max(arg_param.value.m)
+                size = arg_param.value.m.size
 
-            command.append(f"{start} {stop} {size} {units_str}")
+                command.append(f"{start} {stop} {size} {units_str}")
         else:
             command.append(f"({arg_param.value.m}){units_str}")
 
     if meshes:
         command.append("--mesh")
         command.append(_deduce_meshes(meshes))
 
-    return _make_handler(_SESSION.parse_args(command)).run()
+    out = _make_handler(_SESSION.parse_args(command)).run()
+
+    for tmp_f in tmp_files:
+        if os.path.isfile(tmp_f):
+            os.remove(tmp_f)
+
+    return out
 
 
 def _deduce_meshes(meshes):
     if isinstance(meshes, (str, bool)):
         return str(meshes)
 
     err_msg = "Could not deduce mesh parameters from specified meshes argument."
```

### Comparing `cavcalc-1.1.0/src/cavcalc/cavcalc.ini` & `cavcalc-1.2.0/src/cavcalc/cavcalc.ini`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/env.py` & `cavcalc-1.2.0/src/cavcalc/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Local environment settings modification for cavcalc."""
 
 import os
 import warnings
 
 from . import _CONFIG
 from .errors import CavCalcError
+from .parameters import ParameterCategory
+from .parameters.tools import get_names
 
 
 class _ConfigureContext:
     def __init__(self, previous_units: dict[str, str], original_rc_params: dict):
         self.__prev = previous_units
         self.__orig_rc = original_rc_params
 
@@ -92,17 +94,23 @@
             for p in params:
                 # Only use category override if specific units
                 # override is *not* also in the kwargs
                 param_units.setdefault(p, pcat_units)
 
             del param_units[pcat]
 
+    dimensionless_params = get_names(ParameterCategory.Power, ParameterCategory.Stability)
+
     cfg_units = _CONFIG["units"]
     prev = {}
     for p, units in param_units.items():
         if curr_units := cfg_units.get(p):
             prev[p] = curr_units
             cfg_units[p] = units
         else:
-            warnings.warn(f"Ignoring units override for invalid parameter name: {p}")
+            msg = "Ignoring units override for "
+            if p in dimensionless_params:
+                warnings.warn(msg + f"dimensionless parameter: {p}")
+            else:
+                warnings.warn(msg + f"invalid parameter name: {p}")
 
     return _ConfigureContext(prev, orig_rc)
```

### Comparing `cavcalc-1.1.0/src/cavcalc/functions/__init__.py` & `cavcalc-1.2.0/src/cavcalc/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/functions/_maps.py` & `cavcalc-1.2.0/src/cavcalc/functions/_maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,26 @@
         (ParameterType.CAV_LENGTH, ParameterType.REFLECTIVITY_M1, ParameterType.REFLECTIVITY_M2),
         ParameterType.FWHM,
     ),
     pole: (
         (ParameterType.CAV_LENGTH, ParameterType.REFLECTIVITY_M1, ParameterType.REFLECTIVITY_M2),
         ParameterType.POLE,
     ),
+    Aint_of_R1R2: (
+        (ParameterType.REFLECTIVITY_M1, ParameterType.REFLECTIVITY_M2),
+        ParameterType.RES_ENHANCE_INTERNAL,
+    ),
+    Aext_of_R1R2: (
+        (ParameterType.REFLECTIVITY_M1, ParameterType.REFLECTIVITY_M2),
+        ParameterType.RES_ENHANCE_EXTERNAL,
+    ),
+    Atrn_of_R1R2: (
+        (ParameterType.REFLECTIVITY_M1, ParameterType.REFLECTIVITY_M2),
+        ParameterType.TRANSMISSION_INTENSITY_FRAC,
+    ),
 }
 
 
 SYMMETRIC_TARGETS_FUNC_MAP = {
     w_of_gsingle: (
         (ParameterType.CAV_LENGTH, ParameterType.WAVELENGTH, ParameterType.GFACTOR_SINGLE),
         ParameterType.BEAMSIZE,
```

### Comparing `cavcalc-1.1.0/src/cavcalc/functions/_utils.py` & `cavcalc-1.2.0/src/cavcalc/functions/_utils.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/functions/asymmetric.py` & `cavcalc-1.2.0/src/cavcalc/functions/asymmetric.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/functions/resonance.py` & `cavcalc-1.2.0/src/cavcalc/functions/resonance.py`

 * *Files 19% similar despite different names*

```diff
@@ -128,7 +128,43 @@
     In the equation below, :math:`\nu(L)` is the FSR, and :math:`\mathcal{F}(R_1,R_2)` is
     the finesse.
 
     .. math::
         \nu_p(L, R_1, R_2) = \frac{\nu(L)}{2\mathcal{F}(R_1, R_2)}
     """
     return 0.5 * _fsr_base(L) / _finesse_base(R1, R2)
+
+
+@check_physical()
+@ureg.wraps("", ("", ""))
+def Aint_of_R1R2(R1, R2):
+    r"""The internal resonance enhancement factor of a cavity where the first mirror has
+    (power) reflectivity :math:`R_1` and the second mirror has reflectivity :math:`R_2`.
+
+    .. math::
+        A_{\mathrm{circ}} = \frac{1}{(1 - \sqrt{R_1 R_2})^2}
+    """
+    return 1 / (1 - np.sqrt(R1 * R2)) ** 2
+
+
+@check_physical()
+@ureg.wraps("", ("", ""))
+def Aext_of_R1R2(R1, R2):
+    r"""The external resonance enhancement factor of a cavity where the first mirror has
+    (power) reflectivity :math:`R_1` and the second mirror has reflectivity :math:`R_2`.
+
+    .. math::
+        A'_{\mathrm{circ}} = \frac{1 - R_1}{(1 - \sqrt{R_1 R_2})^2}
+    """
+    return (1 - R1) / (1 - np.sqrt(R1 * R2)) ** 2
+
+
+@check_physical()
+@ureg.wraps("", ("", ""))
+def Atrn_of_R1R2(R1, R2):
+    r"""The fractional transmission intensity of a cavity where the first mirror has
+    (power) reflectivity :math:`R_1` and the second mirror has reflectivity :math:`R_2`.
+
+    .. math::
+        A'_{\mathrm{trn}} = \frac{(1 - R_1)(1 - R_2)}{(1 - \sqrt{R_1 R_2})^2}
+    """
+    return (1 - R1) * (1 - R2) / (1 - np.sqrt(R1 * R2)) ** 2
```

### Comparing `cavcalc-1.1.0/src/cavcalc/functions/symmetric.py` & `cavcalc-1.2.0/src/cavcalc/functions/symmetric.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.1.0/src/cavcalc/output.py` & `cavcalc-1.2.0/src/cavcalc/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if not isinstance(output, (SingleOutput, MultiOutput)):
             raise CavCalcError(f"Unrecognised serialized object in {file}")
 
     return output
 
 
 def _param_str_gen(params: Sequence[Union[ArgParameter, TargetParameter]]):
-    return (f"{p.description} = {p.value:~}" for p in params)
+    return (f"{'' if getattr(p, 'was_used', True) else '[UNUSED] '}{p}" for p in params)
 
 
 class BaseOutput(abc.ABC):
     """Abstract base class for output objects. Both :class:`.SingleOutput` and
     :class:`.MultiOutput` derive from this type."""
 
     category_order = (
@@ -263,15 +263,15 @@
             else:
                 plt.sca(fig.subplots())
 
         def _make_label(p: ArgParameter):
             return p.description + (f" [{p.value.units:~}]" if not p.is_unitless else "")
 
         # The non-array arguments specified
-        if fixed := tuple(filter(lambda p: p.is_scalar, given)):
+        if fixed := tuple(filter(lambda p: p.is_scalar and p.was_used, given)):
             fixed_params_str = "with: " + ", ".join(f"{p.symbol_str} = {p.value:~}" for p in fixed)
         else:
             fixed_params_str = ""
 
         if plotting_dims == 1 or num_x_arrays == 1:
             if num_x_arrays > 2:
                 _quit_print("Plots with more than two x-axes are not supported.")
```

### Comparing `cavcalc-1.1.0/src/cavcalc/parameters/_maps.py` & `cavcalc-1.2.0/src/cavcalc/parameters/_maps.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,20 @@
     "gs": ParameterType.GFACTOR_SINGLE,
     "L1": ParameterType.LOSS_M1,
     "L2": ParameterType.LOSS_M2,
     "modesep": ParameterType.MODESEP,
     "pole": ParameterType.POLE,
     "R1": ParameterType.REFLECTIVITY_M1,
     "R2": ParameterType.REFLECTIVITY_M2,
+    "Aint": ParameterType.RES_ENHANCE_INTERNAL,
+    "Aext": ParameterType.RES_ENHANCE_EXTERNAL,
     "Rc": ParameterType.ROC,
     "Rc1": ParameterType.ROC_M1,
     "Rc2": ParameterType.ROC_M2,
+    "Atrn": ParameterType.TRANSMISSION_INTENSITY_FRAC,
     "T1": ParameterType.TRANSMISSION_M1,
     "T2": ParameterType.TRANSMISSION_M2,
     "z0": ParameterType.WAISTPOS,
     "w0": ParameterType.WAISTSIZE,
     "wl": ParameterType.WAVELENGTH,
 }
 
@@ -49,14 +52,17 @@
     ParameterType.POLE: ParameterCategory.Frequency,
     ParameterType.MODESEP: ParameterCategory.Frequency,
     ParameterType.GOUY: ParameterCategory.Phase,
     ParameterType.LOSS_M1: ParameterCategory.Power,
     ParameterType.LOSS_M2: ParameterCategory.Power,
     ParameterType.REFLECTIVITY_M1: ParameterCategory.Power,
     ParameterType.REFLECTIVITY_M2: ParameterCategory.Power,
+    ParameterType.RES_ENHANCE_INTERNAL: ParameterCategory.Power,
+    ParameterType.RES_ENHANCE_EXTERNAL: ParameterCategory.Power,
+    ParameterType.TRANSMISSION_INTENSITY_FRAC: ParameterCategory.Power,
     ParameterType.TRANSMISSION_M1: ParameterCategory.Power,
     ParameterType.TRANSMISSION_M2: ParameterCategory.Power,
     ParameterType.FINESSE: ParameterCategory.Power,
     ParameterType.CAV_GFACTOR: ParameterCategory.Stability,
     ParameterType.GFACTOR_SINGLE: ParameterCategory.Stability,
     ParameterType.GFACTOR_M1: ParameterCategory.Stability,
     ParameterType.GFACTOR_M2: ParameterCategory.Stability,
@@ -79,17 +85,20 @@
     ParameterType.GOUY: "Round-trip Gouy phase",
     ParameterType.LOSS_M1: "Loss of first mirror",
     ParameterType.LOSS_M2: "Loss of second mirror",
     ParameterType.MODESEP: "Mode separation frequency",
     ParameterType.POLE: "Pole frequency",
     ParameterType.REFLECTIVITY_M1: "Reflectivity of first mirror",
     ParameterType.REFLECTIVITY_M2: "Reflectivity of second mirror",
+    ParameterType.RES_ENHANCE_INTERNAL: "Internal resonance enhancement factor",
+    ParameterType.RES_ENHANCE_EXTERNAL: "External resonance enhancement factor",
     ParameterType.ROC: "Radius of curvature of both mirrors",
     ParameterType.ROC_M1: "Radius of curvature of first mirror",
     ParameterType.ROC_M2: "Radius of curvature of second mirror",
+    ParameterType.TRANSMISSION_INTENSITY_FRAC: "Fractional transmission intensity",
     ParameterType.TRANSMISSION_M1: "Transmission of first mirror",
     ParameterType.TRANSMISSION_M2: "Transmission of second mirror",
     ParameterType.WAISTPOS: "Position of beam waist (from first mirror)",
     ParameterType.WAISTSIZE: "Radius of beam at waist",
     ParameterType.WAVELENGTH: "Wavelength of beam",
 }
 
@@ -109,16 +118,19 @@
     ParameterType.GOUY: r"$\psi$",
     ParameterType.LOSS_M1: "$L_1$",
     ParameterType.LOSS_M2: "$L_2$",
     ParameterType.MODESEP: r"$\delta f$",
     ParameterType.POLE: r"$\nu_p$",
     ParameterType.REFLECTIVITY_M1: "$R_1$",
     ParameterType.REFLECTIVITY_M2: "$R_2$",
+    ParameterType.RES_ENHANCE_INTERNAL: r"$A_{\mathrm{circ}}$",
+    ParameterType.RES_ENHANCE_EXTERNAL: r"$A'_{\mathrm{circ}}$",
     ParameterType.ROC: "$R_C$",
     ParameterType.ROC_M1: "$R_{C,1}$",
     ParameterType.ROC_M2: "$R_{C,2}$",
+    ParameterType.TRANSMISSION_INTENSITY_FRAC: r"$A'_{\mathrm{trn}}$",
     ParameterType.TRANSMISSION_M1: "$T_1$",
     ParameterType.TRANSMISSION_M2: "$T_2$",
     ParameterType.WAISTPOS: "$z_0$",
     ParameterType.WAISTSIZE: "$w_0$",
     ParameterType.WAVELENGTH: r"$\lambda$",
 }
```

### Comparing `cavcalc-1.1.0/src/cavcalc/parameters/enums.py` & `cavcalc-1.2.0/src/cavcalc/parameters/enums.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,17 +24,20 @@
     GOUY = auto()
     LOSS_M1 = auto()
     LOSS_M2 = auto()
     MODESEP = auto()
     POLE = auto()
     REFLECTIVITY_M1 = auto()
     REFLECTIVITY_M2 = auto()
+    RES_ENHANCE_INTERNAL = auto()
+    RES_ENHANCE_EXTERNAL = auto()
     ROC = auto()
     ROC_M1 = auto()
     ROC_M2 = auto()
+    TRANSMISSION_INTENSITY_FRAC = auto()
     TRANSMISSION_M1 = auto()
     TRANSMISSION_M2 = auto()
     WAISTPOS = auto()
     WAISTSIZE = auto()
     WAVELENGTH = auto()
```

### Comparing `cavcalc-1.1.0/src/cavcalc/parameters/parameter.py` & `cavcalc-1.2.0/src/cavcalc/parameters/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,45 +52,24 @@
 
                 if not value.check(default_units):
                     _quit_print(f"Invalid units ({value.units}) given for parameter {self.name}")
 
         self._value = value
 
     def __str__(self):
-        if self.value is not None:
-            if self.is_array:
-                value_str = (
-                    f"Values:\n"
-                    f"\t\tfirst = {self.value.m[0]}\n"
-                    f"\t\tlast  = {self.value.m[-1]}\n"
-                    f"\t\tsize  = {self.value.m.size}"
-                )
-            else:
-                value_str = f"Value: {self.value.m}"
-        else:
-            value_str = ""
-
-        return (
-            f"{self.description}:\n"
-            f"\tCategory: {self.category}\n"
-            f"\t{value_str}\n"
-            f"\tUnits: {self.value.units}"
+        return self.description + (
+            f" = {self.value:~}" if self.value is not None else " [uninitialized]"
         )
 
     @property
     def category(self) -> ParameterCategory:
         """The :class:`.ParameterCategory` that this parameter belongs to."""
         return self.__category
 
     @property
-    def compact_str(self):
-        """A shortened string representation of the parameter with its value."""
-        return self.name + f": {self.value:~}" if self.value is not None else ""
-
-    @property
     def description(self):
         """A brief description of the parameter type."""
         return _PTYPE_DESCR_MAP[self.ptype]
 
     @property
     def has_angular_units(self):
         """Whether the units of this parameter are of angular type."""
@@ -156,14 +135,15 @@
         are constructed during the argument parsing, and calculation process.
     """
 
     def __init__(self, name_or_ptype, value: Q_ = None, index: int = None, axis: int = None):
         super().__init__(name_or_ptype, value)
         self.__index = index
         self.__axis = axis
+        self._used = False
 
     @property
     def axis(self):
         """The axis that the parameter corresponds to, as an integer indexed from zero.
 
         If :attr:`.Parameter.is_scalar` is true, then this will be None. Otherwise, it
         is an integer.
@@ -176,14 +156,19 @@
         return f"-{self.name}"
 
     @property
     def index(self):
         """The index of the argument in the sequence of specified args."""
         return self.__index
 
+    @property
+    def was_used(self):
+        """Whether this parameter was used in its associated :func:`.calculate` call."""
+        return self._used
+
 
 class TargetParameter(Parameter):
     """Cavity parameters which represent targets computed by cavcalc.
 
     .. note::
 
         You should never need to instantiate objects of this type manually. These
```

### Comparing `cavcalc-1.1.0/src/cavcalc/parameters/tools.py` & `cavcalc-1.2.0/src/cavcalc/parameters/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Functions for retrieving information on parameters, typically provided via
 both str and :class:`.ParameterType` arguments.
 """
 
+from collections import defaultdict
 from typing import Union as _Union
 
-from . import ParameterType
+from . import ParameterType, ParameterCategory
 from ._maps import (
     NAME_PTYPE_MAP as _NAME_PTYPE_MAP,
     PTYPE_NAME_MAP as _PTYPE_NAME_MAP,
     PTYPE_DESCR_MAP as _PTYPE_DESCR_MAP,
+    PTYPE_CATEGORY_MAP as _PTYPE_CAT_MAP,
 )
 
+from ..errors import CavCalcError
+
 
 def get_default_units(ptype: _Union[str, ParameterType]):
     """Get the default units, as a string, of the given parameter type.
 
     The default units value is obtained from the loaded config file(s); i.e.
     the first instance of the corresponding option in the load order: current
     working directory -> user config directory -> package install location.
@@ -53,23 +57,45 @@
     name : Optional[str]
         The name of the parameter, or ``None`` if ``ptype`` does not correspond to
         any parameter.
     """
     return _PTYPE_NAME_MAP.get(ptype)
 
 
-def get_names():
-    """Retrieve a tuple of the names of all the parameters exposed by cavcalc.
+def get_names(*args) -> tuple[str]:
+    """Retrieve a tuple of the names of all the parameters exposed by cavcalc, or
+    all the parameters in the categories given in ``args``.
+
+    Parameters
+    ----------
+    args : Sequence[:class:`.ParameterCategory`]
+        A sequence of :class:`.ParameterCategory` literals from which
+        to obtain parameter names. If none given, then all parameter
+        names will be returned.
 
     Returns
     -------
     names : tuple[str]
-        The names of all the parameters.
+        The names of the parameters.
     """
-    return tuple(_NAME_PTYPE_MAP.keys())
+    if not args:
+        return tuple(_NAME_PTYPE_MAP.keys())
+
+    if not all(isinstance(arg, ParameterCategory) for arg in args):
+        raise CavCalcError("All args must be of type ParameterCategory.")
+
+    cat_to_types = defaultdict(set)
+    for ptype, cat in _PTYPE_CAT_MAP.items():
+        cat_to_types[cat].add(ptype)
+
+    ptypes = set()
+    for arg in args:
+        ptypes.update(cat_to_types[arg])
+
+    return tuple(get_name(ptype) for ptype in ptypes)
 
 
 def get_names_descriptions() -> dict[str, str]:
     """Get a dictionary of all the parameter names with a description of each of these.
 
     Returns
     -------
@@ -112,15 +138,19 @@
     """
     non_arg_ptypes = (
         ParameterType.FINESSE,
         ParameterType.FSR,
         ParameterType.FWHM,
         ParameterType.MODESEP,
         ParameterType.POLE,
+        ParameterType.RES_ENHANCE_INTERNAL,
+        ParameterType.RES_ENHANCE_EXTERNAL,
+        ParameterType.TRANSMISSION_INTENSITY_FRAC,
         ParameterType.WAISTPOS,
+        ParameterType.WAISTSIZE,
     )
     return tuple(name for name in get_names() if get_type(name) not in non_arg_ptypes)
 
 
 def get_valid_targets():
     """Get the names of all the parameters which can be specified as targets
     in a :func:`.calculate` / CLI call.
```

### Comparing `cavcalc-1.1.0/PKG-INFO` & `cavcalc-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavcalc
-Version: 1.1.0
+Version: 1.2.0
 Summary: A program for computing Fabry-Perot optical cavity parameters.
 Home-page: https://cavcalc.readthedocs.io/en/latest/
 License: GPL-3.0-or-later
 Keywords: physics,optics,interferometry
 Author: Samuel Rowlinson
 Author-email: samueljrowlinson@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -47,15 +47,15 @@
 ```bash
 cavcalc --version
 ```
 
 if you see something along the lines of
 
 ```
-cavcalc v1.1.0
+cavcalc v1.2.0
 ```
 
 then you should be ready to start using `cavcalc`!
 
 **Note**: As is often recommended with the installation of Python packages (especially those with dependencies
 on packages such as `numpy` and `matplotlib`, as is the case here), you should prefer to install `cavcalc` in
 a suitable virtual environment. See [the official documentation on Python virtual environments](https://docs.python.org/3/tutorial/venv.html)
@@ -116,15 +116,15 @@
 
 ### Computing all available parameters
 
 A compute target of `all` is the default choice which is used to calculate all parameters which can be determined
 from the arguments specified. For example, using approximate values of the Advanced LIGO arm cavity parameters,
 
 ```bash
-cavcalc -L 4km -Rc1 1934 -Rc2 2245 -T1 0.014 -L1 37.5e-6 -T2 5e-6 -L2 37.5e-6
+cavcalc -L 4km -Rc1 1934 -Rc2 2245 -T1 0.014 -L1 37.5e-6 -T2 5e-6 -L2 L1
 ```
 
 gives the following output:
 
 ```
 Given:
 	Loss of first mirror = 3.75e-05
@@ -144,14 +144,17 @@
 	FWHM = 84.56921734107604 Hz
 	Mode separation frequency = 4988.072188176178 Hz
 	Pole frequency = 42.28460867053802 Hz
 
 	Finesse = 443.11699254426594
 	Reflectivity of first mirror = 0.9859625
 	Reflectivity of second mirror = 0.9999574999999999
+	Internal resonance enhancement factor = 20036.317877295227
+	External resonance enhancement factor = 281.2598122025325
+	Fractional transmission intensity = 0.011953542018623487
 
 	Position of beam waist (from first mirror) = 1837.2153886417168 m
 
 	Radius of beam at first mirror = 53.421066433049255 mm
 	Radius of beam at second mirror = 62.448079883230896 mm
 	Radius of beam at waist = 11.950538458990879 mm
 
@@ -237,19 +240,22 @@
 
 ![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_w_vs_L_gouy.png)
 
 A matplotlib compliant colour-map can be specified when making an image plot using the `--cmap <name>` option. For example,
 the following command gives the plot shown below.
 
 ```bash
-cavcalc gouy -L 12um -g1 "-2 2 499" -g2 "-2 2 499" --mesh true --plot --cmap Spectral_r
+cavcalc gouy -g1 "-2 2 499" -g2 g1 --mesh true --plot --cmap Spectral_r
 ```
 
 ![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/asymmcav_w0_vs_g1g2.png)
 
+**Note** that here we also used the parameter-referencing feature of `cavcalc`, introduced in v1.2.0, to set
+the values of `g1` to those of `g2`.
+
 ## A note on g-factors
 
 Stability (g) factors are split into four different parameters for implementation purposes and to
 hopefully make it clearer as to which argument is being used and whether the resulting cavity
 computations are for a symmetric or asymmetric cavity. These arguments are detailed here:
 
 - `-gs` : The symmetric, singular stability factor. This represents the individual g-factors of **both**
```

