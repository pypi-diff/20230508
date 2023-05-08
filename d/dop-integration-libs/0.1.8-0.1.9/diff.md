# Comparing `tmp/dop_integration_libs-0.1.8.tar.gz` & `tmp/dop_integration_libs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dop_integration_libs-0.1.8.tar", max compression
+gzip compressed data, was "dop_integration_libs-0.1.9.tar", max compression
```

## Comparing `dop_integration_libs-0.1.8.tar` & `dop_integration_libs-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.8/dop_integration_libs/__init__.py
--rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.8/dop_integration_libs/__main__.py
--rw-r--r--   0        0        0     1724 2023-04-20 12:24:22.512014 dop_integration_libs-0.1.8/dop_integration_libs/environment.py
--rw-r--r--   0        0        0     2349 2023-04-20 12:30:55.216072 dop_integration_libs-0.1.8/dop_integration_libs/logger.py
--rw-r--r--   0        0        0      389 2023-04-20 12:31:02.826341 dop_integration_libs-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.9/dop_integration_libs/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.9/dop_integration_libs/__main__.py
+-rw-r--r--   0        0        0     1724 2023-04-20 12:24:22.512014 dop_integration_libs-0.1.9/dop_integration_libs/environment.py
+-rw-r--r--   0        0        0     2365 2023-04-20 12:34:27.373125 dop_integration_libs-0.1.9/dop_integration_libs/logger.py
+-rw-r--r--   0        0        0      389 2023-04-20 12:34:31.576866 dop_integration_libs-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.9/PKG-INFO
```

### Comparing `dop_integration_libs-0.1.8/dop_integration_libs/environment.py` & `dop_integration_libs-0.1.9/dop_integration_libs/environment.py`

 * *Files identical despite different names*

### Comparing `dop_integration_libs-0.1.8/dop_integration_libs/logger.py` & `dop_integration_libs-0.1.9/dop_integration_libs/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         print(message)
         self.logger.debug(message)
 
     def send_log_to_server(self, log: str):
         """
         This function is used to get the environment variables
         """
-        url = f"{self.env.LOG_API_BASE_URL}/logger/env/"
+        url = f"{self.env.LOG_API_BASE_URL}/logger/log/task/session/log"
         headers = {
             "Authorization": f"Bearer {self.env.LOG_API_TOKEN}"
         }
         body = {
             "task_session_id": self.session_id,
             "log_type": "CONSOLE",
             "log_data": log
```

