# Comparing `tmp/aiocryptopay-0.2.6.tar.gz` & `tmp/aiocryptopay-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocryptopay-0.2.6.tar", max compression
+gzip compressed data, was "aiocryptopay-0.2.7.tar", max compression
```

## Comparing `aiocryptopay-0.2.6.tar` & `aiocryptopay-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2022-12-05 16:03:04.838812 aiocryptopay-0.2.6/LICENSE
--rw-r--r--   0        0        0     1784 2022-12-05 16:03:04.839813 aiocryptopay-0.2.6/README.md
--rw-r--r--   0        0        0       82 2023-03-21 18:17:22.703212 aiocryptopay-0.2.6/aiocryptopay/__init__.py
--rw-r--r--   0        0        0    12938 2023-03-21 18:17:03.282717 aiocryptopay-0.2.6/aiocryptopay/api.py
--rw-r--r--   0        0        0     2136 2023-03-20 12:28:03.059079 aiocryptopay-0.2.6/aiocryptopay/base.py
--rw-r--r--   0        0        0      843 2023-03-21 18:17:03.286716 aiocryptopay-0.2.6/aiocryptopay/const.py
--rw-r--r--   0        0        0      131 2022-12-05 16:07:52.984529 aiocryptopay-0.2.6/aiocryptopay/exceptions/__init__.py
--rw-r--r--   0        0        0     1551 2023-03-20 12:28:03.065080 aiocryptopay-0.2.6/aiocryptopay/exceptions/factory.py
--rw-r--r--   0        0        0        0 2022-12-05 16:03:04.844812 aiocryptopay-0.2.6/aiocryptopay/models/__init__.py
--rw-r--r--   0        0        0      141 2022-12-05 16:07:52.995530 aiocryptopay-0.2.6/aiocryptopay/models/balance.py
--rw-r--r--   0        0        0      224 2023-03-21 18:17:03.290716 aiocryptopay-0.2.6/aiocryptopay/models/currencies.py
--rw-r--r--   0        0        0      793 2022-12-05 16:07:53.022044 aiocryptopay-0.2.6/aiocryptopay/models/invoice.py
--rw-r--r--   0        0        0      130 2022-12-05 16:07:53.002531 aiocryptopay-0.2.6/aiocryptopay/models/profile.py
--rw-r--r--   0        0        0      169 2022-12-05 16:47:13.745316 aiocryptopay-0.2.6/aiocryptopay/models/rates.py
--rw-r--r--   0        0        0      322 2022-12-05 16:07:53.015528 aiocryptopay-0.2.6/aiocryptopay/models/transfer.py
--rw-r--r--   0        0        0      206 2022-12-05 16:07:53.018668 aiocryptopay-0.2.6/aiocryptopay/models/update.py
--rw-r--r--   0        0        0       46 2022-12-05 16:42:12.806836 aiocryptopay-0.2.6/aiocryptopay/utils/__init__.py
--rw-r--r--   0        0        0      793 2022-12-05 16:47:13.754826 aiocryptopay-0.2.6/aiocryptopay/utils/exchange.py
--rw-r--r--   0        0        0      701 2023-03-21 18:17:12.162659 aiocryptopay-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2644 1970-01-01 00:00:00.000000 aiocryptopay-0.2.6/setup.py
--rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 aiocryptopay-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 16:03:04.838812 aiocryptopay-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1784 2022-12-05 16:03:04.839813 aiocryptopay-0.2.7/README.md
+-rw-r--r--   0        0        0       82 2023-05-08 12:47:23.802151 aiocryptopay-0.2.7/aiocryptopay/__init__.py
+-rw-r--r--   0        0        0    12716 2023-05-08 12:46:57.658276 aiocryptopay-0.2.7/aiocryptopay/api.py
+-rw-r--r--   0        0        0     2136 2023-03-20 12:28:03.059079 aiocryptopay-0.2.7/aiocryptopay/base.py
+-rw-r--r--   0        0        0      839 2023-05-08 12:41:06.571903 aiocryptopay-0.2.7/aiocryptopay/const.py
+-rw-r--r--   0        0        0      131 2022-12-05 16:07:52.984529 aiocryptopay-0.2.7/aiocryptopay/exceptions/__init__.py
+-rw-r--r--   0        0        0     1551 2023-03-20 12:28:03.065080 aiocryptopay-0.2.7/aiocryptopay/exceptions/factory.py
+-rw-r--r--   0        0        0        0 2022-12-05 16:03:04.844812 aiocryptopay-0.2.7/aiocryptopay/models/__init__.py
+-rw-r--r--   0        0        0      141 2022-12-05 16:07:52.995530 aiocryptopay-0.2.7/aiocryptopay/models/balance.py
+-rw-r--r--   0        0        0      224 2023-03-21 18:17:03.290716 aiocryptopay-0.2.7/aiocryptopay/models/currencies.py
+-rw-r--r--   0        0        0      793 2022-12-05 16:07:53.022044 aiocryptopay-0.2.7/aiocryptopay/models/invoice.py
+-rw-r--r--   0        0        0      130 2022-12-05 16:07:53.002531 aiocryptopay-0.2.7/aiocryptopay/models/profile.py
+-rw-r--r--   0        0        0      169 2022-12-05 16:47:13.745316 aiocryptopay-0.2.7/aiocryptopay/models/rates.py
+-rw-r--r--   0        0        0      322 2022-12-05 16:07:53.015528 aiocryptopay-0.2.7/aiocryptopay/models/transfer.py
+-rw-r--r--   0        0        0      206 2022-12-05 16:07:53.018668 aiocryptopay-0.2.7/aiocryptopay/models/update.py
+-rw-r--r--   0        0        0       46 2022-12-05 16:42:12.806836 aiocryptopay-0.2.7/aiocryptopay/utils/__init__.py
+-rw-r--r--   0        0        0      793 2022-12-05 16:47:13.754826 aiocryptopay-0.2.7/aiocryptopay/utils/exchange.py
+-rw-r--r--   0        0        0      720 2023-05-08 12:41:06.580901 aiocryptopay-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 aiocryptopay-0.2.7/setup.py
+-rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 aiocryptopay-0.2.7/PKG-INFO
```

### Comparing `aiocryptopay-0.2.6/LICENSE` & `aiocryptopay-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.6/README.md` & `aiocryptopay-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.6/aiocryptopay/api.py` & `aiocryptopay-0.2.7/aiocryptopay/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Consists of API methods only.
         All other methods are hidden in the BaseClient.
     """
 
     API_DOCS = "https://help.crypt.bot/crypto-pay-api"
 
     def __init__(
-            self, token: str, network: Union[str, Networks] = Networks.MAIN_NET
+        self, token: str, network: Union[str, Networks] = Networks.MAIN_NET
     ) -> None:
         super().__init__()
         """
         Init CryptoPay API client
             :param token: Your API token from @CryptoBot
             :param network: Network address https://help.crypt.bot/crypto-pay-api#HYA3
         """
@@ -101,25 +101,25 @@
 
         response = await self._make_request(
             method=method, url=url, headers=self.__headers
         )
         return [Currency(**currency) for currency in response["result"]]
 
     async def create_invoice(
-            self,
-            asset: Union[Assets, str],
-            amount: Union[int, float],
-            description: Optional[str] = None,
-            hidden_message: Optional[str] = None,
-            paid_btn_name: Optional[Union[PaidButtons, str]] = None,
-            paid_btn_url: Optional[str] = None,
-            payload: Optional[str] = None,
-            allow_comments: Optional[bool] = None,
-            allow_anonymous: Optional[bool] = None,
-            expires_in: Optional[int] = None,
+        self,
+        asset: Union[Assets, str],
+        amount: Union[int, float],
+        description: Optional[str] = None,
+        hidden_message: Optional[str] = None,
+        paid_btn_name: Optional[Union[PaidButtons, str]] = None,
+        paid_btn_url: Optional[str] = None,
+        payload: Optional[str] = None,
+        allow_comments: Optional[bool] = None,
+        allow_anonymous: Optional[bool] = None,
+        expires_in: Optional[int] = None,
     ) -> Invoice:
         """
         Use this method to create a new invoice. On success, returns an object of the created invoice.
         https://help.crypt.bot/crypto-pay-api#createInvoice
 
         Args:
             asset (Union[Assets, str]): Currency code. Supported assets: “BTC”, “TON”, “ETH”, “USDT”, “USDC” and “BUSD”.
@@ -140,15 +140,15 @@
         url = f"{self.network}/api/createInvoice"
 
         params = {
             "asset": asset,
             "amount": amount,
             "description": description,
             "hidden_message": hidden_message,
-            "paid_btn_name": paid_btn_name.value if isinstance(paid_btn_name, PaidButtons) else paid_btn_name,
+            "paid_btn_name": paid_btn_name,
             "paid_btn_url": paid_btn_url,
             "payload": payload,
             "allow_comments": allow_comments,
             "allow_anonymous": allow_anonymous,
             "expires_in": expires_in,
         }
 
@@ -160,20 +160,20 @@
 
         response = await self._make_request(
             method=method, url=url, params=params, headers=self.__headers
         )
         return Invoice(**response["result"])
 
     async def get_invoices(
-            self,
-            asset: Optional[Union[Assets, str]] = None,
-            invoice_ids: Optional[Union[List[int], int]] = None,
-            status: Optional[Union[InvoiceStatus, str]] = None,
-            offset: Optional[int] = None,
-            count: Optional[int] = None,
+        self,
+        asset: Optional[Union[Assets, str]] = None,
+        invoice_ids: Optional[Union[List[int], int]] = None,
+        status: Optional[Union[InvoiceStatus, str]] = None,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
     ) -> Optional[Union[Invoice, List[Invoice]]]:
         """
         Use this method to get invoices of your app. On success, returns array of invoices.
         https://help.crypt.bot/crypto-pay-api#getInvoices
 
         Args:
             asset (Optional[Union[Assets, str]], optional): Currency codes separated by comma. Supported assets: “BTC”, “TON”, “ETH”, “USDT”, “USDC” and “BUSD”. Defaults to all assets.
@@ -190,15 +190,15 @@
 
         if invoice_ids and type(invoice_ids) == list:
             invoice_ids = ",".join(map(str, invoice_ids))
 
         params = {
             "asset": asset,
             "invoice_ids": invoice_ids,
-            "status": status.value if isinstance(status, InvoiceStatus) else status,
+            "status": status,
             "offset": offset,
             "count": count,
         }
 
         for key, value in params.copy().items():
             if value is None:
                 del params[key]
@@ -208,21 +208,21 @@
         )
         if len(response["result"]["items"]) > 0:
             if invoice_ids and isinstance(invoice_ids, int):
                 return Invoice(**response["result"]["items"][0])
             return [Invoice(**invoice) for invoice in response["result"]["items"]]
 
     async def transfer(
-            self,
-            user_id: int,
-            asset: Union[Assets, str],
-            amount: Union[int, float],
-            spend_id: Union[str, int],
-            comment: Optional[str] = None,
-            disable_send_notification: Optional[bool] = None,
+        self,
+        user_id: int,
+        asset: Union[Assets, str],
+        amount: Union[int, float],
+        spend_id: Union[str, int],
+        comment: Optional[str] = None,
+        disable_send_notification: Optional[bool] = None,
     ) -> Transfer:
         """
         Use this method to send coins from your app's balance to a user. On success, returns object of completed transfer.
         https://help.crypt.bot/crypto-pay-api#transfer
 
         Args:
             user_id (int): Telegram user ID. User must have previously used @CryptoBot (@CryptoTestnetBot for testnet).
```

### Comparing `aiocryptopay-0.2.6/aiocryptopay/base.py` & `aiocryptopay-0.2.7/aiocryptopay/base.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.6/aiocryptopay/const.py` & `aiocryptopay-0.2.7/aiocryptopay/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from enum import Enum
+from strenum import StrEnum
 
 
-class HTTPMethods(str, Enum):
+class HTTPMethods(StrEnum):
     """Available HTTP methods."""
 
     POST = "POST"
     GET = "GET"
 
 
-class Networks(str, Enum):
+class Networks(StrEnum):
     """Cryptobot networks"""
 
     MAIN_NET = "https://pay.crypt.bot"
     TEST_NET = "https://testnet-pay.crypt.bot"
 
 
-class Assets(str, Enum):
+class Assets(StrEnum):
     """Cryptobot assets"""
 
     BTC = "BTC"
     TON = "TON"
     ETH = "ETH"
     USDT = "USDT"
     USDC = "USDC"
@@ -27,22 +27,22 @@
     BNB = "BNB"
 
     @classmethod
     def values(cls):
         return list(map(lambda asset: asset.value, cls))
 
 
-class PaidButtons(str, Enum):
+class PaidButtons(StrEnum):
     """Cryptobot paid button names"""
 
     VIEW_ITEM = "viewItem"
     OPEN_CHANNEL = "openChannel"
     OPEN_BOT = "openBot"
     CALLBACK = "callback"
 
 
-class InvoiceStatus(str, Enum):
+class InvoiceStatus(StrEnum):
     """Invoice status"""
 
     ACTIVE = "active"
     PAID = "paid"
     EXPIRED = "expired"
```

### Comparing `aiocryptopay-0.2.6/aiocryptopay/exceptions/factory.py` & `aiocryptopay-0.2.7/aiocryptopay/exceptions/factory.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.6/aiocryptopay/models/invoice.py` & `aiocryptopay-0.2.7/aiocryptopay/models/invoice.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.6/aiocryptopay/utils/exchange.py` & `aiocryptopay-0.2.7/aiocryptopay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.6/pyproject.toml` & `aiocryptopay-0.2.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocryptopay"
-version = "0.2.6"
+version = "0.2.7"
 description = "@cryptobot api asynchronous python wrapper"
 authors = ["layerqa"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/layerqa/aiocryptopay"
 documentation = "https://help.crypt.bot/crypto-pay-api"
 keywords = [
@@ -14,16 +14,17 @@
     "cryptopay api",
     "cryptobot api"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.3"
-certifi = "^2022.9.14"
-pydantic = "^1.10.2"
+certifi = "^2023.5.7"
+pydantic = "^1.10.7"
+strenum = "^0.4.10"
 
 [tool.poetry.dev-dependencies]
 aiogram = "^2.22.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
```

### Comparing `aiocryptopay-0.2.6/setup.py` & `aiocryptopay-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,21 @@
  'aiocryptopay.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0',
- 'certifi>=2022.9.14,<2023.0.0',
- 'pydantic>=1.10.2,<2.0.0']
+ 'certifi>=2023.5.7,<2024.0.0',
+ 'pydantic>=1.10.7,<2.0.0',
+ 'strenum>=0.4.10,<0.5.0']
 
 setup_kwargs = {
     'name': 'aiocryptopay',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': '@cryptobot api asynchronous python wrapper',
     'long_description': "## **[@cryptobot](https://t.me/CryptoBot) asynchronous api wrapper**\n**Docs:** https://help.crypt.bot/crypto-pay-api\n\n - MainNet - [@CryptoBot](http://t.me/CryptoBot)\n - TestNet - [@CryptoTestnetBot](http://t.me/CryptoTestnetBot)\n\n\n**Install**\n``` bash\npip install aiocryptopay\npoetry add aiocryptopay\n```\n\n**Basic methods**\n``` python\nfrom aiocryptopay import AioCryptoPay, Networks\n\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\nprofile = await crypto.get_me()\ncurrencies = await crypto.get_currencies()\nbalance = await crypto.get_balance()\nrates = await crypto.get_exchange_rates()\n\nprint(profile, currencies, balance, rates, sep='\\n')\n```\n\n**Create and get invoice methods**\n``` python\nfrom aiocryptopay import AioCryptoPay, Networks\n\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\ninvoice = await crypto.create_invoice(asset='TON', amount=1.5)\nprint(invoice.pay_url)\n\ninvoices = await crypto.get_invoices(invoice_ids=invoice.invoice_id)\nprint(invoices.status)\n```\n\n**WebHook usage**\n``` python\nfrom aiohttp import web\n\nfrom aiocryptopay import AioCryptoPay, Networks\nfrom aiocryptopay.models.update import Update\n\n\nweb_app = web.Application()\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\n\n@crypto.pay_handler()\nasync def invoice_paid(update: Update) -> None:\n    print(update)\n\nasync def create_invoice(app) -> None:\n    invoice = await crypto.create_invoice(asset='TON', amount=1.5)\n    print(invoice.pay_url)\n\nasync def close_session(app) -> None:\n    await crypto.close()\n\n\nweb_app.add_routes([web.post('/crypto-secret-path', crypto.get_updates)])\nweb_app.on_startup.append(create_invoice)\nweb_app.on_shutdown.append(close_session)\nweb.run_app(app=web_app, host='localhost', port=3001)\n```",
     'author': 'layerqa',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/layerqa/aiocryptopay',
```

### Comparing `aiocryptopay-0.2.6/PKG-INFO` & `aiocryptopay-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: aiocryptopay
-Version: 0.2.6
+Version: 0.2.7
 Summary: @cryptobot api asynchronous python wrapper
 Home-page: https://github.com/layerqa/aiocryptopay
 License: MIT
 Keywords: aiocryptopay,cryptobot,cryptopay,cryptopay api,cryptobot api
 Author: layerqa
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: certifi (>=2022.9.14,<2023.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: strenum (>=0.4.10,<0.5.0)
 Project-URL: Documentation, https://help.crypt.bot/crypto-pay-api
 Project-URL: Repository, https://github.com/layerqa/aiocryptopay
 Description-Content-Type: text/markdown
 
 ## **[@cryptobot](https://t.me/CryptoBot) asynchronous api wrapper**
 **Docs:** https://help.crypt.bot/crypto-pay-api
```

