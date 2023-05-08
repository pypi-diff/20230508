# Comparing `tmp/misura-1.5.1.tar.gz` & `tmp/misura-1.5.2.tar.gz`

## Comparing `misura-1.5.1.tar` & `misura-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.1/.gitattributes
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.5.1/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 misura-1.5.1/docs/docs.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/__main__.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/exceptions.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/globals.py
--rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/quantities.py
--rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/tables.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/utilities.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 misura-1.5.1/tests/tests.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.1/LICENSE
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 misura-1.5.1/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 misura-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.2/.gitattributes
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 misura-1.5.2/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 misura-1.5.2/docs/docs.md
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 misura-1.5.2/src/test.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/__main__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/exceptions.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/globals.py
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/quantities.py
+-rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/tables.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.2/src/misura/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.2/LICENSE
+-rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 misura-1.5.2/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 misura-1.5.2/PKG-INFO
```

### Comparing `misura-1.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/.github/workflows/python-publish.yml` & `misura-1.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/docs/docs.md` & `misura-1.5.2/docs/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,42 +30,42 @@
 
 **misura** is written in Python and developed by [Andrea Di Antonio](https://github.com/diantonioandrea).
 
 ## Quantities
 
 [Go back to ToC](#table-of-contents)
 
-Quantities are defined as `misura.quantity(value: any, unit: str = "", uncertainty: any = 0)` objects.
+Quantities are defined as `quantities.quantity(value: any, unit: str = "", uncertainty: any = 0)` objects.
 
 `values` stands for the value of the quantity itself, while `unit` represents its unit of measure.  
 `quantity(2, "kg")` is a well-defined quantity.
 
 `unit` is a string in which the different units of measure must be _separated by a space_ and _followed by their exponent_, if different from `1`.  
 `quantity(3, "m s-1")` is a well-defined quantity.
 
 `uncertainty` stands for the quantity's uncertainty.  
 `quantity(3, "s", 0.5)` is a well-defined quantity.
 
 ### Methods
 
-`misura.quantity` objects implement the following methods:
+`quantities.quantity` objects implement the following methods:
 
 ```python
 def unit(self, print: bool = False) -> str
 def dimesion(self) -> str
 ```
 
 which:
 
 - `unit()`: Returns the units string of the quantity. It returns it in a fancier way if `print = True`.
 - `dimesion()`: Returns the dimesion string of the quantity if it is convertible.
 
 ### Operations
 
-`misura.quantity` objects implement the following dunder methods:
+`quantities.quantity` objects implement the following dunder methods:
 
 ```python
 def __str__(self) -> str
 def __repr__(self) -> str
 def __format__(self, string) -> str
 
 def __int__(self) -> int
@@ -84,15 +84,15 @@
 
 def __add__(self, other: any) -> any
 def __sub__(self, other: any) -> any
 def __mul__(self, other: any) -> any
 def __truediv__(self, other: any) -> any
 def __floordiv__(self, other: any) -> any
 def __pow__(self, other: any) -> any
-# def __mod__(self, other: any) -> any
+def __mod__(self, other: any) -> any
 
 def __lt__(self, other: any) -> any
 def __le__(self, other: any) -> any
 def __gt__(self, other: any) -> any
 def __ge__(self, other: any) -> any
 def __eq__(self, other: any) -> any
 def __ne__(self, other: any) -> any
@@ -230,16 +230,17 @@
 
 ## Global options
 
 [Go back to ToC](#table-of-contents)
 
 **misura** implements the following global options:
 
-- `misura.style.quantityHighlighting`, bool: Enables units of measure highlighting. Dafault: `True`.
-- `misura.style.quantityPlusMinus`, string: "+-" symbol. Dafault: `" \u00b1 "`.
+- `globals.style.quantityHighlighting`, bool: Enables units of measure highlighting. Dafault: `True`.
+- `globals.style.quantityPlusMinus`, string: "+-" symbol. Dafault: `" \u00b1 "`.
+- `globals.logic.ignoreUncertainty`, bool: Whether to ignore uncertainty during comparisons. Dafault: `False`.
 
 Take a look at these [examples](#global-options-1)
 
 ## Exceptions
 
 [Go back to ToC](#table-of-contents)
 
@@ -257,15 +258,15 @@
 ## Examples
 
 [Go back to ToC](#table-of-contents)
 
 ### Quantities
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 import math
 import numpy
 
 num1 = quantity(7, "m s-1", 1)
 num2 = quantity(4, "km")
 num3 = numpy.array([quantity(2, "m", .5), quantity(4, "km", .1)])
 num4 = quantity(numpy.array([1, 2, 3]), "T")
@@ -288,15 +289,16 @@
 4002 ± 100 m
 [1 2 3] T
 ```
 
 ### Units of measure
 
 ```python
-from misura import quantity, convert, addUnit
+from misura.quantities import quantity, convert
+fromm misura.tables import addUnit
 
 addUnit("volume", {"L": 1, "daL": 10, "hL": 100, "kL": 1000, "dL": 0.1, "cL": 0.01, "mL": 0.001}, "dm3")
 
 num1 = quantity(3, "L")
 
 print(convert(num1, "cm3"))
 ```
@@ -306,15 +308,15 @@
 ```
 3000.0 cm(3)
 ```
 
 ### Conversions, unpacking and packing
 
 ```python
-from misura import quantity, convert, unpack, pack
+from misura.quantities import quantity, convert, unpack, pack
 
 num1 = quantity(2, "m2")
 num2 = quantity(4, "kg")
 num3 = quantity(2, "J2")
 num4 = quantity(4, "C H")
 num5 = quantity(7, "N m")
 num6 = quantity(9, "J")
@@ -338,16 +340,16 @@
 16.0 J
 45.0 C(2)
 ```
 
 ### Global options
 
 ```python
-from misura import quantity
-from misura import style
+from misura.quantities import quantity
+from misura.globals import style
 
 style.quantityHighlighting = False
 style.quantityPlusMinus = " +- "
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(5, "s", 1)
```

### Comparing `misura-1.5.1/src/misura/__main__.py` & `misura-1.5.2/src/misura/__main__.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/src/misura/exceptions.py` & `misura-1.5.2/src/misura/exceptions.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/src/misura/quantities.py` & `misura-1.5.2/src/misura/quantities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # Quantities.
 from __future__ import annotations
 
 from colorama import Style
-from math import sqrt
+from math import sqrt, log
 
 from .exceptions import (
     UnitError,
     QuantityError,
     ConversionError,
     UnpackError,
     PackError,
     UncertaintyComparisonError,
 )
 from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
 from .utilities import dictFromUnit, unitFromDict, checkIter, uAll, uAny
+from .globals import style, logic
 
 
 class quantity:
     """
-    The main class of misura, the class of quantities.
+    misura's quantity class.
     """
 
     def __init__(self, value: any, unit: str = "", uncertainty: any = 0) -> None:
         """
-        value: Can be anything that can be somewhat treated as a number.
-        unit: A properly formatted string including all the units with their exponents. e.g. "m s-1".
+        Quantity initialization.
+
+        - value: Can be anything that can be somewhat treated as a number.
+        - unit: A properly formatted string including all the units with their exponents. e.g. "m s-1".
+        - uncertainty: Value's uncertainty.
         """
 
         try:
             assert isinstance(unit, str)
             assert uAll(uncertainty >= 0) if uAny(uncertainty) else True
             assert (
                 (checkIter(value) == checkIter(uncertainty))
@@ -59,17 +63,17 @@
             if self.convertible
             else dict()
         )
 
     def unit(self, print: bool = False) -> str:
         """
         Returns a readable version of the quantity's unit.
-        print = True makes the output fancier.
+
+        'print = True' makes the output fancier.
         """
-        from .globals import style
 
         # Fancy version.
         if print:
             # {"m": 1, "s": -1} -> "[m / s]".
             numerator = " ".join(
                 sorted(
                     [
@@ -120,15 +124,14 @@
 
         # {"m": 1, "s": -1} -> "m s-1".
         return unitFromDict(self.units)
 
     def dimesion(self) -> str:
         """
         Returns a readable version of the quantity's dimesion.
-        No fancy style.
         """
 
         if not len(self.dimesions):
             return ""
 
         # {"length": 2, "time": -1} -> "[length(2) / time]".
         numerator = " * ".join(
@@ -199,18 +202,15 @@
                 if uAny(self.uncertainty)
                 else ""
             )
             + (" " + self.unit(print=True) if self.unit() else "")
         )
 
     # PYTHON TYPES CONVERSION.
-
-    """
-    int, float and complex don't care about uncertainty.
-    """
+    # int, float and complex don't care about uncertainty.
 
     # Int.
     def __int__(self) -> int:
         return int(self.value)
 
     # Float.
     def __float__(self) -> float:
@@ -218,26 +218,22 @@
 
     # Complex.
     def __complex__(self) -> complex:
         return complex(self.value)
 
     # Bool.
     def __bool__(self) -> bool:
-        return bool(self.value or self.uncertainty)
+        return bool(uAny(self.value) or uAny(self.uncertainty))
 
     # MATH.
 
     # Abs.
     def __abs__(self) -> quantity:
-        # Since abs(number) cannot be negative, the uncertainty on this value gets modified.
-        return quantity(
-            abs(self.value),
-            self.unit(),
-            self.uncertainty if uAny(self.uncertainty) < self.value else self.value,
-        )
+        # Ignores the case in which abs(uncertainty) > abs(value).
+        return quantity(abs(self.value), self.unit(), self.uncertainty)
 
     # Positive.
     def __pos__(self) -> quantity:
         return quantity(+self.value, self.unit(), self.uncertainty)
 
     # Negative.
     def __neg__(self) -> quantity:
@@ -270,22 +266,23 @@
         from math import trunc
 
         return quantity(trunc(self.value), self.unit(), trunc(self.uncertainty))
 
     # Addition.
     def __add__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
+            # Addition between pure numbers.
             if self.unit():
                 raise QuantityError(self, quantity(other, ""), "+")
 
             return quantity(self.value + other, "", self.uncertainty)
 
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
-                # Chooses the one to convert.
+                # Chooses the one to convert based on unit length.
                 first = convert(self, other.unit())
                 second = convert(other, self.unit())
 
                 self, other = (
                     (first, other)
                     if len(first.unit()) < len(second.unit())
                     else (self, second)
@@ -302,22 +299,23 @@
 
     def __radd__(self, other: quantity) -> quantity:
         return self.__add__(other)
 
     # Subtraction.
     def __sub__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
+            # Subtraction between pure numbers.
             if self.unit():
                 raise QuantityError(self, quantity(other, ""), "-")
 
             return quantity(self.value - other, "", self.uncertainty)
 
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
-                # Chooses the one to convert.
+                # Chooses the one to convert based on unit length.
                 first = convert(self, other.unit())
                 second = convert(other, self.unit())
 
                 self, other = (
                     (first, other)
                     if len(first.unit()) < len(second.unit())
                     else (self, second)
@@ -329,20 +327,22 @@
         return quantity(
             self.value - other.value,
             self.unit(),
             sqrt(self.uncertainty**2 + other.uncertainty**2),
         )
 
     def __rsub__(self, other: quantity) -> quantity:
-        return self.__sub__(other)
+        return self.__sub__(other) * (-1)
 
     # Multiplication.
     def __mul__(self, other: any) -> any:
         if not isinstance(other, quantity):
-            return quantity(self.value * other, self.unit(), self.uncertainty * other)
+            return quantity(
+                self.value * other, self.unit(), abs(self.uncertainty * other)
+            )
 
         newUnits = self.units.copy()
 
         if self.convertible and other.convertible:
             other = convert(other, self.unit(), partial=True)
 
         for unit in newUnits:
@@ -364,15 +364,17 @@
 
     def __rmul__(self, other: any) -> any:
         return self.__mul__(other)
 
     # Division.
     def __truediv__(self, other: any) -> any:
         if not isinstance(other, quantity):
-            return quantity(self.value / other, self.unit(), self.uncertainty / other)
+            return quantity(
+                self.value / other, self.unit(), abs(self.uncertainty / other)
+            )
 
         newUnits = self.units.copy()
 
         if self.convertible and other.convertible:
             other = convert(other, self.unit(), partial=True)
 
         for unit in newUnits:
@@ -390,16 +392,16 @@
                 (self.uncertainty / other.value) ** 2
                 + (self.value * other.uncertainty / (other.value**2)) ** 2
             ),
         )
 
     def __floordiv__(self, other: any) -> quantity:
         return quantity(
-            self.value // other, self.unit(), self.uncertainty // other
-        )  # Check uncertainty.
+            self.value // other, self.unit(), abs(self.uncertainty // other)
+        )
 
     def __rtruediv__(self, other: any) -> any:
         return self**-1 * other
 
     # Power.
     def __pow__(self, other: any) -> quantity:
         if isinstance(other, quantity):
@@ -420,19 +422,30 @@
             self.value**other,
             unitFromDict(newUnits),
             abs(other) * (self.value ** (other - 1)) * self.uncertainty,
         )
 
     def __rpow__(self, other: any) -> quantity:
         if isinstance(other, quantity):
-            raise QuantityError(self, other, "**")
+            raise QuantityError(other, self, "**")
+
+        if uAny(other <= 0):
+            raise ValueError(
+                "math domain error\nraised on '{}' ** '{}'".format(other, self)
+            )
+
+        return quantity(
+            other**self.value,
+            "",
+            abs(log(other) * (other**self.value) * self.uncertainty),
+        ) * (other != 1) + self * (other == 1)
 
     # Modulo.
-    # def __mod__(self, other: any) -> quantity:
-    #     return quantity(self.value % other, self.unit())
+    def __mod__(self, other: any) -> quantity:
+        return quantity(self.value % other, self.unit(), self.uncertainty % other)
 
     # COMPARISONS.
 
     # Less than.
     def __lt__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value < other
@@ -440,15 +453,17 @@
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, "<")
 
-        if uAny(self.uncertainty) or uAny(self.uncertainty):
+        if (
+            uAny(self.uncertainty) or uAny(self.uncertainty)
+        ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "<")
 
         return self.value < other.value
 
     # Less or equal.
     def __le__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
@@ -457,15 +472,17 @@
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, "<=")
 
-        if uAny(self.uncertainty) or uAny(self.uncertainty):
+        if (
+            uAny(self.uncertainty) or uAny(self.uncertainty)
+        ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "<=")
 
         return self.value <= other.value
 
     # Greater than.
     def __gt__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
@@ -474,15 +491,17 @@
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, ">")
 
-        if uAny(self.uncertainty) or uAny(self.uncertainty):
+        if (
+            uAny(self.uncertainty) or uAny(self.uncertainty)
+        ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, ">")
 
         return self.value > other.value
 
     # Greater or equal.
     def __ge__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
@@ -491,35 +510,41 @@
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, ">=")
 
-        if uAny(self.uncertainty) or uAny(self.uncertainty):
+        if (
+            uAny(self.uncertainty) or uAny(self.uncertainty)
+        ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, ">=")
 
         return self.value >= other.value
 
     # Equal.
     def __eq__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value == other
 
-        if uAny(self.uncertainty) or uAny(self.uncertainty):
+        if (
+            uAny(self.uncertainty) or uAny(self.uncertainty)
+        ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "==")
 
         return self.value == other.value and self.unit() == other.unit()
 
     # Not equal.
     def __ne__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value != other
 
-        if uAny(self.uncertainty) or uAny(self.uncertainty):
+        if (
+            uAny(self.uncertainty) or uAny(self.uncertainty)
+        ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "!=")
 
         return self.value != other.value or self.unit() != other.unit()
 
 
 # CONVERSION, UNPACKING AND PACKING
```

### Comparing `misura-1.5.1/src/misura/tables.py` & `misura-1.5.2/src/misura/tables.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/src/misura/utilities.py` & `misura-1.5.2/src/misura/utilities.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/tests/tests.py` & `misura-1.5.2/src/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Test suite for misura.
 
-from misura import quantity, convert, unpack, pack
-from misura import addUnit
+from misura.quantities import quantity, convert, unpack, pack
+from misura.tables import addUnit
 
 addUnit("bananas", {"bnn": 1, "dabnn": 10, "hbnn": 100, "kbnn": 1000})
 
 num0 = quantity(5, "m2")
 num1 = quantity(67, "km")
 num2 = quantity(12, "A s")
 num3 = quantity(1, "C mW")
@@ -15,17 +15,20 @@
 num7 = quantity(3, "kg km2")
 num8 = quantity(13, "J")
 num9 = quantity(0.9, "mN km")
 num10 = quantity(3, "N m T")
 num11 = quantity(12, "kbnn")
 num12 = quantity(2, "kg", 0.5)
 num13 = quantity(0.7, "m3", 0.15)
+num14 = quantity(3, "", 1)
 
 # Math.
 print(num0**0.5)
+print(7 - num14)
+print(2 ** num14)
 
 # Logical.
 print(num0 > 10)
 print(num0**0.5 < num1)
 print(num0 < 0.02 * num1**2)
 print(num1 == num2)
 print(num1 != num2)
```

### Comparing `misura-1.5.1/LICENSE` & `misura-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.5.1/README.md` & `misura-1.5.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # misura
 
 ```python
->>> from misura import quantity
+>>> from misura.quantities import quantity
 >>> quantity(7, "m", 1.5) / quantity(2, "s")
 3.5 ± 0.75 m / s
 ```
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
 **misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
@@ -51,15 +51,15 @@
 
 ```
 python -m misura
 ```
 
 you'll be able to verify the installation of **misura** along getting some informations about the library and on the available units of measure[^1]:
 
-[^1]: Examle referring to version 1.3.1
+[^1]: Example referring to version 1.3.1
 
 ```
 misura v1.3.1
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
 Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
@@ -110,20 +110,20 @@
 ```
 import misura
 ```
 
 ## Examples
 
 These are some examples of operations between quantities.  
-Note that, by enabling `misura.style.unitHighlighting`, **misura** uses colorama to highlight units of measure. by disabling it, the output is in the form of `num [unit]`
+Note that, by enabling `globals.style.unitHighlighting`, **misura** uses colorama to highlight units of measure. by disabling it, the output is in the form of `num [unit]`
 
 ### Mathematical operations
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4, "m s-1")
 num3 = quantity(2, "s", .5)
 
 print(num1 + num2)
 print((num1 + num2).dimesion())
@@ -141,15 +141,15 @@
 1.0 ± 0.25 m / s(2)
 4 ± 2.0 s(2)
 ```
 
 ### Working with other libraries
 
 ```python
-from misura import quantity, convert
+from misura.quantities import quantity, convert
 from decimal import Decimal, getcontext
 import numpy
 
 getcontext().prec = 40
 
 arr1 = numpy.array([quantity(2, "m"), quantity(50, "m s-1"), quantity(2, "kg")])
 arr2 = quantity(numpy.array([1, 2, 3]), "J")
@@ -169,15 +169,16 @@
 ```
 
 Unit highlighting helps distinguish between different numbers.
 
 ### User defined units of measure
 
 ```python
-from misura import quantity, convert, addUnit
+from misura.quantities import quantity, convert
+from misura.tables import addUnit
 
 addUnit("volume", {"L": 1, "daL": 10, "hL": 100, "kL": 1000, "dL": 0.1, "cL": 0.01, "mL": 0.001}, "dm3")
 
 num1 = quantity(3, "L")
 
 print(convert(num1, "cm3"))
 ```
@@ -187,15 +188,15 @@
 ```
 3000.0 cm(3)
 ```
 
 ### Manual and automatic conversion
 
 ```python
-from misura import quantity, convert
+from misura.quantities import quantity, convert
 
 num1 = quantity(2, "m2")
 num2 = quantity(4, "kg")
 num3 = quantity(400, "m s-1")
 
 print(convert(num1, "cm2"))
 print(num2 + quantity(5, "g"))
@@ -209,15 +210,15 @@
 4.005 kg
 0.4 km / s
 ```
 
 ### Unpack derived quantities
 
 ```python
-from misura import quantity, unpack
+from misura.quantities import quantity, unpack
 
 num1 = quantity(2, "J2")
 num2 = quantity(4, "C H")
 
 print(unpack(num1))
 print(unpack(num2, "H"))
 ```
@@ -228,15 +229,15 @@
 2.0 kg(2) m(4) / s(4)
 4.0 C kg m(2) / A(2) s(2)
 ```
 
 ### Pack derived quantities
 
 ```python
-from misura import quantity, pack
+from misura.quantities import quantity, pack
 
 num1 = quantity(3, "N m T")
 num2 = quantity(45, "A2 s2")
 
 print(pack(num1, "J", ignore="T"))
 print(pack(num2, "C", full=True))
 ```
@@ -247,15 +248,15 @@
 3.0 J T
 45.0 C(2)
 ```
 
 ### Comparisons
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4, "m s-1")
 num3 = quantity(2, "s")
 
 print(num1 > num2)
 print(num2 < 6)
@@ -271,16 +272,16 @@
 misura.conversion.ConversionError: cannot convert from 's' to 'm s-1'
 raised by: '2 s' -> 'm s-1'
 ```
 
 ### Unary operators and functions
 
 ```python
-from misura import quantity
-from misura import style
+from misura.quantities import quantity
+from misura.globals import style
 from math import trunc
 
 style.quantityHighlighting = False
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4.5, "m s-1")
 num3 = quantity(-2, "s")
@@ -297,15 +298,15 @@
 4 [m / s]
 2 [s]
 ```
 
 ### Formatting
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 
 num1 = quantity(2000, "m s-1")
 
 print("Exponential notation: {:.2e}".format(num1))
 ```
 
 The output is:
```

### Comparing `misura-1.5.1/pyproject.toml` & `misura-1.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `misura-1.5.1/PKG-INFO` & `misura-1.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # misura
 
 ```python
->>> from misura import quantity
+>>> from misura.quantities import quantity
 >>> quantity(7, "m", 1.5) / quantity(2, "s")
 3.5 ± 0.75 m / s
 ```
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
 **misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
@@ -68,15 +68,15 @@
 
 ```
 python -m misura
 ```
 
 you'll be able to verify the installation of **misura** along getting some informations about the library and on the available units of measure[^1]:
 
-[^1]: Examle referring to version 1.3.1
+[^1]: Example referring to version 1.3.1
 
 ```
 misura v1.3.1
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
 Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
@@ -127,20 +127,20 @@
 ```
 import misura
 ```
 
 ## Examples
 
 These are some examples of operations between quantities.  
-Note that, by enabling `misura.style.unitHighlighting`, **misura** uses colorama to highlight units of measure. by disabling it, the output is in the form of `num [unit]`
+Note that, by enabling `globals.style.unitHighlighting`, **misura** uses colorama to highlight units of measure. by disabling it, the output is in the form of `num [unit]`
 
 ### Mathematical operations
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4, "m s-1")
 num3 = quantity(2, "s", .5)
 
 print(num1 + num2)
 print((num1 + num2).dimesion())
@@ -158,15 +158,15 @@
 1.0 ± 0.25 m / s(2)
 4 ± 2.0 s(2)
 ```
 
 ### Working with other libraries
 
 ```python
-from misura import quantity, convert
+from misura.quantities import quantity, convert
 from decimal import Decimal, getcontext
 import numpy
 
 getcontext().prec = 40
 
 arr1 = numpy.array([quantity(2, "m"), quantity(50, "m s-1"), quantity(2, "kg")])
 arr2 = quantity(numpy.array([1, 2, 3]), "J")
@@ -186,15 +186,16 @@
 ```
 
 Unit highlighting helps distinguish between different numbers.
 
 ### User defined units of measure
 
 ```python
-from misura import quantity, convert, addUnit
+from misura.quantities import quantity, convert
+from misura.tables import addUnit
 
 addUnit("volume", {"L": 1, "daL": 10, "hL": 100, "kL": 1000, "dL": 0.1, "cL": 0.01, "mL": 0.001}, "dm3")
 
 num1 = quantity(3, "L")
 
 print(convert(num1, "cm3"))
 ```
@@ -204,15 +205,15 @@
 ```
 3000.0 cm(3)
 ```
 
 ### Manual and automatic conversion
 
 ```python
-from misura import quantity, convert
+from misura.quantities import quantity, convert
 
 num1 = quantity(2, "m2")
 num2 = quantity(4, "kg")
 num3 = quantity(400, "m s-1")
 
 print(convert(num1, "cm2"))
 print(num2 + quantity(5, "g"))
@@ -226,15 +227,15 @@
 4.005 kg
 0.4 km / s
 ```
 
 ### Unpack derived quantities
 
 ```python
-from misura import quantity, unpack
+from misura.quantities import quantity, unpack
 
 num1 = quantity(2, "J2")
 num2 = quantity(4, "C H")
 
 print(unpack(num1))
 print(unpack(num2, "H"))
 ```
@@ -245,15 +246,15 @@
 2.0 kg(2) m(4) / s(4)
 4.0 C kg m(2) / A(2) s(2)
 ```
 
 ### Pack derived quantities
 
 ```python
-from misura import quantity, pack
+from misura.quantities import quantity, pack
 
 num1 = quantity(3, "N m T")
 num2 = quantity(45, "A2 s2")
 
 print(pack(num1, "J", ignore="T"))
 print(pack(num2, "C", full=True))
 ```
@@ -264,15 +265,15 @@
 3.0 J T
 45.0 C(2)
 ```
 
 ### Comparisons
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4, "m s-1")
 num3 = quantity(2, "s")
 
 print(num1 > num2)
 print(num2 < 6)
@@ -288,16 +289,16 @@
 misura.conversion.ConversionError: cannot convert from 's' to 'm s-1'
 raised by: '2 s' -> 'm s-1'
 ```
 
 ### Unary operators and functions
 
 ```python
-from misura import quantity
-from misura import style
+from misura.quantities import quantity
+from misura.globals import style
 from math import trunc
 
 style.quantityHighlighting = False
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4.5, "m s-1")
 num3 = quantity(-2, "s")
@@ -314,15 +315,15 @@
 4 [m / s]
 2 [s]
 ```
 
 ### Formatting
 
 ```python
-from misura import quantity
+from misura.quantities import quantity
 
 num1 = quantity(2000, "m s-1")
 
 print("Exponential notation: {:.2e}".format(num1))
 ```
 
 The output is:
```

