# Comparing `tmp/databutton-0.9.1.tar.gz` & `tmp/databutton-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databutton-0.9.1.tar", max compression
+gzip compressed data, was "databutton-0.9.2.tar", max compression
```

## Comparing `databutton-0.9.1.tar` & `databutton-0.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       45 2022-05-25 21:06:11.107783 databutton-0.9.1/LICENSE
--rw-r--r--   0        0        0     1312 2022-05-25 21:06:11.107783 databutton-0.9.1/README.md
--rw-r--r--   0        0        0      377 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/__init__.py
--rw-r--r--   0        0        0        0 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/auth/__init__.py
--rw-r--r--   0        0        0     3231 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/auth/auth.html
--rw-r--r--   0        0        0     1078 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/auth/server.py
--rw-r--r--   0        0        0     9309 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/cli.py
--rw-r--r--   0        0        0        0 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/dataframes/__init__.py
--rw-r--r--   0        0        0      653 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/dataframes/dataframes.py
--rw-r--r--   0        0        0        0 2022-05-25 21:06:11.107783 databutton-0.9.1/databutton/decorators/__init__.py
--rw-r--r--   0        0        0     1366 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/decorators/schedule.py
--rw-r--r--   0        0        0     1586 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/decorators/streamlit.py
--rw-r--r--   0        0        0      302 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/docker/Dockerfile
--rw-r--r--   0        0        0        0 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/helpers/__init__.py
--rw-r--r--   0        0        0     2497 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/helpers/parse.py
--rw-r--r--   0        0        0     4548 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/kubernetes/generate.py
--rw-r--r--   0        0        0        0 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/server/__init__.py
--rw-r--r--   0        0        0     3352 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/server/processes.py
--rw-r--r--   0        0        0     1870 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/server/prod.py
--rw-r--r--   0        0        0     1908 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/server/server.py
--rw-r--r--   0        0        0     5817 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/utils/__init__.py
--rw-r--r--   0        0        0     3553 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/utils/build.py
--rw-r--r--   0        0        0       39 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/utils/config.py
--rw-r--r--   0        0        0     2482 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/utils/deploy.py
--rw-r--r--   0        0        0     1094 2022-05-25 21:06:11.111783 databutton-0.9.1/databutton/utils/log_status.py
--rw-r--r--   0        0        0      221 2022-05-25 21:08:10.207976 databutton-0.9.1/databutton/version.py
--rw-r--r--   0        0        0     1186 2022-05-25 21:08:10.215976 databutton-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2620 2022-05-25 21:08:12.112691 databutton-0.9.1/setup.py
--rw-r--r--   0        0        0     2310 2022-05-25 21:08:12.113191 databutton-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2022-05-27 01:37:07.937800 databutton-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1312 2022-05-27 01:37:07.937800 databutton-0.9.2/README.md
+-rw-r--r--   0        0        0      377 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/auth/__init__.py
+-rw-r--r--   0        0        0     3231 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/auth/auth.html
+-rw-r--r--   0        0        0     1078 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/auth/server.py
+-rw-r--r--   0        0        0     9309 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/cli.py
+-rw-r--r--   0        0        0        0 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/dataframes/__init__.py
+-rw-r--r--   0        0        0      653 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/dataframes/dataframes.py
+-rw-r--r--   0        0        0        0 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/decorators/__init__.py
+-rw-r--r--   0        0        0     1366 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/decorators/schedule.py
+-rw-r--r--   0        0        0     1586 2022-05-27 01:37:07.937800 databutton-0.9.2/databutton/decorators/streamlit.py
+-rw-r--r--   0        0        0      302 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/helpers/__init__.py
+-rw-r--r--   0        0        0     2497 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/helpers/parse.py
+-rw-r--r--   0        0        0     4548 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/kubernetes/generate.py
+-rw-r--r--   0        0        0        0 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/server/__init__.py
+-rw-r--r--   0        0        0     3352 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/server/processes.py
+-rw-r--r--   0        0        0     1870 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/server/prod.py
+-rw-r--r--   0        0        0     1908 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/server/server.py
+-rw-r--r--   0        0        0     5817 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/utils/__init__.py
+-rw-r--r--   0        0        0     3553 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/utils/build.py
+-rw-r--r--   0        0        0       39 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/utils/config.py
+-rw-r--r--   0        0        0     2482 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/utils/deploy.py
+-rw-r--r--   0        0        0     1094 2022-05-27 01:37:07.941800 databutton-0.9.2/databutton/utils/log_status.py
+-rw-r--r--   0        0        0      221 2022-05-27 01:38:56.945177 databutton-0.9.2/databutton/version.py
+-rw-r--r--   0        0        0     1186 2022-05-27 01:38:56.953177 databutton-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2620 2022-05-27 01:38:58.575494 databutton-0.9.2/setup.py
+-rw-r--r--   0        0        0     2310 2022-05-27 01:38:58.575972 databutton-0.9.2/PKG-INFO
```

### Comparing `databutton-0.9.1/README.md` & `databutton-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/auth/auth.html` & `databutton-0.9.2/databutton/auth/auth.html`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/auth/server.py` & `databutton-0.9.2/databutton/auth/server.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/cli.py` & `databutton-0.9.2/databutton/cli.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/dataframes/dataframes.py` & `databutton-0.9.2/databutton/dataframes/dataframes.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/decorators/schedule.py` & `databutton-0.9.2/databutton/decorators/schedule.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/decorators/streamlit.py` & `databutton-0.9.2/databutton/decorators/streamlit.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/helpers/parse.py` & `databutton-0.9.2/databutton/helpers/parse.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/kubernetes/generate.py` & `databutton-0.9.2/databutton/kubernetes/generate.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/server/processes.py` & `databutton-0.9.2/databutton/server/processes.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/server/prod.py` & `databutton-0.9.2/databutton/server/prod.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/server/server.py` & `databutton-0.9.2/databutton/server/server.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/utils/__init__.py` & `databutton-0.9.2/databutton/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/utils/build.py` & `databutton-0.9.2/databutton/utils/build.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/utils/deploy.py` & `databutton-0.9.2/databutton/utils/deploy.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/databutton/utils/log_status.py` & `databutton-0.9.2/databutton/utils/log_status.py`

 * *Files identical despite different names*

### Comparing `databutton-0.9.1/pyproject.toml` & `databutton-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databutton"
-version = "0.9.1"
+version = "0.9.2"
 description = "The CLI for databutton.com"
 authors = ["Databutton <hi@databutton.io>"]
 license = "Databutton"
 readme = "README.md"
 packages = [
   { include = "databutton"}
 ]
@@ -18,15 +18,15 @@
 streamlit = "^1.9.0"
 uvicorn = "^0.17.6"
 watchgod = "^0.8.2"
 PyYAML = "^6.0"
 yaspin = "^2.1.0"
 schedule = "^1.1.0"
 dataclasses-json = "^0.5.7"
-databutton-web = "^0.6.1"
+databutton-web = "^0.8.0"
 # This is the same as streamlit, hopes it works
 pandas = ">=0.21.0"
 sentry-sdk = "^1.5.12"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
```

### Comparing `databutton-0.9.1/setup.py` & `databutton-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 package_data = \
 {'': ['*'], 'databutton': ['docker/*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'click>=7.0,<8.1',
- 'databutton-web>=0.6.1,<0.7.0',
+ 'databutton-web>=0.8.0,<0.9.0',
  'dataclasses-json>=0.5.7,<0.6.0',
  'fastapi>=0.78.0,<0.79.0',
  'httpx>=0.23.0,<0.24.0',
  'pandas>=0.21.0',
  'schedule>=1.1.0,<2.0.0',
  'sentry-sdk>=1.5.12,<2.0.0',
  'streamlit>=1.9.0,<2.0.0',
@@ -31,15 +31,15 @@
  'yaspin>=2.1.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['databutton = databutton.cli:cli']}
 
 setup_kwargs = {
     'name': 'databutton',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'The CLI for databutton.com',
     'long_description': "# databutton-cli\n[![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)\n[![PyPI version fury.io](https://badge.fury.io/py/databutton.svg)](https://pypi.python.org/pypi/databutton/)\n[![PyPI download week](https://img.shields.io/pypi/dw/databutton.svg)](https://pypi.python.org/pypi/databutton/)\n![release](https://github.com/databutton/databutton-cli/actions/workflows/release.yaml/badge.svg)\n\n\n\n\nThe CLI for building and deploying databutton projects\n\n## Getting Started\n\n`pip install databutton`\n\n`databutton create my-project`\n\n`databutton login`\n\n`databutton deploy`\n\n## Developing\n\n### Prerequisites\nThis project uses poetry, so if you haven't already;\n\n`pip install poetry`\n\n### Install dependencies\n\n`poetry install`\n\n### Test\n\n`poetry run pytest`\n\nAlternatively run `poetry run pytest -s` to see `print` statements for debugging purposes.\n\n### Test locally in another package\n\nTo test in another package, you can simply\n\n`pip install -e .` assuming you're in this folder. If not, replace the `.` with the path to the `databutton-cli` folder.\n\n## Authors\n\n* **Databutton** - *Initial work* - [github](https://github.com/databutton)\n\n## License: Copyright (c) Databutton\n\nAll rights reserved.",
     'author': 'Databutton',
     'author_email': 'hi@databutton.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databutton-0.9.1/PKG-INFO` & `databutton-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: databutton
-Version: 0.9.1
+Version: 0.9.2
 Summary: The CLI for databutton.com
 License: Databutton
 Author: Databutton
 Author-email: hi@databutton.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=7.0,<8.1)
-Requires-Dist: databutton-web (>=0.6.1,<0.7.0)
+Requires-Dist: databutton-web (>=0.8.0,<0.9.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: fastapi (>=0.78.0,<0.79.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: pandas (>=0.21.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: sentry-sdk (>=1.5.12,<2.0.0)
 Requires-Dist: streamlit (>=1.9.0,<2.0.0)
```

