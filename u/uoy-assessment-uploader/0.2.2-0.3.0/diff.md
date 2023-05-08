# Comparing `tmp/uoy-assessment-uploader-0.2.2.tar.gz` & `tmp/uoy-assessment-uploader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy-assessment-uploader-0.2.2.tar", last modified: Sun May  7 20:31:01 2023, max compression
+gzip compressed data, was "uoy-assessment-uploader-0.3.0.tar", last modified: Mon May  8 15:54:42 2023, max compression
```

## Comparing `uoy-assessment-uploader-0.2.2.tar` & `uoy-assessment-uploader-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.2.2/LICENSE
--rw-r--r--   0        0        0     1012 2023-05-07 20:29:33.164903 uoy-assessment-uploader-0.2.2/README.md
--rw-r--r--   0        0        0      741 2023-05-07 17:33:43.930544 uoy-assessment-uploader-0.2.2/pyproject.toml
--rwxr-xr-x   0        0        0     7903 2023-05-07 20:30:47.028889 uoy-assessment-uploader-0.2.2/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.2.2/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-08 15:54:31.863871 uoy-assessment-uploader-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/README.md
+-rw-r--r--   0        0        0      741 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0     6783 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     1551 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/selenium.py
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.3.0/PKG-INFO
```

### Comparing `uoy-assessment-uploader-0.2.2/LICENSE` & `uoy-assessment-uploader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.2.2/pyproject.toml` & `uoy-assessment-uploader-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.2.2/uoy_assessment_uploader/__init__.py` & `uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Tool for automating submitting assessments to the University of York Computer Science department."""
 
 import getpass
-import json
+import hashlib
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Optional
 
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.support.wait import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 
+from .selenium import enter_exam_number, load_cookies, login, save_cookies, upload
 
-# todo: re-implement with saml auth and requests, as alternative to selenium
 
-
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 # timeout for selenium waits, in seconds
 TIMEOUT = 10
 
 DEFAULT_ARG_FILE = "exam.zip"
 DEFAULT_ARG_COOKIE_FILE = ".cookies.json"
 
@@ -102,56 +101,14 @@
     dry_run: bool
     cookie_file: Path
     save_cookies: bool
     delete_cookies: bool
     headless: bool
 
 
-def save_cookies(driver: WebDriver, fp: Path):
-    cookies = driver.get_cookies()
-    with open(fp, "w") as f:
-        json.dump(cookies, f)
-
-
-def load_cookies(driver: webdriver.Chrome, fp: Path):
-    try:
-        with open(fp) as f:
-            cookies = json.load(f)
-    except FileNotFoundError:
-        print("Not loading cookies, file doesn't exist.")
-    else:
-        print("Loading cookies.")
-        for c in cookies:
-            driver.execute_cdp_cmd("Network.setCookie", c)
-
-
-def login(driver: WebDriver, username: str, password: str):
-    input_username = driver.find_element(By.ID, "username")
-    input_username.send_keys(username)
-    input_password = driver.find_element(By.ID, "password")
-    input_password.send_keys(password)
-    input_button = driver.find_element(By.NAME, "_eventId_proceed")
-    input_button.click()
-
-
-def enter_exam_number(driver: WebDriver, exam_number: str):
-    input_exam_number = driver.find_element(By.ID, "examNumber")
-    input_exam_number.send_keys(exam_number)
-    input_exam_number.submit()
-
-
-def upload(driver: WebDriver, file_name: str, dry_run: bool):
-    input_file = driver.find_element(By.ID, "file")
-    input_file.send_keys(file_name)
-    input_checkbox = driver.find_element(By.ID, "ownwork")
-    input_checkbox.click()
-    if not dry_run:
-        input_checkbox.submit()
-
-
 def ensure_details(
     current: str, prompt: Optional[str] = None, hide: bool = False
 ) -> str:
     if current is not None:
         return current
 
     if hide:
@@ -217,23 +174,27 @@
 
 def main():
     # load arguments
     parser = get_parser()
     args = Args()
     parser.parse_args(namespace=args)
 
+    # verify arguments
+    submit_url = resolve_submit_url(args.submit_url)
     # check zip to be uploaded exists
     if not args.file.is_file():
         print(f"File doesn't exist '{args.file}'.")
         sys.exit(1)
     print(f"Found file '{args.file}'.")
     file_name = str(args.file.resolve())
-
-    # verify arguments
-    submit_url = resolve_submit_url(args.submit_url)
+    # display hash of file
+    with open(file_name, "rb") as f:
+        # noinspection PyTypeChecker
+        digest = hashlib.file_digest(f, hashlib.md5).hexdigest()
+    print(f"MD5 hash of file: {digest}")
 
     # webdriver setup
     # options
     driver_options = webdriver.ChromeOptions()
     if args.headless:
         driver_options.add_argument("--headless")
```

### Comparing `uoy-assessment-uploader-0.2.2/PKG-INFO` & `uoy-assessment-uploader-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.2.2
+Version: 0.3.0
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -33,25 +33,33 @@
 - ```shell
   python -m uoy_assessment_uploader --help
   ```
   or
 - ```shell
   uoy-assessment-uploader --help
   ```
-  
+
+Once it's submitted, you should receive an email to your uni address with confirmation.
+The email will show you the MD5 hash, like so:
+
+> MD5 hash of file: 97f212cda7e5200a67749cac560a06f4
+
+If this matches the hash shown by the program, you can be certain you successfully uploaded the right file.
+
 ## Example
 ```shell
 uoy-assessment-uploader --username "ab1234" --exam-number "Y1234567" --submit-url "/2021-2/submit/COM00012C/901/A"
 ```
 ```
 Found file 'exam.zip'.
-
+MD5 hash of file: 05086595c7c7c1a962d6eff6872e18c0
 [WDM] - Downloading: 100%|██████████| 6.98M/6.98M [00:00<00:00, 8.98MB/s]
 Loading cookies.
 Logging in..
 Password: <PASSWORD HIDDEN>
 Entering exam number..
 Uploading file...
 Uploaded successfully.
 Saving cookies.
+Finished!
 ```
```

