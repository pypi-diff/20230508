# Comparing `tmp/bdating-common-0.9.8.tar.gz` & `tmp/bdating-common-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdating-common-0.9.8.tar", last modified: Mon Dec  5 10:25:49 2022, max compression
+gzip compressed data, was "bdating-common-0.9.9.tar", last modified: Fri Dec  9 15:40:47 2022, max compression
```

## Comparing `bdating-common-0.9.8.tar` & `bdating-common-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2022-12-05 10:25:49.923884 bdating-common-0.9.8/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      842 2022-12-05 10:25:49.923884 bdating-common-0.9.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      230 2022-12-04 13:54:10.000000 bdating-common-0.9.8/README.md
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2022-12-05 10:25:49.923884 bdating-common-0.9.8/bdating_common/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       20 2022-12-05 10:25:47.000000 bdating-common-0.9.8/bdating_common/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    14517 2022-12-05 10:25:47.000000 bdating-common-0.9.8/bdating_common/api_common.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3338 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/auth0_token_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      771 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/aws_secrets_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2039 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/collect_default.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    12607 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/crypto_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1502 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/enum_translation.yml
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1918 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/errors.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4318 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/es_helper.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     3963 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/event_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3117 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/in_app_notif_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1425 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/json_logger.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5208 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/model.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/multi_threading.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1856 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/notify_helper.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4538 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/report_metrics.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4460 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/schedule_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      712 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/time_helper.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      382 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/utils.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      407 2022-12-04 13:54:10.000000 bdating-common-0.9.8/bdating_common/wallet_helper.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2022-12-05 10:25:49.923884 bdating-common-0.9.8/bdating_common.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      842 2022-12-05 10:25:49.000000 bdating-common-0.9.8/bdating_common.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      915 2022-12-05 10:25:49.000000 bdating-common-0.9.8/bdating_common.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2022-12-05 10:25:49.000000 bdating-common-0.9.8/bdating_common.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      125 2022-12-05 10:25:49.000000 bdating-common-0.9.8/bdating_common.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      181 2022-12-05 10:25:49.000000 bdating-common-0.9.8/bdating_common.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2022-12-05 10:25:49.000000 bdating-common-0.9.8/bdating_common.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2022-12-05 10:25:49.923884 bdating-common-0.9.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1376 2022-12-04 13:54:10.000000 bdating-common-0.9.8/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2022-12-09 15:40:47.746112 bdating-common-0.9.9/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      842 2022-12-09 15:40:47.746112 bdating-common-0.9.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      230 2022-12-04 13:54:10.000000 bdating-common-0.9.9/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2022-12-09 15:40:47.746112 bdating-common-0.9.9/bdating_common/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       20 2022-12-09 15:40:44.000000 bdating-common-0.9.9/bdating_common/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    14781 2022-12-09 15:40:44.000000 bdating-common-0.9.9/bdating_common/api_common.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3338 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/auth0_token_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      771 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/aws_secrets_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2039 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/collect_default.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    12607 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/crypto_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1502 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/enum_translation.yml
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1918 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/errors.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4318 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/es_helper.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     3963 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/event_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3117 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/in_app_notif_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1425 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/json_logger.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5208 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/model.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/multi_threading.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1856 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/notify_helper.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4538 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/report_metrics.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4460 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/schedule_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      712 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/time_helper.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      382 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/utils.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      407 2022-12-04 13:54:10.000000 bdating-common-0.9.9/bdating_common/wallet_helper.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2022-12-09 15:40:47.746112 bdating-common-0.9.9/bdating_common.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      842 2022-12-09 15:40:47.000000 bdating-common-0.9.9/bdating_common.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      915 2022-12-09 15:40:47.000000 bdating-common-0.9.9/bdating_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2022-12-09 15:40:47.000000 bdating-common-0.9.9/bdating_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      125 2022-12-09 15:40:47.000000 bdating-common-0.9.9/bdating_common.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      181 2022-12-09 15:40:47.000000 bdating-common-0.9.9/bdating_common.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2022-12-09 15:40:47.000000 bdating-common-0.9.9/bdating_common.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2022-12-09 15:40:47.746112 bdating-common-0.9.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1376 2022-12-04 13:54:10.000000 bdating-common-0.9.9/setup.py
```

### Comparing `bdating-common-0.9.8/PKG-INFO` & `bdating-common-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdating-common
-Version: 0.9.8
+Version: 0.9.9
 Summary: Bdating common libraries standard library
 Home-page: https://github.com/bdating-io/bdating-python-common
 Author: Zac
 Author-email: zac@bdating.io
 License: UNKNOWN
 Description: # README #
```

### Comparing `bdating-common-0.9.8/bdating_common/api_common.py` & `bdating-common-0.9.9/bdating_common/api_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -354,21 +354,26 @@
         body={...}
         ), wallet=user_id)
 
     or if simply just push a text message
     publish_message("Please display this to the user", wallet=user_id)
 
     """
+    log.info("--- api_common.py:publish_message()")
     if not sync_redis:
         sync_redis = redis.Redis(
             host=settings.redis_host,
             port=settings.redis_port,
             db=settings.in_app_notif_cache_id,
             password=settings.redis_password,
         )
     if isinstance(message, Dict):
         sync_redis.publish(wallet, json.dumps(message, default=str))
+        log.info(f"--- api_common.py:publish_message(): wallet={wallet}, message={json.dumps(message, default=str)}")
     else:
         sync_redis.publish(wallet, json.dumps({
             "type": "message",
             "body": {"message": message}
         }))
+
+        # log.info("--- api_common.py:publish_message(): published message: " , message)
+
```

### Comparing `bdating-common-0.9.8/bdating_common/auth0_token_helper.py` & `bdating-common-0.9.9/bdating_common/auth0_token_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/aws_secrets_helper.py` & `bdating-common-0.9.9/bdating_common/aws_secrets_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/collect_default.py` & `bdating-common-0.9.9/bdating_common/collect_default.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/crypto_helper.py` & `bdating-common-0.9.9/bdating_common/crypto_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/enum_translation.yml` & `bdating-common-0.9.9/bdating_common/enum_translation.yml`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/errors.py` & `bdating-common-0.9.9/bdating_common/errors.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/es_helper.py` & `bdating-common-0.9.9/bdating_common/es_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/event_helper.py` & `bdating-common-0.9.9/bdating_common/event_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/in_app_notif_helper.py` & `bdating-common-0.9.9/bdating_common/in_app_notif_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/json_logger.py` & `bdating-common-0.9.9/bdating_common/json_logger.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/model.py` & `bdating-common-0.9.9/bdating_common/model.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/notify_helper.py` & `bdating-common-0.9.9/bdating_common/notify_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/report_metrics.py` & `bdating-common-0.9.9/bdating_common/report_metrics.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/schedule_helper.py` & `bdating-common-0.9.9/bdating_common/schedule_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common/time_helper.py` & `bdating-common-0.9.9/bdating_common/time_helper.py`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/bdating_common.egg-info/PKG-INFO` & `bdating-common-0.9.9/bdating_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdating-common
-Version: 0.9.8
+Version: 0.9.9
 Summary: Bdating common libraries standard library
 Home-page: https://github.com/bdating-io/bdating-python-common
 Author: Zac
 Author-email: zac@bdating.io
 License: UNKNOWN
 Description: # README #
```

### Comparing `bdating-common-0.9.8/bdating_common.egg-info/SOURCES.txt` & `bdating-common-0.9.9/bdating_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdating-common-0.9.8/setup.py` & `bdating-common-0.9.9/setup.py`

 * *Files identical despite different names*

