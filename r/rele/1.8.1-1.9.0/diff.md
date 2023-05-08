# Comparing `tmp/rele-1.8.1.tar.gz` & `tmp/rele-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rele-1.8.1.tar", last modified: Mon May  8 09:17:57 2023, max compression
+gzip compressed data, was "rele-1.9.0.tar", last modified: Tue May  2 15:01:08 2023, max compression
```

## Comparing `rele-1.8.1.tar` & `rele-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,58 @@
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:57.011007 rele-1.8.1/
--rw-r--r--   0 jsansalo   (501) staff       (20)      566 2023-05-08 08:43:27.000000 rele-1.8.1/AUTHORS.md
--rw-r--r--   0 jsansalo   (501) staff       (20)    11352 2023-05-08 08:43:27.000000 rele-1.8.1/LICENSE
--rw-r--r--   0 jsansalo   (501) staff       (20)     3947 2023-05-08 09:17:57.011205 rele-1.8.1/PKG-INFO
--rw-r--r--   0 jsansalo   (501) staff       (20)     2830 2023-05-08 08:43:27.000000 rele-1.8.1/README.md
--rw-r--r--   0 jsansalo   (501) staff       (20)       76 2023-05-08 08:43:27.000000 rele-1.8.1/pyproject.toml
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:56.989513 rele-1.8.1/rele/
--rw-r--r--   0 jsansalo   (501) staff       (20)      390 2023-05-08 08:48:37.000000 rele-1.8.1/rele/__init__.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1453 2023-05-08 08:44:19.000000 rele-1.8.1/rele/__main__.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      199 2023-05-08 08:43:27.000000 rele-1.8.1/rele/apps.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     8719 2023-05-08 08:44:19.000000 rele-1.8.1/rele/client.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     4352 2023-05-08 08:44:19.000000 rele-1.8.1/rele/config.py
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:57.002518 rele-1.8.1/rele/contrib/
--rw-r--r--   0 jsansalo   (501) staff       (20)      355 2023-05-08 08:43:27.000000 rele-1.8.1/rele/contrib/__init__.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      400 2023-05-08 08:43:27.000000 rele-1.8.1/rele/contrib/django_db_middleware.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      347 2023-05-08 08:43:27.000000 rele-1.8.1/rele/contrib/flask_middleware.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     3860 2023-05-08 08:44:19.000000 rele-1.8.1/rele/contrib/logging_middleware.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      306 2023-05-08 08:43:27.000000 rele-1.8.1/rele/contrib/unrecoverable_middleware.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1224 2023-05-08 08:43:27.000000 rele-1.8.1/rele/contrib/verbose_logging_middleware.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1840 2023-05-08 08:43:27.000000 rele-1.8.1/rele/discover.py
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:57.004109 rele-1.8.1/rele/management/
--rw-r--r--   0 jsansalo   (501) staff       (20)        0 2023-05-08 08:43:27.000000 rele-1.8.1/rele/management/__init__.py
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:57.006258 rele-1.8.1/rele/management/commands/
--rw-r--r--   0 jsansalo   (501) staff       (20)        0 2023-05-08 08:43:27.000000 rele-1.8.1/rele/management/commands/__init__.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1089 2023-05-08 08:43:27.000000 rele-1.8.1/rele/management/commands/runrele.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      728 2023-05-08 08:43:27.000000 rele-1.8.1/rele/management/commands/showsubscriptions.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      537 2023-05-08 08:43:27.000000 rele-1.8.1/rele/management/discover.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     3486 2023-05-08 08:43:27.000000 rele-1.8.1/rele/middleware.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1581 2023-05-08 08:43:27.000000 rele-1.8.1/rele/publishing.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1118 2023-05-08 08:43:27.000000 rele-1.8.1/rele/retry_policy.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     7182 2023-05-08 08:43:27.000000 rele-1.8.1/rele/subscription.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     5727 2023-05-08 09:11:22.000000 rele-1.8.1/rele/worker.py
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:56.997387 rele-1.8.1/rele.egg-info/
--rw-r--r--   0 jsansalo   (501) staff       (20)     3947 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/PKG-INFO
--rw-r--r--   0 jsansalo   (501) staff       (20)      988 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/SOURCES.txt
--rw-r--r--   0 jsansalo   (501) staff       (20)        1 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/dependency_links.txt
--rw-r--r--   0 jsansalo   (501) staff       (20)       48 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/entry_points.txt
--rw-r--r--   0 jsansalo   (501) staff       (20)        1 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/not-zip-safe
--rw-r--r--   0 jsansalo   (501) staff       (20)       80 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/requires.txt
--rw-r--r--   0 jsansalo   (501) staff       (20)       11 2023-05-08 09:17:56.000000 rele-1.8.1/rele.egg-info/top_level.txt
--rw-r--r--   0 jsansalo   (501) staff       (20)      446 2023-05-08 09:17:57.011950 rele-1.8.1/setup.cfg
--rw-r--r--   0 jsansalo   (501) staff       (20)     2227 2023-05-08 08:43:27.000000 rele-1.8.1/setup.py
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:56.965561 rele-1.8.1/tests/
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:57.008788 rele-1.8.1/tests/commands/
--rw-r--r--   0 jsansalo   (501) staff       (20)        0 2023-05-08 08:43:27.000000 rele-1.8.1/tests/commands/__init__.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1326 2023-05-08 08:44:19.000000 rele-1.8.1/tests/commands/test_runrele.py
--rw-r--r--   0 jsansalo   (501) staff       (20)     1602 2023-05-08 08:43:27.000000 rele-1.8.1/tests/commands/test_showsubscriptions.py
-drwxr-xr-x   0 jsansalo   (501) staff       (20)        0 2023-05-08 09:17:57.010100 rele-1.8.1/tests/more_subs/
--rw-r--r--   0 jsansalo   (501) staff       (20)        0 2023-05-08 08:43:27.000000 rele-1.8.1/tests/more_subs/__init__.py
--rw-r--r--   0 jsansalo   (501) staff       (20)      131 2023-05-08 08:43:27.000000 rele-1.8.1/tests/more_subs/subs.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.499046 rele-1.9.0/
+-rw-r--r--   0 abarcel    (501) staff       (20)      566 2023-05-02 14:41:25.000000 rele-1.9.0/AUTHORS.md
+-rw-r--r--   0 abarcel    (501) staff       (20)    11352 2023-05-02 14:41:25.000000 rele-1.9.0/LICENSE
+-rw-r--r--   0 abarcel    (501) staff       (20)     3947 2023-05-02 15:01:08.499324 rele-1.9.0/PKG-INFO
+-rw-r--r--   0 abarcel    (501) staff       (20)     2830 2023-05-02 14:41:25.000000 rele-1.9.0/README.md
+-rw-r--r--   0 abarcel    (501) staff       (20)       76 2023-05-02 14:41:25.000000 rele-1.9.0/pyproject.toml
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.471138 rele-1.9.0/rele/
+-rw-r--r--   0 abarcel    (501) staff       (20)      390 2023-05-02 14:51:26.000000 rele-1.9.0/rele/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1453 2023-05-02 14:41:25.000000 rele-1.9.0/rele/__main__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      199 2023-05-02 14:41:25.000000 rele-1.9.0/rele/apps.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     8719 2023-05-02 14:41:25.000000 rele-1.9.0/rele/client.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     4352 2023-05-02 14:41:25.000000 rele-1.9.0/rele/config.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.481718 rele-1.9.0/rele/contrib/
+-rw-r--r--   0 abarcel    (501) staff       (20)      355 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      400 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/django_db_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      347 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/flask_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     3918 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/logging_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      306 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/unrecoverable_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1224 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/verbose_logging_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1840 2023-05-02 14:41:25.000000 rele-1.9.0/rele/discover.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.483250 rele-1.9.0/rele/management/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/__init__.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.486739 rele-1.9.0/rele/management/commands/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/commands/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1089 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/commands/runrele.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      728 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/commands/showsubscriptions.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      537 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/discover.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     3486 2023-05-02 14:41:25.000000 rele-1.9.0/rele/middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1581 2023-05-02 14:41:25.000000 rele-1.9.0/rele/publishing.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1118 2023-05-02 14:41:25.000000 rele-1.9.0/rele/retry_policy.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     7182 2023-05-02 14:41:25.000000 rele-1.9.0/rele/subscription.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     5562 2023-05-02 14:41:25.000000 rele-1.9.0/rele/worker.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.476846 rele-1.9.0/rele.egg-info/
+-rw-r--r--   0 abarcel    (501) staff       (20)     3947 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/PKG-INFO
+-rw-r--r--   0 abarcel    (501) staff       (20)     1178 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/SOURCES.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)        1 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/dependency_links.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)       48 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/entry_points.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)        1 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/not-zip-safe
+-rw-r--r--   0 abarcel    (501) staff       (20)       80 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/requires.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)       11 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/top_level.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)      446 2023-05-02 15:01:08.500802 rele-1.9.0/setup.cfg
+-rw-r--r--   0 abarcel    (501) staff       (20)     2227 2023-05-02 14:41:25.000000 rele-1.9.0/setup.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.494723 rele-1.9.0/tests/
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.496990 rele-1.9.0/tests/commands/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/tests/commands/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1326 2023-05-02 14:41:25.000000 rele-1.9.0/tests/commands/test_runrele.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1602 2023-05-02 14:41:25.000000 rele-1.9.0/tests/commands/test_showsubscriptions.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.498216 rele-1.9.0/tests/more_subs/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/tests/more_subs/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      131 2023-05-02 14:41:25.000000 rele-1.9.0/tests/more_subs/subs.py
+-rw-r--r--   0 abarcel    (501) staff       (20)    12466 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_client.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     5086 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_config.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      835 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_discover.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1010 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1905 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_publishing.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      464 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_retry_policy.py
+-rw-r--r--   0 abarcel    (501) staff       (20)    12493 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_subscription.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     5540 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_worker.py
```

### Comparing `rele-1.8.1/AUTHORS.md` & `rele-1.9.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/LICENSE` & `rele-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/PKG-INFO` & `rele-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rele
-Version: 1.8.1
+Version: 1.9.0
 Summary: Relé makes integration with Google PubSub easier.
 Home-page: https://github.com/mercadona/rele
 Author: Mercadona Tech
 Author-email: software.online@mercadona.es
 License: Apache Software License 2.0
 Keywords: rele
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rele-1.8.1/README.md` & `rele-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/__main__.py` & `rele-1.9.0/rele/__main__.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/client.py` & `rele-1.9.0/rele/client.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/config.py` & `rele-1.9.0/rele/config.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/contrib/logging_middleware.py` & `rele-1.9.0/rele/contrib/logging_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     def __init__(self):
         self._logger = None
 
     def setup(self, config, **kwargs):
         self._logger = logging.getLogger(__name__)
         self._app_name = config.app_name
+        self._encoder = config.encoder
 
     def _build_data_metrics(
         self, subscription, message, status, start_processing_time=None
     ):
         result = {
             "agent": self._app_name,
             "topic": subscription.topic,
@@ -67,15 +68,15 @@
             f"for {topic}: {str(exception.__class__.__name__)}",
             exc_info=True,
             extra={
                 "metrics": {
                     "name": "publications",
                     "data": {"agent": self._app_name, "topic": topic},
                 },
-                "subscription_message": json.dumps(message),
+                "subscription_message": json.dumps(message, cls=self._encoder),
             },
         )
 
     def pre_process_message(self, subscription, message):
         self._logger.debug(
             f"Start processing message for {subscription}",
             extra={
```

### Comparing `rele-1.8.1/rele/contrib/verbose_logging_middleware.py` & `rele-1.9.0/rele/contrib/verbose_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/discover.py` & `rele-1.9.0/rele/discover.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/management/commands/runrele.py` & `rele-1.9.0/rele/management/commands/runrele.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/management/commands/showsubscriptions.py` & `rele-1.9.0/rele/management/commands/showsubscriptions.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/management/discover.py` & `rele-1.9.0/rele/management/discover.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/middleware.py` & `rele-1.9.0/rele/middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/publishing.py` & `rele-1.9.0/rele/publishing.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/retry_policy.py` & `rele-1.9.0/rele/retry_policy.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/subscription.py` & `rele-1.9.0/rele/subscription.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/rele/worker.py` & `rele-1.9.0/rele/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,27 +84,19 @@
                in this process.
 
         Exits with code 0 for a clean exit.
 
         :param signal: Needed for `signal.signal <https://docs.python.org/3/library/signal.html#signal.signal>`_  # noqa
         :param frame: Needed for `signal.signal <https://docs.python.org/3/library/signal.html#signal.signal>`_  # noqa
         """
-
-        logger.info(f"Rele receive {signal} signal, stopping worker")
-
         run_middleware_hook("pre_worker_stop", self._subscriptions)
         for future in self._futures.values():
             future.cancel()
 
-        logger.info("Rele cancel all futures")
-
         run_middleware_hook("post_worker_stop")
-
-        logger.info("Rele worker stopped")
-
         sys.exit(0)
 
     def _boostrap_consumption(self, subscription):
         if subscription in self._futures:
             self._futures[subscription].cancel()
 
         executor_kwargs = {"thread_name_prefix": "ThreadPoolExecutor-ThreadScheduler"}
```

### Comparing `rele-1.8.1/rele.egg-info/PKG-INFO` & `rele-1.9.0/rele.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rele
-Version: 1.8.1
+Version: 1.9.0
 Summary: Relé makes integration with Google PubSub easier.
 Home-page: https://github.com/mercadona/rele
 Author: Mercadona Tech
 Author-email: software.online@mercadona.es
 License: Apache Software License 2.0
 Keywords: rele
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rele-1.8.1/rele.egg-info/SOURCES.txt` & `rele-1.9.0/rele.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -29,12 +29,20 @@
 rele/contrib/unrecoverable_middleware.py
 rele/contrib/verbose_logging_middleware.py
 rele/management/__init__.py
 rele/management/discover.py
 rele/management/commands/__init__.py
 rele/management/commands/runrele.py
 rele/management/commands/showsubscriptions.py
+tests/test_client.py
+tests/test_config.py
+tests/test_discover.py
+tests/test_middleware.py
+tests/test_publishing.py
+tests/test_retry_policy.py
+tests/test_subscription.py
+tests/test_worker.py
 tests/commands/__init__.py
 tests/commands/test_runrele.py
 tests/commands/test_showsubscriptions.py
 tests/more_subs/__init__.py
 tests/more_subs/subs.py
```

### Comparing `rele-1.8.1/setup.py` & `rele-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/tests/commands/test_runrele.py` & `rele-1.9.0/tests/commands/test_runrele.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.1/tests/commands/test_showsubscriptions.py` & `rele-1.9.0/tests/commands/test_showsubscriptions.py`

 * *Files identical despite different names*

