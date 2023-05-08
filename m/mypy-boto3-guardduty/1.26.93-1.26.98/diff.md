# Comparing `tmp/mypy-boto3-guardduty-1.26.93.tar.gz` & `tmp/mypy-boto3-guardduty-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.26.93.tar", last modified: Thu Mar 16 19:19:49 2023, max compression
+gzip compressed data, was "mypy-boto3-guardduty-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
```

## Comparing `mypy-boto3-guardduty-1.26.93.tar` & `mypy-boto3-guardduty-1.26.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.211278 mypy-boto3-guardduty-1.26.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24423 2023-03-16 19:19:49.211278 mypy-boto3-guardduty-1.26.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.211278 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47290 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47209 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-03-16 19:19:36.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-03-16 19:19:36.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    82571 2023-03-16 19:19:38.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    82490 2023-03-16 19:19:37.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.211278 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24423 2023-03-16 19:19:49.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-16 19:19:49.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:19:49.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:19:49.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-16 19:19:49.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 19:19:49.000000 mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 19:19:49.211278 mypy-boto3-guardduty-1.26.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-16 19:19:35.000000 mypy-boto3-guardduty-1.26.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22921 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.375626 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47307 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    82726 2023-03-23 19:32:13.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-03-23 19:32:12.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/setup.py
```

### Comparing `mypy-boto3-guardduty-1.26.93/LICENSE` & `mypy-boto3-guardduty-1.26.98/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-guardduty-1.26.93/PKG-INFO` & `mypy-boto3-guardduty-1.26.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.26.93
-Summary: Type annotations for boto3.GuardDuty 1.26.93 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.98
+Summary: Type annotations for boto3.GuardDuty 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,14 +321,15 @@
 
 `mypy_boto3_guardduty.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_guardduty.literals import (
     AdminStatusType,
+    AutoEnableMembersType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DescribeMalwareScansPaginatorName,
     DestinationTypeType,
     DetectorFeatureResultType,
     DetectorFeatureType,
@@ -649,42 +650,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-guardduty-1.26.93/README.md` & `mypy-boto3-guardduty-1.26.98/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +289,15 @@
 
 `mypy_boto3_guardduty.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_guardduty.literals import (
     AdminStatusType,
+    AutoEnableMembersType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DescribeMalwareScansPaginatorName,
     DestinationTypeType,
     DetectorFeatureResultType,
     DetectorFeatureType,
@@ -617,42 +618,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/__init__.py` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/__init__.pyi` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/__main__.py` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.26.93\nVersion:         1.26.93\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.GuardDuty 1.26.98\nVersion:         1.26.98\nBuilder version:"
+        " 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.93")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/client.py` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    AutoEnableMembersType,
     EbsSnapshotPreservationType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     IpSetFormatType,
     ThreatIntelSetFormatType,
     UsageStatisticTypeType,
@@ -344,15 +345,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#delete_members)
         """
 
     def delete_publishing_destination(
         self, *, DetectorId: str, DestinationId: str
     ) -> Dict[str, Any]:
         """
-        Deletes the publishing definition with the specified `destinationId` .
+        Deletes the publishing definition with the specified `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_publishing_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#delete_publishing_destination)
         """
 
     def delete_threat_intel_set(self, *, DetectorId: str, ThreatIntelSetId: str) -> Dict[str, Any]:
         """
@@ -390,15 +391,15 @@
         """
 
     def describe_publishing_destination(
         self, *, DetectorId: str, DestinationId: str
     ) -> DescribePublishingDestinationResponseTypeDef:
         """
         Returns information about the publishing destination specified by the provided
-        `destinationId` .
+        `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.describe_publishing_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#describe_publishing_destination)
         """
 
     def disable_organization_admin_account(self, *, AdminAccountId: str) -> Dict[str, Any]:
         """
@@ -519,15 +520,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_invitations_count)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_invitations_count)
         """
 
     def get_ip_set(self, *, DetectorId: str, IpSetId: str) -> GetIPSetResponseTypeDef:
         """
-        Retrieves the IPSet specified by the `ipSetId` .
+        Retrieves the IPSet specified by the `ipSetId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_ip_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_ip_set)
         """
 
     def get_malware_scan_settings(
         self, *, DetectorId: str
@@ -710,15 +711,15 @@
         """
 
     def list_publishing_destinations(
         self, *, DetectorId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListPublishingDestinationsResponseTypeDef:
         """
         Returns a list of publishing destinations associated with the specified
-        `detectorId` .
+        `detectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_publishing_destinations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_publishing_destinations)
         """
 
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -764,15 +765,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#tag_resource)
         """
 
     def unarchive_findings(self, *, DetectorId: str, FindingIds: Sequence[str]) -> Dict[str, Any]:
         """
-        Unarchives GuardDuty findings specified by the `findingIds` .
+        Unarchives GuardDuty findings specified by the `findingIds`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.unarchive_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#unarchive_findings)
         """
 
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
@@ -875,35 +876,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_member_detectors)
         """
 
     def update_organization_configuration(
         self,
         *,
         DetectorId: str,
-        AutoEnable: bool,
+        AutoEnable: bool = ...,
         DataSources: OrganizationDataSourceConfigurationsTypeDef = ...,
-        Features: Sequence[OrganizationFeatureConfigurationTypeDef] = ...
+        Features: Sequence[OrganizationFeatureConfigurationTypeDef] = ...,
+        AutoEnableOrganizationMembers: AutoEnableMembersType = ...
     ) -> Dict[str, Any]:
         """
-        Updates the delegated administrator account with the values provided.
+        Configures the delegated administrator account with the provided values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_organization_configuration)
         """
 
     def update_publishing_destination(
         self,
         *,
         DetectorId: str,
         DestinationId: str,
         DestinationProperties: DestinationPropertiesTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates information about the publishing destination specified by the
-        `destinationId` .
+        `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_publishing_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_publishing_destination)
         """
 
     def update_threat_intel_set(
         self,
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/client.pyi` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    AutoEnableMembersType,
     EbsSnapshotPreservationType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     IpSetFormatType,
     ThreatIntelSetFormatType,
     UsageStatisticTypeType,
@@ -321,15 +322,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#delete_members)
         """
     def delete_publishing_destination(
         self, *, DetectorId: str, DestinationId: str
     ) -> Dict[str, Any]:
         """
-        Deletes the publishing definition with the specified `destinationId` .
+        Deletes the publishing definition with the specified `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_publishing_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#delete_publishing_destination)
         """
     def delete_threat_intel_set(self, *, DetectorId: str, ThreatIntelSetId: str) -> Dict[str, Any]:
         """
         Deletes the ThreatIntelSet specified by the ThreatIntelSet ID.
@@ -363,15 +364,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#describe_organization_configuration)
         """
     def describe_publishing_destination(
         self, *, DetectorId: str, DestinationId: str
     ) -> DescribePublishingDestinationResponseTypeDef:
         """
         Returns information about the publishing destination specified by the provided
-        `destinationId` .
+        `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.describe_publishing_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#describe_publishing_destination)
         """
     def disable_organization_admin_account(self, *, AdminAccountId: str) -> Dict[str, Any]:
         """
         Disables an Amazon Web Services account within the Organization as the GuardDuty
@@ -479,15 +480,15 @@
         current member account except the currently accepted invitation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_invitations_count)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_invitations_count)
         """
     def get_ip_set(self, *, DetectorId: str, IpSetId: str) -> GetIPSetResponseTypeDef:
         """
-        Retrieves the IPSet specified by the `ipSetId` .
+        Retrieves the IPSet specified by the `ipSetId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_ip_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_ip_set)
         """
     def get_malware_scan_settings(
         self, *, DetectorId: str
     ) -> GetMalwareScanSettingsResponseTypeDef:
@@ -654,15 +655,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_organization_admin_accounts)
         """
     def list_publishing_destinations(
         self, *, DetectorId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListPublishingDestinationsResponseTypeDef:
         """
         Returns a list of publishing destinations associated with the specified
-        `detectorId` .
+        `detectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_publishing_destinations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_publishing_destinations)
         """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists tags for a resource.
@@ -702,15 +703,15 @@
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#tag_resource)
         """
     def unarchive_findings(self, *, DetectorId: str, FindingIds: Sequence[str]) -> Dict[str, Any]:
         """
-        Unarchives GuardDuty findings specified by the `findingIds` .
+        Unarchives GuardDuty findings specified by the `findingIds`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.unarchive_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#unarchive_findings)
         """
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
@@ -805,34 +806,35 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_member_detectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_member_detectors)
         """
     def update_organization_configuration(
         self,
         *,
         DetectorId: str,
-        AutoEnable: bool,
+        AutoEnable: bool = ...,
         DataSources: OrganizationDataSourceConfigurationsTypeDef = ...,
-        Features: Sequence[OrganizationFeatureConfigurationTypeDef] = ...
+        Features: Sequence[OrganizationFeatureConfigurationTypeDef] = ...,
+        AutoEnableOrganizationMembers: AutoEnableMembersType = ...
     ) -> Dict[str, Any]:
         """
-        Updates the delegated administrator account with the values provided.
+        Configures the delegated administrator account with the provided values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_organization_configuration)
         """
     def update_publishing_destination(
         self,
         *,
         DetectorId: str,
         DestinationId: str,
         DestinationProperties: DestinationPropertiesTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates information about the publishing destination specified by the
-        `destinationId` .
+        `destinationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_publishing_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_publishing_destination)
         """
     def update_threat_intel_set(
         self,
         *,
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/literals.py` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AdminStatusType",
+    "AutoEnableMembersType",
     "CriterionKeyType",
     "DataSourceStatusType",
     "DataSourceType",
     "DescribeMalwareScansPaginatorName",
     "DestinationTypeType",
     "DetectorFeatureResultType",
     "DetectorFeatureType",
@@ -62,14 +63,15 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
+AutoEnableMembersType = Literal["ALL", "NEW", "NONE"]
 CriterionKeyType = Literal[
     "ACCOUNT_ID",
     "EC2_INSTANCE_ARN",
     "GUARDDUTY_FINDING_ID",
     "SCAN_ID",
     "SCAN_START_TIME",
     "SCAN_STATUS",
@@ -315,14 +317,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/literals.pyi` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AdminStatusType",
+    "AutoEnableMembersType",
     "CriterionKeyType",
     "DataSourceStatusType",
     "DataSourceType",
     "DescribeMalwareScansPaginatorName",
     "DestinationTypeType",
     "DetectorFeatureResultType",
     "DetectorFeatureType",
@@ -60,14 +61,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
+AutoEnableMembersType = Literal["ALL", "NEW", "NONE"]
 CriterionKeyType = Literal[
     "ACCOUNT_ID",
     "EC2_INSTANCE_ARN",
     "GUARDDUTY_FINDING_ID",
     "SCAN_ID",
     "SCAN_START_TIME",
     "SCAN_STATUS",
@@ -313,14 +315,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/paginator.py` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/paginator.pyi` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/type_defs.py` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
+    AutoEnableMembersType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
@@ -3150,30 +3151,32 @@
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
+        "AutoEnableOrganizationMembers": AutoEnableMembersType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
-        "AutoEnable": bool,
     },
 )
 _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
+        "AutoEnable": bool,
         "DataSources": OrganizationDataSourceConfigurationsTypeDef,
         "Features": Sequence[OrganizationFeatureConfigurationTypeDef],
+        "AutoEnableOrganizationMembers": AutoEnableMembersType,
     },
     total=False,
 )
 
 
 class UpdateOrganizationConfigurationRequestRequestTypeDef(
     _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty/type_defs.pyi` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
+    AutoEnableMembersType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
@@ -3073,30 +3074,32 @@
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
+        "AutoEnableOrganizationMembers": AutoEnableMembersType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
-        "AutoEnable": bool,
     },
 )
 _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
+        "AutoEnable": bool,
         "DataSources": OrganizationDataSourceConfigurationsTypeDef,
         "Features": Sequence[OrganizationFeatureConfigurationTypeDef],
+        "AutoEnableOrganizationMembers": AutoEnableMembersType,
     },
     total=False,
 )
 
 class UpdateOrganizationConfigurationRequestRequestTypeDef(
     _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef,
     _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.26.93
-Summary: Type annotations for boto3.GuardDuty 1.26.93 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.98
+Summary: Type annotations for boto3.GuardDuty 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,14 +321,15 @@
 
 `mypy_boto3_guardduty.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_guardduty.literals import (
     AdminStatusType,
+    AutoEnableMembersType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DescribeMalwareScansPaginatorName,
     DestinationTypeType,
     DetectorFeatureResultType,
     DetectorFeatureType,
@@ -649,42 +650,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-guardduty-1.26.93/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.93/setup.py` & `mypy-boto3-guardduty-1.26.98/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-guardduty.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.26.93",
+    version="1.26.98",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GuardDuty 1.26.93 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.GuardDuty 1.26.98 service generated with mypy-boto3-builder"
+        " 7.14.2"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

