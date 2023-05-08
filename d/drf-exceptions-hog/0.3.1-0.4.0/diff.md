# Comparing `tmp/drf-exceptions-hog-0.3.1.tar.gz` & `tmp/drf-exceptions-hog-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-exceptions-hog-0.3.1.tar", last modified: Mon May  1 14:40:12 2023, max compression
+gzip compressed data, was "drf-exceptions-hog-0.4.0.tar", last modified: Mon May  8 14:57:19 2023, max compression
```

## Comparing `drf-exceptions-hog-0.3.1.tar` & `drf-exceptions-hog-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8467 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8467 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/exceptions_hog/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10784 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     7636 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    18090 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/tests/test_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:57:19.134870 drf-exceptions-hog-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     8467 2023-05-08 14:57:19.134870 drf-exceptions-hog-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:57:19.134870 drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8467 2023-05-08 14:57:19.000000 drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-08 14:57:19.000000 drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 14:57:19.000000 drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-08 14:57:19.000000 drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-08 14:57:19.000000 drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:57:19.134870 drf-exceptions-hog-0.4.0/exceptions_hog/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/exceptions_hog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/exceptions_hog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/exceptions_hog/handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/exceptions_hog/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/exceptions_hog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/exceptions_hog/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-08 14:57:19.134870 drf-exceptions-hog-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:57:19.134870 drf-exceptions-hog-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     7636 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19292 2023-05-08 14:57:08.000000 drf-exceptions-hog-0.4.0/tests/test_handler.py
```

### Comparing `drf-exceptions-hog-0.3.1/LICENSE` & `drf-exceptions-hog-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.1/PKG-INFO` & `drf-exceptions-hog-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-exceptions-hog
-Version: 0.3.1
+Version: 0.4.0
 Summary: Standardized and easy-to-parse API error responses for DRF.
 Home-page: https://github.com/posthog/drf-exceptions-hog
 Author: PostHog
 Author-email: hey@posthog.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf-exceptions-hog-0.3.1/README.md` & `drf-exceptions-hog-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/PKG-INFO` & `drf-exceptions-hog-0.4.0/drf_exceptions_hog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-exceptions-hog
-Version: 0.3.1
+Version: 0.4.0
 Summary: Standardized and easy-to-parse API error responses for DRF.
 Home-page: https://github.com/posthog/drf-exceptions-hog
 Author: PostHog
 Author-email: hey@posthog.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf-exceptions-hog-0.3.1/exceptions_hog/exceptions.py` & `drf-exceptions-hog-0.4.0/exceptions_hog/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.1/exceptions_hog/handler.py` & `drf-exceptions-hog-0.4.0/exceptions_hog/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,13 +300,18 @@
         response = dict(
             type=_get_error_type(exc),
             code=exception_list[0][0],
             detail=_get_detail(exc, exception_list[0][1]),
             attr=_get_attr(exception_list[0][1]),
         )
 
+    headers = {}
     if hasattr(exc, "extra"):  # type: ignore
         response["extra"] = exc.extra  # type: ignore
+    # see https://github.com/encode/django-rest-framework/blob/e08e606c82afd0d5ec82b2c58badec11a4ce825e/rest_framework/views.py#L86-L91 # noqa
+    # for the framework code this is based on
+    if isinstance(exc, exceptions.APIException) and getattr(exc, "wait", None):
+        headers["Retry-After"] = "%d" % exc.wait
     if event_id:
         response["error_event_id"] = event_id
 
-    return Response(response, status=_get_http_status(exc))
+    return Response(response, status=_get_http_status(exc), headers=headers)
```

### Comparing `drf-exceptions-hog-0.3.1/exceptions_hog/settings.py` & `drf-exceptions-hog-0.4.0/exceptions_hog/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Dict
+from typing import Any, Dict, Optional
 
 from django.conf import settings
 from rest_framework.settings import APISettings
 
-USER_SETTINGS: Dict = getattr(settings, "EXCEPTIONS_HOG", None)
+USER_SETTINGS: Optional[Any] = getattr(settings, "EXCEPTIONS_HOG", None)
 
 DEFAULTS: Dict = {
     "EXCEPTION_REPORTING": "exceptions_hog.handler.exception_reporter",
     "ENABLE_IN_DEBUG": False,
     "NESTED_KEY_SEPARATOR": "__",
     "SUPPORT_MULTIPLE_EXCEPTIONS": False,
 }
```

### Comparing `drf-exceptions-hog-0.3.1/setup.py` & `drf-exceptions-hog-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.1/tests/test_api.py` & `drf-exceptions-hog-0.4.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.1/tests/test_handler.py` & `drf-exceptions-hog-0.4.0/tests/test_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -249,14 +249,46 @@
         "attr": "my__special___attribute__children_attr",
     }
 
 
 # Django & DRF exceptions
 
 
+def test_throttled_exception_with_no_wait() -> None:
+    throttled = exceptions.Throttled(wait=None)
+    response = exception_handler(throttled)
+    assert response is not None
+    assert response.status_code == status.HTTP_429_TOO_MANY_REQUESTS
+    assert response.data == {
+        "attr": None,
+        "code": "throttled",
+        "detail": "Request was throttled.",
+        "type": "throttled_error",
+    }
+    # older versions in the CI test matrix don't have headers on Response
+    if getattr(response, "headers", None):
+        assert "Retry-After" not in response.headers
+
+
+def test_throttled_exception_with_wait() -> None:
+    throttled = exceptions.Throttled(wait=100)
+    response = exception_handler(throttled)
+    assert response is not None
+    assert response.status_code == status.HTTP_429_TOO_MANY_REQUESTS
+    assert response.data == {
+        "attr": None,
+        "code": "throttled",
+        "detail": "Request was throttled. Expected available in 100 seconds.",
+        "type": "throttled_error",
+    }
+    # older versions in the CI test matrix don't have headers on Response
+    if getattr(response, "headers", None):
+        assert response.headers["Retry-After"] == "100"
+
+
 def test_not_found_exception(res_not_found) -> None:
     response = exception_handler(exceptions.NotFound())
     assert response is not None
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert response.data == res_not_found
 
     # Test Django base exception too
```

