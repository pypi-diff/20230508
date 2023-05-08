# Comparing `tmp/pyaver-0.0.8.tar.gz` & `tmp/pyaver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyaver-0.0.8.tar", last modified: Tue Oct  4 13:41:49 2022, max compression
+gzip compressed data, was "pyaver-0.0.9.tar", last modified: Wed Jan 25 12:59:33 2023, max compression
```

## Comparing `pyaver-0.0.8.tar` & `pyaver-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2022-10-04 13:41:49.000000 pyaver-0.0.8/
--rw-r--r--   0 macbook    (501) staff       (20)      245 2022-10-04 13:41:49.000000 pyaver-0.0.8/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)       29 2022-09-24 14:45:24.000000 pyaver-0.0.8/MANIFEST.in
--rw-r--r--   0 macbook    (501) staff       (20)     2359 2022-09-24 14:45:24.000000 pyaver-0.0.8/README.md
--rw-r--r--   0 macbook    (501) staff       (20)      948 2022-10-04 13:41:47.000000 pyaver-0.0.8/setup.py
--rw-r--r--   0 macbook    (501) staff       (20)      103 2022-10-04 13:41:49.000000 pyaver-0.0.8/setup.cfg
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/pyaver/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/pyaver/idl/
--rw-r--r--   0 macbook    (501) staff       (20)    69764 2022-09-27 15:37:49.000000 pyaver-0.0.8/src/pyaver/idl/6q5ZGhEj6kkmEjuyCXuH4x8493bpi9fNzvy9L8hX83HQ.json
--rw-r--r--   0 macbook    (501) staff       (20)     4209 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/enums.py
--rw-r--r--   0 macbook    (501) staff       (20)    27061 2022-10-04 13:41:13.000000 pyaver-0.0.8/src/pyaver/market.py
--rw-r--r--   0 macbook    (501) staff       (20)     8897 2022-09-30 17:42:38.000000 pyaver-0.0.8/src/pyaver/checks.py
--rw-r--r--   0 macbook    (501) staff       (20)     3282 2022-09-27 15:37:49.000000 pyaver-0.0.8/src/pyaver/constants.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-07-08 10:33:23.000000 pyaver-0.0.8/src/pyaver/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    13036 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/user_host_lifetime.py
--rw-r--r--   0 macbook    (501) staff       (20)     4827 2022-09-26 11:59:26.000000 pyaver-0.0.8/src/pyaver/version_checks.py
--rw-r--r--   0 macbook    (501) staff       (20)    20795 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/orderbook.py
--rw-r--r--   0 macbook    (501) staff       (20)     6601 2022-10-04 13:41:13.000000 pyaver-0.0.8/src/pyaver/event_queue.py
--rw-r--r--   0 macbook    (501) staff       (20)    11021 2022-09-30 17:42:38.000000 pyaver-0.0.8/src/pyaver/aver_client.py
--rw-r--r--   0 macbook    (501) staff       (20)    19397 2022-10-04 12:15:27.000000 pyaver-0.0.8/src/pyaver/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     5199 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/refresh.py
--rw-r--r--   0 macbook    (501) staff       (20)     1507 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/errors.py
--rw-r--r--   0 macbook    (501) staff       (20)     4453 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/layouts.py
--rw-r--r--   0 macbook    (501) staff       (20)     6640 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/slab.py
--rw-r--r--   0 macbook    (501) staff       (20)     5323 2022-09-24 14:45:24.000000 pyaver-0.0.8/src/pyaver/data_classes.py
--rw-r--r--   0 macbook    (501) staff       (20)    59254 2022-10-04 12:15:20.000000 pyaver-0.0.8/src/pyaver/user_market.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/Pyaver.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)      245 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/Pyaver.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      847 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/Pyaver.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)       23 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/Pyaver.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        7 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/Pyaver.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2022-10-04 13:41:49.000000 pyaver-0.0.8/src/Pyaver.egg-info/dependency_links.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-01-25 12:59:33.890262 pyaver-0.0.9/
+-rw-r--r--   0 macbook    (501) staff       (20)     1073 2022-07-08 10:33:23.000000 pyaver-0.0.9/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)       29 2022-09-24 14:45:24.000000 pyaver-0.0.9/MANIFEST.in
+-rw-r--r--   0 macbook    (501) staff       (20)      256 2023-01-25 12:59:33.890402 pyaver-0.0.9/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2359 2022-09-24 14:45:24.000000 pyaver-0.0.9/README.md
+-rw-r--r--   0 macbook    (501) staff       (20)      103 2023-01-25 12:59:33.890954 pyaver-0.0.9/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      948 2023-01-25 12:58:34.000000 pyaver-0.0.9/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-01-25 12:59:33.877807 pyaver-0.0.9/src/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-01-25 12:59:33.881809 pyaver-0.0.9/src/Pyaver.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)      256 2023-01-25 12:59:33.000000 pyaver-0.0.9/src/Pyaver.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      855 2023-01-25 12:59:33.000000 pyaver-0.0.9/src/Pyaver.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-01-25 12:59:33.000000 pyaver-0.0.9/src/Pyaver.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       23 2023-01-25 12:59:33.000000 pyaver-0.0.9/src/Pyaver.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        7 2023-01-25 12:59:33.000000 pyaver-0.0.9/src/Pyaver.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-01-25 12:59:33.888701 pyaver-0.0.9/src/pyaver/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-07-08 10:33:23.000000 pyaver-0.0.9/src/pyaver/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11021 2022-09-30 17:42:38.000000 pyaver-0.0.9/src/pyaver/aver_client.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9226 2023-01-25 12:52:58.000000 pyaver-0.0.9/src/pyaver/checks.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3282 2023-01-13 10:11:24.000000 pyaver-0.0.9/src/pyaver/constants.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5323 2022-09-24 14:45:24.000000 pyaver-0.0.9/src/pyaver/data_classes.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4274 2023-01-25 12:50:22.000000 pyaver-0.0.9/src/pyaver/enums.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1507 2022-09-24 14:45:24.000000 pyaver-0.0.9/src/pyaver/errors.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6601 2022-11-16 12:15:03.000000 pyaver-0.0.9/src/pyaver/event_queue.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-01-25 12:59:33.889652 pyaver-0.0.9/src/pyaver/idl/
+-rw-r--r--   0 macbook    (501) staff       (20)    69764 2022-09-27 15:37:49.000000 pyaver-0.0.9/src/pyaver/idl/6q5ZGhEj6kkmEjuyCXuH4x8493bpi9fNzvy9L8hX83HQ.json
+-rw-r--r--   0 macbook    (501) staff       (20)     4453 2022-09-24 14:45:24.000000 pyaver-0.0.9/src/pyaver/layouts.py
+-rw-r--r--   0 macbook    (501) staff       (20)    27061 2023-01-06 15:21:11.000000 pyaver-0.0.9/src/pyaver/market.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20795 2022-09-24 14:45:24.000000 pyaver-0.0.9/src/pyaver/orderbook.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5199 2022-09-24 14:45:24.000000 pyaver-0.0.9/src/pyaver/refresh.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6640 2022-09-24 14:45:24.000000 pyaver-0.0.9/src/pyaver/slab.py
+-rw-r--r--   0 macbook    (501) staff       (20)    14080 2023-01-25 11:37:34.000000 pyaver-0.0.9/src/pyaver/user_host_lifetime.py
+-rw-r--r--   0 macbook    (501) staff       (20)    59267 2023-01-25 12:52:36.000000 pyaver-0.0.9/src/pyaver/user_market.py
+-rw-r--r--   0 macbook    (501) staff       (20)    21878 2023-01-25 12:32:36.000000 pyaver-0.0.9/src/pyaver/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4827 2023-01-06 15:21:11.000000 pyaver-0.0.9/src/pyaver/version_checks.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyaver-0.0.8/README.md` & `pyaver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/setup.py` & `pyaver-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             (pkg, mod, file)
             for (pkg, mod, file) in modules
             if not any(fnmatch.fnmatchcase(file, pat=pattern) for pattern in excluded)
         ]
 
 setup(
     name='pyaver',
-    version='0.0.08',
+    version='0.0.09',
     license='MIT',
     author="Aver Ramanujan",
     author_email='email@example.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://www.aver.exchange/',
     keywords='Aver Python SDK Solana',
```

### Comparing `pyaver-0.0.8/src/pyaver/idl/6q5ZGhEj6kkmEjuyCXuH4x8493bpi9fNzvy9L8hX83HQ.json` & `pyaver-0.0.9/src/pyaver/idl/6q5ZGhEj6kkmEjuyCXuH4x8493bpi9fNzvy9L8hX83HQ.json`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/enums.py` & `pyaver-0.0.9/src/pyaver/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,7 +146,11 @@
     fee_tier: int
 
 class AccountTypes(str, Enum):
     MARKET = 'Market'
     MARKET_STORE = 'MarketStore'
     USER_MARKET = 'UserMarket'
     USER_HOST_LIFETIME = 'UserHostLifetime'
+
+class PriceFormat(IntEnum):
+    PROBABILITY = 0
+    DECIMAL = 1
```

### Comparing `pyaver-0.0.8/src/pyaver/market.py` & `pyaver-0.0.9/src/pyaver/market.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/checks.py` & `pyaver-0.0.9/src/pyaver/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .utils import round_price_to_nearest_tick_size
+from .utils import round_price_to_nearest_tick_size, round_price_to_nearest_decimal_tick_size
 from .market import AverMarket
-from .enums import MarketStatus, OrderType, Side, SizeFormat
+from .enums import MarketStatus, OrderType, Side, SizeFormat, PriceFormat
 from .user_host_lifetime import UserHostLifetime
 from .data_classes import UserBalanceState, UserMarketState
 
 ###### PLACE ORDER CHECKS
 
 def check_sufficient_lamport_balance(user_balance_state: UserBalanceState):
     if(user_balance_state.lamport_balance < 5000):
@@ -48,14 +48,15 @@
 
 def check_stake_noop(size_format: SizeFormat, limit_price: float, side: Side):
     market_order = (limit_price == 1 and side == Side.BUY) or (limit_price == 0 and side == Side.SELL)
     if(size_format == SizeFormat.STAKE and market_order):
         raise Exception('Market orders are currently not supports for orders specified in STAKE.')
 
 def check_is_order_valid(
+    market: AverMarket,
     outcome_index: int,
     side: Side,
     limit_price: float,
     size: float,
     size_format: SizeFormat,
     tokens_available_to_sell: float,
     tokens_available_to_buy: float,
@@ -72,25 +73,25 @@
 
         Raises:
             Exception: Insufficient Token Balance
 
         Returns:
             bool: True if order is valid
         """
-        limit_price = round_price_to_nearest_tick_size(limit_price)
+        limit_price = round_price_to_nearest_tick_size(limit_price) if market.market_state.rounding_format == PriceFormat.PROBABILITY else round_price_to_nearest_decimal_tick_size(limit_price)
 
         balance_required = size * limit_price if size_format == SizeFormat.PAYOUT else size
         current_balance = tokens_available_to_sell if side == Side.SELL else tokens_available_to_buy
 
         if(current_balance < balance_required):
             raise Exception(f'Insufficient token balance to support this order. Balance: {current_balance}; Required: {balance_required}')
 
 def check_quote_and_base_size_too_small(market: AverMarket, side: Side, size_format: SizeFormat, outcome_id: int, limit_price: float, size: float):
     binary_second_outcome = market.market_state.number_of_outcomes == 2 and outcome_id == 1
-    limit_price_rounded = round_price_to_nearest_tick_size(limit_price)
+    limit_price_rounded = round_price_to_nearest_tick_size(limit_price) if market.market_state.rounding_format == PriceFormat.PROBABILITY else round_price_to_nearest_decimal_tick_size(limit_price)
 
     if(size_format == SizeFormat.PAYOUT):
         max_base_qty = size
         if(limit_price != 0):
             max_quote_qty = limit_price_rounded * max_base_qty
         else:
             max_quote_qty = max_base_qty
```

### Comparing `pyaver-0.0.8/src/pyaver/constants.py` & `pyaver-0.0.9/src/pyaver/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 SYSVAR_RENT_PUBKEY = PublicKey("SysvarRent111111111111111111111111111111111")
 """Public key of the synthetic account that serves the network fee resource consumption."""
 
 ##### OTHER CONSTANTS
 
 SYS_VAR_CLOCK = PublicKey('SysvarC1ock11111111111111111111111111111111')
 
-MAX_ITERATIONS_FOR_CONSUME_EVENTS = 5  
+MAX_ITERATIONS_FOR_CONSUME_EVENTS = 3  
 
 CALLBACK_INFO_LEN = 33
 
 CANCEL_ALL_ORDERS_INSTRUCTION_CHUNK_SIZE = 5
 
 USER_FACING_INSTRUCTIONS_TO_CHECK_IN_IDL = [
   'init_user_market',
```

### Comparing `pyaver-0.0.8/src/pyaver/user_host_lifetime.py` & `pyaver-0.0.9/src/pyaver/user_host_lifetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,14 +264,49 @@
         Returns:
             PublicKey: Public key of UserHostLifetime account
         """
         return PublicKey.find_program_address(
             [bytes('user-host-lifetime', 'utf-8'), bytes(owner), bytes(host)],
             program_id
         )
+    
+    async def make_update_nft_pfp_instruction(
+        self,
+        display_name: str,
+        nft_pubkey: PublicKey
+    ):
+        program = await self.aver_client.get_program_from_program_id(self.program_id)
+
+        return program.instruction['update_nft_pfp_display_name'](
+            nft_pubkey, 
+            display_name,
+            ctx=Context(
+                accounts={
+                    "user": self.user_host_lifetime_state.user,
+                    "user_host_lifetime": self.pubkey,
+                }
+            )
+        )
+  
+    async def update_nft_pfp_display_name(
+        self,
+        user: Keypair,
+        display_name: str,
+        nft_pubkey: PublicKey,
+        send_options: TxOpts = None
+    ):
+        ix = await self.make_update_nft_pfp_instruction(display_name = display_name, nft_pubkey = nft_pubkey)
+    
+        return await sign_and_send_transaction_instructions(
+            self.aver_client,
+            [user],
+            user,
+            [ix],
+            send_options = send_options
+        )
 
     async def make_update_user_host_lifetime_state_instruction(self):
         program = await self.aver_client.get_program_from_program_id(self.program_id)
         # TODO
         return None
 
     async def update_user_host_lifetime_state(self, fee_payer: Keypair = None, send_options: TxOpts = None):
```

### Comparing `pyaver-0.0.8/src/pyaver/version_checks.py` & `pyaver-0.0.9/src/pyaver/version_checks.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/orderbook.py` & `pyaver-0.0.9/src/pyaver/orderbook.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/event_queue.py` & `pyaver-0.0.9/src/pyaver/event_queue.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/aver_client.py` & `pyaver-0.0.9/src/pyaver/aver_client.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/utils.py` & `pyaver-0.0.9/src/pyaver/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -205,14 +205,97 @@
     limit_price_to_6dp = limit_price * factor
     tick_size  = calculate_tick_size_for_price(factor - limit_price_to_6dp if is_binary else limit_price_to_6dp)
     rounded_limit_price_to_6dp = round(limit_price_to_6dp/tick_size) * tick_size
     rounded_limit_price = rounded_limit_price_to_6dp / factor
 
     return rounded_limit_price
 
+def calculate_tick_size_for_decimal_price(limit_price_decimal: float):
+    """
+    Calculates tick size for specific price
+
+    Args:
+        limit_price (float): Limit price in decimal
+
+    Raises:
+        Exception: Limit price too low
+        Exception: Limit price too high
+
+    Returns:
+        int: Tick size
+    """
+    if(limit_price_decimal < 1.01):
+        raise Exception('Limit price too low')
+    if(limit_price_decimal <= 2):
+        return 0.01
+    if(limit_price_decimal <= 3):
+        return 0.02
+    if(limit_price_decimal <= 4):
+        return 0.05
+    if(limit_price_decimal <= 6):
+        return 0.1
+    if(limit_price_decimal <= 10):
+        return 0.2
+    if(limit_price_decimal <= 20):
+        return 0.5
+    if(limit_price_decimal <= 30):
+        return 1
+    if(limit_price_decimal <= 50):
+        return 2
+    if(limit_price_decimal <= 100):
+        return 5
+    if(limit_price_decimal <= 1000):
+        return 10
+    if(limit_price_decimal > 1000):
+        raise Exception('Limit price too high')
+    return limit_price_decimal
+
+def round_price_decimal(tickSize: float, limitPrice: float):
+  return round(limitPrice / tickSize) * tickSize
+
+def round_price_to_nearest_decimal_tick_size(limit_price: float, is_binary: bool = False):
+    """
+    Rounds price to the nearest tick size available
+
+    Args:
+        limit_price (float): Limit price
+
+    Returns:
+        float: Rounded limit price
+    """
+    limit_price_decimal = 1 / limit_price
+    one_in_market_decimals = pow(10, 6)
+
+    min_value_for_market = 1.01
+    max_value_for_market = 1000
+
+    if limit_price_decimal < min_value_for_market: 
+        return 1.0 / min_value_for_market
+    elif limit_price_decimal > max_value_for_market: 
+        return 1.0 / max_value_for_market
+    else:
+        limit_price_decimal_rounded = 0
+
+        if is_binary and limit_price_decimal > 2.0: 
+            limit_price_decimal_rounded = round_price_decimal(
+                calculate_tick_size_for_decimal_price(
+                    1.0 / ((one_in_market_decimals - limit_price) / one_in_market_decimals),
+                ),
+                limit_price_decimal,
+            )
+        else:
+            tick_size = calculate_tick_size_for_decimal_price(limit_price_decimal=limit_price_decimal)
+
+            limit_price_decimal_rounded = round_price_decimal(
+                tickSize=tick_size,
+                limitPrice=limit_price_decimal,
+            )
+
+        return 1.0 / limit_price_decimal_rounded
+
 def parse_user_market_state(buffer: bytes, aver_client: AverClient, program: Program = None):
         """
         Parses raw onchain data to UserMarketState object        
         Args:
             buffer (bytes): Raw bytes coming from onchain
             aver_client (AverClient): AverClient object
             program (Program, optional): Anchor Program. Defaults to first program in client.
```

### Comparing `pyaver-0.0.8/src/pyaver/refresh.py` & `pyaver-0.0.9/src/pyaver/refresh.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/errors.py` & `pyaver-0.0.9/src/pyaver/errors.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/layouts.py` & `pyaver-0.0.9/src/pyaver/layouts.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/slab.py` & `pyaver-0.0.9/src/pyaver/slab.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/data_classes.py` & `pyaver-0.0.9/src/pyaver/data_classes.py`

 * *Files identical despite different names*

### Comparing `pyaver-0.0.8/src/pyaver/user_market.py` & `pyaver-0.0.9/src/pyaver/user_market.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
             check_user_market_full(self.user_market_state)
             check_limit_price_error(limit_price, self.market)
             check_outcome_outside_space(outcome_id, self.market)
             check_incorrect_order_type_for_market_order(limit_price, order_type, side, self.market)
             check_stake_noop(size_format, limit_price, side)
             tokens_available_to_buy = self.calculate_tokens_available_to_buy(outcome_id, limit_price)
             tokens_available_to_sell = self.calculate_tokens_available_to_sell(outcome_id, limit_price)
-            check_is_order_valid(outcome_id, side, limit_price, size, size_format, tokens_available_to_sell, tokens_available_to_buy)
+            check_is_order_valid(self.market, outcome_id, side, limit_price, size, size_format, tokens_available_to_sell, tokens_available_to_buy)
             check_quote_and_base_size_too_small(self.market, side, size_format, outcome_id, limit_price, size)
             check_user_permission_and_quote_token_limit_exceeded(self.market, self.user_market_state, size, limit_price, size_format)
         
         max_base_qty = math.floor(size * (10 ** self.market.market_state.decimals))
         limit_price_u64 = math.ceil(limit_price * (10 ** self.market.market_state.decimals))
 
         is_binary_market_second_outcome = self.market.market_state.number_of_outcomes == 2 and outcome_id == 1
```

### Comparing `pyaver-0.0.8/src/Pyaver.egg-info/SOURCES.txt` & `pyaver-0.0.9/src/Pyaver.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 src/Pyaver.egg-info/PKG-INFO
 src/Pyaver.egg-info/SOURCES.txt
 src/Pyaver.egg-info/dependency_links.txt
```

