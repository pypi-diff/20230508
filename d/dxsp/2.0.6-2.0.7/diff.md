# Comparing `tmp/dxsp-2.0.6.tar.gz` & `tmp/dxsp-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.6.tar", max compression
+gzip compressed data, was "dxsp-2.0.7.tar", max compression
```

## Comparing `dxsp-2.0.6.tar` & `dxsp-2.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-08 06:37:53.863155 dxsp-2.0.6/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-08 06:37:53.863155 dxsp-2.0.6/README.md
--rw-r--r--   0        0        0       86 2023-05-08 06:37:54.559162 dxsp-2.0.6/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26307 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-08 06:37:54.559162 dxsp-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-08 10:31:51.186301 dxsp-2.0.7/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-08 10:31:51.186301 dxsp-2.0.7/README.md
+-rw-r--r--   0        0        0       86 2023-05-08 10:31:51.826299 dxsp-2.0.7/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26429 2023-05-08 10:31:51.186301 dxsp-2.0.7/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-08 10:31:51.826299 dxsp-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.7/PKG-INFO
```

### Comparing `dxsp-2.0.6/LICENSE` & `dxsp-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.6/README.md` & `dxsp-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.6/dxsp/assets/blockchains.py` & `dxsp-2.0.7/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.6/dxsp/default_settings.toml` & `dxsp-2.0.7/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.6/dxsp/main.py` & `dxsp-2.0.7/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,44 +26,42 @@
                 self.logger.info("connected %s", self.w3)
         except Exception as e:
             self.logger.error("connectivity failed %s", e)
             return
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
-        # USER SECRET
+        # USER
         self.wallet_address = settings.dex_wallet_address
         self.private_key = settings.dex_private_key
 
         # COINGECKO
         try:
             self.cg = CoinGeckoAPI()
             assetplatform = self.cg.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
-                           == int(settings.dex_chain_id)]
+                           == int(self.chain_id)]
             self.cg_platform = output_dict[0]['id']
             self.logger.debug("cg_platform %s", self.cg_platform)
         except Exception as e:
             self.logger.error("CoinGecko: %s", e)
             return
 
     async def _get(
-                self,
-                url,
-                params=None,
-                headers=None
+        self,
+        url,
+        params=None,
+        headers=None
             ):
         headers = {"User-Agent": "Mozilla/5.0"}
-        self.logger.debug("_get url %s", url)
         response = requests.get(
-                            url,
-                            params=params,
-                            headers=headers,
-                            timeout=10
-                        )
+            url,
+            params=params,
+            headers=headers,
+            timeout=10)
         return response.json()
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
             router = self.w3.eth.contract(
                 self.w3.to_checksum_address(
@@ -104,47 +102,55 @@
 
     async def oneinch_quote(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
-        asset_out_amount = self.w3.to_wei(amount, 'ether')
-        quote_url = (
-            settings.dex_base_api
-            + "/quote?fromTokenAddress="
-            + str(asset_in_address)
-            + "&toTokenAddress="
-            + str(asset_out_address)
-            + "&amount="
-            + str(asset_out_amount))
-        quote_response = await self._get(quote_url)
-        self.logger.debug("quote %s", quote_response)
-        quote_amount = quote_response['toTokenAmount']
-        quote_decimals = quote_response['fromToken']['decimals']
-        quote = (
-            self.w3.from_wei(int(quote_amount), 'wei') /
-            (10 ** quote_decimals))
-        self.logger.debug("quote %s", quote)
-        return round(quote, 2)
+        try:
+            asset_out_amount = self.w3.to_wei(amount, 'ether')
+            quote_url = (
+                settings.dex_base_api
+                + "/quote?fromTokenAddress="
+                + str(asset_in_address)
+                + "&toTokenAddress="
+                + str(asset_out_address)
+                + "&amount="
+                + str(asset_out_amount))
+            quote_response = await self._get(quote_url)
+            self.logger.debug("quote %s", quote_response)
+            quote_amount = quote_response['toTokenAmount']
+            quote_decimals = quote_response['fromToken']['decimals']
+            quote = (
+                self.w3.from_wei(int(quote_amount), 'wei') /
+                (10 ** quote_decimals))
+            self.logger.debug("quote %s", quote)
+            return round(quote, 2)
+        except Exception as e:
+            self.logger.error("oneinch_quote %s", e)
+            return
 
     async def uniswap_v2_quote(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
-        order_path_dex = [asset_out_address, asset_in_address]
-        router_instance = await self.router()
-        order_min_amount = int(
-            router_instance.functions.getAmountsOut(
-                amount,
-                order_path_dex)
-            .call()[1])
-        return order_min_amount
+        try:
+            order_path_dex = [asset_out_address, asset_in_address]
+            router_instance = await self.router()
+            order_min_amount = int(
+                router_instance.functions.getAmountsOut(
+                    amount,
+                    order_path_dex)
+                .call()[1])
+            return order_min_amount
+        except Exception as e:
+            self.logger.error("uniswap_v2_quote %s", e)
+            return
 
     async def uniswap_v3_quote(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
@@ -153,32 +159,35 @@
     async def execute_order(self, order_params):
         """execute swap function"""
         action = order_params.get('action')
         instrument = order_params.get('instrument')
         quantity = order_params.get('quantity', 1)
 
         try:
-            asset_out_symbol = (settings.trading_quote_ccy if
-                                action == "BUY" else instrument)
-            asset_in_symbol = (instrument if action == "BUY"
-                               else settings.trading_quote_ccy)
+            asset_out_symbol = (
+                settings.trading_quote_ccy if
+                action == "BUY" else instrument)
+            asset_in_symbol = (
+                instrument if action == "BUY"
+                else settings.trading_quote_ccy)
             asset_out_contract = await self.get_token_contract(
                 asset_out_symbol)
             try:
                 asset_out_decimals = (
                     asset_out_contract.functions.decimals().call())
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
                 asset_out_decimals = 18
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
             #  buy or sell %p percentage DEFAULT OPTION is 10%
-            asset_out_amount = ((asset_out_balance) /
-                                (settings.trading_risk_amount
-                                ** asset_out_decimals)
-                                )*(float(quantity)/100)
+            asset_out_amount = (
+                (asset_out_balance) /
+                (settings.trading_risk_amount
+                 ** asset_out_decimals)
+                )*(float(quantity)/100)
 
             order = await self.get_swap(
                     asset_out_symbol,
                     asset_in_symbol,
                     asset_out_amount
                     )
             if order:
@@ -432,15 +441,15 @@
         get token address"""
         self.logger.debug("get_contract_address %s %s", token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and
-                   keyval['chainId'] == settings.dex_chain_id):
+                   keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(
                                 self,
```

### Comparing `dxsp-2.0.6/pyproject.toml` & `dxsp-2.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.6"
+version = "2.0.7"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.6/PKG-INFO` & `dxsp-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.6
+Version: 2.0.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

