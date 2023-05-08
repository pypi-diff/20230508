# Comparing `tmp/databooks-1.3.7.tar.gz` & `tmp/databooks-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databooks-1.3.7.tar", max compression
+gzip compressed data, was "databooks-1.3.8.tar", max compression
```

## Comparing `databooks-1.3.7.tar` & `databooks-1.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1086 2022-11-27 13:19:11.529018 databooks-1.3.7/LICENSE
--rw-r--r--   0        0        0     4327 2022-11-27 13:19:11.529018 databooks-1.3.7/README.md
--rw-r--r--   0        0        0       59 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/__init__.py
--rw-r--r--   0        0        0      136 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/__main__.py
--rw-r--r--   0        0        0     8316 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/affirm.py
--rw-r--r--   0        0        0    16607 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/cli.py
--rw-r--r--   0        0        0     3082 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/common.py
--rw-r--r--   0        0        0      818 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/config.py
--rw-r--r--   0        0        0     4292 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/conflicts.py
--rw-r--r--   0        0        0        0 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/data_models/__init__.py
--rw-r--r--   0        0        0     5105 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/data_models/base.py
--rw-r--r--   0        0        0    10460 2022-11-27 13:19:11.529018 databooks-1.3.7/databooks/data_models/cell.py
--rw-r--r--   0        0        0    11358 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/data_models/notebook.py
--rw-r--r--   0        0        0     2766 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/data_models/rich_helpers.py
--rw-r--r--   0        0        0     6134 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/git_utils.py
--rw-r--r--   0        0        0      780 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/logging.py
--rw-r--r--   0        0        0     3660 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/metadata.py
--rw-r--r--   0        0        0        0 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/py.typed
--rw-r--r--   0        0        0     2258 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/recipes.py
--rw-r--r--   0        0        0     4599 2022-11-27 13:19:11.533018 databooks-1.3.7/databooks/tui.py
--rw-r--r--   0        0        0       22 2022-11-27 13:19:55.781504 databooks-1.3.7/databooks/version.py
--rw-r--r--   0        0        0     1375 2022-11-27 13:19:55.745504 databooks-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     5401 2022-11-27 13:19:58.329629 databooks-1.3.7/setup.py
--rw-r--r--   0        0        0     5297 2022-11-27 13:19:58.330218 databooks-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-08 12:06:22.480543 databooks-1.3.8/LICENSE
+-rw-r--r--   0        0        0     4327 2023-05-08 12:06:22.480543 databooks-1.3.8/README.md
+-rw-r--r--   0        0        0       59 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/__main__.py
+-rw-r--r--   0        0        0     8316 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/affirm.py
+-rw-r--r--   0        0        0    16607 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/cli.py
+-rw-r--r--   0        0        0     3082 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/common.py
+-rw-r--r--   0        0        0      818 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/config.py
+-rw-r--r--   0        0        0     4292 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/conflicts.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/data_models/__init__.py
+-rw-r--r--   0        0        0     5105 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/data_models/base.py
+-rw-r--r--   0        0        0    10460 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/data_models/cell.py
+-rw-r--r--   0        0        0    11358 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/data_models/notebook.py
+-rw-r--r--   0        0        0     2766 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/data_models/rich_helpers.py
+-rw-r--r--   0        0        0     6133 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/git_utils.py
+-rw-r--r--   0        0        0      780 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/logging.py
+-rw-r--r--   0        0        0     3660 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/metadata.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/py.typed
+-rw-r--r--   0        0        0     2258 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/recipes.py
+-rw-r--r--   0        0        0     4599 2023-05-08 12:06:22.480543 databooks-1.3.8/databooks/tui.py
+-rw-r--r--   0        0        0       22 2023-05-08 12:06:56.896317 databooks-1.3.8/databooks/version.py
+-rw-r--r--   0        0        0     1375 2023-05-08 12:06:56.864318 databooks-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 databooks-1.3.8/setup.py
+-rw-r--r--   0        0        0     5348 1970-01-01 00:00:00.000000 databooks-1.3.8/PKG-INFO
```

### Comparing `databooks-1.3.7/LICENSE` & `databooks-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/README.md` & `databooks-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/affirm.py` & `databooks-1.3.8/databooks/affirm.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/cli.py` & `databooks-1.3.8/databooks/cli.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/common.py` & `databooks-1.3.8/databooks/common.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/config.py` & `databooks-1.3.8/databooks/config.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/conflicts.py` & `databooks-1.3.8/databooks/conflicts.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/data_models/base.py` & `databooks-1.3.8/databooks/data_models/base.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/data_models/cell.py` & `databooks-1.3.8/databooks/data_models/cell.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/data_models/notebook.py` & `databooks-1.3.8/databooks/data_models/notebook.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/data_models/rich_helpers.py` & `databooks-1.3.8/databooks/data_models/rich_helpers.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/git_utils.py` & `databooks-1.3.8/databooks/git_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     *,
     repo: Optional[Repo] = None,
     verbose: bool = False,
 ) -> List[DiffContents]:
     """
     Get the noteebook(s) git diff(s).
 
-    By default, diffs are compared with the current working direcotory. That is, staged
+    By default, diffs are compared with the current working directory. That is, staged
      files will still show up in the diffs. Only return the diffs for notebook files.
     """
     if verbose:
         set_verbose(logger)
 
     common_path = find_common_parent(paths or [Path.cwd()])
     repo = get_repo(path=common_path) if repo is None else repo
```

### Comparing `databooks-1.3.7/databooks/logging.py` & `databooks-1.3.8/databooks/logging.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/metadata.py` & `databooks-1.3.8/databooks/metadata.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/recipes.py` & `databooks-1.3.8/databooks/recipes.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/databooks/tui.py` & `databooks-1.3.8/databooks/tui.py`

 * *Files identical despite different names*

### Comparing `databooks-1.3.7/pyproject.toml` & `databooks-1.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databooks"
-version = "1.3.7"  # dynamically set in CI
+version = "1.3.8"  # dynamically set in CI
 description = "A CLI tool to resolve git conflicts and remove metadata in notebooks."
 authors = ["Murilo Cunha <murilo@dataroots.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://datarootsio.github.io/databooks/"
 repository = "https://github.com/datarootsio/databooks/"
 keywords = ["jupyter-notebooks", "cli"]
```

### Comparing `databooks-1.3.7/setup.py` & `databooks-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
  'typing-extensions>=4.0.1,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['databooks = databooks.cli:app']}
 
 setup_kwargs = {
     'name': 'databooks',
-    'version': '1.3.7',
+    'version': '1.3.8',
     'description': 'A CLI tool to resolve git conflicts and remove metadata in notebooks.',
     'long_description': '<p align="center">\n  <a href="https://datarootsio.github.io/databooks/"><img alt="logo" src="https://raw.githubusercontent.com/datarootsio/databooks/main/docs/images/logo.png"></a>\n</p>\n<p align="center">\n  <a href="https://dataroots.io"><img alt="Maintained by dataroots" src="https://dataroots.io/maintained-rnd.svg" /></a>\n  <a href="https://pypi.org/project/databooks/"><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/databooks" /></a>\n  <a href="https://pypi.org/project/databooks/"><img alt="PiPy" src="https://img.shields.io/pypi/v/databooks" /></a>\n  <a href="https://pepy.tech/project/databooks"><img alt="Downloads" src="https://pepy.tech/badge/databooks" /></a>\n  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>\n  <a href="http://mypy-lang.org/"><img alt="Mypy checked" src="https://img.shields.io/badge/mypy-checked-1f5082.svg" /></a>\n  <a href="https://pepy.tech/project/databooks"><img alt="Codecov" src="https://codecov.io/github/datarootsio/databooks/main/graph/badge.svg" /></a>\n  <a href="https://github.com/datarootsio/databooks/actions"><img alt="test" src="https://github.com/datarootsio/databooks/actions/workflows/test.yml/badge.svg" /></a>\n</p>\n\n\n`databooks` is a package to ease the collaboration between data scientists using\n[Jupyter notebooks](https://jupyter.org/), by reducing the number of git conflicts between\ndifferent notebooks and resolution of git conflicts when encountered.\n\nThe key features include:\n\n- CLI tool\n  - Clear notebook metadata\n  - Resolve git conflicts\n- Simple to use\n- Simple API for using modelling and comparing notebooks using [Pydantic](https://pydantic-docs.helpmanual.io/)\n\n## Requirements\n\n`databooks` is built on top of:\n\n- Python 3.7+\n- [Typer](https://typer.tiangolo.com/)\n- [Rich](https://rich.readthedocs.io/en/latest/)\n- [Pydantic](https://pydantic-docs.helpmanual.io/)\n- [GitPython](https://gitpython.readthedocs.io/en/stable/tutorial.html)\n- [Tomli](https://github.com/hukkin/tomli)\n\n## Installation\n\n```\npip install databooks\n```\n\n## Usage\n\n### Clear metadata\n\nSimply specify the paths for notebook files to remove metadata. By doing so, we can\nalready avoid many of the conflicts.\n\n```console\n$ databooks meta [OPTIONS] PATHS...\n```\n\n![databooks meta demo](https://raw.githubusercontent.com/datarootsio/databooks/main/docs/images/databooks-meta.gif)\n\n### Fix git conflicts for notebooks\n\nSpecify the paths for notebook files with conflicts to be fixed. Then, `databooks` finds\nthe source notebooks that caused the conflicts and compares them (so no JSON manipulation!)\n\n```console\n$ databooks fix [OPTIONS] PATHS...\n```\n\n![databooks fix demo](https://raw.githubusercontent.com/datarootsio/databooks/main/docs/images/databooks-fix.gif)\n\n### Assert notebook metadata\n\nSpecify paths of notebooks to be checked, an expression or recipe of what you\'d like to\nenforce. `databooks` will run your checks and raise errors if any notebook does not\ncomply with the desired metadata values. This advanced feature allows users to enforce\ncell tags, sequential cell execution, maximum number of cells, among many other things!\n\nCheck out our [docs](https://databooks.dev/latest/usage/overview/#databooks-assert) for more!\n\n```console\n$ databooks assert [OPTIONS] PATHS...\n```\n\n![databooks assert demo](https://raw.githubusercontent.com/datarootsio/databooks/main/docs/images/databooks-assert.gif)\n\n### Show rich notebook\n\nInstead of launching Jupyter and opening the browser to inspect notebooks, have a quick\nlook at them in the terminal. All you need is to specify the path(s) of the notebook(s).\n\n```console\n$ databooks show [OPTIONS] PATHS...\n```\n\n![databooks show demo](https://raw.githubusercontent.com/datarootsio/databooks/main/docs/images/databooks-show.gif)\n\n### Show rich notebook diffs\n\nSimilar to git diff, but for notebooks! Show a rich diff of the notebooks in the\nterminal. Works for comparing git index with the current working directory, comparing\nbranches or blobs.\n\n```console\n$ databooks diff [OPTIONS] [REF_BASE] [REF_REMOTE] [PATHS]...\n```\n\n![databooks diff demo](https://raw.githubusercontent.com/datarootsio/databooks/main/docs/images/databooks-diff.gif)\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     'author': 'Murilo Cunha',
     'author_email': 'murilo@dataroots.io',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://datarootsio.github.io/databooks/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['databooks',
 'databooks.data_models'] package_data = \ {'': ['*']} install_requires = \
 ['GitPython>=3.1.24,<4.0.0', 'pydantic>=1.8.2,<2.0.0', 'rich>=12.6.0,<13.0.0',
 'tomli>=2.0.1,<3.0.0', 'typer>=0.4.0,<1.0.0', 'typing-
 extensions>=4.0.1,<5.0.0'] entry_points = \ {'console_scripts': ['databooks =
-databooks.cli:app']} setup_kwargs = { 'name': 'databooks', 'version': '1.3.7',
+databooks.cli:app']} setup_kwargs = { 'name': 'databooks', 'version': '1.3.8',
 'description': 'A CLI tool to resolve git conflicts and remove metadata in
 notebooks.', 'long_description': '
                                   \n [logo]\n
 \n
 \n [Maintained_by_dataroots]\n [Python_versions]\n [PiPy]\n [Downloads]\n [Code
              style:_black]\n [Mypy_checked]\n [Codecov]\n [test]\n
 \n\n\n`databooks` is a package to ease the collaboration between data
@@ -49,11 +49,11 @@
 diff, but for notebooks! Show a rich diff of the notebooks in the\nterminal.
 Works for comparing git index with the current working directory,
 comparing\nbranches or blobs.\n\n```console\n$ databooks diff [OPTIONS]
 [REF_BASE] [REF_REMOTE] [PATHS]...\n```\n\n![databooks diff demo](https://
 raw.githubusercontent.com/datarootsio/databooks/main/docs/images/databooks-
 diff.gif)\n\n## License\n\nThis project is licensed under the terms of the MIT
 license.\n', 'author': 'Murilo Cunha', 'author_email': 'murilo@dataroots.io',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://
 datarootsio.github.io/databooks/', 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'entry_points':
 entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `databooks-1.3.7/PKG-INFO` & `databooks-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: databooks
-Version: 1.3.7
+Version: 1.3.8
 Summary: A CLI tool to resolve git conflicts and remove metadata in notebooks.
 Home-page: https://datarootsio.github.io/databooks/
 License: MIT
 Keywords: jupyter-notebooks,cli
 Author: Murilo Cunha
 Author-email: murilo@dataroots.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.24,<4.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer (>=0.4.0,<1.0.0)
 Requires-Dist: typing-extensions (>=4.0.1,<5.0.0)
 Project-URL: Repository, https://github.com/datarootsio/databooks/
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: databooks Version: 1.3.7 Summary: A CLI tool to
+Metadata-Version: 2.1 Name: databooks Version: 1.3.8 Summary: A CLI tool to
 resolve git conflicts and remove metadata in notebooks. Home-page: https://
 datarootsio.github.io/databooks/ License: MIT Keywords: jupyter-notebooks,cli
 Author: Murilo Cunha Author-email: murilo@dataroots.io Requires-Python:
 >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Dist: GitPython (>=3.1.24,<4.0.0) Requires-Dist:
-pydantic (>=1.8.2,<2.0.0) Requires-Dist: rich (>=12.6.0,<13.0.0) Requires-Dist:
-tomli (>=2.0.1,<3.0.0) Requires-Dist: typer (>=0.4.0,<1.0.0) Requires-Dist:
-typing-extensions (>=4.0.1,<5.0.0) Project-URL: Repository, https://github.com/
-datarootsio/databooks/ Description-Content-Type: text/markdown
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: GitPython (>=3.1.24,<4.0.0) Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: typer (>=0.4.0,<1.0.0) Requires-Dist: typing-extensions
+(>=4.0.1,<5.0.0) Project-URL: Repository, https://github.com/datarootsio/
+databooks/ Description-Content-Type: text/markdown
                                     [logo]
   [Maintained_by_dataroots] [Python_versions] [PiPy] [Downloads] [Code_style:
                     black] [Mypy_checked] [Codecov] [test]
 `databooks` is a package to ease the collaboration between data scientists
 using [Jupyter notebooks](https://jupyter.org/), by reducing the number of git
 conflicts between different notebooks and resolution of git conflicts when
 encountered. The key features include: - CLI tool - Clear notebook metadata -
```

