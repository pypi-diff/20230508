# Comparing `tmp/airplanesdk-0.3.7.tar.gz` & `tmp/airplanesdk-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airplanesdk-0.3.7.tar", max compression
+gzip compressed data, was "airplanesdk-0.3.8.tar", max compression
```

## Comparing `airplanesdk-0.3.7.tar` & `airplanesdk-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1080 2022-05-31 16:09:11.992902 airplanesdk-0.3.7/LICENSE
--rw-r--r--   0        0        0     1195 2022-05-31 16:09:11.993023 airplanesdk-0.3.7/README.md
--rw-r--r--   0        0        0      517 2022-07-26 16:51:29.504581 airplanesdk-0.3.7/airplane/__init__.py
--rw-r--r--   0        0        0       22 2022-07-27 21:18:05.662005 airplanesdk-0.3.7/airplane/_version.py
--rw-r--r--   0        0        0     5401 2022-07-26 15:51:09.741539 airplanesdk-0.3.7/airplane/api/client.py
--rw-r--r--   0        0        0     1025 2022-07-26 15:51:09.741891 airplanesdk-0.3.7/airplane/api/types.py
--rw-r--r--   0        0        0     1401 2022-07-26 16:51:29.504912 airplanesdk-0.3.7/airplane/builtins/__init__.py
--rw-r--r--   0        0        0     1672 2022-07-26 16:51:29.505905 airplanesdk-0.3.7/airplane/builtins/email.py
--rw-r--r--   0        0        0    15168 2022-07-26 16:51:29.506150 airplanesdk-0.3.7/airplane/builtins/mongodb.py
--rw-r--r--   0        0        0     2068 2022-07-26 16:51:29.506336 airplanesdk-0.3.7/airplane/builtins/rest.py
--rw-r--r--   0        0        0      829 2022-07-26 16:51:29.506489 airplanesdk-0.3.7/airplane/builtins/slack.py
--rw-r--r--   0        0        0     1483 2022-07-26 16:51:29.506911 airplanesdk-0.3.7/airplane/builtins/sql.py
--rw-r--r--   0        0        0      897 2022-07-26 15:51:09.742279 airplanesdk-0.3.7/airplane/exceptions.py
--rw-r--r--   0        0        0     2943 2022-06-15 19:21:09.596623 airplanesdk-0.3.7/airplane/output.py
--rw-r--r--   0        0        0        0 2022-06-02 19:32:31.590606 airplanesdk-0.3.7/airplane/py.typed
--rw-r--r--   0        0        0     1433 2022-07-27 21:18:05.662302 airplanesdk-0.3.7/airplane/runtime/__init__.py
--rw-r--r--   0        0        0     3037 2022-07-26 15:51:09.742917 airplanesdk-0.3.7/airplane/runtime/standard.py
--rw-r--r--   0        0        0     4812 2022-07-26 15:51:09.743207 airplanesdk-0.3.7/airplane/runtime/workflow.py
--rw-r--r--   0        0        0      720 2022-07-27 21:18:05.662561 airplanesdk-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2022 2022-07-27 21:18:29.176359 airplanesdk-0.3.7/setup.py
--rw-r--r--   0        0        0     2005 2022-07-27 21:18:29.176529 airplanesdk-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-05-31 16:09:11.992902 airplanesdk-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1195 2022-05-31 16:09:11.993023 airplanesdk-0.3.8/README.md
+-rw-r--r--   0        0        0      520 2022-07-27 21:51:13.944803 airplanesdk-0.3.8/airplane/__init__.py
+-rw-r--r--   0        0        0       22 2022-07-27 21:51:13.945159 airplanesdk-0.3.8/airplane/_version.py
+-rw-r--r--   0        0        0     5414 2022-07-27 21:51:13.945553 airplanesdk-0.3.8/airplane/api/client.py
+-rw-r--r--   0        0        0     1025 2022-07-27 21:51:13.945700 airplanesdk-0.3.8/airplane/api/entities.py
+-rw-r--r--   0        0        0     1401 2022-07-26 16:51:29.504912 airplanesdk-0.3.8/airplane/builtins/__init__.py
+-rw-r--r--   0        0        0     1672 2022-07-26 16:51:29.505905 airplanesdk-0.3.8/airplane/builtins/email.py
+-rw-r--r--   0        0        0    15168 2022-07-26 16:51:29.506150 airplanesdk-0.3.8/airplane/builtins/mongodb.py
+-rw-r--r--   0        0        0     2068 2022-07-26 16:51:29.506336 airplanesdk-0.3.8/airplane/builtins/rest.py
+-rw-r--r--   0        0        0      829 2022-07-26 16:51:29.506489 airplanesdk-0.3.8/airplane/builtins/slack.py
+-rw-r--r--   0        0        0     1483 2022-07-26 16:51:29.506911 airplanesdk-0.3.8/airplane/builtins/sql.py
+-rw-r--r--   0        0        0      900 2022-07-27 21:51:13.946025 airplanesdk-0.3.8/airplane/exceptions.py
+-rw-r--r--   0        0        0     2943 2022-06-15 19:21:09.596623 airplanesdk-0.3.8/airplane/output.py
+-rw-r--r--   0        0        0        0 2022-06-02 19:32:31.590606 airplanesdk-0.3.8/airplane/py.typed
+-rw-r--r--   0        0        0     1436 2022-07-27 21:51:13.946355 airplanesdk-0.3.8/airplane/runtime/__init__.py
+-rw-r--r--   0        0        0     3040 2022-07-27 21:51:13.946657 airplanesdk-0.3.8/airplane/runtime/standard.py
+-rw-r--r--   0        0        0     4815 2022-07-27 21:51:13.946915 airplanesdk-0.3.8/airplane/runtime/workflow.py
+-rw-r--r--   0        0        0      720 2022-07-27 21:51:13.947176 airplanesdk-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2022 2022-07-27 21:51:26.166580 airplanesdk-0.3.8/setup.py
+-rw-r--r--   0        0        0     2005 2022-07-27 21:51:26.166755 airplanesdk-0.3.8/PKG-INFO
```

### Comparing `airplanesdk-0.3.7/LICENSE` & `airplanesdk-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/README.md` & `airplanesdk-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/__init__.py` & `airplanesdk-0.3.8/airplane/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """airplane - An SDK for writing Airplane tasks in Python"""
 
 from airplane._version import __version__
 from airplane.api.client import APIClient
-from airplane.api.types import Run, RunStatus
+from airplane.api.entities import Run, RunStatus
 from airplane.builtins import email, mongodb, rest, slack, sql
 from airplane.exceptions import InvalidEnvironmentException, RunPendingException
 from airplane.output import append_output, set_output, write_named_output, write_output
 from airplane.runtime import execute
 
 # Deprecated
 from airplane.runtime.standard import run
```

### Comparing `airplanesdk-0.3.7/airplane/api/client.py` & `airplanesdk-0.3.8/airplane/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from requests import Response
 from requests.models import HTTPError
 
 from airplane._version import __version__
 from airplane.exceptions import InvalidEnvironmentException
 
 
-@dataclass
+@dataclass(frozen=True)
 class ClientOpts:
     """Client options for an APIClient."""
 
     api_host: str
     api_token: str
     env_id: str
```

### Comparing `airplanesdk-0.3.7/airplane/api/types.py` & `airplanesdk-0.3.8/airplane/api/entities.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/builtins/__init__.py` & `airplanesdk-0.3.8/airplane/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/builtins/email.py` & `airplanesdk-0.3.8/airplane/builtins/email.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/builtins/mongodb.py` & `airplanesdk-0.3.8/airplane/builtins/mongodb.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/builtins/rest.py` & `airplanesdk-0.3.8/airplane/builtins/rest.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/builtins/slack.py` & `airplanesdk-0.3.8/airplane/builtins/slack.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/builtins/sql.py` & `airplanesdk-0.3.8/airplane/builtins/sql.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/exceptions.py` & `airplanesdk-0.3.8/airplane/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 
-from airplane.api.types import Run
+from airplane.api.entities import Run
 
 
 class RunPendingException(Exception):
     """Exception that indicates a run is still in pending state."""
 
 
 class InvalidEnvironmentException(Exception):
```

### Comparing `airplanesdk-0.3.7/airplane/output.py` & `airplanesdk-0.3.8/airplane/output.py`

 * *Files identical despite different names*

### Comparing `airplanesdk-0.3.7/airplane/runtime/__init__.py` & `airplanesdk-0.3.8/airplane/runtime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from enum import Enum
 from typing import Any, Dict, Optional
 
-from airplane.api.types import Run
+from airplane.api.entities import Run
 from airplane.runtime.standard import execute as standard_execute
 from airplane.runtime.workflow import execute as workflow_execute
 
 __AIRPLANE_RUNTIME_ENV_VAR = "AIRPLANE_RUNTIME"
 
 
 class RuntimeKind(Enum):
```

### Comparing `airplanesdk-0.3.7/airplane/runtime/standard.py` & `airplanesdk-0.3.8/airplane/runtime/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import backoff
 import deprecation
 import requests
 
 from airplane._version import __version__
 from airplane.api.client import api_client_from_env
-from airplane.api.types import Run, RunStatus
+from airplane.api.entities import Run, RunStatus
 from airplane.exceptions import RunPendingException, RunTerminationException
 
 
 def execute(
     slug: str,
     param_values: Optional[Dict[str, Any]] = None,
     resources: Optional[Dict[str, Any]] = None,
```

### Comparing `airplanesdk-0.3.7/airplane/runtime/workflow.py` & `airplanesdk-0.3.8/airplane/runtime/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Any, Dict, Optional
 
 from temporalio import activity, workflow
 
 from airplane.api.client import ClientOpts, api_client, client_opts_from_env
-from airplane.api.types import Run, RunStatus
+from airplane.api.entities import Run, RunStatus
 
 
 @activity.defn
 def execute_task_activity(
     client_opts: ClientOpts,
     slug: str,
     param_values: Optional[Dict[str, Any]] = None,
```

### Comparing `airplanesdk-0.3.7/pyproject.toml` & `airplanesdk-0.3.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airplanesdk"
-version = "0.3.7"
+version = "0.3.8"
 description = "A Python SDK for writing Airplane tasks"
 authors = ["Airplane <support@airplane.dev>"]
 license = "MIT"
 repository = "https://github.com/airplanedev/python-sdk"
 homepage = "https://airplane.dev"
 readme = "README.md"
 packages = [
```

### Comparing `airplanesdk-0.3.7/setup.py` & `airplanesdk-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['backoff>=1.10.0,<2.0.0',
  'deprecation>=2.1.0,<3.0.0',
  'requests>=2.25.1,<3.0.0',
  'temporalio>=0.1a2,<0.2']
 
 setup_kwargs = {
     'name': 'airplanesdk',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': 'A Python SDK for writing Airplane tasks',
     'long_description': '# Airplane Python SDK [![PyPI](https://img.shields.io/pypi/v/airplanesdk)](https://pypi.org/project/airplanesdk/) [![PyPI - License](https://img.shields.io/pypi/l/airplanesdk)](./LICENSE) [![Docs](https://img.shields.io/badge/Docs-airplane-blue)](https://docs.airplane.dev/creating-tasks/python)\n\nSDK for writing [Airplane](https://airplane.dev) tasks in Python.\n\n## Getting started\n\n```sh\npip install airplanesdk\n```\n\n## Usage\n\nTo write a Python task in Airplane, create a `.py` file and export a function like so:\n\n```py\nimport airplane\n\ndef main(params):\n  return f"Hello, {params[\'name\']}"\n```\n\nYou can configure the parameters that your task will receive in the [Airplane UI](http://app.airplane.dev/). They\'ll be passed through the `params` argument to your function as a dictionary keyed by the slugs you see in the UI.\n\nTo execute your task, first [install the Airplane CLI](https://docs.airplane.dev/platform/airplane-cli).\n\nOnce installed, execute your task locally:\n\n```sh\nairplane dev ./path/to/file.py -- --name=World\n```\n\nIf that looks good, deploy your task to Airplane and give it a [run in the UI](https://app.airplane.dev/library)!\n\n```sh\nairplane deploy ./path/to/file.py\n```\n',
     'author': 'Airplane',
     'author_email': 'support@airplane.dev',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://airplane.dev',
```

### Comparing `airplanesdk-0.3.7/PKG-INFO` & `airplanesdk-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airplanesdk
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Python SDK for writing Airplane tasks
 Home-page: https://airplane.dev
 License: MIT
 Author: Airplane
 Author-email: support@airplane.dev
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

