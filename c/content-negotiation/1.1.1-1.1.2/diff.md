# Comparing `tmp/content-negotiation-1.1.1.tar.gz` & `tmp/content-negotiation-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "content-negotiation-1.1.1.tar", max compression
+gzip compressed data, was "content-negotiation-1.1.2.tar", max compression
```

## Comparing `content-negotiation-1.1.1.tar` & `content-negotiation-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2022-09-12 11:17:43.441145 content-negotiation-1.1.1/LICENSE
--rw-r--r--   0        0        0     3468 2022-09-12 11:17:43.441145 content-negotiation-1.1.1/README.md
--rw-r--r--   0        0        0     1919 2022-09-12 11:17:43.445145 content-negotiation-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      612 2022-09-12 11:17:43.445145 content-negotiation-1.1.1/src/content_negotiation/__init__.py
--rw-r--r--   0        0        0     8662 2022-09-12 11:17:43.445145 content-negotiation-1.1.1/src/content_negotiation/content_negotiation.py
--rw-r--r--   0        0        0     6392 2022-09-12 11:17:43.445145 content-negotiation-1.1.1/src/content_negotiation/language_negotiation.py
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 content-negotiation-1.1.1/setup.py
--rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 content-negotiation-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 08:05:32.477626 content-negotiation-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3468 2023-05-08 08:05:32.477626 content-negotiation-1.1.2/README.md
+-rw-r--r--   0        0        0     1953 2023-05-08 08:05:32.477626 content-negotiation-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      612 2023-05-08 08:05:32.477626 content-negotiation-1.1.2/src/content_negotiation/__init__.py
+-rw-r--r--   0        0        0     8662 2023-05-08 08:05:32.477626 content-negotiation-1.1.2/src/content_negotiation/content_negotiation.py
+-rw-r--r--   0        0        0     6392 2023-05-08 08:05:32.477626 content-negotiation-1.1.2/src/content_negotiation/language_negotiation.py
+-rw-r--r--   0        0        0     4302 1970-01-01 00:00:00.000000 content-negotiation-1.1.2/setup.py
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 content-negotiation-1.1.2/PKG-INFO
```

### Comparing `content-negotiation-1.1.1/LICENSE` & `content-negotiation-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `content-negotiation-1.1.1/README.md` & `content-negotiation-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `content-negotiation-1.1.1/pyproject.toml` & `content-negotiation-1.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 description = "A library for deciding content-type based on media ranges in HTTP Accept headers."
 documentation = "https://content-negotiation.readthedocs.io"
 homepage = "https://github.com/Informasjonsforvaltning/content-negotiation"
 license = "Apache-2.0"
 name = "content-negotiation"
 readme = "README.md"
 repository = "https://github.com/Informasjonsforvaltning/content-negotiation"
-version = "1.1.1"
+version = "1.1.2"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^5.0.1"
 bandit = "^1.7.4"
 black = "^22.1.0"
 codecov = "^2.0.16"
 coverage = "^6.4"
@@ -33,15 +33,15 @@
 flake8-import-order = "^0.18.1"
 mypy = "^0.971"
 nox = "^2022.1.7"
 nox-poetry = "^1.0.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.6.1"
-pytype = "^2022.8.30"
+pytype = {version= "^2022.8.30", python = ">=3.8,<3.11"}
 safety = "^2.1.1"
 sphinx-autodoc-typehints = "^1.11.1"
 sphinxcontrib-napoleon = "^0.7"
 xdoctest = "^1.0.0"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `content-negotiation-1.1.1/src/content_negotiation/__init__.py` & `content-negotiation-1.1.2/src/content_negotiation/__init__.py`

 * *Files identical despite different names*

### Comparing `content-negotiation-1.1.1/src/content_negotiation/content_negotiation.py` & `content-negotiation-1.1.2/src/content_negotiation/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `content-negotiation-1.1.1/src/content_negotiation/language_negotiation.py` & `content-negotiation-1.1.2/src/content_negotiation/language_negotiation.py`

 * *Files identical despite different names*

### Comparing `content-negotiation-1.1.1/setup.py` & `content-negotiation-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ['content_negotiation']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'content-negotiation',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'A library for deciding content-type based on media ranges in HTTP Accept headers.',
     'long_description': '# content-negotiation\n\n![Tests](https://github.com/Informasjonsforvaltning/content-negotiation/workflows/Tests/badge.svg)\n[![codecov](https://codecov.io/gh/Informasjonsforvaltning/content-negotiation/branch/master/graph/badge.svg)](https://codecov.io/gh/Informasjonsforvaltning/content-negotiation)\n[![PyPI](https://img.shields.io/pypi/v/content-negotiation.svg)](https://pypi.org/project/content-negotiation/)\n[![Read the Docs](https://readthedocs.org/projects/content-negotiation/badge/)](https://content-negotiation.readthedocs.io/)\n\nA small Python library supporting content-negotiation.\n\nIt is used to decide content type based on a list of media ranges in the accept header, as well as deciding content-language based on the accept-language header.\n\n* Media ranges/language ranges with a q-value of 0.0 will be ignored.\n* Q-values above 1.0 will be treated as 1.0. Q-values below 0.0 will be treated as 0.0.\n* When a media range is not specified, it will be treated as `*/*`.\n* When a language range is not specified, it will be treated as `*`.\n* When media ranges and language ranges are equal, the first one will be returned.\n\nFor more information on the accept header, see [RFC 7231, section-5.3.2](https://tools.ietf.org/html/rfc7231#section-5.3.2).\nFor more information on the accept-language header, see [RFC 7231, section-5.3.5](https://www.rfc-editor.org/rfc/rfc7231#section-5.3.5)\n\n## Usage\n\n### Install\n\n```Shell\n% pip install content-negotiation\n```\n\n### Getting started\n\n#### Content type\n\n```Python\nfrom content_negotiation import decide_content_type, NoAgreeableContentTypeError\n\naccept_headers = ["application/json", "text/html", "text/plain, text/*;q=0.8"]\nsupported_content_types = ["text/turtle", "application/json"]\n\ntry:\n    content_type = decide_content_type(accept_headers, supported_content_types)\nexcept NoAgreeableContentTypeError:\n    print("No agreeable content type found.")\n    # Handle error, by returning e.g. 406 Not Acceptable\n```\n\n#### Content language\n\n```Python\nfrom content_negotiation import decide_content_language, NoAgreeableContentLanguageError\n\naccept_language_headers = ["en-GB;q=0.8", "nb-NO;q=0.9"]\n   supported_languages = ["en-GB", "en", "nb-NO", "nb", "en-US"]\n\ntry:\n    content_language = decide_decide_language(accept_language_headers, supported_languages)\nexcept NoAgreeableLanguageError:\n    print("No agreeable language found.")\n    # Handle error, by returning e.g. 406 Not Acceptable\n```\n\n## Development\n\n### Requirements\n\n* [pyenv](https://github.com/pyenv/pyenv) (recommended)\n* python3\n* [pipx](https://github.com/pipxproject/pipx) (recommended)\n* [poetry](https://python-poetry.org/) # version v1.2.0 or higher\n* [nox](https://nox.thea.codes/en/stable/)\n\n```Shell\n% pipx install poetry==1.2.0\n% pipx install nox==2022.8.7\n% pipx inject nox nox-poetry==1.0.1\n```\n\n### Install developer tools\n\n```Shell\n% git clone https://github.com/Informasjonsforvaltning/content-negotiation.git\n% cd content-negotiation\n% pyenv install 3.8.13\n% pyenv install 3.9.13\n% pyenv install 3.10.6\n% pyenv local 3.8.13 3.9.13 3.10.6\n% poetry install\n```\n\n### Run all sessions\n\n```Shell\n% nox\n```\n\n### Run all tests with coverage reporting\n\n```Shell\n% nox -rs tests\n```\n\n### Debugging\n\nYou can enter into [Pdb](https://docs.python.org/3/library/pdb.html) by passing `--pdb` to pytest:\n\n```Shell\n% nox -rs tests -- --pdb  --log-cli-level=DEBUG\n```\n\nYou can set breakpoints directly in code by using the function `breakpoint()`.\n',
     'author': 'Stig B. Dørmænen',
     'author_email': 'stigbd@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Informasjonsforvaltning/content-negotiation',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `content-negotiation-1.1.1/PKG-INFO` & `content-negotiation-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: content-negotiation
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library for deciding content-type based on media ranges in HTTP Accept headers.
 Home-page: https://github.com/Informasjonsforvaltning/content-negotiation
 License: Apache-2.0
 Author: Stig B. Dørmænen
 Author-email: stigbd@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
```

