# Comparing `tmp/digital_multimeter-0.5.1.tar.gz` & `tmp/digital_multimeter-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_multimeter-0.5.1.tar", max compression
+gzip compressed data, was "digital_multimeter-0.5.2.tar", max compression
```

## Comparing `digital_multimeter-0.5.1.tar` & `digital_multimeter-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1273 2023-05-06 02:11:48.657947 digital_multimeter-0.5.1/LICENSE
--rw-r--r--   0        0        0     3155 2023-05-07 01:42:21.389047 digital_multimeter-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2617 2023-05-06 13:52:36.944084 digital_multimeter-0.5.1/readme.md
--rw-r--r--   0        0        0      404 2023-05-07 01:42:21.391047 digital_multimeter-0.5.1/src/digital_multimeter/__init__.py
--rw-r--r--   0        0        0        0 2020-11-08 01:13:49.217434 digital_multimeter-0.5.1/src/digital_multimeter/cli/__init__.py
--rw-r--r--   0        0        0     3582 2023-05-06 13:58:12.436781 digital_multimeter-0.5.1/src/digital_multimeter/cli/click.py
--rw-r--r--   0        0        0     3462 2023-05-06 02:27:22.944278 digital_multimeter-0.5.1/src/digital_multimeter/cli/config.py
--rw-r--r--   0        0        0      442 2023-05-07 00:51:28.258205 digital_multimeter-0.5.1/src/digital_multimeter/cli/entrypoints.py
--rw-r--r--   0        0        0       47 2023-05-06 02:27:22.925278 digital_multimeter-0.5.1/src/digital_multimeter/exceptions.py
--rw-r--r--   0        0        0     2087 2023-05-06 14:21:55.093427 digital_multimeter-0.5.1/src/digital_multimeter/main.py
--rw-r--r--   0        0        0      245 2023-05-06 02:12:07.448155 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterBase.py
--rw-r--r--   0        0        0     6727 2023-05-06 02:50:14.875375 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterEDI9604.py
--rw-r--r--   0        0        0     8680 2023-05-06 02:50:14.889375 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py
--rw-r--r--   0        0        0    13869 2023-05-06 02:50:21.414447 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py
--rw-r--r--   0        0        0     1076 2023-05-06 02:40:10.689751 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/__init__.py
--rw-r--r--   0        0        0       35 2023-05-06 02:44:08.655364 digital_multimeter-0.5.1/src/digital_multimeter/utils/__init__.py
--rw-r--r--   0        0        0     2323 2023-05-06 02:27:22.934278 digital_multimeter-0.5.1/src/digital_multimeter/utils/cli_output.py
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 digital_multimeter-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-05-07 01:44:56.429713 digital_multimeter-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3380 2023-05-07 13:37:32.685899 digital_multimeter-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2616 2023-05-08 01:31:13.891811 digital_multimeter-0.5.2/readme.md
+-rw-r--r--   0        0        0      404 2023-05-07 13:37:32.690899 digital_multimeter-0.5.2/src/digital_multimeter/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-08 01:13:49.217434 digital_multimeter-0.5.2/src/digital_multimeter/cli/__init__.py
+-rw-r--r--   0        0        0     3582 2023-05-07 01:44:56.510713 digital_multimeter-0.5.2/src/digital_multimeter/cli/click.py
+-rw-r--r--   0        0        0     3462 2023-05-07 01:44:56.515714 digital_multimeter-0.5.2/src/digital_multimeter/cli/config.py
+-rw-r--r--   0        0        0      442 2023-05-07 01:44:56.519713 digital_multimeter-0.5.2/src/digital_multimeter/cli/entrypoints.py
+-rw-r--r--   0        0        0       47 2023-05-07 01:44:56.523714 digital_multimeter-0.5.2/src/digital_multimeter/exceptions.py
+-rw-r--r--   0        0        0     2087 2023-05-07 01:44:56.527714 digital_multimeter-0.5.2/src/digital_multimeter/main.py
+-rw-r--r--   0        0        0      245 2023-05-07 01:44:56.533714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterBase.py
+-rw-r--r--   0        0        0     6727 2023-05-07 01:44:56.538714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterEDI9604.py
+-rw-r--r--   0        0        0     8680 2023-05-07 01:44:56.544714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py
+-rw-r--r--   0        0        0    13947 2023-05-07 13:32:31.491604 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py
+-rw-r--r--   0        0        0     1076 2023-05-07 01:44:56.554714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-07 01:44:56.561714 digital_multimeter-0.5.2/src/digital_multimeter/utils/__init__.py
+-rw-r--r--   0        0        0     2323 2023-05-07 01:44:56.566714 digital_multimeter-0.5.2/src/digital_multimeter/utils/cli_output.py
+-rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 digital_multimeter-0.5.2/PKG-INFO
```

### Comparing `digital_multimeter-0.5.1/LICENSE` & `digital_multimeter-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/pyproject.toml` & `digital_multimeter-0.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "digital-multimeter"
-version = "0.5.1"
+version = "0.5.2"
 description = "Digital Multimeter provides both a CLI interface and a Python API interface to receive data from a variety of digital multimeters."
 authors = ["Nicholas de Jong <contact@nicholasdejong.com>"]
 license = "BSD-2-Clause"
 readme = "readme.md"
 packages = [{ include = "digital_multimeter", from = "src" }]
-classifiers = ["Environment :: Console", "Intended Audience :: Developers", "Intended Audience :: Information Technology", "Programming Language :: Python :: 3", "License :: OSI Approved :: BSD License"]
+classifiers = [
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "License :: OSI Approved :: BSD License"
+]
 keywords = ["multimeter", "digital multimeter", "dmm", "Digitech", "Digitek", "TekPower", "UniTrend", "Voltcraft"]
 
 [tool.poetry.urls]
 Documentation = "https://digital-multimeter.readthedocs.io/en/latest/"
 Homepage = "https://digital-multimeter.readthedocs.io/en/latest/"
 Repository = "https://github.com/ndejong/digital-multimeter.git"
 "Bug Tracker" = "https://github.com/ndejong/digital-multimeter/issues"
 
 [tool.poetry.scripts]
 dmm = "digital_multimeter.cli.entrypoints:dmm"
 
 [tool.poetry.dependencies]
 python = "^3.5"
-click = ">=7.0.0,<9.0.0"    # https://pypi.org/project/click/#history
-pyserial = ">=3.0.0,<4.0.0" # https://pypi.org/project/pyserial/#history
-pyusb = ">=1.0.0,<2.0.0"    # https://pypi.org/project/pyusb/#history
+click = ">=7.0.0,<9.0.0"        # https://pypi.org/project/click/#history
+pyserial = ">=3.0.0,<4.0.0"     # https://pypi.org/project/pyserial/#history
+pyusb = ">=1.0.0,<2.0.0"        # https://pypi.org/project/pyusb/#history
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"             # https://pypi.org/project/black/#history
-flake8 = "^6.0"             # https://pypi.org/project/flake8/#history
-isort = "^5.12"             # https://pypi.org/project/isort/#history
-pytest = "^7.3"             # https://pypi.org/project/pytest/#history
-safety = "2.4.0b1"          # https://pypi.org/project/safety/#history
-mkdocs = "^1.4"             # https://pypi.org/project/mkdocs/#history
-mkdocs-material = "^9.1"    # https://pypi.org/project/mkdocs-material/#history
-novella = "^0.2"            # https://pypi.org/project/novella/#history
-pydoc-markdown = "^4.6"     # https://pypi.org/project/pydoc-markdown/#history
-
-[tool.poetry.plugins."slap.plugins.repository_ci"]
-github-actions = "slap.ext.repository_ci.github_actions:GithubActionsRepositoryCIPlugin"
+black = "^23.3"                 # https://pypi.org/project/black/#history
+flake8 = "^6.0"                 # https://pypi.org/project/flake8/#history
+isort = "^5.12"                 # https://pypi.org/project/isort/#history
+pytest = "^7.3"                 # https://pypi.org/project/pytest/#history
+safety = "2.4.0b1"              # https://pypi.org/project/safety/#history
+mkdocs = "^1.4"                 # https://pypi.org/project/mkdocs/#history
+# NB: docs/requirements.txt needs to be kept up-to-date manually
+novella = "^0.2"                # https://pypi.org/project/novella/#history
+pydoc-markdown = "^4.6"         # https://pypi.org/project/pydoc-markdown/#history
+mkdocs-material = "^9.1"        # https://pypi.org/project/mkdocs-material/#history
 
 [tool.poetry.plugins."slap.plugins.check"]
 changelog = "slap.ext.checks.changelog:ChangelogValidationCheckPlugin"
 general = "slap.ext.checks.general:GeneralChecksPlugin"
 poetry = "slap.ext.checks.poetry:PoetryChecksPlugin"
 release = "slap.ext.checks.release:ReleaseChecksPlugin"
 
@@ -72,9 +79,13 @@
 combine_as_imports = true
 
 [tool.black]
 line-length = 120
 
 [tool.readthedocs-custom-steps]
 script = """
-novella --site-dir _site/html
+cd docs
+novella --base-url /en/latest/
+mkdir -p ../_readthedocs
+mv _site ../_readthedocs/html
+echo "COMMAND-PREVENTED: $@"
 """
```

### Comparing `digital_multimeter-0.5.1/readme.md` & `digital_multimeter-0.5.2/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/digital-multimeter.svg)](https://github.com/ndejong/digital-multimeter/)
 [![Read the Docs](https://img.shields.io/readthedocs/digital-multimeter)](https://digital-multimeter.readthedocs.io)
 ![License](https://img.shields.io/github/license/ndejong/digital-multimeter.svg)
 
 Digital Multimeter provides both a CLI and Python API interface to receive data 
 from a variety of digital multimeters.  
 
-See the list of supported multimeters [here](https://digital-multimeter.readthedocs.io/en/latest/docs/supported-multimeters).
+See the list of supported multimeters [here](https://digital-multimeter.readthedocs.io/en/latest/supported-multimeters/).
 
 ## Features
 * Command line and Python module interface to digital multimeters
 * Continuous live data readings (using `--count 0`)
 * Output in **json** or **csv** formats
 * Output to console or file, allowing other tools to pickup and use the data
 * Configuration via config-file or environment-variables
@@ -53,15 +53,15 @@
     "unit_name": "second",
     "unit_symbol": "s"
   }
 }
 ```
 
 ## Python API Usage
-Python-module documentation is available [here](https://digital-multimeter.readthedocs.io/en/latest/docs/python-module/).
+Python-module documentation is available [here](https://digital-multimeter.readthedocs.io/en/latest/api/digitalmultimeter/).
 
 ## Project
 * Github - [github.com/ndejong/digital-multimeter](https://github.com/ndejong/digital-multimeter)
 * PyPI - [pypi.python.org/pypi/digital-multimeter](https://pypi.python.org/pypi/digital-multimeter/)
 * ReadTheDocs - [digital-multimeter.readthedocs.io](https://digital-multimeter.readthedocs.io)
 
 ---
```

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/cli/click.py` & `digital_multimeter-0.5.2/src/digital_multimeter/cli/click.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/cli/config.py` & `digital_multimeter-0.5.2/src/digital_multimeter/cli/config.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/main.py` & `digital_multimeter-0.5.2/src/digital_multimeter/main.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterEDI9604.py` & `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterEDI9604.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py` & `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py` & `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     - https://github.com/jsyk/VC870_USB_Datalog
     - http://erste.de/UT61/index.html
     - https://github.com/pklaus/ut61e_python
 """
 
 import logging
 import math
+import platform
 import re
 import time
 
 import usb.core
 import usb.util
 
 from ..exceptions import MultimeterException
@@ -83,20 +84,20 @@
         else:
             logger.debug(
                 "Connected to VID={}, PID={} successfully".format(connect_info.group(1), connect_info.group(2))
             )
 
         # This reset helps to readout the CH9325
         self.dev.reset()
-
-        if self.dev.is_kernel_driver_active(0) is True:
-            logging.debug("Detaching kernel driver before using")
-            self.dev.detach_kernel_driver(0)
-        else:
-            logging.debug("Kernel driver already detached")
+        if platform.system() != "Windows":
+            if self.dev.is_kernel_driver_active(0) is True:
+                logging.debug("Detaching kernel driver before using")
+                self.dev.detach_kernel_driver(0)
+            else:
+                logging.debug("Kernel driver already detached")
 
         # Set default configuration and get it
         self.dev.set_configuration()
         cfg = self.dev.get_active_configuration()
 
         # get an endpoint instance
         interface_number = cfg[(0, 0)].bInterfaceNumber
```

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/__init__.py` & `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/__init__.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/src/digital_multimeter/utils/cli_output.py` & `digital_multimeter-0.5.2/src/digital_multimeter/utils/cli_output.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.1/PKG-INFO` & `digital_multimeter-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-multimeter
-Version: 0.5.1
+Version: 0.5.2
 Summary: Digital Multimeter provides both a CLI interface and a Python API interface to receive data from a variety of digital multimeters.
 License: BSD-2-Clause
 Keywords: multimeter,digital multimeter,dmm,Digitech,Digitek,TekPower,UniTrend,Voltcraft
 Author: Nicholas de Jong
 Author-email: contact@nicholasdejong.com
 Requires-Python: >=3.5,<4.0
 Classifier: Environment :: Console
@@ -15,15 +15,18 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=7.0.0,<9.0.0)
 Requires-Dist: pyserial (>=3.0.0,<4.0.0)
 Requires-Dist: pyusb (>=1.0.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/ndejong/digital-multimeter/issues
 Project-URL: Documentation, https://digital-multimeter.readthedocs.io/en/latest/
 Project-URL: Homepage, https://digital-multimeter.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ndejong/digital-multimeter.git
@@ -34,15 +37,15 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/digital-multimeter.svg)](https://github.com/ndejong/digital-multimeter/)
 [![Read the Docs](https://img.shields.io/readthedocs/digital-multimeter)](https://digital-multimeter.readthedocs.io)
 ![License](https://img.shields.io/github/license/ndejong/digital-multimeter.svg)
 
 Digital Multimeter provides both a CLI and Python API interface to receive data 
 from a variety of digital multimeters.  
 
-See the list of supported multimeters [here](https://digital-multimeter.readthedocs.io/en/latest/docs/supported-multimeters).
+See the list of supported multimeters [here](https://digital-multimeter.readthedocs.io/en/latest/supported-multimeters/).
 
 ## Features
 * Command line and Python module interface to digital multimeters
 * Continuous live data readings (using `--count 0`)
 * Output in **json** or **csv** formats
 * Output to console or file, allowing other tools to pickup and use the data
 * Configuration via config-file or environment-variables
@@ -84,15 +87,15 @@
     "unit_name": "second",
     "unit_symbol": "s"
   }
 }
 ```
 
 ## Python API Usage
-Python-module documentation is available [here](https://digital-multimeter.readthedocs.io/en/latest/docs/python-module/).
+Python-module documentation is available [here](https://digital-multimeter.readthedocs.io/en/latest/api/digitalmultimeter/).
 
 ## Project
 * Github - [github.com/ndejong/digital-multimeter](https://github.com/ndejong/digital-multimeter)
 * PyPI - [pypi.python.org/pypi/digital-multimeter](https://pypi.python.org/pypi/digital-multimeter/)
 * ReadTheDocs - [digital-multimeter.readthedocs.io](https://digital-multimeter.readthedocs.io)
 
 ---
```

