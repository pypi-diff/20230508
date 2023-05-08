# Comparing `tmp/automation-common-test-1.4.0.tar.gz` & `tmp/automation-common-test-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-common-test-1.4.0.tar", last modified: Mon May  8 14:00:52 2023, max compression
+gzip compressed data, was "automation-common-test-1.5.0.tar", last modified: Mon May  8 14:57:00 2023, max compression
```

## Comparing `automation-common-test-1.4.0.tar` & `automation-common-test-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:00:52.291281 automation-common-test-1.4.0/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-08 14:00:52.291089 automation-common-test-1.4.0/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-1.4.0/README.md
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:00:52.289407 automation-common-test-1.4.0/automation_common_test.egg-info/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-08 14:00:52.000000 automation-common-test-1.4.0/automation_common_test.egg-info/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      420 2023-05-08 14:00:52.000000 automation-common-test-1.4.0/automation_common_test.egg-info/SOURCES.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-08 14:00:52.000000 automation-common-test-1.4.0/automation_common_test.egg-info/dependency_links.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-08 14:00:52.000000 automation-common-test-1.4.0/automation_common_test.egg-info/top_level.txt
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:00:52.290204 automation-common-test-1.4.0/helpers/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-1.4.0/helpers/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-1.4.0/helpers/base_locator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     5737 2023-05-08 13:59:43.000000 automation-common-test-1.4.0/helpers/driver_manager.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-1.4.0/helpers/soft_check.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)    66006 2023-04-27 06:59:19.000000 automation-common-test-1.4.0/helpers/web_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-08 14:00:52.291328 automation-common-test-1.4.0/setup.cfg
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-08 14:00:46.000000 automation-common-test-1.4.0/setup.py
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:00:52.290885 automation-common-test-1.4.0/utils/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-1.4.0/utils/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-1.4.0/utils/config_parser.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-1.4.0/utils/encryption_decryption.py
--rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4591 2023-05-07 05:57:59.000000 automation-common-test-1.4.0/utils/post_results_teams.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:57:00.305450 automation-common-test-1.5.0/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-08 14:57:00.305232 automation-common-test-1.5.0/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-1.5.0/README.md
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:57:00.302323 automation-common-test-1.5.0/automation_common_test.egg-info/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-08 14:57:00.000000 automation-common-test-1.5.0/automation_common_test.egg-info/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      420 2023-05-08 14:57:00.000000 automation-common-test-1.5.0/automation_common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-08 14:57:00.000000 automation-common-test-1.5.0/automation_common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-08 14:57:00.000000 automation-common-test-1.5.0/automation_common_test.egg-info/top_level.txt
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:57:00.303623 automation-common-test-1.5.0/helpers/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-1.5.0/helpers/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-1.5.0/helpers/base_locator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     6022 2023-05-08 14:56:34.000000 automation-common-test-1.5.0/helpers/driver_manager.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-1.5.0/helpers/soft_check.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)    66006 2023-04-27 06:59:19.000000 automation-common-test-1.5.0/helpers/web_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-08 14:57:00.305509 automation-common-test-1.5.0/setup.cfg
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-08 14:56:55.000000 automation-common-test-1.5.0/setup.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 14:57:00.304849 automation-common-test-1.5.0/utils/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-1.5.0/utils/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-1.5.0/utils/config_parser.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-1.5.0/utils/encryption_decryption.py
+-rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4591 2023-05-07 05:57:59.000000 automation-common-test-1.5.0/utils/post_results_teams.py
```

### Comparing `automation-common-test-1.4.0/README.md` & `automation-common-test-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.4.0/helpers/driver_manager.py` & `automation-common-test-1.5.0/helpers/driver_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,24 +131,28 @@
 
 
 def set_chrome_options():
     options = webdriver.ChromeOptions()
     if current_os == "Linux":
         options.binary_location = "/usr/bin/google-chrome"
         options.add_argument('--disable-dev-shm-usage')
-    # options.add_argument("--disable-setuid-sandbox")
-    options.add_argument("--no-sandbox")
+    # options.add_argument("--disable-blink-features")
+    user_agent = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.50 ' \
+                 'Safari/537.36 '
+    options.add_argument(f'user-agent={user_agent}')
+    options.add_argument("--disable-blink-features=AutomationControlled")
+    options.add_argument("--disable-setuid-sandbox")
     options.add_argument("--disable-notifications")
     options.add_argument("--disable-popup-blocking")
     options.add_argument("--allow-insecure-localhost")
     options.add_argument('ignore-certificate-errors')
     options.add_experimental_option('excludeSwitches', ['enable-logging'])
     preferences = {
         "profile.default_content_setting_values.automatic_downloads": 1,
-        # "download.default_directory": output_folder,
+        "download.default_directory": output_folder,
         "download.prompt_for_download": False,
         "download.directory_upgrade": True,
         "safebrowsing.enabled": True
     }
     options.add_experimental_option("prefs", preferences)
     return options
```

### Comparing `automation-common-test-1.4.0/helpers/soft_check.py` & `automation-common-test-1.5.0/helpers/soft_check.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.4.0/helpers/web_operations.py` & `automation-common-test-1.5.0/helpers/web_operations.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.4.0/utils/encryption_decryption.py` & `automation-common-test-1.5.0/utils/encryption_decryption.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.4.0/utils/post_results_teams.py` & `automation-common-test-1.5.0/utils/post_results_teams.py`

 * *Files identical despite different names*

