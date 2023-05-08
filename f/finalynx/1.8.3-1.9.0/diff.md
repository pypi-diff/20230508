# Comparing `tmp/finalynx-1.8.3.tar.gz` & `tmp/finalynx-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalynx-1.8.3.tar", max compression
+gzip compressed data, was "finalynx-1.9.0.tar", max compression
```

## Comparing `finalynx-1.8.3.tar` & `finalynx-1.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    35149 2023-04-24 08:19:00.351602 finalynx-1.8.3/LICENSE
--rw-r--r--   0        0        0     6890 2023-04-24 08:19:00.351602 finalynx-1.8.3/README.md
--rw-r--r--   0        0        0     1345 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/__init__.py
--rw-r--r--   0        0        0      770 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/__main__.py
--rw-r--r--   0        0        0      662 2023-04-24 08:19:01.599645 finalynx-1.8.3/finalynx/__meta__.py
--rw-r--r--   0        0        0      993 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/analyzer.py
--rw-r--r--   0        0        0     3187 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/asset_class.py
--rw-r--r--   0        0        0     2398 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/envelopes.py
--rw-r--r--   0        0        0     2858 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/investment_state.py
--rw-r--r--   0        0        0     8096 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/assistant.py
--rw-r--r--   0        0        0      273 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/console.py
--rw-r--r--   0        0        0      424 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/copilot/__init__.py
--rw-r--r--   0        0        0      593 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/copilot/copilot.py
--rw-r--r--   0        0        0      427 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/dashboard/__init__.py
--rw-r--r--   0        0        0    11713 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/dashboard/dashboard.py
--rw-r--r--   0        0        0      891 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/fetch/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/fetch/fetch.py
--rw-r--r--   0        0        0    16256 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/fetch/fetch_finary.py
--rw-r--r--   0        0        0       47 2023-04-24 08:19:00.715614 finalynx-1.8.3/finalynx/finary_api/.git
--rw-r--r--   0        0        0      222 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/.github/dependabot.yml
--rw-r--r--   0        0        0     1905 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/.gitignore
--rw-r--r--   0        0        0     1064 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/LICENSE
--rw-r--r--   0        0        0     5099 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/README.md
--rwxr-xr-x   0        0        0      170 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/check.sh
--rw-r--r--   0        0        0       32 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/credentials.json.tpl
--rw-r--r--   0        0        0      691 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/__init__.py
--rw-r--r--   0        0        0    15625 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/__main__.py
--rw-r--r--   0        0        0      323 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/auth.py
--rw-r--r--   0        0        0      694 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/bank_account_types.py
--rw-r--r--   0        0        0      118 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/constants.py
--rw-r--r--   0        0        0      241 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/crypto_chains.py
--rw-r--r--   0        0        0      824 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/currencies.py
--rw-r--r--   0        0        0      308 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/institutions.py
--rw-r--r--   0        0        0      511 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/precious_metals.py
--rw-r--r--   0        0        0      494 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/scpis.py
--rw-r--r--   0        0        0     3276 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/securities.py
--rw-r--r--   0        0        0     2308 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/signin.py
--rw-r--r--   0        0        0     4177 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_cryptos.py
--rw-r--r--   0        0        0      246 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_me.py
--rw-r--r--   0        0        0     1670 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_portfolio.py
--rw-r--r--   0        0        0     1865 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_precious_metals.py
--rw-r--r--   0        0        0      222 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_real_estates.py
--rw-r--r--   0        0        0      208 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_scpis.py
--rw-r--r--   0        0        0     5680 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_securities.py
--rw-r--r--   0        0        0      221 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_startups.py
--rw-r--r--   0        0        0      196 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/utils.py
--rw-r--r--   0        0        0     3253 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/views.py
--rw-r--r--   0        0        0      478 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/mypy.ini
--rw-r--r--   0        0        0      195 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/requirements-tests.txt
--rw-r--r--   0        0        0       60 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/requirements.txt
--rw-r--r--   0        0        0      224 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/setup.cfg
--rw-r--r--   0        0        0       50 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/tests/data/cryptos.csv
--rw-r--r--   0        0        0      172 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/tests/data/stocks.csv
--rw-r--r--   0        0        0      340 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/tests/data/stocks.json
--rw-r--r--   0        0        0      153 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/parse/__init__.py
--rw-r--r--   0        0        0      739 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/parse/json.py
--rw-r--r--   0        0        0     1007 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/parse/parser.py
--rw-r--r--   0        0        0     2016 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/bucket.py
--rw-r--r--   0        0        0      860 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/constants.py
--rw-r--r--   0        0        0     2427 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/envelope.py
--rw-r--r--   0        0        0     7703 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/folder.py
--rw-r--r--   0        0        0      422 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/hierarchy.py
--rw-r--r--   0        0        0     2436 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/line.py
--rw-r--r--   0        0        0     8333 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/node.py
--rw-r--r--   0        0        0     1195 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/portfolio.py
--rw-r--r--   0        0        0     3624 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/render.py
--rw-r--r--   0        0        0    11976 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/targets.py
--rw-r--r--   0        0        0      419 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/simulator/__init__.py
--rw-r--r--   0        0        0     2385 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/simulator/simulator.py
--rw-r--r--   0        0        0     2088 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/usage.py
--rw-r--r--   0        0        0     1713 2023-04-24 08:19:01.599645 finalynx-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 finalynx-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 13:11:23.607092 finalynx-1.9.0/LICENSE
+-rw-r--r--   0        0        0     6890 2023-04-24 13:11:23.607092 finalynx-1.9.0/README.md
+-rw-r--r--   0        0        0     1355 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/__init__.py
+-rw-r--r--   0        0        0      770 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/__main__.py
+-rw-r--r--   0        0        0      662 2023-04-24 13:11:25.107104 finalynx-1.9.0/finalynx/__meta__.py
+-rw-r--r--   0        0        0      993 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/analyzer/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3187 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/analyzer/asset_class.py
+-rw-r--r--   0        0        0     2398 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/analyzer/envelopes.py
+-rw-r--r--   0        0        0     2858 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/analyzer/investment_state.py
+-rw-r--r--   0        0        0     8899 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/assistant.py
+-rw-r--r--   0        0        0      273 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/console.py
+-rw-r--r--   0        0        0      424 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/copilot/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/copilot/copilot.py
+-rw-r--r--   0        0        0      427 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/dashboard/__init__.py
+-rw-r--r--   0        0        0    11713 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/dashboard/dashboard.py
+-rw-r--r--   0        0        0      891 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/fetch/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-24 13:11:23.623093 finalynx-1.9.0/finalynx/fetch/fetch.py
+-rw-r--r--   0        0        0    16256 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/fetch/fetch_finary.py
+-rw-r--r--   0        0        0       47 2023-04-24 13:11:24.179097 finalynx-1.9.0/finalynx/finary_api/.git
+-rw-r--r--   0        0        0      222 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/.github/dependabot.yml
+-rw-r--r--   0        0        0     1905 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/.gitignore
+-rw-r--r--   0        0        0     1064 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/LICENSE
+-rw-r--r--   0        0        0     5099 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/README.md
+-rwxr-xr-x   0        0        0      170 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/check.sh
+-rw-r--r--   0        0        0       32 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/credentials.json.tpl
+-rw-r--r--   0        0        0      691 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/__init__.py
+-rw-r--r--   0        0        0    15625 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/__main__.py
+-rw-r--r--   0        0        0      323 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/auth.py
+-rw-r--r--   0        0        0      694 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/bank_account_types.py
+-rw-r--r--   0        0        0      118 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/constants.py
+-rw-r--r--   0        0        0      241 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/crypto_chains.py
+-rw-r--r--   0        0        0      824 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/currencies.py
+-rw-r--r--   0        0        0      308 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/institutions.py
+-rw-r--r--   0        0        0      511 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/precious_metals.py
+-rw-r--r--   0        0        0      494 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/scpis.py
+-rw-r--r--   0        0        0     3276 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/securities.py
+-rw-r--r--   0        0        0     2308 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/signin.py
+-rw-r--r--   0        0        0     4177 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_cryptos.py
+-rw-r--r--   0        0        0      246 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_holdings_accounts.py
+-rw-r--r--   0        0        0      411 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_me.py
+-rw-r--r--   0        0        0     1670 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_real_estates.py
+-rw-r--r--   0        0        0      208 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_scpis.py
+-rw-r--r--   0        0        0     5680 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_securities.py
+-rw-r--r--   0        0        0      221 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/user_startups.py
+-rw-r--r--   0        0        0      196 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/finary_api/views.py
+-rw-r--r--   0        0        0      478 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/mypy.ini
+-rw-r--r--   0        0        0      195 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/requirements.txt
+-rw-r--r--   0        0        0      224 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/setup.cfg
+-rw-r--r--   0        0        0       50 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/tests/data/cryptos.csv
+-rw-r--r--   0        0        0      172 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/tests/data/stocks.csv
+-rw-r--r--   0        0        0      340 2023-04-24 13:11:24.187097 finalynx-1.9.0/finalynx/finary_api/tests/data/stocks.json
+-rw-r--r--   0        0        0      153 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/parse/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/parse/json.py
+-rw-r--r--   0        0        0     1007 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/parse/parser.py
+-rw-r--r--   0        0        0     2043 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/bucket.py
+-rw-r--r--   0        0        0     1325 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/constants.py
+-rw-r--r--   0        0        0     2427 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/envelope.py
+-rw-r--r--   0        0        0    10276 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/folder.py
+-rw-r--r--   0        0        0      422 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/hierarchy.py
+-rw-r--r--   0        0        0     2705 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/line.py
+-rw-r--r--   0        0        0     9054 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/node.py
+-rw-r--r--   0        0        0     1195 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/portfolio.py
+-rw-r--r--   0        0        0     3624 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/render.py
+-rw-r--r--   0        0        0    11976 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/portfolio/targets.py
+-rw-r--r--   0        0        0      419 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/simulator/__init__.py
+-rw-r--r--   0        0        0     2385 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/simulator/simulator.py
+-rw-r--r--   0        0        0     2298 2023-04-24 13:11:23.627092 finalynx-1.9.0/finalynx/usage.py
+-rw-r--r--   0        0        0     1713 2023-04-24 13:11:25.107104 finalynx-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 finalynx-1.9.0/PKG-INFO
```

### Comparing `finalynx-1.8.3/LICENSE` & `finalynx-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/README.md` & `finalynx-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/__init__.py` & `finalynx-1.9.0/finalynx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .__meta__ import __version__  # noqa: F401
 
 # Add finary_api submodule to path to allow imports to work
 sys.path.append(os.path.join(os.path.dirname(__file__), "finary_api"))
 
 # Portfolio
 from .portfolio import TargetRange, TargetMin, TargetMax, TargetRatio, TargetGlobalRatio
-from .portfolio import Line, Folder, Bucket, SharedFolder, Portfolio, FolderDisplay
+from .portfolio import Line, LinePerf, Folder, Bucket, SharedFolder, Portfolio, FolderDisplay
 from .portfolio import AssetClass, EnvelopeClass
 from .portfolio import Envelope, EnvelopeState, PEA, PEE, AV, PER
 
 # Fetch
 from .fetch import FetchFinary
 
 # Advisor
```

### Comparing `finalynx-1.8.3/finalynx/__main__.py` & `finalynx-1.9.0/finalynx/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/__meta__.py` & `finalynx-1.9.0/finalynx/__meta__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ```{warning}
 Do not manually change this information.
 ```
 
 Metadata information about Finalynx. This file is used by Fynalinx and updated by the CI/CD pipeline.
 """
 
-__version__ = "1.8.3"
+__version__ = "1.9.0"
 
 __author__ = "Pierre Laclau (MadeInPierre)"
 
 __copyright__ = """
 Copyright (c) 2023, MadeInPierre
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
```

### Comparing `finalynx-1.8.3/finalynx/analyzer/__init__.py` & `finalynx-1.9.0/finalynx/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/analyzer/analyzer.py` & `finalynx-1.9.0/finalynx/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/analyzer/asset_class.py` & `finalynx-1.9.0/finalynx/analyzer/asset_class.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/analyzer/envelopes.py` & `finalynx-1.9.0/finalynx/analyzer/envelopes.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/analyzer/investment_state.py` & `finalynx-1.9.0/finalynx/analyzer/investment_state.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/assistant.py` & `finalynx-1.9.0/finalynx/assistant.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,14 +99,18 @@
             self.show_data = True
         if args["dashboard"]:
             self.launch_dashboard = True
         if args["--format"]:
             self.output_format = args["--format"]
         if args["deltas"]:
             self.output_format = "[console_deltas]"
+        if args["perf"]:
+            self.output_format = "[console_perf]"
+        if args["ideal"]:
+            self.output_format = "[console_ideal]"
         if args["targets"]:
             self.output_format = "[console_targets]"
             self.hide_deltas = True
         if args["text"]:
             self.output_format = "[text]"
             self.hide_deltas = True
         if args["--hide-deltas"]:
@@ -129,60 +133,76 @@
         # simulation = self.scenario.rich_simulation(self.portfolio)  # noqa TODO
 
         # Get recommendations for immediate investment operations
         # recommentations = self.copilot.rich_recommendations(self.portfolio)  # noqa TODO
 
         # Items to be rendered as a row
         render = [
+            Text(" "),
             self.portfolio.tree(
                 output_format=self.output_format,
                 hide_root=self.hide_root,
                 hide_amounts=self.hide_amounts,
             ),
         ]
 
         # Display deltas only if not already printed in the main tree
         if not self.hide_deltas and "delta" not in self.output_format:
             render.append(self.portfolio.tree_delta())
 
         # Final set of results to be displayed
         panels: List[ConsoleRenderable] = [
-            Columns([Text("  ")] + render),  # type: ignore
-            Panel(self.render_envelopes(), title="Investments Summary", padding=(1, 2), expand=False),
+            Panel(self.render_envelopes(), title="Delta Investments", padding=(1, 2), expand=False),
+            Panel(self.render_perf(), title="Performance", padding=(1, 2), expand=False),
         ]
 
         # Show the data fetched from Finary if specified
         if self.show_data:
             panels.append(Panel(finary_tree, title="Finary data"))
 
         # Display the entire portfolio and associated recommendations
-        console.print("\n", Columns(panels, padding=(2, 10)), "\n")
+        console.print("\n", Columns(render, padding=(2, 2)), "\n")  # type: ignore
+        console.print(Columns(panels, padding=(2, 2)), "\n")
 
         # Host a local webserver with the running dashboard
         if self.launch_dashboard:
             console.log("Launching dashboard.")
             Dashboard().run(portfolio=self.portfolio)
 
-    def render_envelopes(self) -> Tree:  # TODO missing deltas for folders as lines (e.g. ramify, or)
+    def render_perf(self) -> Tree:
+        """Print the current and ideal global expected performance."""
+        perf = self.portfolio.get_perf(ideal=False).expected
+        perf_ideal = self.portfolio.get_perf(ideal=True).expected
+
+        tree = Tree("Global Performance", hide_root=True)
+        tree.add(f"Current: [bold green]{perf:.1f} %")
+        tree.add(f"Target: [bold green]{perf_ideal:.1f} % ")
+
+        console.log(
+            f"""Your global portfolio's performance is {perf:.1f}%/yr, follow your targets to get {perf_ideal:.1f}%/yr."""
+        )
+        return tree
+
+    def render_envelopes(self) -> Tree:
         """Sort lines with non-zero deltas by envelopes and display them as
         a summary of transfers to make."""
         tree = Tree("Envelopes", hide_root=True)
 
         for env in self.envelopes:
             children, env_delta = [], 0.0
             for line in env.lines:
                 delta = line.get_delta()
                 if delta != 0 and line.target.check() not in [Target.RESULT_NONE, Target.RESULT_OK]:
                     env_delta += delta
-                    children.append(line.render(output_format="[delta] [name]"))
+                    children.append(line.render(output_format="[delta][name]"))
 
             if children:
                 env_delta = round(env_delta)
                 render_delta = f"[{'green' if env_delta > 0 else 'red'}]{'+' if env_delta > 0 else ''}{env_delta} €"
-                node = tree.add(f"{render_delta} [dodger_blue2 bold]{env.name}")
+                node = tree.add(f"{render_delta} [dodger_blue2 bold]{env.name}[/]")
                 for child in children:
                     node.add(child)
                 node.children[-1].label += "\n"  # type: ignore
 
         def _get_collapsed_folders(node: Folder) -> List[Folder]:
             found = []
             for child in node.children:
```

### Comparing `finalynx-1.8.3/finalynx/copilot/copilot.py` & `finalynx-1.9.0/finalynx/copilot/copilot.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/dashboard/dashboard.py` & `finalynx-1.9.0/finalynx/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/fetch/__init__.py` & `finalynx-1.9.0/finalynx/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/fetch/fetch.py` & `finalynx-1.9.0/finalynx/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/fetch/fetch_finary.py` & `finalynx-1.9.0/finalynx/fetch/fetch_finary.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/.gitignore` & `finalynx-1.9.0/finalynx/finary_api/.gitignore`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/LICENSE` & `finalynx-1.9.0/finalynx/finary_api/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/README.md` & `finalynx-1.9.0/finalynx/finary_api/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/__init__.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/__main__.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/bank_account_types.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/currencies.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/currencies.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/importers/cryptocom.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/securities.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/signin.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/signin.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/user_cryptos.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/user_generic_assets.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/user_holdings_accounts.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/user_portfolio.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/user_portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/user_precious_metals.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/user_securities.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/user_securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/finary_api/finary_api/views.py` & `finalynx-1.9.0/finalynx/finary_api/finary_api/views.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/parse/json.py` & `finalynx-1.9.0/finalynx/parse/json.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/parse/parser.py` & `finalynx-1.9.0/finalynx/parse/parser.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/portfolio/__init__.py` & `finalynx-1.9.0/finalynx/portfolio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 from .constants import AssetClass
 from .constants import EnvelopeClass
 from .envelope import *
 from .folder import Folder
 from .folder import FolderDisplay
 from .hierarchy import Hierarchy
 from .line import Line
+from .line import LinePerf
 from .node import Node
 from .portfolio import Portfolio
 from .targets import *
```

### Comparing `finalynx-1.8.3/finalynx/portfolio/bucket.py` & `finalynx-1.9.0/finalynx/portfolio/bucket.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/portfolio/constants.py` & `finalynx-1.9.0/finalynx/portfolio/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 """
 ```{tip}
 % TODO
 These enumerations are not yet used in Finalynx, but will serve as the basis for the `Analyzer`
 subpackage to classify lines and show relevant statistics.
 ```
 """
+from dataclasses import dataclass
 from enum import Enum
+from typing import Optional
+
+
+@dataclass
+class LinePerf:
+    """Represents a Line's expected performance.
+    :param expected: this investment's expected yearly return (e.g. 2 for 2%/yr)
+    :param skip: Don't use this line when calculating the performance in upper nodes
+    """
+
+    expected: float
+    pessimistic: Optional[float] = 0  # TODO not used
+    optimistic: Optional[float] = 0  # TODO not used
+    skip: bool = False
 
 
 class AssetClass(Enum):
     """Enumeration that defines the asset class for each line."""
 
     CASH = "Cash"
     LIVRET = "Livrets"
```

### Comparing `finalynx-1.8.3/finalynx/portfolio/envelope.py` & `finalynx-1.9.0/finalynx/portfolio/envelope.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/portfolio/folder.py` & `finalynx-1.9.0/finalynx/portfolio/folder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from enum import Enum
 from typing import Any
 from typing import List
 from typing import Optional
-from typing import TYPE_CHECKING
 
 import numpy as np
 from finalynx.console import console
 from finalynx.portfolio.targets import TargetRatio
 from rich.tree import Tree
 
 from .constants import AssetClass
 from .line import Line
+from .line import LinePerf
 from .node import Node
-
-if TYPE_CHECKING:
-    from .targets import Target
+from .targets import Target
 
 
 class FolderDisplay(Enum):
     """Enumeration to select how a folder should be displayed.
 
     There are three options:
     - **Expanded:** Show all children in the output.
@@ -39,37 +37,42 @@
         name: str,
         asset_class: AssetClass = AssetClass.UNKNOWN,
         parent: Optional["Folder"] = None,
         target: Optional["Target"] = None,
         children: Optional[List["Node"]] = None,
         newline: bool = False,
         display: FolderDisplay = FolderDisplay.EXPANDED,
+        perf: Optional[LinePerf] = None,
     ):
         """
         This class handles the orchestration of rendering of its children.
 
         :param name: Name to be displayed in the final output.
+        :param asset_class: Useful shortcut to set all chidlren's asset class at once. Children keep priority
+        over this shortcut.
         :param parent: Optional Node object as a parent. Each folder sets their children's
         parents as itself by default.
         :param target: Optional `Target` instance for this folder to render the total amount
         based on your own investment objectives.
         :param children: List of `Node` objects contained in the folder. The folder's amount
         corresponds to the sum of the amounts contained in all children.
         :param newline: When printing to the console, you can print a blank line after this folder
         for better readability.
         :param display: Choose how the folder should be displayed (expanded, collapsed or as a line).
+        :param perf: Useful shortcut to set all chidlren's performance at once. Children keep priority
+        over this shortcut.
         """
         super().__init__(name, parent, target, newline)
         self.children = [] if children is None else children
         self.display = display
 
         for child in self.children:
             child.set_parent(self)
 
-        self.set_children_class(asset_class)
+        self.set_children(asset_class, perf)
 
     def add_child(self, child: Node) -> None:
         """Manually add a child at the end of the existing children in this folder.
         :param child: Any `Node` object to add as a child.
         :returns: Nohing to return.
         """
         child.set_parent(self)
@@ -77,14 +80,47 @@
 
     def get_amount(self) -> float:
         """Get the total amount contained in this folder.
         :returns: The sum of what each child's `get_amount()` method returns.
         """
         return float(np.sum([child.get_amount() for child in self.children]) if self.children else 0)
 
+    def get_ideal(self) -> float:
+        """:returns: The ideal amount to be invested in this node based on surrounding targets."""
+        return (
+            self.target.get_ideal()
+            if self.target.check() != Target.RESULT_NONE
+            else float(np.sum([c.get_ideal() for c in self.children]))
+        )
+
+    def get_perf(self, ideal: bool = True) -> LinePerf:
+        """Get the weighted mean expected performance of all children to get the folder's
+        expected performance."""
+
+        # Get children's performances
+        children = [c for c in self.children if not (isinstance(c, Line) and c.perf.skip)]
+        perfs = [c.get_perf(ideal) if isinstance(c, Folder) else c.get_perf() for c in children]
+
+        # If this folder is empty or all children want to be skipped, mark self as skipped
+        if not children or np.all([p.skip for p in perfs]):
+            return LinePerf(0, skip=True)
+
+        # Get every not-skipped children's expected amounts (either current or ideal)
+        amounts = [(c.get_ideal() if ideal else c.get_amount()) for c in children]
+        total = np.sum(amounts)
+
+        # If children have not set targets, give identical weights to each child
+        if not total:
+            weights = list(np.ones(len(amounts)) / len(amounts))
+        else:
+            weights = [e / total for e in amounts]
+
+        # Calculate the folder's performance as the weighted sum of not-skipped children's performances
+        return LinePerf(np.sum([w * p.expected for w, p in zip(weights, perfs)]))
+
     def tree(
         self,
         output_format: str = "[console]",
         _tree: Optional[Tree] = None,
         hide_root: bool = False,
         **render_args: Any,
     ) -> Tree:
@@ -102,14 +138,15 @@
         render = self.render(output_format, **render_args)
         node = _tree.add(render) if _tree else Tree(render, guide_style="grey42", hide_root=hide_root)
         if self.display == FolderDisplay.EXPANDED:
             for child in self.children:
                 child.tree(output_format=output_format, _tree=node, **render_args)
         return node
 
+    # TODO convert this to show any customizable output_format?
     def tree_delta(self, _tree: Optional[Tree] = None) -> Tree:
         """Generates a tree with delta amounts to be invested to reach the ideal portfolio allocation."""
         render = self._render_delta()
 
         # Follow the same print policy as the main tree
         if self.display == FolderDisplay.COLLAPSED and self.newline:
             render += "\n"
@@ -156,20 +193,23 @@
             if isinstance(child, Line) and child.key == key:
                 child.amount += amount
                 success = True
             elif isinstance(child, Folder) and child.set_child_amount(key, amount):
                 success = True
         return success
 
-    def set_children_class(self, asset_class: AssetClass) -> None:
+    def set_children(self, asset_class: AssetClass, perf: Optional[LinePerf]) -> None:
+        """Used at initialization time by Folders to set attributes once in the Folder
+        instead of setting it in each child."""
         for child in self.children:
             if isinstance(child, Line):
                 child.asset_class = asset_class if child.asset_class is AssetClass.UNKNOWN else child.asset_class
+                child.perf = perf if perf and child.perf.expected == 0 else child.perf
             elif isinstance(child, Folder):
-                child.set_children_class(asset_class)
+                child.set_children(asset_class, perf)
             else:
                 raise ValueError("Unrecognized node type.")
 
     def _render_name_color(self) -> str:
         """Internal method that overrides the superclass' render method to display
         the folder name with a bold font of different color.
         """
@@ -184,7 +224,15 @@
 
     def _render_newline(self) -> str:
         """Internal method that overrides the superclass' render method to display
         a new line after the folder has rendered.
         :returns: The newline character depending on the user configuration.
         """
         return "\n" if self.newline and self.display != FolderDisplay.EXPANDED else ""
+
+    def _render_ideal(self) -> str:
+        """:returns: A string representation of the ideal amount to be invested in
+        this folder. If this folder has no target, use the sum of its children's ideals."""
+        if self.target.check() != Target.RESULT_NONE:
+            return self.target.render_ideal()
+        ideal = float(np.sum([c.get_ideal() for c in self.children]))
+        return f"{round(ideal)} € " if ideal else ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finalynx-1.8.3/finalynx/portfolio/line.py` & `finalynx-1.9.0/finalynx/portfolio/line.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import TYPE_CHECKING
 
 from .constants import AssetClass
+from .constants import LinePerf
 from .node import Node
 
 if TYPE_CHECKING:
     from .envelope import Envelope
     from .targets import Target
     from .folder import Folder
 
@@ -21,14 +22,15 @@
         asset_class: AssetClass = AssetClass.UNKNOWN,
         parent: Optional["Folder"] = None,
         target: Optional["Target"] = None,
         key: Optional[str] = None,
         amount: float = 0,
         newline: bool = False,
         envelope: Optional["Envelope"] = None,
+        perf: Optional[LinePerf] = None,
     ):
         """
         This is a subclass of `Node` that adds an `amount` and `key` property.
 
         :param name: The name that will be displayed in the final portfolio tree.
         :param parent: Parent of this line. If this line is created in a `Folder` instance,
         the folder will set iself as the parent at the initialization stage.
@@ -45,18 +47,23 @@
         }
 
         super().__init__(name, parent, target, newline, agents=render_agents)
         self.asset_class = asset_class
         self.key = key if key is not None else name
         self.amount = amount
         self.envelope = envelope
+        self.perf = perf if perf else LinePerf(0)
 
         # Let the envelope know that this is a child line
         if self.envelope:
             self.envelope.link_line(self)
 
     def get_amount(self) -> float:
         """:returns: The amount invested in this line."""
         return self.amount
 
+    def get_perf(self) -> LinePerf:
+        """:returns: The expected yearly performance of this line (set by user)."""
+        return self.perf
+
     def _render_account_code(self) -> str:
         return f"[{self.envelope.code}] " if self.envelope else ""
```

### Comparing `finalynx-1.8.3/finalynx/portfolio/node.py` & `finalynx-1.9.0/finalynx/portfolio/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict
 from typing import Optional
 from typing import TYPE_CHECKING
 
 import numpy as np
 from rich.tree import Tree
 
+from .constants import LinePerf
 from .hierarchy import Hierarchy
 from .render import Render
 from .targets import Target
 
 if TYPE_CHECKING:
     from .folder import Folder
 
@@ -47,15 +48,17 @@
         if target is not None:
             target.set_parent(self)
 
         # Setup custom aliases for node rendering
         render_aliases: Dict[str, str] = {
             "[text]": "[target_text][prehint] [name] [hint][newline]",
             "[console]": "[target] [account_code][name_color][name][/] [dim white][hint][/][newline]",
-            "[console_deltas]": "[delta][account_code][name_color][name][/] [newline]",
+            "[console_ideal]": "[bold green][ideal][/][account_code][name_color][name][/][newline]",
+            "[console_deltas]": "[delta][account_code][name_color][name][/][newline]",
+            "[console_perf]": "[bold green][perf][/][account_code][name_color][name][/][newline]",
             "[console_targets]": "[bold green][goal][/][account_code][name_color][name][/][newline]",
             "[text_targets]": "[goal][name][newline]",
             "[dashboard_tree]": "[amount] [currency] [name]",
             "[dashboard_console]": "[bold][target][/][bright_black][prehint][/] [name_color][name][/] [bright_black][hint][/][newline]",
             "[target]": "[[target_color]][target_text][/]",
             "[target_text]": "[target_symbol] [amount] [currency]",
         }
@@ -63,14 +66,15 @@
             "name": self._render_name,
             "name_color": self._render_name_color,
             "newline": self._render_newline,
             "amount": self._render_amount,
             "goal": self._render_goal,
             "ideal": self._render_ideal,
             "delta": self._render_delta,
+            "perf": self._render_perf,
             "hint": self._render_hint,
             "prehint": self._render_prehint,
             "currency": self._render_currency,
             "target_symbol": self.target._render_target_symbol,
             "target_color": self.target._render_target_color,
         }
         render_aliases.update(aliases if aliases else {})
@@ -85,14 +89,18 @@
         """:returns: The ideal amount to be invested in this node based on surrounding targets."""
         return self.target.get_ideal()
 
     def get_delta(self) -> float:
         """:returns: How much should be invested in this node to reach the ideal amount set by the target."""
         return self.get_ideal() - self.get_amount()
 
+    def get_perf(self) -> LinePerf:
+        """:returns: The expected yearly performance of this node."""
+        raise NotImplementedError("Must be overridden by children classes")
+
     def tree(
         self,
         output_format: str = "[console]",
         _tree: Optional[Tree] = None,
         hide_root: bool = False,
         **render_args: Any,
     ) -> Tree:
@@ -164,20 +172,25 @@
         max_length = (
             np.max([len(str(abs(round(c.get_delta())))) for c in self.parent.children])
             if (self.parent and self.parent.children)
             else 0
         )
         return f"[{color}]{'+' if delta > 0 else '-'}{abs(delta):>{max_length}} €[/] "
 
+    def _render_perf(self) -> str:
+        """:returns: A formatted rendering of the node's expected yearly performance."""
+        perf = self.get_perf()
+        return f"[{'strike ' if perf.skip else ''}bold green]{perf.expected:.1f} %[/] " if perf else ""
+
     def _render_name(self) -> str:
         """:returns: A formatted rendering of the node name."""
         return self.name
 
     def _render_name_color(self) -> str:
-        """:returns: A formatted rendering of the node name."""
+        """:returns: A formatted rendering of the node name's color."""
         return "[black]"
 
     def _render_newline(self) -> str:
         """:returns: A rendering of the newline if set by the user."""
         return "\n" if self.newline else ""
 
     def __repr__(self) -> str:
```

### Comparing `finalynx-1.8.3/finalynx/portfolio/portfolio.py` & `finalynx-1.9.0/finalynx/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/portfolio/render.py` & `finalynx-1.9.0/finalynx/portfolio/render.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/portfolio/targets.py` & `finalynx-1.9.0/finalynx/portfolio/targets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/simulator/simulator.py` & `finalynx-1.9.0/finalynx/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.3/finalynx/usage.py` & `finalynx-1.9.0/finalynx/usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 
 # Define the finalynx command-line usage which varies depending on how it's called.
 # When "sys.argv[0]" is the path to a python script, it means the user is using its own script.
 # Otherwise, the user is using
 __doc__ = f"""
 Finalynx command line v{__version__}
 Usage:
-  finalynx {main_filter(main_usage)}[targets | deltas | text | --format=string] [dashboard] [options]
+  finalynx {main_filter(main_usage)}[ideal | targets | deltas | perf | text | --format=string] [dashboard] [options]
   finalynx (-h | --help)
   finalynx (-v | --version)
 
 Options:
   -h --help            Show this help message and exit
   -v --version         Display the current version and exit
 {main_filter(main_options)}
   dashboard            Launch an interactive web dashboard!
 
   --hide-deltas        Don't show delta investment recommendations next to the tree
   --format=string      Customize the output format to your own style and information
+  ideal                Shortcut to --format="[console_ideal]" (show ideal amounts to follow all targets)
   targets              Shortcut to --format="[console_targets]" (show target values instead of amounts)
   deltas               Shortcut to --format="[console_deltas]" (show deltas instead of amounts)
+  perf                 Shortcut to --format="[console_perf]" (show expected performances)
   text                 Shortcut to --format="[console_text]" (no colors)
 
   -i --ignore-orphans  Ignore fetched lines that you didn't reference in your portfolio
   -c --clear-cache     Delete any data from Finary that was cached locally
   -f --force-signin    Clear cache, cookies and credentials files to sign in again
   -a --hide-amounts    Display your portfolio with dots instead of the real values (easier to share)
   -d --show-data       Show what has been fetched online (e.g. from your Finary account)
```

### Comparing `finalynx-1.8.3/pyproject.toml` & `finalynx-1.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finalynx"
-version = "1.8.3"
+version = "1.9.0"
 description = "A command line investment assistant to organize your portfolio and simulate its future to reach your life goals."
 authors = ["MadeInPierre <pielaclau@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "finalynx"}]
 include = [{ path = "finalynx/finary_api/**/*" }]
 
@@ -48,15 +48,15 @@
 upload_to_pypi = true
 upload_to_release = true
 commit_subject = "chore(release): auto bump version to {version}"
 build_command = "pip install poetry && poetry build"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.8.3"
+version = "1.9.0"
 tag_format = "v$version"
 
 [tool.mypy]
 exclude = [
     "finary_api/*",
     "docs/*",
     "tests/*.py"
```

### Comparing `finalynx-1.8.3/PKG-INFO` & `finalynx-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalynx
-Version: 1.8.3
+Version: 1.9.0
 Summary: A command line investment assistant to organize your portfolio and simulate its future to reach your life goals.
 License: GPLv3
 Author: MadeInPierre
 Author-email: pielaclau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finalynx Version: 1.8.3 Summary: A command line
+Metadata-Version: 2.1 Name: finalynx Version: 1.9.0 Summary: A command line
 investment assistant to organize your portfolio and simulate its future to
 reach your life goals. License: GPLv3 Author: MadeInPierre Author-email:
 pielaclau@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: docopt (==0.6.2)
```

