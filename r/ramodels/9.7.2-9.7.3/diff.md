# Comparing `tmp/ramodels-9.7.2.tar.gz` & `tmp/ramodels-9.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramodels-9.7.2.tar", max compression
+gzip compressed data, was "ramodels-9.7.3.tar", max compression
```

## Comparing `ramodels-9.7.2.tar` & `ramodels-9.7.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2058 2022-08-26 10:03:29.255423 ramodels-9.7.2/README.md
--rw-r--r--   0        0        0     1265 2022-08-26 10:55:48.582213 ramodels-9.7.2/pyproject.toml
--rw-r--r--   0        0        0      300 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/__init__.py
--rw-r--r--   0        0        0     3107 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/base.py
--rw-r--r--   0        0        0     1056 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/exceptions.py
--rw-r--r--   0        0        0     1081 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/lora/__init__.py
--rw-r--r--   0        0        0    20773 2022-08-26 10:39:51.610638 ramodels-9.7.2/ramodels/lora/_shared.py
--rw-r--r--   0        0        0     2969 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/lora/facet.py
--rw-r--r--   0        0        0     4322 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/lora/itsystem.py
--rw-r--r--   0        0        0     3404 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/lora/klasse.py
--rw-r--r--   0        0        0     3501 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/lora/organisation.py
--rw-r--r--   0        0        0     1520 2022-08-26 10:39:51.614638 ramodels-9.7.2/ramodels/mo/__init__.py
--rw-r--r--   0        0        0    10895 2022-08-26 10:39:51.614638 ramodels-9.7.2/ramodels/mo/_shared.py
--rw-r--r--   0        0        0     2003 2022-08-26 10:39:51.614638 ramodels-9.7.2/ramodels/mo/class_.py
--rw-r--r--   0        0        0     1615 2022-08-26 10:39:51.614638 ramodels-9.7.2/ramodels/mo/detail.py
--rw-r--r--   0        0        0     3143 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/__init__.py
--rw-r--r--   0        0        0      926 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/_shared.py
--rw-r--r--   0        0        0     7248 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/address.py
--rw-r--r--   0        0        0     5527 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/association.py
--rw-r--r--   0        0        0     8163 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/engagement.py
--rw-r--r--   0        0        0     3814 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/engagement_association.py
--rw-r--r--   0        0        0     4186 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/it_system.py
--rw-r--r--   0        0        0     2491 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/kle.py
--rw-r--r--   0        0        0     2645 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/leave.py
--rw-r--r--   0        0        0     4897 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/manager.py
--rw-r--r--   0        0        0     1493 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/related_unit.py
--rw-r--r--   0        0        0     2544 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/details/role.py
--rw-r--r--   0        0        0     6357 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/employee.py
--rw-r--r--   0        0        0     1893 2022-08-26 10:39:51.614638 ramodels-9.7.2/ramodels/mo/facet.py
--rw-r--r--   0        0        0      962 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/organisation.py
--rw-r--r--   0        0        0     5396 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/mo/organisation_unit.py
--rw-r--r--   0        0        0        0 2022-08-26 10:35:29.379027 ramodels-9.7.2/ramodels/py.typed
--rw-r--r--   0        0        0     3119 2022-08-26 10:55:49.967526 ramodels-9.7.2/setup.py
--rw-r--r--   0        0        0     2868 2022-08-26 10:55:49.968173 ramodels-9.7.2/PKG-INFO
+-rw-r--r--   0        0        0     2058 2022-08-26 10:06:31.279430 ramodels-9.7.3/README.md
+-rw-r--r--   0        0        0     1265 2022-08-26 13:01:53.430356 ramodels-9.7.3/pyproject.toml
+-rw-r--r--   0        0        0      300 2022-08-26 12:59:23.221522 ramodels-9.7.3/ramodels/__init__.py
+-rw-r--r--   0        0        0     3107 2022-08-26 12:59:23.221522 ramodels-9.7.3/ramodels/base.py
+-rw-r--r--   0        0        0     1056 2022-08-26 12:59:23.221522 ramodels-9.7.3/ramodels/exceptions.py
+-rw-r--r--   0        0        0     1081 2022-08-26 12:59:23.221522 ramodels-9.7.3/ramodels/lora/__init__.py
+-rw-r--r--   0        0        0    20773 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/lora/_shared.py
+-rw-r--r--   0        0        0     2969 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/lora/facet.py
+-rw-r--r--   0        0        0     4322 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/lora/itsystem.py
+-rw-r--r--   0        0        0     3404 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/lora/klasse.py
+-rw-r--r--   0        0        0     3501 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/lora/organisation.py
+-rw-r--r--   0        0        0     1520 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/__init__.py
+-rw-r--r--   0        0        0    10640 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/_shared.py
+-rw-r--r--   0        0        0     1968 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/class_.py
+-rw-r--r--   0        0        0     1615 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/detail.py
+-rw-r--r--   0        0        0     3143 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/__init__.py
+-rw-r--r--   0        0        0      926 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/_shared.py
+-rw-r--r--   0        0        0     7248 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/address.py
+-rw-r--r--   0        0        0     5527 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/association.py
+-rw-r--r--   0        0        0     8163 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/engagement.py
+-rw-r--r--   0        0        0     3814 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/engagement_association.py
+-rw-r--r--   0        0        0     4186 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/it_system.py
+-rw-r--r--   0        0        0     2491 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/kle.py
+-rw-r--r--   0        0        0     2645 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/leave.py
+-rw-r--r--   0        0        0     4897 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/manager.py
+-rw-r--r--   0        0        0     1493 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/related_unit.py
+-rw-r--r--   0        0        0     2544 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/details/role.py
+-rw-r--r--   0        0        0     6357 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/employee.py
+-rw-r--r--   0        0        0     1858 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/facet.py
+-rw-r--r--   0        0        0      962 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/organisation.py
+-rw-r--r--   0        0        0     5396 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/mo/organisation_unit.py
+-rw-r--r--   0        0        0        0 2022-08-26 12:59:23.225522 ramodels-9.7.3/ramodels/py.typed
+-rw-r--r--   0        0        0     3119 2022-08-26 13:01:54.119845 ramodels-9.7.3/setup.py
+-rw-r--r--   0        0        0     2868 2022-08-26 13:01:54.120314 ramodels-9.7.3/PKG-INFO
```

### Comparing `ramodels-9.7.2/README.md` & `ramodels-9.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/pyproject.toml` & `ramodels-9.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "ramodels"
-version = "9.7.2"
+version = "9.7.3"
 description = "Pydantic data models for OS2mo"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ra-data-models"
 keywords = ["os2mo", "data models"]
```

### Comparing `ramodels-9.7.2/ramodels/base.py` & `ramodels-9.7.3/ramodels/base.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/exceptions.py` & `ramodels-9.7.3/ramodels/exceptions.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/lora/__init__.py` & `ramodels-9.7.3/ramodels/lora/__init__.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/lora/_shared.py` & `ramodels-9.7.3/ramodels/lora/_shared.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/lora/facet.py` & `ramodels-9.7.3/ramodels/lora/facet.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/lora/itsystem.py` & `ramodels-9.7.3/ramodels/lora/itsystem.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/lora/klasse.py` & `ramodels-9.7.3/ramodels/lora/klasse.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/lora/organisation.py` & `ramodels-9.7.3/ramodels/lora/organisation.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/__init__.py` & `ramodels-9.7.3/ramodels/mo/__init__.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/_shared.py` & `ramodels-9.7.3/ramodels/mo/_shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 from uuid import UUID
 from uuid import uuid4
 
-from pydantic import ConstrainedStr
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 from ramodels.base import RABase
 from ramodels.base import tz_isodate
 
 try:
@@ -380,17 +379,7 @@
             century = 1800
 
     try:
         date(year=century + year, month=month, day=day)
     except Exception:
         raise ValueError("CPR number is invalid.")
     return cpr_no
-
-
-class AlphaStr(ConstrainedStr):
-    """
-    Define custom type for string to make it
-    strict alphanumeric and min length of 1
-    Typically use in Pydantic models
-    """
-
-    regex = re.compile("^[a-zA-Z0-9_]+$")
```

### Comparing `ramodels-9.7.2/ramodels/mo/class_.py` & `ramodels-9.7.3/ramodels/mo/class_.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # --------------------------------------------------------------------------------------
 from typing import Optional
 from uuid import UUID
 
 from pydantic import Field
 from ramodels.mo._shared import MOBase
 
-from ._shared import AlphaStr
 
 # --------------------------------------------------------------------------------------
 # Code
 # --------------------------------------------------------------------------------------
 
 
 class ClassBase(MOBase):
@@ -42,10 +41,10 @@
     org_uuid: UUID = Field(description="UUID of the related organisation.")
 
 
 class ClassWrite(ClassBase):
 
     """A MO Class write object."""
 
-    name: AlphaStr = Field(description="Mo-class name.")
+    name: str = Field(description="Mo-class name.")
     facet_uuid: Optional[UUID] = Field(description="UUID of the related facet.")
     org_uuid: UUID = Field(description="UUID of the related organisation.")
```

### Comparing `ramodels-9.7.2/ramodels/mo/detail.py` & `ramodels-9.7.3/ramodels/mo/detail.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/__init__.py` & `ramodels-9.7.3/ramodels/mo/details/__init__.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/_shared.py` & `ramodels-9.7.3/ramodels/mo/details/_shared.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/address.py` & `ramodels-9.7.3/ramodels/mo/details/address.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/association.py` & `ramodels-9.7.3/ramodels/mo/details/association.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/engagement.py` & `ramodels-9.7.3/ramodels/mo/details/engagement.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/engagement_association.py` & `ramodels-9.7.3/ramodels/mo/details/engagement_association.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/it_system.py` & `ramodels-9.7.3/ramodels/mo/details/it_system.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/kle.py` & `ramodels-9.7.3/ramodels/mo/details/kle.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/leave.py` & `ramodels-9.7.3/ramodels/mo/details/leave.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/manager.py` & `ramodels-9.7.3/ramodels/mo/details/manager.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/related_unit.py` & `ramodels-9.7.3/ramodels/mo/details/related_unit.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/details/role.py` & `ramodels-9.7.3/ramodels/mo/details/role.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/employee.py` & `ramodels-9.7.3/ramodels/mo/employee.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/facet.py` & `ramodels-9.7.3/ramodels/mo/facet.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # --------------------------------------------------------------------------------------
 from typing import Optional
 from uuid import UUID
 
 from pydantic import Field
 from ramodels.mo._shared import MOBase
 
-from ._shared import AlphaStr
 
 # --------------------------------------------------------------------------------------
 # Facet models
 # --------------------------------------------------------------------------------------
 
 
 class FacetRead(MOBase):
@@ -30,12 +29,12 @@
     description: str = Field(description="Description of the facet object.", default="")
 
 
 class FacetWrite(MOBase):
     """A MO Facet write object."""
 
     type_: str = Field("facet", alias="type", description="The object type")
-    description: AlphaStr = Field(description="Description of the facet object.")
+    description: str = Field(description="Description of the facet object.")
     org_uuid: UUID = Field(description="UUID of the related organisation.")
     user_key: str = Field(description="Short, unique key.")
     published: Optional[str] = Field(description="Published state of the facet object.")
     parent_uuid: Optional[UUID] = Field(description="UUID of the parent facet.")
```

### Comparing `ramodels-9.7.2/ramodels/mo/organisation.py` & `ramodels-9.7.3/ramodels/mo/organisation.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/ramodels/mo/organisation_unit.py` & `ramodels-9.7.3/ramodels/mo/organisation_unit.py`

 * *Files identical despite different names*

### Comparing `ramodels-9.7.2/setup.py` & `ramodels-9.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0']}
 
 entry_points = \
 {'console_scripts': ['lorafetch = ramodels.fetch:gen_models']}
 
 setup_kwargs = {
     'name': 'ramodels',
-    'version': '9.7.2',
+    'version': '9.7.3',
     'description': 'Pydantic data models for OS2mo',
     'long_description': '<!--\nSPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>\nSPDX-License-Identifier: MPL-2.0\n-->\n\n\n# MoLoRa Data Models\n\nRAModels - MoLoRa data validation models powered by [pydantic](https://github.com/samuelcolvin/pydantic/#pydantic).\n\n## Versioning\nThis project uses [Semantic Versioning](https://semver.org/) with the following strategy:\n- MAJOR: Incompatible changes to existing data models\n- MINOR: Backwards compatible updates to existing data models OR new models added\n- PATCH: Backwards compatible bug fixes\n\n\n## Authors\n\nMagenta ApS <https://magenta.dk>\n\n## License\n- This project: [MPL-2.0](MPL-2.0.txt)\n- Dependencies:\n  - pydantic: [MIT](MIT.txt)\n\nThis project uses [REUSE](https://reuse.software) for licensing. All licenses can be found in the [LICENSES folder](LICENSES/) of the project.\n\n## Development\n### Prerequisites\n\n- [Poetry](https://github.com/python-poetry/poetry) \n- [Pre-commit](https://github.com/pre-commit/pre-commit)\n\n\n### Getting Started\n\n1. Clone the repository:  \n`git clone git@git.magenta.dk:rammearkitektur/ra-data-models.git`\n\n2. Install all dependencies:   \n`poetry install`\n\n3. Set up pre-commit:  \n`pre-commit install`\n\n\n### Running the tests\n\nYou use `poetry` and `pytest` to run the tests:\n\n`poetry run pytest`  \n\n  \nYou can also run specific files\n\n`poetry run pytest tests/<test_folder>/<test_file.py>`\n\nand even use filtering with `-k`\n\n`poetry run pytest -k "Manager"`\n\n  \nYou can use the flags `-vx` where `v` prints the test & `x` makes the test stop if any tests fails (Verbose, X-fail)\n\n### Pre-commit usage \nPre-commit must either be used via your virtual environment or globally.\nIf you want to pre-commit globally, the following extra dependencies are needed:  \n`pip install mypy pydantic`  \n\n\n### Models\n\n## LoRa\n`LoRa` implements the OIO standard version 1.1. The [standard](https://digitaliser.dk/resource/1569113) with\n[specification](https://www.digitaliser.dk/resource/1569113/artefact/Specifikationafserviceinterfacefororganisation-OIO-Godkendt%5bvs.1.1%5d.pdf?artefact=true&PID=1569586)\n',
     'author': 'Magenta',
     'author_email': 'info@magenta.dk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://magenta.dk/',
```

### Comparing `ramodels-9.7.2/PKG-INFO` & `ramodels-9.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramodels
-Version: 9.7.2
+Version: 9.7.3
 Summary: Pydantic data models for OS2mo
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,data models
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.8,<4.0
```

