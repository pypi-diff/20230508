# Comparing `tmp/hue_sunrise-0.6.8.tar.gz` & `tmp/hue_sunrise-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hue_sunrise-0.6.8.tar", max compression
+gzip compressed data, was "hue_sunrise-0.6.9.tar", max compression
```

## Comparing `hue_sunrise-0.6.8.tar` & `hue_sunrise-0.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1804 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/README.md
--rw-r--r--   0        0        0     1090 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     5459 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/src/hue_sunrise/__init__.py
--rw-r--r--   0        0        0      853 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/src/hue_sunrise/colors.py
--rw-r--r--   0        0        0     3287 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/src/hue_sunrise/connector.py
--rw-r--r--   0        0        0     3033 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/src/hue_sunrise/main.py
--rw-r--r--   0        0        0     2439 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/src/hue_sunrise/scene.py
--rw-r--r--   0        0        0      310 2023-02-06 02:05:07.265079 hue_sunrise-0.6.8/src/hue_sunrise/state.py
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 hue_sunrise-0.6.8/setup.py
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 hue_sunrise-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1804 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/README.md
+-rw-r--r--   0        0        0     1090 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     5459 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/src/hue_sunrise/__init__.py
+-rw-r--r--   0        0        0      853 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/src/hue_sunrise/colors.py
+-rw-r--r--   0        0        0     3287 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/src/hue_sunrise/connector.py
+-rw-r--r--   0        0        0     3033 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/src/hue_sunrise/main.py
+-rw-r--r--   0        0        0     2439 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/src/hue_sunrise/scene.py
+-rw-r--r--   0        0        0      310 2023-02-21 14:26:29.276628 hue_sunrise-0.6.9/src/hue_sunrise/state.py
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 hue_sunrise-0.6.9/setup.py
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 hue_sunrise-0.6.9/PKG-INFO
```

### Comparing `hue_sunrise-0.6.8/README.md` & `hue_sunrise-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `hue_sunrise-0.6.8/pyproject.toml` & `hue_sunrise-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hue-sunrise"
-version = "0.6.8"
+version = "0.6.9"
 description = ""
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "hue_sunrise", from = "src" }
 ]
```

### Comparing `hue_sunrise-0.6.8/src/hue_sunrise/__init__.py` & `hue_sunrise-0.6.9/src/hue_sunrise/__init__.py`

 * *Files identical despite different names*

### Comparing `hue_sunrise-0.6.8/src/hue_sunrise/colors.py` & `hue_sunrise-0.6.9/src/hue_sunrise/colors.py`

 * *Files identical despite different names*

### Comparing `hue_sunrise-0.6.8/src/hue_sunrise/connector.py` & `hue_sunrise-0.6.9/src/hue_sunrise/connector.py`

 * *Files identical despite different names*

### Comparing `hue_sunrise-0.6.8/src/hue_sunrise/main.py` & `hue_sunrise-0.6.9/src/hue_sunrise/main.py`

 * *Files identical despite different names*

### Comparing `hue_sunrise-0.6.8/src/hue_sunrise/scene.py` & `hue_sunrise-0.6.9/src/hue_sunrise/scene.py`

 * *Files identical despite different names*

### Comparing `hue_sunrise-0.6.8/setup.py` & `hue_sunrise-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['appdirs>=1.4.4,<2.0.0', 'requests>=2.28.1,<3.0.0', 'typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['hue-sunrise = hue_sunrise.main:app']}
 
 setup_kwargs = {
     'name': 'hue-sunrise',
-    'version': '0.6.8',
+    'version': '0.6.9',
     'description': '',
     'long_description': '# Hue sunrise\n\n[![pipeline status](https://gitlab.com/marvin.vanaalst/hue-sunrise/badges/main/pipeline.svg)](https://gitlab.com/marvin.vanaalst/hue-sunrise/-/commits/main)\n[![coverage report](https://gitlab.com/marvin.vanaalst/hue-sunrise/badges/main/coverage.svg)](https://gitlab.com/marvin.vanaalst/hue-sunrise/-/commits/main)\n[![PyPi](https://img.shields.io/pypi/v/hue-sunrise)](https://pypi.org/project/hue-sunrise/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Downloads](https://pepy.tech/badge/hue-sunrise)](https://pepy.tech/project/hue-sunrise)\n\nEnjoy waking up more gently by having your [philips hue](https://www.philips-hue.com/de-de) lights simulate a sunrise.\n\n## Installation\n\n```bash\npip install hue-sunrise\n```\n\n## Usage\n\nFirst register your Hue bridge interactively\n\n```bash\nhue-sunrise register\n```\n\nThen simply call it with\n\n```bash\nhue-sunrise run\n```\n\nAnd view the config using\n\n```bash\nhue-sunrise config show\n```\n\nIf you want to change the configuration use\n\n```bash\nhue-sunrise config ip               # IP address of your Hue bridge\nhue-sunrise config lights           # lights which should participate\nhue-sunrise config scene-length     # how many minutes the sunrise should take\nhue-sunrise config afterglow        # how many minutes to stay lit after the sunrise\n```\n\nor, if you want to change where the configuration files are stored use the following environment variables\n\n```bash\nHS_CONFIG_PATH\nHS_LOG_PATH\n```\n\n\nAnd finally if anything failed an you need to manually switch of the lights use\n\n```bash\nhue-sunrise shutdown\n```\n\n## Thanks\n\nThe beautiful CLI is due to [typer](https://typer.tiangolo.com/).\n',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hue_sunrise-0.6.8/PKG-INFO` & `hue_sunrise-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hue-sunrise
-Version: 0.6.8
+Version: 0.6.9
 Summary: 
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

