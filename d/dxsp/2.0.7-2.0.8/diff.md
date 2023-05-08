# Comparing `tmp/dxsp-2.0.7.tar.gz` & `tmp/dxsp-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.7.tar", max compression
+gzip compressed data, was "dxsp-2.0.8.tar", max compression
```

## Comparing `dxsp-2.0.7.tar` & `dxsp-2.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-08 10:31:51.186301 dxsp-2.0.7/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-08 10:31:51.186301 dxsp-2.0.7/README.md
--rw-r--r--   0        0        0       86 2023-05-08 10:31:51.826299 dxsp-2.0.7/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26429 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-08 10:31:51.826299 dxsp-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-08 12:00:54.029170 dxsp-2.0.8/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-08 12:00:54.029170 dxsp-2.0.8/README.md
+-rw-r--r--   0        0        0       86 2023-05-08 12:00:54.689184 dxsp-2.0.8/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/config.py
+-rw-r--r--   0        0        0     3271 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26429 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-08 12:00:54.689184 dxsp-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.8/PKG-INFO
```

### Comparing `dxsp-2.0.7/LICENSE` & `dxsp-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.7/README.md` & `dxsp-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.7/dxsp/assets/blockchains.py` & `dxsp-2.0.8/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.7/dxsp/default_settings.toml` & `dxsp-2.0.8/dxsp/default_settings.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 [default]
 loglevel = "INFO"
-
 #📝tokenlist
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-
 #📝trading setup
 trading_quote_ccy = "USDT"
 trading_risk_amount = 10 # for 10% of the position
 trading_slippage = 2 #for 2 % slippage
-
 #user settings
 dex_wallet_address = "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE" #this is an example
 dex_private_key = "0x111111111117dc0aaaaaa0fa6a738034aaaa302" #this is an example
-
+dex_block_explorer_api =  "798437294880920392"  #this is an example
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
-dex_block_explorer_api =  ""
 dex_protocol_type = "1inch" 
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" 
 dex_base_api = "https://api.1inch.exchange/v5.0/1"
 
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
-
 #0️⃣0x
 dex_0x_url = "https://api.0x.org/mainnet/"
 dex_0x_limit_url = ""
-
-#📝apollo
+#🪐apollo
 apollo_spot_api_key = ""
 apollo_spot_api_secret = ""
 apollo_future_api_key = ""
 apollo_future_api_secret = ""
 
+[chain_1]
+dex_chain_id = 1
+dex_rpc = "https://rpc.ankr.com/eth"
+dex_block_explorer_url = "https://api.etherscan.io/api?"
+dex_protocol_type = "uniswap_v2"
+dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
+dex_base_api = "https://goerli.api.0x.org/"
+
 [chain_5]
 loglevel = "DEBUG"
 dex_chain_id = 5
 dex_rpc = "https://rpc.ankr.com/eth_goerli"
 dex_block_explorer_url = "https://api-Goerli.etherscan.io/api?"
 dex_block_explorer_api =  ""
 dex_protocol_type = "uniswap_v2"
```

### Comparing `dxsp-2.0.7/dxsp/main.py` & `dxsp-2.0.8/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.7/pyproject.toml` & `dxsp-2.0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.7"
+version = "2.0.8"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.7/PKG-INFO` & `dxsp-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.7
+Version: 2.0.8
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

