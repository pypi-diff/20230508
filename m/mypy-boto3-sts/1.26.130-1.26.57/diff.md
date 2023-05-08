# Comparing `tmp/mypy-boto3-sts-1.26.130.tar.gz` & `tmp/mypy-boto3-sts-1.26.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sts-1.26.130.tar", last modified: Mon May  8 19:32:44 2023, max compression
+gzip compressed data, was "mypy-boto3-sts-1.26.57.tar", last modified: Wed Jan 25 20:48:09 2023, max compression
```

## Comparing `mypy-boto3-sts-1.26.130.tar` & `mypy-boto3-sts-1.26.57.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:44.012988 mypy-boto3-sts-1.26.130/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-08 19:32:44.012988 mypy-boto3-sts-1.26.130/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:44.012988 mypy-boto3-sts-1.26.130/mypy_boto3_sts/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:32:44.012988 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-08 19:32:43.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-08 19:32:43.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:32:43.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:32:43.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 19:32:43.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 19:32:43.000000 mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:32:44.012988 mypy-boto3-sts-1.26.130/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-08 19:32:31.000000 mypy-boto3-sts-1.26.130/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:09.416243 mypy-boto3-sts-1.26.57/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-01-25 20:48:09.412243 mypy-boto3-sts-1.26.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:09.412243 mypy-boto3-sts-1.26.57/mypy_boto3_sts/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:09.412243 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-01-25 20:48:09.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-25 20:48:09.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:09.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:09.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-25 20:48:09.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-25 20:48:09.000000 mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:48:09.416243 mypy-boto3-sts-1.26.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-25 20:47:56.000000 mypy-boto3-sts-1.26.57/setup.py
```

### Comparing `mypy-boto3-sts-1.26.130/LICENSE` & `mypy-boto3-sts-1.26.57/LICENSE`

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

### Comparing `mypy-boto3-sts-1.26.130/PKG-INFO` & `mypy-boto3-sts-1.26.57/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sts
-Version: 1.26.130
-Summary: Type annotations for boto3.STS 1.26.130 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.57
+Summary: Type annotations for boto3.STS 1.26.57 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sts"></a>
 
 # mypy-boto3-sts
 
 [![PyPI - mypy-boto3-sts](https://img.shields.io/pypi/v/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sts?color=blue)](https://pypistats.org/packages/mypy-boto3-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.STS 1.26.130](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[boto3.STS 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,42 +330,42 @@
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

### Comparing `mypy-boto3-sts-1.26.130/README.md` & `mypy-boto3-sts-1.26.57/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sts"></a>
 
 # mypy-boto3-sts
 
 [![PyPI - mypy-boto3-sts](https://img.shields.io/pypi/v/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sts?color=blue)](https://pypistats.org/packages/mypy-boto3-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.STS 1.26.130](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[boto3.STS 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,42 +298,42 @@
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

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/__main__.py` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.STS 1.26.130\nVersion:         1.26.130\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.STS 1.26.57\nVersion:         1.26.57\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.130")
+    print("1.26.57")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/client.py` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         Policy: str = ...,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         DurationSeconds: int = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> GetFederationTokenResponseTypeDef:
         """
         Returns a set of temporary security credentials (consisting of an access key ID,
-        a secret access key, and a security token) for a user.
+        a secret access key, and a security token) for a federated user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_federation_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/client/#get_federation_token)
         """
 
     def get_session_token(
         self, *, DurationSeconds: int = ..., SerialNumber: str = ..., TokenCode: str = ...
```

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/client.pyi` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         Policy: str = ...,
         PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,
         DurationSeconds: int = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> GetFederationTokenResponseTypeDef:
         """
         Returns a set of temporary security credentials (consisting of an access key ID,
-        a secret access key, and a security token) for a user.
+        a secret access key, and a security token) for a federated user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_federation_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/client/#get_federation_token)
         """
     def get_session_token(
         self, *, DurationSeconds: int = ..., SerialNumber: str = ..., TokenCode: str = ...
     ) -> GetSessionTokenResponseTypeDef:
```

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/literals.py` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -167,15 +166,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -186,15 +184,14 @@
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
@@ -256,15 +253,14 @@
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
@@ -346,20 +342,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/literals.pyi` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -165,15 +164,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -184,15 +182,14 @@
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
@@ -254,15 +251,14 @@
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
@@ -344,20 +340,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/type_defs.py` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts/type_defs.pyi` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/PKG-INFO` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sts
-Version: 1.26.130
-Summary: Type annotations for boto3.STS 1.26.130 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.57
+Summary: Type annotations for boto3.STS 1.26.57 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sts"></a>
 
 # mypy-boto3-sts
 
 [![PyPI - mypy-boto3-sts](https://img.shields.io/pypi/v/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sts?color=blue)](https://pypistats.org/packages/mypy-boto3-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.STS 1.26.130](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[boto3.STS 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,42 +330,42 @@
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

### Comparing `mypy-boto3-sts-1.26.130/mypy_boto3_sts.egg-info/SOURCES.txt` & `mypy-boto3-sts-1.26.57/mypy_boto3_sts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.26.130/setup.py` & `mypy-boto3-sts-1.26.57/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-sts.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-sts",
-    version="1.26.130",
+    version="1.26.57",
     packages=["mypy_boto3_sts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.STS 1.26.130 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.STS 1.26.57 service generated with mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/",
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

