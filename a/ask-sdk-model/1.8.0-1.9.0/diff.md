# Comparing `tmp/ask-sdk-model-1.8.0.tar.gz` & `tmp/ask-sdk-model-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ask-sdk-model-1.8.0.tar", last modified: Wed Mar 13 23:18:44 2019, max compression
+gzip compressed data, was "dist/ask-sdk-model-1.9.0.tar", last modified: Thu Mar 28 17:47:57 2019, max compression
```

## Comparing `ask-sdk-model-1.8.0.tar` & `ask-sdk-model-1.9.0.tar`

### file list

```diff
@@ -1,429 +1,439 @@
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2615 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/CHANGELOG.rst
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       97 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/requirements.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/setup.cfg
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       81 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/MANIFEST.in
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      982 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/README.rst
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    20332 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/SOURCES.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/dependency_links.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       14 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/top_level.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/not-zip-safe
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5656 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       52 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model.egg-info/requires.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      544 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/LICENSE
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5656 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2113 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/setup.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/gadget_controller/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      669 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/gadget_controller/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4759 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/gadget_controller/set_light_directive.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      740 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7487 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/charge_amazon_pay_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8335 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/setup_amazon_pay_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4198 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3789 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      890 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7159 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3621 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/amazon_pay_error_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8069 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2086 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/payment_action.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4173 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/price.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1101 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6171 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_order_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6476 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/base_amazon_pay_entity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7833 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/authorize_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4690 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6130 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/billing_agreement_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4331 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_credit.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5999 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_billing_agreement_attributes.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2086 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/payment_action.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3516 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/price.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2026 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10028 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6366 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5173 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1393 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1830 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/release_environment.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5498 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_order_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7301 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/destination.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2110 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7144 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorize_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4003 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5427 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3652 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_credit.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5304 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_billing_agreement_attributes.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3609 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/price.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2001 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    11066 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7159 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/billing_agreement_details.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5328 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      930 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1751 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/release_environment.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7274 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/destination.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4417 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/charge_amazon_pay_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3813 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/setup_amazon_pay_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      798 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3761 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/amazon_pay_error_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1825 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/position.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5802 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/user_event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4646 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/render_document_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5530 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/auto_page_command.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1153 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6361 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/speak_item_command.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1851 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/align.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1837 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/highlight_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3232 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/runtime.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4404 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/execute_commands_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5806 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/command.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5565 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/set_page_command.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3303 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/alexa_presentation_apl_interface.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/automotive/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      664 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/automotive/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2926 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/automotive/automotive_state.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1762 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/touch.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1766 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/shape.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      776 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1830 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/keyboard.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7681 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/viewport_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4949 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/experience.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4186 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/text_content.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1757 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/back_button_behavior.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5045 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/list_template2.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1587 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4012 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/text_field.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3850 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/hint.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4880 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template7.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3404 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/hint_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3528 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/render_template_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5862 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/template.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3904 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/list_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1826 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/image_size.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3240 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/plain_text.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4656 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/element_selected_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5045 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/list_template1.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5068 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template1.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2985 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/display_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5407 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template2.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3236 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/rich_text.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3630 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/image.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3405 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/display_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3236 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/plain_text_hint.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5407 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template3.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3973 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/image_instance.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5193 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template6.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3030 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/error_cause.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5302 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/exception_encountered_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3480 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4460 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/system_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      822 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1904 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/error_type.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      890 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5638 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/connections_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4382 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/base_entity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      731 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4768 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/postal_address.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4184 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/restaurant.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3837 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/connections_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4275 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/send_response_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5415 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/send_request_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6308 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/connections_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4219 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/print_pdf_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      993 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4790 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/schedule_food_establishment_reservation_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4528 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/print_image_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5355 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/schedule_taxi_reservation_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5454 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/base_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4243 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/print_web_page_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4461 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/play_command_issued_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      892 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4477 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/previous_command_issued_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4461 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/next_command_issued_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4465 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/pause_command_issued_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2790 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_player_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5046 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_finished_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3037 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/stop_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1899 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/player_activity.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3500 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3640 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/clear_queue_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3941 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/stream.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3975 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_player_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1777 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/clear_behavior.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5799 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_failed_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5042 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_stopped_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1537 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3983 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/current_playback_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4102 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/play_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2165 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/error_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3762 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4503 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_item_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/play_behavior.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5042 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_started_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5070 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_nearly_finished_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5681 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/geolocation_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      944 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2790 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/geolocation_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1857 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4345 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/coordinate.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4015 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/speed.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3903 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/heading.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3853 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/altitude.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4153 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/location_services.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1873 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/access.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/messaging/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      679 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/messaging/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4734 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/messaging/message_received_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      707 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2260 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/purchase_result.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3256 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/in_skill_product.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      780 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2784 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/video_app_interface.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3221 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3450 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/video_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3533 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/launch_directive.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5810 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/start_input_handler_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      822 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5713 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/input_handler_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3608 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/stop_input_handler_directive.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4069 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/resolution.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      818 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3408 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2040 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/status_code.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3335 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/value_wrapper.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3485 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/value.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4048 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/resolutions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6563 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/intent_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1807 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/permission_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3426 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/application.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5126 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/permissions.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/__init__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5702 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission_changed_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4174 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_body.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7115 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/account_linked_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1288 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3393 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission_body.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3064 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/account_linked_body.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5202 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/skill_enabled_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5206 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/skill_disabled_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3062 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/proactive_subscription_event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2981 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5706 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission_accepted_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5931 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1902 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slot_confirmation_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1631 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5599 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/slot.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1909 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/intent_confirmation_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6388 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/supported_interfaces.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      960 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4154 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_slot.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4938 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_intent.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6359 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_intent_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2462 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_intent_values.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2465 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_understand_slot_values.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2302 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_slot_values.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      957 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/__version__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3908 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/session_ended_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5338 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7864 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4983 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/device.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1929 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/session_ended_reason.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4857 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/user.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3508 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/scope.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2329 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4601 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/launch_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5573 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/session.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4056 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/response_envelope.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3026 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/link_account_card.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3737 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/plain_text_output_speech.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3245 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/reprompt.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1084 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3717 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/ssml_output_speech.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3766 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/standard_card.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4514 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/output_speech.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3381 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/image.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4382 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/card.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1926 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/play_behavior.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3377 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/ask_for_permissions_consent_card.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3452 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/ui/simple_card.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      806 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4114 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/animation_step.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4815 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/light_animation.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2085 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/trigger_event_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4465 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/set_light_parameters.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8519 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/base_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1762 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/api_client_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3375 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3282 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/speak_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4502 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/directive_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      865 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/header.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3908 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/send_directive_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3878 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/directive/directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4665 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/service_client_factory.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1169 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1499 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/api_client.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5032 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_deleted_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6402 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4889 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_started_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3291 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6487 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/get_reminder_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3367 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/alert_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5240 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/trigger.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5053 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1856 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4119 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/get_reminders_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4889 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_updated_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4913 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_status_changed_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1772 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/recurrence_freq.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3637 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/spoken_text.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3400 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/alert_info_spoken_info.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1751 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4389 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/recurrence.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1833 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/recurrence_day.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3097 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_deleted_event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/push_notification_status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1856 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/trigger_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4889 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_created_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4949 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3489 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3528 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/push_notification.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    16534 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_management_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1516 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/serializer.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5168 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/address.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3458 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7740 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/device_address_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      782 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3327 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/short_address.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2446 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/api_configuration.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3473 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1750 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/distance_units.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      852 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2317 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/error_code.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    20764 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/ups_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3335 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/phone_number.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1763 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/ups/temperature_unit.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3401 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7978 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/lwa_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      823 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4104 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/access_token_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3840 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/access_token_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2045 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/access_token.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3099 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2153 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/product_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4036 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/in_skill_products_response.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      987 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2085 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/purchasable_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7363 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/in_skill_product.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10442 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/monetization_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1998 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/purchase_mode.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2043 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/entitled_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1688 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/service_client_response.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3195 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4017 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/relevant_audience.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1973 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/relevant_audience_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      955 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6182 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/create_proactive_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1894 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/skill_stage.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6322 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/proactive_events_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3397 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1941 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/service_exception.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4358 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/progress_recognizer.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3772 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/deviation_recognizer.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5087 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/input_event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1133 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1835 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/input_event_action_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2105 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/event_reporting_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6041 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/pattern_recognizer.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2214 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/pattern_recognizer_anchor_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3915 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/input_handler_event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4722 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/recognizer.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6884 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/event.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4867 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/pattern.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1871 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/api_client_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1494 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/api_client_message.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1362 2019-03-13 23:17:02.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/authentication_configuration.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3009 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/forbidden_error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5722 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_items_deleted_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2996 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_body.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3258 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/error.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4422 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_list_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5666 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_created_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    30771 2019-03-13 23:17:43.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_management_service_client.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5722 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_items_created_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1781 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4749 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_list_item.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1742 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1753 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_item_state.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3323 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_item_body.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5666 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_updated_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3683 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/update_list_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5722 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_items_updated_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5666 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_deleted_event_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3467 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/status.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3449 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/create_list_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2961 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/links.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4852 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_list.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3517 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/create_list_item_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3347 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_lists_metadata.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3861 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/update_list_item_request.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-13 23:18:44.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3468 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog/delegate_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3792 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog/confirm_slot_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3778 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog/elicit_slot_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      841 2019-03-13 23:18:20.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3488 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/dialog/confirm_intent_directive.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    16001 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6588 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/session_ended_request.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6747 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/context.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5329 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/request_envelope.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1986 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/session_ended_error_type.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4404 2019-03-13 23:17:42.000000 ask-sdk-model-1.8.0/ask_sdk_model/intent.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2791 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       97 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/requirements.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/setup.cfg
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       81 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/MANIFEST.in
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      982 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/README.rst
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    20685 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/SOURCES.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/dependency_links.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       14 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/top_level.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/not-zip-safe
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5904 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       52 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model.egg-info/requires.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      544 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/LICENSE
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5904 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2113 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/setup.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/gadget_controller/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      669 2019-03-28 17:47:33.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/gadget_controller/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4759 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/gadget_controller/set_light_directive.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      740 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7487 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/charge_amazon_pay_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8335 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/setup_amazon_pay_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4198 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3789 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      890 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7159 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3621 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/amazon_pay_error_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8069 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:33.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2086 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/payment_action.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4173 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/price.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1101 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6171 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_order_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6476 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/base_amazon_pay_entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7833 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/authorize_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4690 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6130 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/billing_agreement_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4331 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_credit.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5999 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_billing_agreement_attributes.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2086 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/payment_action.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3516 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/price.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2026 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10028 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6366 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5173 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1393 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1830 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/release_environment.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5498 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_order_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7301 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/destination.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2110 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7144 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorize_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4003 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5427 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3652 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_credit.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5304 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_billing_agreement_attributes.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3609 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/price.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2001 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    11066 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7159 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/billing_agreement_details.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5328 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      930 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1751 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/release_environment.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7274 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/destination.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4417 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/charge_amazon_pay_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3813 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/setup_amazon_pay_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      798 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3761 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/amazon_pay_error_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:33.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1825 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/position.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5802 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/user_event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4646 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/render_document_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5530 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/auto_page_command.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1153 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6361 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/speak_item_command.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1851 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/align.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1837 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/highlight_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3232 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/runtime.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4404 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/execute_commands_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5806 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/command.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5565 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/set_page_command.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3303 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/alexa_presentation_apl_interface.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/automotive/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      664 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/automotive/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2926 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/automotive/automotive_state.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1762 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/touch.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1766 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/shape.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      776 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1830 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/keyboard.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7681 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/viewport_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4949 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/experience.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4186 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/text_content.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1757 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/back_button_behavior.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5045 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/list_template2.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1587 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4012 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/text_field.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3850 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/hint.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4880 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template7.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3404 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/hint_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3528 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/render_template_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5862 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/template.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3904 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/list_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1826 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/image_size.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3240 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/plain_text.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4656 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/element_selected_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5045 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/list_template1.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5068 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template1.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2985 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/display_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5407 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template2.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3236 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/rich_text.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3630 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/image.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3405 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/display_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3236 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/plain_text_hint.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5407 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template3.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3973 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/image_instance.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5193 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template6.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3030 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/error_cause.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5302 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/exception_encountered_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3480 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4460 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/system_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      822 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1904 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/error_type.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      890 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5638 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/connections_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4382 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/base_entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      731 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4768 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/postal_address.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4184 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/restaurant.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3837 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/connections_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4275 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/send_response_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5415 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/send_request_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6308 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/connections_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4219 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/print_pdf_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      993 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4790 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/schedule_food_establishment_reservation_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4528 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/print_image_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5355 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/schedule_taxi_reservation_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5454 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/base_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4243 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/print_web_page_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4461 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/play_command_issued_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      892 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4477 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/previous_command_issued_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4461 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/next_command_issued_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4465 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/pause_command_issued_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2790 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_player_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5046 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_finished_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3037 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/stop_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1899 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/player_activity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3500 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3640 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/clear_queue_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3941 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/stream.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3975 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_player_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1777 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/clear_behavior.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5799 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_failed_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5042 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_stopped_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1537 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3983 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/current_playback_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4102 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/play_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2165 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/error_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3762 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4503 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_item_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/play_behavior.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5042 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_started_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5070 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_nearly_finished_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5681 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/geolocation_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      944 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2790 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/geolocation_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1857 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4345 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/coordinate.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4015 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/speed.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3903 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/heading.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3853 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/altitude.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4153 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/location_services.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1873 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/access.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/messaging/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      679 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/messaging/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4734 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/messaging/message_received_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      707 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2260 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/purchase_result.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3256 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/in_skill_product.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      780 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2784 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/video_app_interface.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3221 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3450 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/video_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3533 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/launch_directive.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5810 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/start_input_handler_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      822 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5713 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/input_handler_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3608 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/stop_input_handler_directive.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4069 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/resolution.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      818 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3408 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2040 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/status_code.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3335 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/value_wrapper.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3485 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/value.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4048 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/resolutions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6563 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/intent_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1807 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/permission_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3426 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/application.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5126 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/permissions.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/__init__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5702 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission_changed_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4174 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_body.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7115 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/account_linked_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1288 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3393 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission_body.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3064 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/account_linked_body.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5202 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/skill_enabled_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5206 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/skill_disabled_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3062 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/proactive_subscription_event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2981 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5706 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission_accepted_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5931 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1902 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slot_confirmation_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1631 2019-03-28 17:47:33.000000 ask-sdk-model-1.9.0/ask_sdk_model/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5599 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/slot.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1909 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/intent_confirmation_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6388 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/supported_interfaces.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      960 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4154 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_slot.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4938 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_intent.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6359 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_intent_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2462 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_intent_values.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2465 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_understand_slot_values.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2302 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_slot_values.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      957 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/__version__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/dynamic/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      796 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/dynamic/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3498 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/dynamic/entity_value_and_synonyms.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/dynamic/update_behavior.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3764 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/dynamic/entity_list_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3802 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/dynamic/entity.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      618 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/er/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3908 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/session_ended_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5338 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8116 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4983 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/device.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1929 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/session_ended_reason.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4857 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/user.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3508 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/scope.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2329 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4601 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/launch_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5573 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/session.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4056 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/response_envelope.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3026 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/link_account_card.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3737 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/plain_text_output_speech.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3245 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/reprompt.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1084 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3717 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/ssml_output_speech.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3766 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/standard_card.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4514 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/output_speech.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3381 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/image.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4382 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/card.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1926 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/play_behavior.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3377 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/ask_for_permissions_consent_card.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3452 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/ui/simple_card.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      806 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4114 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/animation_step.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4815 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/light_animation.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2085 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/trigger_event_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4465 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/set_light_parameters.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8519 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/base_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1762 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/api_client_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3375 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3282 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/speak_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4502 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/directive_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      865 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3180 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/header.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3908 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/send_directive_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3878 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/directive/directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4665 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/service_client_factory.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1169 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1499 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/api_client.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5032 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_deleted_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6402 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4889 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_started_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3291 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6487 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/get_reminder_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3367 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/alert_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5240 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/trigger.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5053 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1856 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4119 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/get_reminders_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4889 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_updated_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4913 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_status_changed_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1772 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/recurrence_freq.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3637 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/spoken_text.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3400 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/alert_info_spoken_info.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1751 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4389 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/recurrence.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1833 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/recurrence_day.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3097 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_deleted_event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1820 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/push_notification_status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1856 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/trigger_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4889 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_created_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4949 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3489 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3528 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/push_notification.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    16534 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_management_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1516 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/serializer.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5168 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/address.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3458 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7740 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/device_address_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      782 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3327 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/short_address.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2446 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/api_configuration.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3473 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1750 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/distance_units.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      852 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2317 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/error_code.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    20764 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/ups_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3335 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/phone_number.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1763 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/ups/temperature_unit.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3401 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7978 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/lwa_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      823 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4104 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/access_token_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3840 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/access_token_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2045 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/access_token.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3099 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2153 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/product_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4036 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/in_skill_products_response.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2184 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/entitlement_reason.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1037 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2085 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/purchasable_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8016 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/in_skill_product.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    10442 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/monetization_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1998 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/purchase_mode.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2043 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/entitled_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1688 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/service_client_response.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3195 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4017 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/relevant_audience.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1973 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/relevant_audience_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      955 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6182 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/create_proactive_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1894 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/skill_stage.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6322 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/proactive_events_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3397 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1941 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/service_exception.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4358 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/progress_recognizer.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3772 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/deviation_recognizer.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5087 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/input_event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1133 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1835 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/input_event_action_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2105 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/event_reporting_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6041 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/pattern_recognizer.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2214 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/pattern_recognizer_anchor_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3915 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/input_handler_event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4722 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/recognizer.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6884 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/event.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4867 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/pattern.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1871 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/api_client_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1494 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/api_client_message.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1362 2019-03-28 17:46:16.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/authentication_configuration.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3009 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/forbidden_error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5722 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_items_deleted_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2996 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_body.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3258 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/error.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4422 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_list_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5666 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_created_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    30771 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_management_service_client.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5722 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_items_created_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1781 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4749 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_list_item.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1742 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1753 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_item_state.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3323 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_item_body.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5666 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_updated_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3683 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/update_list_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5722 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_items_updated_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5666 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_deleted_event_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3467 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/status.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3449 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/create_list_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2961 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/links.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4852 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_list.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3517 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/create_list_item_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3347 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_lists_metadata.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3861 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/update_list_item_request.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-28 17:47:57.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3468 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/delegate_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3792 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/confirm_slot_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3778 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/elicit_slot_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      906 2019-03-28 17:47:34.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3488 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/confirm_intent_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4113 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/dialog/dynamic_entities_directive.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    16001 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6588 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/session_ended_request.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6747 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/context.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5329 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/request_envelope.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1986 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/session_ended_error_type.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4404 2019-03-28 17:46:56.000000 ask-sdk-model-1.9.0/ask_sdk_model/intent.py
```

### Comparing `ask-sdk-model-1.8.0/CHANGELOG.rst` & `ask-sdk-model-1.9.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -120,7 +120,16 @@
 
 1.8.0
 ~~~~~~~
 
 This release contains the following :
 Introduces support for customizing your skill’s experience for Echo Auto, which is now shipping to select customers via our invite program, and vehicles and other aftermarket devices that support Alexa Auto. 
 The automotive experience introduces another way for customers to interact with skills, while they are on-the-go and their attention is on the road. Now you can adapt your skill experience to be succinct, location-aware, and adaptive to your customer’s needs while they’re outside the home.
+
+
+1.9.0
+~~~~~~~
+
+This release contains the following changes : 
+
+- Dynamic entities for customized interactions
+- Add additional 'entitlementReason' field in In-Skill products
```

### Comparing `ask-sdk-model-1.8.0/README.rst` & `ask-sdk-model-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model.egg-info/SOURCES.txt` & `ask-sdk-model-1.9.0/ask_sdk_model.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,22 @@
 ask_sdk_model/canfulfill/can_fulfill_slot.py
 ask_sdk_model/canfulfill/can_fulfill_slot_values.py
 ask_sdk_model/canfulfill/can_understand_slot_values.py
 ask_sdk_model/dialog/__init__.py
 ask_sdk_model/dialog/confirm_intent_directive.py
 ask_sdk_model/dialog/confirm_slot_directive.py
 ask_sdk_model/dialog/delegate_directive.py
+ask_sdk_model/dialog/dynamic_entities_directive.py
 ask_sdk_model/dialog/elicit_slot_directive.py
+ask_sdk_model/er/__init__.py
+ask_sdk_model/er/dynamic/__init__.py
+ask_sdk_model/er/dynamic/entity.py
+ask_sdk_model/er/dynamic/entity_list_item.py
+ask_sdk_model/er/dynamic/entity_value_and_synonyms.py
+ask_sdk_model/er/dynamic/update_behavior.py
 ask_sdk_model/events/__init__.py
 ask_sdk_model/events/skillevents/__init__.py
 ask_sdk_model/events/skillevents/account_linked_body.py
 ask_sdk_model/events/skillevents/account_linked_request.py
 ask_sdk_model/events/skillevents/permission.py
 ask_sdk_model/events/skillevents/permission_accepted_request.py
 ask_sdk_model/events/skillevents/permission_body.py
@@ -305,14 +312,15 @@
 ask_sdk_model/services/lwa/access_token.py
 ask_sdk_model/services/lwa/access_token_request.py
 ask_sdk_model/services/lwa/access_token_response.py
 ask_sdk_model/services/lwa/error.py
 ask_sdk_model/services/lwa/lwa_client.py
 ask_sdk_model/services/monetization/__init__.py
 ask_sdk_model/services/monetization/entitled_state.py
+ask_sdk_model/services/monetization/entitlement_reason.py
 ask_sdk_model/services/monetization/error.py
 ask_sdk_model/services/monetization/in_skill_product.py
 ask_sdk_model/services/monetization/in_skill_products_response.py
 ask_sdk_model/services/monetization/monetization_service_client.py
 ask_sdk_model/services/monetization/product_type.py
 ask_sdk_model/services/monetization/purchasable_state.py
 ask_sdk_model/services/monetization/purchase_mode.py
```

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model.egg-info/PKG-INFO` & `ask-sdk-model-1.9.0/ask_sdk_model.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk-model
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK Model package provides model definitions, for building Alexa Skills.
 Home-page: https://github.com/alexa/alexa-apis-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ==============================================
         ASK SDK Model - Model definitions for ASK SDK
@@ -149,14 +149,23 @@
         1.8.0
         ~~~~~~~
         
         This release contains the following :
         Introduces support for customizing your skill’s experience for Echo Auto, which is now shipping to select customers via our invite program, and vehicles and other aftermarket devices that support Alexa Auto. 
         The automotive experience introduces another way for customers to interact with skills, while they are on-the-go and their attention is on the road. Now you can adapt your skill experience to be succinct, location-aware, and adaptive to your customer’s needs while they’re outside the home.
         
+        
+        1.9.0
+        ~~~~~~~
+        
+        This release contains the following changes : 
+        
+        - Dynamic entities for customized interactions
+        - Add additional 'entitlementReason' field in In-Skill products
+        
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,Models
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-model-1.8.0/LICENSE` & `ask-sdk-model-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/PKG-INFO` & `ask-sdk-model-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk-model
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK Model package provides model definitions, for building Alexa Skills.
 Home-page: https://github.com/alexa/alexa-apis-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ==============================================
         ASK SDK Model - Model definitions for ASK SDK
@@ -149,14 +149,23 @@
         1.8.0
         ~~~~~~~
         
         This release contains the following :
         Introduces support for customizing your skill’s experience for Echo Auto, which is now shipping to select customers via our invite program, and vehicles and other aftermarket devices that support Alexa Auto. 
         The automotive experience introduces another way for customers to interact with skills, while they are on-the-go and their attention is on the road. Now you can adapt your skill experience to be succinct, location-aware, and adaptive to your customer’s needs while they’re outside the home.
         
+        
+        1.9.0
+        ~~~~~~~
+        
+        This release contains the following changes : 
+        
+        - Dynamic entities for customized interactions
+        - Add additional 'entitlementReason' field in In-Skill products
+        
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,Models
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-model-1.8.0/setup.py` & `ask-sdk-model-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/gadget_controller/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/gadget_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/gadget_controller/set_light_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/gadget_controller/set_light_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/charge_amazon_pay_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/charge_amazon_pay_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/request/setup_amazon_pay_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/request/setup_amazon_pay_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay_result.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay_result.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay_result.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay_result.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/charge_amazon_pay.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/amazon_pay_error_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/amazon_pay_error_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/v1/setup_amazon_pay.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/payment_action.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/payment_action.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/price.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/price.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_order_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_order_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/base_amazon_pay_entity.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/base_amazon_pay_entity.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/authorize_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/authorize_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/billing_agreement_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/billing_agreement_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_credit.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/provider_credit.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_billing_agreement_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/request/seller_billing_agreement_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/payment_action.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/payment_action.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/price.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/price.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_details.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_details.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_details.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_details.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorization_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/release_environment.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/release_environment.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_order_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_order_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/destination.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/destination.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorize_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/authorize_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/billing_agreement_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_credit.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/provider_credit.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_billing_agreement_attributes.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/v1/seller_billing_agreement_attributes.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/price.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/price.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_details.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_details.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/billing_agreement_details.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/billing_agreement_details.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/authorization_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/release_environment.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/release_environment.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/model/response/destination.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/model/response/destination.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/charge_amazon_pay_result.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/charge_amazon_pay_result.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/setup_amazon_pay_result.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/setup_amazon_pay_result.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/amazonpay/response/amazon_pay_error_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/amazonpay/response/amazon_pay_error_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/position.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/position.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/user_event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/user_event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/render_document_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/render_document_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/auto_page_command.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/auto_page_command.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/speak_item_command.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/speak_item_command.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/align.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/align.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/highlight_mode.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/highlight_mode.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/runtime.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/runtime.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/execute_commands_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/execute_commands_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/command.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/command.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/set_page_command.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/set_page_command.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/alexa/presentation/apl/alexa_presentation_apl_interface.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/alexa/presentation/apl/alexa_presentation_apl_interface.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/automotive/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/automotive/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/automotive/automotive_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/automotive/automotive_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/touch.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/touch.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/shape.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/shape.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/keyboard.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/keyboard.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/viewport_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/viewport_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/viewport/experience.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/viewport/experience.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/text_content.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/text_content.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/back_button_behavior.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/back_button_behavior.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/list_template2.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/list_template2.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/text_field.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/text_field.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/hint.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/hint.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template7.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template7.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/hint_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/hint_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/render_template_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/render_template_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/template.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/template.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/list_item.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/list_item.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/image_size.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/image_size.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/plain_text.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/plain_text.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/element_selected_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/element_selected_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/list_template1.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/list_template1.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template1.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template1.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/display_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/display_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template2.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template2.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/rich_text.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/rich_text.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/image.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/image.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/display_interface.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/display_interface.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/plain_text_hint.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/plain_text_hint.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template3.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template3.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/image_instance.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/image_instance.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/display/body_template6.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/display/body_template6.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/error_cause.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/error_cause.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/exception_encountered_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/exception_encountered_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/system_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/system_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/system/error_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/system/error_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/connections_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/connections_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/base_entity.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/base_entity.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/postal_address.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/postal_address.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/entities/restaurant.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/entities/restaurant.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/connections_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/connections_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/send_response_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/send_response_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/send_request_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/send_request_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/connections_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/connections_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/print_pdf_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/print_pdf_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/schedule_food_establishment_reservation_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/schedule_food_establishment_reservation_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/print_image_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/print_image_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/schedule_taxi_reservation_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/schedule_taxi_reservation_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/base_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/base_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/connections/requests/print_web_page_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/connections/requests/print_web_page_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/play_command_issued_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/play_command_issued_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/previous_command_issued_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/previous_command_issued_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/next_command_issued_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/next_command_issued_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/playbackcontroller/pause_command_issued_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/playbackcontroller/pause_command_issued_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_player_interface.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_player_interface.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_finished_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_finished_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/stop_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/stop_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/player_activity.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/player_activity.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/clear_queue_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/clear_queue_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/stream.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/stream.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_player_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_player_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/clear_behavior.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/clear_behavior.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_failed_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_failed_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_stopped_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_stopped_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/current_playback_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/current_playback_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/play_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/play_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/error_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/error_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_item.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_item.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/audio_item_metadata.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/audio_item_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/play_behavior.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/play_behavior.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_started_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_started_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/audioplayer/playback_nearly_finished_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/audioplayer/playback_nearly_finished_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/geolocation_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/geolocation_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/geolocation_interface.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/geolocation_interface.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/coordinate.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/coordinate.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/speed.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/speed.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/heading.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/heading.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/altitude.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/altitude.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/location_services.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/location_services.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/geolocation/access.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/geolocation/access.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/messaging/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/messaging/message_received_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/messaging/message_received_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/purchase_result.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/purchase_result.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/v1/in_skill_product.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/v1/in_skill_product.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/monetization/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/monetization/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/video_app_interface.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/video_app_interface.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/metadata.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/metadata.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/video_item.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/video_item.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/videoapp/launch_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/videoapp/launch_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/start_input_handler_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/start_input_handler_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/input_handler_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/input_handler_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/interfaces/game_engine/stop_input_handler_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/interfaces/game_engine/stop_input_handler_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/resolution.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/resolution.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/status_code.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/status_code.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/value_wrapper.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/value_wrapper.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/value.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/value.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slu/entityresolution/resolutions.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slu/entityresolution/resolutions.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/intent_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/intent_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/permission_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/permission_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/application.py` & `ask-sdk-model-1.9.0/ask_sdk_model/application.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/permissions.py` & `ask-sdk-model-1.9.0/ask_sdk_model/permissions.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission_changed_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission_changed_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_body.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_body.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/account_linked_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/account_linked_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission_body.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission_body.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/account_linked_body.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/account_linked_body.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/skill_enabled_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/skill_enabled_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/skill_disabled_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/skill_disabled_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/proactive_subscription_event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/proactive_subscription_event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/permission_accepted_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/permission_accepted_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/events/skillevents/proactive_subscription_changed_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slot_confirmation_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slot_confirmation_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/slot.py` & `ask-sdk-model-1.9.0/ask_sdk_model/slot.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/intent_confirmation_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/intent_confirmation_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/supported_interfaces.py` & `ask-sdk-model-1.9.0/ask_sdk_model/supported_interfaces.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_slot.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_slot.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_intent.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_intent.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_intent_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_intent_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_intent_values.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_intent_values.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_understand_slot_values.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_understand_slot_values.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/canfulfill/can_fulfill_slot_values.py` & `ask-sdk-model-1.9.0/ask_sdk_model/canfulfill/can_fulfill_slot_values.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/__version__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for
 # the specific language governing permissions and limitations under the License.
 #
 
 __pip_package_name__ = 'ask-sdk-model'
 __description__ = 'The ASK SDK Model package provides model definitions, for building Alexa Skills.'
 __url__ = 'https://github.com/alexa/alexa-apis-for-python'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 __author__ = 'Alexa Skills Kit'
 __author_email__ = 'ask-sdk-dynamic@amazon.com'
 __license__ = 'Apache 2.0'
 __keywords__ = ['ASK SDK', 'Alexa Skills Kit', 'Alexa', 'Models']
```

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/session_ended_error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/session_ended_error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/directive.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         |
         | AudioPlayer.Play: :py:class:`ask_sdk_model.interfaces.audioplayer.play_directive.PlayDirective`,
         |
         | Alexa.Presentation.APL.ExecuteCommands: :py:class:`ask_sdk_model.interfaces.alexa.presentation.apl.execute_commands_directive.ExecuteCommandsDirective`,
         |
         | Connections.SendRequest: :py:class:`ask_sdk_model.interfaces.connections.send_request_directive.SendRequestDirective`,
         |
+        | Dialog.UpdateDynamicEntities: :py:class:`ask_sdk_model.dialog.dynamic_entities_directive.DynamicEntitiesDirective`,
+        |
         | Display.RenderTemplate: :py:class:`ask_sdk_model.interfaces.display.render_template_directive.RenderTemplateDirective`,
         |
         | GadgetController.SetLight: :py:class:`ask_sdk_model.interfaces.gadget_controller.set_light_directive.SetLightDirective`,
         |
         | Dialog.Delegate: :py:class:`ask_sdk_model.dialog.delegate_directive.DelegateDirective`,
         |
         | Hint: :py:class:`ask_sdk_model.interfaces.display.hint_directive.HintDirective`,
@@ -82,14 +84,15 @@
 
     discriminator_value_class_map = {
         'AudioPlayer.Stop': 'ask_sdk_model.interfaces.audioplayer.stop_directive.StopDirective',
         'Dialog.ConfirmSlot': 'ask_sdk_model.dialog.confirm_slot_directive.ConfirmSlotDirective',
         'AudioPlayer.Play': 'ask_sdk_model.interfaces.audioplayer.play_directive.PlayDirective',
         'Alexa.Presentation.APL.ExecuteCommands': 'ask_sdk_model.interfaces.alexa.presentation.apl.execute_commands_directive.ExecuteCommandsDirective',
         'Connections.SendRequest': 'ask_sdk_model.interfaces.connections.send_request_directive.SendRequestDirective',
+        'Dialog.UpdateDynamicEntities': 'ask_sdk_model.dialog.dynamic_entities_directive.DynamicEntitiesDirective',
         'Display.RenderTemplate': 'ask_sdk_model.interfaces.display.render_template_directive.RenderTemplateDirective',
         'GadgetController.SetLight': 'ask_sdk_model.interfaces.gadget_controller.set_light_directive.SetLightDirective',
         'Dialog.Delegate': 'ask_sdk_model.dialog.delegate_directive.DelegateDirective',
         'Hint': 'ask_sdk_model.interfaces.display.hint_directive.HintDirective',
         'Dialog.ConfirmIntent': 'ask_sdk_model.dialog.confirm_intent_directive.ConfirmIntentDirective',
         'GameEngine.StartInputHandler': 'ask_sdk_model.interfaces.game_engine.start_input_handler_directive.StartInputHandlerDirective',
         'VideoApp.Launch': 'ask_sdk_model.interfaces.videoapp.launch_directive.LaunchDirective',
```

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/device.py` & `ask-sdk-model-1.9.0/ask_sdk_model/device.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/session_ended_reason.py` & `ask-sdk-model-1.9.0/ask_sdk_model/session_ended_reason.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/user.py` & `ask-sdk-model-1.9.0/ask_sdk_model/user.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/scope.py` & `ask-sdk-model-1.9.0/ask_sdk_model/scope.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/dialog_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/dialog_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/launch_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/launch_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/session.py` & `ask-sdk-model-1.9.0/ask_sdk_model/session.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/response_envelope.py` & `ask-sdk-model-1.9.0/ask_sdk_model/response_envelope.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/link_account_card.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/link_account_card.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/plain_text_output_speech.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/plain_text_output_speech.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/reprompt.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/reprompt.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/ssml_output_speech.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/ssml_output_speech.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/standard_card.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/standard_card.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/output_speech.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/output_speech.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/image.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/image.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/card.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/card.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/play_behavior.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/play_behavior.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/ask_for_permissions_consent_card.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/ask_for_permissions_consent_card.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/ui/simple_card.py` & `ask-sdk-model-1.9.0/ask_sdk_model/ui/simple_card.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/animation_step.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/animation_step.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/light_animation.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/light_animation.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/trigger_event_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/trigger_event_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/gadget_controller/set_light_parameters.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/gadget_controller/set_light_parameters.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/base_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/base_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/api_client_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/api_client_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/speak_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/speak_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/directive_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/directive_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/header.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/header.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/send_directive_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/send_directive_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/directive/directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/directive/directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/service_client_factory.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/service_client_factory.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/api_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/api_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_deleted_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_deleted_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_started_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_started_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/get_reminder_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/get_reminder_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/alert_info.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/alert_info.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/trigger.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/trigger.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/get_reminders_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/get_reminders_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_updated_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_updated_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_status_changed_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_status_changed_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/recurrence_freq.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/recurrence_freq.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/spoken_text.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/spoken_text.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/alert_info_spoken_info.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/alert_info_spoken_info.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/recurrence.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/recurrence.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/recurrence_day.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/recurrence_day.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_deleted_event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_deleted_event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/push_notification_status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/push_notification_status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/trigger_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/trigger_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_created_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_created_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/push_notification.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/push_notification.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/reminder_management/reminder_management_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/reminder_management/reminder_management_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/serializer.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/serializer.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/address.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/address.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/device_address_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/device_address_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/device_address/short_address.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/device_address/short_address.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/api_configuration.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/api_configuration.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/distance_units.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/distance_units.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/error_code.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/error_code.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/ups_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/ups_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/phone_number.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/phone_number.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/ups/temperature_unit.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/ups/temperature_unit.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/lwa_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/lwa_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/access_token_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/access_token_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/access_token_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/access_token_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/lwa/access_token.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/lwa/access_token.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/product_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/product_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/in_skill_products_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/in_skill_products_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 # the specific language governing permissions and limitations under the License.
 #
 from __future__ import absolute_import
 
 from .error import Error
 from .product_type import ProductType
 from .in_skill_products_response import InSkillProductsResponse
+from .entitlement_reason import EntitlementReason
 from .purchasable_state import PurchasableState
 from .in_skill_product import InSkillProduct
 from .monetization_service_client import MonetizationServiceClient
 from .purchase_mode import PurchaseMode
 from .entitled_state import EntitledState
```

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/purchasable_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/purchasable_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/in_skill_product.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/in_skill_product.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 if typing.TYPE_CHECKING:
     from typing import Dict, List, Optional
     from datetime import datetime
     from ask_sdk_model.services.monetization.purchasable_state import PurchasableState
     from ask_sdk_model.services.monetization.purchase_mode import PurchaseMode
     from ask_sdk_model.services.monetization.entitled_state import EntitledState
     from ask_sdk_model.services.monetization.product_type import ProductType
+    from ask_sdk_model.services.monetization.entitlement_reason import EntitlementReason
 
 
 class InSkillProduct(object):
     """
 
     :param product_id: Product Id
     :type product_id: (optional) str
@@ -42,46 +43,50 @@
     :type object_type: (optional) ask_sdk_model.services.monetization.product_type.ProductType
     :param summary: Product summary in the language from the \&quot;Accept-Language\&quot; header
     :type summary: (optional) str
     :param purchasable: 
     :type purchasable: (optional) ask_sdk_model.services.monetization.purchasable_state.PurchasableState
     :param entitled: 
     :type entitled: (optional) ask_sdk_model.services.monetization.entitled_state.EntitledState
+    :param entitlement_reason: 
+    :type entitlement_reason: (optional) ask_sdk_model.services.monetization.entitlement_reason.EntitlementReason
     :param active_entitlement_count: Total active purchases of the product made by the user. Note - For ENTITLEMENT and SUBSCRIPTION product types, the value is either zero(NOT_ENTITLED) or one(ENTITLED). For CONSUMABLE product type the value is zero or more, as CONSUMABLE can be re-purchased.
     :type active_entitlement_count: (optional) int
     :param purchase_mode: 
     :type purchase_mode: (optional) ask_sdk_model.services.monetization.purchase_mode.PurchaseMode
 
     """
     deserialized_types = {
         'product_id': 'str',
         'reference_name': 'str',
         'name': 'str',
         'object_type': 'ask_sdk_model.services.monetization.product_type.ProductType',
         'summary': 'str',
         'purchasable': 'ask_sdk_model.services.monetization.purchasable_state.PurchasableState',
         'entitled': 'ask_sdk_model.services.monetization.entitled_state.EntitledState',
+        'entitlement_reason': 'ask_sdk_model.services.monetization.entitlement_reason.EntitlementReason',
         'active_entitlement_count': 'int',
         'purchase_mode': 'ask_sdk_model.services.monetization.purchase_mode.PurchaseMode'
     }
 
     attribute_map = {
         'product_id': 'productId',
         'reference_name': 'referenceName',
         'name': 'name',
         'object_type': 'type',
         'summary': 'summary',
         'purchasable': 'purchasable',
         'entitled': 'entitled',
+        'entitlement_reason': 'entitlementReason',
         'active_entitlement_count': 'activeEntitlementCount',
         'purchase_mode': 'purchaseMode'
     }
 
-    def __init__(self, product_id=None, reference_name=None, name=None, object_type=None, summary=None, purchasable=None, entitled=None, active_entitlement_count=None, purchase_mode=None):
-        # type: (Optional[str], Optional[str], Optional[str], Optional[ProductType], Optional[str], Optional[PurchasableState], Optional[EntitledState], Optional[int], Optional[PurchaseMode]) -> None
+    def __init__(self, product_id=None, reference_name=None, name=None, object_type=None, summary=None, purchasable=None, entitled=None, entitlement_reason=None, active_entitlement_count=None, purchase_mode=None):
+        # type: (Optional[str], Optional[str], Optional[str], Optional[ProductType], Optional[str], Optional[PurchasableState], Optional[EntitledState], Optional[EntitlementReason], Optional[int], Optional[PurchaseMode]) -> None
         """
 
         :param product_id: Product Id
         :type product_id: (optional) str
         :param reference_name: Developer selected in-skill product name. This is for developer reference only.
         :type reference_name: (optional) str
         :param name: Name of the product in the language from the \&quot;Accept-Language\&quot; header
@@ -90,28 +95,31 @@
         :type object_type: (optional) ask_sdk_model.services.monetization.product_type.ProductType
         :param summary: Product summary in the language from the \&quot;Accept-Language\&quot; header
         :type summary: (optional) str
         :param purchasable: 
         :type purchasable: (optional) ask_sdk_model.services.monetization.purchasable_state.PurchasableState
         :param entitled: 
         :type entitled: (optional) ask_sdk_model.services.monetization.entitled_state.EntitledState
+        :param entitlement_reason: 
+        :type entitlement_reason: (optional) ask_sdk_model.services.monetization.entitlement_reason.EntitlementReason
         :param active_entitlement_count: Total active purchases of the product made by the user. Note - For ENTITLEMENT and SUBSCRIPTION product types, the value is either zero(NOT_ENTITLED) or one(ENTITLED). For CONSUMABLE product type the value is zero or more, as CONSUMABLE can be re-purchased.
         :type active_entitlement_count: (optional) int
         :param purchase_mode: 
         :type purchase_mode: (optional) ask_sdk_model.services.monetization.purchase_mode.PurchaseMode
         """
         self.__discriminator_value = None
 
         self.product_id = product_id
         self.reference_name = reference_name
         self.name = name
         self.object_type = object_type
         self.summary = summary
         self.purchasable = purchasable
         self.entitled = entitled
+        self.entitlement_reason = entitlement_reason
         self.active_entitlement_count = active_entitlement_count
         self.purchase_mode = purchase_mode
 
     def to_dict(self):
         # type: () -> Dict[str, object]
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/monetization_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/monetization_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/purchase_mode.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/purchase_mode.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/monetization/entitled_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/monetization/entitled_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/service_client_response.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/service_client_response.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/relevant_audience.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/relevant_audience.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/relevant_audience_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/relevant_audience_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/create_proactive_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/create_proactive_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/skill_stage.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/skill_stage.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/proactive_events_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/proactive_events_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/proactive_events/event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/proactive_events/event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/service_exception.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/service_exception.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/progress_recognizer.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/progress_recognizer.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/deviation_recognizer.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/deviation_recognizer.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/input_event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/input_event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/input_event_action_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/input_event_action_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/event_reporting_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/event_reporting_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/pattern_recognizer.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/pattern_recognizer.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/pattern_recognizer_anchor_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/pattern_recognizer_anchor_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/input_handler_event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/input_handler_event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/recognizer.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/recognizer.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/event.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/event.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/game_engine/pattern.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/game_engine/pattern.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/api_client_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/api_client_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/api_client_message.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/api_client_message.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/authentication_configuration.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/authentication_configuration.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/forbidden_error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/forbidden_error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_items_deleted_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_items_deleted_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_body.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_body.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/error.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/error.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_list_metadata.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_list_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_created_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_created_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_management_service_client.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_management_service_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_items_created_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_items_created_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_list_item.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_list_item.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_item_state.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_item_state.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_item_body.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_item_body.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_updated_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_updated_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/update_list_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/update_list_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_items_updated_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_items_updated_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/list_deleted_event_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/list_deleted_event_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/status.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/status.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/create_list_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/create_list_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/links.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/links.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_list.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_list.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/create_list_item_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/create_list_item_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/alexa_lists_metadata.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/alexa_lists_metadata.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/services/list_management/update_list_item_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/services/list_management/update_list_item_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/dialog/delegate_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/dialog/delegate_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/dialog/confirm_slot_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/dialog/confirm_slot_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/dialog/elicit_slot_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/dialog/elicit_slot_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/dialog/__init__.py` & `ask-sdk-model-1.9.0/ask_sdk_model/dialog/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 #
 from __future__ import absolute_import
 
 from .delegate_directive import DelegateDirective
 from .confirm_slot_directive import ConfirmSlotDirective
 from .elicit_slot_directive import ElicitSlotDirective
 from .confirm_intent_directive import ConfirmIntentDirective
+from .dynamic_entities_directive import DynamicEntitiesDirective
```

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/dialog/confirm_intent_directive.py` & `ask-sdk-model-1.9.0/ask_sdk_model/dialog/confirm_intent_directive.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/session_ended_request.py` & `ask-sdk-model-1.9.0/ask_sdk_model/session_ended_request.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/context.py` & `ask-sdk-model-1.9.0/ask_sdk_model/context.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/request_envelope.py` & `ask-sdk-model-1.9.0/ask_sdk_model/request_envelope.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/session_ended_error_type.py` & `ask-sdk-model-1.9.0/ask_sdk_model/session_ended_error_type.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-model-1.8.0/ask_sdk_model/intent.py` & `ask-sdk-model-1.9.0/ask_sdk_model/intent.py`

 * *Files identical despite different names*

