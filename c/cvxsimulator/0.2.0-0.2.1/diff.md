# Comparing `tmp/cvxsimulator-0.2.0.tar.gz` & `tmp/cvxsimulator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.2.0.tar", max compression
+gzip compressed data, was "cvxsimulator-0.2.1.tar", max compression
```

## Comparing `cvxsimulator-0.2.0.tar` & `cvxsimulator-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1102 2023-05-07 03:49:46.163568 cvxsimulator-0.2.0/LICENSE
--rw-r--r--   0        0        0     4473 2023-05-07 03:49:46.163568 cvxsimulator-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1520 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/month.py
--rw-r--r--   0        0        0     5814 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      541 2023-05-07 03:50:40.831761 cvxsimulator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 cvxsimulator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-08 20:13:39.782319 cvxsimulator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4050 2023-05-08 20:13:39.782319 cvxsimulator-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1409 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/month.py
+-rw-r--r--   0        0        0     5814 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      596 2023-05-08 20:14:34.870395 cvxsimulator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 cvxsimulator-0.2.1/PKG-INFO
```

### Comparing `cvxsimulator-0.2.0/LICENSE` & `cvxsimulator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.0/README.md` & `cvxsimulator-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
-[![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
-[![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
-[![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
@@ -25,18 +22,20 @@
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
 ### Create the portfolio object
 
 The user defines a portfolio object by loading a frame of prices and initialize the initial amount of cash used in our experiment:
 
 ```python
+from pathlib import Path
+
 import pandas as pd
 from cvx.simulator.portfolio import build_portfolio
 
-prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill(
+prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 portfolio = build_portfolio(prices=prices, initial_cash=1e6)
 ```
 
 It is also possible to specify a model for trading costs.
 
 ### Loop through time
```

### Comparing `cvxsimulator-0.2.0/cvx/simulator/metrics.py` & `cvxsimulator-0.2.1/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.0/cvx/simulator/month.py` & `cvxsimulator-0.2.1/cvx/simulator/month.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 def monthlytable(returns: pd.Series):
     """
     Get a table of monthly returns.
 
     Args:
         returns: Series of individual returns.
-        fct: Function to use for total return calculation.
-            If not given, compounded logic is used.
 
     Returns:
         DataFrame with monthly returns, their STDev and YTD.
     """
 
     def _compound(rets):
         """
```

### Comparing `cvxsimulator-0.2.0/cvx/simulator/portfolio.py` & `cvxsimulator-0.2.1/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.0/pyproject.toml` & `cvxsimulator-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.2.0"
+version = "v0.2.1"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.2"
-pandas = "*"
+pandas = "<2.0.0"   # unfortunately otherwise crash with quantstats
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.3"
 pytest-cov = "3.0.0"
 yfinance = "*"
 quantstats = "*"
 plotly = "*"
```

### Comparing `cvxsimulator-0.2.0/PKG-INFO` & `cvxsimulator-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas
+Requires-Dist: pandas (<2.0.0)
 Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
-[![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
-[![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
-[![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
@@ -41,18 +38,20 @@
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
 ### Create the portfolio object
 
 The user defines a portfolio object by loading a frame of prices and initialize the initial amount of cash used in our experiment:
 
 ```python
+from pathlib import Path
+
 import pandas as pd
 from cvx.simulator.portfolio import build_portfolio
 
-prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill(
+prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 portfolio = build_portfolio(prices=prices, initial_cash=1e6)
 ```
 
 It is also possible to specify a model for trading costs.
 
 ### Loop through time
```

