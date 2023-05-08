# Comparing `tmp/pybet-0.6.1.tar.gz` & `tmp/pybet-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybet-0.6.1.tar", max compression
+gzip compressed data, was "pybet-0.6.2.tar", max compression
```

## Comparing `pybet-0.6.1.tar` & `pybet-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.6.1/LICENSE
--rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.6.1/pybet/__init__.py
--rw-r--r--   0        0        0     8054 2023-05-04 23:05:01.296759 pybet-0.6.1/pybet/market.py
--rw-r--r--   0        0        0    11292 2023-02-18 00:28:56.233330 pybet-0.6.1/pybet/odds.py
--rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.6.1/pybet/staking/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-29 12:08:45.277280 pybet-0.6.1/pybet/staking/kelly.py
--rw-r--r--   0        0        0      936 2023-05-04 23:14:29.139911 pybet-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.6.1/README.md
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.6.2/LICENSE
+-rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.6.2/pybet/__init__.py
+-rw-r--r--   0        0        0     8054 2023-05-04 23:05:01.296759 pybet-0.6.2/pybet/market.py
+-rw-r--r--   0        0        0    11717 2023-05-08 20:37:50.564904 pybet-0.6.2/pybet/odds.py
+-rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.6.2/pybet/staking/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-29 12:08:45.277280 pybet-0.6.2/pybet/staking/kelly.py
+-rw-r--r--   0        0        0      989 2023-05-08 20:40:41.727261 pybet-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.6.2/README.md
+-rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.6.2/PKG-INFO
```

### Comparing `pybet-0.6.1/LICENSE` & `pybet-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybet-0.6.1/pybet/market.py` & `pybet-0.6.2/pybet/market.py`

 * *Files identical despite different names*

### Comparing `pybet-0.6.1/pybet/odds.py` & `pybet-0.6.2/pybet/odds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from decimal import Decimal
 from fractions import Fraction
+from math import inf
 from typing import overload, List, Tuple, Union
 
 
 class FractionalOddsSets:
     """Constant lists of fractional odds for use in Odds instances to determine the proximate fractional odds to any particular value"""
 
     STANDARD = (
@@ -134,18 +135,18 @@
         :rtype: Odds
 
         :Example:
             >>> Odds.percentage(40)
             Decimal('2.5')
         """
 
-        if not 0 < value < 100:
+        if not 0 <= value <= 100:
             raise ValueError("Percentage must be between 0 and 100")
 
-        return cls(100 / value)
+        return cls(100 / value) if value > 0 else cls(inf)
 
     @classmethod
     def probability(cls, value: Decimal) -> Odds:
         """Creates an Odds instance from an equivalent probability > 0 and < 1
 
         :param value: A representation of the odds as a probability
         :type value: Decimal
@@ -154,21 +155,34 @@
         :rtype: Odds
 
         :Example:
             >>> Odds.probability(0.4)
             Decimal('2.5')
         """
 
-        if not 0 < value < 1:
+        if not 0 <= value <= 1:
             raise ValueError("Probability must be between 0 and 1")
 
-        return cls(1 / value)
+        return cls(1 / value) if value > 0 else cls(inf)
 
     # Dunder methods
 
+    def __repr__(self) -> str:
+        """A string representation of the odds as a decimal to two decimal places
+
+        :return: The odds to two decimal places
+        :rtype: str
+
+        :Example:
+            >>> repr(Odds(3.25))
+            Odds('3.25')
+        """
+
+        return f"{self.__class__.__name__}('{str(self)}')"
+
     def __str__(self) -> str:
         """A string representation of the odds as a decimal to two decimal places
 
         :return: The odds to two decimal places
         :rtype: str
 
         :Example:
```

### Comparing `pybet-0.6.1/pybet/staking/kelly.py` & `pybet-0.6.2/pybet/staking/kelly.py`

 * *Files identical despite different names*

### Comparing `pybet-0.6.1/pyproject.toml` & `pybet-0.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybet"
-version = "0.6.1"
+version = "0.6.2"
 description = "A library of betting utilities to assist with calculation of bets, stakes and markets"
 license = "GPL-3.0-only"
 authors = ["Robert Peacock <robertjamespeacock@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/peaky76/pybet"
 documentation = "https://pybet.readthedocs.io/"
 keywords = ["betting", "gambling"]
@@ -17,17 +17,21 @@
 [tool.poetry.dependencies]
 python = "^3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 auto-changelog = "^0.6.0"
 black = "^23.1.0"
 coverage = "^7.1.0"
-sphinx = "^6.1.3"
-sphinx-rtd-theme = "^1.2.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.265"
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+
+[tool.ruff]
+ignore = ["E501"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pybet-0.6.1/README.md` & `pybet-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pybet-0.6.1/PKG-INFO` & `pybet-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybet
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library of betting utilities to assist with calculation of bets, stakes and markets
 Home-page: https://github.com/peaky76/pybet
 License: GPL-3.0-only
 Keywords: betting,gambling
 Author: Robert Peacock
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

