# Comparing `tmp/python_opensky-0.0.4.tar.gz` & `tmp/python_opensky-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.0.4.tar", max compression
+gzip compressed data, was "python_opensky-0.0.5.tar", max compression
```

## Comparing `python_opensky-0.0.4.tar` & `python_opensky-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-05-07 21:55:50.807930 python_opensky-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     5339 2023-05-07 21:55:50.807930 python_opensky-0.0.4/README.md
--rw-r--r--   0        0        0     3659 2023-05-07 21:56:19.087712 python_opensky-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      444 2023-05-07 21:55:50.807930 python_opensky-0.0.4/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      753 2023-05-07 21:55:50.807930 python_opensky-0.0.4/src/python_opensky/const.py
--rw-r--r--   0        0        0      202 2023-05-07 21:55:50.807930 python_opensky-0.0.4/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     2822 2023-05-07 21:55:50.807930 python_opensky-0.0.4/src/python_opensky/models.py
--rw-r--r--   0        0        0     4499 2023-05-07 21:55:50.807930 python_opensky-0.0.4/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-05-07 21:55:50.807930 python_opensky-0.0.4/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6741 1970-01-01 00:00:00.000000 python_opensky-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-07 22:20:29.800087 python_opensky-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     5324 2023-05-07 22:20:29.800087 python_opensky-0.0.5/README.md
+-rw-r--r--   0        0        0     3659 2023-05-07 22:20:51.844076 python_opensky-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      753 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/const.py
+-rw-r--r--   0        0        0      202 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     2822 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/models.py
+-rw-r--r--   0        0        0     4499 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6726 1970-01-01 00:00:00.000000 python_opensky-0.0.5/PKG-INFO
```

### Comparing `python_opensky-0.0.4/LICENSE.md` & `python_opensky-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.4/README.md` & `python_opensky-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE.md)
 
 [![Build Status][build-shield]][build]
 [![Code Coverage][codecov-shield]][codecov]
-[![Code Quality][code-quality-shield]][code-quality]
+[![Code Smells][code-smells]][sonarcloud]
 
 Asynchronous Python client for the OpenSky API.
 
 ## About
 
 This package allows you to request data about aircraft around the world.
 
 ## Installation
 
 ```bash
-pip install python_opensky
+pip install python-opensky
 ```
 
 ## Usage
 
 ```python
 import asyncio
 
@@ -125,30 +125,30 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
-[build-shield]: https://github.com/joostlek/python-opensky/workflows/Continuous%20Integration/badge.svg
+[build-shield]: https://github.com/joostlek/python-opensky/actions/workflows/tests.yaml/badge.svg
 [build]: https://github.com/joostlek/python-opensky/actions
-[code-quality-shield]: https://img.shields.io/lgtm/grade/python/g/joostlek/python-opensky.svg?logo=lgtm&logoWidth=18
-[code-quality]: https://lgtm.com/projects/g/joostlek/python-opensky/context:python
+[code-smells]: https://sonarcloud.io/api/project_badges/measure?project=joostlek_python-opensky&metric=code_smells
 [codecov-shield]: https://codecov.io/gh/joostlek/python-opensky/branch/master/graph/badge.svg
 [codecov]: https://codecov.io/gh/joostlek/python-opensky
 [commits-shield]: https://img.shields.io/github/commit-activity/y/joostlek/python-opensky.svg
 [commits]: https://github.com/joostlek/python-opensky/commits/master
 [contributors]: https://github.com/joostlek/python-opensky/graphs/contributors
 [frenck]: https://github.com/frenck
 [joostlek]: https://github.com/joostlek
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/joostlek/python-opensky.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
-[python-versions-shield]: https://img.shields.io/pypi/pyversions/opensky
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/python-opensky
 [releases-shield]: https://img.shields.io/github/release/joostlek/python-opensky.svg
 [releases]: https://github.com/joostlek/python-opensky/releases
 [semver]: http://semver.org/spec/v2.0.0.html
-[pypi]: https://pypi.org/project/python_opensky/
+[sonarcloud]: https://sonarcloud.io/summary/new_code?id=joostlek_python-opensky
+[pypi]: https://pypi.org/project/python-opensky/
```

### Comparing `python_opensky-0.0.4/pyproject.toml` & `python_opensky-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.0.4"
+version = "0.0.5"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
```

### Comparing `python_opensky-0.0.4/src/python_opensky/const.py` & `python_opensky-0.0.5/src/python_opensky/const.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.4/src/python_opensky/models.py` & `python_opensky-0.0.5/src/python_opensky/models.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.4/src/python_opensky/opensky.py` & `python_opensky-0.0.5/src/python_opensky/opensky.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.4/PKG-INFO` & `python_opensky-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -37,26 +37,26 @@
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE.md)
 
 [![Build Status][build-shield]][build]
 [![Code Coverage][codecov-shield]][codecov]
-[![Code Quality][code-quality-shield]][code-quality]
+[![Code Smells][code-smells]][sonarcloud]
 
 Asynchronous Python client for the OpenSky API.
 
 ## About
 
 This package allows you to request data about aircraft around the world.
 
 ## Installation
 
 ```bash
-pip install python_opensky
+pip install python-opensky
 ```
 
 ## Usage
 
 ```python
 import asyncio
 
@@ -158,31 +158,31 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
-[build-shield]: https://github.com/joostlek/python-opensky/workflows/Continuous%20Integration/badge.svg
+[build-shield]: https://github.com/joostlek/python-opensky/actions/workflows/tests.yaml/badge.svg
 [build]: https://github.com/joostlek/python-opensky/actions
-[code-quality-shield]: https://img.shields.io/lgtm/grade/python/g/joostlek/python-opensky.svg?logo=lgtm&logoWidth=18
-[code-quality]: https://lgtm.com/projects/g/joostlek/python-opensky/context:python
+[code-smells]: https://sonarcloud.io/api/project_badges/measure?project=joostlek_python-opensky&metric=code_smells
 [codecov-shield]: https://codecov.io/gh/joostlek/python-opensky/branch/master/graph/badge.svg
 [codecov]: https://codecov.io/gh/joostlek/python-opensky
 [commits-shield]: https://img.shields.io/github/commit-activity/y/joostlek/python-opensky.svg
 [commits]: https://github.com/joostlek/python-opensky/commits/master
 [contributors]: https://github.com/joostlek/python-opensky/graphs/contributors
 [frenck]: https://github.com/frenck
 [joostlek]: https://github.com/joostlek
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/joostlek/python-opensky.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
-[python-versions-shield]: https://img.shields.io/pypi/pyversions/opensky
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/python-opensky
 [releases-shield]: https://img.shields.io/github/release/joostlek/python-opensky.svg
 [releases]: https://github.com/joostlek/python-opensky/releases
 [semver]: http://semver.org/spec/v2.0.0.html
-[pypi]: https://pypi.org/project/python_opensky/
+[sonarcloud]: https://sonarcloud.io/summary/new_code?id=joostlek_python-opensky
+[pypi]: https://pypi.org/project/python-opensky/
```

