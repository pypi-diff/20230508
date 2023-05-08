# Comparing `tmp/hf-webdriver-manager-0.1.0.tar.gz` & `tmp/hf-webdriver-manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/hf_webdriver_manager/hf_webdriver_manager/dist/.tmp-f1x3rprw/hf-webdriver-manager-0.1.0.tar", last modified: Sat Apr  1 05:00:03 2023, max compression
+gzip compressed data, was "/home/runner/work/hf_webdriver_manager/hf_webdriver_manager/dist/.tmp-pouv72s3/hf-webdriver-manager-0.2.0.tar", last modified: Mon May  8 12:33:34 2023, max compression
```

## Comparing `hf-webdriver-manager-0.1.0.tar` & `hf-webdriver-manager-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_brave_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_chromium_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_custom_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_custom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_edge_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_firefox_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_ie_driver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2630 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_opera_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_silent_global_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/webdriver_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/webdriver_manager/config/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/driver_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:00:03.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/ie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/drivers/opera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/microsoft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-04-01 04:59:35.000000 hf-webdriver-manager-0.1.0/webdriver_manager/opera.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_brave_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_chromium_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_custom_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_edge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_firefox_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_ie_driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2630 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_opera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_silent_global_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/driver_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/ie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/drivers/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/microsoft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-08 12:32:53.000000 hf-webdriver-manager-0.2.0/webdriver_manager/opera.py
```

### Comparing `hf-webdriver-manager-0.1.0/LICENSE` & `hf-webdriver-manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/PKG-INFO` & `hf-webdriver-manager-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-webdriver-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library provides the way to automatically manage drivers for different browsers.
 Home-page: https://github.com/HansBug/hf_webdriver_manager
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
@@ -44,23 +44,19 @@
 ## Support the library on [Patreon](https://www.patreon.com/automation_remarks)
 
 The main idea is to simplify management of binary drivers for different browsers.
 
 For now support:
 
 - [ChromeDriver](#use-with-chrome)
-
+- [EdgeChromiumDriver](#use-with-edge)
 - [GeckoDriver](#use-with-firefox)
-
 - [IEDriver](#use-with-ie)
-
 - [OperaDriver](#use-with-opera)
 
-- [EdgeChromiumDriver](#use-with-edge)
-
 Compatible with Selenium 4.x and below.
 
 Before:
 You need to download the chromedriver binary, unzip it somewhere on your PC and set the path to this driver like this:
 
 ```python
 from selenium import webdriver
@@ -136,14 +132,33 @@
 from selenium.webdriver.chrome.service import Service as BraveService
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 driver = webdriver.Chrome(service=BraveService(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
 ```
 
+#### Use with Edge
+
+```python
+# selenium 3
+from selenium import webdriver
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+```
+
+```python
+# selenium 4
+from selenium import webdriver
+from selenium.webdriver.edge.service import Service as EdgeService
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+```
+
 #### Use with Firefox
 
 ```python
 # selenium 3
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 
@@ -174,54 +189,50 @@
 from selenium import webdriver
 from selenium.webdriver.ie.service import Service as IEService
 from webdriver_manager.microsoft import IEDriverManager
 
 driver = webdriver.Ie(service=IEService(IEDriverManager().install()))
 ```
 
-#### Use with Edge
+#### Use with Opera
 
 ```python
 # selenium 3
 from selenium import webdriver
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
+
+driver = webdriver.Remote(webdriver_service.service_url, webdriver.DesiredCapabilities.OPERA)
 ```
 
 ```python
 # selenium 4
 from selenium import webdriver
-from selenium.webdriver.edge.service import Service as EdgeService
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
-
-driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
-```
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-#### Use with Opera
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
 
-```python
-# selenium 3 & 4
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
+options = webdriver.ChromeOptions()
+options.add_experimental_option('w3c', True)
 
-driver = webdriver.Opera(executable_path=OperaDriverManager().install())
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 If the Opera browser is installed in a location other than `C:/Program Files` or `C:/Program Files (x86)` on windows
 and `/usr/bin/opera` for all unix variants and mac, then use the below code,
 
 ```python
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
-
 options = webdriver.ChromeOptions()
-options.add_argument('allow-elevated-browser')
-options.binary_location = "C:\\Users\\USERNAME\\FOLDERLOCATION\\Opera\\VERSION\\opera.exe"
-driver = webdriver.Opera(executable_path=OperaDriverManager().install(), options=options)
+options.binary_location = "path/to/opera.exe"
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 #### Get browser version from path
 
 To get the version of the browser from the executable of the browser itself:
 
 ```python
@@ -232,38 +243,18 @@
 ```
 
 ## Configuration
 
 **webdriver_manager** has several configuration variables you can be interested in.
 Any variable can be set using either .env file or via python directly
 
-### `INDEX_SITE_ROOT`
-
-This is the index site of this mirror, default value
-is `https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master`. If you need to change this, just
-set `INDEX_SITE_ROOT`'s environment variable.
-
-### `NO_INDEX_SITE`
-
-If this env is set, value of `INDEX_SITE_ROOT` will be treated as the huggingface mirror instead of url index site.
-
-For example, we use the [index site on gitee](https://gitee.com/hansbug/browser_drivers_mirror_index) to reduce the
-direct accesses to https://huggingface.co :
+### `DRIVER_SITE`
 
-```bash
-export INDEX_SITE_ROOT=https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master
-export NO_INDEX_SITE=
-```
-
-When you do not need the index site, just directly access the huggingface, you can set the env as the following code
-
-```bash
-export INDEX_SITE_ROOT=https://huggingface.co/HansBug/browser_drivers_mirror/resolve/main
-export NO_INDEX_SITE=1
-```
+You can change the resource address of the Selenium browser driver by setting the `DRIVER_SITE` environment variable.
+The default value is `https://huggingface.co/datasets/HansBug/browser_drivers_mirror/resolve/main`.
 
 ### `WDM_LOG`
 
 Turn off hf-webdriver-manager logs use:
 
 ```python
 import logging
```

### Comparing `hf-webdriver-manager-0.1.0/README.md` & `hf-webdriver-manager-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,19 @@
 ## Support the library on [Patreon](https://www.patreon.com/automation_remarks)
 
 The main idea is to simplify management of binary drivers for different browsers.
 
 For now support:
 
 - [ChromeDriver](#use-with-chrome)
-
+- [EdgeChromiumDriver](#use-with-edge)
 - [GeckoDriver](#use-with-firefox)
-
 - [IEDriver](#use-with-ie)
-
 - [OperaDriver](#use-with-opera)
 
-- [EdgeChromiumDriver](#use-with-edge)
-
 Compatible with Selenium 4.x and below.
 
 Before:
 You need to download the chromedriver binary, unzip it somewhere on your PC and set the path to this driver like this:
 
 ```python
 from selenium import webdriver
@@ -106,14 +102,33 @@
 from selenium.webdriver.chrome.service import Service as BraveService
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 driver = webdriver.Chrome(service=BraveService(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
 ```
 
+#### Use with Edge
+
+```python
+# selenium 3
+from selenium import webdriver
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+```
+
+```python
+# selenium 4
+from selenium import webdriver
+from selenium.webdriver.edge.service import Service as EdgeService
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+```
+
 #### Use with Firefox
 
 ```python
 # selenium 3
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 
@@ -144,54 +159,50 @@
 from selenium import webdriver
 from selenium.webdriver.ie.service import Service as IEService
 from webdriver_manager.microsoft import IEDriverManager
 
 driver = webdriver.Ie(service=IEService(IEDriverManager().install()))
 ```
 
-#### Use with Edge
+#### Use with Opera
 
 ```python
 # selenium 3
 from selenium import webdriver
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
+
+driver = webdriver.Remote(webdriver_service.service_url, webdriver.DesiredCapabilities.OPERA)
 ```
 
 ```python
 # selenium 4
 from selenium import webdriver
-from selenium.webdriver.edge.service import Service as EdgeService
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
-
-driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
-```
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-#### Use with Opera
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
 
-```python
-# selenium 3 & 4
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
+options = webdriver.ChromeOptions()
+options.add_experimental_option('w3c', True)
 
-driver = webdriver.Opera(executable_path=OperaDriverManager().install())
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 If the Opera browser is installed in a location other than `C:/Program Files` or `C:/Program Files (x86)` on windows
 and `/usr/bin/opera` for all unix variants and mac, then use the below code,
 
 ```python
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
-
 options = webdriver.ChromeOptions()
-options.add_argument('allow-elevated-browser')
-options.binary_location = "C:\\Users\\USERNAME\\FOLDERLOCATION\\Opera\\VERSION\\opera.exe"
-driver = webdriver.Opera(executable_path=OperaDriverManager().install(), options=options)
+options.binary_location = "path/to/opera.exe"
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 #### Get browser version from path
 
 To get the version of the browser from the executable of the browser itself:
 
 ```python
@@ -202,38 +213,18 @@
 ```
 
 ## Configuration
 
 **webdriver_manager** has several configuration variables you can be interested in.
 Any variable can be set using either .env file or via python directly
 
-### `INDEX_SITE_ROOT`
-
-This is the index site of this mirror, default value
-is `https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master`. If you need to change this, just
-set `INDEX_SITE_ROOT`'s environment variable.
-
-### `NO_INDEX_SITE`
-
-If this env is set, value of `INDEX_SITE_ROOT` will be treated as the huggingface mirror instead of url index site.
-
-For example, we use the [index site on gitee](https://gitee.com/hansbug/browser_drivers_mirror_index) to reduce the
-direct accesses to https://huggingface.co :
+### `DRIVER_SITE`
 
-```bash
-export INDEX_SITE_ROOT=https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master
-export NO_INDEX_SITE=
-```
-
-When you do not need the index site, just directly access the huggingface, you can set the env as the following code
-
-```bash
-export INDEX_SITE_ROOT=https://huggingface.co/HansBug/browser_drivers_mirror/resolve/main
-export NO_INDEX_SITE=1
-```
+You can change the resource address of the Selenium browser driver by setting the `DRIVER_SITE` environment variable.
+The default value is `https://huggingface.co/datasets/HansBug/browser_drivers_mirror/resolve/main`.
 
 ### `WDM_LOG`
 
 Turn off hf-webdriver-manager logs use:
 
 ```python
 import logging
```

### Comparing `hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/PKG-INFO` & `hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-webdriver-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library provides the way to automatically manage drivers for different browsers.
 Home-page: https://github.com/HansBug/hf_webdriver_manager
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
@@ -44,23 +44,19 @@
 ## Support the library on [Patreon](https://www.patreon.com/automation_remarks)
 
 The main idea is to simplify management of binary drivers for different browsers.
 
 For now support:
 
 - [ChromeDriver](#use-with-chrome)
-
+- [EdgeChromiumDriver](#use-with-edge)
 - [GeckoDriver](#use-with-firefox)
-
 - [IEDriver](#use-with-ie)
-
 - [OperaDriver](#use-with-opera)
 
-- [EdgeChromiumDriver](#use-with-edge)
-
 Compatible with Selenium 4.x and below.
 
 Before:
 You need to download the chromedriver binary, unzip it somewhere on your PC and set the path to this driver like this:
 
 ```python
 from selenium import webdriver
@@ -136,14 +132,33 @@
 from selenium.webdriver.chrome.service import Service as BraveService
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 driver = webdriver.Chrome(service=BraveService(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
 ```
 
+#### Use with Edge
+
+```python
+# selenium 3
+from selenium import webdriver
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+```
+
+```python
+# selenium 4
+from selenium import webdriver
+from selenium.webdriver.edge.service import Service as EdgeService
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+```
+
 #### Use with Firefox
 
 ```python
 # selenium 3
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 
@@ -174,54 +189,50 @@
 from selenium import webdriver
 from selenium.webdriver.ie.service import Service as IEService
 from webdriver_manager.microsoft import IEDriverManager
 
 driver = webdriver.Ie(service=IEService(IEDriverManager().install()))
 ```
 
-#### Use with Edge
+#### Use with Opera
 
 ```python
 # selenium 3
 from selenium import webdriver
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
+
+driver = webdriver.Remote(webdriver_service.service_url, webdriver.DesiredCapabilities.OPERA)
 ```
 
 ```python
 # selenium 4
 from selenium import webdriver
-from selenium.webdriver.edge.service import Service as EdgeService
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
-
-driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
-```
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-#### Use with Opera
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
 
-```python
-# selenium 3 & 4
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
+options = webdriver.ChromeOptions()
+options.add_experimental_option('w3c', True)
 
-driver = webdriver.Opera(executable_path=OperaDriverManager().install())
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 If the Opera browser is installed in a location other than `C:/Program Files` or `C:/Program Files (x86)` on windows
 and `/usr/bin/opera` for all unix variants and mac, then use the below code,
 
 ```python
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
-
 options = webdriver.ChromeOptions()
-options.add_argument('allow-elevated-browser')
-options.binary_location = "C:\\Users\\USERNAME\\FOLDERLOCATION\\Opera\\VERSION\\opera.exe"
-driver = webdriver.Opera(executable_path=OperaDriverManager().install(), options=options)
+options.binary_location = "path/to/opera.exe"
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 #### Get browser version from path
 
 To get the version of the browser from the executable of the browser itself:
 
 ```python
@@ -232,38 +243,18 @@
 ```
 
 ## Configuration
 
 **webdriver_manager** has several configuration variables you can be interested in.
 Any variable can be set using either .env file or via python directly
 
-### `INDEX_SITE_ROOT`
-
-This is the index site of this mirror, default value
-is `https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master`. If you need to change this, just
-set `INDEX_SITE_ROOT`'s environment variable.
-
-### `NO_INDEX_SITE`
-
-If this env is set, value of `INDEX_SITE_ROOT` will be treated as the huggingface mirror instead of url index site.
-
-For example, we use the [index site on gitee](https://gitee.com/hansbug/browser_drivers_mirror_index) to reduce the
-direct accesses to https://huggingface.co :
+### `DRIVER_SITE`
 
-```bash
-export INDEX_SITE_ROOT=https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master
-export NO_INDEX_SITE=
-```
-
-When you do not need the index site, just directly access the huggingface, you can set the env as the following code
-
-```bash
-export INDEX_SITE_ROOT=https://huggingface.co/HansBug/browser_drivers_mirror/resolve/main
-export NO_INDEX_SITE=1
-```
+You can change the resource address of the Selenium browser driver by setting the `DRIVER_SITE` environment variable.
+The default value is `https://huggingface.co/datasets/HansBug/browser_drivers_mirror/resolve/main`.
 
 ### `WDM_LOG`
 
 Turn off hf-webdriver-manager logs use:
 
 ```python
 import logging
```

### Comparing `hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/SOURCES.txt` & `hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/hf_webdriver_manager.egg-info/requires.txt` & `hf-webdriver-manager-0.2.0/hf_webdriver_manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/setup.py` & `hf-webdriver-manager-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_brave_driver.py` & `hf-webdriver-manager-0.2.0/tests/test_brave_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_chrome_driver.py` & `hf-webdriver-manager-0.2.0/tests/test_chrome_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_chromium_driver.py` & `hf-webdriver-manager-0.2.0/tests/test_chromium_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_custom_http_client.py` & `hf-webdriver-manager-0.2.0/tests/test_custom_http_client.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_custom_logger.py` & `hf-webdriver-manager-0.2.0/tests/test_custom_logger.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_downloader.py` & `hf-webdriver-manager-0.2.0/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_edge_driver.py` & `hf-webdriver-manager-0.2.0/tests/test_edge_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_firefox_manager.py` & `hf-webdriver-manager-0.2.0/tests/test_firefox_manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_ie_driver.py` & `hf-webdriver-manager-0.2.0/tests/test_ie_driver.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_opera_manager.py` & `hf-webdriver-manager-0.2.0/tests/test_opera_manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/tests/test_utils.py` & `hf-webdriver-manager-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/chrome.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/chrome.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import os
 from typing import Optional
+from urllib.parse import urljoin
 
 from .core.download_manager import DownloadManager, WDMDownloadManager
-from .core.manager import DriverManager, INDEX_SITE_ROOT, NO_INDEX_SITE
+from .core.manager import DriverManager, get_driver_site
 from .core.utils import ChromeType
 from .drivers.chrome import ChromeDriver
 
 
 class ChromeDriverManager(DriverManager):
     def __init__(
             self,
             version: Optional[str] = None,
             os_type: Optional[str] = None,
             path: Optional[str] = None,
             name: str = "chromedriver",
-            url: str = f'{INDEX_SITE_ROOT}/google',
-            latest_release_url: str = f'{INDEX_SITE_ROOT}/google/LATEST_RELEASE',
+            url: str = f'google',
+            latest_release_url: str = f'google/LATEST_RELEASE',
             chrome_type: str = ChromeType.GOOGLE,
             cache_valid_range: int = 1,
             download_manager: Optional[DownloadManager] = None,
-            use_index=not NO_INDEX_SITE,
     ):
         download_manager = download_manager or WDMDownloadManager()
         driver = ChromeDriver(
             name=name,
             version=version,
             os_type=os_type,
-            url=url,
-            latest_release_url=latest_release_url,
+            url=urljoin(get_driver_site(), url),
+            latest_release_url=urljoin(get_driver_site(), latest_release_url),
             chrome_type=chrome_type,
             http_client=download_manager.http_client,
-            use_index=use_index,
         )
         DriverManager.__init__(
             self, driver, path,
             cache_valid_range=cache_valid_range,
             download_manager=download_manager
         )
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/config/meta.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for hf-webdriver-manager package.
 """
 
 #: Title of this project (should be `hf-webdriver-manager`).
 __TITLE__ = "hf-webdriver-manager"
 
 #: Version of this project.
-__VERSION__ = "0.1.0"
+__VERSION__ = "0.2.0"
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'Library provides the way to automatically manage drivers for different browsers.'
 
 #: Author of this project.
 __AUTHOR__ = "HansBug"
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/archive.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/archive.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/config.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/config.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/download_manager.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/download_manager.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/driver.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/driver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import requests
 
-from .logger import log
 from .utils import get_browser_version_from_os
 from .utils import os_type as _utils_os_type
 
 
 class Driver(object):
     def __init__(
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client,
-            use_index=False,
     ):
         self._name = name
         self._url = url
         self._version = version
         self._os_type = os_type
         if os_type is None:
             self._os_type = _utils_os_type()
         self._latest_release_url = latest_release_url
         self._http_client = http_client
         self._browser_version = None
         self._driver_to_download_version = None
-        self._use_index = bool(use_index)
 
     def get_name(self):
         return self._name
 
     def get_os_type(self):
         return self._os_type
 
@@ -74,25 +71,14 @@
         )
         driver_binary_name = (
             f"{driver_binary_name}.exe" if "win" in self.get_os_type() else driver_binary_name
         )
         return driver_binary_name
 
     def _url_postprocess(self, url):
-        if self._use_index:
-            index_url = f'{url}_index'
-            log(f'Fetching resource url from index {index_url!r} ...')
-            resp = requests.get(index_url)
-            if resp.ok:
-                return resp.text.strip()
-            elif resp.status_code == 404:
-                raise ValueError(f'There is no such driver by url of index - {url}.')
-            else:
-                resp.raise_for_status()
+        resp = requests.head(url)
+        if resp.ok:
+            return url
+        elif resp.status_code == 404:
+            raise ValueError(f'There is no such driver by url {url}.')
         else:
-            resp = requests.head(url)
-            if resp.ok:
-                return url
-            elif resp.status_code == 404:
-                raise ValueError(f'There is no such driver by url {url}.')
-            else:
-                resp.raise_for_status()
+            resp.raise_for_status()
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/driver_cache.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/driver_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,20 +74,20 @@
 
     def find_driver(self, driver: Driver):
         """Find driver by '{os_type}_{driver_name}_{driver_version}_{browser_version}'."""
         os_type = driver.get_os_type()
         driver_name = driver.get_name()
         browser_version = driver.get_browser_version_from_os()
         driver_version = self.get_cache_key_driver_version(driver)
-
+        browser_type = driver.get_browser_type()
         metadata = self.load_metadata_content()
 
         key = self.__get_metadata_key(driver)
         if key not in metadata:
-            log(f'There is no [{os_type}] {driver_name} "{driver_version}" for browser "{browser_version}" in cache')
+            log(f'There is no [{os_type}] {driver_name} "{driver_version}" for browser {browser_type} "{browser_version}" in cache')
             return None
 
         driver_info = metadata[key]
         path = driver_info["binary_path"]
         if not os.path.exists(path):
             return None
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/http.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/http.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/logger.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/logger.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/manager.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import os
 
 from .download_manager import WDMDownloadManager
 from .driver import Driver
 from .driver_cache import DriverCache
 from .logger import log
 
-INDEX_SITE_ROOT = os.environ.get(
-    'INDEX_SITE_ROOT',
-    'https://gitee.com/hansbug/browser_drivers_mirror_index/raw/master',
-)
-NO_INDEX_SITE = bool(os.environ.get('NO_INDEX_SITE', '').strip())
+
+def get_driver_site():
+    drive_site = os.environ.get(
+        'DRIVER_SITE',
+        'https://huggingface.co/datasets/HansBug/browser_drivers_mirror/resolve/main'
+    )
+    if not drive_site.endswith('/'):
+        drive_site = f'{drive_site}/'
+
+    return drive_site
 
 
 class DriverManager(object):
     def __init__(
             self,
             driver: Driver,
             root_dir=None,
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/core/utils.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/core/utils.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/dispatch.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/dispatch.py`

 * *Files identical despite different names*

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/drivers/chrome.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/chrome.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,18 +12,17 @@
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client,
             chrome_type=ChromeType.GOOGLE,
-            use_index=False,
     ):
         super(ChromeDriver, self).__init__(
-            name, version, os_type, url, latest_release_url, http_client, use_index
+            name, version, os_type, url, latest_release_url, http_client
         )
         self._browser_type = chrome_type
         self._os_type = self.get_os_type()
 
     def get_os_type(self):
         os_type = super().get_os_type()
         if "win" in os_type:
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/drivers/edge.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,17 @@
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client,
-            use_index=False,
     ):
         super(EdgeChromiumDriver, self).__init__(
-            name, version, os_type, url, latest_release_url, http_client, use_index,
+            name, version, os_type, url, latest_release_url, http_client
         )
         self._os_type = self.get_os_type()
 
     def get_stable_release_version(self):
         """Stable driver version when browser version was not determined."""
         stable_url = self._latest_release_url.replace("LATEST_RELEASE", "LATEST_STABLE")
         resp = self._http_client.get(url=stable_url)
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/drivers/firefox.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/ie.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,56 @@
+import requests
+
 from webdriver_manager.core.driver import Driver
 from webdriver_manager.core.logger import log
-from webdriver_manager.core.utils import is_arch, is_mac_os
 
 
-class GeckoDriver(Driver):
+class IEDriver(Driver):
     def __init__(
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client,
-            use_index=False,
     ):
-        super(GeckoDriver, self).__init__(
-            name, version, os_type, url, latest_release_url, http_client, use_index,
+        super(IEDriver, self).__init__(
+            name, version, os_type, url, latest_release_url, http_client
         )
-        self._os_type = self.get_os_type()
+        self.os_type = "x64" if self._os_type == "win64" else "Win32"
+        # todo: for 'browser_version' implement installed IE version detection
+        #       like chrome or firefox
 
     def get_latest_release_version(self) -> str:
-        determined_browser_version = self.get_browser_version_from_os()
-        log(f"Get LATEST {self._name} version for {determined_browser_version} firefox")
+        log(f"Get LATEST driver version for Internet Explorer")
         resp = self._http_client.get(url=self.latest_release_url)
-        return resp.text.strip()
+        return resp.text.strip().replace("selenium-", "")
 
-    def get_driver_download_url(self):
-        """Like https://github.com/mozilla/geckodriver/releases/download/v0.11.1/geckodriver-v0.11.1-linux64.tar.gz"""
-        driver_version_to_download = self.get_driver_version_to_download()
-        log(f"Getting latest firefox release info for {driver_version_to_download}")
-        _exts = ['tar.gz', 'zip', 'gz']
-        for ext in _exts:
-            name = f"{self.get_name()}-{driver_version_to_download}-{self._os_type}.{ext}"
-            url = f'{self._url}/{driver_version_to_download}/{name}'
-            try:
-                return self._url_postprocess(url)
-            except (ValueError, IOError):
-                continue
+    def _get_version_to_fulfill(self, version):
+        response = requests.get(f'{self._latest_release_url}_{version}')
+        if response.status_code != 404:
+            response.raise_for_status()
+            return response.text.strip().replace("selenium-", "")
         else:
-            # noinspection PyUnboundLocalVariable
-            raise ValueError(f'There is no such driver by url {url}.')
+            raise ValueError(f'Unknown version of ie webdriver - {version!r}.')
 
-    def get_os_type(self):
-        os_type = super().get_os_type()
-        if not is_mac_os(os_type):
-            return os_type
-
-        macos = 'macos'
-        if is_arch(os_type):
-            return f"{macos}-aarch64"
-        return macos
+    def get_driver_version_to_download(self):
+        if not self._driver_to_download_version:
+            self._driver_to_download_version = self._get_version_to_fulfill(self._version) \
+                if self._version not in (None, "latest") else self.get_latest_release_version()
+        return self._driver_to_download_version
+
+    def get_driver_download_url(self):
+        """Like https://github.com/seleniumhq/selenium/releases/download/3.141.59/IEDriverServer_Win32_3.141.59.zip"""
+        driver_version_to_download = self.get_driver_version_to_download()
+        log(f"Getting latest ie release info for {driver_version_to_download}")
+        filename = f"{self._name}_{self.os_type}_{driver_version_to_download}.zip"
+        url = f'{self._url}/selenium-{driver_version_to_download}/{filename}'
+        return self._url_postprocess(url)
 
     @property
     def latest_release_url(self):
         return self._latest_release_url
 
     def get_browser_type(self):
-        return "firefox"
+        return "msie"
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/drivers/ie.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/opera.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,36 @@
-import requests
-
 from webdriver_manager.core.driver import Driver
 from webdriver_manager.core.logger import log
 
 
-class IEDriver(Driver):
+class OperaDriver(Driver):
     def __init__(
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client,
-            use_index=False,
     ):
-        super(IEDriver, self).__init__(
-            name, version, os_type, url, latest_release_url, http_client, use_index,
+        super(OperaDriver, self).__init__(
+            name, version, os_type, url, latest_release_url, http_client,
         )
-        self.os_type = "x64" if self._os_type == "win64" else "Win32"
-        # todo: for 'browser_version' implement installed IE version detection
-        #       like chrome or firefox
 
     def get_latest_release_version(self) -> str:
-        log(f"Get LATEST driver version for Internet Explorer")
         resp = self._http_client.get(url=self.latest_release_url)
-        return resp.text.strip().replace("selenium-", "")
-
-    def _get_version_to_fulfill(self, version):
-        response = requests.get(f'{self._latest_release_url}_{version}')
-        if response.status_code != 404:
-            response.raise_for_status()
-            return response.text.strip().replace("selenium-", "")
-        else:
-            raise ValueError(f'Unknown version of ie webdriver - {version!r}.')
-
-    def get_driver_version_to_download(self):
-        if not self._driver_to_download_version:
-            self._driver_to_download_version = self._get_version_to_fulfill(self._version) \
-                if self._version not in (None, "latest") else self.get_latest_release_version()
-        return self._driver_to_download_version
+        return resp.text.strip()
 
-    def get_driver_download_url(self):
-        """Like https://github.com/seleniumhq/selenium/releases/download/3.141.59/IEDriverServer_Win32_3.141.59.zip"""
+    def get_driver_download_url(self) -> str:
+        """Like https://github.com/operasoftware/operachromiumdriver/releases/download/v.2.45/operadriver_linux64.zip"""
         driver_version_to_download = self.get_driver_version_to_download()
-        log(f"Getting latest ie release info for {driver_version_to_download}")
-        filename = f"{self._name}_{self.os_type}_{driver_version_to_download}.zip"
-        url = f'{self._url}/selenium-{driver_version_to_download}/{filename}'
+        log(f"Getting latest opera release info for {driver_version_to_download}")
+        name = "{0}_{1}.zip".format(self.get_name(), self.get_os_type())
+        url = f'{self._url}/{driver_version_to_download}/{name}'
         return self._url_postprocess(url)
 
     @property
     def latest_release_url(self):
         return self._latest_release_url
 
     def get_browser_type(self):
-        return "msie"
+        return "opera"
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/drivers/opera.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/drivers/firefox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,58 @@
 from webdriver_manager.core.driver import Driver
 from webdriver_manager.core.logger import log
+from webdriver_manager.core.utils import is_arch, is_mac_os
 
 
-class OperaDriver(Driver):
+class GeckoDriver(Driver):
     def __init__(
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client,
-            use_index=False,
     ):
-        super(OperaDriver, self).__init__(
-            name, version, os_type, url, latest_release_url, http_client, use_index,
+        super(GeckoDriver, self).__init__(
+            name, version, os_type, url, latest_release_url, http_client
         )
+        self._os_type = self.get_os_type()
 
     def get_latest_release_version(self) -> str:
+        determined_browser_version = self.get_browser_version_from_os()
+        log(f"Get LATEST {self._name} version for {determined_browser_version} firefox")
         resp = self._http_client.get(url=self.latest_release_url)
         return resp.text.strip()
 
-    def get_driver_download_url(self) -> str:
-        """Like https://github.com/operasoftware/operachromiumdriver/releases/download/v.2.45/operadriver_linux64.zip"""
+    def get_driver_download_url(self):
+        """Like https://github.com/mozilla/geckodriver/releases/download/v0.11.1/geckodriver-v0.11.1-linux64.tar.gz"""
         driver_version_to_download = self.get_driver_version_to_download()
-        log(f"Getting latest opera release info for {driver_version_to_download}")
-        name = "{0}_{1}.zip".format(self.get_name(), self.get_os_type())
-        url = f'{self._url}/{driver_version_to_download}/{name}'
-        return self._url_postprocess(url)
+        log(f"Getting latest firefox release info for {driver_version_to_download}")
+        _exts = ['tar.gz', 'zip', 'gz']
+        for ext in _exts:
+            name = f"{self.get_name()}-{driver_version_to_download}-{self._os_type}.{ext}"
+            url = f'{self._url}/{driver_version_to_download}/{name}'
+            try:
+                return self._url_postprocess(url)
+            except (ValueError, IOError):
+                continue
+        else:
+            # noinspection PyUnboundLocalVariable
+            raise ValueError(f'There is no such driver by url {url}.')
+
+    def get_os_type(self):
+        os_type = super().get_os_type()
+        if not is_mac_os(os_type):
+            return os_type
+
+        macos = 'macos'
+        if is_arch(os_type):
+            return f"{macos}-aarch64"
+        return macos
 
     @property
     def latest_release_url(self):
         return self._latest_release_url
 
     def get_browser_type(self):
-        return "opera"
+        return "firefox"
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/firefox.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/firefox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import os
 from typing import Optional
+from urllib.parse import urljoin
 
 from .core.download_manager import DownloadManager, WDMDownloadManager
-from .core.manager import DriverManager, INDEX_SITE_ROOT, NO_INDEX_SITE
+from .core.manager import DriverManager, get_driver_site
 from .drivers.firefox import GeckoDriver
 
 
 class GeckoDriverManager(DriverManager):
     def __init__(
             self,
             version: Optional[str] = None,
             os_type: Optional[str] = None,
             path: Optional[str] = None,
             name: str = "geckodriver",
-            url: str = f"{INDEX_SITE_ROOT}/firefox",
-            latest_release_url: str = f"{INDEX_SITE_ROOT}/firefox/LATEST_RELEASE",
+            url: str = f"firefox",
+            latest_release_url: str = f"firefox/LATEST_RELEASE",
             cache_valid_range: int = 1,
             download_manager: Optional[DownloadManager] = None,
-            use_index=not NO_INDEX_SITE,
     ):
         download_manager = download_manager or WDMDownloadManager()
+
         driver = GeckoDriver(
             version=version,
             os_type=os_type,
             name=name,
-            url=url,
-            latest_release_url=latest_release_url,
+            url=urljoin(get_driver_site(), url),
+            latest_release_url=urljoin(get_driver_site(), latest_release_url),
             http_client=download_manager.http_client,
-            use_index=use_index,
         )
         DriverManager.__init__(
             self, driver, path,
             cache_valid_range=cache_valid_range,
             download_manager=download_manager
         )
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/microsoft.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/microsoft.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import os
 from typing import Optional
+from urllib.parse import urljoin
 
 from .core.download_manager import DownloadManager, WDMDownloadManager
-from .core.manager import DriverManager, INDEX_SITE_ROOT, NO_INDEX_SITE
+from .core.manager import DriverManager, get_driver_site
 from .drivers.edge import EdgeChromiumDriver
 from .drivers.ie import IEDriver
 
 
 class IEDriverManager(DriverManager):
     def __init__(
             self,
             version: Optional[str] = None,
             os_type: Optional[str] = None,
             path: Optional[str] = None,
             name: str = "IEDriverServer",
-            url: str = f"{INDEX_SITE_ROOT}/ie",
-            latest_release_url: str = f"{INDEX_SITE_ROOT}/ie/LATEST_RELEASE",
+            url: str = f"ie",
+            latest_release_url: str = f"ie/LATEST_RELEASE",
             cache_valid_range: int = 1,
             download_manager: Optional[DownloadManager] = None,
-            use_index=not NO_INDEX_SITE,
     ):
         download_manager = download_manager or WDMDownloadManager()
         driver = IEDriver(
             version=version,
             os_type=os_type,
             name=name,
-            url=url,
-            latest_release_url=latest_release_url,
+            url=urljoin(get_driver_site(), url),
+            latest_release_url=urljoin(get_driver_site(), latest_release_url),
             http_client=download_manager.http_client,
-            use_index=use_index,
         )
         DriverManager.__init__(
             self, driver, path, cache_valid_range,
             download_manager=download_manager
         )
 
     def install(self) -> str:
@@ -42,29 +41,27 @@
 class EdgeChromiumDriverManager(DriverManager):
     def __init__(
             self,
             version: Optional[str] = None,
             os_type: str = None,
             path: Optional[str] = None,
             name: str = "edgedriver",
-            url: str = f"{INDEX_SITE_ROOT}/edge",
-            latest_release_url: str = f"{INDEX_SITE_ROOT}/edge/LATEST_RELEASE",
+            url: str = f"edge",
+            latest_release_url: str = f"edge/LATEST_RELEASE",
             cache_valid_range: int = 1,
             download_manager: Optional[DownloadManager] = None,
-            use_index=not NO_INDEX_SITE,
     ):
         download_manager = download_manager or WDMDownloadManager()
         driver = EdgeChromiumDriver(
             version=version,
             os_type=os_type,
             name=name,
-            url=url,
-            latest_release_url=latest_release_url,
+            url=urljoin(get_driver_site(), url),
+            latest_release_url=urljoin(get_driver_site(), latest_release_url),
             http_client=download_manager.http_client,
-            use_index=use_index,
         )
         DriverManager.__init__(
             self, driver, path, cache_valid_range,
             download_manager=download_manager
         )
 
     def install(self) -> str:
```

### Comparing `hf-webdriver-manager-0.1.0/webdriver_manager/opera.py` & `hf-webdriver-manager-0.2.0/webdriver_manager/opera.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import os
 from typing import Optional
+from urllib.parse import urljoin
 
 from .core.download_manager import DownloadManager, WDMDownloadManager
-from .core.manager import DriverManager, INDEX_SITE_ROOT, NO_INDEX_SITE
+from .core.manager import DriverManager, get_driver_site
 from .drivers.opera import OperaDriver
 
 
 class OperaDriverManager(DriverManager):
     def __init__(
             self,
             version: Optional[str] = None,
             os_type: Optional[str] = None,
             path: Optional[str] = None,
             name: str = "operadriver",
-            url: str = f"{INDEX_SITE_ROOT}/opera",
-            latest_release_url: str = f"{INDEX_SITE_ROOT}/opera/LATEST_RELEASE",
+            url: str = f"opera",
+            latest_release_url: str = f"opera/LATEST_RELEASE",
             cache_valid_range: int = 1,
             download_manager: Optional[DownloadManager] = None,
-            use_index=not NO_INDEX_SITE,
     ):
+
         download_manager = download_manager or WDMDownloadManager()
         driver = OperaDriver(
             name=name,
             version=version,
             os_type=os_type,
-            url=url,
-            latest_release_url=latest_release_url,
+            url=urljoin(get_driver_site(), url),
+            latest_release_url=urljoin(get_driver_site(), latest_release_url),
             http_client=download_manager.http_client,
-            use_index=use_index,
         )
         DriverManager.__init__(
             self, driver, path, cache_valid_range,
             download_manager=download_manager
         )
 
     def install(self) -> str:
```

