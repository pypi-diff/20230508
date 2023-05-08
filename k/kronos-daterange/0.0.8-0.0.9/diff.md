# Comparing `tmp/kronos-daterange-0.0.8.tar.gz` & `tmp/kronos-daterange-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kronos-daterange-0.0.8.tar", max compression
+gzip compressed data, was "kronos-daterange-0.0.9.tar", max compression
```

## Comparing `kronos-daterange-0.0.8.tar` & `kronos-daterange-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1514 2022-04-29 00:36:00.635208 kronos-daterange-0.0.8/LICENSE.rst
--rw-r--r--   0        0        0     4130 2022-11-09 01:11:45.598701 kronos-daterange-0.0.8/README.md
--rw-r--r--   0        0        0     2711 2023-02-07 00:27:15.934407 kronos-daterange-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      229 2023-02-07 00:26:12.601948 kronos-daterange-0.0.8/src/kronos/__init__.py
--rw-r--r--   0        0        0    14221 2023-02-07 00:19:15.670294 kronos-daterange-0.0.8/src/kronos/kronos.py
--rw-r--r--   0        0        0     7837 2022-11-12 00:24:02.861696 kronos-daterange-0.0.8/src/kronos/utilities.py
--rw-r--r--   0        0        0     5044 2023-02-07 00:27:23.485743 kronos-daterange-0.0.8/setup.py
--rw-r--r--   0        0        0     5158 2023-02-07 00:27:23.486133 kronos-daterange-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-04-29 00:36:00.635208 kronos-daterange-0.0.9/LICENSE.rst
+-rw-r--r--   0        0        0     4168 2023-02-11 19:21:33.903842 kronos-daterange-0.0.9/README.md
+-rw-r--r--   0        0        0     2711 2023-02-11 19:21:33.904202 kronos-daterange-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      229 2023-02-11 19:21:33.904576 kronos-daterange-0.0.9/src/kronos/__init__.py
+-rw-r--r--   0        0        0    14238 2023-02-11 19:21:33.905032 kronos-daterange-0.0.9/src/kronos/kronos.py
+-rw-r--r--   0        0        0     7837 2022-11-12 00:24:02.861696 kronos-daterange-0.0.9/src/kronos/utilities.py
+-rw-r--r--   0        0        0     5092 2023-02-11 19:22:31.690934 kronos-daterange-0.0.9/setup.py
+-rw-r--r--   0        0        0     5196 2023-02-11 19:22:31.691436 kronos-daterange-0.0.9/PKG-INFO
```

### Comparing `kronos-daterange-0.0.8/LICENSE.rst` & `kronos-daterange-0.0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `kronos-daterange-0.0.8/README.md` & `kronos-daterange-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,36 @@
 Kronos makes dateranges easier.
 
 
 * GitHub repo: <https://github.com/nat5142/kronos.git>
 * Documentation: <https://nat5142-kronos.readthedocs.io/>
 * Free software: BSD
 
+<br>
 
 ## Quickstart
+---
 
 Install from pip:
 
 ```shell
 pip install kronos-daterange
 ```
 
 Import & basic init:
 ```python
 from kronos import Kronos
 
 kronos = Kronos(start_date='2022-01-01', end_date='2022-01-31')
 ```
 
+<br>
 
 ## Feature Demo
+---
 
 ```python
 # import
 from kronos import Kronos
 
 # init --> defaults to range of <yesterday, today> unless otherwise specified by `KRONOS_DATERANGE` environment variable
 kronos = Kronos()
@@ -94,15 +98,18 @@
 
 # relative shift forward/back
 kronos = Kronos()
 kronos.shift_range(weeks=-1)  # pipes kwargs into timedelta
 # Kronos(start_date='2022-10-12', end_date='2022-10-13', ... )
 ```
 
+<br>
+
 ## Defaults/Environment Variables
+---
 
 Kronos is prepared to accept the following environment variables:
 
 - `KRONOS_TIMEZONE`, which defaults to UTC if not set. Can often be overridden at method-levels for one-off timezone conversions.
 - `KRONOS_FORMAT`, the strptime date format string for your dates.
 - `KRONOS_DATERANGE` (see below)
 
@@ -119,13 +126,16 @@
 - `LATEST`: start/end dates of yesterady/today
 - `YESTERDAY_TODAY`: same as `LATEST`
 - `LAST_MONTH`: previous calendar month
 - `MTD`: month-to-date
 - `LAST_{X}_DAYS`: relative range where end_date is today, start date is set X days behind.
 - `THIS_WEEK__{X}`: week-to-date starting on previous day of week specified by X. Valid values for X: `SUN, MON, TUES, WED, THURS, FRI, SAT`
 
+<br>
+
 ## Credits
+---
 
 This package was created with [Cookiecutter][cookiecutter] and the [fedejaure/cookiecutter-modern-pypackage][cookiecutter-modern-pypackage] project template.
 
 [cookiecutter]: https://github.com/cookiecutter/cookiecutter
 [cookiecutter-modern-pypackage]: https://github.com/fedejaure/cookiecutter-modern-pypackage
```

### Comparing `kronos-daterange-0.0.8/pyproject.toml` & `kronos-daterange-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "kronos-daterange"
-version = "0.0.8"
+version = "0.0.9"
 description = "Kronos makes date ranges easier."
 authors = ["Nick Tulli <ntulli.dev@gmail.com>"]
 
 readme = "README.md"
 homepage = "https://github.com/nat5142/kronos"
 repository = "https://github.com/nat5142/kronos"
 documentation = "https://nat5142-kronos.readthedocs.io/"
```

### Comparing `kronos-daterange-0.0.8/src/kronos/kronos.py` & `kronos-daterange-0.0.9/src/kronos/kronos.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,21 +237,21 @@
             tz = make_timezone(timezone=timezone)
         else:
             tz = self.tz
 
         return datetime.now(tz=tz)
 
     def last_x_days(self, x: int = 30) -> Kronos:
-        """Get the last `x` days since today.
+        """ Get the last `x` days since today.
 
         :param x: number of days to go back, defaults to 30
         :type x: int, optional
         """
         start_date = self.now() - timedelta(days=x)
-        return Kronos(start_date=start_date.strftime('%Y-%m-%d'), end_date=self.now().strftime('%Y-%m-%d'))
+        return self.__class__(start_date=start_date.strftime('%Y-%m-%d'), end_date=self.now().strftime('%Y-%m-%d'))
     
     def list_date_range(self) -> List[datetime]:
         """ List all dates in the Kronos daterange as datetime objects.
 
         :return: a list of each day in the range
         :rtype: List[datetime]
         """
@@ -299,14 +299,14 @@
 
         :param kwargs: key-value pairs to be deconstructed into timedelta(...) kwargs.
         :return: a timedelta-shifted Kronos object.
         :rtype: Kronos
         """
         new_start = (self._start_date + timedelta(**kwargs)).strftime(self.date_format)
         new_end = (self._end_date + timedelta(**kwargs)).strftime(self.date_format)
-        return Kronos(new_start, new_end)
+        return self.__class__(new_start, new_end)
 
     def __repr__(self):
         return "Kronos(start_date='{}', end_date='{}', date_format='{}', timezone='{}')".format(
             self.start_date, self.end_date, self.date_format, self.tz.zone
         )
```

### Comparing `kronos-daterange-0.0.8/src/kronos/utilities.py` & `kronos-daterange-0.0.9/src/kronos/utilities.py`

 * *Files identical despite different names*

### Comparing `kronos-daterange-0.0.8/setup.py` & `kronos-daterange-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['python-dotenv>=0.21.0,<0.22.0', 'pytz>=2022.1,<2023.0']
 
 setup_kwargs = {
     'name': 'kronos-daterange',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Kronos makes date ranges easier.',
-    'long_description': '\n# Kronos\n\n\n<div align="center">\n\n[![PyPI - Version](https://img.shields.io/pypi/v/kronos-daterange.svg)](https://pypi.python.org/pypi/kronos-daterange)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kronos-daterange.svg)](https://pypi.python.org/pypi/kronos-daterange)\n[![Tests](https://github.com/nat5142/kronos/workflows/tests/badge.svg)](https://github.com/nat5142/kronos/actions?workflow=tests)\n[![Codecov](https://codecov.io/gh/nat5142/kronos/branch/main/graph/badge.svg)](https://codecov.io/gh/nat5142/kronos)\n[![Read the Docs](https://readthedocs.org/projects/nat5142-kronos/badge/)](https://kronos.readthedocs.io/)\n[![PyPI - License](https://img.shields.io/pypi/l/kronos-daterange.svg)](https://pypi.python.org/pypi/kronos-daterange)\n\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n\n</div>\n\n\nKronos makes dateranges easier.\n\n\n* GitHub repo: <https://github.com/nat5142/kronos.git>\n* Documentation: <https://nat5142-kronos.readthedocs.io/>\n* Free software: BSD\n\n\n## Quickstart\n\nInstall from pip:\n\n```shell\npip install kronos-daterange\n```\n\nImport & basic init:\n```python\nfrom kronos import Kronos\n\nkronos = Kronos(start_date=\'2022-01-01\', end_date=\'2022-01-31\')\n```\n\n\n## Feature Demo\n\n```python\n# import\nfrom kronos import Kronos\n\n# init --> defaults to range of <yesterday, today> unless otherwise specified by `KRONOS_DATERANGE` environment variable\nkronos = Kronos()\n\n# manually set dates\nkronos = Kronos(start_date=\'2022-10-17\', end_date=\'2022-10-23\')\n\n# set timezone\nkronos = Kronos(timezone=\'America/New_York\') \n\n# specify date format\nkronos = Kronos(start_date=\'10/20/2022\', end_date=\'10/31/2022\', date_format=\'%m/%d/%Y\')\n\n# access start, end dates\nkronos = Kronos()\nkronos.start_date\n# 2022-10-19\nkronos.end_date\n# 2022-10-20\n\n# `date_format` carries over to properties:\nkronos = Kronos(date_format=\'%m/%d/%Y\')\nkronos.start_date\n# 10/19/2022\nkronos.end_date\n# 10/20/2022\n\n# format start and end date with new format\nkronos.format_start(\'%Y-%m-%d %H:%M:%S\')\n# 2022-10-20 00:00:00\nkronos.format_end(\'%Y-%m-%d %H:%M:%S\')\n# 2022-10-21 23:59:59\n\n# get the current date in specified timezone\nkronos = Kronos(\'America/Los_Angeles\')\nkronos.current_date\n# 2022-10-20\nkronos = Kronos(\'America/Los_Angeles\', date_format=\'%m/%d/%Y\')\nkronos.current_date\n# 10/20/2022\n\n# overwrite your object\'s timezone without altering the time\nkronos = Kronos(timezone=\'UTC\')\nkronos.change_timezone(tz=\'America/New_York\')\n\n# relative shift forward/back\nkronos = Kronos()\nkronos.shift_range(weeks=-1)  # pipes kwargs into timedelta\n# Kronos(start_date=\'2022-10-12\', end_date=\'2022-10-13\', ... )\n```\n\n## Defaults/Environment Variables\n\nKronos is prepared to accept the following environment variables:\n\n- `KRONOS_TIMEZONE`, which defaults to UTC if not set. Can often be overridden at method-levels for one-off timezone conversions.\n- `KRONOS_FORMAT`, the strptime date format string for your dates.\n- `KRONOS_DATERANGE` (see below)\n\nNote that both `KRONOS_TIMEZONE` and `KRONOS_FORMAT` can be set during init as `timezone=` and `date_format=` arguments, respectively.\n\n### `KRONOS_TIMEZONE`:\n\nCan be any valid timezone name (find them at `pytz.all_timezones`)\n\n### `KRONOS_DATERANGE`:\n\nList of accepted values:\n\n- `LATEST`: start/end dates of yesterady/today\n- `YESTERDAY_TODAY`: same as `LATEST`\n- `LAST_MONTH`: previous calendar month\n- `MTD`: month-to-date\n- `LAST_{X}_DAYS`: relative range where end_date is today, start date is set X days behind.\n- `THIS_WEEK__{X}`: week-to-date starting on previous day of week specified by X. Valid values for X: `SUN, MON, TUES, WED, THURS, FRI, SAT`\n\n## Credits\n\nThis package was created with [Cookiecutter][cookiecutter] and the [fedejaure/cookiecutter-modern-pypackage][cookiecutter-modern-pypackage] project template.\n\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[cookiecutter-modern-pypackage]: https://github.com/fedejaure/cookiecutter-modern-pypackage\n',
+    'long_description': '\n# Kronos\n\n\n<div align="center">\n\n[![PyPI - Version](https://img.shields.io/pypi/v/kronos-daterange.svg)](https://pypi.python.org/pypi/kronos-daterange)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kronos-daterange.svg)](https://pypi.python.org/pypi/kronos-daterange)\n[![Tests](https://github.com/nat5142/kronos/workflows/tests/badge.svg)](https://github.com/nat5142/kronos/actions?workflow=tests)\n[![Codecov](https://codecov.io/gh/nat5142/kronos/branch/main/graph/badge.svg)](https://codecov.io/gh/nat5142/kronos)\n[![Read the Docs](https://readthedocs.org/projects/nat5142-kronos/badge/)](https://kronos.readthedocs.io/)\n[![PyPI - License](https://img.shields.io/pypi/l/kronos-daterange.svg)](https://pypi.python.org/pypi/kronos-daterange)\n\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n\n</div>\n\n\nKronos makes dateranges easier.\n\n\n* GitHub repo: <https://github.com/nat5142/kronos.git>\n* Documentation: <https://nat5142-kronos.readthedocs.io/>\n* Free software: BSD\n\n<br>\n\n## Quickstart\n---\n\nInstall from pip:\n\n```shell\npip install kronos-daterange\n```\n\nImport & basic init:\n```python\nfrom kronos import Kronos\n\nkronos = Kronos(start_date=\'2022-01-01\', end_date=\'2022-01-31\')\n```\n\n<br>\n\n## Feature Demo\n---\n\n```python\n# import\nfrom kronos import Kronos\n\n# init --> defaults to range of <yesterday, today> unless otherwise specified by `KRONOS_DATERANGE` environment variable\nkronos = Kronos()\n\n# manually set dates\nkronos = Kronos(start_date=\'2022-10-17\', end_date=\'2022-10-23\')\n\n# set timezone\nkronos = Kronos(timezone=\'America/New_York\') \n\n# specify date format\nkronos = Kronos(start_date=\'10/20/2022\', end_date=\'10/31/2022\', date_format=\'%m/%d/%Y\')\n\n# access start, end dates\nkronos = Kronos()\nkronos.start_date\n# 2022-10-19\nkronos.end_date\n# 2022-10-20\n\n# `date_format` carries over to properties:\nkronos = Kronos(date_format=\'%m/%d/%Y\')\nkronos.start_date\n# 10/19/2022\nkronos.end_date\n# 10/20/2022\n\n# format start and end date with new format\nkronos.format_start(\'%Y-%m-%d %H:%M:%S\')\n# 2022-10-20 00:00:00\nkronos.format_end(\'%Y-%m-%d %H:%M:%S\')\n# 2022-10-21 23:59:59\n\n# get the current date in specified timezone\nkronos = Kronos(\'America/Los_Angeles\')\nkronos.current_date\n# 2022-10-20\nkronos = Kronos(\'America/Los_Angeles\', date_format=\'%m/%d/%Y\')\nkronos.current_date\n# 10/20/2022\n\n# overwrite your object\'s timezone without altering the time\nkronos = Kronos(timezone=\'UTC\')\nkronos.change_timezone(tz=\'America/New_York\')\n\n# relative shift forward/back\nkronos = Kronos()\nkronos.shift_range(weeks=-1)  # pipes kwargs into timedelta\n# Kronos(start_date=\'2022-10-12\', end_date=\'2022-10-13\', ... )\n```\n\n<br>\n\n## Defaults/Environment Variables\n---\n\nKronos is prepared to accept the following environment variables:\n\n- `KRONOS_TIMEZONE`, which defaults to UTC if not set. Can often be overridden at method-levels for one-off timezone conversions.\n- `KRONOS_FORMAT`, the strptime date format string for your dates.\n- `KRONOS_DATERANGE` (see below)\n\nNote that both `KRONOS_TIMEZONE` and `KRONOS_FORMAT` can be set during init as `timezone=` and `date_format=` arguments, respectively.\n\n### `KRONOS_TIMEZONE`:\n\nCan be any valid timezone name (find them at `pytz.all_timezones`)\n\n### `KRONOS_DATERANGE`:\n\nList of accepted values:\n\n- `LATEST`: start/end dates of yesterady/today\n- `YESTERDAY_TODAY`: same as `LATEST`\n- `LAST_MONTH`: previous calendar month\n- `MTD`: month-to-date\n- `LAST_{X}_DAYS`: relative range where end_date is today, start date is set X days behind.\n- `THIS_WEEK__{X}`: week-to-date starting on previous day of week specified by X. Valid values for X: `SUN, MON, TUES, WED, THURS, FRI, SAT`\n\n<br>\n\n## Credits\n---\n\nThis package was created with [Cookiecutter][cookiecutter] and the [fedejaure/cookiecutter-modern-pypackage][cookiecutter-modern-pypackage] project template.\n\n[cookiecutter]: https://github.com/cookiecutter/cookiecutter\n[cookiecutter-modern-pypackage]: https://github.com/fedejaure/cookiecutter-modern-pypackage\n',
     'author': 'Nick Tulli',
     'author_email': 'ntulli.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/nat5142/kronos',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `kronos-daterange-0.0.8/PKG-INFO` & `kronos-daterange-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kronos-daterange
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kronos makes date ranges easier.
 Home-page: https://github.com/nat5142/kronos
 Keywords: kronos,kronos-daterange,daterange
 Author: Nick Tulli
 Author-email: ntulli.dev@gmail.com
 Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -46,32 +46,36 @@
 Kronos makes dateranges easier.
 
 
 * GitHub repo: <https://github.com/nat5142/kronos.git>
 * Documentation: <https://nat5142-kronos.readthedocs.io/>
 * Free software: BSD
 
+<br>
 
 ## Quickstart
+---
 
 Install from pip:
 
 ```shell
 pip install kronos-daterange
 ```
 
 Import & basic init:
 ```python
 from kronos import Kronos
 
 kronos = Kronos(start_date='2022-01-01', end_date='2022-01-31')
 ```
 
+<br>
 
 ## Feature Demo
+---
 
 ```python
 # import
 from kronos import Kronos
 
 # init --> defaults to range of <yesterday, today> unless otherwise specified by `KRONOS_DATERANGE` environment variable
 kronos = Kronos()
@@ -119,15 +123,18 @@
 
 # relative shift forward/back
 kronos = Kronos()
 kronos.shift_range(weeks=-1)  # pipes kwargs into timedelta
 # Kronos(start_date='2022-10-12', end_date='2022-10-13', ... )
 ```
 
+<br>
+
 ## Defaults/Environment Variables
+---
 
 Kronos is prepared to accept the following environment variables:
 
 - `KRONOS_TIMEZONE`, which defaults to UTC if not set. Can often be overridden at method-levels for one-off timezone conversions.
 - `KRONOS_FORMAT`, the strptime date format string for your dates.
 - `KRONOS_DATERANGE` (see below)
 
@@ -144,14 +151,17 @@
 - `LATEST`: start/end dates of yesterady/today
 - `YESTERDAY_TODAY`: same as `LATEST`
 - `LAST_MONTH`: previous calendar month
 - `MTD`: month-to-date
 - `LAST_{X}_DAYS`: relative range where end_date is today, start date is set X days behind.
 - `THIS_WEEK__{X}`: week-to-date starting on previous day of week specified by X. Valid values for X: `SUN, MON, TUES, WED, THURS, FRI, SAT`
 
+<br>
+
 ## Credits
+---
 
 This package was created with [Cookiecutter][cookiecutter] and the [fedejaure/cookiecutter-modern-pypackage][cookiecutter-modern-pypackage] project template.
 
 [cookiecutter]: https://github.com/cookiecutter/cookiecutter
 [cookiecutter-modern-pypackage]: https://github.com/fedejaure/cookiecutter-modern-pypackage
```

