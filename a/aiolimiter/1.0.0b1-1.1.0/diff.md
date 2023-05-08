# Comparing `tmp/aiolimiter-1.0.0b1.tar.gz` & `tmp/aiolimiter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolimiter-1.0.0b1.tar", last modified: Sun Dec  1 15:52:13 2019, max compression
+gzip compressed data, was "aiolimiter-1.1.0.tar", max compression
```

## Comparing `aiolimiter-1.0.0b1.tar` & `aiolimiter-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      762 2019-12-01 15:50:51.837520 aiolimiter-1.0.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2019-12-01 15:50:51.837520 aiolimiter-1.0.0b1/LICENSE.txt
--rw-r--r--   0        0        0     3290 2019-12-01 15:50:51.837520 aiolimiter-1.0.0b1/README.md
--rw-r--r--   0        0        0     2324 2019-12-01 15:50:51.841520 aiolimiter-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      415 2019-12-01 15:50:51.841520 aiolimiter-1.0.0b1/src/aiolimiter/__init__.py
--rw-r--r--   0        0        0      594 2019-12-01 15:50:51.841520 aiolimiter-1.0.0b1/src/aiolimiter/compat.py
--rw-r--r--   0        0        0     4170 2019-12-01 15:50:51.841520 aiolimiter-1.0.0b1/src/aiolimiter/leakybucket.py
--rw-r--r--   0        0        0      113 2019-12-01 15:50:51.841520 aiolimiter-1.0.0b1/src/aiolimiter/py.typed
--rw-r--r--   0        0        0     4359 2019-12-01 15:52:13.151195 aiolimiter-1.0.0b1/setup.py
--rw-r--r--   0        0        0     4761 2019-12-01 15:52:13.151514 aiolimiter-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1355 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3294 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/README.md
+-rw-r--r--   0        0        0     2152 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/src/aiolimiter/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/src/aiolimiter/compat.py
+-rw-r--r--   0        0        0     4348 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/src/aiolimiter/leakybucket.py
+-rw-r--r--   0        0        0      113 2023-05-08 15:06:17.559435 aiolimiter-1.1.0/src/aiolimiter/py.typed
+-rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 aiolimiter-1.1.0/PKG-INFO
```

### Comparing `aiolimiter-1.0.0b1/CHANGELOG.md` & `aiolimiter-1.1.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,43 @@
     entries.
 
     WARNING: Don't drop the next directive!
 -->
 
 <!-- Towncrier release notes start -->
 
+## Aiolimiter 1.1.0 (2023-05-08)
+
+
+
+### Features
+
+- Add ``__slots__`` to the ``AsyncLimiter`` class, reducing memory requirements. ([#85](https://github.com/mjpieters/aiolimiter/issues/85))
+
+
+
+### Deprecations and Removals
+
+- Dropped support for Python 3.6 ([#62](https://github.com/mjpieters/aiolimiter/issues/62))
+
+
+
+### Misc
+
+- [#95](https://github.com/mjpieters/aiolimiter/issues/95)
+
+
+## Aiolimiter 1.0.0 (2021-10-15)
+
+### Bugfixes
+
+- Avoid warnings on Python 3.8 and up by not passing in the loop to
+  ``asyncio.wait_for()``. ([#46](https://github.com/mjpieters/aiolimiter/issues/46))
+
+
 ## Aiolimiter 1.0.0b1 (2019-12-01)
 
 ### Improved Documentation
 
 - Corrected build process to ensure CHANGELOG.md is updated on release. ([#4](https://github.com/mjpieters/aiolimiter/issues/4))
```

### Comparing `aiolimiter-1.0.0b1/LICENSE.txt` & `aiolimiter-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiolimiter-1.0.0b1/README.md` & `aiolimiter-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 
 ## Installation
 
 ```sh
 $ pip install aiolimiter
 ```
 
-The library requires Python 3.6 or newer.
+The library requires Python 3.7 or newer.
 
 ## Requirements
 
-- Python >= 3.6
+- Python >= 3.7
 
 ## License
 
 `aiolimiter` is offered under the [MIT license](./LICENSE.txt).
 
 ## Source code
 
@@ -64,15 +64,15 @@
 or have some suggestions to improve the library.
 
 ## Developer setup
 
 This project uses [poetry][] to manage dependencies, testing and releases. Make sure you have installed that tool, then run the following command to get set up:
 
 ```sh
-poetry install -E docs && poetry run doit devsetup
+poetry install --with docs && poetry run doit devsetup
 ```
 
 Apart from using `poetry run doit devsetup`, you can either use `poetry shell` to enter a shell environment with a virtualenv set up for you, or use `poetry run ...` to run commands within the virtualenv.
 
 Tests are run with `pytest` and `tox`. Releases are made with `poetry build` and `poetry publish`. Code quality is maintained with `flake8`, `black` and `mypy`, and `pre-commit` runs quick checks to maintain the standards set.
 
 A series of `doit` tasks are defined; run `poetry run doit list` (or `doit list` with `poetry shell` activated) to list them. The default action is to run a full linting, testing and building run. It is recommended you run this before creating a pull request.
```

### Comparing `aiolimiter-1.0.0b1/src/aiolimiter/leakybucket.py` & `aiolimiter-1.1.0/src/aiolimiter/leakybucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2019 Martijn Pieters
 # Licensed under the MIT license as detailed in LICENSE.txt
 
 import asyncio
+from contextlib import AbstractAsyncContextManager
 from types import TracebackType
 from typing import Dict, Optional, Type
 
-from .compat import AsyncContextManagerBase, current_task, get_running_loop
+from .compat import wait_for
 
 
-class AsyncLimiter(AsyncContextManagerBase):
+class AsyncLimiter(AbstractAsyncContextManager):
     """A leaky bucket rate limiter.
 
     This is an :ref:`asynchronous context manager <async-context-managers>`;
     when used with :keyword:`async with`, entering the context acquires
     capacity::
 
         limiter = AsyncLimiter(10)
@@ -25,29 +26,38 @@
        blocking.
     :param time_period: duration, in seconds, of the time period in which to
        limit the rate. Note that up to `max_rate` acquisitions are allowed
        within this time period in a burst.
 
     """
 
+    __slots__ = (
+        "max_rate",
+        "time_period",
+        "_rate_per_sec",
+        "_level",
+        "_last_check",
+        "_waiters",
+    )
+
     max_rate: float  #: The configured `max_rate` value for this limiter.
     time_period: float  #: The configured `time_period` value for this limiter.
 
     def __init__(self, max_rate: float, time_period: float = 60) -> None:
         self.max_rate = max_rate
         self.time_period = time_period
         self._rate_per_sec = max_rate / time_period
         self._level = 0.0
         self._last_check = 0.0
         # queue of waiting futures to signal capacity to
         self._waiters: Dict[asyncio.Task, asyncio.Future] = {}
 
     def _leak(self) -> None:
         """Drip out capacity from the bucket."""
-        loop = get_running_loop()
+        loop = asyncio.get_running_loop()
         if self._level:
             # drip out enough level for the elapsed time since
             # we last checked
             elapsed = loop.time() - self._last_check
             decrement = elapsed * self._rate_per_sec
             self._level = max(self._level - decrement, 0)
         self._last_check = loop.time()
@@ -80,25 +90,25 @@
         :exception: Raises :exc:`ValueError` if `amount` is greater than
            :attr:`max_rate`.
 
         """
         if amount > self.max_rate:
             raise ValueError("Can't acquire more than the maximum capacity")
 
-        loop = get_running_loop()
-        task = current_task(loop)
+        loop = asyncio.get_running_loop()
+        task = asyncio.current_task(loop)
         assert task is not None
         while not self.has_capacity(amount):
             # wait for the next drip to have left the bucket
             # add a future to the _waiters map to be notified
             # 'early' if capacity has come up
             fut = loop.create_future()
             self._waiters[task] = fut
             try:
-                await asyncio.wait_for(
+                await wait_for(
                     asyncio.shield(fut), 1 / self._rate_per_sec * amount, loop=loop
                 )
             except asyncio.TimeoutError:
                 pass
             fut.cancel()
         self._waiters.pop(task, None)
```

### Comparing `aiolimiter-1.0.0b1/setup.py` & `aiolimiter-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aiolimiter
+Version: 1.1.0
+Summary: asyncio rate limiter, a leaky bucket implementation
+Home-page: https://github.com/mjpieters/aiolimiter
+License: MIT
+Keywords: asyncio,rate-limiting,leaky-bucket
+Author: Martijn Pieters
+Author-email: mj@zopatista.com
+Requires-Python: >=3.7,<4.0
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib_metadata (>=1.3,<5.0) ; python_version < "3.8"
+Project-URL: CI: Azure Pipelines, https://dev.azure.com/mjpieters/aiolimiter/_build
+Project-URL: Coverage: codecov, https://codecov.io/github/aiolimiter/aiosignal
+Project-URL: Documentation, http://aiolimiter.readthedocs.org/en/stable/
+Project-URL: GitHub: issues, https://github.com/mjpieters/aiolimiter/issues
+Project-URL: Repository, https://github.com/mjpieters/aiolimiter
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# aiolimiter
 
-packages = \
-['aiolimiter']
+[![Azure Pipelines status for master branch][azure_badge]][azure_status]
+[![codecov.io status for master branch][codecov_badge]][codecov_status]
+[![Latest PyPI package version][pypi_badge]][aiolimiter_release]
+[![Latest Read The Docs][rtd_badge]][aiolimiter_docs]
 
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=0.23,<1.1.0'],
- 'docs': ['sphinx>=2.2.1,<3.0.0',
-          'aiohttp-theme>=0.1.6,<0.2.0',
-          'sphinx-autodoc-typehints>=1.10.3,<2.0.0',
-          'sphinxcontrib-spelling>=4.3.0,<5.0.0',
-          'toml>=0.10.0,<0.11.0']}
-
-setup_kwargs = {
-    'name': 'aiolimiter',
-    'version': '1.0.0b1',
-    'description': 'asyncio rate limiter, a leaky bucket implementation',
-    'long_description': '# aiolimiter\n\n[![Azure Pipelines status for master branch][azure_badge]][azure_status]\n[![codecov.io status for master branch][codecov_badge]][codecov_status]\n[![Latest PyPI package version][pypi_badge]][aiolimiter_release]\n[![Latest Read The Docs][rtd_badge]][aiolimiter_docs]\n\n[azure_badge]: https://dev.azure.com/mjpieters/aiolimiter/_apis/build/status/CI?branchName=master\n[azure_status]: https://dev.azure.com/mjpieters/aiolimiter/_build/latest?definitionId=4&branchName=master "Azure Pipelines status for master branch"\n[codecov_badge]: https://codecov.io/gh/mjpieters/aiolimiter/branch/master/graph/badge.svg\n[codecov_status]: https://codecov.io/gh/mjpieters/aiolimiter "codecov.io status for master branch"\n[pypi_badge]: https://badge.fury.io/py/aiolimiter.svg\n[aiolimiter_release]: https://pypi.org/project/aiolimiter "Latest PyPI package version"\n[rtd_badge]: https://readthedocs.org/projects/aiolimiter/badge/?version=latest\n[aiolimiter_docs]: https://aiolimiter.readthedocs.io/en/latest/?badge=latest "Latest Read The Docs"\n\n## Introduction\n\nAn efficient implementation of a rate limiter for asyncio.\n\nThis project implements the [Leaky bucket algorithm][], giving you precise control over the rate a code section can be entered:\n\n```python\nfrom aiolimiter import AsyncLimiter\n\n# allow for 100 concurrent entries within a 30 second window\nrate_limit = AsyncLimiter(100, 30)\n\n\nasync def some_coroutine():\n    async with rate_limit:\n        # this section is *at most* going to entered 100 times\n        # in a 30 second period.\n        await do_something()\n```\n\nIt was first developed [as an answer on Stack Overflow][so45502319].\n\n## Documentation\n\nhttps://aiolimiter.readthedocs.io\n\n## Installation\n\n```sh\n$ pip install aiolimiter\n```\n\nThe library requires Python 3.6 or newer.\n\n## Requirements\n\n- Python >= 3.6\n\n## License\n\n`aiolimiter` is offered under the [MIT license](./LICENSE.txt).\n\n## Source code\n\nThe project is hosted on [GitHub][].\n\nPlease file an issue in the [bug tracker][] if you have found a bug\nor have some suggestions to improve the library.\n\n## Developer setup\n\nThis project uses [poetry][] to manage dependencies, testing and releases. Make sure you have installed that tool, then run the following command to get set up:\n\n```sh\npoetry install -E docs && poetry run doit devsetup\n```\n\nApart from using `poetry run doit devsetup`, you can either use `poetry shell` to enter a shell environment with a virtualenv set up for you, or use `poetry run ...` to run commands within the virtualenv.\n\nTests are run with `pytest` and `tox`. Releases are made with `poetry build` and `poetry publish`. Code quality is maintained with `flake8`, `black` and `mypy`, and `pre-commit` runs quick checks to maintain the standards set.\n\nA series of `doit` tasks are defined; run `poetry run doit list` (or `doit list` with `poetry shell` activated) to list them. The default action is to run a full linting, testing and building run. It is recommended you run this before creating a pull request.\n\n[leaky bucket algorithm]: https://en.wikipedia.org/wiki/Leaky_bucket\n[so45502319]: https://stackoverflow.com/a/45502319/100297\n[github]: https://github.com/mjpieters/aiolimiter\n[bug tracker]: https://github.com/mjpieters/aiolimiter/issues\n[poetry]: https://poetry.eustace.io/\n',
-    'author': 'Martijn Pieters',
-    'author_email': 'mj@zopatista.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mjpieters/aiolimiter',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
-}
+[azure_badge]: https://dev.azure.com/mjpieters/aiolimiter/_apis/build/status/CI?branchName=master
+[azure_status]: https://dev.azure.com/mjpieters/aiolimiter/_build/latest?definitionId=4&branchName=master "Azure Pipelines status for master branch"
+[codecov_badge]: https://codecov.io/gh/mjpieters/aiolimiter/branch/master/graph/badge.svg
+[codecov_status]: https://codecov.io/gh/mjpieters/aiolimiter "codecov.io status for master branch"
+[pypi_badge]: https://badge.fury.io/py/aiolimiter.svg
+[aiolimiter_release]: https://pypi.org/project/aiolimiter "Latest PyPI package version"
+[rtd_badge]: https://readthedocs.org/projects/aiolimiter/badge/?version=latest
+[aiolimiter_docs]: https://aiolimiter.readthedocs.io/en/latest/?badge=latest "Latest Read The Docs"
 
+## Introduction
+
+An efficient implementation of a rate limiter for asyncio.
+
+This project implements the [Leaky bucket algorithm][], giving you precise control over the rate a code section can be entered:
+
+```python
+from aiolimiter import AsyncLimiter
+
+# allow for 100 concurrent entries within a 30 second window
+rate_limit = AsyncLimiter(100, 30)
+
+
+async def some_coroutine():
+    async with rate_limit:
+        # this section is *at most* going to entered 100 times
+        # in a 30 second period.
+        await do_something()
+```
+
+It was first developed [as an answer on Stack Overflow][so45502319].
+
+## Documentation
+
+https://aiolimiter.readthedocs.io
+
+## Installation
+
+```sh
+$ pip install aiolimiter
+```
+
+The library requires Python 3.7 or newer.
+
+## Requirements
+
+- Python >= 3.7
+
+## License
+
+`aiolimiter` is offered under the [MIT license](./LICENSE.txt).
+
+## Source code
+
+The project is hosted on [GitHub][].
+
+Please file an issue in the [bug tracker][] if you have found a bug
+or have some suggestions to improve the library.
+
+## Developer setup
+
+This project uses [poetry][] to manage dependencies, testing and releases. Make sure you have installed that tool, then run the following command to get set up:
+
+```sh
+poetry install --with docs && poetry run doit devsetup
+```
+
+Apart from using `poetry run doit devsetup`, you can either use `poetry shell` to enter a shell environment with a virtualenv set up for you, or use `poetry run ...` to run commands within the virtualenv.
+
+Tests are run with `pytest` and `tox`. Releases are made with `poetry build` and `poetry publish`. Code quality is maintained with `flake8`, `black` and `mypy`, and `pre-commit` runs quick checks to maintain the standards set.
+
+A series of `doit` tasks are defined; run `poetry run doit list` (or `doit list` with `poetry shell` activated) to list them. The default action is to run a full linting, testing and building run. It is recommended you run this before creating a pull request.
+
+[leaky bucket algorithm]: https://en.wikipedia.org/wiki/Leaky_bucket
+[so45502319]: https://stackoverflow.com/a/45502319/100297
+[github]: https://github.com/mjpieters/aiolimiter
+[bug tracker]: https://github.com/mjpieters/aiolimiter/issues
+[poetry]: https://poetry.eustace.io/
 
-setup(**setup_kwargs)
```

