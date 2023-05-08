# Comparing `tmp/biolink-model-3.3.2.tar.gz` & `tmp/biolink-model-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biolink-model-3.3.2.tar", last modified: Thu May  4 23:02:29 2023, max compression
+gzip compressed data, was "biolink-model-3.3.3.tar", last modified: Mon May  8 15:13:20 2023, max compression
```

## Comparing `biolink-model-3.3.2.tar` & `biolink-model-3.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:02:29.325390 biolink-model-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-04 23:02:17.000000 biolink-model-3.3.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-04 23:02:17.000000 biolink-model-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-04 23:02:29.325390 biolink-model-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-04 23:02:17.000000 biolink-model-3.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:02:29.321390 biolink-model-3.3.2/biolink/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 23:02:17.000000 biolink-model-3.3.2/biolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   651883 2023-05-04 23:02:17.000000 biolink-model-3.3.2/biolink/model.py
--rw-r--r--   0 runner    (1001) docker     (123)  1193584 2023-05-04 23:02:17.000000 biolink-model-3.3.2/biolink/pydanticmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:02:29.325390 biolink-model-3.3.2/biolink_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-04 23:02:29.000000 biolink-model-3.3.2/biolink_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 23:02:29.000000 biolink-model-3.3.2/biolink_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:02:29.000000 biolink-model-3.3.2/biolink_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 23:02:29.000000 biolink-model-3.3.2/biolink_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 23:02:29.000000 biolink-model-3.3.2/biolink_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 23:02:17.000000 biolink-model-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 23:02:29.325390 biolink-model-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-04 23:02:17.000000 biolink-model-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:20.687583 biolink-model-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 15:13:10.000000 biolink-model-3.3.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-08 15:13:10.000000 biolink-model-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-08 15:13:20.687583 biolink-model-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-08 15:13:10.000000 biolink-model-3.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:20.683583 biolink-model-3.3.3/biolink/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-08 15:13:10.000000 biolink-model-3.3.3/biolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   651883 2023-05-08 15:13:10.000000 biolink-model-3.3.3/biolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1193584 2023-05-08 15:13:10.000000 biolink-model-3.3.3/biolink/pydanticmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:20.687583 biolink-model-3.3.3/biolink_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 15:13:20.000000 biolink-model-3.3.3/biolink_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-08 15:13:11.000000 biolink-model-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 15:13:20.687583 biolink-model-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 15:13:11.000000 biolink-model-3.3.3/setup.py
```

### Comparing `biolink-model-3.3.2/AUTHORS` & `biolink-model-3.3.3/AUTHORS`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.2/LICENSE` & `biolink-model-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.2/PKG-INFO` & `biolink-model-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.3.2
+Version: 3.3.3
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.3.2/README.md` & `biolink-model-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.2/biolink/__init__.py` & `biolink-model-3.3.3/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.3.2/biolink/model.py` & `biolink-model-3.3.3/biolink/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 2320 4175 746f 2067 656e 6572 6174 6564  # Auto generated
 00000010: 2066 726f 6d20 6269 6f6c 696e 6b2d 6d6f   from biolink-mo
 00000020: 6465 6c2e 7961 6d6c 2062 7920 7079 7468  del.yaml by pyth
 00000030: 6f6e 6765 6e2e 7079 2076 6572 7369 6f6e  ongen.py version
 00000040: 3a20 302e 392e 300a 2320 4765 6e65 7261  : 0.9.0.# Genera
 00000050: 7469 6f6e 2064 6174 653a 2032 3032 332d  tion date: 2023-
-00000060: 3035 2d30 3454 3231 3a33 313a 3439 0a23  05-04T21:31:49.#
+00000060: 3035 2d30 3454 3233 3a30 323a 3033 0a23  05-04T23:02:03.#
 00000070: 2053 6368 656d 613a 2042 696f 6c69 6e6b   Schema: Biolink
 00000080: 2d4d 6f64 656c 0a23 0a23 2069 643a 2068  -Model.#.# id: h
 00000090: 7474 7073 3a2f 2f77 3369 642e 6f72 672f  ttps://w3id.org/
 000000a0: 6269 6f6c 696e 6b2f 6269 6f6c 696e 6b2d  biolink/biolink-
 000000b0: 6d6f 6465 6c0a 2320 6465 7363 7269 7074  model.# descript
 000000c0: 696f 6e3a 2045 6e74 6974 7920 616e 6420  ion: Entity and 
 000000d0: 6173 736f 6369 6174 696f 6e20 7461 786f  association taxo
@@ -80,15 +80,15 @@
 000004f0: 6d6c 5f72 756e 7469 6d65 2e75 7469 6c73  ml_runtime.utils
 00000500: 2e6d 6574 616d 6f64 656c 636f 7265 2069  .metamodelcore i
 00000510: 6d70 6f72 7420 426f 6f6c 2c20 5552 496f  mport Bool, URIo
 00000520: 7243 5552 4945 2c20 5853 4444 6174 652c  rCURIE, XSDDate,
 00000530: 2058 5344 5469 6d65 0a0a 6d65 7461 6d6f   XSDTime..metamo
 00000540: 6465 6c5f 7665 7273 696f 6e20 3d20 2231  del_version = "1
 00000550: 2e37 2e30 220a 7665 7273 696f 6e20 3d20  .7.0".version = 
-00000560: 2233 2e33 2e31 220a 0a23 204f 7665 7277  "3.3.1"..# Overw
+00000560: 2233 2e33 2e32 220a 0a23 204f 7665 7277  "3.3.2"..# Overw
 00000570: 7269 7465 2064 6174 6163 6c61 7373 6573  rite dataclasses
 00000580: 205f 696e 6974 5f66 6e20 746f 2061 6464   _init_fn to add
 00000590: 202a 2a6b 7761 7267 7320 696e 205f 5f69   **kwargs in __i
 000005a0: 6e69 745f 5f0a 6461 7461 636c 6173 7365  nit__.dataclasse
 000005b0: 732e 5f69 6e69 745f 666e 203d 2064 6174  s._init_fn = dat
 000005c0: 6163 6c61 7373 6573 5f69 6e69 745f 666e  aclasses_init_fn
 000005d0: 5f77 6974 685f 6b77 6172 6773 0a0a 2320  _with_kwargs..#
```

### Comparing `biolink-model-3.3.2/biolink/pydanticmodel.py` & `biolink-model-3.3.3/biolink/pydanticmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime, date
 from enum import Enum
 from typing import List, Dict, Optional, Any, Union, Literal
 from pydantic import BaseModel as BaseModel, Field
 from linkml_runtime.linkml_model import Decimal
 
 metamodel_version = "None"
-version = "3.3.1"
+version = "3.3.2"
 
 class WeakRefShimBaseModel(BaseModel):
    __slots__ = '__weakref__'
     
 class ConfiguredBaseModel(WeakRefShimBaseModel,
                 validate_assignment = True, 
                 validate_all = True,
```

### Comparing `biolink-model-3.3.2/biolink_model.egg-info/PKG-INFO` & `biolink-model-3.3.3/biolink_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.3.2
+Version: 3.3.3
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.3.2/pyproject.toml` & `biolink-model-3.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 linkml = "^1.4"
 curies = "^0.5.2"
 prefixmaps = "^0.1.4"
 pytest = "^7.3.1"
+bs4 = "^0.0.1"
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "pep440"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `biolink-model-3.3.2/setup.cfg` & `biolink-model-3.3.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = biolink_model
 description = 'A high level datamodel of biological entities and associations'
-version = 3.3.2
+version = 3.3.3
 url = https://github.com/biolink/biolink-model
 author = Harold Solbrig
 author-email = smoxon@lbl.gov
 summary = Biolink Model
 home-page = https://biolink.github.io/biolink-model/docs/
 license = CC0 1.0 Universal
 python-requires = >=3.9
```

### Comparing `biolink-model-3.3.2/setup.py` & `biolink-model-3.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as FH:
     REQUIREMENTS = FH.readlines()
 
 NAME = 'biolink-model'
-VERSION = '3.3.2'
+VERSION = '3.3.3'
 
 DESCRIPTION = 'Biolink Model: A high level datamodel of biological entities and associations'
 URL = 'https://github.com/biolink/biolink-model'
 AUTHOR = 'Deepak Unni', 'Sierra Moxon'
 EMAIL = 'smoxon@lbl.gov'
 REQUIRES_PYTHON = '>=3.9'
 LICENSE = 'BSD'
```

