# Comparing `tmp/cashfree_lrs_client-1.0.5.tar.gz` & `tmp/cashfree_lrs_client-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashfree_lrs_client-1.0.5.tar", max compression
+gzip compressed data, was "cashfree_lrs_client-1.0.6.tar", max compression
```

## Comparing `cashfree_lrs_client-1.0.5.tar` & `cashfree_lrs_client-1.0.6.tar`

### file list

```diff
@@ -1,114 +1,115 @@
--rw-r--r--   0        0        0     5353 2023-05-03 17:46:50.957705 cashfree_lrs_client-1.0.5/README.md
--rw-r--r--   0        0        0     1759 2023-05-03 17:46:50.997706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/__init__.py
--rw-r--r--   0        0        0       99 2023-05-03 17:46:51.001706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/__init__.py
--rw-r--r--   0        0        0    53538 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/default_api.py
--rw-r--r--   0        0        0    53935 2023-05-03 17:46:50.933705 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/lrs_api.py
--rw-r--r--   0        0        0    30034 2023-05-03 17:46:51.013706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_client.py
--rw-r--r--   0        0        0      844 2023-05-03 17:46:51.013706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_response.py
--rw-r--r--   0        0        0      214 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/__init__.py
--rw-r--r--   0        0        0     1655 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/path_to_api.py
--rw-r--r--   0        0        0      246 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      119 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/beneficiaries.py
--rw-r--r--   0        0        0      121 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/fx_rate_details.py
--rw-r--r--   0        0        0      105 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders.py
--rw-r--r--   0        0        0      137 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders_documents_upload.py
--rw-r--r--   0        0        0      153 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
--rw-r--r--   0        0        0      136 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders_order_id_process.py
--rw-r--r--   0        0        0      111 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/remitters.py
--rw-r--r--   0        0        0      109 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/webhooks.py
--rw-r--r--   0        0        0      306 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      308 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tags/lrs_api.py
--rw-r--r--   0        0        0    15922 2023-05-03 17:46:50.989706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/configuration.py
--rw-r--r--   0        0        0     2815 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
--rw-r--r--   0        0        0     2331 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderRequest.md
--rw-r--r--   0        0        0     1337 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderResponse.md
--rw-r--r--   0        0        0     2583 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateRemitterRequest.md
--rw-r--r--   0        0        0      389 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Currency.md
--rw-r--r--   0        0        0      859 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Error.md
--rw-r--r--   0        0        0     1656 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/FetchForexRateRequest.md
--rw-r--r--   0        0        0    59748 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/LrsApi.md
--rw-r--r--   0        0        0      343 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Purpose.md
--rw-r--r--   0        0        0     1239 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SetupWebhooksRequest.md
--rw-r--r--   0        0        0      896 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SuccessMessage.md
--rw-r--r--   0        0        0     5118 2023-05-03 17:46:51.005706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/exceptions.py
--rw-r--r--   0        0        0      353 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/__init__.py
--rw-r--r--   0        0        0      884 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.py
--rw-r--r--   0        0        0      815 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.pyi
--rw-r--r--   0        0        0    14903 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.py
--rw-r--r--   0        0        0    13066 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.pyi
--rw-r--r--   0        0        0    11475 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.py
--rw-r--r--   0        0        0    10572 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.pyi
--rw-r--r--   0        0        0     8398 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.py
--rw-r--r--   0        0        0     8166 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.pyi
--rw-r--r--   0        0        0    12349 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.py
--rw-r--r--   0        0        0    10785 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.pyi
--rw-r--r--   0        0        0     1192 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.py
--rw-r--r--   0        0        0     1031 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.pyi
--rw-r--r--   0        0        0     3384 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.py
--rw-r--r--   0        0        0     3384 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.pyi
--rw-r--r--   0        0        0     5805 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     5697 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
--rw-r--r--   0        0        0     1368 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.py
--rw-r--r--   0        0        0     1169 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.pyi
--rw-r--r--   0        0        0     3663 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.py
--rw-r--r--   0        0        0     3663 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.pyi
--rw-r--r--   0        0        0     2477 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.py
--rw-r--r--   0        0        0     2477 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.pyi
--rw-r--r--   0        0        0     1119 2023-05-03 17:46:51.001706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/__init__.py
--rw-r--r--   0        0        0      714 2023-05-03 17:46:50.657701 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/country.py
--rw-r--r--   0        0        0     1975 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary200_response.py
--rw-r--r--   0        0        0     5660 2023-05-03 17:46:50.689701 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary_request.py
--rw-r--r--   0        0        0     5041 2023-05-03 17:46:50.721702 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_request.py
--rw-r--r--   0        0        0     3426 2023-05-03 17:46:50.741702 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_response.py
--rw-r--r--   0        0        0     1951 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter200_response.py
--rw-r--r--   0        0        0     5347 2023-05-03 17:46:50.757702 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter_request.py
--rw-r--r--   0        0        0      765 2023-05-03 17:46:50.769703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/currency.py
--rw-r--r--   0        0        0     2088 2023-05-03 17:46:50.785703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/error.py
--rw-r--r--   0        0        0     3279 2023-05-03 17:46:50.793703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     2903 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/order_response.py
--rw-r--r--   0        0        0      780 2023-05-03 17:46:50.797703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/purpose.py
--rw-r--r--   0        0        0     1943 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks200_response.py
--rw-r--r--   0        0        0     2361 2023-05-03 17:46:50.801703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks_request.py
--rw-r--r--   0        0        0     1909 2023-05-03 17:46:50.809703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/success_message.py
--rw-r--r--   0        0        0      644 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/__init__.py
--rw-r--r--   0        0        0    12582 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.py
--rw-r--r--   0        0        0    12396 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.pyi
--rw-r--r--   0        0        0      326 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/__init__.py
--rw-r--r--   0        0        0    11760 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.py
--rw-r--r--   0        0        0    11604 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.pyi
--rw-r--r--   0        0        0      309 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/__init__.py
--rw-r--r--   0        0        0    13005 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.py
--rw-r--r--   0        0        0    12789 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.pyi
--rw-r--r--   0        0        0      343 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
--rw-r--r--   0        0        0    12334 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.py
--rw-r--r--   0        0        0    12148 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
--rw-r--r--   0        0        0      361 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
--rw-r--r--   0        0        0    15715 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
--rw-r--r--   0        0        0    15469 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
--rw-r--r--   0        0        0      343 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
--rw-r--r--   0        0        0     8093 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.py
--rw-r--r--   0        0        0     7937 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
--rw-r--r--   0        0        0      315 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/__init__.py
--rw-r--r--   0        0        0    12525 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.py
--rw-r--r--   0        0        0    12339 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.pyi
--rw-r--r--   0        0        0      313 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    11939 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.py
--rw-r--r--   0        0        0    11783 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.pyi
--rw-r--r--   0        0        0    12643 2023-05-03 17:46:51.017706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/rest.py
--rw-r--r--   0        0        0    97649 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/schemas.py
--rw-r--r--   0        0        0        0 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/__init__.py
--rw-r--r--   0        0        0     2694 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_beneficiary_request.py
--rw-r--r--   0        0        0     2292 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_request.py
--rw-r--r--   0        0        0     1952 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_response.py
--rw-r--r--   0        0        0     2486 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_remitter_request.py
--rw-r--r--   0        0        0      738 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_currency.py
--rw-r--r--   0        0        0     1439 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_error.py
--rw-r--r--   0        0        0     1860 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
--rw-r--r--   0        0        0     1845 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_lrs_api.py
--rw-r--r--   0        0        0      731 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_purpose.py
--rw-r--r--   0        0        0     1737 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_setup_webhooks_request.py
--rw-r--r--   0        0        0     1493 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_success_message.py
--rw-r--r--   0        0        0      683 2023-05-03 17:46:50.985706 cashfree_lrs_client-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6256 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5265 2023-05-08 08:42:49.801334 cashfree_lrs_client-1.0.6/README.md
+-rw-r--r--   0        0        0     1847 2023-05-08 08:42:49.825335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-08 08:42:49.829335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/__init__.py
+-rw-r--r--   0        0        0    53538 2023-05-08 08:42:26.100904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/default_api.py
+-rw-r--r--   0        0        0    54075 2023-05-08 08:42:49.785334 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/lrs_api.py
+-rw-r--r--   0        0        0    30034 2023-05-08 08:42:49.837335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_client.py
+-rw-r--r--   0        0        0      844 2023-05-08 08:42:49.837335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/__init__.py
+-rw-r--r--   0        0        0     1655 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      246 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/beneficiaries.py
+-rw-r--r--   0        0        0      121 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/fx_rate_details.py
+-rw-r--r--   0        0        0      105 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders.py
+-rw-r--r--   0        0        0      137 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders_documents_upload.py
+-rw-r--r--   0        0        0      153 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
+-rw-r--r--   0        0        0      136 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders_order_id_process.py
+-rw-r--r--   0        0        0      111 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/remitters.py
+-rw-r--r--   0        0        0      109 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/webhooks.py
+-rw-r--r--   0        0        0      306 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      308 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tags/lrs_api.py
+-rw-r--r--   0        0        0    16079 2023-05-08 08:42:49.825335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/configuration.py
+-rw-r--r--   0        0        0     2815 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
+-rw-r--r--   0        0        0     2331 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderRequest.md
+-rw-r--r--   0        0        0     1337 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderResponse.md
+-rw-r--r--   0        0        0     2583 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateRemitterRequest.md
+-rw-r--r--   0        0        0      389 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Currency.md
+-rw-r--r--   0        0        0      859 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Error.md
+-rw-r--r--   0        0        0     1656 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/FetchForexRateRequest.md
+-rw-r--r--   0        0        0    59748 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/LrsApi.md
+-rw-r--r--   0        0        0      343 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Purpose.md
+-rw-r--r--   0        0        0     1239 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SetupWebhooksRequest.md
+-rw-r--r--   0        0        0      896 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SuccessMessage.md
+-rw-r--r--   0        0        0     5118 2023-05-08 08:42:49.833335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/exceptions.py
+-rw-r--r--   0        0        0      353 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.py
+-rw-r--r--   0        0        0      815 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.pyi
+-rw-r--r--   0        0        0    14903 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.py
+-rw-r--r--   0        0        0    13066 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.pyi
+-rw-r--r--   0        0        0    11475 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.py
+-rw-r--r--   0        0        0    10572 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.pyi
+-rw-r--r--   0        0        0     8398 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.py
+-rw-r--r--   0        0        0     8166 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.pyi
+-rw-r--r--   0        0        0    12349 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.py
+-rw-r--r--   0        0        0    10785 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.pyi
+-rw-r--r--   0        0        0     1192 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.py
+-rw-r--r--   0        0        0     1031 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.pyi
+-rw-r--r--   0        0        0     3384 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.py
+-rw-r--r--   0        0        0     3384 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.pyi
+-rw-r--r--   0        0        0     5805 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     5697 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
+-rw-r--r--   0        0        0     1368 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.py
+-rw-r--r--   0        0        0     1169 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.pyi
+-rw-r--r--   0        0        0     3663 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.py
+-rw-r--r--   0        0        0     3663 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.pyi
+-rw-r--r--   0        0        0     2477 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.py
+-rw-r--r--   0        0        0     2477 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.pyi
+-rw-r--r--   0        0        0     1207 2023-05-08 08:42:49.829335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-08 08:42:49.533329 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/country.py
+-rw-r--r--   0        0        0     1975 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary200_response.py
+-rw-r--r--   0        0        0     5660 2023-05-08 08:42:49.545329 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary_request.py
+-rw-r--r--   0        0        0     5041 2023-05-08 08:42:49.565330 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_request.py
+-rw-r--r--   0        0        0     3426 2023-05-08 08:42:49.597330 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_response.py
+-rw-r--r--   0        0        0     1951 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter200_response.py
+-rw-r--r--   0        0        0     5347 2023-05-08 08:42:49.629331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter_request.py
+-rw-r--r--   0        0        0      765 2023-05-08 08:42:49.637331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/currency.py
+-rw-r--r--   0        0        0     2088 2023-05-08 08:42:49.641331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/error.py
+-rw-r--r--   0        0        0     3279 2023-05-08 08:42:49.649331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     2775 2023-05-08 08:42:49.653331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_response.py
+-rw-r--r--   0        0        0     2903 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/order_response.py
+-rw-r--r--   0        0        0      780 2023-05-08 08:42:49.661332 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/purpose.py
+-rw-r--r--   0        0        0     1943 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks200_response.py
+-rw-r--r--   0        0        0     2361 2023-05-08 08:42:49.669332 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks_request.py
+-rw-r--r--   0        0        0     1909 2023-05-08 08:42:49.673332 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/success_message.py
+-rw-r--r--   0        0        0      644 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/__init__.py
+-rw-r--r--   0        0        0    12582 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.py
+-rw-r--r--   0        0        0    12396 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.pyi
+-rw-r--r--   0        0        0      326 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/__init__.py
+-rw-r--r--   0        0        0    11760 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.py
+-rw-r--r--   0        0        0    11604 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/__init__.py
+-rw-r--r--   0        0        0    13005 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.py
+-rw-r--r--   0        0        0    12789 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
+-rw-r--r--   0        0        0    12334 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.py
+-rw-r--r--   0        0        0    12148 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
+-rw-r--r--   0        0        0    15715 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
+-rw-r--r--   0        0        0    15469 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
+-rw-r--r--   0        0        0     8093 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.py
+-rw-r--r--   0        0        0     7937 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/__init__.py
+-rw-r--r--   0        0        0    12525 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.py
+-rw-r--r--   0        0        0    12339 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.pyi
+-rw-r--r--   0        0        0      313 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    11939 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.py
+-rw-r--r--   0        0        0    11783 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0    12769 2023-05-08 08:42:49.841335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/rest.py
+-rw-r--r--   0        0        0    97649 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_beneficiary_request.py
+-rw-r--r--   0        0        0     2292 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_request.py
+-rw-r--r--   0        0        0     1952 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_response.py
+-rw-r--r--   0        0        0     2486 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_remitter_request.py
+-rw-r--r--   0        0        0      738 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_currency.py
+-rw-r--r--   0        0        0     1439 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_error.py
+-rw-r--r--   0        0        0     1860 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     1845 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_lrs_api.py
+-rw-r--r--   0        0        0      731 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_purpose.py
+-rw-r--r--   0        0        0     1737 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_setup_webhooks_request.py
+-rw-r--r--   0        0        0     1493 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_success_message.py
+-rw-r--r--   0        0        0      683 2023-05-08 08:42:49.817335 cashfree_lrs_client-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6168 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.6/PKG-INFO
```

### Comparing `cashfree_lrs_client-1.0.5/README.md` & `cashfree_lrs_client-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.5
-- Package version: 1.0.5
+- API version: 1.0.6
+- Package version: 1.0.6
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -46,15 +46,14 @@
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from __future__ import print_function
 
 import time
 import cashfree_lrs_client
 from cashfree_lrs_client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://sandbox.cashfree.com/pg/lrs
@@ -91,17 +90,15 @@
 with cashfree_lrs_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = cashfree_lrs_client.LrsApi(api_client)
     files = None # List[bytearray] | Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB
 
     try:
         # Upload Documents in Bulk
-        api_response = api_instance.bulk_documents_upload(files)
-        print("The response of LrsApi->bulk_documents_upload:\n")
-        pprint(api_response)
+        api_instance.bulk_documents_upload(files)
     except ApiException as e:
         print("Exception when calling LrsApi->bulk_documents_upload: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
@@ -125,14 +122,15 @@
  - [CreateBeneficiaryRequest](docs/CreateBeneficiaryRequest.md)
  - [CreateOrderRequest](docs/CreateOrderRequest.md)
  - [CreateOrderResponse](docs/CreateOrderResponse.md)
  - [CreateRemitterRequest](docs/CreateRemitterRequest.md)
  - [Currency](docs/Currency.md)
  - [Error](docs/Error.md)
  - [FetchForexRateRequest](docs/FetchForexRateRequest.md)
+ - [FetchForexRateResponse](docs/FetchForexRateResponse.md)
  - [Purpose](docs/Purpose.md)
  - [SetupWebhooksRequest](docs/SetupWebhooksRequest.md)
  - [SuccessMessage](docs/SuccessMessage.md)
 
 
 ## Documentation For Authorization
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/__init__.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 # import apis into sdk package
 from cashfree_lrs_client.api.lrs_api import LrsApi
 
 # import ApiClient
 from cashfree_lrs_client.api_response import ApiResponse
 from cashfree_lrs_client.api_client import ApiClient
@@ -36,10 +36,11 @@
 from cashfree_lrs_client.models.create_beneficiary_request import CreateBeneficiaryRequest
 from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.currency import Currency
 from cashfree_lrs_client.models.error import Error
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
+from cashfree_lrs_client.models.fetch_forex_rate_response import FetchForexRateResponse
 from cashfree_lrs_client.models.purpose import Purpose
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
 from cashfree_lrs_client.models.success_message import SuccessMessage
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/default_api.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/lrs_api.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/lrs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
 import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBytes, StrictStr, conlist
 
 from typing import Any, Dict, Optional, Union
 
 from cashfree_lrs_client.models.create_beneficiary_request import CreateBeneficiaryRequest
 from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
+from cashfree_lrs_client.models.fetch_forex_rate_response import FetchForexRateResponse
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
 from cashfree_lrs_client.models.success_message import SuccessMessage
 
 from cashfree_lrs_client.api_client import ApiClient
 from cashfree_lrs_client.api_response import ApiResponse
 from cashfree_lrs_client.exceptions import (  # noqa: F401
     ApiTypeError,
@@ -48,15 +50,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def bulk_documents_upload(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> object:  # noqa: E501
+    def bulk_documents_upload(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> None:  # noqa: E501
         """Upload Documents in Bulk  # noqa: E501
 
         Use this API to Upload documents before Order creation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_documents_upload(files, async_req=True)
@@ -69,15 +71,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: object
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the bulk_documents_upload_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.bulk_documents_upload_with_http_info(files, **kwargs)  # noqa: E501
 
     @validate_arguments
@@ -111,15 +113,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'files'
         ]
@@ -173,18 +175,15 @@
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['X-Client-ID', 'X-Client-Secret', 'X-API-Version']  # noqa: E501
 
-        _response_types_map = {
-            '200': "object",
-            '413': "Error",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
             '/orders/documents/upload', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
@@ -638,15 +637,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def fetch_forex_rate(self, fetch_forex_rate_request : Optional[FetchForexRateRequest] = None, **kwargs) -> None:  # noqa: E501
+    def fetch_forex_rate(self, fetch_forex_rate_request : Optional[FetchForexRateRequest] = None, **kwargs) -> FetchForexRateResponse:  # noqa: E501
         """Fetch FX Rate  # noqa: E501
 
         Use this API to get the foreign exchange rate.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.fetch_forex_rate(fetch_forex_rate_request, async_req=True)
@@ -659,15 +658,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: FetchForexRateResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the fetch_forex_rate_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.fetch_forex_rate_with_http_info(fetch_forex_rate_request, **kwargs)  # noqa: E501
 
     @validate_arguments
@@ -701,15 +700,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(FetchForexRateResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'fetch_forex_rate_request'
         ]
@@ -762,15 +761,17 @@
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['X-Client-ID', 'X-Client-Secret', 'X-API-Version']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "FetchForexRateResponse",
+        }
 
         return self.api_client.call_api(
             '/fx-rate/details', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_client.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.5/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.6/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/path_to_api.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tags/lrs_api.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tags/lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/configuration.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -159,14 +159,18 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
@@ -407,16 +411,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.5\n"\
-               "SDK Package Version: 1.0.5".\
+               "Version of the API: 1.0.6\n"\
+               "SDK Package Version: 1.0.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderRequest.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderResponse.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderResponse.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateRemitterRequest.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateRemitterRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Error.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Error.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/FetchForexRateRequest.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/FetchForexRateRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/LrsApi.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/LrsApi.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SetupWebhooksRequest.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SetupWebhooksRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SuccessMessage.md` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SuccessMessage.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/exceptions.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/__init__.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -19,10 +19,11 @@
 from cashfree_lrs_client.models.create_beneficiary_request import CreateBeneficiaryRequest
 from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.currency import Currency
 from cashfree_lrs_client.models.error import Error
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
+from cashfree_lrs_client.models.fetch_forex_rate_response import FetchForexRateResponse
 from cashfree_lrs_client.models.purpose import Purpose
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
 from cashfree_lrs_client.models.success_message import SuccessMessage
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/country.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/country.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary200_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter200_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/currency.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/error.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/order_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/purpose.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/purpose.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks200_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/success_message.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/success_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/__init__.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.pyi` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/rest.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.5
+    The version of the OpenAPI document: 1.0.6
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -63,14 +63,18 @@
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.tls_server_name:
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
+
+
         if configuration.socket_options is not None:
             addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
```

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/schemas.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/schemas.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_beneficiary_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_response.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_remitter_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_currency.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_error.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_lrs_api.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_purpose.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_setup_webhooks_request.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_success_message.py` & `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.5/pyproject.toml` & `cashfree_lrs_client-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cashfree_lrs_client"
-version = "1.0.5"
+version = "1.0.6"
 description = "Cashfree LRS"
 authors = ["CashFree Care <nextgenapi@cashfree.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_REPO_ID/GIT_USER_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Cashfree LRS"]
```

### Comparing `cashfree_lrs_client-1.0.5/PKG-INFO` & `cashfree_lrs_client-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashfree-lrs-client
-Version: 1.0.5
+Version: 1.0.6
 Summary: Cashfree LRS
 Home-page: https://github.com/GIT_REPO_ID/GIT_USER_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,Cashfree LRS
 Author: CashFree Care
 Author-email: nextgenapi@cashfree.com
 Requires-Python: >=3.7,<4.0
@@ -23,16 +23,16 @@
 Description-Content-Type: text/markdown
 
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.5
-- Package version: 1.0.5
+- API version: 1.0.6
+- Package version: 1.0.6
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -70,15 +70,14 @@
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from __future__ import print_function
 
 import time
 import cashfree_lrs_client
 from cashfree_lrs_client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://sandbox.cashfree.com/pg/lrs
@@ -115,17 +114,15 @@
 with cashfree_lrs_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = cashfree_lrs_client.LrsApi(api_client)
     files = None # List[bytearray] | Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB
 
     try:
         # Upload Documents in Bulk
-        api_response = api_instance.bulk_documents_upload(files)
-        print("The response of LrsApi->bulk_documents_upload:\n")
-        pprint(api_response)
+        api_instance.bulk_documents_upload(files)
     except ApiException as e:
         print("Exception when calling LrsApi->bulk_documents_upload: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
@@ -149,14 +146,15 @@
  - [CreateBeneficiaryRequest](docs/CreateBeneficiaryRequest.md)
  - [CreateOrderRequest](docs/CreateOrderRequest.md)
  - [CreateOrderResponse](docs/CreateOrderResponse.md)
  - [CreateRemitterRequest](docs/CreateRemitterRequest.md)
  - [Currency](docs/Currency.md)
  - [Error](docs/Error.md)
  - [FetchForexRateRequest](docs/FetchForexRateRequest.md)
+ - [FetchForexRateResponse](docs/FetchForexRateResponse.md)
  - [Purpose](docs/Purpose.md)
  - [SetupWebhooksRequest](docs/SetupWebhooksRequest.md)
  - [SuccessMessage](docs/SuccessMessage.md)
 
 
 ## Documentation For Authorization
```

