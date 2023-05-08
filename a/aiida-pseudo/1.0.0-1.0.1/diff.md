# Comparing `tmp/aiida-pseudo-1.0.0.tar.gz` & `tmp/aiida-pseudo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-pseudo-1.0.0.tar", last modified: Wed Jan 25 13:23:48 2023, max compression
+gzip compressed data, was "aiida-pseudo-1.0.1.tar", last modified: Mon May  8 09:08:03 2023, max compression
```

## Comparing `aiida-pseudo-1.0.0.tar` & `aiida-pseudo-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1188 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/.gitignore
--rw-r--r--   0        0        0     1078 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      184 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    12298 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     8871 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/README.md
--rw-r--r--   0        0        0     3245 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/__init__.py
--rw-r--r--   0        0        0      250 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/__init__.py
--rw-r--r--   0        0        0     3848 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/family.py
--rw-r--r--   0        0        0    19531 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/install.py
--rw-r--r--   0        0        0     2226 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/list.py
--rw-r--r--   0        0        0      202 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/params/__init__.py
--rw-r--r--   0        0        0      370 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/params/arguments.py
--rw-r--r--   0        0        0     3635 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/params/options.py
--rw-r--r--   0        0        0     7303 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/params/types.py
--rw-r--r--   0        0        0     1031 2023-01-25 13:23:43.579676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/root.py
--rw-r--r--   0        0        0     2663 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/cli/utils.py
--rw-r--r--   0        0        0       60 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/common/__init__.py
--rw-r--r--   0        0        0      245 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/common/units.py
--rw-r--r--   0        0        0      105 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/__init__.py
--rw-r--r--   0        0        0      382 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/__init__.py
--rw-r--r--   0        0        0     2886 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/jthxml.py
--rw-r--r--   0        0        0     7954 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/pseudo.py
--rw-r--r--   0        0        0     2742 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/psf.py
--rw-r--r--   0        0        0     4519 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/psml.py
--rw-r--r--   0        0        0     3076 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/psp8.py
--rw-r--r--   0        0        0     4707 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/upf.py
--rw-r--r--   0        0        0     6686 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/vps.py
--rw-r--r--   0        0        0      102 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/__init__.py
--rw-r--r--   0        0        0      308 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/__init__.py
--rw-r--r--   0        0        0      545 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/cutoffs.py
--rw-r--r--   0        0        0    15544 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/pseudo.py
--rw-r--r--   0        0        0    18127 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/pseudo_dojo.py
--rw-r--r--   0        0        0     3973 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/sssp.py
--rw-r--r--   0        0        0      178 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/mixins/__init__.py
--rw-r--r--   0        0        0    14194 2023-01-25 13:23:43.583676 aiida-pseudo-1.0.0/src/aiida_pseudo/groups/mixins/cutoffs.py
--rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 aiida-pseudo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1188 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1078 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      230 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0    13321 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     8871 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/README.md
+-rw-r--r--   0        0        0     3245 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/__init__.py
+-rw-r--r--   0        0        0     3848 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/family.py
+-rw-r--r--   0        0        0    19578 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/install.py
+-rw-r--r--   0        0        0     2226 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/list.py
+-rw-r--r--   0        0        0      202 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/__init__.py
+-rw-r--r--   0        0        0      370 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/arguments.py
+-rw-r--r--   0        0        0     3635 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/options.py
+-rw-r--r--   0        0        0     7303 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/types.py
+-rw-r--r--   0        0        0     1031 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/root.py
+-rw-r--r--   0        0        0     2663 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/utils.py
+-rw-r--r--   0        0        0       60 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/common/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/common/units.py
+-rw-r--r--   0        0        0      105 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/__init__.py
+-rw-r--r--   0        0        0     2886 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/jthxml.py
+-rw-r--r--   0        0        0     7954 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/pseudo.py
+-rw-r--r--   0        0        0     2742 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psf.py
+-rw-r--r--   0        0        0     4519 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psml.py
+-rw-r--r--   0        0        0     3076 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psp8.py
+-rw-r--r--   0        0        0     4707 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/upf.py
+-rw-r--r--   0        0        0     6686 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/vps.py
+-rw-r--r--   0        0        0      102 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/cutoffs.py
+-rw-r--r--   0        0        0    15544 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo.py
+-rw-r--r--   0        0        0    18127 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo_dojo.py
+-rw-r--r--   0        0        0     3973 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/sssp.py
+-rw-r--r--   0        0        0      178 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/mixins/__init__.py
+-rw-r--r--   0        0        0    14194 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/mixins/cutoffs.py
+-rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 aiida-pseudo-1.0.1/PKG-INFO
```

### Comparing `aiida-pseudo-1.0.0/.gitignore` & `aiida-pseudo-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/.pre-commit-config.yaml` & `aiida-pseudo-1.0.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 -   repo: https://github.com/ikamensh/flynt/
     rev: '0.76'
     hooks:
     -   id: flynt
 
 -   repo: https://github.com/pycqa/isort
-    rev: '5.10.1'
+    rev: '5.12.0'
     hooks:
     -   id: isort
 
 -   repo: https://github.com/pre-commit/mirrors-yapf
     rev: 'v0.32.0'
     hooks:
     -   id: yapf
```

### Comparing `aiida-pseudo-1.0.0/CHANGELOG.md` & `aiida-pseudo-1.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Change log
 
+## `1.0.1` - 2023-05-08
+
+### Fixes
+- CLI: Change `Critical` to `Report` if family exists in `install` command [[3887762]](https://github.com/aiidateam/aiida-pseudo/commit/38877622cb658d7b37fd0f93fbdd649256146aa2)
+
+### Dependencies
+- Update pre-commit requirement `isort==5.12.0` [[d3b494e]](https://github.com/aiidateam/aiida-pseudo/commit/d3b494e68444b68f200f8f01a3673b8d028ffa3e)
+
+### Devops
+- Update compatibility matrix in `README.md` [[c04a7a7]](https://github.com/aiidateam/aiida-pseudo/commit/c04a7a775ef80ad41642e9faf506a2c632860c17)
+- Update Python version and `setup-python` action in CI/CD [[a62ce90]](https://github.com/aiidateam/aiida-pseudo/commit/a62ce90183414ef948262024cd0b03552ef2a7c1)
+- Docs: Update the URL for the `aiida-core` intersphinx inventory [[6756d1b]](https://github.com/aiidateam/aiida-pseudo/commit/6756d1b3ca05d3017c2d829924da0f6fd8b7ccb4)
+- Docs: Update Python version on RTD to 3.11 [[853adbf]](https://github.com/aiidateam/aiida-pseudo/commit/853adbf86b539367d54cf83d470bcfd8a27196fd)
+
+
 ## `1.0.0` - 2023-01-24
 
 As the package has been in production for quite some while, the current state, which was already released with `v0.9.0`, is released as the first stable major version.
 The only change is the removal of a workaround that was added to `v0.6.0` for backwards-compatibility.
 
 ### Changes
 - `RecommendedCutoffMixin`: Remove workaround for stringency units [[#147]](https://github.com/aiidateam/aiida-pseudo/pull/147)
```

### Comparing `aiida-pseudo-1.0.0/LICENSE.txt` & `aiida-pseudo-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/README.md` & `aiida-pseudo-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ## Compatibility matrix
 
 The following table shows which versions of `aiida-pseudo` are compatible with which versions of AiiDA and Python.
 
 | Plugin | AiiDA | Python |
 |-       |-      |-       |
-| `v0.8.0 < v1.0.0` | ![Compatibility for v0.8][AiiDA v2.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.8.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
+| `v0.8.0 < v2.0.0` | ![Compatibility for v0.8][AiiDA v2.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.8.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
 | `v0.7.0 < v0.8.0` | ![Compatibility for v0.7][AiiDA v2.0.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.7.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
 | `v0.1.0 < v0.7.0` | ![Compatibility for v0.6][AiiDA v1.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.6.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
 
 ## License
 The `aiida-pseudo` plugin package is released under the MIT license.
 See the `LICENSE.txt` file for more details.
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 workflows/ci/badge.svg?event=push)](https://github.com/aiidateam/aiida-pseudo/
 actions) [![Docs status](https://readthedocs.org/projects/aiida-pseudo/badge)]
 (http://aiida-pseudo.readthedocs.io/) AiiDA plugin that simplifies working with
 pseudopotentials. For more information on how to install and use the package,
 please consult [the documentation](http://aiida-pseudo.readthedocs.io/). ##
 Compatibility matrix The following table shows which versions of `aiida-pseudo`
 are compatible with which versions of AiiDA and Python. | Plugin | AiiDA |
-Python | |- |- |- | | `v0.8.0 < v1.0.0` | ![Compatibility for v0.8][AiiDA v2.x]
+Python | |- |- |- | | `v0.8.0 < v2.0.0` | ![Compatibility for v0.8][AiiDA v2.x]
 | [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/
 0.8.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) | | `v0.7.0 < v0.8.0` |
 ![Compatibility for v0.7][AiiDA v2.0.x] | [![PyPI pyversions](https://
 img.shields.io/pypi/pyversions/aiida-pseudo/0.7.0.svg)](https://
 pypi.python.org/pypi/aiida-pseudo/) | | `v0.1.0 < v0.7.0` | ![Compatibility for
 v0.6][AiiDA v1.x] | [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
 aiida-pseudo/0.6.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) | ##
```

### Comparing `aiida-pseudo-1.0.0/pyproject.toml` & `aiida-pseudo-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/family.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/family.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/install.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """Command to install a pseudo potential family."""
 import json
 import pathlib
 import shutil
+import sys
 import tempfile
 import typing as t
 
 from aiida.cmdline.params import options as options_core
 from aiida.cmdline.utils import decorators, echo
 import click
 import requests
@@ -206,15 +207,16 @@
     configuration = SsspConfiguration(version, functional, protocol)
     label = SsspFamily.format_configuration_label(configuration)
 
     if configuration not in SsspFamily.valid_configurations:
         echo.echo_critical(f'{configuration} is not a valid configuration.')
 
     if not download_only and QueryBuilder().append(SsspFamily, filters={'label': label}).first():
-        echo.echo_critical(f'{SsspFamily.__name__}<{label}> is already installed')
+        echo.echo_report(f'{SsspFamily.__name__}<{label}> is already installed')
+        sys.exit(1)
 
     with tempfile.TemporaryDirectory() as dirpath:
 
         dirpath = pathlib.Path(dirpath)
         filepath_archive = dirpath / 'archive.tar.gz'
         filepath_metadata = dirpath / 'metadata.json'
 
@@ -311,15 +313,16 @@
     label = PseudoDojoFamily.format_configuration_label(configuration)
     description = f'{configuration} installed with aiida-pseudo v{__version__}'
 
     if configuration not in PseudoDojoFamily.valid_configurations:
         echo.echo_critical(f'{configuration} is not a valid configuration')
 
     if not download_only and QueryBuilder().append(PseudoDojoFamily, filters={'label': label}).first():
-        echo.echo_critical(f'{PseudoDojoFamily.__name__}<{label}> is already installed.')
+        echo.echo_report(f'{PseudoDojoFamily.__name__}<{label}> is already installed.')
+        sys.exit(1)
 
     with tempfile.TemporaryDirectory() as dirpath:
 
         dirpath = pathlib.Path(dirpath)
         filepath_archive = dirpath / 'archive.tgz'
         filepath_metadata = dirpath / 'metadata.tgz'
```

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/list.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/list.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/params/options.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/options.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/params/types.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/types.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/root.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/root.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/cli/utils.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/jthxml.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/jthxml.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/pseudo.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/pseudo.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/psf.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psf.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/psml.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psml.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/psp8.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psp8.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/upf.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/upf.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/data/pseudo/vps.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/vps.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/cutoffs.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/cutoffs.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/pseudo.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/pseudo_dojo.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo_dojo.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/groups/family/sssp.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/sssp.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/src/aiida_pseudo/groups/mixins/cutoffs.py` & `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/mixins/cutoffs.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.0/PKG-INFO` & `aiida-pseudo-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-pseudo
-Version: 1.0.0
+Version: 1.0.1
 Summary: AiiDA plugin that simplifies working with pseudo potentials.
 Keywords: aiida,pseudopotentials
 Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -48,15 +48,15 @@
 
 ## Compatibility matrix
 
 The following table shows which versions of `aiida-pseudo` are compatible with which versions of AiiDA and Python.
 
 | Plugin | AiiDA | Python |
 |-       |-      |-       |
-| `v0.8.0 < v1.0.0` | ![Compatibility for v0.8][AiiDA v2.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.8.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
+| `v0.8.0 < v2.0.0` | ![Compatibility for v0.8][AiiDA v2.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.8.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
 | `v0.7.0 < v0.8.0` | ![Compatibility for v0.7][AiiDA v2.0.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.7.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
 | `v0.1.0 < v0.7.0` | ![Compatibility for v0.6][AiiDA v1.x] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.6.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/) |
 
 ## License
 The `aiida-pseudo` plugin package is released under the MIT license.
 See the `LICENSE.txt` file for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiida-pseudo Version: 1.0.0 Summary: AiiDA plugin
+Metadata-Version: 2.1 Name: aiida-pseudo Version: 1.0.1 Summary: AiiDA plugin
 that simplifies working with pseudo potentials. Keywords:
 aiida,pseudopotentials Author-email: "Sebastiaan P. Huber"
 sphuber.net> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: AiiDA Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Programming Language :: Python Classifier: Programming
@@ -27,15 +27,15 @@
 aiidateam/aiida-pseudo/workflows/ci/badge.svg?event=push)](https://github.com/
 aiidateam/aiida-pseudo/actions) [![Docs status](https://readthedocs.org/
 projects/aiida-pseudo/badge)](http://aiida-pseudo.readthedocs.io/) AiiDA plugin
 that simplifies working with pseudopotentials. For more information on how to
 install and use the package, please consult [the documentation](http://aiida-
 pseudo.readthedocs.io/). ## Compatibility matrix The following table shows
 which versions of `aiida-pseudo` are compatible with which versions of AiiDA
-and Python. | Plugin | AiiDA | Python | |- |- |- | | `v0.8.0 < v1.0.0` | !
+and Python. | Plugin | AiiDA | Python | |- |- |- | | `v0.8.0 < v2.0.0` | !
 [Compatibility for v0.8][AiiDA v2.x] | [![PyPI pyversions](https://
 img.shields.io/pypi/pyversions/aiida-pseudo/0.8.0.svg)](https://
 pypi.python.org/pypi/aiida-pseudo/) | | `v0.7.0 < v0.8.0` | ![Compatibility for
 v0.7][AiiDA v2.0.x] | [![PyPI pyversions](https://img.shields.io/pypi/
 pyversions/aiida-pseudo/0.7.0.svg)](https://pypi.python.org/pypi/aiida-pseudo/
 ) | | `v0.1.0 < v0.7.0` | ![Compatibility for v0.6][AiiDA v1.x] | [![PyPI
 pyversions](https://img.shields.io/pypi/pyversions/aiida-pseudo/0.6.0.svg)]
```

