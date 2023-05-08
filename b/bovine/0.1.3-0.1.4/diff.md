# Comparing `tmp/bovine-0.1.3.tar.gz` & `tmp/bovine-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.1.3.tar", max compression
+gzip compressed data, was "bovine-0.1.4.tar", max compression
```

## Comparing `bovine-0.1.3.tar` & `bovine-0.1.4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0     1364 2023-04-30 17:02:34.666958 bovine-0.1.3/README.md
--rw-r--r--   0        0        0     9265 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 17:02:34.802960 bovine-0.1.3/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      173 2023-04-30 17:03:24.323409 bovine-0.1.3/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3612 2023-04-30 17:03:24.323409 bovine-0.1.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     2819 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0      922 2023-04-30 17:03:24.883414 bovine-0.1.3/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
--rw-r--r--   0        0        0     3638 2023-04-30 17:03:24.895414 bovine-0.1.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1212 2023-04-30 17:03:25.031416 bovine-0.1.3/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3339 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2837 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      434 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      498 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/test_collection_helper.py
--rw-r--r--   0        0        0     4957 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4645 2023-04-30 17:03:24.875414 bovine-0.1.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4269 2023-04-30 17:03:24.879414 bovine-0.1.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4086 2023-04-30 17:03:24.879414 bovine-0.1.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4584 2023-04-30 17:03:25.039415 bovine-0.1.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3327 2023-04-30 17:03:25.047416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3188 2023-04-30 17:03:25.051416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1951 2023-04-30 17:03:25.055416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1386 2023-04-30 17:03:25.059416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     4203 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4240 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2195 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1442 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1397 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1034 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      817 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2836 2023-04-30 17:03:24.879414 bovine-0.1.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      908 2023-04-30 17:03:24.883414 bovine-0.1.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
--rw-r--r--   0        0        0     4763 2023-04-30 17:03:25.071416 bovine-0.1.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      787 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     2722 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/__init__.py
--rw-r--r--   0        0        0     2854 2023-04-30 17:03:24.575411 bovine-0.1.3/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/bearer.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1719 2023-04-30 17:03:24.619412 bovine-0.1.3/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1014 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2534 2023-04-30 17:03:24.619412 bovine-0.1.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
--rw-r--r--   0        0        0     1237 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     1529 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     2479 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
--rw-r--r--   0        0        0     1352 2023-04-30 17:03:25.075416 bovine-0.1.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2648 2023-04-30 17:03:25.079416 bovine-0.1.3/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1217 2023-04-30 17:03:25.083416 bovine-0.1.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2102 2023-04-30 17:03:25.083416 bovine-0.1.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      814 2023-04-30 17:03:25.087416 bovine-0.1.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1794 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/bearer.py
--rw-r--r--   0        0        0       91 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/consts.py
--rw-r--r--   0        0        0     1520 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/event_source.py
--rw-r--r--   0        0        0      787 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3001 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/moo_auth.py
--rw-r--r--   0        0        0      948 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     1150 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     3278 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/signed_http_methods.py
--rw-r--r--   0        0        0      609 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0     1149 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1153 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      522 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     4141 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3749 2023-04-30 17:03:24.623412 bovine-0.1.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2863 2023-04-30 17:03:24.763413 bovine-0.1.3/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2909 2023-04-30 17:03:24.763413 bovine-0.1.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2257 2023-04-30 17:03:24.763413 bovine-0.1.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2363 2023-04-30 17:03:25.027415 bovine-0.1.3/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5821 2023-04-30 17:03:25.095416 bovine-0.1.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2742 2023-04-30 17:03:25.099416 bovine-0.1.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     7454 2023-04-30 17:03:25.107416 bovine-0.1.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2674 2023-04-30 17:03:25.115416 bovine-0.1.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2664 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test.py
--rw-r--r--   0        0        0     4995 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/ed25519_key.py
--rw-r--r--   0        0        0      864 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/msg.py
--rw-r--r--   0        0        0      178 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/test_bovine_client.py
--rw-r--r--   0        0        0      282 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/types.py
--rw-r--r--   0        0        0      667 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/__init__.py
--rw-r--r--   0        0        0      848 2023-04-30 17:03:24.575411 bovine-0.1.3/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      877 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0     3465 2023-04-30 17:03:25.123416 bovine-0.1.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1662 2023-04-30 17:03:25.127416 bovine-0.1.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      973 2023-04-30 17:03:25.131416 bovine-0.1.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      519 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/date.py
--rw-r--r--   0        0        0     1210 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0     1795 2023-04-30 17:03:25.131416 bovine-0.1.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1967 2023-04-30 17:03:25.135416 bovine-0.1.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      659 2023-04-30 17:03:25.135416 bovine-0.1.3/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0      599 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      261 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0      761 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      191 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1229 2023-04-30 17:02:34.670958 bovine-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 bovine-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1436 2023-05-08 17:50:40.301592 bovine-0.1.4/README.md
+-rw-r--r--   0        0        0     9265 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:50:40.421594 bovine-0.1.4/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-08 17:51:20.694005 bovine-0.1.4/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3612 2023-05-08 17:51:20.694005 bovine-0.1.4/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2819 2023-05-08 17:51:21.102010 bovine-0.1.4/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      922 2023-05-08 17:51:21.210011 bovine-0.1.4/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-05-08 17:51:21.222011 bovine-0.1.4/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1212 2023-05-08 17:51:21.246011 bovine-0.1.4/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3339 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2837 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      434 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0      498 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitypub/test_collection_helper.py
+-rw-r--r--   0        0        0     4957 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4645 2023-05-08 17:51:21.206011 bovine-0.1.4/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4269 2023-05-08 17:51:21.206011 bovine-0.1.4/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4028 2023-05-08 17:51:21.206011 bovine-0.1.4/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4584 2023-05-08 17:51:21.258011 bovine-0.1.4/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3327 2023-05-08 17:51:21.262011 bovine-0.1.4/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3113 2023-05-08 17:51:21.270011 bovine-0.1.4/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1951 2023-05-08 17:51:21.274011 bovine-0.1.4/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1386 2023-05-08 17:51:21.278011 bovine-0.1.4/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     4203 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4178 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1257 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-05-08 17:51:21.206011 bovine-0.1.4/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2023-05-08 17:51:21.210011 bovine-0.1.4/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-05-08 17:51:21.286012 bovine-0.1.4/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      787 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     2722 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     2854 2023-05-08 17:51:20.918008 bovine-0.1.4/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-05-08 17:51:20.922008 bovine-0.1.4/bovine/clients/__pycache__/bearer.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-05-08 17:51:20.922008 bovine-0.1.4/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1719 2023-05-08 17:51:20.962008 bovine-0.1.4/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1014 2023-05-08 17:51:20.922008 bovine-0.1.4/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2534 2023-05-08 17:51:20.962008 bovine-0.1.4/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-05-08 17:51:20.922008 bovine-0.1.4/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     1529 2023-05-08 17:51:21.098010 bovine-0.1.4/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     2479 2023-05-08 17:51:21.098010 bovine-0.1.4/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
+-rw-r--r--   0        0        0     1352 2023-05-08 17:51:21.294012 bovine-0.1.4/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2648 2023-05-08 17:51:21.298012 bovine-0.1.4/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1217 2023-05-08 17:51:21.302012 bovine-0.1.4/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2102 2023-05-08 17:51:21.302012 bovine-0.1.4/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      814 2023-05-08 17:51:21.306012 bovine-0.1.4/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1794 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      787 2023-05-08 17:50:40.301592 bovine-0.1.4/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      609 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1149 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3749 2023-05-08 17:51:20.962008 bovine-0.1.4/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-05-08 17:51:21.094009 bovine-0.1.4/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-05-08 17:51:21.098010 bovine-0.1.4/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-05-08 17:51:21.098010 bovine-0.1.4/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-05-08 17:51:21.098010 bovine-0.1.4/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-05-08 17:51:21.242011 bovine-0.1.4/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5821 2023-05-08 17:51:21.314012 bovine-0.1.4/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2742 2023-05-08 17:51:21.318012 bovine-0.1.4/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     7454 2023-05-08 17:51:21.330012 bovine-0.1.4/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2674 2023-05-08 17:51:21.338012 bovine-0.1.4/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2664 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/ed25519_key.py
+-rw-r--r--   0        0        0      864 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/msg.py
+-rw-r--r--   0        0        0      178 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0      282 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/types.py
+-rw-r--r--   0        0        0      667 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-08 17:51:20.918008 bovine-0.1.4/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-05-08 17:51:20.922008 bovine-0.1.4/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-05-08 17:51:21.342012 bovine-0.1.4/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1662 2023-05-08 17:51:21.350012 bovine-0.1.4/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      973 2023-05-08 17:51:21.350012 bovine-0.1.4/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      519 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/date.py
+-rw-r--r--   0        0        0     1210 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0     1795 2023-05-08 17:51:21.354012 bovine-0.1.4/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1967 2023-05-08 17:51:21.354012 bovine-0.1.4/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      659 2023-05-08 17:51:21.354012 bovine-0.1.4/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      599 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0      761 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      191 2023-05-08 17:50:40.305592 bovine-0.1.4/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1229 2023-05-08 17:50:40.305592 bovine-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 bovine-0.1.4/PKG-INFO
```

### Comparing `bovine-0.1.3/README.md` & `bovine-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,7 +21,12 @@
 
 - [aiohttp](https://docs.aiohttp.org/en/stable/index.html) for http requests.
 - [quart](https://quart.palletsprojects.com/en/latest/) as a webserver.
 - [cryptography](https://cryptography.io/en/latest/).
 - [pytest](https://docs.pytest.org/en/7.3.x/) for testing.
 - [ruff](https://pypi.org/project/ruff/) for linting.
 
+
+## Todo
+
+- [ ] Document FediVerse crawler behavior in server tutorial
+
```

### Comparing `bovine-0.1.3/bovine/__init__.py` & `bovine-0.1.4/bovine/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc` & `bovine-0.1.4/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 3339 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0b0d 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 0b0d 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `bovine-0.1.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc` & `bovine-0.1.4/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 150b 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 150b 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 8400 5a05 6407 6408 8400 5a06 4700  d...Z.d.d...Z.G.
 00000060: 6409 640a 8400 640a 8302 5a07 6401 5300  d.d...d...Z.d.S.
 00000070: 290b e900 0000 004e 2901 da0e 7072 696e  )......N)...prin
```

### Comparing `bovine-0.1.3/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc` & `bovine-0.1.4/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b201 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 b201 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 0003 0000 0040 0000 0073 2a00 0000  .......@...s*...
 00000060: 6500 5a01 6400 5a02 6401 6503 6602 6402  e.Z.d.Z.d.e.f.d.
 00000070: 6403 8404 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.1.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 c50a 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 c50a 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6400 6401 6c0a 5a0a 6400 6403 6c0b 6d0c  d.d.l.Z.d.d.l.m.
 00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `bovine-0.1.3/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 498 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f201 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 f201 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6403 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6506 6a0b a00c 6405  l.m.Z...e.j...d.
 00000070: a101 6406 6407 8400 8301 5a0d 6401 5300  ..d.d.....Z.d.S.
```

### Comparing `bovine-0.1.3/bovine/activitypub/authorization_wrapper.py` & `bovine-0.1.4/bovine/activitypub/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitypub/collection_helper.py` & `bovine-0.1.4/bovine/activitypub/collection_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitypub/test_actor.py` & `bovine-0.1.4/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/__init__.py` & `bovine-0.1.4/bovine/activitystreams/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 4957 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 5d13 0000  o.......*.Nd]...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 5d13 0000  o.......p6Yd]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 650b 6408 6504 6508 650a 6602 1900 6604  e.d.e.e.e.f...f.
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 4203 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 6b10 0000  o.......*.Ndk...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 6b10 0000  o.......p6Ydk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6501  d.l.m.Z.m.Z...e.
 00000050: 4700 6403 6404 8400 6404 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 4700 6405 6406 8400 6406 8302 5a07 6407  G.d.d...d...Z.d.
 00000070: 5300 2908 e900 0000 0029 02da 0964 6174  S.)......)...dat
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 4240 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,256 +1,252 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9010 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 5210 0000  o.......p6YdR...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 6d07 5a07 0100 6404 6405 6c08  m.Z.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6502 4700 6406 6407 8400  m.Z...e.G.d.d...
-00000070: 6407 8302 8301 5a0a 4700 6408 6409 8400  d.....Z.G.d.d...
-00000080: 6409 8302 5a0b 6401 5300 290a e900 0000  d...Z.d.S.).....
-00000090: 004e 2902 da09 6461 7461 636c 6173 73da  .N)...dataclass.
-000000a0: 0566 6965 6c64 2903 da04 4c69 7374 da08  .field)...List..
-000000b0: 4f70 7469 6f6e 616c da03 5365 74e9 0100  Optional..Set...
-000000c0: 0000 2901 da1b 6665 6469 7665 7273 655f  ..)...fediverse_
-000000d0: 6861 6e64 6c65 5f66 726f 6d5f 6163 746f  handle_from_acto
-000000e0: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-000000f0: 0000 0300 0000 4000 0000 735a 0100 0065  ......@...sZ...e
-00000100: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000110: 0564 023c 0064 035a 0665 0765 0419 0065  .d.<.d.Z.e.e...e
-00000120: 0564 043c 0064 035a 0865 0765 0419 0065  .d.<.d.Z.e.e...e
-00000130: 0564 053c 0064 035a 0965 0765 0419 0065  .d.<.d.Z.e.e...e
-00000140: 0564 063c 0064 035a 0a65 0765 0419 0065  .d.<.d.Z.e.e...e
-00000150: 0564 073c 0065 0b65 0c64 088d 015a 0d65  .d.<.e.e.d...Z.e
-00000160: 0e65 0419 0065 0564 093c 0065 0b65 0c64  .e...e.d.<.e.e.d
-00000170: 088d 015a 0f65 0e65 0419 0065 0564 0a3c  ...Z.e.e...e.d.<
-00000180: 0064 035a 1065 0765 0419 0065 0564 0b3c  .d.Z.e.e...e.d.<
-00000190: 0064 035a 1165 0765 0419 0065 0564 0c3c  .d.Z.e.e...e.d.<
-000001a0: 0064 035a 1265 0765 0419 0065 0564 0d3c  .d.Z.e.e...e.d.<
-000001b0: 0064 035a 1365 0765 1419 0065 0564 0e3c  .d.Z.e.e...e.d.<
-000001c0: 0064 035a 1565 0765 1619 0065 0564 0f3c  .d.Z.e.e...e.d.<
-000001d0: 0064 035a 1765 0765 1619 0065 0564 103c  .d.Z.e.e...e.d.<
-000001e0: 0064 035a 1865 0765 0419 0065 0564 113c  .d.Z.e.e...e.d.<
-000001f0: 0064 035a 1965 0765 0419 0065 0564 123c  .d.Z.e.e...e.d.<
-00000200: 0065 0b65 1a64 088d 015a 1b65 1c65 1419  .e.e.d...Z.e.e..
-00000210: 0065 0564 133c 0065 0b65 1a64 088d 015a  .e.d.<.e.e.d...Z
-00000220: 1d65 1c65 1419 0065 0564 143c 0064 035a  .e.e...e.d.<.d.Z
-00000230: 1e65 0765 0419 0065 0564 153c 0064 1664  .e.e...e.d.<.d.d
-00000240: 1784 005a 1f64 1864 1984 005a 2064 1a64  ...Z.d.d...Z d.d
-00000250: 1b84 005a 2164 0353 0029 1cda 064f 626a  ...Z!d.S.)...Obj
-00000260: 6563 747a 7a41 2064 6174 6163 6c61 7373  ectzzA dataclass
-00000270: 2072 6570 7265 7365 6e74 696e 6720 616e   representing an
-00000280: 2060 4163 7469 7669 7479 5374 7265 616d   `ActivityStream
-00000290: 7320 4f62 6a65 6374 0a20 2020 203c 6874  s Object.    <ht
-000002a0: 7470 733a 2f2f 7777 772e 7733 2e6f 7267  tps://www.w3.org
-000002b0: 2f54 522f 6163 7469 7669 7479 7374 7265  /TR/activitystre
-000002c0: 616d 732d 766f 6361 6275 6c61 7279 2f23  ams-vocabulary/#
-000002d0: 6f62 6a65 6374 2d74 7970 6573 3e60 5fda  object-types>`_.
-000002e0: 0474 7970 654e da0d 6174 7472 6962 7574  .typeN..attribut
-000002f0: 6564 5f74 6fda 0966 6f6c 6c6f 7765 7273  ed_to..followers
-00000300: da02 6964 da09 7075 626c 6973 6865 6429  ..id..published)
-00000310: 01da 0f64 6566 6175 6c74 5f66 6163 746f  ...default_facto
-00000320: 7279 da02 746f da02 6363 da04 6e61 6d65  ry..to..cc..name
-00000330: da07 7375 6d6d 6172 79da 0763 6f6e 7465  ..summary..conte
-00000340: 6e74 da06 736f 7572 6365 da05 7769 6474  nt..source..widt
-00000350: 68da 0668 6569 6768 74da 0b69 6e5f 7265  h..height..in_re
-00000360: 706c 795f 746f da03 7572 6cda 0374 6167  ply_to..url..tag
-00000370: da0a 6174 7461 6368 6d65 6e74 da04 6872  ..attachment..hr
-00000380: 6566 6301 0000 0000 0000 0000 0000 0001  efc.............
-00000390: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
-000003a0: 7c00 6a00 a001 6401 a101 0100 7c00 6a02  |.j...d.....|.j.
-000003b0: 7210 7c00 6a03 a001 7c00 6a02 a101 0100  r.|.j...|.j.....
-000003c0: 7c00 5300 a902 4e7a 2c68 7474 7073 3a2f  |.S...Nz,https:/
-000003d0: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
-000003e0: 6374 6976 6974 7973 7472 6561 6d73 2350  ctivitystreams#P
-000003f0: 7562 6c69 6329 0472 1000 0000 da03 6164  ublic).r......ad
-00000400: 6472 0c00 0000 7211 0000 00a9 01da 0473  dr....r........s
-00000410: 656c 66a9 0072 2100 0000 fa5a 2f77 6f6f  elf..r!....Z/woo
-00000420: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-00000430: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
-00000440: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-00000450: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
-00000460: 6561 6d73 2f6f 626a 6563 745f 6661 6374  eams/object_fact
-00000470: 6f72 792e 7079 da09 6173 5f70 7562 6c69  ory.py..as_publi
-00000480: 6323 0000 0073 0800 0000 0c01 0601 0e01  c#...s..........
-00000490: 0401 7a10 4f62 6a65 6374 2e61 735f 7075  ..z.Object.as_pu
-000004a0: 626c 6963 6301 0000 0000 0000 0000 0000  blicc...........
-000004b0: 0001 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
-000004c0: 0000 7c00 6a00 720a 7c00 6a01 a002 7c00  ..|.j.r.|.j...|.
-000004d0: 6a00 a101 0100 7c00 6a03 a002 6401 a101  j.....|.j...d...
-000004e0: 0100 7c00 5300 721d 0000 0029 0472 0c00  ..|.S.r....).r..
-000004f0: 0000 7210 0000 0072 1e00 0000 7211 0000  ..r....r....r...
-00000500: 0072 1f00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
-00000510: 7222 0000 00da 0b61 735f 756e 6c69 7374  r".....as_unlist
-00000520: 6564 2900 0000 7308 0000 0006 010e 010c  ed)...s.........
-00000530: 0104 017a 124f 626a 6563 742e 6173 5f75  ...z.Object.as_u
-00000540: 6e6c 6973 7465 6463 0100 0000 0000 0000  nlistedc........
-00000550: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
-00000560: 73fc 0000 0064 017c 006a 0064 029c 027d  s....d.|.j.d...}
-00000570: 0169 0064 037c 006a 0193 0164 0474 027c  .i.d.|.j...d.t.|
-00000580: 006a 0383 0193 0164 0574 027c 006a 047c  .j.....d.t.|.j.|
-00000590: 006a 0318 0083 0193 0164 067c 006a 0593  .j.......d.|.j..
-000005a0: 0164 077c 006a 0693 0164 087c 006a 0793  .d.|.j...d.|.j..
-000005b0: 0164 097c 006a 0893 0164 0a7c 006a 0993  .d.|.j...d.|.j..
-000005c0: 0164 0b7c 006a 0a93 0164 0c7c 006a 0b93  .d.|.j...d.|.j..
-000005d0: 0164 0d7c 006a 0c93 0164 0e7c 006a 0d93  .d.|.j...d.|.j..
-000005e0: 0164 0f7c 006a 0e93 0164 107c 006a 0f93  .d.|.j...d.|.j..
-000005f0: 0164 117c 006a 1093 0164 127c 006a 1193  .d.|.j...d.|.j..
-00000600: 017d 027c 02a0 12a1 0044 005d 0a5c 027d  .}.|.....D.].\.}
-00000610: 037d 047c 0472 5d7c 047c 017c 033c 0071  .}.|.r]|.|.|.<.q
-00000620: 5364 047c 0176 0072 6d74 137c 0164 0419  Sd.|.v.rmt.|.d..
-00000630: 0083 0164 136b 0272 6d7c 0164 043d 0064  ...d.k.rm|.d.=.d
-00000640: 057c 0176 0072 7c74 137c 0164 0519 0083  .|.v.r|t.|.d....
-00000650: 0164 136b 0272 7c7c 0164 053d 007c 0153  .d.k.r||.d.=.|.S
-00000660: 0029 144e 7a25 6874 7470 733a 2f2f 7777  .).Nz%https://ww
-00000670: 772e 7733 2e6f 7267 2f6e 732f 6163 7469  w.w3.org/ns/acti
-00000680: 7669 7479 7374 7265 616d 7329 027a 0840  vitystreams).z.@
-00000690: 636f 6e74 6578 7472 0a00 0000 da0c 6174  contextr......at
-000006a0: 7472 6962 7574 6564 546f 7210 0000 0072  tributedTor....r
-000006b0: 1100 0000 720d 0000 005a 0969 6e52 6570  ....r....Z.inRep
-000006c0: 6c79 546f 720e 0000 0072 1500 0000 7212  lyTor....r....r.
-000006d0: 0000 0072 1900 0000 7213 0000 0072 1400  ...r....r....r..
-000006e0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000006f0: 0072 1600 0000 7217 0000 0072 0100 0000  .r....r....r....
-00000700: 2914 720a 0000 0072 0b00 0000 da04 6c69  ).r....r......li
-00000710: 7374 7210 0000 0072 1100 0000 720d 0000  str....r....r...
-00000720: 0072 1800 0000 720e 0000 0072 1500 0000  .r....r....r....
-00000730: 7212 0000 0072 1900 0000 7213 0000 0072  r....r....r....r
-00000740: 1400 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
-00000750: 0000 0072 1600 0000 7217 0000 00da 0569  ...r....r......i
-00000760: 7465 6d73 da03 6c65 6e29 0572 2000 0000  tems..len).r ...
-00000770: da06 7265 7375 6c74 da0c 6578 7472 615f  ..result..extra_
-00000780: 6669 656c 6473 da03 6b65 79da 0576 616c  fields..key..val
-00000790: 7565 7221 0000 0072 2100 0000 7222 0000  uer!...r!...r"..
-000007a0: 00da 0562 7569 6c64 2f00 0000 735a 0000  ...build/...sZ..
-000007b0: 0002 0204 0106 fe02 0506 0102 ff0a 0202  ................
-000007c0: fe10 0302 fd06 0402 fc06 0502 fb06 0602  ................
-000007d0: fa06 0702 f906 0802 f806 0902 f706 0a02  ................
-000007e0: f606 0b02 f506 0c02 f406 0d02 f306 0e02  ................
-000007f0: f206 0f02 f106 1004 f010 1304 0108 0102  ................
-00000800: 8018 0206 0118 0106 0104 027a 0c4f 626a  ...........z.Obj
-00000810: 6563 742e 6275 696c 6429 22da 085f 5f6e  ect.build)"..__n
-00000820: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000830: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000840: 075f 5f64 6f63 5f5f da03 7374 72da 0f5f  .__doc__..str.._
-00000850: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 720b  _annotations__r.
-00000860: 0000 0072 0500 0000 720c 0000 0072 0d00  ...r....r....r..
-00000870: 0000 720e 0000 0072 0300 0000 da03 7365  ..r....r......se
-00000880: 7472 1000 0000 7206 0000 0072 1100 0000  tr....r....r....
-00000890: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-000008a0: 1500 0000 da04 6469 6374 7216 0000 00da  ......dictr.....
-000008b0: 0369 6e74 7217 0000 0072 1800 0000 7219  .intr....r....r.
-000008c0: 0000 0072 2600 0000 721a 0000 0072 0400  ...r&...r....r..
-000008d0: 0000 721b 0000 0072 1c00 0000 7223 0000  ..r....r....r#..
-000008e0: 0072 2400 0000 722d 0000 0072 2100 0000  .r$...r-...r!...
-000008f0: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00000900: 0900 0000 0800 0000 732e 0000 000a 0004  ........s.......
-00000910: 0208 0310 0110 0110 0110 0116 0116 0110  ................
-00000920: 0210 0110 0110 0110 0210 0110 0210 0116  ................
-00000930: 0116 0110 0108 0208 060c 0672 0900 0000  ...........r....
-00000940: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000950: 0003 0000 0040 0000 0073 3a00 0000 6500  .....@...s:...e.
-00000960: 5a01 6400 5a02 6401 5a03 640d 6403 6404  Z.d.Z.d.Z.d.d.d.
-00000970: 8401 5a04 6405 6406 8400 5a05 6407 6408  ..Z.d.d...Z.d.d.
-00000980: 8400 5a06 6409 640a 8400 5a07 640b 640c  ..Z.d.d...Z.d.d.
-00000990: 8400 5a08 6402 5300 290e da0d 4f62 6a65  ..Z.d.S.)...Obje
-000009a0: 6374 4661 6374 6f72 797a 344f 626a 6563  ctFactoryz4Objec
-000009b0: 7446 6163 746f 7279 2075 7375 616c 6c79  tFactory usually
-000009c0: 2063 7265 6174 6564 2074 6872 6f75 6768   created through
-000009d0: 2061 2042 6f76 696e 6543 6c69 656e 744e   a BovineClientN
-000009e0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000009f0: 0002 0000 0043 0000 0073 3200 0000 7c02  .....C...s2...|.
-00000a00: 720b 7c02 7c00 5f00 7c02 6a01 7c00 5f01  r.|.|._.|.j.|._.
-00000a10: 6400 5300 7c01 7215 6400 7c00 5f00 7c01  d.S.|.r.d.|._.|.
-00000a20: 7c00 5f01 6400 5300 7402 6401 8301 8201  |._.d.S.t.d.....
-00000a30: 2902 4e7a 3e59 6f75 206e 6565 6420 746f  ).Nz>You need to
-00000a40: 2065 6974 6865 7220 7370 6563 6966 7920   either specify 
-00000a50: 6163 746f 725f 696e 666f 726d 6174 696f  actor_informatio
-00000a60: 6e20 6f72 2061 2042 6f76 696e 6543 6c69  n or a BovineCli
-00000a70: 656e 7429 03da 0663 6c69 656e 74da 0b69  ent)...client..i
-00000a80: 6e66 6f72 6d61 7469 6f6e da09 5479 7065  nformation..Type
-00000a90: 4572 726f 7229 0372 2000 0000 da11 6163  Error).r .....ac
-00000aa0: 746f 725f 696e 666f 726d 6174 696f 6e72  tor_informationr
-00000ab0: 3800 0000 7221 0000 0072 2100 0000 7222  8...r!...r!...r"
-00000ac0: 0000 00da 085f 5f69 6e69 745f 5f57 0000  .....__init__W..
-00000ad0: 0073 1200 0000 0401 0601 0c01 0401 0601  .s..............
-00000ae0: 0a01 0202 0201 04ff 7a16 4f62 6a65 6374  ........z.Object
-00000af0: 4661 6374 6f72 792e 5f5f 696e 6974 5f5f  Factory.__init__
-00000b00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b10: 0007 0000 004b 0000 00f3 2400 0000 7400  .....K....$...t.
-00000b20: 6406 7c00 6a01 6401 1900 6402 7c00 6a01  d.|.j.d...d.|.j.
-00000b30: a002 6403 a101 6404 9c03 7c01 a401 8e01  ..d...d...|.....
-00000b40: 5300 2907 7a15 4372 6561 7465 7320 6120  S.).z.Creates a 
-00000b50: 4e6f 7465 204f 626a 6563 7472 0d00 0000  Note Objectr....
-00000b60: 5a04 4e6f 7465 720c 0000 00a9 0372 0b00  Z.Noter......r..
-00000b70: 0000 720a 0000 0072 0c00 0000 4e72 2100  ..r....r....Nr!.
-00000b80: 0000 a903 7209 0000 0072 3900 0000 da03  ....r....r9.....
-00000b90: 6765 74a9 0272 2000 0000 da06 6b77 6172  get..r .....kwar
-00000ba0: 6773 7221 0000 0072 2100 0000 7222 0000  gsr!...r!...r"..
-00000bb0: 00da 046e 6f74 6563 0000 00f3 0e00 0000  ...notec........
-00000bc0: 0402 0801 0201 0a01 04fd 0204 06fc 7a12  ..............z.
-00000bd0: 4f62 6a65 6374 4661 6374 6f72 792e 6e6f  ObjectFactory.no
-00000be0: 7465 6301 0000 0000 0000 0000 0000 0002  tec.............
-00000bf0: 0000 0007 0000 004b 0000 0072 3d00 0000  .......K...r=...
-00000c00: 2907 7a19 4372 6561 7465 7320 616e 2041  ).z.Creates an A
-00000c10: 7274 6963 6c65 204f 626a 6563 7472 0d00  rticle Objectr..
-00000c20: 0000 5a07 4172 7469 636c 6572 0c00 0000  ..Z.Articler....
-00000c30: 723e 0000 004e 7221 0000 0072 3f00 0000  r>...Nr!...r?...
-00000c40: 7241 0000 0072 2100 0000 7221 0000 0072  rA...r!...r!...r
-00000c50: 2200 0000 da07 6172 7469 636c 656c 0000  ".....articlel..
-00000c60: 0072 4400 0000 7a15 4f62 6a65 6374 4661  .rD...z.ObjectFa
-00000c70: 6374 6f72 792e 6172 7469 636c 6563 0100  ctory.articlec..
-00000c80: 0000 0000 0000 0000 0000 0200 0000 0700  ................
-00000c90: 0000 4b00 0000 723d 0000 0029 077a 1743  ..K...r=...).z.C
-00000ca0: 7265 6174 6573 2061 6e20 4576 656e 7420  reates an Event 
-00000cb0: 4f62 6a65 6374 720d 0000 00da 0545 7665  Objectr......Eve
-00000cc0: 6e74 720c 0000 0072 3e00 0000 4e72 2100  ntr....r>...Nr!.
-00000cd0: 0000 723f 0000 0072 4100 0000 7221 0000  ..r?...rA...r!..
-00000ce0: 0072 2100 0000 7222 0000 00da 0565 7665  .r!...r".....eve
-00000cf0: 6e74 7500 0000 7244 0000 007a 134f 626a  ntu...rD...z.Obj
-00000d00: 6563 7446 6163 746f 7279 2e65 7665 6e74  ectFactory.event
-00000d10: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000d20: 0005 0000 00c3 0000 0073 4a00 0000 8101  .........sJ.....
-00000d30: 7c00 6a00 7308 7401 6401 8301 8201 7c00  |.j.s.t.d.....|.
-00000d40: 6a00 6a00 a002 7c01 a101 4900 6402 4800  j.j...|...I.d.H.
-00000d50: 7d02 7403 a004 7c02 a005 a100 4900 6402  }.t...|.....I.d.
-00000d60: 4800 a101 7d03 7406 6403 7c01 7407 7c03  H...}.t.d.|.t.|.
-00000d70: 8301 6404 8d03 5300 2905 7a88 4372 6561  ..d...S.).z.Crea
-00000d80: 7465 7320 6120 6d65 6e74 696f 6e20 6f62  tes a mention ob
-00000d90: 6a65 6374 2066 6f72 2061 6e6f 7468 6572  ject for another
-00000da0: 2061 6374 6f72 2e20 5265 7175 6972 6573   actor. Requires
-00000db0: 2063 6c69 656e 7420 746f 2062 6520 7365   client to be se
-00000dc0: 742e 0a0a 2020 2020 2020 2020 3a70 6172  t...        :par
-00000dd0: 616d 2061 6374 6f72 5f74 6f5f 6d65 6e74  am actor_to_ment
-00000de0: 696f 6e3a 2054 6865 2055 5249 206f 6620  ion: The URI of 
-00000df0: 7468 6520 6163 746f 7220 746f 206d 656e  the actor to men
-00000e00: 7469 6f6e 7a26 636c 6965 6e74 206e 6565  tionz&client nee
-00000e10: 6473 2074 6f20 6265 2073 6574 2061 7420  ds to be set at 
-00000e20: 636f 6e73 7472 7563 7469 6f6e 4e5a 074d  constructionNZ.M
-00000e30: 656e 7469 6f6e 2903 720a 0000 0072 1c00  ention).r....r..
-00000e40: 0000 7212 0000 0029 0872 3800 0000 723a  ..r....).r8...r:
-00000e50: 0000 0072 4000 0000 da04 6a73 6f6e da05  ...r@.....json..
-00000e60: 6c6f 6164 73da 0474 6578 7472 0900 0000  loads..textr....
-00000e70: 7208 0000 0029 0472 2000 0000 5a10 6163  r....).r ...Z.ac
-00000e80: 746f 725f 746f 5f6d 656e 7469 6f6e da08  tor_to_mention..
-00000e90: 7265 7370 6f6e 7365 5a0c 7265 6d6f 7465  responseZ.remote
-00000ea0: 5f61 6374 6f72 7221 0000 0072 2100 0000  _actorr!...r!...
-00000eb0: 7222 0000 00da 156d 656e 7469 6f6e 5f66  r".....mention_f
-00000ec0: 6f72 5f61 6374 6f72 5f75 7269 7e00 0000  or_actor_uri~...
-00000ed0: 7314 0000 0002 8006 0508 0114 0214 0102  s...............
-00000ee0: 0202 0102 0106 0106 fd7a 234f 626a 6563  .........z#Objec
-00000ef0: 7446 6163 746f 7279 2e6d 656e 7469 6f6e  tFactory.mention
-00000f00: 5f66 6f72 5f61 6374 6f72 5f75 7269 2902  _for_actor_uri).
-00000f10: 4e4e 2909 722e 0000 0072 2f00 0000 7230  NN).r....r/...r0
-00000f20: 0000 0072 3100 0000 723c 0000 0072 4300  ...r1...r<...rC.
-00000f30: 0000 7245 0000 0072 4700 0000 724c 0000  ..rE...rG...rL..
-00000f40: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
-00000f50: 7222 0000 0072 3700 0000 5400 0000 730e  r"...r7...T...s.
-00000f60: 0000 0008 0004 010a 0208 0c08 0908 090c  ................
-00000f70: 0972 3700 0000 290c 7248 0000 00da 0b64  .r7...).rH.....d
-00000f80: 6174 6163 6c61 7373 6573 7202 0000 0072  ataclassesr....r
-00000f90: 0300 0000 da06 7479 7069 6e67 7204 0000  ......typingr...
-00000fa0: 0072 0500 0000 7206 0000 00da 0575 7469  .r....r......uti
-00000fb0: 6c73 7208 0000 0072 0900 0000 7237 0000  lsr....r....r7..
-00000fc0: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
-00000fd0: 7222 0000 00da 083c 6d6f 6475 6c65 3e01  r".....<module>.
-00000fe0: 0000 0073 0e00 0000 0800 1001 1401 0c02  ...s............
-00000ff0: 0203 1001 124b                           .....K
+00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
+00000050: 0100 6403 6404 6c07 6d08 5a08 0100 6501  ..d.d.l.m.Z...e.
+00000060: 4700 6405 6406 8400 6406 8302 8301 5a09  G.d.d...d.....Z.
+00000070: 4700 6407 6408 8400 6408 8302 5a0a 6409  G.d.d...d...Z.d.
+00000080: 5300 290a e900 0000 0029 02da 0964 6174  S.)......)...dat
+00000090: 6163 6c61 7373 da05 6669 656c 6429 03da  aclass..field)..
+000000a0: 044c 6973 74da 084f 7074 696f 6e61 6cda  .List..Optional.
+000000b0: 0353 6574 e901 0000 0029 01da 1b66 6564  .Set.....)...fed
+000000c0: 6976 6572 7365 5f68 616e 646c 655f 6672  iverse_handle_fr
+000000d0: 6f6d 5f61 6374 6f72 6300 0000 0000 0000  om_actorc.......
+000000e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000000f0: 0073 5a01 0000 6500 5a01 6400 5a02 5500  .sZ...e.Z.d.Z.U.
+00000100: 6401 5a03 6504 6505 6402 3c00 6403 5a06  d.Z.e.e.d.<.d.Z.
+00000110: 6507 6504 1900 6505 6404 3c00 6403 5a08  e.e...e.d.<.d.Z.
+00000120: 6507 6504 1900 6505 6405 3c00 6403 5a09  e.e...e.d.<.d.Z.
+00000130: 6507 6504 1900 6505 6406 3c00 6403 5a0a  e.e...e.d.<.d.Z.
+00000140: 6507 6504 1900 6505 6407 3c00 650b 650c  e.e...e.d.<.e.e.
+00000150: 6408 8d01 5a0d 650e 6504 1900 6505 6409  d...Z.e.e...e.d.
+00000160: 3c00 650b 650c 6408 8d01 5a0f 650e 6504  <.e.e.d...Z.e.e.
+00000170: 1900 6505 640a 3c00 6403 5a10 6507 6504  ..e.d.<.d.Z.e.e.
+00000180: 1900 6505 640b 3c00 6403 5a11 6507 6504  ..e.d.<.d.Z.e.e.
+00000190: 1900 6505 640c 3c00 6403 5a12 6507 6504  ..e.d.<.d.Z.e.e.
+000001a0: 1900 6505 640d 3c00 6403 5a13 6507 6514  ..e.d.<.d.Z.e.e.
+000001b0: 1900 6505 640e 3c00 6403 5a15 6507 6516  ..e.d.<.d.Z.e.e.
+000001c0: 1900 6505 640f 3c00 6403 5a17 6507 6516  ..e.d.<.d.Z.e.e.
+000001d0: 1900 6505 6410 3c00 6403 5a18 6507 6504  ..e.d.<.d.Z.e.e.
+000001e0: 1900 6505 6411 3c00 6403 5a19 6507 6504  ..e.d.<.d.Z.e.e.
+000001f0: 1900 6505 6412 3c00 650b 651a 6408 8d01  ..e.d.<.e.e.d...
+00000200: 5a1b 651c 6514 1900 6505 6413 3c00 650b  Z.e.e...e.d.<.e.
+00000210: 651a 6408 8d01 5a1d 651c 6514 1900 6505  e.d...Z.e.e...e.
+00000220: 6414 3c00 6403 5a1e 6507 6504 1900 6505  d.<.d.Z.e.e...e.
+00000230: 6415 3c00 6416 6417 8400 5a1f 6418 6419  d.<.d.d...Z.d.d.
+00000240: 8400 5a20 641a 641b 8400 5a21 6403 5300  ..Z d.d...Z!d.S.
+00000250: 291c da06 4f62 6a65 6374 7a7a 4120 6461  )...ObjectzzA da
+00000260: 7461 636c 6173 7320 7265 7072 6573 656e  taclass represen
+00000270: 7469 6e67 2061 6e20 6041 6374 6976 6974  ting an `Activit
+00000280: 7953 7472 6561 6d73 204f 626a 6563 740a  yStreams Object.
+00000290: 2020 2020 3c68 7474 7073 3a2f 2f77 7777      <https://www
+000002a0: 2e77 332e 6f72 672f 5452 2f61 6374 6976  .w3.org/TR/activ
+000002b0: 6974 7973 7472 6561 6d73 2d76 6f63 6162  itystreams-vocab
+000002c0: 756c 6172 792f 236f 626a 6563 742d 7479  ulary/#object-ty
+000002d0: 7065 733e 605f da04 7479 7065 4eda 0d61  pes>`_..typeN..a
+000002e0: 7474 7269 6275 7465 645f 746f da09 666f  ttributed_to..fo
+000002f0: 6c6c 6f77 6572 73da 0269 64da 0970 7562  llowers..id..pub
+00000300: 6c69 7368 6564 2901 da0f 6465 6661 756c  lished)...defaul
+00000310: 745f 6661 6374 6f72 79da 0274 6fda 0263  t_factory..to..c
+00000320: 63da 046e 616d 65da 0773 756d 6d61 7279  c..name..summary
+00000330: da07 636f 6e74 656e 74da 0673 6f75 7263  ..content..sourc
+00000340: 65da 0577 6964 7468 da06 6865 6967 6874  e..width..height
+00000350: da0b 696e 5f72 6570 6c79 5f74 6fda 0375  ..in_reply_to..u
+00000360: 726c da03 7461 67da 0a61 7474 6163 686d  rl..tag..attachm
+00000370: 656e 74da 0468 7265 6663 0100 0000 0000  ent..hrefc......
+00000380: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000390: 0000 7324 0000 007c 006a 00a0 0164 01a1  ..s$...|.j...d..
+000003a0: 0101 007c 006a 0272 107c 006a 03a0 017c  ...|.j.r.|.j...|
+000003b0: 006a 02a1 0101 007c 0053 00a9 024e 7a2c  .j.....|.S...Nz,
+000003c0: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
+000003d0: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
+000003e0: 7265 616d 7323 5075 626c 6963 2904 7210  reams#Public).r.
+000003f0: 0000 00da 0361 6464 720c 0000 0072 1100  .....addr....r..
+00000400: 0000 a901 da04 7365 6c66 a900 7221 0000  ......self..r!..
+00000410: 00fa 5a2f 776f 6f64 7065 636b 6572 2f73  ..Z/woodpecker/s
+00000420: 7263 2f63 6f64 6562 6572 672e 6f72 672f  rc/codeberg.org/
+00000430: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+00000440: 7669 6e65 2f62 6f76 696e 652f 6163 7469  vine/bovine/acti
+00000450: 7669 7479 7374 7265 616d 732f 6f62 6a65  vitystreams/obje
+00000460: 6374 5f66 6163 746f 7279 2e70 79da 0961  ct_factory.py..a
+00000470: 735f 7075 626c 6963 2200 0000 7308 0000  s_public"...s...
+00000480: 000c 0106 010e 0104 017a 104f 626a 6563  .........z.Objec
+00000490: 742e 6173 5f70 7562 6c69 6363 0100 0000  t.as_publicc....
+000004a0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000004b0: 4300 0000 7324 0000 007c 006a 0072 0a7c  C...s$...|.j.r.|
+000004c0: 006a 01a0 027c 006a 00a1 0101 007c 006a  .j...|.j.....|.j
+000004d0: 03a0 0264 01a1 0101 007c 0053 0072 1d00  ...d.....|.S.r..
+000004e0: 0000 2904 720c 0000 0072 1000 0000 721e  ..).r....r....r.
+000004f0: 0000 0072 1100 0000 721f 0000 0072 2100  ...r....r....r!.
+00000500: 0000 7221 0000 0072 2200 0000 da0b 6173  ..r!...r".....as
+00000510: 5f75 6e6c 6973 7465 6428 0000 0073 0800  _unlisted(...s..
+00000520: 0000 0601 0e01 0c01 0401 7a12 4f62 6a65  ..........z.Obje
+00000530: 6374 2e61 735f 756e 6c69 7374 6564 6301  ct.as_unlistedc.
+00000540: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+00000550: 0000 0043 0000 0073 fc00 0000 6401 7c00  ...C...s....d.|.
+00000560: 6a00 6402 9c02 7d01 6900 6403 7c00 6a01  j.d...}.i.d.|.j.
+00000570: 9301 6404 7402 7c00 6a03 8301 9301 6405  ..d.t.|.j.....d.
+00000580: 7402 7c00 6a04 7c00 6a03 1800 8301 9301  t.|.j.|.j.......
+00000590: 6406 7c00 6a05 9301 6407 7c00 6a06 9301  d.|.j...d.|.j...
+000005a0: 6408 7c00 6a07 9301 6409 7c00 6a08 9301  d.|.j...d.|.j...
+000005b0: 640a 7c00 6a09 9301 640b 7c00 6a0a 9301  d.|.j...d.|.j...
+000005c0: 640c 7c00 6a0b 9301 640d 7c00 6a0c 9301  d.|.j...d.|.j...
+000005d0: 640e 7c00 6a0d 9301 640f 7c00 6a0e 9301  d.|.j...d.|.j...
+000005e0: 6410 7c00 6a0f 9301 6411 7c00 6a10 9301  d.|.j...d.|.j...
+000005f0: 6412 7c00 6a11 9301 7d02 7c02 a012 a100  d.|.j...}.|.....
+00000600: 4400 5d0a 5c02 7d03 7d04 7c04 725d 7c04  D.].\.}.}.|.r]|.
+00000610: 7c01 7c03 3c00 7153 6404 7c01 7600 726d  |.|.<.qSd.|.v.rm
+00000620: 7413 7c01 6404 1900 8301 6413 6b02 726d  t.|.d.....d.k.rm
+00000630: 7c01 6404 3d00 6405 7c01 7600 727c 7413  |.d.=.d.|.v.r|t.
+00000640: 7c01 6405 1900 8301 6413 6b02 727c 7c01  |.d.....d.k.r||.
+00000650: 6405 3d00 7c01 5300 2914 4e7a 2568 7474  d.=.|.S.).Nz%htt
+00000660: 7073 3a2f 2f77 7777 2e77 332e 6f72 672f  ps://www.w3.org/
+00000670: 6e73 2f61 6374 6976 6974 7973 7472 6561  ns/activitystrea
+00000680: 6d73 2902 7a08 4063 6f6e 7465 7874 720a  ms).z.@contextr.
+00000690: 0000 00da 0c61 7474 7269 6275 7465 6454  .....attributedT
+000006a0: 6f72 1000 0000 7211 0000 0072 0d00 0000  or....r....r....
+000006b0: 5a09 696e 5265 706c 7954 6f72 0e00 0000  Z.inReplyTor....
+000006c0: 7215 0000 0072 1200 0000 7219 0000 0072  r....r....r....r
+000006d0: 1300 0000 7214 0000 0072 1a00 0000 721b  ....r....r....r.
+000006e0: 0000 0072 1c00 0000 7216 0000 0072 1700  ...r....r....r..
+000006f0: 0000 7201 0000 0029 1472 0a00 0000 720b  ..r....).r....r.
+00000700: 0000 00da 046c 6973 7472 1000 0000 7211  .....listr....r.
+00000710: 0000 0072 0d00 0000 7218 0000 0072 0e00  ...r....r....r..
+00000720: 0000 7215 0000 0072 1200 0000 7219 0000  ..r....r....r...
+00000730: 0072 1300 0000 7214 0000 0072 1a00 0000  .r....r....r....
+00000740: 721b 0000 0072 1c00 0000 7216 0000 0072  r....r....r....r
+00000750: 1700 0000 da05 6974 656d 73da 036c 656e  ......items..len
+00000760: 2905 7220 0000 00da 0672 6573 756c 74da  ).r .....result.
+00000770: 0c65 7874 7261 5f66 6965 6c64 73da 036b  .extra_fields..k
+00000780: 6579 da05 7661 6c75 6572 2100 0000 7221  ey..valuer!...r!
+00000790: 0000 0072 2200 0000 da05 6275 696c 642e  ...r".....build.
+000007a0: 0000 0073 5a00 0000 0202 0401 06fe 0205  ...sZ...........
+000007b0: 0601 02ff 0a02 02fe 1003 02fd 0604 02fc  ................
+000007c0: 0605 02fb 0606 02fa 0607 02f9 0608 02f8  ................
+000007d0: 0609 02f7 060a 02f6 060b 02f5 060c 02f4  ................
+000007e0: 060d 02f3 060e 02f2 060f 02f1 0610 04f0  ................
+000007f0: 1013 0401 0801 0280 1802 0601 1801 0601  ................
+00000800: 0402 7a0c 4f62 6a65 6374 2e62 7569 6c64  ..z.Object.build
+00000810: 2922 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )"..__name__..__
+00000820: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000830: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
+00000840: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
+00000850: 6f6e 735f 5f72 0b00 0000 7205 0000 0072  ons__r....r....r
+00000860: 0c00 0000 720d 0000 0072 0e00 0000 7203  ....r....r....r.
+00000870: 0000 00da 0373 6574 7210 0000 0072 0600  .....setr....r..
+00000880: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000890: 0072 1400 0000 7215 0000 00da 0464 6963  .r....r......dic
+000008a0: 7472 1600 0000 da03 696e 7472 1700 0000  tr......intr....
+000008b0: 7218 0000 0072 1900 0000 7226 0000 0072  r....r....r&...r
+000008c0: 1a00 0000 7204 0000 0072 1b00 0000 721c  ....r....r....r.
+000008d0: 0000 0072 2300 0000 7224 0000 0072 2d00  ...r#...r$...r-.
+000008e0: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
+000008f0: 0072 2200 0000 7209 0000 0007 0000 0073  .r"...r........s
+00000900: 2e00 0000 0a00 0402 0803 1001 1001 1001  ................
+00000910: 1001 1601 1601 1002 1001 1001 1001 1002  ................
+00000920: 1001 1002 1001 1601 1601 1001 0802 0806  ................
+00000930: 0c06 7209 0000 0063 0000 0000 0000 0000  ..r....c........
+00000940: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000950: 733a 0000 0065 005a 0164 005a 0264 015a  s:...e.Z.d.Z.d.Z
+00000960: 0364 0d64 0364 0484 015a 0464 0564 0684  .d.d.d...Z.d.d..
+00000970: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
+00000980: 005a 0764 0b64 0c84 005a 0864 0253 0029  .Z.d.d...Z.d.S.)
+00000990: 0eda 0d4f 626a 6563 7446 6163 746f 7279  ...ObjectFactory
+000009a0: 7a34 4f62 6a65 6374 4661 6374 6f72 7920  z4ObjectFactory 
+000009b0: 7573 7561 6c6c 7920 6372 6561 7465 6420  usually created 
+000009c0: 7468 726f 7567 6820 6120 426f 7669 6e65  through a Bovine
+000009d0: 436c 6965 6e74 4e63 0300 0000 0000 0000  ClientNc........
+000009e0: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+000009f0: 7332 0000 007c 0272 0b7c 027c 005f 007c  s2...|.r.|.|._.|
+00000a00: 026a 017c 005f 0164 0053 007c 0172 1564  .j.|._.d.S.|.r.d
+00000a10: 007c 005f 007c 017c 005f 0164 0053 0074  .|._.|.|._.d.S.t
+00000a20: 0264 0183 0182 0129 024e 7a3e 596f 7520  .d.....).Nz>You 
+00000a30: 6e65 6564 2074 6f20 6569 7468 6572 2073  need to either s
+00000a40: 7065 6369 6679 2061 6374 6f72 5f69 6e66  pecify actor_inf
+00000a50: 6f72 6d61 7469 6f6e 206f 7220 6120 426f  ormation or a Bo
+00000a60: 7669 6e65 436c 6965 6e74 2903 da06 636c  vineClient)...cl
+00000a70: 6965 6e74 da0b 696e 666f 726d 6174 696f  ient..informatio
+00000a80: 6eda 0954 7970 6545 7272 6f72 2903 7220  n..TypeError).r 
+00000a90: 0000 00da 1161 6374 6f72 5f69 6e66 6f72  .....actor_infor
+00000aa0: 6d61 7469 6f6e 7238 0000 0072 2100 0000  mationr8...r!...
+00000ab0: 7221 0000 0072 2200 0000 da08 5f5f 696e  r!...r".....__in
+00000ac0: 6974 5f5f 5600 0000 7312 0000 0004 0106  it__V...s.......
+00000ad0: 010c 0104 0106 010a 0102 0202 0104 ff7a  ...............z
+00000ae0: 164f 626a 6563 7446 6163 746f 7279 2e5f  .ObjectFactory._
+00000af0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000b00: 0000 0000 0200 0000 0700 0000 4b00 0000  ............K...
+00000b10: f324 0000 0074 0064 067c 006a 0164 0119  .$...t.d.|.j.d..
+00000b20: 0064 027c 006a 01a0 0264 03a1 0164 049c  .d.|.j...d...d..
+00000b30: 037c 01a4 018e 0153 0029 077a 1543 7265  .|.....S.).z.Cre
+00000b40: 6174 6573 2061 204e 6f74 6520 4f62 6a65  ates a Note Obje
+00000b50: 6374 720d 0000 005a 044e 6f74 6572 0c00  ctr....Z.Noter..
+00000b60: 0000 a903 720b 0000 0072 0a00 0000 720c  ....r....r....r.
+00000b70: 0000 004e 7221 0000 00a9 0372 0900 0000  ...Nr!.....r....
+00000b80: 7239 0000 00da 0367 6574 a902 7220 0000  r9.....get..r ..
+00000b90: 00da 066b 7761 7267 7372 2100 0000 7221  ...kwargsr!...r!
+00000ba0: 0000 0072 2200 0000 da04 6e6f 7465 6200  ...r".....noteb.
+00000bb0: 0000 f30e 0000 0004 0208 0102 010a 0104  ................
+00000bc0: fd02 0406 fc7a 124f 626a 6563 7446 6163  .....z.ObjectFac
+00000bd0: 746f 7279 2e6e 6f74 6563 0100 0000 0000  tory.notec......
+00000be0: 0000 0000 0000 0200 0000 0700 0000 4b00  ..............K.
+00000bf0: 0000 723d 0000 0029 077a 1943 7265 6174  ..r=...).z.Creat
+00000c00: 6573 2061 6e20 4172 7469 636c 6520 4f62  es an Article Ob
+00000c10: 6a65 6374 720d 0000 005a 0741 7274 6963  jectr....Z.Artic
+00000c20: 6c65 720c 0000 0072 3e00 0000 4e72 2100  ler....r>...Nr!.
+00000c30: 0000 723f 0000 0072 4100 0000 7221 0000  ..r?...rA...r!..
+00000c40: 0072 2100 0000 7222 0000 00da 0761 7274  .r!...r".....art
+00000c50: 6963 6c65 6b00 0000 7244 0000 007a 154f  iclek...rD...z.O
+00000c60: 626a 6563 7446 6163 746f 7279 2e61 7274  bjectFactory.art
+00000c70: 6963 6c65 6301 0000 0000 0000 0000 0000  iclec...........
+00000c80: 0002 0000 0007 0000 004b 0000 0072 3d00  .........K...r=.
+00000c90: 0000 2907 7a17 4372 6561 7465 7320 616e  ..).z.Creates an
+00000ca0: 2045 7665 6e74 204f 626a 6563 7472 0d00   Event Objectr..
+00000cb0: 0000 da05 4576 656e 7472 0c00 0000 723e  ....Eventr....r>
+00000cc0: 0000 004e 7221 0000 0072 3f00 0000 7241  ...Nr!...r?...rA
+00000cd0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00000ce0: 0000 da05 6576 656e 7474 0000 0072 4400  ....eventt...rD.
+00000cf0: 0000 7a13 4f62 6a65 6374 4661 6374 6f72  ..z.ObjectFactor
+00000d00: 792e 6576 656e 7463 0200 0000 0000 0000  y.eventc........
+00000d10: 0000 0000 0300 0000 0500 0000 c300 0000  ................
+00000d20: 7334 0000 0081 017c 006a 0073 0874 0164  s4.....|.j.s.t.d
+00000d30: 0183 0182 017c 006a 00a0 027c 01a1 0149  .....|.j...|...I
+00000d40: 0064 0248 007d 0274 0364 037c 0174 047c  .d.H.}.t.d.|.t.|
+00000d50: 0283 0164 048d 0353 0029 057a 8843 7265  ...d...S.).z.Cre
+00000d60: 6174 6573 2061 206d 656e 7469 6f6e 206f  ates a mention o
+00000d70: 626a 6563 7420 666f 7220 616e 6f74 6865  bject for anothe
+00000d80: 7220 6163 746f 722e 2052 6571 7569 7265  r actor. Require
+00000d90: 7320 636c 6965 6e74 2074 6f20 6265 2073  s client to be s
+00000da0: 6574 2e0a 0a20 2020 2020 2020 203a 7061  et...        :pa
+00000db0: 7261 6d20 6163 746f 725f 746f 5f6d 656e  ram actor_to_men
+00000dc0: 7469 6f6e 3a20 5468 6520 5552 4920 6f66  tion: The URI of
+00000dd0: 2074 6865 2061 6374 6f72 2074 6f20 6d65   the actor to me
+00000de0: 6e74 696f 6e7a 2663 6c69 656e 7420 6e65  ntionz&client ne
+00000df0: 6564 7320 746f 2062 6520 7365 7420 6174  eds to be set at
+00000e00: 2063 6f6e 7374 7275 6374 696f 6e4e 5a07   constructionNZ.
+00000e10: 4d65 6e74 696f 6e29 0372 0a00 0000 721c  Mention).r....r.
+00000e20: 0000 0072 1200 0000 2905 7238 0000 0072  ...r....).r8...r
+00000e30: 3a00 0000 da0d 7072 6f78 795f 656c 656d  :.....proxy_elem
+00000e40: 656e 7472 0900 0000 7208 0000 0029 0372  entr....r....).r
+00000e50: 2000 0000 5a10 6163 746f 725f 746f 5f6d   ...Z.actor_to_m
+00000e60: 656e 7469 6f6e 5a0c 7265 6d6f 7465 5f61  entionZ.remote_a
+00000e70: 6374 6f72 7221 0000 0072 2100 0000 7222  ctorr!...r!...r"
+00000e80: 0000 00da 156d 656e 7469 6f6e 5f66 6f72  .....mention_for
+00000e90: 5f61 6374 6f72 5f75 7269 7d00 0000 7312  _actor_uri}...s.
+00000ea0: 0000 0002 8006 0508 0112 0202 0202 0102  ................
+00000eb0: 0106 0106 fd7a 234f 626a 6563 7446 6163  .....z#ObjectFac
+00000ec0: 746f 7279 2e6d 656e 7469 6f6e 5f66 6f72  tory.mention_for
+00000ed0: 5f61 6374 6f72 5f75 7269 2902 4e4e 2909  _actor_uri).NN).
+00000ee0: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00000ef0: 3100 0000 723c 0000 0072 4300 0000 7245  1...r<...rC...rE
+00000f00: 0000 0072 4700 0000 7249 0000 0072 2100  ...rG...rI...r!.
+00000f10: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00000f20: 0072 3700 0000 5300 0000 730e 0000 0008  .r7...S...s.....
+00000f30: 0004 010a 0208 0c08 0908 090c 0972 3700  .............r7.
+00000f40: 0000 4e29 0bda 0b64 6174 6163 6c61 7373  ..N)...dataclass
+00000f50: 6573 7202 0000 0072 0300 0000 da06 7479  esr....r......ty
+00000f60: 7069 6e67 7204 0000 0072 0500 0000 7206  pingr....r....r.
+00000f70: 0000 00da 0575 7469 6c73 7208 0000 0072  .....utilsr....r
+00000f80: 0900 0000 7237 0000 0072 2100 0000 7221  ....r7...r!...r!
+00000f90: 0000 0072 2100 0000 7222 0000 00da 083c  ...r!...r".....<
+00000fa0: 6d6f 6475 6c65 3e01 0000 0073 0c00 0000  module>....s....
+00000fb0: 1000 1401 0c02 0203 1001 124b            ...........K
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9308 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 9308 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6402 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6410 6406 6407 8404 5a0a 6410 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 640a 640b 8400 5a0c 6410 640c  ..Z.d.d...Z.d.d.
@@ -242,16 +242,16 @@
 00000f10: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
 00000f20: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
 00000f30: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
 00000f40: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
 00000f50: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
 00000f60: 7d06 7d05 6400 5300 290d 4e72 0600 0000  }.}.d.S.).Nr....
 00000f70: 7207 0000 0072 0800 0000 720a 0000 003e  r....r....r....>
-00000f80: 0400 0000 722f 0000 0072 3000 0000 7218  ....r/...r0...r.
-00000f90: 0000 0072 0c00 0000 720e 0000 0029 017a  ...r....r....).z
+00000f80: 0400 0000 7230 0000 0072 0c00 0000 7218  ....r0...r....r.
+00000f90: 0000 0072 2f00 0000 720e 0000 0029 017a  ...r/...r....).z
 00000fa0: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
 00000fb0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
 00000fc0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
 00000fd0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
 00000fe0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
 00000ff0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
 00001000: 3029 73da 0373 6574 7224 0000 0029 06da  0)s..setr$...)..
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1442 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 a205 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 a205 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 640c 6406 6407 8404 5a0a 640c 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 640c 640a 640b 8404 5a0c 6401  ..Z.d.d.d...Z.d.
@@ -61,35 +61,35 @@
 000003c0: 6601 6413 7c09 7c0a 6602 a104 7404 a009  f.d.|.|.f...t...
 000003d0: 7c09 a101 7404 a009 7c0a a101 6414 9c02  |...t...|...d...
 000003e0: 1600 7d0b 6415 6416 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
 000003f0: 740a 7404 a00b 7c0c a101 8301 8201 6400  t.t...|.......d.
 00000400: 0400 7d09 0400 7d02 7d0a 6400 5300 2917  ..}...}.}.d.S.).
 00000410: 4efa 1c68 7474 703a 2f2f 6578 616d 706c  N..http://exampl
 00000420: 652e 636f 6d2f 6163 746f 722f 3132 3329  e.com/actor/123)
-00000430: 01da 0269 643e 0500 0000 fa08 4063 6f6e  ...id>......@con
-00000440: 7465 7874 da05 696e 626f 7872 0700 0000  text..inboxr....
-00000450: da06 6f75 7462 6f78 da04 7479 7065 a901  ..outbox..type..
+00000430: 01da 0269 643e 0500 0000 da05 696e 626f  ...id>......inbo
+00000440: 78fa 0840 636f 6e74 6578 74da 066f 7574  x..@context..out
+00000450: 626f 78da 0474 7970 6572 0700 0000 a901  box..typer......
 00000460: fa02 3d3d 2901 7a62 2528 7079 3729 730a  ..==).zb%(py7)s.
 00000470: 7b25 2870 7937 2973 203d 2025 2870 7930  {%(py7)s = %(py0
 00000480: 2973 2825 2870 7935 2973 0a7b 2528 7079  )s(%(py5)s.{%(py
 00000490: 3529 7320 3d20 2528 7079 3329 730a 7b25  5)s = %(py3)s.{%
 000004a0: 2870 7933 2973 203d 2025 2870 7931 2973  (py3)s = %(py1)s
 000004b0: 2e6b 6579 730a 7d28 290a 7d29 0a7d 203d  .keys.}().}).} =
 000004c0: 3d20 2528 7079 3130 2973 da03 7365 74da  = %(py10)s..set.
 000004d0: 0672 6573 756c 7429 06da 0370 7930 da03  .result)...py0..
 000004e0: 7079 31da 0370 7933 da03 7079 35da 0370  py1..py3..py5..p
 000004f0: 7937 da04 7079 3130 7a0f 6173 7365 7274  y7..py10z.assert
 00000500: 2025 2870 7931 3229 73da 0470 7931 327a   %(py12)s..py12z
-00000510: 084a 6f68 6e20 446f 653e 0600 0000 da04  .John Doe>......
-00000520: 6e61 6d65 7208 0000 0072 0900 0000 7207  namer....r....r.
-00000530: 0000 0072 0a00 0000 720b 0000 005a 1130  ...r....r....Z.0
+00000510: 084a 6f68 6e20 446f 653e 0600 0000 7208  .John Doe>....r.
+00000520: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00000530: 0000 da04 6e61 6d65 7207 0000 005a 1130  ....namer....Z.0
 00000540: 3132 3334 3536 3738 3930 3132 3334 3536  1234567890123456
-00000550: da03 6b65 793e 0700 0000 7217 0000 0072  ..key>....r....r
-00000560: 0800 0000 7209 0000 0072 0700 0000 720a  ....r....r....r.
-00000570: 0000 00da 0970 7562 6c69 634b 6579 720b  .....publicKeyr.
+00000550: da03 6b65 793e 0700 0000 da09 7075 626c  ..key>......publ
+00000560: 6963 4b65 7972 0800 0000 7209 0000 0072  icKeyr....r....r
+00000570: 0a00 0000 720b 0000 0072 1700 0000 7207  ....r....r....r.
 00000580: 0000 0072 1900 0000 7a04 236b 6579 2903  ...r....z.#key).
 00000590: 7207 0000 00da 056f 776e 6572 da0c 7075  r......owner..pu
 000005a0: 626c 6963 4b65 7950 656d a901 7a12 2528  blicKeyPem..z.%(
 000005b0: 7079 3129 7320 3d3d 2025 2870 7934 2973  py1)s == %(py4)s
 000005c0: a902 7211 0000 00da 0370 7934 fa0e 6173  ..r......py4..as
 000005d0: 7365 7274 2025 2870 7936 2973 da03 7079  sert %(py6)s..py
 000005e0: 3629 1072 0400 0000 da05 6275 696c 64da  6).r......build.
@@ -152,16 +152,16 @@
 00000970: 7d01 7c01 640c 1900 640d 1900 7d02 640a  }.|.d...d...}.d.
 00000980: 7d03 7c02 7c03 6b02 7d04 7c04 73b0 7402  }.|.|.k.}.|.s.t.
 00000990: a003 6405 7c04 6601 6406 7c02 7c03 6602  ..d.|.f.d.|.|.f.
 000009a0: a104 7402 a004 7c02 a101 7402 a004 7c03  ..t...|...t...|.
 000009b0: a101 6407 9c02 1600 7d05 6408 6409 7c05  ..d.....}.d.d.|.
 000009c0: 6901 1600 7d06 7405 7402 a006 7c06 a101  i...}.t.t...|...
 000009d0: 8301 8201 6400 0400 7d02 0400 7d04 7d03  ....d...}...}.}.
-000009e0: 6400 5300 290e 4e72 0600 0000 7209 0000  d.S.).Nr....r...
-000009f0: 0072 0a00 0000 a903 7207 0000 0072 0900  .r......r....r..
+000009e0: 6400 5300 290e 4e72 0600 0000 7208 0000  d.S.).Nr....r...
+000009f0: 0072 0a00 0000 a903 7207 0000 0072 0800  .r......r....r..
 00000a00: 0000 720a 0000 0072 0c00 0000 721c 0000  ..r....r....r...
 00000a10: 0072 1d00 0000 721f 0000 0072 2000 0000  .r....r....r ...
 00000a20: 7a18 6874 7470 3a2f 2f65 7861 6d70 6c65  z.http://example
 00000a30: 2e63 6f6d 2f70 726f 7879 2901 da0a 7669  .com/proxy)...vi
 00000a40: 7369 6269 6c69 7479 da09 656e 6470 6f69  sibility..endpoi
 00000a50: 6e74 73da 0870 726f 7879 5572 6c29 0a72  nts..proxyUrl).r
 00000a60: 0400 0000 7221 0000 0072 2300 0000 7224  ....r!...r#...r$
@@ -181,15 +181,15 @@
 00000b40: 7d02 6405 6406 6901 7d03 7c02 7c03 6b02  }.d.d.i.}.|.|.k.
 00000b50: 7d04 7c04 7341 7403 a004 6408 7c04 6601  }.|.sAt...d.|.f.
 00000b60: 6409 7c02 7c03 6602 a104 7403 a005 7c02  d.|.|.f...t...|.
 00000b70: a101 7403 a005 7c03 a101 640a 9c02 1600  ..t...|...d.....
 00000b80: 7d05 640b 640c 7c05 6901 1600 7d06 7406  }.d.d.|.i...}.t.
 00000b90: 7403 a007 7c06 a101 8301 8201 6400 0400  t...|.......d...
 00000ba0: 7d02 0400 7d04 7d03 6400 5300 290d 4e72  }...}.}.d.S.).Nr
-00000bb0: 0600 0000 7209 0000 0072 0a00 0000 723c  ....r....r....r<
+00000bb0: 0600 0000 7208 0000 0072 0a00 0000 723c  ....r....r....r<
 00000bc0: 0000 0072 0b00 0000 5a05 496d 6167 65da  ...r....Z.Image.
 00000bd0: 0469 636f 6e72 0c00 0000 721c 0000 0072  .iconr....r....r
 00000be0: 1d00 0000 721f 0000 0072 2000 0000 2908  ....r....r ...).
 00000bf0: 7204 0000 0072 4400 0000 7221 0000 0072  r....rD...r!...r
 00000c00: 2300 0000 7224 0000 0072 2800 0000 7229  #...r$...r(...r)
 00000c10: 0000 0072 2a00 0000 7242 0000 0072 3900  ...r*...rB...r9.
 00000c20: 0000 7239 0000 0072 3a00 0000 da14 7465  ..r9...r:.....te
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1397 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,200 +1,195 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7505 0000  o.......*.Ndu...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 e904 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
+00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
-00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
-00000050: 6400 6402 6c07 6d08 5a08 0100 6403 6404  d.d.l.m.Z...d.d.
-00000060: 6c09 6d0a 5a0a 0100 640a 6406 6407 8404  l.m.Z...d.d.d...
-00000070: 5a0b 640a 6408 6409 8404 5a0c 6401 5300  Z.d.d.d...Z.d.S.
-00000080: 290b e900 0000 004e 2901 da09 4173 796e  )......N)...Asyn
-00000090: 634d 6f63 6be9 0100 0000 2901 da0d 4f62  cMock.....)...Ob
-000000a0: 6a65 6374 4661 6374 6f72 79da 0672 6574  jectFactory..ret
-000000b0: 7572 6e63 0000 0000 0000 0000 0000 0000  urnc............
-000000c0: 0e00 0000 0900 0000 4300 0000 73da 0100  ........C...s...
-000000d0: 0074 0064 0164 0264 039c 0283 017d 007c  .t.d.d.d.....}.|
-000000e0: 00a0 01a1 00a0 02a1 007d 0164 047c 015f  .........}.d.|._
-000000f0: 037c 01a0 04a1 007d 027c 026a 057d 037c  .|.....}.|.j.}.|
-00000100: 0383 007d 0474 067c 0483 017d 0568 0064  ...}.t.|...}.h.d
-00000110: 05a3 017d 067c 057c 066b 027d 077c 0773  ...}.|.|.k.}.|.s
-00000120: 7574 07a0 0864 067c 0766 0164 077c 057c  ut...d.|.f.d.|.|
-00000130: 0666 02a1 0464 0874 09a0 0aa1 0076 0073  .f...d.t.....v.s
-00000140: 3d74 07a0 0b74 06a1 0172 4274 07a0 0c74  =t...t...rBt...t
-00000150: 06a1 016e 0164 0864 0974 09a0 0aa1 0076  ...n.d.d.t.....v
-00000160: 0073 4e74 07a0 0b7c 02a1 0172 5374 07a0  .sNt...|...rSt..
-00000170: 0c7c 02a1 016e 0164 0974 07a0 0c7c 03a1  .|...n.d.t...|..
-00000180: 0174 07a0 0c7c 04a1 0174 07a0 0c7c 05a1  .t...|...t...|..
-00000190: 0174 07a0 0c7c 06a1 0164 0a9c 0616 007d  .t...|...d.....}
-000001a0: 0864 0b64 0c7c 0869 0116 007d 0974 0d74  .d.d.|.i...}.t.t
-000001b0: 07a0 0e7c 09a1 0183 0182 0164 0004 007d  ...|.......d...}
-000001c0: 0304 007d 0404 007d 0504 007d 077d 067c  ...}...}...}.}.|
-000001d0: 0264 0d19 007d 0a64 0e67 017d 0b7c 0a7c  .d...}.d.g.}.|.|
-000001e0: 0b6b 027d 037c 0373 af74 07a0 0864 067c  .k.}.|.s.t...d.|
-000001f0: 0366 0164 0f7c 0a7c 0b66 02a1 0474 07a0  .f.d.|.|.f...t..
-00000200: 0c7c 0aa1 0174 07a0 0c7c 0ba1 0164 109c  .|...t...|...d..
-00000210: 0216 007d 0c64 1164 127c 0c69 0116 007d  ...}.d.d.|.i...}
-00000220: 0d74 0d74 07a0 0e7c 0da1 0183 0182 0164  .t.t...|.......d
-00000230: 0004 007d 0a04 007d 037d 0b7c 0264 1319  ...}...}.}.|.d..
-00000240: 007d 0a64 0267 017d 0b7c 0a7c 0b6b 027d  .}.d.g.}.|.|.k.}
-00000250: 037c 0373 e574 07a0 0864 067c 0366 0164  .|.s.t...d.|.f.d
-00000260: 0f7c 0a7c 0b66 02a1 0474 07a0 0c7c 0aa1  .|.|.f...t...|..
-00000270: 0174 07a0 0c7c 0ba1 0164 109c 0216 007d  .t...|...d.....}
-00000280: 0c64 1164 127c 0c69 0116 007d 0d74 0d74  .d.d.|.i...}.t.t
-00000290: 07a0 0e7c 0da1 0183 0182 0164 0004 007d  ...|.......d...}
-000002a0: 0a04 007d 037d 0b64 0053 0029 144e da08  ...}.}.d.S.).N..
-000002b0: 6163 746f 725f 6964 da09 666f 6c6c 6f77  actor_id..follow
-000002c0: 6572 7329 02da 0269 6472 0700 0000 da04  ers)...idr......
-000002d0: 7465 7874 3e06 0000 00fa 0840 636f 6e74  text>......@cont
-000002e0: 6578 74da 0274 6fda 0c61 7474 7269 6275  ext..to..attribu
-000002f0: 7465 6454 6fda 0474 7970 65da 0263 63da  tedTo..type..cc.
-00000300: 0763 6f6e 7465 6e74 a901 fa02 3d3d a901  .content....==..
-00000310: 7a62 2528 7079 3729 730a 7b25 2870 7937  zb%(py7)s.{%(py7
-00000320: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
-00000330: 7935 2973 0a7b 2528 7079 3529 7320 3d20  y5)s.{%(py5)s = 
-00000340: 2528 7079 3329 730a 7b25 2870 7933 2973  %(py3)s.{%(py3)s
-00000350: 203d 2025 2870 7931 2973 2e6b 6579 730a   = %(py1)s.keys.
-00000360: 7d28 290a 7d29 0a7d 203d 3d20 2528 7079  }().}).} == %(py
-00000370: 3130 2973 da03 7365 74da 0672 6573 756c  10)s..set..resul
-00000380: 74a9 06da 0370 7930 da03 7079 31da 0370  t....py0..py1..p
-00000390: 7933 da03 7079 35da 0370 7937 da04 7079  y3..py5..py7..py
-000003a0: 3130 fa0f 6173 7365 7274 2025 2870 7931  10..assert %(py1
-000003b0: 3229 73da 0470 7931 3272 0b00 0000 7a2c  2)s..py12r....z,
-000003c0: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
-000003d0: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
-000003e0: 7265 616d 7323 5075 626c 6963 a901 7a12  reams#Public..z.
-000003f0: 2528 7079 3129 7320 3d3d 2025 2870 7934  %(py1)s == %(py4
-00000400: 2973 a902 7217 0000 00da 0370 7934 fa0e  )s..r......py4..
-00000410: 6173 7365 7274 2025 2870 7936 2973 da03  assert %(py6)s..
-00000420: 7079 3672 0e00 0000 290f 7204 0000 00da  py6r....).r.....
-00000430: 046e 6f74 65da 0961 735f 7075 626c 6963  .note..as_public
-00000440: 720f 0000 00da 0562 7569 6c64 da04 6b65  r......build..ke
-00000450: 7973 7213 0000 00da 0a40 7079 7465 7374  ysr......@pytest
-00000460: 5f61 72da 115f 6361 6c6c 5f72 6570 7263  _ar.._call_reprc
-00000470: 6f6d 7061 7265 da0c 4070 795f 6275 696c  ompare..@py_buil
-00000480: 7469 6e73 da06 6c6f 6361 6c73 da18 5f73  tins..locals.._s
-00000490: 686f 756c 645f 7265 7072 5f67 6c6f 6261  hould_repr_globa
-000004a0: 6c5f 6e61 6d65 da09 5f73 6166 6572 6570  l_name.._saferep
-000004b0: 72da 0e41 7373 6572 7469 6f6e 4572 726f  r..AssertionErro
-000004c0: 72da 135f 666f 726d 6174 5f65 7870 6c61  r.._format_expla
-000004d0: 6e61 7469 6f6e 290e da0e 6f62 6a65 6374  nation)...object
-000004e0: 5f66 6163 746f 7279 7223 0000 0072 1400  _factoryr#...r..
-000004f0: 0000 da0b 4070 795f 6173 7365 7274 32da  ....@py_assert2.
-00000500: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
-00000510: 795f 6173 7365 7274 36da 0b40 7079 5f61  y_assert6..@py_a
-00000520: 7373 6572 7439 da0b 4070 795f 6173 7365  ssert9..@py_asse
-00000530: 7274 38da 0c40 7079 5f66 6f72 6d61 7431  rt8..@py_format1
-00000540: 31da 0c40 7079 5f66 6f72 6d61 7431 33da  1..@py_format13.
-00000550: 0b40 7079 5f61 7373 6572 7430 da0b 4070  .@py_assert0..@p
-00000560: 795f 6173 7365 7274 33da 0b40 7079 5f66  y_assert3..@py_f
-00000570: 6f72 6d61 7435 da0b 4070 795f 666f 726d  ormat5..@py_form
-00000580: 6174 37a9 0072 3b00 0000 fa5f 2f77 6f6f  at7..r;...._/woo
-00000590: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-000005a0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
-000005b0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-000005c0: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
-000005d0: 6561 6d73 2f74 6573 745f 6f62 6a65 6374  eams/test_object
-000005e0: 5f66 6163 746f 7279 2e70 79da 1374 6573  _factory.py..tes
-000005f0: 745f 6f62 6a65 6374 5f66 6163 746f 7279  t_object_factory
-00000600: 0700 0000 736a 0000 000e 010c 0206 0108  ....sj..........
-00000610: 0102 0202 0726 f902 070e f902 0704 f904  .....&..........
-00000620: 0706 f902 0702 f902 0704 f902 0702 f904  ................
-00000630: 0706 f904 0706 f902 0702 f902 0704 f902  ................
-00000640: 0702 f904 0704 f902 0702 f902 0702 f902  ................
-00000650: 0702 f902 0702 f902 0702 f902 0702 f902  ................
-00000660: 0702 f902 0718 f902 0702 f902 0718 f96c  ...............l
-00000670: 0970 0172 3d00 0000 6300 0000 0000 0000  .p.r=...c.......
-00000680: 0000 0000 0013 0000 0009 0000 00c3 0000  ................
-00000690: 0073 8402 0000 8101 7400 8300 7d00 7400  .s......t...}.t.
-000006a0: 8300 7d01 6401 7d02 7c01 7c00 6a01 6a02  ..}.d.}.|.|.j.j.
-000006b0: 5f03 7404 a005 6402 7c02 6403 6404 6405  _.t...d.|.d.d.d.
-000006c0: 9c04 a101 7c01 6a06 5f03 7407 7c00 6406  ....|.j._.t.|.d.
-000006d0: 8d01 7d03 7c03 a008 7c02 a101 4900 6400  ..}.|...|...I.d.
-000006e0: 4800 7d04 7c04 a009 a100 7d05 7c05 6a0a  H.}.|.....}.|.j.
-000006f0: 7d06 7c06 8300 7d07 740b 7c07 8301 7d08  }.|...}.t.|...}.
-00000700: 6800 6407 a301 7d09 7c08 7c09 6b02 7d0a  h.d...}.|.|.k.}.
-00000710: 7c0a 738c 740c a00d 6408 7c0a 6601 6409  |.s.t...d.|.f.d.
-00000720: 7c08 7c09 6602 a104 640a 740e a00f a100  |.|.f...d.t.....
-00000730: 7600 7354 740c a010 740b a101 7259 740c  v.sTt...t...rYt.
-00000740: a011 740b a101 6e01 640a 640b 740e a00f  ..t...n.d.d.t...
-00000750: a100 7600 7365 740c a010 7c05 a101 726a  ..v.set...|...rj
-00000760: 740c a011 7c05 a101 6e01 640b 740c a011  t...|...n.d.t...
-00000770: 7c06 a101 740c a011 7c07 a101 740c a011  |...t...|...t...
-00000780: 7c08 a101 740c a011 7c09 a101 640c 9c06  |...t...|...d...
-00000790: 1600 7d0b 640d 640e 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
-000007a0: 7412 740c a013 7c0c a101 8301 8201 6400  t.t...|.......d.
-000007b0: 0400 7d06 0400 7d07 0400 7d08 0400 7d0a  ..}...}...}...}.
-000007c0: 7d09 7c05 640f 1900 7d0d 6410 7d0e 7c0d  }.|.d...}.d.}.|.
-000007d0: 7c0e 6b02 7d06 7c06 73c5 740c a00d 6408  |.k.}.|.s.t...d.
-000007e0: 7c06 6601 6411 7c0d 7c0e 6602 a104 740c  |.f.d.|.|.f...t.
-000007f0: a011 7c0d a101 740c a011 7c0e a101 6412  ..|...t...|...d.
-00000800: 9c02 1600 7d0f 6413 6414 7c0f 6901 1600  ....}.d.d.|.i...
-00000810: 7d10 7412 740c a013 7c10 a101 8301 8201  }.t.t...|.......
-00000820: 6400 0400 7d0d 0400 7d06 7d0e 7c05 6415  d...}...}.}.|.d.
-00000830: 1900 7d0d 7c0d 7c02 6b02 7d06 7c06 9001  ..}.|.|.k.}.|...
-00000840: 7306 740c a00d 6408 7c06 6601 6416 7c0d  s.t...d.|.f.d.|.
-00000850: 7c02 6602 a104 740c a011 7c0d a101 6417  |.f...t...|...d.
-00000860: 740e a00f a100 7600 73ef 740c a010 7c02  t.....v.s.t...|.
-00000870: a101 72f4 740c a011 7c02 a101 6e01 6417  ..r.t...|...n.d.
-00000880: 6418 9c02 1600 7d11 6419 641a 7c11 6901  d.....}.d.d.|.i.
-00000890: 1600 7d12 7412 740c a013 7c12 a101 8301  ..}.t.t...|.....
-000008a0: 8201 6400 0400 7d0d 7d06 7c05 641b 1900  ..d...}.}.|.d...
-000008b0: 7d0d 641c 7d0e 7c0d 7c0e 6b02 7d06 7c06  }.d.}.|.|.k.}.|.
-000008c0: 9001 733a 740c a00d 6408 7c06 6601 6411  ..s:t...d.|.f.d.
-000008d0: 7c0d 7c0e 6602 a104 740c a011 7c0d a101  |.|.f...t...|...
-000008e0: 740c a011 7c0e a101 6412 9c02 1600 7d0f  t...|...d.....}.
-000008f0: 6413 6414 7c0f 6901 1600 7d10 7412 740c  d.d.|.i...}.t.t.
-00000900: a013 7c10 a101 8301 8201 6400 0400 7d0d  ..|.......d...}.
-00000910: 0400 7d06 7d0e 6400 5300 291d 4e7a 1468  ..}.}.d.S.).Nz.h
-00000920: 7474 7073 3a2f 2f72 656d 6f74 652f 616c  ttps://remote/al
-00000930: 6963 657a 2568 7474 7073 3a2f 2f77 7777  icez%https://www
-00000940: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
-00000950: 6974 7973 7472 6561 6d73 da06 5065 7273  itystreams..Pers
-00000960: 6f6e 5a06 616c 7973 7361 2904 720a 0000  onZ.alyssa).r...
-00000970: 0072 0800 0000 720d 0000 00da 1170 7265  .r....r......pre
-00000980: 6665 7272 6564 5573 6572 6e61 6d65 2901  ferredUsername).
-00000990: da06 636c 6965 6e74 3e04 0000 00da 046e  ..client>......n
-000009a0: 616d 65da 0468 7265 6672 0d00 0000 720a  ame..hrefr....r.
-000009b0: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
-000009c0: 0000 da07 6d65 6e74 696f 6e72 1500 0000  ....mentionr....
-000009d0: 721c 0000 0072 1d00 0000 720d 0000 00da  r....r....r.....
-000009e0: 074d 656e 7469 6f6e 721e 0000 0072 1f00  .Mentionr....r..
-000009f0: 0000 7221 0000 0072 2200 0000 7242 0000  ..r!...r"...rB..
-00000a00: 0029 017a 1225 2870 7931 2973 203d 3d20  .).z.%(py1)s == 
-00000a10: 2528 7079 3329 73da 0a72 656d 6f74 655f  %(py3)s..remote_
-00000a20: 7572 6929 0272 1700 0000 7218 0000 007a  uri).r....r....z
-00000a30: 0e61 7373 6572 7420 2528 7079 3529 7372  .assert %(py5)sr
-00000a40: 1900 0000 7241 0000 007a 0d61 6c79 7373  ....rA...z.alyss
-00000a50: 6140 7265 6d6f 7465 2914 7202 0000 0072  a@remote).r....r
-00000a60: 4000 0000 da03 6765 74da 0c72 6574 7572  @.....get..retur
-00000a70: 6e5f 7661 6c75 65da 046a 736f 6eda 0564  n_value..json..d
-00000a80: 756d 7073 7209 0000 0072 0400 0000 da15  umpsr....r......
-00000a90: 6d65 6e74 696f 6e5f 666f 725f 6163 746f  mention_for_acto
-00000aa0: 725f 7572 6972 2500 0000 7226 0000 0072  r_urir%...r&...r
-00000ab0: 1300 0000 7227 0000 0072 2800 0000 7229  ....r'...r(...r)
-00000ac0: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
-00000ad0: 0000 722d 0000 0072 2e00 0000 2913 5a0b  ..r-...r....).Z.
-00000ae0: 6d6f 636b 5f63 6c69 656e 745a 0d6d 6f63  mock_clientZ.moc
-00000af0: 6b5f 7265 7370 6f6e 7365 7245 0000 0072  k_responserE...r
-00000b00: 2f00 0000 5a0e 6d65 6e74 696f 6e5f 6f62  /...Z.mention_ob
-00000b10: 6a65 6374 7243 0000 0072 3000 0000 7231  jectrC...r0...r1
-00000b20: 0000 0072 3200 0000 7233 0000 0072 3400  ...r2...r3...r4.
-00000b30: 0000 7235 0000 0072 3600 0000 7237 0000  ..r5...r6...r7..
-00000b40: 0072 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
-00000b50: da0b 4070 795f 666f 726d 6174 34da 0b40  ..@py_format4..@
-00000b60: 7079 5f66 6f72 6d61 7436 723b 0000 0072  py_format6r;...r
-00000b70: 3b00 0000 723c 0000 00da 1a74 6573 745f  ;...r<.....test_
-00000b80: 6d65 6e74 696f 6e5f 666f 725f 6163 746f  mention_for_acto
-00000b90: 725f 7572 691b 0000 0073 2600 0000 0280  r_uri....s&.....
-00000ba0: 0601 0601 0401 0a02 0402 0202 0201 0201  ................
-00000bb0: 0201 04fc 08ff 0a09 1002 0801 d602 6a01  ..............j.
-00000bc0: 7e01 7001 724d 0000 0029 0272 0500 0000  ~.p.rM...).r....
-00000bd0: 4e29 0dda 0862 7569 6c74 696e 7372 2900  N)...builtinsr).
-00000be0: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
-00000bf0: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
-00000c00: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
-00000c10: 6572 2700 0000 7248 0000 00da 0d75 6e69  er'...rH.....uni
-00000c20: 7474 6573 742e 6d6f 636b 7202 0000 0072  ttest.mockr....r
-00000c30: 2f00 0000 7204 0000 0072 3d00 0000 724d  /...r....r=...rM
-00000c40: 0000 0072 3b00 0000 723b 0000 0072 3b00  ...r;...r;...r;.
-00000c50: 0000 723c 0000 00da 083c 6d6f 6475 6c65  ..r<.....<module
-00000c60: 3e01 0000 0073 0a00 0000 2200 0c01 0c02  >....s....".....
-00000c70: 0a03 0e14                                ....
+00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
+00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
+00000060: 640a 6406 6407 8404 5a0a 640a 6408 6409  d.d.d...Z.d.d.d.
+00000070: 8404 5a0b 6401 5300 290b e900 0000 004e  ..Z.d.S.)......N
+00000080: 2901 da09 4173 796e 634d 6f63 6be9 0100  )...AsyncMock...
+00000090: 0000 2901 da0d 4f62 6a65 6374 4661 6374  ..)...ObjectFact
+000000a0: 6f72 79da 0672 6574 7572 6e63 0000 0000  ory..returnc....
+000000b0: 0000 0000 0000 0000 0e00 0000 0900 0000  ................
+000000c0: 4300 0000 73da 0100 0074 0064 0164 0264  C...s....t.d.d.d
+000000d0: 039c 0283 017d 007c 00a0 01a1 00a0 02a1  .....}.|........
+000000e0: 007d 0164 047c 015f 037c 01a0 04a1 007d  .}.d.|._.|.....}
+000000f0: 027c 026a 057d 037c 0383 007d 0474 067c  .|.j.}.|...}.t.|
+00000100: 0483 017d 0568 0064 05a3 017d 067c 057c  ...}.h.d...}.|.|
+00000110: 066b 027d 077c 0773 7574 07a0 0864 067c  .k.}.|.sut...d.|
+00000120: 0766 0164 077c 057c 0666 02a1 0464 0874  .f.d.|.|.f...d.t
+00000130: 09a0 0aa1 0076 0073 3d74 07a0 0b74 06a1  .....v.s=t...t..
+00000140: 0172 4274 07a0 0c74 06a1 016e 0164 0864  .rBt...t...n.d.d
+00000150: 0974 09a0 0aa1 0076 0073 4e74 07a0 0b7c  .t.....v.sNt...|
+00000160: 02a1 0172 5374 07a0 0c7c 02a1 016e 0164  ...rSt...|...n.d
+00000170: 0974 07a0 0c7c 03a1 0174 07a0 0c7c 04a1  .t...|...t...|..
+00000180: 0174 07a0 0c7c 05a1 0174 07a0 0c7c 06a1  .t...|...t...|..
+00000190: 0164 0a9c 0616 007d 0864 0b64 0c7c 0869  .d.....}.d.d.|.i
+000001a0: 0116 007d 0974 0d74 07a0 0e7c 09a1 0183  ...}.t.t...|....
+000001b0: 0182 0164 0004 007d 0304 007d 0404 007d  ...d...}...}...}
+000001c0: 0504 007d 077d 067c 0264 0d19 007d 0a64  ...}.}.|.d...}.d
+000001d0: 0e67 017d 0b7c 0a7c 0b6b 027d 037c 0373  .g.}.|.|.k.}.|.s
+000001e0: af74 07a0 0864 067c 0366 0164 0f7c 0a7c  .t...d.|.f.d.|.|
+000001f0: 0b66 02a1 0474 07a0 0c7c 0aa1 0174 07a0  .f...t...|...t..
+00000200: 0c7c 0ba1 0164 109c 0216 007d 0c64 1164  .|...d.....}.d.d
+00000210: 127c 0c69 0116 007d 0d74 0d74 07a0 0e7c  .|.i...}.t.t...|
+00000220: 0da1 0183 0182 0164 0004 007d 0a04 007d  .......d...}...}
+00000230: 037d 0b7c 0264 1319 007d 0a64 0267 017d  .}.|.d...}.d.g.}
+00000240: 0b7c 0a7c 0b6b 027d 037c 0373 e574 07a0  .|.|.k.}.|.s.t..
+00000250: 0864 067c 0366 0164 0f7c 0a7c 0b66 02a1  .d.|.f.d.|.|.f..
+00000260: 0474 07a0 0c7c 0aa1 0174 07a0 0c7c 0ba1  .t...|...t...|..
+00000270: 0164 109c 0216 007d 0c64 1164 127c 0c69  .d.....}.d.d.|.i
+00000280: 0116 007d 0d74 0d74 07a0 0e7c 0da1 0183  ...}.t.t...|....
+00000290: 0182 0164 0004 007d 0a04 007d 037d 0b64  ...d...}...}.}.d
+000002a0: 0053 0029 144e da08 6163 746f 725f 6964  .S.).N..actor_id
+000002b0: da09 666f 6c6c 6f77 6572 7329 02da 0269  ..followers)...i
+000002c0: 6472 0700 0000 da04 7465 7874 3e06 0000  dr......text>...
+000002d0: 00da 0c61 7474 7269 6275 7465 6454 6ffa  ...attributedTo.
+000002e0: 0840 636f 6e74 6578 74da 0474 7970 65da  .@context..type.
+000002f0: 0763 6f6e 7465 6e74 da02 746f da02 6363  .content..to..cc
+00000300: a901 fa02 3d3d a901 7a62 2528 7079 3729  ....==..zb%(py7)
+00000310: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
+00000320: 7930 2973 2825 2870 7935 2973 0a7b 2528  y0)s(%(py5)s.{%(
+00000330: 7079 3529 7320 3d20 2528 7079 3329 730a  py5)s = %(py3)s.
+00000340: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
+00000350: 2973 2e6b 6579 730a 7d28 290a 7d29 0a7d  )s.keys.}().}).}
+00000360: 203d 3d20 2528 7079 3130 2973 da03 7365   == %(py10)s..se
+00000370: 74da 0672 6573 756c 74a9 06da 0370 7930  t..result....py0
+00000380: da03 7079 31da 0370 7933 da03 7079 35da  ..py1..py3..py5.
+00000390: 0370 7937 da04 7079 3130 fa0f 6173 7365  .py7..py10..asse
+000003a0: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
+000003b0: 3272 0e00 0000 7a2c 6874 7470 733a 2f2f  2r....z,https://
+000003c0: 7777 772e 7733 2e6f 7267 2f6e 732f 6163  www.w3.org/ns/ac
+000003d0: 7469 7669 7479 7374 7265 616d 7323 5075  tivitystreams#Pu
+000003e0: 626c 6963 a901 7a12 2528 7079 3129 7320  blic..z.%(py1)s 
+000003f0: 3d3d 2025 2870 7934 2973 a902 7217 0000  == %(py4)s..r...
+00000400: 00da 0370 7934 fa0e 6173 7365 7274 2025  ...py4..assert %
+00000410: 2870 7936 2973 da03 7079 3672 0f00 0000  (py6)s..py6r....
+00000420: 290f 7204 0000 00da 046e 6f74 65da 0961  ).r......note..a
+00000430: 735f 7075 626c 6963 720d 0000 00da 0562  s_publicr......b
+00000440: 7569 6c64 da04 6b65 7973 7213 0000 00da  uild..keysr.....
+00000450: 0a40 7079 7465 7374 5f61 72da 115f 6361  .@pytest_ar.._ca
+00000460: 6c6c 5f72 6570 7263 6f6d 7061 7265 da0c  ll_reprcompare..
+00000470: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
+00000480: 6361 6c73 da18 5f73 686f 756c 645f 7265  cals.._should_re
+00000490: 7072 5f67 6c6f 6261 6c5f 6e61 6d65 da09  pr_global_name..
+000004a0: 5f73 6166 6572 6570 72da 0e41 7373 6572  _saferepr..Asser
+000004b0: 7469 6f6e 4572 726f 72da 135f 666f 726d  tionError.._form
+000004c0: 6174 5f65 7870 6c61 6e61 7469 6f6e 290e  at_explanation).
+000004d0: da0e 6f62 6a65 6374 5f66 6163 746f 7279  ..object_factory
+000004e0: 7223 0000 0072 1400 0000 da0b 4070 795f  r#...r......@py_
+000004f0: 6173 7365 7274 32da 0b40 7079 5f61 7373  assert2..@py_ass
+00000500: 6572 7434 da0b 4070 795f 6173 7365 7274  ert4..@py_assert
+00000510: 36da 0b40 7079 5f61 7373 6572 7439 da0b  6..@py_assert9..
+00000520: 4070 795f 6173 7365 7274 38da 0c40 7079  @py_assert8..@py
+00000530: 5f66 6f72 6d61 7431 31da 0c40 7079 5f66  _format11..@py_f
+00000540: 6f72 6d61 7431 33da 0b40 7079 5f61 7373  ormat13..@py_ass
+00000550: 6572 7430 da0b 4070 795f 6173 7365 7274  ert0..@py_assert
+00000560: 33da 0b40 7079 5f66 6f72 6d61 7435 da0b  3..@py_format5..
+00000570: 4070 795f 666f 726d 6174 37a9 0072 3b00  @py_format7..r;.
+00000580: 0000 fa5f 2f77 6f6f 6470 6563 6b65 722f  ..._/woodpecker/
+00000590: 7372 632f 636f 6465 6265 7267 2e6f 7267  src/codeberg.org
+000005a0: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+000005b0: 6f76 696e 652f 626f 7669 6e65 2f61 6374  ovine/bovine/act
+000005c0: 6976 6974 7973 7472 6561 6d73 2f74 6573  ivitystreams/tes
+000005d0: 745f 6f62 6a65 6374 5f66 6163 746f 7279  t_object_factory
+000005e0: 2e70 79da 1374 6573 745f 6f62 6a65 6374  .py..test_object
+000005f0: 5f66 6163 746f 7279 0600 0000 736a 0000  _factory....sj..
+00000600: 000e 010c 0206 0108 0102 0202 0726 f902  .............&..
+00000610: 070e f902 0704 f904 0706 f902 0702 f902  ................
+00000620: 0704 f902 0702 f904 0706 f904 0706 f902  ................
+00000630: 0702 f902 0704 f902 0702 f904 0704 f902  ................
+00000640: 0702 f902 0702 f902 0702 f902 0702 f902  ................
+00000650: 0702 f902 0702 f902 0702 f902 0718 f902  ................
+00000660: 0702 f902 0718 f96c 0970 0172 3d00 0000  .......l.p.r=...
+00000670: 6300 0000 0000 0000 0000 0000 0012 0000  c...............
+00000680: 0009 0000 00c3 0000 0073 6c02 0000 8101  .........sl.....
+00000690: 7400 8300 7d00 6401 7d01 6402 7c01 6403  t...}.d.}.d.|.d.
+000006a0: 6404 6405 9c04 7c00 6a01 5f02 7403 7c00  d.d...|.j._.t.|.
+000006b0: 6406 8d01 7d02 7c02 a004 7c01 a101 4900  d...}.|...|...I.
+000006c0: 6400 4800 7d03 7c03 a005 a100 7d04 7c04  d.H.}.|.....}.|.
+000006d0: 6a06 7d05 7c05 8300 7d06 7407 7c06 8301  j.}.|...}.t.|...
+000006e0: 7d07 6800 6407 a301 7d08 7c07 7c08 6b02  }.h.d...}.|.|.k.
+000006f0: 7d09 7c09 7381 7408 a009 6408 7c09 6601  }.|.s.t...d.|.f.
+00000700: 6409 7c07 7c08 6602 a104 640a 740a a00b  d.|.|.f...d.t...
+00000710: a100 7600 7349 7408 a00c 7407 a101 724e  ..v.sIt...t...rN
+00000720: 7408 a00d 7407 a101 6e01 640a 640b 740a  t...t...n.d.d.t.
+00000730: a00b a100 7600 735a 7408 a00c 7c04 a101  ....v.sZt...|...
+00000740: 725f 7408 a00d 7c04 a101 6e01 640b 7408  r_t...|...n.d.t.
+00000750: a00d 7c05 a101 7408 a00d 7c06 a101 7408  ..|...t...|...t.
+00000760: a00d 7c07 a101 7408 a00d 7c08 a101 640c  ..|...t...|...d.
+00000770: 9c06 1600 7d0a 640d 640e 7c0a 6901 1600  ....}.d.d.|.i...
+00000780: 7d0b 740e 7408 a00f 7c0b a101 8301 8201  }.t.t...|.......
+00000790: 6400 0400 7d05 0400 7d06 0400 7d07 0400  d...}...}...}...
+000007a0: 7d09 7d08 7c04 640f 1900 7d0c 6410 7d0d  }.}.|.d...}.d.}.
+000007b0: 7c0c 7c0d 6b02 7d05 7c05 73ba 7408 a009  |.|.k.}.|.s.t...
+000007c0: 6408 7c05 6601 6411 7c0c 7c0d 6602 a104  d.|.f.d.|.|.f...
+000007d0: 7408 a00d 7c0c a101 7408 a00d 7c0d a101  t...|...t...|...
+000007e0: 6412 9c02 1600 7d0e 6413 6414 7c0e 6901  d.....}.d.d.|.i.
+000007f0: 1600 7d0f 740e 7408 a00f 7c0f a101 8301  ..}.t.t...|.....
+00000800: 8201 6400 0400 7d0c 0400 7d05 7d0d 7c04  ..d...}...}.}.|.
+00000810: 6415 1900 7d0c 7c0c 7c01 6b02 7d05 7c05  d...}.|.|.k.}.|.
+00000820: 73fa 7408 a009 6408 7c05 6601 6416 7c0c  s.t...d.|.f.d.|.
+00000830: 7c01 6602 a104 7408 a00d 7c0c a101 6417  |.f...t...|...d.
+00000840: 740a a00b a100 7600 73e3 7408 a00c 7c01  t.....v.s.t...|.
+00000850: a101 72e8 7408 a00d 7c01 a101 6e01 6417  ..r.t...|...n.d.
+00000860: 6418 9c02 1600 7d10 6419 641a 7c10 6901  d.....}.d.d.|.i.
+00000870: 1600 7d11 740e 7408 a00f 7c11 a101 8301  ..}.t.t...|.....
+00000880: 8201 6400 0400 7d0c 7d05 7c04 641b 1900  ..d...}.}.|.d...
+00000890: 7d0c 641c 7d0d 7c0c 7c0d 6b02 7d05 7c05  }.d.}.|.|.k.}.|.
+000008a0: 9001 732e 7408 a009 6408 7c05 6601 6411  ..s.t...d.|.f.d.
+000008b0: 7c0c 7c0d 6602 a104 7408 a00d 7c0c a101  |.|.f...t...|...
+000008c0: 7408 a00d 7c0d a101 6412 9c02 1600 7d0e  t...|...d.....}.
+000008d0: 6413 6414 7c0e 6901 1600 7d0f 740e 7408  d.d.|.i...}.t.t.
+000008e0: a00f 7c0f a101 8301 8201 6400 0400 7d0c  ..|.......d...}.
+000008f0: 0400 7d05 7d0d 6400 5300 291d 4e7a 1468  ..}.}.d.S.).Nz.h
+00000900: 7474 7073 3a2f 2f72 656d 6f74 652f 616c  ttps://remote/al
+00000910: 6963 657a 2568 7474 7073 3a2f 2f77 7777  icez%https://www
+00000920: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
+00000930: 6974 7973 7472 6561 6d73 da06 5065 7273  itystreams..Pers
+00000940: 6f6e 5a06 616c 7973 7361 2904 720b 0000  onZ.alyssa).r...
+00000950: 0072 0800 0000 720c 0000 00da 1170 7265  .r....r......pre
+00000960: 6665 7272 6564 5573 6572 6e61 6d65 2901  ferredUsername).
+00000970: da06 636c 6965 6e74 3e04 0000 00da 0468  ..client>......h
+00000980: 7265 66da 046e 616d 6572 0b00 0000 720c  ref..namer....r.
+00000990: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
+000009a0: 0000 da07 6d65 6e74 696f 6e72 1500 0000  ....mentionr....
+000009b0: 721c 0000 0072 1d00 0000 720c 0000 00da  r....r....r.....
+000009c0: 074d 656e 7469 6f6e 721e 0000 0072 1f00  .Mentionr....r..
+000009d0: 0000 7221 0000 0072 2200 0000 7241 0000  ..r!...r"...rA..
+000009e0: 0029 017a 1225 2870 7931 2973 203d 3d20  .).z.%(py1)s == 
+000009f0: 2528 7079 3329 73da 0a72 656d 6f74 655f  %(py3)s..remote_
+00000a00: 7572 6929 0272 1700 0000 7218 0000 007a  uri).r....r....z
+00000a10: 0e61 7373 6572 7420 2528 7079 3529 7372  .assert %(py5)sr
+00000a20: 1900 0000 7242 0000 007a 0d61 6c79 7373  ....rB...z.alyss
+00000a30: 6140 7265 6d6f 7465 2910 7202 0000 00da  a@remote).r.....
+00000a40: 0d70 726f 7879 5f65 6c65 6d65 6e74 da0c  .proxy_element..
+00000a50: 7265 7475 726e 5f76 616c 7565 7204 0000  return_valuer...
+00000a60: 00da 156d 656e 7469 6f6e 5f66 6f72 5f61  ...mention_for_a
+00000a70: 6374 6f72 5f75 7269 7225 0000 0072 2600  ctor_urir%...r&.
+00000a80: 0000 7213 0000 0072 2700 0000 7228 0000  ..r....r'...r(..
+00000a90: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
+00000aa0: 722c 0000 0072 2d00 0000 722e 0000 0029  r,...r-...r....)
+00000ab0: 125a 0b6d 6f63 6b5f 636c 6965 6e74 7245  .Z.mock_clientrE
+00000ac0: 0000 0072 2f00 0000 5a0e 6d65 6e74 696f  ...r/...Z.mentio
+00000ad0: 6e5f 6f62 6a65 6374 7243 0000 0072 3000  n_objectrC...r0.
+00000ae0: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
+00000af0: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
+00000b00: 7237 0000 0072 3800 0000 7239 0000 0072  r7...r8...r9...r
+00000b10: 3a00 0000 da0b 4070 795f 666f 726d 6174  :.....@py_format
+00000b20: 34da 0b40 7079 5f66 6f72 6d61 7436 723b  4..@py_format6r;
+00000b30: 0000 0072 3b00 0000 723c 0000 00da 1a74  ...r;...r<.....t
+00000b40: 6573 745f 6d65 6e74 696f 6e5f 666f 725f  est_mention_for_
+00000b50: 6163 746f 725f 7572 691a 0000 0073 1e00  actor_uri....s..
+00000b60: 0000 0280 0601 0401 0203 0201 0201 0201  ................
+00000b70: 0afc 0a07 1002 0801 d602 6a01 7c01 7001  ..........j.|.p.
+00000b80: 724b 0000 0029 0272 0500 0000 4e29 0cda  rK...).r....N)..
+00000b90: 0862 7569 6c74 696e 7372 2900 0000 da19  .builtinsr).....
+00000ba0: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+00000bb0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+00000bc0: 7469 6f6e da07 7265 7772 6974 6572 2700  tion..rewriter'.
+00000bd0: 0000 da0d 756e 6974 7465 7374 2e6d 6f63  ....unittest.moc
+00000be0: 6b72 0200 0000 722f 0000 0072 0400 0000  kr....r/...r....
+00000bf0: 723d 0000 0072 4b00 0000 723b 0000 0072  r=...rK...r;...r
+00000c00: 3b00 0000 723b 0000 0072 3c00 0000 da08  ;...r;...r<.....
+00000c10: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000c20: 0026 000c 020a 030e 14                   .&.......
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1034 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0a04 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 0a04 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 640b 6405 6406 8404 5a08 640b  Z...d.d.d...Z.d.
 00000060: 6407 6408 8404 5a09 640b 6409 640a 8404  d.d...Z.d.d.d...
 00000070: 5a0a 6401 5300 290c e900 0000 004e e901  Z.d.S.)......N..
```

### Comparing `bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 3103 0000  o.......*.Nd1...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 3103 0000  o.......p6Yd1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6407 6405 6406 8404 5a08 6401  Z...d.d.d...Z.d.
 00000060: 5300 2908 e900 0000 004e e901 0000 0029  S.)......N.....)
 00000070: 01da 154f 7264 6572 6564 436f 6c6c 6563  ...OrderedCollec
```

### Comparing `bovine-0.1.3/bovine/activitystreams/activity_factory.py` & `bovine-0.1.4/bovine/activitystreams/activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/object_factory.py` & `bovine-0.1.4/bovine/activitystreams/object_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from dataclasses import dataclass, field
 from typing import List, Optional, Set
 
 from .utils import fediverse_handle_from_actor
 
 
 @dataclass
@@ -127,15 +126,14 @@
         """Creates a mention object for another actor. Requires client to be set.
 
         :param actor_to_mention: The URI of the actor to mention"""
 
         if not self.client:
             raise TypeError("client needs to be set at construction")
 
-        response = await self.client.client.get(actor_to_mention)
-        remote_actor = json.loads(await response.text())
+        remote_actor = await self.client.proxy_element(actor_to_mention)
 
         return Object(
             type="Mention",
             href=actor_to_mention,
             name=fediverse_handle_from_actor(remote_actor),
         )
```

### Comparing `bovine-0.1.3/bovine/activitystreams/test_activity_factory.py` & `bovine-0.1.4/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/test_actor.py` & `bovine-0.1.4/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/test_object_factory.py` & `bovine-0.1.4/bovine/activitystreams/test_object_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from unittest.mock import AsyncMock
 
 from .object_factory import ObjectFactory
 
 
 def test_object_factory() -> None:
     object_factory = ObjectFactory({"id": "actor_id", "followers": "followers"})
@@ -22,27 +21,22 @@
 
     assert result["to"] == ["https://www.w3.org/ns/activitystreams#Public"]
     assert result["cc"] == ["followers"]
 
 
 async def test_mention_for_actor_uri() -> None:
     mock_client = AsyncMock()
-    mock_response = AsyncMock()
     remote_uri = "https://remote/alice"
 
-    mock_client.client.get.return_value = mock_response
-
-    mock_response.text.return_value = json.dumps(
-        {
-            "@context": "https://www.w3.org/ns/activitystreams",
-            "id": remote_uri,
-            "type": "Person",
-            "preferredUsername": "alyssa",
-        }
-    )
+    mock_client.proxy_element.return_value = {
+        "@context": "https://www.w3.org/ns/activitystreams",
+        "id": remote_uri,
+        "type": "Person",
+        "preferredUsername": "alyssa",
+    }
 
     object_factory = ObjectFactory(client=mock_client)
 
     mention_object = await object_factory.mention_for_actor_uri(remote_uri)
     mention = mention_object.build()
 
     assert set(mention.keys()) == {"@context", "type", "href", "name"}
```

### Comparing `bovine-0.1.3/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.1.4/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.1.4/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/utils/__init__.py` & `bovine-0.1.4/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.4/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 3209 0000  o.......*.Nd2...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 3209 0000  o.......p6Yd2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6504 6404 6505 6604  m.Z...d.e.d.e.f.
 00000050: 6405 6406 8404 5a06 6403 6501 6504 6505  d.d...Z.d.e.e.e.
 00000060: 4200 1900 6404 6501 6505 1900 6604 6407  B...d.e.e...f.d.
 00000070: 6408 8404 5a07 6409 640a 8400 5a08 6403  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.1.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc` & `bovine-0.1.4/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 1303 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 1303 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6404  d.l.Z.d.d...Z.d.
 00000040: 6405 8400 5a02 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000050: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
 00000060: 0000 0007 0000 0043 0000 0073 6000 0000  .......C...s`...
 00000070: 6401 7c00 7600 7217 7400 6402 7c00 6401  d.|.v.r.t.d.|.d.
```

### Comparing `bovine-0.1.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 da08 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 da08 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6405 6406  Z.m.Z.m.Z...d.d.
 00000070: 8400 5a0d 6407 6408 8400 5a0e 6409 640a  ..Z.d.d...Z.d.d.
@@ -30,19 +30,19 @@
 000001d0: 740d 7407 a00e 7c05 a101 8301 8201 6400  t.t...|.......d.
 000001e0: 0400 7d03 7d02 6400 5300 290f 4eda 044e  ..}.}.d.S.).N..N
 000001f0: 6f74 65da 0761 6363 6f75 6e74 fa11 6163  ote..account..ac
 00000200: 636f 756e 742f 666f 6c6c 6f77 6572 73a9  count/followers.
 00000210: 03da 0474 7970 65da 0d61 7474 7269 6275  ...type..attribu
 00000220: 7465 645f 746f da09 666f 6c6c 6f77 6572  ted_to..follower
 00000230: 73da 0263 63da 0274 6fda 0473 616d 653e  s..cc..to..same>
-00000240: 0500 0000 7a2c 6874 7470 733a 2f2f 7777  ....z,https://ww
-00000250: 772e 7733 2e6f 7267 2f6e 732f 6163 7469  w.w3.org/ns/acti
-00000260: 7669 7479 7374 7265 616d 7323 5075 626c  vitystreams#Publ
-00000270: 6963 7211 0000 0072 1000 0000 720a 0000  icr....r....r...
-00000280: 0072 0f00 0000 a901 fa02 3d3d 2901 7a12  .r........==).z.
+00000240: 0500 0000 7211 0000 0072 1000 0000 720a  ....r....r....r.
+00000250: 0000 0072 0f00 0000 7a2c 6874 7470 733a  ...r....z,https:
+00000260: 2f2f 7777 772e 7733 2e6f 7267 2f6e 732f  //www.w3.org/ns/
+00000270: 6163 7469 7669 7479 7374 7265 616d 7323  activitystreams#
+00000280: 5075 626c 6963 a901 fa02 3d3d 2901 7a12  Public....==).z.
 00000290: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
 000002a0: 2973 da0a 7265 6369 7069 656e 7473 2902  )s..recipients).
 000002b0: da03 7079 30da 0370 7933 7a0e 6173 7365  ..py0..py3z.asse
 000002c0: 7274 2025 2870 7935 2973 da03 7079 3529  rt %(py5)s..py5)
 000002d0: 0f72 0200 0000 da09 6173 5f70 7562 6c69  .r......as_publi
 000002e0: 6372 0f00 0000 da03 6164 6472 1000 0000  cr......addr....
 000002f0: da05 6275 696c 6472 0700 0000 da0a 4070  ..buildr......@p
```

### Comparing `bovine-0.1.3/bovine/activitystreams/utils/print.py` & `bovine-0.1.4/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/activitystreams/utils/test_utils.py` & `bovine-0.1.4/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/__init__.py` & `bovine-0.1.4/bovine/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2722 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 a20a 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 a20a 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6403 6404 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 6d0a 5a0a 0100 6500 a00b 650c a101 5a0d  m.Z...e...e...Z.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/bearer.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/bearer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1794 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0207 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 0207 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000060: 8400 6407 8302 5a07 6401 5300 2908 e900  ..d...Z.d.S.)...
 00000070: 0000 004e 2901 da0b 6765 745f 676d 745f  ...N)...get_gmt_
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/event_source.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/event_source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1520 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f005 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 f005 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a05 6402 5300  d.d...d...Z.d.S.
 00000060: 2906 e900 0000 0029 01da 0444 6963 744e  )......)...DictN
 00000070: 2901 da0f 5365 7276 6572 5365 6e74 4576  )...ServerSentEv
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/lookup_account.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 1303 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 1303 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6501 a005 6506 a101 5a07 6404 6502  ..e...e...Z.d.e.
 00000060: 6a08 6405 6509 6406 650a 6606 6407 6408  j.d.e.d.e.f.d.d.
 00000070: 8404 5a0b 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/moo_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 3001 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b90b 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 b90b 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 8400 5a0c 4700  m.Z...d.d...Z.G.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b403 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 b403 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6404 6503  e.f.d.d...Z.d.e.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/signed_http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1150 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7e04 0000  o.......*.Nd~...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 7e04 0000  o.......p6Yd~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 4400 0000 6500  .....@...sD...e.
 00000070: 5a01 6400 5a02 6401 5a03 640d 6403 6404  Z.d.Z.d.Z.d.d.d.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 ce0c 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 ce0c 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 609 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 6102 0000  o.......*.Nda...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 6102 0000  o.......p6Yda...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6408 6406 6407 8404 5a0a 6401 5300 2909  d.d.d...Z.d.S.).
 00000070: e900 0000 004e 2901 da09 4173 796e 634d  .....N)...AsyncM
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1149 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7d04 0000  o.......*.Nd}...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 7d04 0000  o.......p6Yd}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 6d0a  d.d.l.m.Z.m.Z.m.
 00000060: 5a0a 0100 6404 6405 8400 5a0b 6406 6407  Z...d.d...Z.d.d.
 00000070: 8400 5a0c 6408 6409 8400 5a0d 640a 640b  ..Z.d.d...Z.d.d.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 3f01 0000  o.......*.Nd?...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 3f01 0000  o.......p6Yd?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 8400 5a09 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0e66 6574 6368 5f6e  .....)...fetch_n
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 8104 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 8104 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a09  Z.m.Z...d.d.l.Z.
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405 6406  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.1.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0a02 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 0a02 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a08 6400 6403  Z...d.d.l.Z.d.d.
 00000060: 6c09 6d0a 5a0a 0100 6404 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6406 6407 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
```

### Comparing `bovine-0.1.3/bovine/clients/bearer.py` & `bovine-0.1.4/bovine/clients/bearer.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/event_source.py` & `bovine-0.1.4/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/lookup_account.py` & `bovine-0.1.4/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/moo_auth.py` & `bovine-0.1.4/bovine/clients/moo_auth.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/nodeinfo.py` & `bovine-0.1.4/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/signed_http.py` & `bovine-0.1.4/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/signed_http_methods.py` & `bovine-0.1.4/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/test_event_source.py` & `bovine-0.1.4/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/test_lookup_account.py` & `bovine-0.1.4/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/test_signed_http.py` & `bovine-0.1.4/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/clients/test_signed_http_client.py` & `bovine-0.1.4/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/__init__.py` & `bovine-0.1.4/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 4141 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 2d10 0000  o.......*.Nd-...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 2d10 0000  o.......p6Yd-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6406 6407 6c0c 6d0d 5a0d 6d0e 5a0e  Z.d.d.l.m.Z.m.Z.
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/helper.cpython-310.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2664 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 680a 0000  o.......*.Ndh...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 680a 0000  o.......p6Ydh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/http_signature.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 4008 0000  o.......*.Nd@...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 4008 0000  o.......p6Yd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6405  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6500 a00c 650d a101 5a0e 6407 6408  ..e...e...Z.d.d.
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7e0b 0000  o.......*.Nd~...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 7e0b 0000  o.......p6Yd~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c04 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6404 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f204 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 f204 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 a001 6502 a101 5a03  d.l.Z.e...e...Z.
 00000040: 4700 6402 6403 8400 6403 8302 5a04 6404  G.d.d...d...Z.d.
 00000050: 6405 8400 5a05 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000060: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000070: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 2199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9708 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 9708 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
 00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
 00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
 00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
 00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 4995 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 8313 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 8313 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
 00000070: 5a0e 0100 6403 6405 6c0f 6d10 5a10 0100  Z...d.d.l.m.Z...
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 8003 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 8003 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6403 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6406 6407  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 5081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 d913 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 d913 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6402 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6402 6405  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6406 6407 8400 5a0e  l.m.Z...d.d...Z.
```

### Comparing `bovine-0.1.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b704 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 b704 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0953 6967 6e61 7475  .....)...Signatu
```

### Comparing `bovine-0.1.3/bovine/crypto/helper.py` & `bovine-0.1.4/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/http_signature.py` & `bovine-0.1.4/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/signature_checker.py` & `bovine-0.1.4/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/signature_parser.py` & `bovine-0.1.4/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/test.py` & `bovine-0.1.4/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/test_crypto.py` & `bovine-0.1.4/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/test_helper.py` & `bovine-0.1.4/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/test_http_signature.py` & `bovine-0.1.4/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/crypto/test_signature_parser.py` & `bovine-0.1.4/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/msg.py` & `bovine-0.1.4/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/types.py` & `bovine-0.1.4/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/utils/__init__.py` & `bovine-0.1.4/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.4/bovine/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9b02 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 9b02 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6503 6403 6503 6404 6503 6405 6504 6608  e.d.e.d.e.d.e.f.
 00000050: 6406 6407 8404 5a05 6408 6503 6405 6502  d.d...Z.d.e.d.e.
 00000060: 6503 6501 6503 1900 6602 1900 6604 6409  e.e.e...f...f.d.
 00000070: 640a 8404 5a06 640b 5300 290c e900 0000  d...Z.d.S.).....
```

### Comparing `bovine-0.1.3/bovine/utils/__pycache__/date.cpython-310.pyc` & `bovine-0.1.4/bovine/utils/__pycache__/date.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0702 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 0702 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 6d02 5a02  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6505 6602 6404 6405 8404 5a06 6406 6505  e.f.d.d...Z.d.e.
 00000060: 6403 6500 6604 6407 6408 8404 5a07 640f  d.e.f.d.d...Z.d.
 00000070: 640a 6500 640b 6508 6403 6509 6606 640c  d.e.d.e.d.e.f.d.
```

### Comparing `bovine-0.1.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 761 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f902 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 f902 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100  l.m.Z.m.Z.m.Z...
 00000070: 640c 6406 6407 8404 5a0d 640c 6408 6409  d.d.d...Z.d.d.d.
```

### Comparing `bovine-0.1.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 c401 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 c401 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1670 6172 7365 5f66 6564 6976 6572 7365  .parse_fediverse
```

### Comparing `bovine-0.1.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 191 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 bf00 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 bf00 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1777 6562 6669 6e67 6572 5f72 6573 706f  .webfinger_respo
```

### Comparing `bovine-0.1.3/bovine/utils/date.py` & `bovine-0.1.4/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/utils/msg/__init__.py` & `bovine-0.1.4/bovine/utils/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.4/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 1210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 ba04 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 ba04 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6406 6407 8400  d.l.m.Z...d.d...
 00000060: 5a07 6408 6500 6a08 6409 6509 640a 6509  Z.d.e.j.d.e.d.e.
 00000070: 6606 640b 640c 8404 5a0a 640d 640e 8400  f.d.d...Z.d.d...
```

### Comparing `bovine-0.1.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.4/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 599 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 5702 0000  o.......*.NdW...
+00000000: 6f0d 0d0a 0000 0000 7036 5964 5702 0000  o.......p6YdW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6412 6405 6406 8404 5a0a 6412 6407 6408  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 6506 6a0c a00d 6409 640a 640b  ..Z.e.j...d.d.d.
```

### Comparing `bovine-0.1.3/bovine/utils/msg/__pycache__/validation.cpython-310.pyc` & `bovine-0.1.4/bovine/utils/msg/__pycache__/validation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 17:02:34 2023 UTC, .py size: 261 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0501 0000  o.......*.Nd....
+00000000: 6f0d 0d0a 0000 0000 7036 5964 0501 0000  o.......p6Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6500 6401 4200 6602 6402 6403 8404 5a01  e.d.B.f.d.d...Z.
 00000040: 6404 6502 6602 6405 6406 8404 5a03 6401  d.e.f.d.d...Z.d.
 00000050: 5300 2907 da03 746f 734e 6301 0000 0000  S.)...tosNc.....
 00000060: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
 00000070: 0000 0073 1e00 0000 7c00 6400 7500 7206  ...s....|.d.u.r.
```

### Comparing `bovine-0.1.3/bovine/utils/msg/test_validation.py` & `bovine-0.1.4/bovine/utils/msg/test_validation.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/bovine/utils/test_date.py` & `bovine-0.1.4/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.3/pyproject.toml` & `bovine-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.1.3"
+version = "0.1.4"
 description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
```

### Comparing `bovine-0.1.3/PKG-INFO` & `bovine-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.1.3
+Version: 0.1.4
 Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -46,7 +46,12 @@
 - [aiohttp](https://docs.aiohttp.org/en/stable/index.html) for http requests.
 - [quart](https://quart.palletsprojects.com/en/latest/) as a webserver.
 - [cryptography](https://cryptography.io/en/latest/).
 - [pytest](https://docs.pytest.org/en/7.3.x/) for testing.
 - [ruff](https://pypi.org/project/ruff/) for linting.
 
 
+## Todo
+
+- [ ] Document FediVerse crawler behavior in server tutorial
+
+
```

