# Comparing `tmp/robocorp_browser-0.2.0.tar.gz` & `tmp/robocorp_browser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.2.0.tar", max compression
+gzip compressed data, was "robocorp_browser-0.3.0.tar", max compression
```

## Comparing `robocorp_browser-0.2.0.tar` & `robocorp_browser-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       94 2023-04-04 11:49:45.057278 robocorp_browser-0.2.0/README.md
--rw-r--r--   0        0        0      553 2023-04-25 10:40:34.964275 robocorp_browser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-04-25 10:39:03.643383 robocorp_browser-0.2.0/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     3106 2023-04-25 10:39:03.643516 robocorp_browser-0.2.0/src/robocorp/browser/browser.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 robocorp_browser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-04-28 10:50:56.511915 robocorp_browser-0.3.0/README.md
+-rw-r--r--   0        0        0      704 2023-05-08 12:31:25.572018 robocorp_browser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-05-08 08:00:17.798903 robocorp_browser-0.3.0/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     2948 2023-05-08 10:36:59.939742 robocorp_browser-0.3.0/src/robocorp/browser/browser.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 robocorp_browser-0.3.0/PKG-INFO
```

### Comparing `robocorp_browser-0.2.0/pyproject.toml` & `robocorp_browser-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.2.0"
+version = "0.3.0"
 description = "Robocorp browser automation library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
-    "Antero V. <antero@robocorp.com>",
+	"Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 playwright = "^1.32.1"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = ".."}
+black = "^23.1.0"
+ruff = "^0.0.255"
+mypy = "^1.1.1"
+pytest = "^7.2.2"
+pytest-xdist = "^3.2.1"
+pytest-regressions = "1.0.6"
+lazydocs = "^0.4.8"
+pydocstyle = "^6.3.0"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_browser-0.2.0/src/robocorp/browser/browser.py` & `robocorp_browser-0.3.0/src/robocorp/browser/browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from pathlib import Path
+# TODO: don't let playwright print directly into stdout, it's breaking console behaviour
 import platform
+from pathlib import Path
 from typing import Literal
 
-from playwright.sync_api import Browser, Page, sync_playwright as _sync_playwright
+from playwright.sync_api import Browser, Page
+from playwright.sync_api import sync_playwright as _sync_playwright
 
 
 def _registry_path(browser: Literal["chrome", "firefox"]) -> str:
     if platform.system() == "Windows":
         import winreg
 
         location = winreg.HKEY_LOCAL_MACHINE
@@ -35,40 +37,41 @@
     },
 }
 
 
 def _get_executable_path(browser: Literal["firefox", "chrome"]) -> str:
     browser = browser.lower()
     system = platform.system()
+
     if system == "Windows":
         return _registry_path(browser)
 
-    system = platform.system()
     assert browser in EXECUTABLE_PATHS
     executable_path = EXECUTABLE_PATHS[browser][system]
     assert Path(executable_path).exists()
+
     return str(executable_path)
 
 
 def open_browser(
     browser: Literal["firefox", "chrome"] = "chrome",
     headless=True
     # TODO: support more args
 ) -> Browser:
-    """Launches a Playwright browser instance.
+    """Launch a Playwright browser instance.
 
     Args:
-        browser: Specifies which browser to use. Supported browsers are: ``chrome`` and ``firefox``.
+        browser: Specifies which browser to use.
+            Supported browsers are: ``chrome`` and ``firefox``.
         headless: If set to False a GUI is provided, otherwise it is hidden.
 
     Returns:
         Browser: A Browser instance.
 
     """
-
     playwright = _sync_playwright().start()
 
     assert playwright
     # TODO: allow user to also pass their own custom path?
     executable_path = _get_executable_path(browser)
 
     if browser == "chrome":
@@ -77,15 +80,15 @@
     launched_browser = playwright[browser].launch(
         executable_path=executable_path, headless=headless
     )
     return launched_browser
 
 
 def open_url(url: str, headless=True) -> Page:
-    """Launches a Playwright browser instance and opens the given URL.
+    """Launch a Playwright browser instance and opens the given URL.
 
     Note:
         Uses the ``chrome`` browser.
 
     Args:
         url: Navigates to the provided URL.
         headless: If set to False a GUI is provided, otherwise it is hidden.
@@ -94,21 +97,7 @@
         Page: A Page instance.
 
     """
     browser = open_browser(headless=headless)
     page = browser.new_page()
     page.goto(url)
     return page
-
-
-# TODO: don't let playwright print directly into stdout, it's breaking console behaviour
-
-# Close All Browsers
-
-
-#  Click Button    Start
-
-
-# Input Text    alias:First Name    ${person}[First Name]
-
-
-# Capture Element Screenshot    alias:Congratulations
```

### Comparing `robocorp_browser-0.2.0/PKG-INFO` & `robocorp_browser-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 0.2.0
+Version: 0.3.0
 Summary: Robocorp browser automation library
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

