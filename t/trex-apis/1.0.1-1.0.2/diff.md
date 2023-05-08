# Comparing `tmp/trex-apis-1.0.1.tar.gz` & `tmp/trex-apis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.1.tar", last modified: Fri Apr 28 10:20:58 2023, max compression
+gzip compressed data, was "trex-apis-1.0.2.tar", last modified: Mon May  8 02:59:42 2023, max compression
```

## Comparing `trex-apis-1.0.1.tar` & `trex-apis-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.080119 trex-apis-1.0.1/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-28 10:20:58.080278 trex-apis-1.0.1/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.1/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-28 10:20:58.080863 trex-apis-1.0.1/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-04-28 10:15:51.000000 trex-apis-1.0.1/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.056928 trex-apis-1.0.1/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1283 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.057376 trex-apis-1.0.1/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.1/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.1/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.071145 trex-apis-1.0.1/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.1/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11544 2023-04-24 08:15:59.000000 trex-apis-1.0.1/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.1/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35834 2023-04-25 09:25:42.000000 trex-apis-1.0.1/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.1/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.1/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12965 2023-03-24 05:50:51.000000 trex-apis-1.0.1/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11098 2023-04-24 10:10:40.000000 trex-apis-1.0.1/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.1/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.1/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.1/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.1/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.1/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36081 2023-04-03 08:51:30.000000 trex-apis-1.0.1/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.1/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.1/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.072252 trex-apis-1.0.1/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.1/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4555 2023-04-18 09:35:03.000000 trex-apis-1.0.1/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.075430 trex-apis-1.0.1/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.1/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.1/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.1/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.1/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-1.0.1/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.076455 trex-apis-1.0.1/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.1/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.1/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.078380 trex-apis-1.0.1/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.1/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.1/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.1/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.400350 trex-apis-1.0.2/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-08 02:59:42.400508 trex-apis-1.0.2/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.2/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-08 02:59:42.401034 trex-apis-1.0.2/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-05-08 02:59:25.000000 trex-apis-1.0.2/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.371375 trex-apis-1.0.2/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1328 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.371975 trex-apis-1.0.2/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.2/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.2/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.390752 trex-apis-1.0.2/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.2/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11544 2023-04-24 08:15:59.000000 trex-apis-1.0.2/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.2/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-05 09:27:49.000000 trex-apis-1.0.2/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.2/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.2/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12965 2023-03-24 05:50:51.000000 trex-apis-1.0.2/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1214 2023-05-07 13:49:51.000000 trex-apis-1.0.2/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-05 09:32:39.000000 trex-apis-1.0.2/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.2/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.2/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.2/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.2/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.2/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36081 2023-04-03 08:51:30.000000 trex-apis-1.0.2/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.2/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.2/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.392060 trex-apis-1.0.2/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.2/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4734 2023-05-05 09:06:37.000000 trex-apis-1.0.2/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.395362 trex-apis-1.0.2/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.2/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.2/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.2/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.2/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-1.0.2/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.396583 trex-apis-1.0.2/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.2/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.2/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.398606 trex-apis-1.0.2/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.2/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.2/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.2/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.1/setup.py` & `trex-apis-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.1',
+     version='1.0.2',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.1/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.2/trex_apis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 trexapi/controllers/__init__.py
 trexapi/controllers/api_routes.py
 trexapi/controllers/app_api_routes.py
 trexapi/controllers/customer_api_routes.py
 trexapi/controllers/customer_membership_api_routes.py
 trexapi/controllers/customer_reward_api_routes.py
 trexapi/controllers/loyalty_api_routes.py
+trexapi/controllers/lucky_draw_api_routes.py
 trexapi/controllers/outlet_api_routes.py
 trexapi/controllers/payment_api_routes.py
 trexapi/controllers/pos_api_routes.py
 trexapi/controllers/reward_api_routes.py
 trexapi/controllers/sales_api_routes.py
 trexapi/controllers/transaction_api_routes.py
 trexapi/controllers/user_api_routes.py
```

### Comparing `trex-apis-1.0.1/trexapi/conf.py` & `trex-apis-1.0.2/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/customer_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 from trexlib.utils.log_util import get_tracelog
 from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 from flask.json import jsonify
 from datetime import datetime
 from trexapi.decorators.api_decorators import auth_token_required,\
-    outlet_key_required
+    outlet_key_required, test_session_expired
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.user_models import User
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from trexmodel.models.datastore.merchant_models import Outlet,\
@@ -412,15 +412,16 @@
         else:
             return create_rest_message(gettext('Customer is not exist'), status_code=StatusCode.BAD_REQUEST)
     else:
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
 
 
 @customer_api_bp.route('/search/<limit>', methods=['POST'])
-#@auth_token_required
+@auth_token_required
+#@test_session_expired
 def search_customer(limit):
     
     search_member_data_in_json   = request.get_json()
     search_customer_form         = CustomerSearchForm(ImmutableMultiDict(search_member_data_in_json))
     
     logger.debug('search_member_data_in_json=%s', search_member_data_in_json)
     
@@ -471,14 +472,15 @@
         #return create_rest_message(status_code=StatusCode.OK, customer_list=customer_list)
         return jsonify(customer_list)
     else:
         return create_rest_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
 
 @customer_api_bp.route('/reference-code/<reference_code>/list-membership', methods=['GET'])
 @auth_token_required
+#@test_session_expired
 def list_customer_membership(reference_code):
     if is_not_empty(reference_code):
         acct_id   = request.headers.get('x-acct-id')
         db_client = create_db_client(caller_info="list_customer_membership")
         customer_membership_final_list = []
         
         logger.debug('reference_code=%s', reference_code)
@@ -535,14 +537,15 @@
     else:
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
                 
 
 
 @customer_api_bp.route('/reference-code/<reference_code>/transaction/limit/<limit>', methods=['GET'])
 @auth_token_required
+#@test_session_expired
 def list_customer_transaction(reference_code, limit):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
         limit_int = int(limit, 10)
         acct_id   = request.headers.get('x-acct-id')
@@ -608,14 +611,15 @@
 @model_transactional(desc="revert_customer_transaction")
 def __revert_customer_transaction(customer_transction, reverted_by, reverted_datetime):     
     return revert_transaction(customer_transction, reverted_by, reverted_datetime=reverted_datetime)
 
     
 @customer_api_bp.route('/reference-code/<reference_code>/redemption/limit/<limit>', methods=['GET'])
 @auth_token_required
+#@test_session_expired
 def list_customer_redemption(reference_code, limit):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
         limit_int = int(limit, 10)
         acct_id   = request.headers.get('x-acct-id')
```

### Comparing `trex-apis-1.0.1/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/outlet_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from trexapi.controllers.pos_api_routes import get_product_category_structure_code_label_json
 from flask_restful import abort
 from flask.helpers import url_for
 from trexmodel.models import merchant_helpers
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from flask.json import jsonify
 from trexadmin.libs.http import create_rest_message, StatusCode
-from trexapi.decorators.api_decorators import auth_token_required
+from trexapi.decorators.api_decorators import auth_token_required,\
+    test_session_expired
 from trexapi.utils.api_helpers import get_logged_in_api_username
 from flask_babel import gettext
 from trexapi.utils.reward_transaction_helper import revert_redemption,\
     revert_transaction
 from trexmodel.models.datastore.redeem_models import CustomerRedemption 
 from trexmodel.models.datastore.model_decorators import model_transactional
 from datetime import datetime
@@ -91,14 +92,15 @@
         return output_json
     else:
         abort
         
         
 @outlet_api_bp.route('/outlet-key/<outlet_key>/sales-transaction/limit/<limit>', methods=['GET'])
 @auth_token_required
+#@test_session_expired
 def list_outlet_transaction(outlet_key, limit):
     db_client = create_db_client(caller_info="list_outlet_transaction")
     transactions_list = []
     limit_int = int(limit)
     outlet = None
     with db_client.context():
         outlet = Outlet.fetch(outlet_key)
@@ -120,15 +122,16 @@
         return jsonify(transactions_list)
         
     else:
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
 
 
 @outlet_api_bp.route('/outlet-key/<outlet_key>/redemption/limit/<limit>', methods=['GET'])
-#@auth_token_required
+@auth_token_required
+#@test_session_expired
 def list_outlet_redemption(outlet_key, limit):
     db_client = create_db_client(caller_info="list_outlet_transaction")
     redemptions_list = []
     limit_int = int(limit)
     outlet = None
     with db_client.context():
         outlet = Outlet.fetch(outlet_key)
```

### Comparing `trex-apis-1.0.1/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/user_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.2/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.2/trexapi/decorators/api_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 from trexlib.utils.crypto_util import decrypt_json
 import logging
 from datetime import datetime
 
 logger = logging.getLogger('decorator')
 #logger = logging.getLogger('debug')
 
+def test_session_expired(f):
+    @wraps(f)
+    def decorated_function(*args, **kwargs):
+        return ("Authenticated token is expired", 401)
+    
+    return decorated_function
+
 def auth_token_required(f):
     @wraps(f)
     def decorated_function(*args, **kwargs):
         auth_token  = request.headers.get('x-auth-token')
         acct_id     = request.headers.get('x-acct-id')
             
         logger.debug('acct_id=%s', acct_id)
```

### Comparing `trex-apis-1.0.1/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.2/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.2/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/forms/sales_api_forms.py` & `trex-apis-1.0.2/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.2/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.2/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/utils/api_helpers.py` & `trex-apis-1.0.2/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.1/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.2/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

