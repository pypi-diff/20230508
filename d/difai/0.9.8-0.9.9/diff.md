# Comparing `tmp/difai-0.9.8.tar.gz` & `tmp/difai-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "difai-0.9.8.tar", max compression
+gzip compressed data, was "difai-0.9.9.tar", max compression
```

## Comparing `difai-0.9.8.tar` & `difai-0.9.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1614 2023-01-09 02:05:37.518541 difai-0.9.8/README.md
--rw-r--r--   0        0        0     1603 2023-01-09 02:05:37.520542 difai-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3505 2023-01-09 02:05:37.520542 difai-0.9.8/src/difai/__init__.py
--rw-r--r--   0        0        0     1296 2023-01-09 02:05:37.520542 difai-0.9.8/src/difai/main.py
--rw-r--r--   0        0        0        0 2023-01-09 02:05:37.520542 difai-0.9.8/src/difai/py.typed
--rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 difai-0.9.8/setup.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 difai-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1614 2023-01-16 02:05:47.259264 difai-0.9.9/README.md
+-rw-r--r--   0        0        0     1603 2023-01-16 02:05:47.260264 difai-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3505 2023-01-16 02:05:47.260264 difai-0.9.9/src/difai/__init__.py
+-rw-r--r--   0        0        0     1296 2023-01-16 02:05:47.261264 difai-0.9.9/src/difai/main.py
+-rw-r--r--   0        0        0        0 2023-01-16 02:05:47.261264 difai-0.9.9/src/difai/py.typed
+-rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 difai-0.9.9/setup.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 difai-0.9.9/PKG-INFO
```

### Comparing `difai-0.9.8/README.md` & `difai-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `difai-0.9.8/pyproject.toml` & `difai-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "difai"
-version = "0.9.8"
+version = "0.9.9"
 description = "'Did I forget any imports' generates requirement files for you"
 license = "WTFPL"
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 maintainers = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/marvin.vanaalst/difai"
 repository = "https://gitlab.com/marvin.vanaalst/difai"
```

### Comparing `difai-0.9.8/src/difai/__init__.py` & `difai-0.9.9/src/difai/__init__.py`

 * *Files identical despite different names*

### Comparing `difai-0.9.8/src/difai/main.py` & `difai-0.9.9/src/difai/main.py`

 * *Files identical despite different names*

### Comparing `difai-0.9.8/setup.py` & `difai-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['difai = difai.main:app']}
 
 setup_kwargs = {
     'name': 'difai',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': "'Did I forget any imports' generates requirement files for you",
     'long_description': '# Did I forget any imports?\n\n[![pipeline status](https://gitlab.com/marvin.vanaalst/difai/badges/main/pipeline.svg)](https://gitlab.com/marvin.vanaalst/difai/-/commits/main)\n[![coverage report](https://gitlab.com/marvin.vanaalst/difai/badges/main/coverage.svg)](https://gitlab.com/marvin.vanaalst/difai/-/commits/main)\n[![PyPi](https://img.shields.io/pypi/v/difai)](https://pypi.org/project/difai/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Downloads](https://pepy.tech/badge/difai)](https://pepy.tech/project/difai)\n\nDIFAI searches for import statements for all the python and jupyter notebook files in the current directory. It then uses `pip freeze` to get your installed versions and `pip-compile` to generate a `requirements.txt` file containing all of your dependencies and their depdendencies including hashes for a reproducible build.\n\n## Run\n\nSimply call `difai` in the current folder.\nYou can change the input (where the `.py` and `.ipynb` files are read) and output (where the `requirement.in` and `requirements.txt` files are written) folders using\n`--in-path` and `--out-path` respectively.\nIn order to exclude certain packages from the search, you can use the `--exclude` option.\n\n## Pipeline\n\n<div class="center">\n\n```mermaid\ngraph TB\n    A[glob] --> B\n    A --> C\n    B[.py] --> D\n    C[.ipynb] -->|nbconvert| B\n    D[AST]  --> E\n    X[pip freeze] --> E\n    E[requirements.in] -->|pip tools| F\n    F[requirements.txt]\n```\n\n</div>\n',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'Marvin van Aalst',
     'maintainer_email': 'marvin.vanaalst@gmail.com',
     'url': 'https://gitlab.com/marvin.vanaalst/difai',
```

### Comparing `difai-0.9.8/PKG-INFO` & `difai-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difai
-Version: 0.9.8
+Version: 0.9.9
 Summary: 'Did I forget any imports' generates requirement files for you
 Home-page: https://gitlab.com/marvin.vanaalst/difai
 License: WTFPL
 Keywords: packaging
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Maintainer: Marvin van Aalst
```

