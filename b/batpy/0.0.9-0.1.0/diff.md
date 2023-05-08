# Comparing `tmp/batpy-0.0.9.tar.gz` & `tmp/batpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batpy-0.0.9.tar", max compression
+gzip compressed data, was "batpy-0.1.0.tar", max compression
```

## Comparing `batpy-0.0.9.tar` & `batpy-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rwxr-xr-x   0        0        0     1073 2023-05-04 11:50:54.051104 batpy-0.0.9/LICENSE
--rw-r--r--   0        0        0     4365 2023-05-04 11:50:54.051104 batpy-0.0.9/README.md
--rw-r--r--   0        0        0     1825 2023-05-04 11:51:27.531087 batpy-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/__init__.py
--rw-r--r--   0        0        0     5157 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/batpac_battery.py
--rw-r--r--   0        0        0    27747 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/batpac_tool.py
--rw-r--r--   0        0        0     2158 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30586 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batpac_config.toml
--rw-r--r--   0        0        0    83193 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48369 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batteries_config.toml
--rw-r--r--   0        0        0     2177 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/is_version_compatible.py
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 batpy-0.0.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-08 01:57:49.005917 batpy-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5605 2023-05-08 01:57:49.005917 batpy-0.1.0/README.md
+-rw-r--r--   0        0        0     1827 2023-05-08 01:58:24.470527 batpy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      236 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/__init__.py
+-rw-r--r--   0        0        0     5810 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/batpac_battery.py
+-rw-r--r--   0        0        0     3979 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/batpac_datasets.py
+-rw-r--r--   0        0        0    31170 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/batpac_tool.py
+-rw-r--r--   0        0        0   209566 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     2158 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30666 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    57647 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0    83193 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48449 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0   209566 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     2158 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30666 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    57647 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0    83193 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48449 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0      145 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/is_version_compatible.py
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 batpy-0.1.0/PKG-INFO
```

### Comparing `batpy-0.0.9/LICENSE` & `batpy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batpy-0.0.9/README.md` & `batpy-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
 [![Docs](https://github.com/rginster/batpy/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/documentation.yaml)
 [![pages-build-deployment](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment)
+[![codecov](https://codecov.io/gh/rginster/batpy/branch/main/graph/badge.svg?token=JH8L3B14AW)](https://codecov.io/gh/rginster/batpy)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/batpy)
 [![PyPi](https://img.shields.io/pypi/v/batpy.svg)](https://pypi.python.org/pypi/batpy)
 [![PyPi](https://img.shields.io/pypi/dm/batpy.svg)](https://pypi.python.org/pypi/batpy)
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
@@ -25,26 +26,50 @@
 `batpy` is able to read, write, and calculate batteries in the [BatPaC tool](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 
 
 ```python
 from batpy.batpac_battery import BatpacBattery
 from batpy.batpac_tool import BatpacTool
+from batpy import batpac_datasets
 
-# Constants
+# Paths to TOML configurations on local system
 BATPY_BATPAC_EXCEL = "./BatPaC 5.0 2022-07-22.xlsm"
 
 BATPY_BATPAC_BATTERY_CONFIG = "./batpy_batteries_config.toml"
-BATPY_BATPAC_USER_INPUT_CONFIG = "./batpy_batpac_user_input_cells.toml"
+BATPY_BATPAC_USER_INPUT_CONFIG = (
+    "./batpy_batpac_user_input_cells.toml"
+)
 BATPY_BATPAC_TOOL_CONFIG = "./batpy_batpac_config.toml"
 
 BATPY_BATPAC_TOOL_CALCULATION_VALIDATION_CONFIG = (
     "./batpy_batpac_calculation_and_validation_results.toml"
 )
 
+ADDITIONAL_USER_DEFINED_RESULTS_CELLS = (
+    "./batpy_batpac_summary_of_results.toml"
+)
+
+# Get included datasets
+# Show available versions
+batpac_datasets.get_available_batpy_dataset_versions()
+
+# Show latest version
+batpac_datasets.get_latest_batpy_dataset_version()
+
+
+# Show available dataset of specified version (default latest)
+batpac_datasets.get_available_batpy_dataset_names()
+
+
+# Load included dataset:
+batpy_batpac_battery_design = batpac_datasets.get_batpy_dataset(
+    "batpy_batpac_battery_design", "0.1.0"
+)
+
 
 # Create batteries
 bat1 = BatpacBattery("Battery 1")
 bat2 = BatpacBattery("Battery 2")
 bat3 = BatpacBattery("Battery 3")
 bat4 = BatpacBattery("Battery 4")
 bat5 = BatpacBattery("Battery 5")
@@ -53,15 +78,15 @@
 
 # Change battery properties
 # a) Write individual properties for created batteries
 bat1.set_new_property("Dashboard", "Number of modules in parallel", 10)
 
 # b) Load individiual battery configuration from file
 bat2.load_battery_file(
-    "./battery_config.toml", "Battery"
+    BATPY_BATPAC_BATTERY_CONFIG, "Battery 2"
 )
 
 # Create BatPaC instance
 battery_calculation = BatpacTool(
     BATPY_BATPAC_EXCEL,
     BATPY_BATPAC_USER_INPUT_CONFIG,
     BATPY_BATPAC_TOOL_CALCULATION_VALIDATION_CONFIG,
@@ -99,14 +124,29 @@
 # Load configuration file for BatPaC instance
 battery_calculation.load_batpac_file(BATPY_BATPAC_TOOL_CONFIG)
 
 # Write configuration in Excel file and calculate batteries
 battery_calculation.calculate()
 battery_calculation.read_calculation_and_validation_results()
 
+# Read additional user defined cells
+# a) From file path
+user_results = battery_calculation.read_from_user_input(
+    ADDITIONAL_USER_DEFINED_RESULTS_CELLS
+)
+print(user_results)
+print(user_results["Summary of Results"]["Battery 1"])
+
+# b) From included configuration
+user_results_included_configuration = battery_calculation.read_from_user_input(
+    batpy_batpac_battery_design
+)
+print(user_results_included_configuration)
+print(user_results_included_configuration["Battery Design"]["Battery 1"])
+
 # Save configuration from Excel:
 battery_calculation.save_config(
     batpac_path="./saved_batpac_config.toml",
     battery_path="./saved_batteries_config.toml",
 )
 
 # Save Excel file
```

### Comparing `batpy-0.0.9/pyproject.toml` & `batpy-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "batpy"
-version = "0.0.9"
+version = "0.1.0"
 description = "A python package to read, write, and calculate batteries in the BatPaC tool."
 authors = ["Raphael Ginster <r.ginster@tu-braunschweig.de>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rginster.github.io/batpy/"
 repository = "https://github.com/rginster/batpy"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 xlwings = "^0.30.4"
 pathlib = "^1.0.1"
 toml = "^0.10.2"
 prettytable = "^3.7.0"
 tqdm = "^4.65.0"
 semantic-version = "^2.10.0"
 
@@ -22,15 +22,15 @@
 flake8 = "^6.0.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 python-semantic-release = "^7.33.3"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
-myst-nb = {version = "^0.17.2", python = "^3.9"}
+myst-nb = {version = "^0.17.2", python = "^3.10"}
 sphinx-autoapi = "^2.1.0"
 sphinx-rtd-theme = "^1.2.0"
 pre-commit = "^3.3.1"
 removestar = "^1.3.1"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 dodgy = "^0.2.1"
@@ -50,11 +50,11 @@
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = false                      # don't auto-upload to PyPI
 remove_dist = false                         # don't remove dists
-patch_without_tag = true                    # patch release by default
+patch_without_tag = false                   # patch release by default
 
 [tool.black]
 line-length = 79
```

### Comparing `batpy-0.0.9/src/batpy/batpac_battery.py` & `batpy-0.1.0/src/batpy/batpac_battery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 # -*- coding: UTF-8 -*-
 """Module, which includes the class BatpacBattery
 """
 import logging
 from pathlib import Path
 
+import semantic_version
 import toml
 
-logger = logging.getLogger(__name__)
-logging.basicConfig(
-    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t\
-        %(lineno)s\t- %(message)s",
-    filename="batpy.log",
-    filemode="w",
-    level=logging.INFO,
-)
+import batpy
+from batpy.is_version_compatible import is_version_compatible
 
 
 class BatpacBattery:
     """Battery class for interaction with BatPaC
 
     This battery class is used to interact with BatPaC and stores battery
     parameters in the dictionary properties.
@@ -40,35 +35,37 @@
         "NCM811 - G"
 
         >>> battery2 = BatPaC_battery()
         >>> print(battery2.name)
         "Battery"
         """
         self.name = name
+        self.version = semantic_version.Version(batpy.__version__)
         logging.info("[ ] Create battery %s", self.name)
         self.properties = {}
         logging.info("[+] Battery %s created", self.name)
         logging.debug(
             "[ ] Properties of battery %s: %s",
             self.name,
             self.properties,
         )
 
     def load_battery_file(
-        self, path_to_battery_file: Path, battery_name: str = "Battery"
+        self, path_to_battery_file: Path | str, battery_name: str = "Battery"
     ) -> bool:
         """Load a battery configuration file
 
         Load the properties for a battery from a TOML battery configuration
         file.
 
         Parameters
         ----------
-        path_to_battery_file : Path
-            Path to the TOML battery configuration file.
+        path_to_battery_file : Path | str
+            Path to the TOML battery configuration file. It is also possible to
+            load the included batpy datasets.
         battery_name : str, optional
             Name of the table in the TOML file from which to load the battery
             properties. Thereby, the battery_name, by default "Battery", does
             not have to be equal to self.name.
 
         Returns
         -------
@@ -81,42 +78,56 @@
         Examples
         --------
         battery_config.toml contains a table with the name ["NCM"].
         All key - value pairs are to be loaded for the battery "NCM811 - G".
 
         >>> battery1 = BatPaC_battery("NCM811 - G")
         >>> battery1.load_battery_file("./battery_config.toml", "NCM")
+        >>> from batpy import batpac_datasets
+        >>> battery1.load_battery_file(
+                batpac_datasets.get_batpy_dataset("batpy_batteries_config"),
+                "Battery 1"
+            )
         """
         logging.info(
             "[ ] Load battery config for %s from %s",
             battery_name,
             path_to_battery_file,
         )
-        config = toml.load(path_to_battery_file)
-        loaded = False
-        if battery_name in config:
-            config = config[battery_name]
-            for sheet in config:
-                for key in config[sheet]:
-                    self.set_new_property(sheet, key, config[sheet][key])
-            logging.info(
-                "[+] Battery config for %s from %s loaded",
-                battery_name,
-                path_to_battery_file,
-            )
-            loaded = True
-        else:
-            logging.warning(
-                "[!] No battery config for %s in %s found",
-                battery_name,
-                path_to_battery_file,
+        try:
+            Path.exists(Path(path_to_battery_file))
+            config = toml.load(path_to_battery_file)
+        except (AttributeError, OSError):
+            config = toml.loads(path_to_battery_file)
+        config_metadata = config.pop("batpy")
+        if is_version_compatible(
+            self.version,
+            semantic_version.Version(config_metadata["BatPaC SemVer"]),
+        ):
+            loaded = False
+            if battery_name in config:
+                config = config[battery_name]
+                for sheet in config:
+                    for key in config[sheet]:
+                        self.set_new_property(sheet, key, config[sheet][key])
+                logging.info(
+                    "[+] Battery config for %s from %s loaded",
+                    battery_name,
+                    path_to_battery_file,
+                )
+                loaded = True
+            else:
+                logging.warning(
+                    "[!] No battery config for %s in %s found",
+                    battery_name,
+                    path_to_battery_file,
+                )
+            logging.debug(
+                "[ ] Battery properties for %s: %s", self.name, self.properties
             )
-        logging.debug(
-            "[ ] Battery properties for %s: %s", self.name, self.properties
-        )
         return loaded
 
     def set_property(self, sheet: str, name: str, value: any) -> None:
         """Set an existing property of the battery
 
         Set an existing property of the battery in the format
         {"sheet" : {"name" : value} }.
```

### Comparing `batpy-0.0.9/src/batpy/batpac_tool.py` & `batpy-0.1.0/src/batpy/batpac_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 # -*- coding: UTF-8 -*-
 """Module, which includes the class BatpacTool
 """
 import logging
-import warnings
 from pathlib import Path
 
 import semantic_version
 import toml
 import xlwings as xw
 from prettytable import PrettyTable
 from tqdm import tqdm
 
+import batpy
 from batpy.batpac_battery import BatpacBattery
 from batpy.is_version_compatible import is_version_compatible
 
-logger = logging.getLogger(__name__)
-logging.basicConfig(
-    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t\
-        %(lineno)s\t- %(message)s",
-    filename="batpy.log",
-    filemode="w",
-    level=logging.INFO,
-)
-
 
 class BatpacTool:
     """BatPaC class which interacts with the BatPaC Excel tool
 
     This BatPaC class is used to interact directly with the BatPaC Excel tool
     and can store individual batteries (class BatPaC_battery) and additional
     parameters of the BatPaC Excel tool in the dictionary properties.
     """
 
     def __init__(
         self,
         batpac_workbook_path: Path,
-        cell_definition_user_input_toml_path: Path,
-        cell_definition_calculation_and_validation_results: Path = None,
-        cell_definition_additional_user_input_toml_path: Path = None,
-        cell_definition_additional_user_results_toml_path: Path = None,
+        cell_definition_user_input_toml_path: Path | str,
+        cell_definition_calculation_validation_results: Path | str = None,
+        # cell_definition_additional_user_input_toml_path: Path = None,
+        # cell_definition_additional_user_results_toml_path: Path = None,
         excel_visible: bool = False,
     ) -> None:
         """Initialize BatPaC
 
         Initialize the BatPaC object.
 
         Parameters
         ----------
         batpac_workbook_path : Path
             Path to the BatPaC Excel tool (*.xlsm).
-        cell_definition_user_input_toml_path : Path
-            Path to the TOML file, which contains the configuration for the
-            standard user input cells (defined by Argonne National Laboratory)
-            in the BatPaC Excel tool.
-        cell_definition_calculation_and_validation_results : Path, optional
-            Path to the TOML file, which contains the configuration for the
-            calculation and validation results
-            in the BatPaC Excel tool, by default None.
+        cell_definition_user_input_toml_path : Path | str
+            Path to the TOML file or string (default dataset), which contains
+            the configuration for the standard user input cells (defined by
+            Argonne National Laboratory) in the BatPaC Excel tool.
+        cell_definition_calculation_validation_results : Path | str, optional
+            Path to the TOML file or string (default dataset), which contains
+            the configuration for the calculation and validation results in the
+            BatPaC Excel tool, by default None.
         cell_definition_additional_user_input_toml_path : Path, optional
             Path to the TOML file, which contains additional cells for user
             input, that are not included in the standard user inputs in the
             BatPaC Excel tool, by default None.
         cell_definition_additional_user_results_toml_path : Path, optional
             Path to the TOML file, which contains additional cells for  user
             input, that are not included in the standard user inputs in the
@@ -70,58 +61,50 @@
             False.
         """
         logging.info(
             "[ ] Create BatPaC from %s and load cell references from %s",
             batpac_workbook_path,
             cell_definition_user_input_toml_path,
         )
-        self.version = semantic_version.Version("0.1.0")
-        self.workbook_path = batpac_workbook_path
-        self.toml_path = cell_definition_user_input_toml_path
-        self.toml_calculation_validation_results_path = (
-            cell_definition_calculation_and_validation_results
+        self.version = semantic_version.Version(batpy.__version__)
+
+        self.excel_cells = self.load_user_file(
+            cell_definition_user_input_toml_path
         )
-        config = toml.load(self.toml_path)
-        config_metadata = config.pop("batpy")
-        self.batpac_version = config_metadata["BatPaC version"]
-        if is_version_compatible(
-            self.version,
-            semantic_version.Version(config_metadata["BatPaC SemVer"]),
-        ):
-            self.batpac_semver = semantic_version.Version(
-                config_metadata["BatPaC SemVer"]
+        if cell_definition_calculation_validation_results:
+            self.toml_calculation_validation_results = self.load_user_file(
+                cell_definition_calculation_validation_results
             )
-
-        self.excel_cells = config
         self.batteries = []
-        self.wb = xw.Book(batpac_workbook_path)
-        self.app = self.wb.app
-        self.app.visible = excel_visible
+        self.workbook = xw.Book(batpac_workbook_path)
+        # self.app = self.workbook.app
+        self.workbook.app.visible = excel_visible
         self.max_batteries = 7
         self.properties = {}
         logging.info(
-            "[+] Created BatPaC version %s (SemVer: %s) from %s and load \
+            "[+] Created BatPaC from %s and load \
                     cell references from %s",
-            self.batpac_version,
-            self.batpac_semver,
-            self.workbook_path,
-            self.toml_path,
+            batpac_workbook_path,
+            cell_definition_user_input_toml_path,
         )
 
     def __del__(self) -> None:
         """Destructor of BatPac object
 
         Set the Excel calculation method to "automatic" and the
         "screen_updating" to True after object destruction.
         """
         try:
-            self.wb.app.calculation = "automatic"
-            self.wb.app.screen_updating = True
+            self.workbook.app.calculation = "automatic"
+            self.workbook.app.screen_updating = True
         except BaseException as error:
             logging.error("An exception occurred: %s", error)
+            raise KeyError(
+                "Could not access the workbook (may already be closed)."
+            ) from error
 
     def is_version_compatible(
         self,
         version_to_check: semantic_version.Version,
         include_minor: bool = False,
     ) -> bool:
         """Check for version compatibility
@@ -149,29 +132,69 @@
         ValueError
             If version is not compatible a ValueError will occur.
         """
         return is_version_compatible(
             self.version, version_to_check, include_minor
         )
 
-    def load_batpac_file(self, path_to_batpac_file: Path) -> None:
+    def load_user_file(self, path_to_user_file: Path | str) -> dict:
+        """Load user file configuration
+
+        Load the user configuration from a TOML user file.
+
+        Parameters
+        ----------
+        path_to_user_file : Path | str
+            Path to the TOML user file or string (default dataset).
+
+        Returns
+        -------
+        dict
+            Returns dictionary representation of read TOML file.
+        """
+        logging.info("[ ] Load BatPaC file from %s", path_to_user_file)
+
+        try:
+            Path.exists(Path(path_to_user_file))
+            config = toml.load(path_to_user_file)
+        except (AttributeError, OSError):
+            config = toml.loads(path_to_user_file)
+        config_metadata = config.pop("batpy")
+        self.is_version_compatible(
+            semantic_version.Version(config_metadata["BatPaC SemVer"])
+        )
+        logging.info("[+] Loaded user file from %s", path_to_user_file)
+        logging.debug("[ ] Config properties %s", config)
+        return config
+
+    def load_batpac_file(self, path_to_batpac_file: Path | str) -> None:
         """Load BatPaC configuration
 
         Load the properties for the BatPaC object from a TOML battery
         configuration file.
 
         Parameters
         ----------
-        path_to_batpac_file : Path
+        path_to_batpac_file : Path | str
             Path to the TOML BatPaC configuration file.
         """
         logging.info("[ ] Load BatPaC file from %s", path_to_batpac_file)
-        self.properties = toml.load(path_to_batpac_file)
-        logging.info("[+] Loaded BatPaC file from %s", path_to_batpac_file)
-        logging.debug("[ ] BatPaC properties %s", self.properties)
+
+        try:
+            Path.exists(Path(path_to_batpac_file))
+            config = toml.load(path_to_batpac_file)
+        except (AttributeError, OSError):
+            config = toml.loads(path_to_batpac_file)
+        config_metadata = config.pop("batpy")
+        if self.is_version_compatible(
+            semantic_version.Version(config_metadata["BatPaC SemVer"])
+        ):
+            self.properties = config
+            logging.info("[+] Loaded BatPaC file from %s", path_to_batpac_file)
+            logging.debug("[ ] BatPaC properties %s", self.properties)
 
     def add_battery(self, batteries: list[BatpacBattery]) -> None:
         """Add battery object to BatPaC object
 
         Add multiple battery objects to the BatPaC object.
 
         Parameters
@@ -242,117 +265,119 @@
                 battery.name,
                 battery.properties,
             )
         logging.info(
             "[+] Batteries from file %s loaded", path_to_batteries_file
         )
 
-    def write_value_direct(
-        self, worksheet: str, range: str, value: any
+    def _write_value_direct(
+        self, worksheet: str, cell_range: str, value: any
     ) -> None:
         """Write value in BatPaC Excel tool
 
         Write a value directly in the BatPaC Excel tool.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
-        range : str
+        cell_range : str
             Cell range of the BatPaC Excel tool.
         value : any
             Value to write in the BatPaC Excel tool.
         """
-        self.wb.sheets[worksheet][range].value = value
+        self.workbook.sheets[worksheet][cell_range].value = value
 
-    def read_value_direct(self, worksheet: str, range: str) -> any:
+    def _read_value_direct(self, worksheet: str, cell_range: str) -> any:
         """Read value from BatPaC Excel tool
 
         Read a value directly from the BatPaC Excel tool.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
-        range : str
+        cell_range : str
             Cell range of the BatPaC Excel tool.
 
         Returns
         -------
         any
             Value of the BatPaC Excel tool cell.
 
         Raises
         ------
         KeyError
             Raises KeyError if the specified worksheet or range could not be
             found.
         """
         try:
-            value = self.wb.sheets[worksheet][range].value
+            value = self.workbook.sheets[worksheet][cell_range].value
             return value
         except BaseException as error:
             logging.error("An exception occurred: %s", error)
-            logging.warning("[!] Key %s , %s not found", worksheet, range)
-            raise KeyError
+            logging.warning("[!] Key %s , %s not found", worksheet, cell_range)
+            raise KeyError from error
 
-    def wb_helper_range(
+    def _wb_helper_range(
         self,
         worksheet: str,
         name: str,
         battery: BatpacBattery = None,
-        additional_cell_config: Path | dict = None,
+        additional_cell_config: Path | dict | str = None,
     ) -> str:
         """Helper function for workbook range
 
         Function to find the cell range of a specified cell description.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         battery : BatPaC_battery, optional
             BatPaC_battery object, if the returned cell is battery specific, by
             default None.
-        additional_cell_config : Path | dict, optional
-            Path to TOML file or dictionary, which contains additional cell
-            configuration to consider, by default None.
+        additional_cell_config : Path | dict | str, optional
+            Path to TOML file or dictionary or str (default dataset), which
+            contains additional cell configuration to consider,
+            by default None.
 
         Returns
         -------
         str
             Excel cell range.
 
         Raises
         ------
         KeyError
             Raises KeyError, if worksheet name or cell description could not be
             found.
         """
         try:
             if additional_cell_config is not None:
-                if type(additional_cell_config) is Path:
-                    additional_cell_config = toml.load(additional_cell_config)
-                range_dict = additional_cell_config
+                if isinstance(additional_cell_config, dict):
+                    range_dict = additional_cell_config
+                else:
+                    range_dict = self.load_user_file(additional_cell_config)
             else:
                 range_dict = self.excel_cells
 
             if battery is None:
-                range = range_dict[worksheet][name]
+                cell_range = range_dict[worksheet][name]
             else:
-                range = range_dict[worksheet][
+                cell_range = range_dict[worksheet][
                     "Battery " + str(self.batteries.index(battery) + 1)
                 ][name]
-            return range
+            return cell_range
         except BaseException as error:
             logging.error("An exception occurred: %s", error)
             logging.warning("[!] Key %s , %s not found", worksheet, name)
-            raise KeyError
+            raise KeyError from error
 
     def write_value(self, worksheet: str, name: str, value: any) -> None:
         """Write value in BatPaC Excel tool
 
         Write value in BatPaC Excel tool without input the exact cell range.
 
         Parameters
@@ -360,66 +385,67 @@
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         value : any
             Value to write in the BatPaC Excel tool.
         """
-        self.write_value_direct(
-            worksheet, self.wb_helper_range(worksheet, name), value
+        self._write_value_direct(
+            worksheet, self._wb_helper_range(worksheet, name), value
         )
         logging.debug(
             "[ ] Write in %s %s (%s) = %s",
             worksheet,
-            self.wb_helper_range(worksheet, name),
+            self._wb_helper_range(worksheet, name),
             name,
             value,
         )
 
     def read_value(
         self,
         worksheet: str,
         name: str,
-        additional_cell_config: Path | dict = None,
+        additional_cell_config: Path | dict | str = None,
     ) -> any:
         """Read value from BatPaC Excel tool
 
         Read value from BatPaC Excel tool without input the exact cell range.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
-        additional_cell_config : Path | dict, optional
-            Path to TOML file or dictionary, which contains additional cell
-            configuration to consider, by default None.
+        additional_cell_config : Path | dict | str, optional
+            Path to TOML file or dictionary or string (default dataset), which
+            contains additional cell configuration to consider,
+            by default None.
 
         Returns
         -------
         any
             Value of the BatPaC Excel tool cell.
         """
-        return self.read_value_direct(
+        return self._read_value_direct(
             worksheet,
-            self.wb_helper_range(
+            self._wb_helper_range(
                 worksheet,
                 name,
                 battery=None,
                 additional_cell_config=additional_cell_config,
             ),
         )
 
     def read_value_battery(
         self,
         worksheet: str,
         name: str,
         battery: BatpacBattery,
-        additional_cell_config: Path | dict = None,
+        additional_cell_config: Path | dict | str = None,
     ) -> any:
         """Read battery specific value from BatPaC Excel tool
 
         Read battery specific value from BatPaC Excel tool without input the
         exact cell range.
 
         Parameters
@@ -428,25 +454,26 @@
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
         battery : BatPaC_battery
             BatPaC_battery object, if the returned cell is battery specific, by
             default None.
         additional_cell_config : Path | dict, optional
-            Path to TOML file or dictionary, which contains additional cell
-            configuration to consider, by default None.
+            Path to TOML file or dictionary or string (default dataset), which
+            contains additional cell configuration to consider,
+            by default None.
 
         Returns
         -------
         any
             Value of the BatPaC Excel tool cell.
         """
-        return self.read_value_direct(
+        return self._read_value_direct(
             worksheet,
-            self.wb_helper_range(
+            self._wb_helper_range(
                 worksheet, name, battery, additional_cell_config
             ),
         )
 
     def write_value_battery(
         self, worksheet: str, name: str, battery: BatpacBattery, value: any
     ) -> None:
@@ -463,158 +490,174 @@
             Name of the BatPaC Excel cell description.
         battery : BatPaC_battery
             BatPaC_battery object, if the returned cell is battery specific,
             by default None.
         value : any
             Value to write in the BatPaC Excel tool.
         """
-        self.write_value_direct(
-            worksheet, self.wb_helper_range(worksheet, name, battery), value
+        self._write_value_direct(
+            worksheet, self._wb_helper_range(worksheet, name, battery), value
         )
         logging.debug(
             "[ ] Write for %s in %s %s (%s) = %s",
             battery.name,
             worksheet,
-            self.wb_helper_range(worksheet, name, battery),
+            self._wb_helper_range(worksheet, name, battery),
             name,
             value,
         )
 
     def stop_automatic_calculation(self) -> None:
         """Stop automatic Excel calculation
         Stop the automatic Excel and BatPaC calculation.
         """
         self.write_value("Dashboard", "Restart (0/1)", 0)
-        self.wb.app.calculation = "manual"
-        self.wb.app.screen_updating = False
+        self.workbook.app.calculation = "manual"
+        self.workbook.app.screen_updating = False
 
     def start_automatic_calculation(self) -> None:
         """Start automatic Excel calculation
         Start the automatic Excel and BatPaC calculation.
         """
-        reset_macro = self.wb.macro("Module1.Reset")
+        reset_macro = self.workbook.macro("Module1.Reset")
         reset_macro()
-        self.wb.app.calculation = "automatic"
-        self.wb.app.screen_updating = True
+        self.workbook.app.calculation = "automatic"
+        self.workbook.app.screen_updating = True
 
-    def read_from_user_input(self, user_read_file: Path) -> dict:
+    def read_from_user_input(self, user_read_file: Path | str) -> dict:
         """Read user specified input from BatPaC Excel tool
 
         Read additional cell values from BatPaC Excel tool specified by user
         input.
 
         Parameters
         ----------
-        user_read_file : Path
-            Path to the TOML file containing additional cell ranges from which
-            values are to be read.
+        user_read_file : Path | str
+            Path to the TOML file or string (default dataset) containing
+            additional cell ranges from which values are to be read.
 
         Returns
         -------
         dict
             Dictionary in the format {"sheet" : {"name" : value} }
-
-        Raises
-        ------
-        ValueError
-            Raises ValueError, if the user input is not valid.
         """
-        warnings.warn("This function is not implemented.")
-        if user_read_file.is_file():
-            return True
-        logging.warning("[!] %s is not a valid file", user_read_file)
-        raise ValueError(f"{user_read_file} is not a valid file")
+
+        additional_cells = self.load_user_file(user_read_file)
+        values_dict = additional_cells
+        for sheet_name, sheet_key in additional_cells.items():
+            for batpac_key, batpac_cell_range in sheet_key.items():
+                if isinstance(batpac_cell_range, dict):
+                    for (
+                        battery_key,
+                        battery_cell_range,
+                    ) in batpac_cell_range.items():
+                        values_dict[sheet_name][batpac_key][
+                            battery_key
+                        ] = self._read_value_direct(
+                            sheet_name, battery_cell_range
+                        )
+                else:
+                    values_dict[sheet_name][
+                        batpac_key
+                    ] = self._read_value_direct(sheet_name, batpac_cell_range)
+
+        return values_dict
 
     def read_calculation_and_validation_results(
-        self, toml_file_calculation_validation_results: Path = None
-    ) -> dict | bool:
+        self, toml_file_calculation_validation_results: Path | str = None
+    ) -> dict:
         """Read calculation and validation results
 
         Read the calculation and validation results from the BatPaC Excel tool.
 
         Parameters
         ----------
-        toml_file_calculation_validation_results : Path, optional
-            Path to the TOML file containing the specified cell ranges of the
-            calculation and validation results, by default None.
+        toml_file_calculation_validation_results : Path | str, optional
+            Path to the TOML file or string (default dataset), containing the
+            specified cell ranges of the calculation and validation results,
+            by default None.
 
         Returns
         -------
-        dict | bool
-            Returns a dictionary if a TOML file is specified, otherwise False.
+        dict
+            Returns a dictionary of the calculation and validation results.
+
+        Raises
+        ------
+        KeyError
+            If no configuration for calculation and validation found.
         """
+
         if toml_file_calculation_validation_results is None:
-            if self.toml_calculation_validation_results_path is None:
+            if self.toml_calculation_validation_results is None:
                 logging.warning(
-                    "[!] No toml file for calculation and validation found"
+                    "[!] No toml file for calculation and validation found."
+                )
+                raise KeyError(
+                    "No configuration for calculation and validation found."
                 )
-                return False
         else:
-            self.toml_calculation_validation_results_path = (
+            self.toml_calculation_validation_results = self.load_user_file(
                 toml_file_calculation_validation_results
             )
 
-        additional_cell_config = toml.load(
-            self.toml_calculation_validation_results_path
-        )
-
         config_errors = ["Configuration Errors (see table to right)"]
         config_warnings = ["Configuration Warnings (see table  to right)"]
         plant_size = ["Plant Size, GWh"]
         power_to_energy = ["Power-to-energy ratio"]
         adequacy_cooling = ["Adequacy of cooling"]
         cathode_thickness = ["Cathode thickness limited by"]
         table_columns = ["Parameter"]
         for battery in self.batteries:
             config_errors.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Configuration Errors (see table to right)",
                     battery,
-                    additional_cell_config,
+                    self.toml_calculation_validation_results,
                 )
             )
             config_warnings.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Configuration Warnings (see table  to right)",
                     battery,
-                    additional_cell_config,
+                    self.toml_calculation_validation_results,
                 )
             )
             plant_size.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Plant Size, GWh",
                     battery,
-                    additional_cell_config,
+                    self.toml_calculation_validation_results,
                 )
             )
             power_to_energy.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Power-to-energy ratio",
                     battery,
-                    additional_cell_config,
+                    self.toml_calculation_validation_results,
                 )
             )
             adequacy_cooling.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Adequacy of cooling",
                     battery,
-                    additional_cell_config,
+                    self.toml_calculation_validation_results,
                 )
             )
             cathode_thickness.append(
                 self.read_value_battery(
                     "Dashboard",
                     "Cathode thickness limited by",
                     battery,
-                    additional_cell_config,
+                    self.toml_calculation_validation_results,
                 )
             )
             table_columns.append(battery.name)
 
         table = [
             table_columns,
             config_errors,
@@ -692,97 +735,130 @@
         ----------
         path : Path, optional
             If the path is specified, the BatPaC Excel tool will be saved under
             the path, by default None will overwrite the current BatPaC Excel
             tool.
         """
         logging.info("[ ] Save workbook")
-        if path is None:
-            path = self.workbook_path
-        self.wb.save(path)
-        self.wb = xw.Book(path)
-        self.app = self.wb.app
+        self.workbook.save(path)
+        self.workbook = xw.Book(path)
+        # self.app = self.workbook.app
         logging.info("[+] Saved workbook in %s", path)
 
     def close(self) -> bool:
         """Close BatPaC Excel tool
 
         Close the BatPaC Excel tool if other workbooks are open, otherwise the
         Excel instance will be closed.
 
         Returns
         -------
         bool
             True, if BatPaC Excel tool is closed.
         """
-        if len(self.wb.app.books) == 1:
-            self.wb.app.quit()
+        if len(self.workbook.app.books) == 1:
+            self.workbook.app.quit()
             logging.info("[+] Workbook and Excel closed")
             return True
-        self.wb.close()
+        self.workbook.close()
         logging.info("[+] Workbook closed")
         return True
 
-    def save_config(
-        self, batpac_path: Path = None, battery_path: Path = None
-    ) -> None:
+    def _save_batpac_config(self, batpac_path: Path = None) -> None:
         """Save BatPaC_tool configuration
 
-        Read all BatPaC_tool properties and its included [BatPaC_battery]
-        properties from the BatPaC Excel tool, save these properties in the
-        BatPaC_tool and [BatPaC_battery] objects, and write them as TOML file.
+        Read all BatPaC_tool properties from the BatPaC Excel tool, save
+        these properties in the BatPaC_tool object, and write them as TOML
+        file.
 
         Parameters
         ----------
         batpac_path : Path, optional
             If specified, storage path to the TOML file for BatPaC_tool
             properties, by default None.
-        battery_path : Path, optional
-            If specified, storage path to the TOML file for [BatPaC_battery]
-            properties, by default None.
         """
         for sheet in self.excel_cells:
             for key, value in self.excel_cells[sheet].items():
                 if isinstance(value, dict):
-                    battery_number = int(key.replace("Battery ", "")) - 1
-                    for battery_key, battery_value_range in value.items():
-                        self.batteries[battery_number].set_new_property(
-                            sheet,
-                            battery_key,
-                            self.read_value_direct(sheet, battery_value_range),
-                        )
-                else:
-                    self.set_new_property(
-                        sheet, key, self.read_value(sheet, key)
-                    )
+                    continue
+                self.set_new_property(sheet, key, self.read_value(sheet, key))
 
         if batpac_path is not None:
-            with open(batpac_path, "w") as toml_file:
+            with open(batpac_path, "w", encoding="utf-8") as toml_file:
                 for sheet in tqdm(
                     self.properties, "Saving BatPaC config from each sheet"
                 ):
                     toml_file.write(f'["{sheet}"]\n')
                     for key, value in self.properties[sheet].items():
                         if value is None or key == "Restart (0/1)":
                             toml_file.write("# ")
                         if isinstance(value, str):
                             toml_file.write(f"'{key}' = '{value}'\n")
                         else:
                             toml_file.write(f"'{key}' = {value}\n")
                     toml_file.write("\n")
 
+    def _save_battery_config(self, battery_path: Path = None) -> None:
+        """Save [BatPaC_battery] configuration
+
+        Read all BatPaC_tool included [BatPaC_battery] properties from the
+        BatPaC Excel tool, save these properties in the [BatPaC_battery]
+        objects, and write them as TOML file.
+
+        Parameters
+        ----------
+        battery_path : Path, optional
+            If specified, storage path to the TOML file for [BatPaC_battery]
+            properties, by default None.
+        """
+        for sheet in self.excel_cells:
+            for key, value in self.excel_cells[sheet].items():
+                if isinstance(value, dict):
+                    battery_number = int(key.replace("Battery ", "")) - 1
+                    for battery_key, battery_value_range in value.items():
+                        self.batteries[battery_number].set_new_property(
+                            sheet,
+                            battery_key,
+                            self._read_value_direct(
+                                sheet, battery_value_range
+                            ),
+                        )
+                else:
+                    continue
+
         if battery_path is not None:
-            with open(battery_path, "w") as toml_file:
+            with open(battery_path, "w", encoding="utf-8") as toml_file:
                 for battery in tqdm(
                     self.batteries,
                     "Saving battery configuration for each battery",
                 ):
                     for sheet in battery.properties:
                         toml_file.write(f'["{battery.name}"."{sheet}"]\n')
                         for key, value in battery.properties[sheet].items():
                             if value is None:
                                 toml_file.write("# ")
                             if isinstance(value, str):
                                 toml_file.write(f"'{key}' = '{value}'\n")
                             else:
                                 toml_file.write(f"'{key}' = {value}\n")
                     toml_file.write("\n")
+
+    def save_config(
+        self, batpac_path: Path = None, battery_path: Path = None
+    ) -> None:
+        """Save BatPaC_tool configuration
+
+        Read all BatPaC_tool properties and its included [BatPaC_battery]
+        properties from the BatPaC Excel tool, save these properties in the
+        BatPaC_tool and [BatPaC_battery] objects, and write them as TOML file.
+
+        Parameters
+        ----------
+        batpac_path : Path, optional
+            If specified, storage path to the TOML file for BatPaC_tool
+            properties, by default None.
+        battery_path : Path, optional
+            If specified, storage path to the TOML file for [BatPaC_battery]
+            properties, by default None.
+        """
+        self._save_batpac_config(batpac_path)
+        self._save_battery_config(battery_path)
```

### Comparing `batpy-0.0.9/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.9/src/batpy/data/batpy_batpac_config.toml` & `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+["batpy"]
+"BatPaC version" = "BatPaC 5.0 2022-07-22"
+"BatPaC SemVer" = "0.0.0"
+
 ["Dashboard"]
 'Electrode Couple' = 'NMC811-G (Energy)'
 'Positive active material specific capacity, mAh/g' = 200.0
 'Void volume fraction, % of positive electrode' = 20.0
 'Positive foil thickness, mm' = 10.0
 'Maximum positive electrode thickness, µm' = 110.0
 # 'Restart (0/1)' = 1.0
```

### Comparing `batpy-0.0.9/src/batpy/data/batpy_batpac_user_input_cells.toml` & `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.9/src/batpy/data/batpy_batteries_config.toml` & `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batteries_config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+["batpy"]
+"BatPaC version" = "BatPaC 5.0 2022-07-22"
+"BatPaC SemVer" = "0.0.0"
+
 ["Battery 1"."Dashboard"]
 'Number of modules in parallel' = 10000.0
 'Target rated peak power of pack, kW' = 100.0
 'Duration at rated power, s' = 10.0
 'Override duration at rated peak power, s' = 2.0
 'Operating initial SOC for rated peak power, %' = 20.0
 'Override for operating initial SOC for rated peak power, %' = 1.0
```

### Comparing `batpy-0.0.9/src/batpy/is_version_compatible.py` & `batpy-0.1.0/src/batpy/is_version_compatible.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 # -*- coding: UTF-8 -*-
 """Module, which includes the function is_version_compatible
 """
 import logging
 
 import semantic_version
 
-logger = logging.getLogger(__name__)
-logging.basicConfig(
-    format="%(asctime)s [%(levelname)s]: \t%(filename)s\t%(funcName)s\t\
-        %(lineno)s\t- %(message)s",
-    filename="batpy.log",
-    filemode="w",
-    level=logging.INFO,
-)
-
 
 def is_version_compatible(
     self_version: semantic_version.Version,
     version_to_check: semantic_version.Version,
     include_minor: bool = False,
 ) -> bool:
     """Check for version compatibility
```

### Comparing `batpy-0.0.9/PKG-INFO` & `batpy-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: batpy
-Version: 0.0.9
+Version: 0.1.0
 Summary: A python package to read, write, and calculate batteries in the BatPaC tool.
 Home-page: https://github.com/rginster/batpy
 License: MIT
 Author: Raphael Ginster
 Author-email: r.ginster@tu-braunschweig.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: prettytable (>=3.7.0,<4.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
@@ -21,14 +20,15 @@
 Project-URL: Documentation, https://rginster.github.io/batpy/
 Project-URL: Repository, https://github.com/rginster/batpy
 Description-Content-Type: text/markdown
 
 [![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
 [![Docs](https://github.com/rginster/batpy/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/documentation.yaml)
 [![pages-build-deployment](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment)
+[![codecov](https://codecov.io/gh/rginster/batpy/branch/main/graph/badge.svg?token=JH8L3B14AW)](https://codecov.io/gh/rginster/batpy)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/batpy)
 [![PyPi](https://img.shields.io/pypi/v/batpy.svg)](https://pypi.python.org/pypi/batpy)
 [![PyPi](https://img.shields.io/pypi/dm/batpy.svg)](https://pypi.python.org/pypi/batpy)
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
@@ -49,26 +49,50 @@
 `batpy` is able to read, write, and calculate batteries in the [BatPaC tool](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 
 
 ```python
 from batpy.batpac_battery import BatpacBattery
 from batpy.batpac_tool import BatpacTool
+from batpy import batpac_datasets
 
-# Constants
+# Paths to TOML configurations on local system
 BATPY_BATPAC_EXCEL = "./BatPaC 5.0 2022-07-22.xlsm"
 
 BATPY_BATPAC_BATTERY_CONFIG = "./batpy_batteries_config.toml"
-BATPY_BATPAC_USER_INPUT_CONFIG = "./batpy_batpac_user_input_cells.toml"
+BATPY_BATPAC_USER_INPUT_CONFIG = (
+    "./batpy_batpac_user_input_cells.toml"
+)
 BATPY_BATPAC_TOOL_CONFIG = "./batpy_batpac_config.toml"
 
 BATPY_BATPAC_TOOL_CALCULATION_VALIDATION_CONFIG = (
     "./batpy_batpac_calculation_and_validation_results.toml"
 )
 
+ADDITIONAL_USER_DEFINED_RESULTS_CELLS = (
+    "./batpy_batpac_summary_of_results.toml"
+)
+
+# Get included datasets
+# Show available versions
+batpac_datasets.get_available_batpy_dataset_versions()
+
+# Show latest version
+batpac_datasets.get_latest_batpy_dataset_version()
+
+
+# Show available dataset of specified version (default latest)
+batpac_datasets.get_available_batpy_dataset_names()
+
+
+# Load included dataset:
+batpy_batpac_battery_design = batpac_datasets.get_batpy_dataset(
+    "batpy_batpac_battery_design", "0.1.0"
+)
+
 
 # Create batteries
 bat1 = BatpacBattery("Battery 1")
 bat2 = BatpacBattery("Battery 2")
 bat3 = BatpacBattery("Battery 3")
 bat4 = BatpacBattery("Battery 4")
 bat5 = BatpacBattery("Battery 5")
@@ -77,15 +101,15 @@
 
 # Change battery properties
 # a) Write individual properties for created batteries
 bat1.set_new_property("Dashboard", "Number of modules in parallel", 10)
 
 # b) Load individiual battery configuration from file
 bat2.load_battery_file(
-    "./battery_config.toml", "Battery"
+    BATPY_BATPAC_BATTERY_CONFIG, "Battery 2"
 )
 
 # Create BatPaC instance
 battery_calculation = BatpacTool(
     BATPY_BATPAC_EXCEL,
     BATPY_BATPAC_USER_INPUT_CONFIG,
     BATPY_BATPAC_TOOL_CALCULATION_VALIDATION_CONFIG,
@@ -123,14 +147,29 @@
 # Load configuration file for BatPaC instance
 battery_calculation.load_batpac_file(BATPY_BATPAC_TOOL_CONFIG)
 
 # Write configuration in Excel file and calculate batteries
 battery_calculation.calculate()
 battery_calculation.read_calculation_and_validation_results()
 
+# Read additional user defined cells
+# a) From file path
+user_results = battery_calculation.read_from_user_input(
+    ADDITIONAL_USER_DEFINED_RESULTS_CELLS
+)
+print(user_results)
+print(user_results["Summary of Results"]["Battery 1"])
+
+# b) From included configuration
+user_results_included_configuration = battery_calculation.read_from_user_input(
+    batpy_batpac_battery_design
+)
+print(user_results_included_configuration)
+print(user_results_included_configuration["Battery Design"]["Battery 1"])
+
 # Save configuration from Excel:
 battery_calculation.save_config(
     batpac_path="./saved_batpac_config.toml",
     battery_path="./saved_batteries_config.toml",
 )
 
 # Save Excel file
```

