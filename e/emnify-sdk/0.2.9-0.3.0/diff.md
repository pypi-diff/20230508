# Comparing `tmp/emnify-sdk-0.2.9.tar.gz` & `tmp/emnify-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emnify-sdk-0.2.9.tar", last modified: Tue Jan 31 16:12:16 2023, max compression
+gzip compressed data, was "emnify-sdk-0.3.0.tar", last modified: Mon May  8 07:55:34 2023, max compression
```

## Comparing `emnify-sdk-0.2.9.tar` & `emnify-sdk-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.892481 emnify-sdk-0.2.9/
--rw-r--r--   0 root         (0) root         (0)    11312 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3299 2023-01-31 16:12:16.892481 emnify-sdk-0.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2838 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.884481 emnify-sdk-0.2.9/emnify/
--rw-r--r--   0 root         (0) root         (0)       49 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/api_manager.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/constants.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/emnify.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.884481 emnify-sdk-0.2.9/emnify/modules/
--rw-r--r--   0 root         (0) root         (0)       34 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.884481 emnify-sdk-0.2.9/emnify/modules/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96544 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/api/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.888481 emnify-sdk-0.2.9/emnify/modules/device/
--rw-r--r--   0 root         (0) root         (0)       35 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/device/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/device/api_call_manager.py
--rw-r--r--   0 root         (0) root         (0)    13745 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/device/manager.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/device/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.888481 emnify-sdk-0.2.9/emnify/modules/operator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/operator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/operator/api_call_manager.py
--rw-r--r--   0 root         (0) root         (0)      470 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/operator/manager.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/operator/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.892481 emnify-sdk-0.2.9/emnify/modules/sim/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/sim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/sim/api_call_manager.py
--rw-r--r--   0 root         (0) root         (0)     4561 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/sim/manager.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/emnify/modules/sim/models.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-01-31 16:12:11.000000 emnify-sdk-0.2.9/emnify/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 16:12:16.892481 emnify-sdk-0.2.9/emnify_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3299 2023-01-31 16:12:16.000000 emnify-sdk-0.2.9/emnify_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-01-31 16:12:16.000000 emnify-sdk-0.2.9/emnify_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 16:12:16.000000 emnify-sdk-0.2.9/emnify_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-01-31 16:12:16.000000 emnify-sdk-0.2.9/emnify_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-31 16:12:16.000000 emnify-sdk-0.2.9/emnify_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-31 16:11:19.000000 emnify-sdk-0.2.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-31 16:12:16.892481 emnify-sdk-0.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1178 2023-01-31 16:12:11.000000 emnify-sdk-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11312 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/api_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/constants.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/emnify.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify/modules/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify/modules/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96544 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/api/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify/modules/device/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/device/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/device/api_call_manager.py
+-rw-r--r--   0 root         (0) root         (0)    14053 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/device/manager.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/device/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify/modules/operator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/operator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/operator/api_call_manager.py
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/operator/manager.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/operator/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify/modules/sim/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/sim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/sim/api_call_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5895 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/sim/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/emnify/modules/sim/models.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-08 07:55:29.000000 emnify-sdk-0.3.0/emnify/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/emnify_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-08 07:55:34.000000 emnify-sdk-0.3.0/emnify_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-08 07:55:34.000000 emnify-sdk-0.3.0/emnify_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 07:55:34.000000 emnify-sdk-0.3.0/emnify_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-08 07:55:34.000000 emnify-sdk-0.3.0/emnify_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-08 07:55:34.000000 emnify-sdk-0.3.0/emnify_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-05-08 07:55:29.000000 emnify-sdk-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 07:55:34.127178 emnify-sdk-0.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    11265 2023-05-08 07:54:40.000000 emnify-sdk-0.3.0/tests/test_emnify.py
```

### Comparing `emnify-sdk-0.2.9/LICENSE` & `emnify-sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/PKG-INFO` & `emnify-sdk-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: emnify-sdk
-Version: 0.2.9
-Summary: Supply your swarm of IoT Devices with cloud connectivity by EMnify. Automate your routines with this SDK for Python.
-Home-page: https://github.com/EMnify/emnify-sdk-python
-Author: EMnify
-Author-email: 
-Project-URL: Bug Tracker, https://github.com/EMnify/emnify-sdk-python
-Keywords: Swagger,EMnify Python SDK,IoT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # emnify Python SDK
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=reliability_rating&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=coverage&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=sqale_rating&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=security_rating&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=bugs&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=vulnerabilities&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
@@ -44,17 +31,26 @@
 pip install emnify-sdk
 ```
 
 ## Documentation
 
 Read more about working with the Python SDK and the underlying concepts in the [emnify product documentation](https://docs.emnify.com/sdks/python).
 
+### API reference
+
+We use [sphinx-autoapi](https://github.com/readthedocs/sphinx-autoapi) to auto-generate the API reference documentation within this repository. 
+This documentation is hosted separately on [GitHub Pages](https://emnify.github.io/emnify-sdk-python/autoapi/index.html). 
+
+> 🗺️ _Note: We plan to eventually migrate the API reference documentation into our [product documentation platform](https://docs.emnify.com/)._
+
+See our [documentation guide](./docs/README.md) if you're interested in contributing to the API reference or running the documentation locally.
+
 ## Contributing
 
-If you've found a bug or would like to add new features, [open an issue](https://github.com/emnify/emnify-sdk-python/issues/new) or [create a pull request](https://github.com/emnify/emnify-sdk-python/pulls) to this Github repository.
+If you've found a bug or want to add new features, [open an issue](https://github.com/emnify/emnify-sdk-python/issues/new) or [create a pull request](https://github.com/emnify/emnify-sdk-python/pulls) to this GitHub repository.
 
 See our [development guide](./DEVELOPMENT.md) for how to get started.
 
 Please note that this project is governed by [emnify's Code of Conduct](https://github.com/emnify/.github/blob/main/CODE_OF_CONDUCT.md). By participating, you agree to abide by its terms.
 
 ## Get support
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emnify-sdk-0.2.9/README.md` & `emnify-sdk-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: emnify-sdk
+Version: 0.3.0
+Summary: Supply your swarm of IoT Devices with cloud connectivity by EMnify. Automate your routines with this SDK for Python.
+Home-page: https://github.com/EMnify/emnify-sdk-python
+Author: EMnify
+Author-email: 
+Project-URL: Bug Tracker, https://github.com/EMnify/emnify-sdk-python
+Keywords: Swagger,EMnify Python SDK,IoT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # emnify Python SDK
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=reliability_rating&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=coverage&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=sqale_rating&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=security_rating&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=bugs&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=EMnify_emnify-sdk-python&metric=vulnerabilities&token=cb362b064422f10be97244bb527b8bc37e1378b4)](https://sonarcloud.io/summary/new_code?id=EMnify_emnify-sdk-python)
@@ -31,17 +44,26 @@
 pip install emnify-sdk
 ```
 
 ## Documentation
 
 Read more about working with the Python SDK and the underlying concepts in the [emnify product documentation](https://docs.emnify.com/sdks/python).
 
+### API reference
+
+We use [sphinx-autoapi](https://github.com/readthedocs/sphinx-autoapi) to auto-generate the API reference documentation within this repository. 
+This documentation is hosted separately on [GitHub Pages](https://emnify.github.io/emnify-sdk-python/autoapi/index.html). 
+
+> 🗺️ _Note: We plan to eventually migrate the API reference documentation into our [product documentation platform](https://docs.emnify.com/)._
+
+See our [documentation guide](./docs/README.md) if you're interested in contributing to the API reference or running the documentation locally.
+
 ## Contributing
 
-If you've found a bug or would like to add new features, [open an issue](https://github.com/emnify/emnify-sdk-python/issues/new) or [create a pull request](https://github.com/emnify/emnify-sdk-python/pulls) to this Github repository.
+If you've found a bug or want to add new features, [open an issue](https://github.com/emnify/emnify-sdk-python/issues/new) or [create a pull request](https://github.com/emnify/emnify-sdk-python/pulls) to this GitHub repository.
 
 See our [development guide](./DEVELOPMENT.md) for how to get started.
 
 Please note that this project is governed by [emnify's Code of Conduct](https://github.com/emnify/.github/blob/main/CODE_OF_CONDUCT.md). By participating, you agree to abide by its terms.
 
 ## Get support
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emnify-sdk-0.2.9/emnify/api_manager.py` & `emnify-sdk-0.3.0/emnify/api_manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/constants.py` & `emnify-sdk-0.3.0/emnify/constants.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/emnify.py` & `emnify-sdk-0.3.0/emnify/emnify.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/errors.py` & `emnify-sdk-0.3.0/emnify/errors.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/modules/api/models.py` & `emnify-sdk-0.3.0/emnify/modules/api/models.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/modules/device/api_call_manager.py` & `emnify-sdk-0.3.0/emnify/modules/device/api_call_manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/modules/device/manager.py` & `emnify-sdk-0.3.0/emnify/modules/device/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,17 +205,23 @@
     def change_status(
             self, device: typing.Union[
                 device_models.UpdateDevice, device_models.Device, device_models.RetrieveDevice, int
             ],
             enable: bool = None, disable: bool = None
     ) -> None:
         """
-        :param device: id or device model for update
-        :param enable: boolean parameter for enable a Device
-        :param disable: boolean parameter for disable a Device
+        Change the status of a device and assigned SIM to enabled or disabled.
+
+        :param device: The ID or device model to update.
+        :type device: Union[UpdateDevice, Device, RetrieveDevice, int]
+        :param enable: Whether to enable the device.
+        :type enable: bool
+        :param disable: Whether to disable the device.
+        :type disable: bool
+        :raises ValidationErrorException: If neither `enable` nor `disable` is provided, or if both are provided.
         """
         if not (enable or disable) or (enable and disable):
             raise emnify_errors.ValidationErrorException('"enable" or "disable" arguments must be provided ')
         new_status = emnify_constants.DeviceStatuses.ENABLED_DICT.value \
             if enable else emnify_constants.DeviceStatuses.DISABLED_DICT.value
         if isinstance(device, int):
             device = self.retrieve_device(device)
```

### Comparing `emnify-sdk-0.2.9/emnify/modules/device/models.py` & `emnify-sdk-0.3.0/emnify/modules/device/models.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/modules/sim/api_call_manager.py` & `emnify-sdk-0.3.0/emnify/modules/sim/api_call_manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify/modules/sim/models.py` & `emnify-sdk-0.3.0/emnify/modules/sim/models.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.2.9/emnify_sdk.egg-info/PKG-INFO` & `emnify-sdk-0.3.0/emnify_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emnify-sdk
-Version: 0.2.9
+Version: 0.3.0
 Summary: Supply your swarm of IoT Devices with cloud connectivity by EMnify. Automate your routines with this SDK for Python.
 Home-page: https://github.com/EMnify/emnify-sdk-python
 Author: EMnify
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/EMnify/emnify-sdk-python
 Keywords: Swagger,EMnify Python SDK,IoT
 Requires-Python: >=3.6
@@ -44,17 +44,26 @@
 pip install emnify-sdk
 ```
 
 ## Documentation
 
 Read more about working with the Python SDK and the underlying concepts in the [emnify product documentation](https://docs.emnify.com/sdks/python).
 
+### API reference
+
+We use [sphinx-autoapi](https://github.com/readthedocs/sphinx-autoapi) to auto-generate the API reference documentation within this repository. 
+This documentation is hosted separately on [GitHub Pages](https://emnify.github.io/emnify-sdk-python/autoapi/index.html). 
+
+> 🗺️ _Note: We plan to eventually migrate the API reference documentation into our [product documentation platform](https://docs.emnify.com/)._
+
+See our [documentation guide](./docs/README.md) if you're interested in contributing to the API reference or running the documentation locally.
+
 ## Contributing
 
-If you've found a bug or would like to add new features, [open an issue](https://github.com/emnify/emnify-sdk-python/issues/new) or [create a pull request](https://github.com/emnify/emnify-sdk-python/pulls) to this Github repository.
+If you've found a bug or want to add new features, [open an issue](https://github.com/emnify/emnify-sdk-python/issues/new) or [create a pull request](https://github.com/emnify/emnify-sdk-python/pulls) to this GitHub repository.
 
 See our [development guide](./DEVELOPMENT.md) for how to get started.
 
 Please note that this project is governed by [emnify's Code of Conduct](https://github.com/emnify/.github/blob/main/CODE_OF_CONDUCT.md). By participating, you agree to abide by its terms.
 
 ## Get support
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emnify-sdk-0.2.9/emnify_sdk.egg-info/SOURCES.txt` & `emnify-sdk-0.3.0/emnify_sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 emnify/modules/sim/api_call_manager.py
 emnify/modules/sim/manager.py
 emnify/modules/sim/models.py
 emnify_sdk.egg-info/PKG-INFO
 emnify_sdk.egg-info/SOURCES.txt
 emnify_sdk.egg-info/dependency_links.txt
 emnify_sdk.egg-info/requires.txt
-emnify_sdk.egg-info/top_level.txt
+emnify_sdk.egg-info/top_level.txt
+tests/test_emnify.py
```

### Comparing `emnify-sdk-0.2.9/setup.py` & `emnify-sdk-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 from setuptools import setup, find_packages
 import os
 
 NAME = os.getenv('PYPI_PACKAGE_NAME') or "emnify-sdk"
-VERSION = "0.2.9"
+VERSION = "0.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

