# Comparing `tmp/dxsp-2.0.8.tar.gz` & `tmp/dxsp-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.8.tar", max compression
+gzip compressed data, was "dxsp-2.0.9.tar", max compression
```

## Comparing `dxsp-2.0.8.tar` & `dxsp-2.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-08 12:00:54.029170 dxsp-2.0.8/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-08 12:00:54.029170 dxsp-2.0.8/README.md
--rw-r--r--   0        0        0       86 2023-05-08 12:00:54.689184 dxsp-2.0.8/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/config.py
--rw-r--r--   0        0        0     3271 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26429 2023-05-08 12:00:54.029170 dxsp-2.0.8/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-08 12:00:54.689184 dxsp-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-08 13:45:01.323274 dxsp-2.0.9/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-08 13:45:01.323274 dxsp-2.0.9/README.md
+-rw-r--r--   0        0        0       86 2023-05-08 13:45:02.315296 dxsp-2.0.9/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/config.py
+-rw-r--r--   0        0        0     3109 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    25292 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-08 13:45:02.315296 dxsp-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.9/PKG-INFO
```

### Comparing `dxsp-2.0.8/LICENSE` & `dxsp-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.8/README.md` & `dxsp-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.8/dxsp/assets/blockchains.py` & `dxsp-2.0.9/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.8/dxsp/default_settings.toml` & `dxsp-2.0.9/dxsp/default_settings.toml`

 * *Files 7% similar despite different names*

```diff
@@ -42,25 +42,23 @@
 dex_base_api = "https://goerli.api.0x.org/"
 
 [chain_5]
 loglevel = "DEBUG"
 dex_chain_id = 5
 dex_rpc = "https://rpc.ankr.com/eth_goerli"
 dex_block_explorer_url = "https://api-Goerli.etherscan.io/api?"
-dex_block_explorer_api =  ""
 dex_protocol_type = "uniswap_v2"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_base_api = "https://goerli.api.0x.org/"
 
 [chain_11155111]
 loglevel = "DEBUG"
 dex_chain_id = 11155111
 dex_rpc = "https://rpc.ankr.com/eth_sepolia"
 dex_block_explorer_url = "https://api-Sepolia.etherscan.io/api?"
-dex_block_explorer_api =  ""
 dex_protocol_type = "0x"
 dex_router_contract_addr = "0x1f98431c8ad98523631ae4a59f267346ea31f984"
 dex_base_api = "https://sepolia.api.0x.org/"
 
 [chain_56]
 dex_chain_id = 56
 dex_rpc = "https://rpc.ankr.com/bsc"
@@ -71,21 +69,17 @@
 dex_base_api = "https://api.1inch.exchange/v5.0/56"
 
 [chain_97]
 loglevel = "DEBUG"
 dex_chain_id = 97
 dex_rpc = "https://rpc.ankr.com/bsc_testnet_chapel"
 dex_block_explorer_url = "https://api-testnet.bscscan.com/api?"
-dex_block_explorer_api =  ""
-dex_protocol_type = ""
 dex_router_contract_addr = ""
 dex_base_api = ""
 
 [chain_42161]
 loglevel = "DEBUG"
 dex_chain_id = 42161
 dex_rpc = "https://rpc.ankr.com/arbitrum"
 dex_block_explorer_url = "https://api-testnet.bscscan.com/api?"
-dex_block_explorer_api =  ""
-dex_protocol_type = ""
 dex_router_contract_addr = "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f"
 dex_base_api = "https://api.1inch.exchange/v5.0/42161"
```

### Comparing `dxsp-2.0.8/dxsp/main.py` & `dxsp-2.0.9/dxsp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,21 +113,18 @@
                 + "/quote?fromTokenAddress="
                 + str(asset_in_address)
                 + "&toTokenAddress="
                 + str(asset_out_address)
                 + "&amount="
                 + str(asset_out_amount))
             quote_response = await self._get(quote_url)
-            self.logger.debug("quote %s", quote_response)
             quote_amount = quote_response['toTokenAmount']
-            quote_decimals = quote_response['fromToken']['decimals']
-            quote = (
-                self.w3.from_wei(int(quote_amount), 'wei') /
-                (10 ** quote_decimals))
-            self.logger.debug("quote %s", quote)
+            # quote_decimals = quote_response['fromToken']['decimals']
+            quote = self.w3.from_wei(int(quote_amount), 'ether')
+            # /(10 ** quote_decimals))
             return round(quote, 2)
         except Exception as e:
             self.logger.error("oneinch_quote %s", e)
             return
 
     async def uniswap_v2_quote(
         self,
@@ -165,24 +162,26 @@
         try:
             asset_out_symbol = (
                 settings.trading_quote_ccy if
                 action == "BUY" else instrument)
             asset_in_symbol = (
                 instrument if action == "BUY"
                 else settings.trading_quote_ccy)
-            asset_out_contract = await self.get_token_contract(
-                asset_out_symbol)
             try:
+                asset_out_contract = await self.get_token_contract(
+                    asset_out_symbol)
                 asset_out_decimals = (
-                    asset_out_contract.functions.decimals().call())
+                    asset_out_contract.functions.decimals().call()
+                    or 18)
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
                 asset_out_decimals = 18
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            #  buy or sell %p percentage DEFAULT OPTION is 10%
+
+            #  Amount to risk percentage - DEFAULT OPTION is 10%
             asset_out_amount = (
                 (asset_out_balance) /
                 (settings.trading_risk_amount
                  ** asset_out_decimals)
                 )*(float(quantity)/100)
 
             order = await self.get_swap(
@@ -211,15 +210,15 @@
             asset_out_address = await self.search_contract(
                 asset_out_symbol)
             asset_out_contract = await self.get_token_contract(
                 asset_out_symbol)
             if asset_out_contract is None:
                 raise ValueError("No contract identified")
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            if asset_out_balance == 0:
+            if asset_out_balance == (0 or None):
                 self.logger.warning("No Money")
                 raise ValueError("No Money")
                 return
             # ASSETS IN
             asset_in_address = await self.search_contract(asset_in_symbol)
             self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
@@ -230,19 +229,20 @@
             self.logger.debug("asset_out_decimals %s", asset_out_decimals)
             asset_out_amount = amount * 10 ** asset_out_decimals
             asset_out_amount_converted = self.w3.to_wei(
                 asset_out_amount, 'ether')
 
             order_amount = int(
                 (asset_out_amount_converted *
-                 (settings.slippage/100)))
+                 (settings.trading_slippage/100)))
             self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
-            await self.get_approve(asset_out_address)
+            if (await self.get_approve(asset_out_address)) is None:
+                return
 
             # 1INCH
             if self.protocol_type in ["1inch"]:
                 swap_order = await self.oneinch_swap(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
@@ -289,15 +289,15 @@
                     + "&toTokenAddress="
                     + asset_in_address
                     + "&amount="
                     + amount
                     + "&fromAddress="
                     + self.wallet_address
                     + "&slippage="
-                    + settings.slippage
+                    + settings.trading_slippage
                     )
         swap_order = await self._get(swap_url)
         swap_order_status = swap_order['statusCode']
         if swap_order_status != 200:
             return
         return swap_order
 
@@ -354,24 +354,27 @@
             self.logger.info("trade %s", trade)
             return trade
         except Exception as e:
             self.logger.error("get_confirmation %s", e)
             return
 
     async def get_block_explorer_status(self, txHash):
-        if settings.block_explorer_api:
-            self.logger.debug("get_block_explorer_status %s", txHash)
-            checkTransactionSuccessURL = (
-                settings.block_explorer_url
-                + "?module=transaction&action=gettxreceiptstatus&txhash="
-                + str(txHash)
-                + "&apikey="
-                + str(settings.block_explorer_api))
-            checkTransactionRequest = self._get(checkTransactionSuccessURL)
-            return checkTransactionRequest['status']
+        try:
+            if settings.block_explorer_api:
+                checkTransactionSuccessURL = (
+                    settings.block_explorer_url
+                    + "?module=transaction&action=gettxreceiptstatus&txhash="
+                    + str(txHash)
+                    + "&apikey="
+                    + str(settings.block_explorer_api))
+                checkTransactionRequest = self._get(checkTransactionSuccessURL)
+                return checkTransactionRequest['status']
+        except Exception as e:
+            self.logger.error("get_block_explorer_status %s", e)
+            return
 
 # ###CONTRACT SEARCH
     async def search_contract(
                             self,
                             token
                             ):
         """search a contract function"""
@@ -397,53 +400,48 @@
                 return self.w3.to_checksum_address(token_contract)
             self.logger.info("no contract found for %s", token)
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
 
     async def search_cg(self, token):
-        """search coingecko"""
-        self.logger.debug("search_cg")
+        """🦎 search coingecko"""
         try:
             search_results = self.cg.search(query=token)
             search_dict = search_results['coins']
             filtered_dict = [x for x in search_dict if
                              x['symbol'] == token.upper()]
             api_dict = [sub['api_symbol'] for sub in filtered_dict]
-            self.logger.debug("api_dict %s", api_dict)
             for i in api_dict:
                 coin_dict = self.cg.get_coin_by_id(i)
                 try:
                     if coin_dict['platforms'][f'{self.cg_platform}']:
                         return coin_dict
                 except KeyError:
                     pass
         except Exception as e:
             self.logger.error("search_cg %s", e)
             return
 
     async def search_cg_contract(self, token):
-        """search coingecko contract"""
-        self.logger.debug("🦎search_cg_contract %s", token)
+        """🦎 search coingecko contract"""
         try:
             coin_info = await self.search_cg(token)
             if coin_info is not None:
                 return coin_info['platforms'][f'{self.cg_platform}']
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
 
     async def get_contract_address(
                             self,
                             token_list_url,
                             symbol
                         ):
-        """Given a token symbol and json format url address tokenlist,
-        get token address"""
-        self.logger.debug("get_contract_address %s %s", token_list_url, symbol)
+        """Given a token symbol and json tokenlist, get token address"""
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and
                    keyval['chainId'] == self.chain_id):
                     return keyval['address']
@@ -463,70 +461,79 @@
             return self.w3.eth.contract(
                 address=token_address,
                 abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s", e)
             return
 
-# ###UTILS
-    async def get_approve(
-                        self,
-                        asset_out_address: str,
-                        amount=None
-                    ):
+# W3 UTILS
+    async def get_approve(self, asset_out_address):
+        try:
+            if self.protocol_type in ["1inch", "1inch_limit"]:
+                await self.get_approve_1inch(asset_out_address)
+            elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+                await self.get_approve_uniswap(asset_out_address)
+        except Exception as e:
+            self.logger.error("get_approve %s", e)
+            return None
 
-        self.logger.debug("get_approve %s", asset_out_address)
-        if self.protocol_type in ["1inch", "1inch_limit"]:
+    async def get_approve_1inch(self, asset_out_address):
+        try:
             approval_check_URL = (
                 settings.dex_base_api
                 + "/approve/allowance?tokenAddress="
                 + str(asset_out_address)
                 + "&walletAddress="
                 + str(self.wallet_address))
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check == 0):
                 approval_URL = (
                     settings.dex_base_api
                     + "/approve/transaction?tokenAddress="
                     + str(asset_out_address))
                 approval_response = await self._get(approval_URL)
-        elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+                return approval_response
+        except Exception as e:
+            self.logger.error("get_approve_uniswap %s", e)
+            return None
+
+    async def get_approve_uniswap(self, asset_out_address):
+
+        try:
             asset_out_abi = await self.get_abi(asset_out_address)
             asset_out_contract = self.w3.eth.contract(
-                                 address=asset_out_address,
-                                 abi=asset_out_abi)
+                address=asset_out_address,
+                abi=asset_out_abi)
             approval_check = asset_out_contract.functions.allowance(
-                             self.w3.to_checksum_address(self.wallet_address),
-                             self.w3.to_checksum_address(
+                            self.w3.to_checksum_address(self.wallet_address),
+                            self.w3.to_checksum_address(
                                 settings.dex_router_contract_addr)
-                             ).call()
+                            ).call()
             if (approval_check == 0):
                 approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
-                asset_out_abi = await self.get_abi(asset_out_address)
-                asset_out_contract = self.w3.eth.contract(
-                                     address=asset_out_address,
-                                     abi=asset_out_abi)
                 approval_TX = asset_out_contract.functions.approve(
                                 self.w3.to_checksum_address(
                                     settings.router_contract_addr),
                                 approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = (
                     self.w3.eth.wait_for_transaction_receipt(
                         approval_txHash,
                         timeout=120,
                         poll_latency=0.1))
                 return approval_txHash_complete
+        except Exception as e:
+            self.logger.error("get_approve_uniswap %s", e)
+            return None
 
     async def get_sign(
-                    self,
-                    order
-                ):
-        self.logger.debug("get_sign %s", order)
+        self,
+        order
+         ):
 
         try:
             if not isinstance(order, dict):
                 raise ValueError("Transaction must be a dictionary")
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 order_params = {
                             'from': self.wallet_address,
@@ -552,29 +559,28 @@
             self.logger.error("get_sign: %s", e)
             raise
         except Exception as e:
             self.logger.error("get_sign: %s", e)
             raise RuntimeError("Failed to sign transaction")
 
     async def get_gas(
-                    self,
-                    tx
-                ):
+        self,
+        tx
+         ):
         # Log the transaction
         self.logger.debug("get_gas %s", tx)
         # Estimate the gas cost of the transaction
         gasestimate = self.w3.eth.estimate_gas(tx) * 1.25
         # Return the estimated gas cost in wei
         return int(self.w3.to_wei(gasestimate, 'wei'))
 
     async def get_gasPrice(self, tx):
         '''
         Get the gas price for a transaction
         '''
-        self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasprice, 'gwei')
 
     async def get_abi(self, addr):
         # Log a debug message to the logger
         self.logger.debug("get_abi %s", addr)
         if settings.dex_block_explorer_api:
@@ -582,105 +588,93 @@
                 # Create a dictionary of parameters
                 params = {
                     "module": "contract",
                     "action": "getabi",
                     "address": addr,
                     "apikey": settings.dex_block_explorer_api
                     }
-                # Create a dictionary of headers
-                headers = {"User-Agent": "Mozilla/5.0"}
                 # Make a GET request to the block explorer URL
                 resp = await self._get(
-                                       url=settings.dex_block_explorer_url,
-                                       params=params,
-                                       headers=headers
-                                       )
+                    url=settings.dex_block_explorer_url,
+                    params=params,
+                     )
                 # If the response status is 1, log the ABI
                 if resp['status'] == "1":
                     self.logger.debug("ABI found %s", resp)
                     abi = resp["result"]
                     return abi
                 # If no ABI is identified, log a warning
                 self.logger.warning("No ABI identified")
+                return None
             except Exception as e:
                 # Log an error
-                self.logger.error("error get_abi %s", e)
-                return
+                self.logger.error("get_abi %s", e)
+                return None
         else:
             # If no block_explorer_api is set, log a warning
             self.logger.warning("No block_explorer_api.")
             return
 
 # USER BALANCE AND POSITION RELATED
 
     async def get_token_balance(
-                                self,
-                                token
-                            ):
-        self.logger.debug("get_token_balance %s", token)
+        self,
+        token
+         ):
 
         try:
-            token_address = await self.search_contract(token)
-            if token_address is None:
-                raise ValueError(f"Token address not found for {token}")
-            token_abi = await self.get_abi(token_address)
-            if token_abi is None:
-                raise ValueError(f"ABI not found for {token_address}")
-            token_contract = self.w3.eth.contract(
-                address=token_address,
-                abi=token_abi)
+            token_contract = self.get_token_contract(token)
             token_balance = 0
-            try:
-                token_balance = token_contract.functions.balanceOf(
-                    self.wallet_address).call()
-            except ValueError as e:
-                self.logger.warning("Invalid address: %s", e)
+            token_balance = token_contract.functions.balanceOf(
+                self.wallet_address).call()
             return 0 if token_balance <= 0 else token_balance
         except Exception as e:
-            self.logger.error("get_token_balance %s: %s", token, e)
+            self.logger.error("get_token_balance: %s", e)
             return 0
 
     async def get_account_balance(
-                            self
-                        ):
+        self
+         ):
 
         try:
             balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(
                     self.wallet_address))
             balance = (self.w3.from_wei(balance, 'ether'))
             try:
                 trading_quote_ccy_balance = (
                     await self.get_trading_quote_ccy_balance())
                 if trading_quote_ccy_balance:
                     balance += "💵" + trading_quote_ccy_balance
-            except Exception as e:
-                self.logger.error("trading_quote_ccy_balance error: %s", e)
+            except Exception:
+                pass
 
             return round(balance, 5)
 
         except Exception as e:
-            self.logger.error("get_account_balance error: %s", e)
-            return "balance error"
+            self.logger.error("get_account_balance: %s", e)
+            return 0
 
     async def get_trading_quote_ccy_balance(
-                                self
-                            ):
+        self
+         ):
 
         try:
             trading_quote_ccy_balance = await self.get_token_balance(
                 settings.trading_quote_ccy)
             if trading_quote_ccy_balance:
                 return trading_quote_ccy_balance
             return 0
         except Exception as e:
-            self.logger.error("get_trading_quote_ccy_balance error: %s", e)
+            self.logger.error("quote_ccy_balance: %s", e)
             return 0
 
-    async def get_account_position(self):
+    async def get_account_position(
+        self
+         ):
 
         try:
             self.logger.debug("get_account_position")
             return
         except Exception as e:
-            self.logger.error("get_account_position error: %s", e)
+            self.logger.error("get_account_position: %s", e)
             return 0
```

### Comparing `dxsp-2.0.8/pyproject.toml` & `dxsp-2.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.8"
+version = "2.0.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.8/PKG-INFO` & `dxsp-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.8
+Version: 2.0.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

