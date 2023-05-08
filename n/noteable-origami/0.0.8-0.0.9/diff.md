# Comparing `tmp/noteable_origami-0.0.8.tar.gz` & `tmp/noteable_origami-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noteable_origami-0.0.8.tar", max compression
+gzip compressed data, was "noteable_origami-0.0.9.tar", max compression
```

## Comparing `noteable_origami-0.0.8.tar` & `noteable_origami-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1516 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/LICENSE
--rw-r--r--   0        0        0     1824 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/README.md
--rw-r--r--   0        0        0        0 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/__init__.py
--rw-r--r--   0        0        0       18 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/_version.py
--rw-r--r--   0        0        0    35776 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/client.py
--rw-r--r--   0        0        0     3154 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/format.py
--rw-r--r--   0        0        0      400 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/pathing.py
--rw-r--r--   0        0        0      208 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/tests/__init__.py
--rw-r--r--   0        0        0     6609 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/tests/test_client.py
--rw-r--r--   0        0        0        0 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/tests/types/__init__.py
--rw-r--r--   0        0        0     1813 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/tests/types/test_kernels.py
--rw-r--r--   0        0        0     4549 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/access_levels.py
--rw-r--r--   0        0        0    12013 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/deltas.py
--rw-r--r--   0        0        0    13889 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/files.py
--rw-r--r--   0        0        0     6788 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/jobs.py
--rw-r--r--   0        0        0     9512 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/kernels.py
--rw-r--r--   0        0        0     1517 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/models.py
--rw-r--r--   0        0        0    21180 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/origami/types/rtu.py
--rw-r--r--   0        0        0     2551 2022-10-26 18:27:44.417003 noteable_origami-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 noteable_origami-0.0.8/setup.py
--rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 noteable_origami-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1824 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/__init__.py
+-rw-r--r--   0        0        0       18 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/_version.py
+-rw-r--r--   0        0        0    35727 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/client.py
+-rw-r--r--   0        0        0     3154 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/format.py
+-rw-r--r--   0        0        0      400 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/pathing.py
+-rw-r--r--   0        0        0      208 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/__init__.py
+-rw-r--r--   0        0        0     6534 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/test_client.py
+-rw-r--r--   0        0        0        0 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/types/__init__.py
+-rw-r--r--   0        0        0     1813 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/types/test_kernels.py
+-rw-r--r--   0        0        0     4549 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/access_levels.py
+-rw-r--r--   0        0        0    12013 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/deltas.py
+-rw-r--r--   0        0        0    13889 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/files.py
+-rw-r--r--   0        0        0     6788 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/jobs.py
+-rw-r--r--   0        0        0     9512 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/kernels.py
+-rw-r--r--   0        0        0     1517 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/models.py
+-rw-r--r--   0        0        0    21180 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/rtu.py
+-rw-r--r--   0        0        0     2551 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 noteable_origami-0.0.9/setup.py
+-rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 noteable_origami-0.0.9/PKG-INFO
```

### Comparing `noteable_origami-0.0.8/LICENSE` & `noteable_origami-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/README.md` & `noteable_origami-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/client.py` & `noteable_origami-0.0.9/origami/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,15 @@
                     ", using default empty config"
                 )
                 config = ClientConfig()
             else:
                 config = ClientConfig.parse_file(settings.auth0_config_path)
 
         self.config = config
-        self.config.domain = os.getenv(
-            "NOTEABLE_URI", os.getenv("NOTEABLE_DOMAIN", self.config.domain)
-        )
+        self.config.domain = os.getenv("NOTEABLE_DOMAIN", self.config.domain)
         self.file_session_cache = {}
 
         self.user = None
         self.token = api_token or os.getenv("NOTEABLE_TOKEN") or self.get_token()
         if isinstance(self.token, str):
             self.token = Token(access_token=self.token)
         self.rtu_socket = None
```

### Comparing `noteable_origami-0.0.8/origami/format.py` & `noteable_origami-0.0.9/origami/format.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/tests/test_client.py` & `noteable_origami-0.0.9/origami/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,16 @@
 
 def test_token_is_loaded_from_env(client_config):
     os.environ["NOTEABLE_TOKEN"] = "fake-token-env"
     client = NoteableClient(config=client_config)
     assert client.token.access_token == "fake-token-env"
 
 
-@pytest.mark.parametrize("env_name", ["NOTEABLE_URI", "NOTEABLE_DOMAIN"])
-def test_domain_is_loaded_from_env(client_config, env_name):
-    os.environ[env_name] = "https://example.com"
+def test_domain_is_loaded_from_env(client_config):
+    os.environ["NOTEABLE_DOMAIN"] = "https://example.com"
     client = NoteableClient(config=client_config)
     assert client.config.domain == "https://example.com"
 
 
 @pytest.mark.asyncio
 async def test_client_ping(connect_mock, client):
     # The connect does a ping to ensure that the connection is healthy
```

### Comparing `noteable_origami-0.0.8/origami/tests/types/test_kernels.py` & `noteable_origami-0.0.9/origami/tests/types/test_kernels.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/access_levels.py` & `noteable_origami-0.0.9/origami/types/access_levels.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/deltas.py` & `noteable_origami-0.0.9/origami/types/deltas.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/files.py` & `noteable_origami-0.0.9/origami/types/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/jobs.py` & `noteable_origami-0.0.9/origami/types/jobs.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/kernels.py` & `noteable_origami-0.0.9/origami/types/kernels.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/models.py` & `noteable_origami-0.0.9/origami/types/models.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/origami/types/rtu.py` & `noteable_origami-0.0.9/origami/types/rtu.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.8/pyproject.toml` & `noteable_origami-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "noteable-origami"
-version = "0.0.8"
+version = "0.0.9"
 description = "The Noteable API interface"
 authors = ["Matt Seal <matt@noteable.io>"]
 maintainers = ["Matt Seal <matt@noteable.io>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/noteable-io/origami"
 # old setup.cfg had a bdist_wheel option.
@@ -35,15 +35,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 bitmath = "^1.3.3"
 httpx = "^0.23.0"
 jwt = "^1.3.1"
 nbformat = "^5.4.0"
 orjson = "^3.6.8"
-pydantic = "^1.9.1"
+pydantic = "^1.9.0"
 structlog = "^22.1.0"
 websockets = "^10.3"
 backoff = "^2.1.2"
 
 [tool.poetry.dev-dependencies]
 black = {version = "^22.3.0", allow-prereleases = true}
 isort = "^5.10.1"
```

### Comparing `noteable_origami-0.0.8/setup.py` & `noteable_origami-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 install_requires = \
 ['backoff>=2.1.2,<3.0.0',
  'bitmath>=1.3.3,<2.0.0',
  'httpx>=0.23.0,<0.24.0',
  'jwt>=1.3.1,<2.0.0',
  'nbformat>=5.4.0,<6.0.0',
  'orjson>=3.6.8,<4.0.0',
- 'pydantic>=1.9.1,<2.0.0',
+ 'pydantic>=1.9.0,<2.0.0',
  'structlog>=22.1.0,<23.0.0',
  'websockets>=10.3,<11.0']
 
 setup_kwargs = {
     'name': 'noteable-origami',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'The Noteable API interface',
     'long_description': '# Origami\nA library capturing message patterns and protocols speaking to Noteable\'s APIs\n<p align="center">\n<a href="https://github.com/noteable-io/origami/actions/workflows/ci.yaml">\n    <img src="https://github.com/noteable-io/origami/actions/workflows/ci.yaml/badge.svg" alt="CI" />\n</a>\n<a href="https://codecov.io/gh/noteable-io/origami" > \n <img src="https://codecov.io/gh/noteable-io/origami/branch/main/graph/badge.svg" alt="codecov code coverage"/> \n </a>\n<img alt="PyPI - License" src="https://img.shields.io/pypi/l/noteable-origami" />\n<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/noteable-origami" />\n<img alt="PyPI" src="https://img.shields.io/pypi/v/noteable-origami">\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n</p>\n\n---------\n\n[Install](#installation) | [Getting Started](#getting-started) | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing](./CONTRIBUTING.md)\n\n## Requirements\n\nPython 3.8+\n\n## Installation\n\n### Poetry\n\n```shell\npoetry add noteable-origami\n```\n\n\n### Pip\n```shell\npip install noteable-origami\n```\n\n## Getting Started\n\nGet your access token from https://app.noteable.world/api/token\n\n```python\nfrom origami.client import NoteableClient\n\ntoken = \'ey...\' # from https://app.noteable.world/api/token\nasync with NoteableClient(api_token=token) as client:\n    await client.ping_rtu()\n```\n\n## Contributing\n\nSee [CONTRIBUTING.md](./CONTRIBUTING.md).\n\n-------\n\n<p align="center">Open sourced with ❤️ by <a href="https://noteable.io">Noteable</a> for the community.</p>\n\n<img href="https://pages.noteable.io/private-beta-access" src="https://assets.noteable.io/github/2022-07-29/noteable.png" alt="Boost Data Collaboration with Notebooks">\n',
     'author': 'Matt Seal',
     'author_email': 'matt@noteable.io',
     'maintainer': 'Matt Seal',
     'maintainer_email': 'matt@noteable.io',
     'url': 'https://github.com/noteable-io/origami',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['origami',
 'origami.tests', 'origami.tests.types', 'origami.types'] package_data = \ {'':
 ['*']} install_requires = \ ['backoff>=2.1.2,<3.0.0', 'bitmath>=1.3.3,<2.0.0',
 'httpx>=0.23.0,<0.24.0', 'jwt>=1.3.1,<2.0.0', 'nbformat>=5.4.0,<6.0.0',
-'orjson>=3.6.8,<4.0.0', 'pydantic>=1.9.1,<2.0.0', 'structlog>=22.1.0,<23.0.0',
+'orjson>=3.6.8,<4.0.0', 'pydantic>=1.9.0,<2.0.0', 'structlog>=22.1.0,<23.0.0',
 'websockets>=10.3,<11.0'] setup_kwargs = { 'name': 'noteable-origami',
-'version': '0.0.8', 'description': 'The Noteable API interface',
+'version': '0.0.9', 'description': 'The Noteable API interface',
 'long_description': '# Origami\nA library capturing message patterns and
 protocols speaking to Noteable\'s APIs\n
  \n\n_[CI]\n\n\n_[codecov_code_coverage]_\n\n[PyPI - License]\n[PyPI - Python
                     Version]\n[PyPI]\n[Code_style:_black]\n
 \n\n---------\n\n[Install](#installation) | [Getting Started](#getting-started)
 | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) |
 [Contributing](./CONTRIBUTING.md)\n\n## Requirements\n\nPython 3.8+\n\n##
```

### Comparing `noteable_origami-0.0.8/PKG-INFO` & `noteable_origami-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteable-origami
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Noteable API interface
 Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause
 Keywords: notebook,api,noteable
 Author: Matt Seal
 Author-email: matt@noteable.io
 Maintainer: Matt Seal
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: backoff (>=2.1.2,<3.0.0)
 Requires-Dist: bitmath (>=1.3.3,<2.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: jwt (>=1.3.1,<2.0.0)
 Requires-Dist: nbformat (>=5.4.0,<6.0.0)
 Requires-Dist: orjson (>=3.6.8,<4.0.0)
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: structlog (>=22.1.0,<23.0.0)
 Requires-Dist: websockets (>=10.3,<11.0)
 Project-URL: Repository, https://github.com/noteable-io/origami
 Description-Content-Type: text/markdown
 
 # Origami
 A library capturing message patterns and protocols speaking to Noteable's APIs
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: noteable-origami Version: 0.0.8 Summary: The
+Metadata-Version: 2.1 Name: noteable-origami Version: 0.0.9 Summary: The
 Noteable API interface Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause Keywords: notebook,api,noteable Author: Matt Seal Author-
 email: matt@noteable.io Maintainer: Matt Seal Maintainer-email:
 matt@noteable.io Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: backoff
 (>=2.1.2,<3.0.0) Requires-Dist: bitmath (>=1.3.3,<2.0.0) Requires-Dist: httpx
 (>=0.23.0,<0.24.0) Requires-Dist: jwt (>=1.3.1,<2.0.0) Requires-Dist: nbformat
 (>=5.4.0,<6.0.0) Requires-Dist: orjson (>=3.6.8,<4.0.0) Requires-Dist: pydantic
-(>=1.9.1,<2.0.0) Requires-Dist: structlog (>=22.1.0,<23.0.0) Requires-Dist:
+(>=1.9.0,<2.0.0) Requires-Dist: structlog (>=22.1.0,<23.0.0) Requires-Dist:
 websockets (>=10.3,<11.0) Project-URL: Repository, https://github.com/noteable-
 io/origami Description-Content-Type: text/markdown # Origami A library
 capturing message patterns and protocols speaking to Noteable's APIs
  [CI] [codecov_code_coverage] [PyPI - License] [PyPI - Python Version] [PyPI]
                               [Code_style:_black]
 --------- [Install](#installation) | [Getting Started](#getting-started) |
 [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing]
```

