# Comparing `tmp/hf-webdriver-manager-0.2.0.tar.gz` & `tmp/hf-webdriver-manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/hf_webdriver_manager/hf_webdriver_manager/dist/.tmp-pouv72s3/hf-webdriver-manager-0.2.0.tar", last modified: Mon May  8 12:33:34 2023, max compression
+gzip compressed data, was "/home/runner/work/hf_webdriver_manager/hf_webdriver_manager/dist/.tmp-51760kwi/hf-webdriver-manager-0.2.1.tar", last modified: Mon May  8 14:18:05 2023, max compression
```

## Comparing `hf-webdriver-manager-0.2.0.tar` & `hf-webdriver-manager-0.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_brave_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_chromium_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_custom_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_custom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_edge_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_firefox_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_ie_driver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2630 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_opera_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_silent_global_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/config/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/driver_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/ie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/opera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/microsoft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/opera.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_brave_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_chromium_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_custom_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_edge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_firefox_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_ie_driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2630 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_opera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_silent_global_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/webdriver_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/webdriver_manager/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/driver_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:18:05.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/ie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/drivers/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/microsoft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-08 14:17:30.000000 hf-webdriver-manager-0.2.1/webdriver_manager/opera.py
```

### Comparing `hf-webdriver-manager-0.2.0/LICENSE` & `hf-webdriver-manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/PKG-INFO` & `hf-webdriver-manager-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-webdriver-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library provides the way to automatically manage drivers for different browsers.
 Home-page: https://github.com/HansBug/hf_webdriver_manager
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `hf-webdriver-manager-0.2.0/README.md` & `hf-webdriver-manager-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/PKG-INFO` & `hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-webdriver-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library provides the way to automatically manage drivers for different browsers.
 Home-page: https://github.com/HansBug/hf_webdriver_manager
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/SOURCES.txt` & `hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/requires.txt` & `hf-webdriver-manager-0.2.1/hf_webdriver_manager.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 certifi>=2022
 packaging>=21
 python-dotenv>=0.20.0
 requests>=2.20
 tqdm>=4.20
+hbutils>=0.9.0
 
 [:python_full_version >= "3.6.8"]
 pyparsing>=3.0.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
 urllib3~=1.13
```

### Comparing `hf-webdriver-manager-0.2.0/setup.py` & `hf-webdriver-manager-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_brave_driver.py` & `hf-webdriver-manager-0.2.1/tests/test_brave_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_chrome_driver.py` & `hf-webdriver-manager-0.2.1/tests/test_chrome_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_chromium_driver.py` & `hf-webdriver-manager-0.2.1/tests/test_chromium_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_custom_http_client.py` & `hf-webdriver-manager-0.2.1/tests/test_custom_http_client.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_custom_logger.py` & `hf-webdriver-manager-0.2.1/tests/test_custom_logger.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_downloader.py` & `hf-webdriver-manager-0.2.1/tests/test_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from webdriver_manager.drivers.chrome import ChromeDriver
 
 download_manager = WDMDownloadManager()
 
 
 def test_can_download_driver_as_zip_file(delete_drivers_dir):
     file = download_manager.download_file("http://chromedriver.storage.googleapis.com/2.26/chromedriver_win32.zip")
-    assert file.filename == "driver.zip"
+    assert file.filename == "chromedriver_win32.zip"
     archive = save_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert archive.file_path == f"{DEFAULT_PROJECT_ROOT_CACHE_PATH}{os.sep}{file.filename}"
     assert archive.unpack(DEFAULT_PROJECT_ROOT_CACHE_PATH) == ["chromedriver.exe"]
 
 
 def test_can_download_driver_as_tar_gz(delete_drivers_dir):
     file = download_manager.download_file(
@@ -32,10 +32,10 @@
 def test_can_download_chrome_driver(delete_drivers_dir, version):
     driver = ChromeDriver(name="chromedriver", version=version, os_type="win32",
                           url="http://chromedriver.storage.googleapis.com",
                           latest_release_url="http://chromedriver.storage.googleapis.com/LATEST_RELEASE",
                           chrome_type=ChromeType.GOOGLE, http_client=WDMHttpClient())
 
     file = download_manager.download_file(driver.get_driver_download_url())
-    assert file.filename == "driver.zip"
+    assert file.filename == "chromedriver_win32.zip"
     archive = save_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert "chromedriver.exe" in archive.unpack(DEFAULT_PROJECT_ROOT_CACHE_PATH)
```

### Comparing `hf-webdriver-manager-0.2.0/tests/test_edge_driver.py` & `hf-webdriver-manager-0.2.1/tests/test_edge_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_firefox_manager.py` & `hf-webdriver-manager-0.2.1/tests/test_firefox_manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_ie_driver.py` & `hf-webdriver-manager-0.2.1/tests/test_ie_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_opera_manager.py` & `hf-webdriver-manager-0.2.1/tests/test_opera_manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/tests/test_utils.py` & `hf-webdriver-manager-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/chrome.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/chrome.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/config/meta.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for hf-webdriver-manager package.
 """
 
 #: Title of this project (should be `hf-webdriver-manager`).
 __TITLE__ = "hf-webdriver-manager"
 
 #: Version of this project.
-__VERSION__ = "0.2.0"
+__VERSION__ = "0.2.1"
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'Library provides the way to automatically manage drivers for different browsers.'
 
 #: Author of this project.
 __AUTHOR__ = "HansBug"
```

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/archive.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/archive.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/config.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/config.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/download_manager.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/download_manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/driver.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/driver_cache.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/driver_cache.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/http.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/http.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/logger.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/logger.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/manager.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/core/utils.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import os
 import platform
 import re
 import subprocess
 import sys
 
+from hbutils.system import urlsplit
 from tqdm import tqdm
 
 from webdriver_manager.core.archive import Archive
 
 
 class File(object):
     def __init__(self, stream):
@@ -19,21 +20,16 @@
     @property
     def filename(self) -> str:
         try:
             filename = re.findall(
                 r'filename=\s*[\"\']?(?P<filename>[^\s\"\';]+)[\"\'\s]?',
                 self.__stream.headers["content-disposition"],
             )[0]
-        except KeyError:
-            filename = f"{self.__temp_name}.zip"
-        except IndexError:
-            filename = f"{self.__temp_name}.exe"
-
-        if '"' in filename:
-            filename = filename.replace('"', "")
+        except (KeyError, IndexError):
+            filename = urlsplit(self.__stream.request.url).filename
 
         return filename
 
 
 def save_file(file: File, directory: str):
     os.makedirs(directory, exist_ok=True)
```

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/dispatch.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/dispatch.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/chrome.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/drivers/chrome.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/edge.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/drivers/edge.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/firefox.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/drivers/firefox.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/ie.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/drivers/ie.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/opera.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/drivers/opera.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/firefox.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/firefox.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/microsoft.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/microsoft.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.2.0/webdriver_manager/opera.py` & `hf-webdriver-manager-0.2.1/webdriver_manager/opera.py`

 * *Files identical despite different names*

