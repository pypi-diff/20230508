# Comparing `tmp/tariochbctools-0.8.0.tar.gz` & `tmp/tariochbctools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpc0afggxs/tmp8wzj5gb4/tariochbctools-0.8.0.tar", last modified: Tue Jul  7 20:08:40 2020, max compression
+gzip compressed data, was "/tmp/tmp0nyub0p0/tmpnuga9oeb/tariochbctools-0.9.0.tar", last modified: Fri Jul 17 12:26:43 2020, max compression
```

## Comparing `tariochbctools-0.8.0.tar` & `tariochbctools-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6699 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4476 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       90 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      647 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/
--rw-r--r--   0 runner    (1001) docker     (116)      363 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/bitst/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/bitst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4820 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/bitst/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/general/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1929 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/general/mt940importer.py
--rw-r--r--   0 runner    (1001) docker     (116)      567 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/general/priceLookup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/ibkr/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/ibkr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5736 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/ibkr/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/revolut/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/revolut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2318 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/revolut/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/schedule/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1601 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/schedule/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/stocks/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/stocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3534 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/stocks/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/transferwise/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/transferwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2612 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/transferwise/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/truelayer/
--rw-r--r--   0 runner    (1001) docker     (116)     3467 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/truelayer/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/zak/
--rw-r--r--   0 runner    (1001) docker     (116)     3035 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/zak/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/importers/zkb/
--rw-r--r--   0 runner    (1001) docker     (116)     1414 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/importers/zkb/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/generate_base_ccy_prices.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/prices/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1058 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/prices/alphavantage.py
--rw-r--r--   0 runner    (1001) docker     (116)     1130 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/prices/alphavantagefx.py
--rw-r--r--   0 runner    (1001) docker     (116)      649 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/prices/bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1059 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/src/tariochbctools/plugins/prices/exchangeratesapi.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6699 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-07 20:08:35.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      101 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/src/tariochbctools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/tests/tariochbctools/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-07 20:08:40.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/
--rw-r--r--   0 runner    (1001) docker     (116)      189 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/entry_already_exists_expected.beancount
--rw-r--r--   0 runner    (1001) docker     (116)      252 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/entry_already_exists_input.beancount
--rw-r--r--   0 runner    (1001) docker     (116)       63 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/missing_fx_expected.beancount
--rw-r--r--   0 runner    (1001) docker     (116)      120 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/missing_fx_input.beancount
--rw-r--r--   0 runner    (1001) docker     (116)      189 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/normal_expected.beancount
--rw-r--r--   0 runner    (1001) docker     (116)      179 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/normal_input.beancount
--rw-r--r--   0 runner    (1001) docker     (116)     1012 2020-07-07 20:08:00.000000 tariochbctools-0.8.0/tests/tariochbctools/plugins/test_generate_base_ccy_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     1074 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     7207 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4888 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       90 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      647 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/
+-rw-r--r--   0 runner    (1001) docker     (116)      363 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/bitst/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/bitst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4820 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/bitst/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/general/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1929 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/general/mt940importer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      567 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/general/priceLookup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/ibkr/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/ibkr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5731 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/ibkr/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/revolut/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/revolut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2318 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/revolut/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/schedule/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1601 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/schedule/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/stocks/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/stocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3534 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/stocks/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/transferwise/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/transferwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2612 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/transferwise/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/truelayer/
+-rw-r--r--   0 runner    (1001) docker     (116)     3467 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/truelayer/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/zak/
+-rw-r--r--   0 runner    (1001) docker     (116)     3035 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/zak/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/importers/zkb/
+-rw-r--r--   0 runner    (1001) docker     (116)     1414 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/importers/zkb/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1167 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/generate_base_ccy_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1058 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/alphavantage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1130 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/alphavantagefx.py
+-rw-r--r--   0 runner    (1001) docker     (116)      649 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/bitstamp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1059 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/exchangeratesapi.py
+-rw-r--r--   0 runner    (1001) docker     (116)      920 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/src/tariochbctools/plugins/prices/ibkr.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     7207 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2345 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-17 12:26:37.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      101 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/src/tariochbctools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/tests/tariochbctools/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 12:26:43.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/
+-rw-r--r--   0 runner    (1001) docker     (116)      189 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/entry_already_exists_expected.beancount
+-rw-r--r--   0 runner    (1001) docker     (116)      252 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/entry_already_exists_input.beancount
+-rw-r--r--   0 runner    (1001) docker     (116)       63 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/missing_fx_expected.beancount
+-rw-r--r--   0 runner    (1001) docker     (116)      120 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/missing_fx_input.beancount
+-rw-r--r--   0 runner    (1001) docker     (116)      189 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/normal_expected.beancount
+-rw-r--r--   0 runner    (1001) docker     (116)      179 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/data/generate_base_ccy_prices/normal_input.beancount
+-rw-r--r--   0 runner    (1001) docker     (116)     1012 2020-07-17 12:26:10.000000 tariochbctools-0.9.0/tests/tariochbctools/plugins/test_generate_base_ccy_prices.py
```

### Comparing `tariochbctools-0.8.0/LICENSE` & `tariochbctools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/PKG-INFO` & `tariochbctools-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tariochbctools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Importers, plugins and price fetchers for Beancount
 Home-page: https://github.com/tarioch/beancounttools/
 Author: Patrick Ruckstuhl
 Author-email: patrick@ch.tario.org
 License: MIT
 Description: .. image:: https://img.shields.io/pypi/l/tariochbctools.svg
            :target: https://pypi.python.org/pypi/tariochbctools
@@ -65,14 +65,26 @@
         Fetches prices from `exchangeratesapi.io <https://exchangeratesapi.io//>`_
         
         ::
         
           2019-01-01 commodity EUR
             price: "CHF:tariochbctools.plugins.prices.exchangeratesapi/EUR"
         
+        **interactivebrokers**
+        
+        Fetches prices from `interactivebrokers <https://www.interactivebrokers.com/>`_
+        Only works if you have open positions with the symbols.
+        Requires the environment variables ``IBKR_TOKEN`` to be set with your flex query token and ``IBKR_QUERY_ID``
+        with a flex query that contains the open positions.
+        
+        ::
+        
+          2019-01-01 commodity VWRL
+            price: "CHF:tariochbctools.plugins.prices.ibkr/VWRL"
+        
         
         importers
         ---------
         **bitstamp**
         
         Import transactions from `Bitstamp <https://www.bitstamp.com/>`_
```

### Comparing `tariochbctools-0.8.0/README.rst` & `tariochbctools-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,26 @@
 Fetches prices from `exchangeratesapi.io <https://exchangeratesapi.io//>`_
 
 ::
 
   2019-01-01 commodity EUR
     price: "CHF:tariochbctools.plugins.prices.exchangeratesapi/EUR"
 
+**interactivebrokers**
+
+Fetches prices from `interactivebrokers <https://www.interactivebrokers.com/>`_
+Only works if you have open positions with the symbols.
+Requires the environment variables ``IBKR_TOKEN`` to be set with your flex query token and ``IBKR_QUERY_ID``
+with a flex query that contains the open positions.
+
+::
+
+  2019-01-01 commodity VWRL
+    price: "CHF:tariochbctools.plugins.prices.ibkr/VWRL"
+
 
 importers
 ---------
 **bitstamp**
 
 Import transactions from `Bitstamp <https://www.bitstamp.com/>`_
```

### Comparing `tariochbctools-0.8.0/setup.cfg` & `tariochbctools-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/setup.py` & `tariochbctools-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/bitst/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/bitst/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/general/mt940importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/general/mt940importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/general/priceLookup.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/general/priceLookup.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/ibkr/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/ibkr/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     'description': trx.description,
                     'type': trx.type
                 })
 
         result = []
         for trx in transactions:
             if trx['type'] == CashAction.DIVIDEND:
-                asset = trx['symbol'].replace('z', '')
+                asset = trx['symbol'].rstrip('z')
                 payDate = trx['date'].date()
                 totalDividend = trx['amount']
                 totalWithholding = -trx['whAmount']
                 totalPayout = totalDividend - totalWithholding
                 currency = trx['currency']
 
                 _, rows = query.run_query(
```

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/revolut/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/revolut/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/schedule/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/schedule/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/stocks/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/stocks/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/transferwise/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/transferwise/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/truelayer/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/truelayer/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/zak/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/zak/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/importers/zkb/importer.py` & `tariochbctools-0.9.0/src/tariochbctools/importers/zkb/importer.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/plugins/generate_base_ccy_prices.py` & `tariochbctools-0.9.0/src/tariochbctools/plugins/generate_base_ccy_prices.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/plugins/prices/alphavantage.py` & `tariochbctools-0.9.0/src/tariochbctools/plugins/prices/alphavantage.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/plugins/prices/alphavantagefx.py` & `tariochbctools-0.9.0/src/tariochbctools/plugins/prices/alphavantagefx.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/plugins/prices/bitstamp.py` & `tariochbctools-0.9.0/src/tariochbctools/plugins/prices/bitstamp.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools/plugins/prices/exchangeratesapi.py` & `tariochbctools-0.9.0/src/tariochbctools/plugins/prices/exchangeratesapi.py`

 * *Files identical despite different names*

### Comparing `tariochbctools-0.8.0/src/tariochbctools.egg-info/PKG-INFO` & `tariochbctools-0.9.0/src/tariochbctools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tariochbctools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Importers, plugins and price fetchers for Beancount
 Home-page: https://github.com/tarioch/beancounttools/
 Author: Patrick Ruckstuhl
 Author-email: patrick@ch.tario.org
 License: MIT
 Description: .. image:: https://img.shields.io/pypi/l/tariochbctools.svg
            :target: https://pypi.python.org/pypi/tariochbctools
@@ -65,14 +65,26 @@
         Fetches prices from `exchangeratesapi.io <https://exchangeratesapi.io//>`_
         
         ::
         
           2019-01-01 commodity EUR
             price: "CHF:tariochbctools.plugins.prices.exchangeratesapi/EUR"
         
+        **interactivebrokers**
+        
+        Fetches prices from `interactivebrokers <https://www.interactivebrokers.com/>`_
+        Only works if you have open positions with the symbols.
+        Requires the environment variables ``IBKR_TOKEN`` to be set with your flex query token and ``IBKR_QUERY_ID``
+        with a flex query that contains the open positions.
+        
+        ::
+        
+          2019-01-01 commodity VWRL
+            price: "CHF:tariochbctools.plugins.prices.ibkr/VWRL"
+        
         
         importers
         ---------
         **bitstamp**
         
         Import transactions from `Bitstamp <https://www.bitstamp.com/>`_
```

### Comparing `tariochbctools-0.8.0/src/tariochbctools.egg-info/SOURCES.txt` & `tariochbctools-0.9.0/src/tariochbctools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/tariochbctools/plugins/__init__.py
 src/tariochbctools/plugins/generate_base_ccy_prices.py
 src/tariochbctools/plugins/prices/__init__.py
 src/tariochbctools/plugins/prices/alphavantage.py
 src/tariochbctools/plugins/prices/alphavantagefx.py
 src/tariochbctools/plugins/prices/bitstamp.py
 src/tariochbctools/plugins/prices/exchangeratesapi.py
+src/tariochbctools/plugins/prices/ibkr.py
 tests/__init__.py
 tests/tariochbctools/__init__.py
 tests/tariochbctools/plugins/__init__.py
 tests/tariochbctools/plugins/test_generate_base_ccy_prices.py
 tests/tariochbctools/plugins/data/generate_base_ccy_prices/entry_already_exists_expected.beancount
 tests/tariochbctools/plugins/data/generate_base_ccy_prices/entry_already_exists_input.beancount
 tests/tariochbctools/plugins/data/generate_base_ccy_prices/missing_fx_expected.beancount
```

### Comparing `tariochbctools-0.8.0/tests/tariochbctools/plugins/test_generate_base_ccy_prices.py` & `tariochbctools-0.9.0/tests/tariochbctools/plugins/test_generate_base_ccy_prices.py`

 * *Files identical despite different names*

