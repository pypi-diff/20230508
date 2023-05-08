# Comparing `tmp/volttron_actuator-0.1.1a3.tar.gz` & `tmp/volttron_actuator-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_actuator-0.1.1a3.tar", max compression
+gzip compressed data, was "volttron_actuator-0.1.1a4.tar", max compression
```

## Comparing `volttron_actuator-0.1.1a3.tar` & `volttron_actuator-0.1.1a4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10255 2023-05-08 19:20:06.110185 volttron_actuator-0.1.1a3/LICENSE
--rw-r--r--   0        0        0     2666 2023-05-08 19:20:06.110185 volttron_actuator-0.1.1a3/README.md
--rw-r--r--   0        0        0     1910 2023-05-08 19:21:19.094532 volttron_actuator-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0     1570 2023-05-08 19:20:06.110185 volttron_actuator-0.1.1a3/src/actuator/__init__.py
--rw-r--r--   0        0        0    52552 2023-05-08 19:20:06.110185 volttron_actuator-0.1.1a3/src/actuator/agent.py
--rw-r--r--   0        0        0    16122 2023-05-08 19:20:06.110185 volttron_actuator-0.1.1a3/src/actuator/scheduler.py
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a3/setup.py
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0    10255 2023-05-08 19:23:43.230098 volttron_actuator-0.1.1a4/LICENSE
+-rw-r--r--   0        0        0     2666 2023-05-08 19:23:43.230098 volttron_actuator-0.1.1a4/README.md
+-rw-r--r--   0        0        0     1910 2023-05-08 19:25:05.805904 volttron_actuator-0.1.1a4/pyproject.toml
+-rw-r--r--   0        0        0     1570 2023-05-08 19:23:43.230098 volttron_actuator-0.1.1a4/src/actuator/__init__.py
+-rw-r--r--   0        0        0    52552 2023-05-08 19:23:43.230098 volttron_actuator-0.1.1a4/src/actuator/agent.py
+-rw-r--r--   0        0        0    16122 2023-05-08 19:23:43.230098 volttron_actuator-0.1.1a4/src/actuator/scheduler.py
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a4/setup.py
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a4/PKG-INFO
```

### Comparing `volttron_actuator-0.1.1a3/LICENSE` & `volttron_actuator-0.1.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a3/README.md` & `volttron_actuator-0.1.1a4/README.md`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a3/pyproject.toml` & `volttron_actuator-0.1.1a4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 ignore_whitespace = true
 
 [tool.mypy]
-python_version = 3.8
+python_version = 3.10
 show_error_context = true
 pretty = true
 show_column_numbers = true
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-actuator"
-version = "0.1.1a3"
+version = "0.1.1a4"
 description = "The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-actuator"
 homepage = "https://github.com/VOLTTRON/volttron-actuator"
 keywords = []
@@ -35,15 +35,15 @@
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 tzlocal = "^4.2"
-volttron = ">=10.0.2rc0,<11.0"
+volttron = ">=10.0.rc0,<11.0"
 types-tzlocal = "^4.2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.4.0rc0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
```

### Comparing `volttron_actuator-0.1.1a3/src/actuator/__init__.py` & `volttron_actuator-0.1.1a4/src/actuator/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a3/src/actuator/agent.py` & `volttron_actuator-0.1.1a4/src/actuator/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a3/src/actuator/scheduler.py` & `volttron_actuator-0.1.1a4/src/actuator/scheduler.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a3/setup.py` & `volttron_actuator-0.1.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['types-tzlocal>=4.2.2.2,<5.0.0.0',
  'tzlocal>=4.2,<5.0',
- 'volttron>=10.0.2rc0,<11.0']
+ 'volttron>=10.0.rc0,<11.0']
 
 entry_points = \
 {'console_scripts': ['volttron-actuator = actuator.agent:main']}
 
 setup_kwargs = {
     'name': 'volttron-actuator',
-    'version': '0.1.1a3',
+    'version': '0.1.1a4',
     'description': 'The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.',
     'long_description': '# volttron-actuator\n\n[![Passing?](https://github.com/eclipse-volttron/volttron-actuator/actions/workflows/run-tests.yml/badge.svg)](https://github.com/VOLTTRON/volttron-actuator/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-actuator.svg)](https://pypi.org/project/volttron-actuator/)\n\n\nThe Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.\n\n# Requires\n\n* python >= 3.10\n* volttron >= 10.0\n* tzlocal >= 4.2\n* types-tzlocal >= 4.2.2.2\n\n# Documentation\nMore detailed documentation can be found on [ReadTheDocs](https://volttron.readthedocs.io/en/modular/). The RST source\nof the documentation for this component is located in the "docs" directory of this repository.\n\n# Installation\n\nBefore installing, VOLTTRON should be installed and running.  Its virtual environment should be active.\nInformation on how to install of the VOLTTRON platform can be found\n[here](https://github.com/eclipse-volttron/volttron-core).\n\nInstall and start the volttron-actuator.\n\n```shell\nvctl install volttron-actuator --agent-config <path to agent config> --start\n```\n\nView the status of the installed agent\n\n```shell\nvctl status\n```\n\n# Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'Mark Bonicillo',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/VOLTTRON/volttron-actuator',
```

### Comparing `volttron_actuator-0.1.1a3/PKG-INFO` & `volttron_actuator-0.1.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-actuator
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.
 Home-page: https://github.com/VOLTTRON/volttron-actuator
 License: Apache-2.0
 Author: Mark Bonicillo
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: types-tzlocal (>=4.2.2.2,<5.0.0.0)
 Requires-Dist: tzlocal (>=4.2,<5.0)
-Requires-Dist: volttron (>=10.0.2rc0,<11.0)
+Requires-Dist: volttron (>=10.0.rc0,<11.0)
 Project-URL: Repository, https://github.com/VOLTTRON/volttron-actuator
 Description-Content-Type: text/markdown
 
 # volttron-actuator
 
 [![Passing?](https://github.com/eclipse-volttron/volttron-actuator/actions/workflows/run-tests.yml/badge.svg)](https://github.com/VOLTTRON/volttron-actuator/actions/workflows/run-tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/volttron-actuator.svg)](https://pypi.org/project/volttron-actuator/)
```

