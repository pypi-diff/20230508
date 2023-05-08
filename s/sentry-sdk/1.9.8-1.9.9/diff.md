# Comparing `tmp/sentry-sdk-1.9.8.tar.gz` & `tmp/sentry-sdk-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-sdk-1.9.8.tar", last modified: Mon Sep  5 12:02:34 2022, max compression
+gzip compressed data, was "sentry-sdk-1.9.9.tar", last modified: Mon Sep 26 13:01:53 2022, max compression
```

## Comparing `sentry-sdk-1.9.8.tar` & `sentry-sdk-1.9.9.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:34.825051 sentry-sdk-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2022-09-05 12:02:34.825051 sentry-sdk-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:34.817051 sentry-sdk-1.9.8/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/_functools.py
--rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)    16515 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     9341 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (121)    23088 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:34.821051 sentry-sdk-1.9.8/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (121)     6755 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4781 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8177 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (121)    11710 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (121)    15733 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (121)     6488 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/bottle.py
--rw-r--r--   0 runner    (1001) docker     (121)     9746 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/celery.py
--rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:34.821051 sentry-sdk-1.9.8/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (121)    18875 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5916 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     5394 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (121)     7322 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8151 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     8130 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (121)     8656 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)     7424 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5867 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/quart.py
--rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (121)    11311 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:34.825051 sentry-sdk-1.9.8/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8465 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)    19764 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (121)     7273 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (121)    11351 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     7353 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    16853 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)    16443 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)    29857 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17008 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17126 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)    28545 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:02:34.817051 sentry-sdk-1.9.8/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2022-09-05 12:02:34.000000 sentry-sdk-1.9.8/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-09-05 12:02:34.000000 sentry-sdk-1.9.8/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 12:02:34.000000 sentry-sdk-1.9.8/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 12:02:34.000000 sentry-sdk-1.9.8/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-09-05 12:02:34.000000 sentry-sdk-1.9.8/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-05 12:02:34.000000 sentry-sdk-1.9.8/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 12:02:34.825051 sentry-sdk-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-09-05 12:02:14.000000 sentry-sdk-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:53.124182 sentry-sdk-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6842 2022-09-26 13:01:53.124182 sentry-sdk-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:53.100181 sentry-sdk-1.9.9/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16947 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9400 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23052 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:53.120182 sentry-sdk-1.9.9/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     6755 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4781 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8177 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11710 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15733 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6488 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9746 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/celery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:53.120182 sentry-sdk-1.9.9/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (121)    18973 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5916 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5394 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7322 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8151 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8130 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8656 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4520 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7424 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5867 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/quart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11311 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:53.120182 sentry-sdk-1.9.9/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8465 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19751 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7273 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11363 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17778 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    16853 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16443 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28850 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17154 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17126 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28537 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:01:53.104182 sentry-sdk-1.9.9/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6842 2022-09-26 13:01:53.000000 sentry-sdk-1.9.9/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-09-26 13:01:53.000000 sentry-sdk-1.9.9/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 13:01:53.000000 sentry-sdk-1.9.9/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 13:01:53.000000 sentry-sdk-1.9.9/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-09-26 13:01:53.000000 sentry-sdk-1.9.9/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-26 13:01:53.000000 sentry-sdk-1.9.9/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-26 13:01:53.124182 sentry-sdk-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-09-26 13:01:39.000000 sentry-sdk-1.9.9/setup.py
```

### Comparing `sentry-sdk-1.9.8/LICENSE` & `sentry-sdk-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/PKG-INFO` & `sentry-sdk-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 1.9.8
+Version: 1.9.9
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: BSD
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-sdk Version: 1.9.8 Summary: Python client
+Metadata-Version: 2.1 Name: sentry-sdk Version: 1.9.9 Summary: Python client
 for Sentry (https://sentry.io) Home-page: https://github.com/getsentry/sentry-
 python Author: Sentry Team and Contributors Author-email: hello@sentry.io
 License: BSD Project-URL: Documentation, https://docs.sentry.io/platforms/
 python/ Project-URL: Changelog, https://github.com/getsentry/sentry-python/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Web Environment Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
```

### Comparing `sentry-sdk-1.9.8/README.md` & `sentry-sdk-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/__init__.py` & `sentry-sdk-1.9.9/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/_compat.py` & `sentry-sdk-1.9.9/sentry_sdk/_compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     T = TypeVar("T")
 
 
 PY2 = sys.version_info[0] == 2
 
 if PY2:
-    import urlparse  # noqa
+    import urlparse
 
     text_type = unicode  # noqa
 
     string_types = (str, text_type)
     number_types = (int, long, float)  # noqa
     int_types = (int, long)  # noqa
     iteritems = lambda x: x.iteritems()  # noqa: B301
@@ -35,15 +35,15 @@
 
 else:
     import urllib.parse as urlparse  # noqa
 
     text_type = str
     string_types = (text_type,)  # type: Tuple[type]
     number_types = (int, float)  # type: Tuple[type, type]
-    int_types = (int,)  # noqa
+    int_types = (int,)
     iteritems = lambda x: x.items()
 
     def implements_str(x):
         # type: (T) -> T
         return x
 
     def reraise(tp, value, tb=None):
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/_functools.py` & `sentry-sdk-1.9.9/sentry_sdk/_functools.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/_queue.py` & `sentry-sdk-1.9.9/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/_types.py` & `sentry-sdk-1.9.9/sentry_sdk/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         "error",
         "crash",
         "transaction",
         "security",
         "attachment",
         "session",
         "internal",
+        "profile",
     ]
     SessionStatus = Literal["ok", "exited", "crashed", "abnormal"]
     EndpointType = Literal["store", "envelope"]
 
     DurationUnit = Literal[
         "nanosecond",
         "microsecond",
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/api.py` & `sentry-sdk-1.9.9/sentry_sdk/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     **kwargs  # type: Any
 ):
     # type: (...) -> None
     return Hub.current.add_breadcrumb(crumb, hint, **kwargs)
 
 
 @overload
-def configure_scope():  # noqa: F811
+def configure_scope():
     # type: () -> ContextManager[Scope]
     pass
 
 
 @overload
 def configure_scope(  # noqa: F811
     callback,  # type: Callable[[Scope], None]
@@ -126,15 +126,15 @@
     callback=None,  # type: Optional[Callable[[Scope], None]]
 ):
     # type: (...) -> Optional[ContextManager[Scope]]
     return Hub.current.configure_scope(callback)
 
 
 @overload
-def push_scope():  # noqa: F811
+def push_scope():
     # type: () -> ContextManager[Scope]
     pass
 
 
 @overload
 def push_scope(  # noqa: F811
     callback,  # type: Callable[[Scope], None]
@@ -147,39 +147,39 @@
 def push_scope(  # noqa: F811
     callback=None,  # type: Optional[Callable[[Scope], None]]
 ):
     # type: (...) -> Optional[ContextManager[Scope]]
     return Hub.current.push_scope(callback)
 
 
-@scopemethod  # noqa
+@scopemethod
 def set_tag(key, value):
     # type: (str, Any) -> None
     return Hub.current.scope.set_tag(key, value)
 
 
-@scopemethod  # noqa
+@scopemethod
 def set_context(key, value):
     # type: (str, Dict[str, Any]) -> None
     return Hub.current.scope.set_context(key, value)
 
 
-@scopemethod  # noqa
+@scopemethod
 def set_extra(key, value):
     # type: (str, Any) -> None
     return Hub.current.scope.set_extra(key, value)
 
 
-@scopemethod  # noqa
+@scopemethod
 def set_user(value):
     # type: (Optional[Dict[str, Any]]) -> None
     return Hub.current.scope.set_user(value)
 
 
-@scopemethod  # noqa
+@scopemethod
 def set_level(value):
     # type: (str) -> None
     return Hub.current.scope.set_level(value)
 
 
 @hubmethod
 def flush(
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/attachments.py` & `sentry-sdk-1.9.9/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/client.py` & `sentry-sdk-1.9.9/sentry_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from sentry_sdk.serializer import serialize
 from sentry_sdk.transport import make_transport
 from sentry_sdk.consts import DEFAULT_OPTIONS, SDK_INFO, ClientConstructor
 from sentry_sdk.integrations import setup_integrations
 from sentry_sdk.utils import ContextVar
 from sentry_sdk.sessions import SessionFlusher
 from sentry_sdk.envelope import Envelope
+from sentry_sdk.profiler import setup_profiler
 from sentry_sdk.tracing_utils import has_tracestate_enabled, reinflate_tracestate
 
 from sentry_sdk._types import MYPY
 
 if MYPY:
     from typing import Any
     from typing import Callable
@@ -126,14 +127,21 @@
                 with_auto_enabling_integrations=self.options[
                     "auto_enabling_integrations"
                 ],
             )
         finally:
             _client_init_debug.set(old_debug)
 
+        profiles_sample_rate = self.options["_experiments"].get("profiles_sample_rate")
+        if profiles_sample_rate is not None and profiles_sample_rate > 0:
+            try:
+                setup_profiler(self.options)
+            except ValueError as e:
+                logger.debug(str(e))
+
     @property
     def dsn(self):
         # type: () -> Optional[str]
         """Returns the configured DSN as string."""
         return self.options["dsn"]
 
     def _prepare_event(
@@ -399,14 +407,15 @@
                 headers["trace"] = dynamic_sampling_context
 
             envelope = Envelope(headers=headers)
 
             if is_transaction:
                 if "profile" in event_opt:
                     event_opt["profile"]["transaction_id"] = event_opt["event_id"]
+                    event_opt["profile"]["environment"] = event_opt.get("environment")
                     event_opt["profile"]["version_name"] = event_opt.get("release", "")
                     envelope.add_profile(event_opt.pop("profile"))
                 envelope.add_transaction(event_opt)
             else:
                 envelope.add_event(event_opt)
 
             for attachment in attachments or ():
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/consts.py` & `sentry-sdk-1.9.9/sentry_sdk/consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         "Experiments",
         {
             "max_spans": Optional[int],
             "record_sql_params": Optional[bool],
             "smart_transaction_trimming": Optional[bool],
             "propagate_tracestate": Optional[bool],
             "custom_measurements": Optional[bool],
-            "enable_profiling": Optional[bool],
+            "profiles_sample_rate": Optional[float],
+            "profiler_mode": Optional[str],
         },
         total=False,
     )
 
 DEFAULT_QUEUE_SIZE = 100
 DEFAULT_MAX_BREADCRUMBS = 100
 
@@ -99,13 +100,13 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "1.9.8"
+VERSION = "1.9.9"
 SDK_INFO = {
     "name": "sentry.python",
     "version": VERSION,
     "packages": [{"name": "pypi:sentry-sdk", "version": VERSION}],
 }
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/debug.py` & `sentry-sdk-1.9.9/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/envelope.py` & `sentry-sdk-1.9.9/sentry_sdk/envelope.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,16 @@
             return "attachment"
         elif ty == "transaction":
             return "transaction"
         elif ty == "event":
             return "error"
         elif ty == "client_report":
             return "internal"
+        elif ty == "profile":
+            return "profile"
         else:
             return "default"
 
     def get_bytes(self):
         # type: (...) -> bytes
         return self.payload.get_bytes()
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/hub.py` & `sentry-sdk-1.9.9/sentry_sdk/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,15 +542,15 @@
                 self.client and self.client.options["_experiments"].get("max_spans")
             ) or 1000
             transaction.init_span_recorder(maxlen=max_spans)
 
         return transaction
 
     @overload
-    def push_scope(  # noqa: F811
+    def push_scope(
         self, callback=None  # type: Optional[None]
     ):
         # type: (...) -> ContextManager[Scope]
         pass
 
     @overload
     def push_scope(  # noqa: F811
@@ -591,30 +591,30 @@
         Try to use the context manager :py:meth:`push_scope` instead.
         """
         rv = self._stack.pop()
         assert self._stack, "stack must have at least one layer"
         return rv
 
     @overload
-    def configure_scope(  # noqa: F811
+    def configure_scope(
         self, callback=None  # type: Optional[None]
     ):
         # type: (...) -> ContextManager[Scope]
         pass
 
     @overload
     def configure_scope(  # noqa: F811
         self, callback  # type: Callable[[Scope], None]
     ):
         # type: (...) -> None
         pass
 
     def configure_scope(  # noqa
         self, callback=None  # type: Optional[Callable[[Scope], None]]
-    ):  # noqa
+    ):
         # type: (...) -> Optional[ContextManager[Scope]]
 
         """
         Reconfigures the scope.
 
         :param callback: If provided, call the callback with the current scope.
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/__init__.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/_wsgi_common.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/aiohttp.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/argv.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/asgi.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/atexit.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/aws_lambda.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/beam.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/boto3.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/bottle.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/celery.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/celery.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/chalice.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/dedupe.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/django/__init__.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 from sentry_sdk.integrations.django.transactions import LEGACY_RESOLVER
 from sentry_sdk.integrations.django.templates import (
     get_template_frame_from_exception,
     patch_templates,
 )
 from sentry_sdk.integrations.django.middleware import patch_django_middlewares
+from sentry_sdk.integrations.django.signals_handlers import patch_signals
 from sentry_sdk.integrations.django.views import patch_views
 
 
 if MYPY:
     from typing import Any
     from typing import Callable
     from typing import Dict
@@ -208,14 +209,15 @@
                 id(value),
             )
 
         _patch_channels()
         patch_django_middlewares()
         patch_views()
         patch_templates()
+        patch_signals()
 
 
 _DRF_PATCHED = False
 _DRF_PATCH_LOCK = threading.Lock()
 
 
 def _patch_drf():
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/django/asgi.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/django/middleware.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/django/templates.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/django/transactions.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/django/views.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/excepthook.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/excepthook.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/executing.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/falcon.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/fastapi.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/flask.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/gcp.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/gnu_backtrace.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/httpx.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/logging.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/modules.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/pure_eval.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/pyramid.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/quart.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/redis.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/redis.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/rq.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/sanic.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/serverless.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/serverless.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def overload(x):
         # type: (F) -> F
         return x
 
 
 @overload
-def serverless_function(f, flush=True):  # noqa: F811
+def serverless_function(f, flush=True):
     # type: (F, bool) -> F
     pass
 
 
 @overload
 def serverless_function(f=None, flush=True):  # noqa: F811
     # type: (None, bool) -> Callable[[F], F]
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/spark/spark_driver.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/spark/spark_worker.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/sqlalchemy.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/starlette.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/starlette.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     from starlette.middleware.exceptions import ExceptionMiddleware  # type: ignore
 except ImportError:
     # Startlette 0.19.1
     from starlette.exceptions import ExceptionMiddleware  # type: ignore
 
 try:
     # Optional dependency of Starlette to parse form data.
-    import multipart  # type: ignore # noqa: F401
+    import multipart  # type: ignore
 except ImportError:
     multipart = None
 
 
 _DEFAULT_TRANSACTION_NAME = "generic Starlette request"
 
 TRANSACTION_STYLE_VALUES = ("endpoint", "url")
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/stdlib.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/threading.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/tornado.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/trytond.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/integrations/wsgi.py` & `sentry-sdk-1.9.9/sentry_sdk/integrations/wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     capture_internal_exceptions,
     event_from_exception,
 )
 from sentry_sdk._compat import PY2, reraise, iteritems
 from sentry_sdk.tracing import Transaction, TRANSACTION_SOURCE_ROUTE
 from sentry_sdk.sessions import auto_session_tracking
 from sentry_sdk.integrations._wsgi_common import _filter_headers
-from sentry_sdk.profiler import profiling
+from sentry_sdk.profiler import start_profiling
 
 from sentry_sdk._types import MYPY
 
 if MYPY:
     from typing import Callable
     from typing import Dict
     from typing import Iterator
@@ -127,15 +127,15 @@
                         op="http.server",
                         name="generic WSGI request",
                         source=TRANSACTION_SOURCE_ROUTE,
                     )
 
                     with hub.start_transaction(
                         transaction, custom_sampling_context={"wsgi_environ": environ}
-                    ), profiling(transaction, hub):
+                    ), start_profiling(transaction, hub):
                         try:
                             rv = self.app(
                                 environ,
                                 partial(
                                     _sentry_start_response, start_response, transaction
                                 ),
                             )
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/scope.py` & `sentry-sdk-1.9.9/sentry_sdk/scope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/serializer.py` & `sentry-sdk-1.9.9/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/session.py` & `sentry-sdk-1.9.9/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/sessions.py` & `sentry-sdk-1.9.9/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/tracing.py` & `sentry-sdk-1.9.9/sentry_sdk/tracing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import uuid
 import random
 import time
-import platform
 
 from datetime import datetime, timedelta
 
 import sentry_sdk
 
-from sentry_sdk.profiler import has_profiling_enabled
 from sentry_sdk.utils import logger
 from sentry_sdk._types import MYPY
 
 
 if MYPY:
     import typing
 
     from typing import Optional
     from typing import Any
     from typing import Dict
     from typing import List
     from typing import Tuple
     from typing import Iterator
-    from sentry_sdk.profiler import Sampler
 
     from sentry_sdk._types import SamplingContext, MeasurementUnit
 
 
 # Transaction source
 # see https://develop.sentry.dev/sdk/event-payloads/transaction/#transaction-annotations
 TRANSACTION_SOURCE_CUSTOM = "custom"
@@ -576,16 +573,16 @@
         self.parent_sampled = parent_sampled
         # if tracestate isn't inherited and set here, it will get set lazily,
         # either the first time an outgoing request needs it for a header or the
         # first time an event needs it for inclusion in the captured data
         self._sentry_tracestate = sentry_tracestate
         self._third_party_tracestate = third_party_tracestate
         self._measurements = {}  # type: Dict[str, Any]
-        self._profile = None  # type: Optional[Sampler]
-        self._baggage = baggage  # type: Optional[Baggage]
+        self._profile = None  # type: Optional[Dict[str, Any]]
+        self._baggage = baggage
 
     def __repr__(self):
         # type: () -> str
         return (
             "<%s(name=%r, op=%r, trace_id=%r, span_id=%r, parent_span_id=%r, sampled=%r, source=%r)>"
             % (
                 self.__class__.__name__,
@@ -669,34 +666,16 @@
             "contexts": {"trace": self.get_trace_context()},
             "tags": self._tags,
             "timestamp": self.timestamp,
             "start_timestamp": self.start_timestamp,
             "spans": finished_spans,
         }
 
-        if (
-            has_profiling_enabled(hub)
-            and hub.client is not None
-            and self._profile is not None
-        ):
-            event["profile"] = {
-                "device_os_name": platform.system(),
-                "device_os_version": platform.release(),
-                "duration_ns": self._profile.duration,
-                "environment": hub.client.options["environment"],
-                "platform": "python",
-                "platform_version": platform.python_version(),
-                "profile_id": uuid.uuid4().hex,
-                "profile": self._profile.to_json(),
-                "trace_id": self.trace_id,
-                "transaction_id": None,  # Gets added in client.py
-                "transaction_name": self.name,
-                "version_code": "",  # TODO: Determine appropriate value. Currently set to empty string so profile will not get rejected.
-                "version_name": None,  # Gets added in client.py
-            }
+        if hub.client is not None and self._profile is not None:
+            event["profile"] = self._profile
 
         if has_custom_measurements_enabled():
             event["measurements"] = self._measurements
 
         return hub.capture_event(event)
 
     def set_measurement(self, name, value, unit=""):
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/tracing_utils.py` & `sentry-sdk-1.9.9/sentry_sdk/tracing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,22 +455,24 @@
         third_party_items = ""
         mutable = True
 
         if header:
             for item in header.split(","):
                 if "=" not in item:
                     continue
-                item = item.strip()
-                key, val = item.split("=")
-                if Baggage.SENTRY_PREFIX_REGEX.match(key):
-                    baggage_key = unquote(key.split("-")[1])
-                    sentry_items[baggage_key] = unquote(val)
-                    mutable = False
-                else:
-                    third_party_items += ("," if third_party_items else "") + item
+
+                with capture_internal_exceptions():
+                    item = item.strip()
+                    key, val = item.split("=")
+                    if Baggage.SENTRY_PREFIX_REGEX.match(key):
+                        baggage_key = unquote(key.split("-")[1])
+                        sentry_items[baggage_key] = unquote(val)
+                        mutable = False
+                    else:
+                        third_party_items += ("," if third_party_items else "") + item
 
         return Baggage(sentry_items, third_party_items, mutable)
 
     @classmethod
     def populate_from_transaction(cls, transaction):
         # type: (Transaction) -> Baggage
         """
@@ -534,16 +536,17 @@
         return header
 
     def serialize(self, include_third_party=False):
         # type: (bool) -> str
         items = []
 
         for key, val in iteritems(self.sentry_items):
-            item = Baggage.SENTRY_PREFIX + quote(key) + "=" + quote(val)
-            items.append(item)
+            with capture_internal_exceptions():
+                item = Baggage.SENTRY_PREFIX + quote(key) + "=" + quote(str(val))
+                items.append(item)
 
         if include_third_party:
             items.append(self.third_party_items)
 
         return ",".join(items)
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/transport.py` & `sentry-sdk-1.9.9/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk/utils.py` & `sentry-sdk-1.9.9/sentry_sdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -857,15 +857,15 @@
         # backport (also a PyPI package) works with asyncio under Python 3.6
         #
         # Import it if available.
         if sys.version_info < (3, 7):
             # `aiocontextvars` is absolutely required for functional
             # contextvars on Python 3.6.
             try:
-                from aiocontextvars import ContextVar  # noqa
+                from aiocontextvars import ContextVar
 
                 return True, ContextVar
             except ImportError:
                 pass
         else:
             # On Python 3.7 contextvars are functional.
             try:
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk/worker.py` & `sentry-sdk-1.9.9/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/sentry_sdk.egg-info/PKG-INFO` & `sentry-sdk-1.9.9/sentry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 1.9.8
+Version: 1.9.9
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: BSD
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-sdk Version: 1.9.8 Summary: Python client
+Metadata-Version: 2.1 Name: sentry-sdk Version: 1.9.9 Summary: Python client
 for Sentry (https://sentry.io) Home-page: https://github.com/getsentry/sentry-
 python Author: Sentry Team and Contributors Author-email: hello@sentry.io
 License: BSD Project-URL: Documentation, https://docs.sentry.io/platforms/
 python/ Project-URL: Changelog, https://github.com/getsentry/sentry-python/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Web Environment Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk.egg-info/SOURCES.txt` & `sentry-sdk-1.9.9/sentry_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,13 +67,14 @@
 sentry_sdk/integrations/threading.py
 sentry_sdk/integrations/tornado.py
 sentry_sdk/integrations/trytond.py
 sentry_sdk/integrations/wsgi.py
 sentry_sdk/integrations/django/__init__.py
 sentry_sdk/integrations/django/asgi.py
 sentry_sdk/integrations/django/middleware.py
+sentry_sdk/integrations/django/signals_handlers.py
 sentry_sdk/integrations/django/templates.py
 sentry_sdk/integrations/django/transactions.py
 sentry_sdk/integrations/django/views.py
 sentry_sdk/integrations/spark/__init__.py
 sentry_sdk/integrations/spark/spark_driver.py
 sentry_sdk/integrations/spark/spark_worker.py
```

### Comparing `sentry-sdk-1.9.8/sentry_sdk.egg-info/requires.txt` & `sentry-sdk-1.9.9/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry-sdk-1.9.8/setup.py` & `sentry-sdk-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="1.9.8",
+    version="1.9.9",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

