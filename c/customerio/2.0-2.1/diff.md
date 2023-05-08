# Comparing `tmp/customerio-2.0.tar.gz` & `tmp/customerio-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customerio-2.0.tar", last modified: Thu Mar 30 20:33:38 2023, max compression
+gzip compressed data, was "dist/customerio-2.1.tar", last modified: Mon May  8 21:20:11 2023, max compression
```

## Comparing `customerio-2.0.tar` & `customerio-2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 danho      (502) staff       (20)        0 2023-03-30 20:33:38.104751 customerio-2.0/
--rw-r--r--   0 danho      (502) staff       (20)       44 2023-03-30 00:07:31.000000 customerio-2.0/AUTHORS
--rw-r--r--   0 danho      (502) staff       (20)     1067 2023-03-30 00:07:31.000000 customerio-2.0/LICENSE
--rw-r--r--   0 danho      (502) staff       (20)      702 2023-03-30 20:33:38.104569 customerio-2.0/PKG-INFO
--rw-r--r--   0 danho      (502) staff       (20)    11018 2023-03-30 00:07:31.000000 customerio-2.0/README.md
-drwxr-xr-x   0 danho      (502) staff       (20)        0 2023-03-30 20:33:38.101652 customerio-2.0/customerio/
--rw-r--r--   0 danho      (502) staff       (20)      206 2023-03-30 00:07:31.000000 customerio-2.0/customerio/__init__.py
--rw-r--r--   0 danho      (502) staff       (20)      408 2023-03-30 20:15:51.000000 customerio-2.0/customerio/__version__.py
--rw-r--r--   0 danho      (502) staff       (20)     4777 2023-03-30 01:17:06.000000 customerio-2.0/customerio/api.py
--rw-r--r--   0 danho      (502) staff       (20)     4179 2023-03-30 00:07:31.000000 customerio-2.0/customerio/client_base.py
--rw-r--r--   0 danho      (502) staff       (20)       64 2023-03-30 00:07:31.000000 customerio-2.0/customerio/constants.py
--rw-r--r--   0 danho      (502) staff       (20)      248 2023-03-30 00:07:31.000000 customerio-2.0/customerio/regions.py
--rw-r--r--   0 danho      (502) staff       (20)     8331 2023-03-30 00:07:31.000000 customerio-2.0/customerio/track.py
-drwxr-xr-x   0 danho      (502) staff       (20)        0 2023-03-30 20:33:38.103006 customerio-2.0/customerio.egg-info/
--rw-r--r--   0 danho      (502) staff       (20)      702 2023-03-30 20:33:38.000000 customerio-2.0/customerio.egg-info/PKG-INFO
--rw-r--r--   0 danho      (502) staff       (20)      439 2023-03-30 20:33:38.000000 customerio-2.0/customerio.egg-info/SOURCES.txt
--rw-r--r--   0 danho      (502) staff       (20)        1 2023-03-30 20:33:38.000000 customerio-2.0/customerio.egg-info/dependency_links.txt
--rw-r--r--   0 danho      (502) staff       (20)       17 2023-03-30 20:33:38.000000 customerio-2.0/customerio.egg-info/requires.txt
--rw-r--r--   0 danho      (502) staff       (20)       17 2023-03-30 20:33:38.000000 customerio-2.0/customerio.egg-info/top_level.txt
--rw-r--r--   0 danho      (502) staff       (20)       38 2023-03-30 20:33:38.104811 customerio-2.0/setup.cfg
--rw-r--r--   0 danho      (502) staff       (20)     1034 2023-03-30 00:07:31.000000 customerio-2.0/setup.py
-drwxr-xr-x   0 danho      (502) staff       (20)        0 2023-03-30 20:33:38.104261 customerio-2.0/tests/
--rw-r--r--   0 danho      (502) staff       (20)        0 2023-03-30 00:07:31.000000 customerio-2.0/tests/__init__.py
--rw-r--r--   0 danho      (502) staff       (20)     3064 2023-03-30 00:07:31.000000 customerio-2.0/tests/server.py
--rw-r--r--   0 danho      (502) staff       (20)     3224 2023-03-30 00:07:31.000000 customerio-2.0/tests/test_api.py
--rw-r--r--   0 danho      (502) staff       (20)    14327 2023-03-30 00:07:31.000000 customerio-2.0/tests/test_customerio.py
+drwxr-xr-x   0 colby      (501) staff       (20)        0 2023-05-08 21:20:11.000000 customerio-2.1/
+-rw-r--r--   0 colby      (501) staff       (20)       44 2023-04-24 19:42:08.000000 customerio-2.1/AUTHORS
+-rw-r--r--   0 colby      (501) staff       (20)     1067 2023-04-24 19:42:08.000000 customerio-2.1/LICENSE
+-rw-r--r--   0 colby      (501) staff       (20)      730 2023-05-08 21:20:11.000000 customerio-2.1/PKG-INFO
+-rw-r--r--   0 colby      (501) staff       (20)    11933 2023-04-24 22:59:41.000000 customerio-2.1/README.md
+drwxr-xr-x   0 colby      (501) staff       (20)        0 2023-05-08 21:20:11.000000 customerio-2.1/customerio/
+-rw-r--r--   0 colby      (501) staff       (20)      223 2023-04-24 19:59:32.000000 customerio-2.1/customerio/__init__.py
+-rw-r--r--   0 colby      (501) staff       (20)      408 2023-04-24 19:56:44.000000 customerio-2.1/customerio/__version__.py
+-rw-r--r--   0 colby      (501) staff       (20)     7371 2023-04-27 15:18:08.000000 customerio-2.1/customerio/api.py
+-rw-r--r--   0 colby      (501) staff       (20)     4179 2023-04-24 22:09:09.000000 customerio-2.1/customerio/client_base.py
+-rw-r--r--   0 colby      (501) staff       (20)       64 2021-10-13 16:03:19.000000 customerio-2.1/customerio/constants.py
+-rw-r--r--   0 colby      (501) staff       (20)      248 2021-10-14 16:12:11.000000 customerio-2.1/customerio/regions.py
+-rw-r--r--   0 colby      (501) staff       (20)     8331 2023-04-24 22:54:41.000000 customerio-2.1/customerio/track.py
+drwxr-xr-x   0 colby      (501) staff       (20)        0 2023-05-08 21:20:11.000000 customerio-2.1/customerio.egg-info/
+-rw-r--r--   0 colby      (501) staff       (20)      730 2023-05-08 21:20:11.000000 customerio-2.1/customerio.egg-info/PKG-INFO
+-rw-r--r--   0 colby      (501) staff       (20)      439 2023-05-08 21:20:11.000000 customerio-2.1/customerio.egg-info/SOURCES.txt
+-rw-r--r--   0 colby      (501) staff       (20)        1 2023-05-08 21:20:11.000000 customerio-2.1/customerio.egg-info/dependency_links.txt
+-rw-r--r--   0 colby      (501) staff       (20)       17 2023-05-08 21:20:11.000000 customerio-2.1/customerio.egg-info/requires.txt
+-rw-r--r--   0 colby      (501) staff       (20)       17 2023-05-08 21:20:11.000000 customerio-2.1/customerio.egg-info/top_level.txt
+-rw-r--r--   0 colby      (501) staff       (20)       38 2023-05-08 21:20:11.000000 customerio-2.1/setup.cfg
+-rw-r--r--   0 colby      (501) staff       (20)     1034 2023-04-24 19:42:08.000000 customerio-2.1/setup.py
+drwxr-xr-x   0 colby      (501) staff       (20)        0 2023-05-08 21:20:11.000000 customerio-2.1/tests/
+-rw-r--r--   0 colby      (501) staff       (20)        0 2021-10-13 16:03:19.000000 customerio-2.1/tests/__init__.py
+-rw-r--r--   0 colby      (501) staff       (20)     3064 2023-04-24 22:09:53.000000 customerio-2.1/tests/server.py
+-rw-r--r--   0 colby      (501) staff       (20)     3959 2023-04-24 21:28:20.000000 customerio-2.1/tests/test_api.py
+-rw-r--r--   0 colby      (501) staff       (20)    14327 2021-10-13 16:03:19.000000 customerio-2.1/tests/test_customerio.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `customerio-2.0/LICENSE` & `customerio-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `customerio-2.0/PKG-INFO` & `customerio-2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: customerio
-Version: 2.0
+Version: 2.1
 Summary: Customer.io Python bindings.
 Home-page: https://github.com/customerio/customerio-python
 Author: Peaberry Software Inc.
 Author-email: support@customerio.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS
+
+UNKNOWN
+
```

### Comparing `customerio-2.0/README.md` & `customerio-2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -184,16 +184,19 @@
 
 Unsuppresses the specified customer. We will remove the supplied id from our suppression list and start accepting new identify and track calls for the customer as normal
 
 See REST documentation [here](https://learn.customer.io/api/#apisuppress_delete)
 
 ### Send Transactional Messages
 
-To use the [Transactional API](https://customer.io/docs/transactional-api), instantiate the Customer.io object using an [app key](https://customer.io/docs/managing-credentials#app-api-keys) and create a request object containing:
+To use the [Transactional API](https://customer.io/docs/transactional-api), instantiate the Customer.io object using an [app key](https://customer.io/docs/managing-credentials#app-api-keys) and create a request object for your message type.
 
+## Email
+
+SendEmailRequest requires:
 * `transactional_message_id`: the ID of the transactional message you want to send, or the `body`, `from`, and `subject` of a new message.
 * `to`: the email address of your recipients 
 * an `identifiers` object containing the `id` of your recipient. If the `id` does not exist, Customer.io will create it.
 * a `message_data` object containing properties that you want reference in your message using Liquid.
 * You can also send attachments with your message. Use `attach` to encode attachments.
 
 Use `send_email` referencing your request to send a transactional message. [Learn more about transactional messages and `SendEmailRequest` properties](https://customer.io/docs/transactional-api).
@@ -222,14 +225,46 @@
 with open("path to file", "rb") as f:
   request.attach('receipt.pdf', f.read())
 
 response = client.send_email(request)
 print(response)
 ```
 
+## Push
+
+SendPushRequest requires:
+* `transactional_message_id`: the ID of the transactional push message you want to send.
+* an `identifiers` object containing the `id` or `email` of your recipient. If the profile does not exist, Customer.io will create it.
+
+Use `send_push` referencing your request to send a transactional message. [Learn more about transactional messages and `SendPushRequest` properties](https://customer.io/docs/transactional-api).
+
+```python
+from customerio import APIClient, Regions, SendPushRequest
+client = APIClient("your API key", region=Regions.US)
+
+request = SendPushRequest(
+  transactional_message_id="3",
+  message_data={
+    "name": "person",
+    "items": [
+      {
+        "name": "shoes",
+        "price": "59.99",
+      },
+    ]
+  },
+  identifiers={
+    "id": "2",
+  }
+)
+
+response = client.send_push(request)
+print(response)
+```
+
 ## Notes
 - The Customer.io Python SDK depends on the [`Requests`](https://pypi.org/project/requests/) library which includes [`urllib3`](https://pypi.org/project/urllib3/) as a transitive dependency.  The [`Requests`](https://pypi.org/project/requests/) library leverages connection pooling defined in [`urllib3`](https://pypi.org/project/urllib3/).  [`urllib3`](https://pypi.org/project/urllib3/) only attempts to retry invocations of `HTTP` methods which are understood to be idempotent (See: [`Retry.DEFAULT_ALLOWED_METHODS`](https://github.com/urllib3/urllib3/blob/main/src/urllib3/util/retry.py#L184)).  Since the `POST` method is not considered to be idempotent, any invocations which require `POST` are not retried.
 
 - It is possible to have the Customer.io Python SDK effectively *disable* connection pooling by passing a named initialization parameter `use_connection_pooling` to either the `APIClient` class or `CustomerIO` class.  Setting this parameter to `False` (default: `True`) causes the [`Session`](https://github.com/psf/requests/blob/main/requests/sessions.py#L355) to be initialized and discarded after each request.  If you are experiencing integration issues where the cause is reported as `Connection Reset by Peer`, this may correct the problem.  It will, however, impose a slight performance penalty as the TCP connection set-up and tear-down will now occur for each request.
 
 ### Usage Example Disabling Connection Pooling
 ```python
```

#### html2text {}

```diff
@@ -94,49 +94,61 @@
 #apisuppress_add) ### Unsuppress a customer ```python cio.unsuppress
 (customer_id="1") ``` Unsuppresses the specified customer. We will remove the
 supplied id from our suppression list and start accepting new identify and
 track calls for the customer as normal See REST documentation [here](https://
 learn.customer.io/api/#apisuppress_delete) ### Send Transactional Messages To
 use the [Transactional API](https://customer.io/docs/transactional-api),
 instantiate the Customer.io object using an [app key](https://customer.io/docs/
-managing-credentials#app-api-keys) and create a request object containing: *
-`transactional_message_id`: the ID of the transactional message you want to
-send, or the `body`, `from`, and `subject` of a new message. * `to`: the email
-address of your recipients * an `identifiers` object containing the `id` of
-your recipient. If the `id` does not exist, Customer.io will create it. * a
-`message_data` object containing properties that you want reference in your
-message using Liquid. * You can also send attachments with your message. Use
-`attach` to encode attachments. Use `send_email` referencing your request to
+managing-credentials#app-api-keys) and create a request object for your message
+type. ## Email SendEmailRequest requires: * `transactional_message_id`: the ID
+of the transactional message you want to send, or the `body`, `from`, and
+`subject` of a new message. * `to`: the email address of your recipients * an
+`identifiers` object containing the `id` of your recipient. If the `id` does
+not exist, Customer.io will create it. * a `message_data` object containing
+properties that you want reference in your message using Liquid. * You can also
+send attachments with your message. Use `attach` to encode attachments. Use
+`send_email` referencing your request to send a transactional message. [Learn
+more about transactional messages and `SendEmailRequest` properties](https://
+customer.io/docs/transactional-api). ```python from customerio import
+APIClient, Regions, SendEmailRequest client = APIClient("your API key",
+region=Regions.US) request = SendEmailRequest( to="person@example.com",
+transactional_message_id="3", message_data={ "name": "person", "items": [
+{ "name": "shoes", "price": "59.99", }, ] }, identifiers={ "id": "2", } ) with
+open("path to file", "rb") as f: request.attach('receipt.pdf', f.read())
+response = client.send_email(request) print(response) ``` ## Push
+SendPushRequest requires: * `transactional_message_id`: the ID of the
+transactional push message you want to send. * an `identifiers` object
+containing the `id` or `email` of your recipient. If the profile does not
+exist, Customer.io will create it. Use `send_push` referencing your request to
 send a transactional message. [Learn more about transactional messages and
-`SendEmailRequest` properties](https://customer.io/docs/transactional-api).
-```python from customerio import APIClient, Regions, SendEmailRequest client =
-APIClient("your API key", region=Regions.US) request = SendEmailRequest
-( to="person@example.com", transactional_message_id="3", message_data={ "name":
-"person", "items": [ { "name": "shoes", "price": "59.99", }, ] }, identifiers=
-{ "id": "2", } ) with open("path to file", "rb") as f: request.attach
-('receipt.pdf', f.read()) response = client.send_email(request) print(response)
-``` ## Notes - The Customer.io Python SDK depends on the [`Requests`](https://
-pypi.org/project/requests/) library which includes [`urllib3`](https://
-pypi.org/project/urllib3/) as a transitive dependency. The [`Requests`](https:/
-/pypi.org/project/requests/) library leverages connection pooling defined in
-[`urllib3`](https://pypi.org/project/urllib3/). [`urllib3`](https://pypi.org/
-project/urllib3/) only attempts to retry invocations of `HTTP` methods which
-are understood to be idempotent (See: [`Retry.DEFAULT_ALLOWED_METHODS`](https:/
-/github.com/urllib3/urllib3/blob/main/src/urllib3/util/retry.py#L184)). Since
-the `POST` method is not considered to be idempotent, any invocations which
-require `POST` are not retried. - It is possible to have the Customer.io Python
-SDK effectively *disable* connection pooling by passing a named initialization
-parameter `use_connection_pooling` to either the `APIClient` class or
-`CustomerIO` class. Setting this parameter to `False` (default: `True`) causes
-the [`Session`](https://github.com/psf/requests/blob/main/requests/
-sessions.py#L355) to be initialized and discarded after each request. If you
-are experiencing integration issues where the cause is reported as `Connection
-Reset by Peer`, this may correct the problem. It will, however, impose a slight
-performance penalty as the TCP connection set-up and tear-down will now occur
-for each request. ### Usage Example Disabling Connection Pooling ```python from
+`SendPushRequest` properties](https://customer.io/docs/transactional-api).
+```python from customerio import APIClient, Regions, SendPushRequest client =
+APIClient("your API key", region=Regions.US) request = SendPushRequest
+( transactional_message_id="3", message_data={ "name": "person", "items": [
+{ "name": "shoes", "price": "59.99", }, ] }, identifiers={ "id": "2", } )
+response = client.send_push(request) print(response) ``` ## Notes - The
+Customer.io Python SDK depends on the [`Requests`](https://pypi.org/project/
+requests/) library which includes [`urllib3`](https://pypi.org/project/urllib3/
+) as a transitive dependency. The [`Requests`](https://pypi.org/project/
+requests/) library leverages connection pooling defined in [`urllib3`](https://
+pypi.org/project/urllib3/). [`urllib3`](https://pypi.org/project/urllib3/) only
+attempts to retry invocations of `HTTP` methods which are understood to be
+idempotent (See: [`Retry.DEFAULT_ALLOWED_METHODS`](https://github.com/urllib3/
+urllib3/blob/main/src/urllib3/util/retry.py#L184)). Since the `POST` method is
+not considered to be idempotent, any invocations which require `POST` are not
+retried. - It is possible to have the Customer.io Python SDK effectively
+*disable* connection pooling by passing a named initialization parameter
+`use_connection_pooling` to either the `APIClient` class or `CustomerIO` class.
+Setting this parameter to `False` (default: `True`) causes the [`Session`]
+(https://github.com/psf/requests/blob/main/requests/sessions.py#L355) to be
+initialized and discarded after each request. If you are experiencing
+integration issues where the cause is reported as `Connection Reset by Peer`,
+this may correct the problem. It will, however, impose a slight performance
+penalty as the TCP connection set-up and tear-down will now occur for each
+request. ### Usage Example Disabling Connection Pooling ```python from
 customerio import CustomerIO, Regions cio = CustomerIO(site_id, api_key,
 region=Regions.US, use_connection_pooling=False) ``` ## Running tests Changes
 to the library can be tested by running `make test` from the parent directory.
 ## Thanks! * [Dimitriy Narkevich](https://github.com/dimier) for creating the
 library. * [EZL](https://github.com/ezl) for contributing customer deletes and
 improving README * [Noemi Millman](https://github.com/sbnoemi) for adding
 custom JSON encoder * [Jason Kraus](https://github.com/zbyte64) for event
```

### Comparing `customerio-2.0/customerio/client_base.py` & `customerio-2.1/customerio/client_base.py`

 * *Files identical despite different names*

### Comparing `customerio-2.0/customerio/track.py` & `customerio-2.1/customerio/track.py`

 * *Files identical despite different names*

### Comparing `customerio-2.0/customerio.egg-info/PKG-INFO` & `customerio-2.1/customerio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: customerio
-Version: 2.0
+Version: 2.1
 Summary: Customer.io Python bindings.
 Home-page: https://github.com/customerio/customerio-python
 Author: Peaberry Software Inc.
 Author-email: support@customerio.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS
+
+UNKNOWN
+
```

### Comparing `customerio-2.0/setup.py` & `customerio-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `customerio-2.0/tests/server.py` & `customerio-2.1/tests/server.py`

 * *Files identical despite different names*

### Comparing `customerio-2.0/tests/test_customerio.py` & `customerio-2.1/tests/test_customerio.py`

 * *Files identical despite different names*

