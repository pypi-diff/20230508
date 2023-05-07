# Comparing `tmp/pyproject-generator-0.2.2.tar.gz` & `tmp/pyproject-generator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.2.2.tar", last modified: Fri May  5 12:52:50 2023, max compression
+gzip compressed data, was "pyproject-generator-0.2.3.tar", last modified: Sun May  7 22:37:15 2023, max compression
```

## Comparing `pyproject-generator-0.2.2.tar` & `pyproject-generator-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.893064 pyproject-generator-0.2.2/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.2.2/LICENSE
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3920 2023-05-05 12:52:50.893353 pyproject-generator-0.2.2/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3379 2023-05-05 12:46:17.000000 pyproject-generator-0.2.2/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.2.2/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 12:52:50.894321 pyproject-generator-0.2.2/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.867921 pyproject-generator-0.2.2/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.874713 pyproject-generator-0.2.2/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.2.2/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 12:52:44.000000 pyproject-generator-0.2.2/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:42:30.000000 pyproject-generator-0.2.2/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.875391 pyproject-generator-0.2.2/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      315 2023-05-05 03:34:04.000000 pyproject-generator-0.2.2/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.2.2/src/pyproject/licenses.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-05-05 12:40:42.000000 pyproject-generator-0.2.2/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15276 2023-05-05 12:49:16.000000 pyproject-generator-0.2.2/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-05 02:42:30.000000 pyproject-generator-0.2.2/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.887199 pyproject-generator-0.2.2/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.2.2/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.2.2/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.2.2/src/pyproject/templates/license_bsd3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.2.2/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.2.2/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.2.2/src/pyproject/templates/pre_commit_config.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.2.2/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.2.2/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      603 2023-05-05 12:52:13.000000 pyproject-generator-0.2.2/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.2.2/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.2.2/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.891750 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3920 2023-05-05 12:52:50.000000 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1054 2023-05-05 12:52:50.000000 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 12:52:50.000000 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 12:52:50.000000 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 12:52:50.000000 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 12:52:50.000000 pyproject-generator-0.2.2/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:52:50.892656 pyproject-generator-0.2.2/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:42:30.000000 pyproject-generator-0.2.2/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.403766 pyproject-generator-0.2.3/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.2.3/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4200 2023-05-07 22:37:15.404135 pyproject-generator-0.2.3/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3659 2023-05-06 14:06:08.000000 pyproject-generator-0.2.3/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.2.3/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-07 22:37:15.405511 pyproject-generator-0.2.3/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.370496 pyproject-generator-0.2.3/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.379989 pyproject-generator-0.2.3/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.2.3/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-07 22:37:10.000000 pyproject-generator-0.2.3/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4070 2023-05-06 12:36:27.000000 pyproject-generator-0.2.3/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.382112 pyproject-generator-0.2.3/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      337 2023-05-05 15:13:27.000000 pyproject-generator-0.2.3/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.2.3/src/pyproject/licenses.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-05-05 12:40:42.000000 pyproject-generator-0.2.3/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    16834 2023-05-07 22:02:11.000000 pyproject-generator-0.2.3/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2851 2023-05-06 22:21:55.000000 pyproject-generator-0.2.3/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.397328 pyproject-generator-0.2.3/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.2.3/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.2.3/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.2.3/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.2.3/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      603 2023-05-05 12:52:13.000000 pyproject-generator-0.2.3/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.2.3/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.2.3/src/pyproject/templates/tox.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      189 2023-05-05 20:21:04.000000 pyproject-generator-0.2.3/src/pyproject/utils.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.400538 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4200 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1095 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.402686 pyproject-generator-0.2.3/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      303 2023-05-06 12:39:33.000000 pyproject-generator-0.2.3/tests/test_cli.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1802 2023-05-06 12:35:08.000000 pyproject-generator-0.2.3/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.2.2/LICENSE` & `pyproject-generator-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/PKG-INFO` & `pyproject-generator-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.2.2
+Version: 0.2.3
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,16 @@
 [![PyPI version](https://badge.fury.io/py/pyproject-generator.svg)](https://badge.fury.io/py/pyproject-generator)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyproject)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+![Tests](https://github.com/CangyuanLi/pyproject/actions/workflows/tests.yaml/badge.svg)
+![Coverage](https://github.com/CangyuanLi/pyproject/blob/master/assets/coverage.svg)
 
 
 ## What is it?
 
 **pyproject** is a command line utility to setup and distribute Python packages.
 
 # Usage:
@@ -51,15 +53,15 @@
 ```sh
 pyproject init {project_name}
 ```
 
 to create your project folder. It will automatically setup a package structure, virtual
 environment, and install packages.
 
-![](demo.gif)
+![](https://raw.githubusercontent.com/CangyuanLi/pyproject/master/assets/demo.gif)
 
 The final project structure looks like
 
 ```sh
 ├── .git
 ├── .github
 │   └── workflows
@@ -72,14 +74,15 @@
 │   └── benchmark.py
 ├── pyproject.toml
 ├── requirements_dev.txt
 ├── setup.cfg
 ├── src
 │   └── myproject
 │       ├── __init__.py
+│       ├── __version__.py
 │       └── py.typed
 ├── tests
 │   └── test_myproject.py
 └── tox.ini
 ```
 
 ## Configuring pyproject-generator
```

### Comparing `pyproject-generator-0.2.2/README.md` & `pyproject-generator-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 [![PyPI version](https://badge.fury.io/py/pyproject-generator.svg)](https://badge.fury.io/py/pyproject-generator)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyproject)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+![Tests](https://github.com/CangyuanLi/pyproject/actions/workflows/tests.yaml/badge.svg)
+![Coverage](https://github.com/CangyuanLi/pyproject/blob/master/assets/coverage.svg)
 
 
 ## What is it?
 
 **pyproject** is a command line utility to setup and distribute Python packages.
 
 # Usage:
@@ -35,15 +37,15 @@
 ```sh
 pyproject init {project_name}
 ```
 
 to create your project folder. It will automatically setup a package structure, virtual
 environment, and install packages.
 
-![](demo.gif)
+![](https://raw.githubusercontent.com/CangyuanLi/pyproject/master/assets/demo.gif)
 
 The final project structure looks like
 
 ```sh
 ├── .git
 ├── .github
 │   └── workflows
@@ -56,14 +58,15 @@
 │   └── benchmark.py
 ├── pyproject.toml
 ├── requirements_dev.txt
 ├── setup.cfg
 ├── src
 │   └── myproject
 │       ├── __init__.py
+│       ├── __version__.py
 │       └── py.typed
 ├── tests
 │   └── test_myproject.py
 └── tox.ini
 ```
 
 ## Configuring pyproject-generator
```

### Comparing `pyproject-generator-0.2.2/setup.cfg` & `pyproject-generator-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/cli.py` & `pyproject-generator-0.2.3/src/pyproject/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,34 +80,38 @@
         version="%(prog)s {version}".format(version=__version__),
         help="Displays package version",
     )
 
     return parser
 
 
+def _validate_input(args, logger: Logger):
+    if args.action not in ACTIONS:
+        logger.error(f"Invalid choice `{args.action}`, choose from {ACTIONS}")
+
+    if args.action == "init" and args.project_name is None:
+        logger.error("Action `init` requires project name")
+
+    if args.license not in LICENSES and args.license is not None:
+        logger.error(f"Invalid choice `{args.license}`, choose from {ALLOWED_LICENSES}")
+
+
 def main():
     parser = get_parser()
     args = parser.parse_args()
 
     options = {"quiet": args.quiet}
 
     # set up the console for logging
     logging_level = Level.INFO
     if options["quiet"]:
         logging_level = Level.ERROR
     logger = Logger(logging_level)
 
-    if args.action not in ACTIONS:
-        logger.error(f"Invalid choice `{args.action}`, choose from {ACTIONS}")
-
-    if args.action == "init" and args.project_name is None:
-        logger.error("Action `init` requires project name")
-
-    if args.license not in LICENSES and args.license is not None:
-        logger.error(f"Invalid choice `{args.license}`, choose from {ALLOWED_LICENSES}")
+    _validate_input(args, logger)
 
     config = {
         "pypi_username": args.pypi_username,
         "pypi_password": args.pypi_password,
         "github_url": args.github_url,
         "author": args.author,
         "email": args.email,
```

### Comparing `pyproject-generator-0.2.2/src/pyproject/licenses.py` & `pyproject-generator-0.2.3/src/pyproject/licenses.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/logger.py` & `pyproject-generator-0.2.3/src/pyproject/logger.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/project_builder.py` & `pyproject-generator-0.2.3/src/pyproject/project_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Literal, Optional, Union
 
 import platformdirs
 from rich.panel import Panel
 
 from .licenses import LICENSES, License
 from .logger import Logger
+from .utils import squash_collection
 
 # Globals
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
 USER_CONFIG_PATH = platformdirs.user_config_dir(
     appname="pyproject-generator", appauthor="cangyuanli"
@@ -264,15 +265,15 @@
         license = self._config.license.short_name
         (proj_path / "LICENSE").write_text(templates[f"license_{license}"])
 
     @staticmethod
     def _init_github_actions(proj_path, templates: dict):
         workflows_path = proj_path / ".github/workflows"
         workflows_path.mkdir(parents=True)
-        (workflows_path / "tests.yml").write_text(templates["tests"])
+        (workflows_path / "tests.yaml").write_text(templates["tests"])
 
     def init_project(self, project_name: str):
         """Called when user specifies `action = init`.
 
         Args:
             project_name (str): User-supplied name of project
         """
@@ -351,43 +352,69 @@
                 ["python", "-m", "pip", "install", "-U", "pip"],
                 stdout=subprocess.DEVNULL,
             ),
             text="pip",
             clear=False,
         )
 
+        not_installed = []
         for dep in sorted(list(self._config.dependencies)):
-            self._logger.spinner(
-                lambda: venv_builder.run_bin(
-                    ["pip", "install", dep], stdout=subprocess.DEVNULL
-                ),
-                text=dep,
-                clear=False,
+            try:
+                self._logger.spinner(
+                    lambda: venv_builder.run_bin(
+                        ["pip", "install", dep],
+                        stdout=subprocess.DEVNULL,
+                        stderr=subprocess.DEVNULL,
+                    ),
+                    text=dep,
+                    clear=False,
+                )
+            except subprocess.CalledProcessError:
+                not_installed.append(dep)
+
+        if len(not_installed) > 0:
+            self._logger.warning(
+                f"Failed to install {squash_collection(not_installed)}"
             )
 
         self._logger.info(Panel("Finalizing project..."), justify="left")
 
         # Create requirements_dev file
         def _create_req_file():
             reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
             (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
         self._logger.spinner(
             _create_req_file,
             "Creating requirements_dev.txt",
         )
 
-        # Ensure pre-commit is up to date
-        self._logger.spinner(
-            lambda: venv_builder.run_bin(
-                ["pre-commit", "autoupdate"], cwd=proj_path, stdout=subprocess.DEVNULL
-            ),
-            "Ensuring pre-commit config is up to date",
-            clear=True,
-        )
+        if (
+            "pre-commit" in self._config.dependencies
+            and "pre-commit" not in not_installed
+        ):
+            # Ensure pre-commit is up to date
+            self._logger.spinner(
+                lambda: venv_builder.run_bin(
+                    ["pre-commit", "autoupdate"],
+                    cwd=proj_path,
+                    stdout=subprocess.DEVNULL,
+                ),
+                "Ensuring pre-commit config is up to date",
+                clear=True,
+            )
+
+            # Install pre-commit hooks
+            self._logger.spinner(
+                lambda: venv_builder.run_bin(
+                    ["pre-commit", "install"], cwd=proj_path, stdout=subprocess.DEVNULL
+                ),
+                "Installing pre-commit hooks",
+                clear=True,
+            )
 
         self._logger.info(f"Done setting up {project_name}!", style="green")
 
     def _parse_config_file(self, filename: PathLike) -> Config:
         if filename == "default_config.json":
             path = BASE_PATH / "config/default_config.json"
         elif filename == "config.json":
@@ -450,30 +477,53 @@
         """Discover the virtual environment and upload project to PyPI."""
         username = self._config.pypi_username
         password = self._config.pypi_password
 
         env = Env()
 
         # python -m build generates a dist folder, remove this in preparation
-        shutil.rmtree(self.proj_path / "dist", ignore_errors=True)
+        self._logger.spinner(
+            lambda: shutil.rmtree(self.proj_path / "dist", ignore_errors=True),
+            "Removing existing build",
+            prefix="",
+            clear=False,
+        )
 
-        env.run_bin(["python", "-m", "build"])
-        env.run_bin(["twine", "check", "dist/*"])
+        self._logger.spinner(
+            lambda: env.run_bin(["python", "-m", "build"], stdout=subprocess.DEVNULL),
+            "Building project",
+            prefix="",
+            clear=False,
+        )
+        self._logger.spinner(
+            lambda: env.run_bin(
+                ["twine", "check", "dist/*"], stdout=subprocess.DEVNULL
+            ),
+            "Checking build",
+            prefix="",
+            clear=False,
+        )
 
         if username == "" and password == "":
             twine_args = []
         elif username == "" and password != "":
             twine_args = ["-p", password]
-            env.run_bin(["twine", "upload", "dist/*", "-p", password])
         elif username != "" and password == "":
             twine_args = ["-u", username]
         else:
             twine_args = ["-u", username, "-p", password]
 
-        env.run_bin(["twine", "upload", "dist/*"] + twine_args)
+        # Upload to pypi
+        self._logger.info("\n", end="")
+
+        # allow twine to use its own errors
+        try:
+            env.run_bin(["twine", "upload", "dist/*"] + twine_args)
+        except subprocess.CalledProcessError:
+            pass
 
     def dispatch(self, action: Action, **kwargs):
         if action == "init":
             self.init_project(**kwargs)
         elif action == "upload":
             self.upload()
         elif action == "config":
```

### Comparing `pyproject-generator-0.2.2/src/pyproject/spinner.py` & `pyproject-generator-0.2.3/src/pyproject/spinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional
 
 from rich.console import Console
 
 BACKSPACE = "\b"
 CLEAR_LINE = "\033[K"
 CHECKMARK = "[green]\u2713[/green]"
-XMARK = "[red]\u274C[/red]"
+XMARK = "[red]\u2717[/red]"
 
 
 class Spinner:
     def __init__(
         self,
         console: Console,
         text: str,
@@ -80,18 +80,23 @@
     def __enter__(self):
         if sys.stdout.isatty():  # if file stream is active
             self._screen_lock = threading.Lock()
             self.busy = True
             self.thread = threading.Thread(target=self.spinner_task)
             self.thread.start()
 
-    def __exit__(self, exception: Optional[BaseException], value, tb):
-        if exception is not None:
+    def __exit__(
+        self, exception_type: Optional[BaseException], exception_value, traceback
+    ):
+        end_mark = CHECKMARK
+
+        if exception_type is not None:
             end_mark = XMARK
-        else:
-            end_mark = CHECKMARK
 
         if sys.stdout.isatty():
             self.busy = False
             self.remove_spinner(end_mark, cleanup=True)
         else:
             sys.stdout.write("\r")
+
+        if exception_type is not None:
+            raise exception_value
```

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.2.3/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.2.3/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/license_bsd3.template` & `pyproject-generator-0.2.3/src/pyproject/templates/license_bsd3.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.2.3/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/pre_commit_config.template` & `pyproject-generator-0.2.3/src/pyproject/templates/pre_commit_config.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/readme.template` & `pyproject-generator-0.2.3/src/pyproject/templates/readme.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/setup.template` & `pyproject-generator-0.2.3/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject/templates/tests.template` & `pyproject-generator-0.2.3/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.2/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.2.3/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.2.2
+Version: 0.2.3
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,16 @@
 [![PyPI version](https://badge.fury.io/py/pyproject-generator.svg)](https://badge.fury.io/py/pyproject-generator)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyproject)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+![Tests](https://github.com/CangyuanLi/pyproject/actions/workflows/tests.yaml/badge.svg)
+![Coverage](https://github.com/CangyuanLi/pyproject/blob/master/assets/coverage.svg)
 
 
 ## What is it?
 
 **pyproject** is a command line utility to setup and distribute Python packages.
 
 # Usage:
@@ -51,15 +53,15 @@
 ```sh
 pyproject init {project_name}
 ```
 
 to create your project folder. It will automatically setup a package structure, virtual
 environment, and install packages.
 
-![](demo.gif)
+![](https://raw.githubusercontent.com/CangyuanLi/pyproject/master/assets/demo.gif)
 
 The final project structure looks like
 
 ```sh
 ├── .git
 ├── .github
 │   └── workflows
@@ -72,14 +74,15 @@
 │   └── benchmark.py
 ├── pyproject.toml
 ├── requirements_dev.txt
 ├── setup.cfg
 ├── src
 │   └── myproject
 │       ├── __init__.py
+│       ├── __version__.py
 │       └── py.typed
 ├── tests
 │   └── test_myproject.py
 └── tox.ini
 ```
 
 ## Configuring pyproject-generator
```

### Comparing `pyproject-generator-0.2.2/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.2.3/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
 src/pyproject/licenses.py
 src/pyproject/logger.py
 src/pyproject/project_builder.py
 src/pyproject/spinner.py
+src/pyproject/utils.py
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/license_apache.template
 src/pyproject/templates/license_bsd3.template
 src/pyproject/templates/license_gpl_v3.template
 src/pyproject/templates/license_mit.template
 src/pyproject/templates/pre_commit_config.template
@@ -23,8 +24,9 @@
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
 src/pyproject_generator.egg-info/SOURCES.txt
 src/pyproject_generator.egg-info/dependency_links.txt
 src/pyproject_generator.egg-info/entry_points.txt
 src/pyproject_generator.egg-info/requires.txt
 src/pyproject_generator.egg-info/top_level.txt
+tests/test_cli.py
 tests/test_pyproject.py
```

