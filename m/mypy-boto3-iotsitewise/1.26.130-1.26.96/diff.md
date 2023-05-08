# Comparing `tmp/mypy-boto3-iotsitewise-1.26.130.tar.gz` & `tmp/mypy-boto3-iotsitewise-1.26.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsitewise-1.26.130.tar", last modified: Mon May  8 19:32:44 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsitewise-1.26.96.tar", last modified: Tue Mar 21 19:19:40 2023, max compression
```

## Comparing `mypy-boto3-iotsitewise-1.26.130.tar` & `mypy-boto3-iotsitewise-1.26.96.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:44.000988 mypy-boto3-iotsitewise-1.26.130/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28388 2023-05-08 19:32:44.000988 mypy-boto3-iotsitewise-1.26.130/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26883 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:44.000988 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-08 19:32:27.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   105727 2023-05-08 19:32:30.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105526 2023-05-08 19:32:28.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 19:32:25.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-08 19:32:26.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:44.000988 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28388 2023-05-08 19:32:43.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-08 19:32:43.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:32:43.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:32:43.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 19:32:43.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 19:32:43.000000 mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:32:44.000988 mypy-boto3-iotsitewise-1.26.130/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 19:32:24.000000 mypy-boto3-iotsitewise-1.26.130/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.917032 mypy-boto3-iotsitewise-1.26.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28402 2023-03-21 19:19:40.917032 mypy-boto3-iotsitewise-1.26.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.917032 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-03-21 19:19:21.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105727 2023-03-21 19:19:24.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105526 2023-03-21 19:19:21.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-03-21 19:19:20.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.917032 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28402 2023-03-21 19:19:40.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-21 19:19:40.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 19:19:40.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-21 19:19:40.000000 mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:19:40.917032 mypy-boto3-iotsitewise-1.26.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-21 19:19:19.000000 mypy-boto3-iotsitewise-1.26.96/setup.py
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/LICENSE` & `mypy-boto3-iotsitewise-1.26.96/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/PKG-INFO` & `mypy-boto3-iotsitewise-1.26.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.26.130
-Summary: Type annotations for boto3.IoTSiteWise 1.26.130 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.96
+Summary: Type annotations for boto3.IoTSiteWise 1.26.96 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsitewise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.26.130](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -734,42 +734,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/README.md` & `mypy-boto3-iotsitewise-1.26.96/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsitewise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.26.130](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -702,42 +702,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/__init__.py` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/__init__.pyi` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/client.py` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/client.pyi` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/literals.py` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -420,15 +419,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -515,15 +513,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/literals.pyi` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -418,15 +417,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -513,15 +511,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/paginator.py` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/paginator.pyi` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/type_defs.py` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/type_defs.pyi` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/waiter.py` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise/waiter.pyi` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/PKG-INFO` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.26.130
-Summary: Type annotations for boto3.IoTSiteWise 1.26.130 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.96
+Summary: Type annotations for boto3.IoTSiteWise 1.26.96 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsitewise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.26.130](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -734,42 +734,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-iotsitewise-1.26.130/mypy_boto3_iotsitewise.egg-info/SOURCES.txt` & `mypy-boto3-iotsitewise-1.26.96/mypy_boto3_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.26.130/setup.py` & `mypy-boto3-iotsitewise-1.26.96/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-iotsitewise.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-iotsitewise",
-    version="1.26.130",
+    version="1.26.96",
     packages=["mypy_boto3_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSiteWise 1.26.130 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTSiteWise 1.26.96 service generated with mypy-boto3-builder"
+        " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

