# Comparing `tmp/vigilant_kit-1.2.1.tar.gz` & `tmp/vigilant_kit-1.2.2.tar.gz`

## Comparing `vigilant_kit-1.2.1.tar` & `vigilant_kit-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/.vigilant.env.example
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/actions.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/browser_options.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/LICENSE
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/.vigilant.env.example
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/bin/doc_generator.py
+-rw-r--r--   0        0        0    31508 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/actions.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/browser_options.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/PKG-INFO
```

### Comparing `vigilant_kit-1.2.1/docs/browser_options.md` & `vigilant_kit-1.2.2/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/docs/native_selenium.md` & `vigilant_kit-1.2.2/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/docs/selenium_install.md` & `vigilant_kit-1.2.2/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/docs/tutorial_pytest.md` & `vigilant_kit-1.2.2/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/docs/vigilant_pytest.md` & `vigilant_kit-1.2.2/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/docs/vigilant_unittest.md` & `vigilant_kit-1.2.2/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.2/src/vgl_cli/install_dev_kit_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.2/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.2/src/vgl_cli/install_webdriver_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/src/vgl_cli/run_selenium_command.py` & `vigilant_kit-1.2.2/src/vgl_cli/run_selenium_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.2/src/vgl_cli/vgl.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.2/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/.gitignore` & `vigilant_kit-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/LICENSE` & `vigilant_kit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.1/README.md` & `vigilant_kit-1.2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Vigilant Kit
-Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. It provides
-methods for interacting with the WebBrowser, assertions, and waiting. With Vigilant, you can start writing complex test
+Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With Vigilant, you can start writing complex test
 cases in a minute.
 
 ## Why Vigilant?
-- **Easy to start & Fast To Write**: Easy configuration process, straightforward way to writing your tests.
-Vigilant provides you with methods that help you write functional tests quickly without spending time on writing 
-boilerplate code every time you start a new project. 
+- **Easy to start & Fast To Write**: Vigilant provides you with methods that help you write functional tests quickly 
+without spending time on writing boilerplate code every time you start a new project.
 - **Flexible Framework Usage**: Usage is not limited to a single testing framework; you can use Vigilant with unittest,
   pytest, or anything else.
 
 ## What it includes?
 Methods for **interacting** with WebBrowser (`click`, `scroll_to`,  etc.), **assertions** (`see`, `dont_see`, `see_text`
 , etc.) **waiters** (`wait_for_element_to_be_visible`, `wait_for_element_to_be_clickable`, etc.)
 It is already there, ready to use.
```

### Comparing `vigilant_kit-1.2.1/pyproject.toml` & `vigilant_kit-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.2.1/PKG-INFO` & `vigilant_kit-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Description-Content-Type: text/markdown
 
 # Vigilant Kit
-Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. It provides
-methods for interacting with the WebBrowser, assertions, and waiting. With Vigilant, you can start writing complex test
+Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With Vigilant, you can start writing complex test
 cases in a minute.
 
 ## Why Vigilant?
-- **Easy to start & Fast To Write**: Easy configuration process, straightforward way to writing your tests.
-Vigilant provides you with methods that help you write functional tests quickly without spending time on writing 
-boilerplate code every time you start a new project. 
+- **Easy to start & Fast To Write**: Vigilant provides you with methods that help you write functional tests quickly 
+without spending time on writing boilerplate code every time you start a new project.
 - **Flexible Framework Usage**: Usage is not limited to a single testing framework; you can use Vigilant with unittest,
   pytest, or anything else.
 
 ## What it includes?
 Methods for **interacting** with WebBrowser (`click`, `scroll_to`,  etc.), **assertions** (`see`, `dont_see`, `see_text`
 , etc.) **waiters** (`wait_for_element_to_be_visible`, `wait_for_element_to_be_clickable`, etc.)
 It is already there, ready to use.
```

