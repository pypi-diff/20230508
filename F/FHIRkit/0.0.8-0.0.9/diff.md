# Comparing `tmp/FHIRkit-0.0.8.tar.gz` & `tmp/FHIRkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FHIRkit-0.0.8.tar", last modified: Sun May  1 06:26:16 2022, max compression
+gzip compressed data, was "FHIRkit-0.0.9.tar", last modified: Sun May  1 06:52:01 2022, max compression
```

## Comparing `FHIRkit-0.0.8.tar` & `FHIRkit-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/
--rw-r--r--   0 axelvanraes   (501) staff       (20)      569 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/PKG-INFO
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1094 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/LICENSE.md
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/FHIRkit.egg-info/
--rw-r--r--   0 axelvanraes   (501) staff       (20)      569 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/FHIRkit.egg-info/PKG-INFO
--rw-r--r--   0 axelvanraes   (501) staff       (20)      699 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/FHIRkit.egg-info/SOURCES.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)       18 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/FHIRkit.egg-info/requires.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)        8 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/FHIRkit.egg-info/top_level.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)        1 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/FHIRkit.egg-info/dependency_links.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)      100 2022-02-08 13:17:47.000000 FHIRkit-0.0.8/pyproject.toml
--rw-r--r--   0 axelvanraes   (501) staff       (20)       71 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/README.md
--rw-r--r--   0 axelvanraes   (501) staff       (20)      656 2022-05-01 06:26:02.000000 FHIRkit-0.0.8/setup.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)       38 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/setup.cfg
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/fhirkit/
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1248 2022-05-01 06:23:40.000000 FHIRkit-0.0.8/fhirkit/OperationOutcome.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     5440 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/ChoiceTypeMixin.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1318 2022-05-01 06:22:32.000000 FHIRkit-0.0.8/fhirkit/Bundle.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     2620 2022-05-01 06:23:24.000000 FHIRkit-0.0.8/fhirkit/Observation.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1962 2022-04-22 12:20:17.000000 FHIRkit-0.0.8/fhirkit/Server.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     5922 2022-05-01 06:22:43.000000 FHIRkit-0.0.8/fhirkit/CodeSystem.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     4852 2022-05-01 06:22:51.000000 FHIRkit-0.0.8/fhirkit/elements.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     4845 2022-05-01 06:24:50.000000 FHIRkit-0.0.8/fhirkit/ValueSet.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     3861 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/Resource.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      365 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/__init__.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      181 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/metadata_types.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      411 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/data_types.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     2090 2022-05-01 06:25:21.000000 FHIRkit-0.0.8/fhirkit/Procedure.py
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:26:16.000000 FHIRkit-0.0.8/fhirkit/snomed/
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1742 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/snomed/elements.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     3515 2022-05-01 06:25:05.000000 FHIRkit-0.0.8/fhirkit/snomed/ValueSet.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      125 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/snomed/__init__.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)       35 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/snomed/consts.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     7387 2022-04-22 13:40:46.000000 FHIRkit-0.0.8/fhirkit/snomed/terminology.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      381 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/CompositionValueSet.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1254 2022-04-22 12:20:17.000000 FHIRkit-0.0.8/fhirkit/SimpleFHIRServer.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     2668 2022-04-22 12:04:21.000000 FHIRkit-0.0.8/fhirkit/Parameter.py
+drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.336513 FHIRkit-0.0.9/
+drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.332555 FHIRkit-0.0.9/FHIRkit.egg-info/
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      538 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/PKG-INFO
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      699 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/SOURCES.txt
+-rw-r--r--   0 axelvanraes   (501) staff       (20)        1 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/dependency_links.txt
+-rw-r--r--   0 axelvanraes   (501) staff       (20)       18 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/requires.txt
+-rw-r--r--   0 axelvanraes   (501) staff       (20)        8 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/top_level.txt
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     1094 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/LICENSE.md
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      538 2022-05-01 06:52:01.336158 FHIRkit-0.0.9/PKG-INFO
+-rw-r--r--   0 axelvanraes   (501) staff       (20)       71 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/README.md
+drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.335141 FHIRkit-0.0.9/fhirkit/
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     1318 2022-05-01 06:22:32.000000 FHIRkit-0.0.9/fhirkit/Bundle.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     5440 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/ChoiceTypeMixin.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     5944 2022-05-01 06:51:03.000000 FHIRkit-0.0.9/fhirkit/CodeSystem.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      381 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/CompositionValueSet.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     2620 2022-05-01 06:23:24.000000 FHIRkit-0.0.9/fhirkit/Observation.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     1248 2022-05-01 06:23:40.000000 FHIRkit-0.0.9/fhirkit/OperationOutcome.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     2668 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/Parameter.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     2090 2022-05-01 06:25:21.000000 FHIRkit-0.0.9/fhirkit/Procedure.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     4487 2022-05-01 06:50:11.000000 FHIRkit-0.0.9/fhirkit/Resource.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     1962 2022-04-22 12:20:17.000000 FHIRkit-0.0.9/fhirkit/Server.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     1254 2022-04-22 12:20:17.000000 FHIRkit-0.0.9/fhirkit/SimpleFHIRServer.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     4873 2022-05-01 06:50:33.000000 FHIRkit-0.0.9/fhirkit/ValueSet.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      365 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/__init__.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      411 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/data_types.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     4949 2022-05-01 06:50:00.000000 FHIRkit-0.0.9/fhirkit/elements.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      181 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/metadata_types.py
+drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.335923 FHIRkit-0.0.9/fhirkit/snomed/
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     3515 2022-05-01 06:25:05.000000 FHIRkit-0.0.9/fhirkit/snomed/ValueSet.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      125 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/snomed/__init__.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)       35 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/snomed/consts.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     1742 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/snomed/elements.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)     7387 2022-04-22 13:40:46.000000 FHIRkit-0.0.9/fhirkit/snomed/terminology.py
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      100 2022-02-08 13:17:47.000000 FHIRkit-0.0.9/pyproject.toml
+-rw-r--r--   0 axelvanraes   (501) staff       (20)       38 2022-05-01 06:52:01.336572 FHIRkit-0.0.9/setup.cfg
+-rw-r--r--   0 axelvanraes   (501) staff       (20)      656 2022-05-01 06:51:44.000000 FHIRkit-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `FHIRkit-0.0.8/LICENSE.md` & `FHIRkit-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/FHIRkit.egg-info/SOURCES.txt` & `FHIRkit-0.0.9/FHIRkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/setup.py` & `FHIRkit-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 setup(
     name="FHIRkit",
-    version="0.0.8",
+    version="0.0.9",
     description="Toolkit to handle FHIR Resources in a more efficient, pythonic way.",
     long_description=open("README.md").read(),
     url="",
     author="",
     author_email="",
     license="MIT",
     classifiers=classifiers,
```

### Comparing `FHIRkit-0.0.8/fhirkit/OperationOutcome.py` & `FHIRkit-0.0.9/fhirkit/OperationOutcome.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/ChoiceTypeMixin.py` & `FHIRkit-0.0.9/fhirkit/ChoiceTypeMixin.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/Bundle.py` & `FHIRkit-0.0.9/fhirkit/Bundle.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/Observation.py` & `FHIRkit-0.0.9/fhirkit/Observation.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/Server.py` & `FHIRkit-0.0.9/fhirkit/Server.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/CodeSystem.py` & `FHIRkit-0.0.9/fhirkit/CodeSystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from pydantic import AnyUrl, Field, StrictBool, StrictStr, validator
-from fhirkit.Resource import DomainResource
+from fhirkit.Resource import CanonicalResource, DomainResource
 from fhirkit.ChoiceTypeMixin import ChoiceTypeMixinBase, validate_choice_types
 from fhirkit.elements import (
     BackboneElement,
     CodeableConcept,
     Coding,
     Identifier,
     UsageContext,
@@ -103,15 +103,15 @@
 ) -> Generator[C, None, None]:
     for c in s:
         yield c
         if len(c.concept) > 0:
             yield from traverse_concepts(c.concept)
 
 
-class CodeSystem(DomainResource):
+class CodeSystem(CanonicalResource):
     resourceType = Field("CodeSystem", const=True)
     url: Optional[AnyUrl]
     identifier: Sequence[Identifier] = []
     version: Optional[str]
     name: Optional[str]
     title: Optional[str]
     status: Literal["draft", "active", "retired", "unknown"]
```

### Comparing `FHIRkit-0.0.8/fhirkit/elements.py` & `FHIRkit-0.0.9/fhirkit/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,19 @@
         Literal["phone", "fax", "email", "pager", "url", "sms", "other"]
     ] = None
     value: Optional[str] = None
     use: Optional[Literal["home", "work", "temp", "old", "mobile"]] = None
     period: Period
 
 
+class ContactDetail(Element):
+    name: Optional[str]
+    telecom: Sequence[ContactPoint] = []
+
+
 class UsageContextValueChoiceType(ChoiceTypeMixinBase):
     _choice_type_fields: ClassVar[Set[str]] = [
         "valueQuantity",
         "valueRange",
         "valueCodeableConcept",
         "valueReference",
     ]
```

### Comparing `FHIRkit-0.0.8/fhirkit/ValueSet.py` & `FHIRkit-0.0.9/fhirkit/ValueSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 from typing import Iterable, List, Optional, Sequence, Union
 from pydantic import AnyUrl, BaseModel, Field, HttpUrl
 from fhirkit.data_types import dateTime
 from fhirkit.elements import BackboneElement, CodeableConcept, Coding, UsageContext
-from fhirkit.Resource import Resource
+from fhirkit.Resource import CanonicalResource, Resource
 
 
 class VSDesignation(BaseModel):
     language: Optional[str]
     use: Optional[Coding]
     value: str
 
@@ -66,15 +66,15 @@
     offset: Optional[int]
     total: Optional[int]
     contains: List[VSCodingWithDesignation] = []
     identifier: Optional[AnyUrl] = None
     timestamp: dateTime = Field(default_factory=datetime.now)
 
 
-class ValueSet(Resource):
+class ValueSet(CanonicalResource):
     resourceType = Field("ValueSet", const=True)
     url: Optional[AnyUrl]
     name: Optional[str]
     compose: Optional[VSCompose]
     expansion: Optional[VSExpansion]
     useContext: Sequence[UsageContext] = Field([], repr=True)
```

### Comparing `FHIRkit-0.0.8/fhirkit/Resource.py` & `FHIRkit-0.0.9/fhirkit/Resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,26 @@
     Set,
     Tuple,
     Union,
     Generator,
 )
 from pydantic import AnyUrl, BaseModel, HttpUrl, Field, PrivateAttr
 from fhirkit.Server import AbstractFHIRTerminologyServer
-from fhirkit.data_types import Code, Id, Instant
-from fhirkit.elements import BackboneElement, Element, Narrative, Extension, Coding
+from fhirkit.data_types import Code, Id, Instant, dateTime
+from fhirkit.elements import (
+    BackboneElement,
+    CodeableConcept,
+    ContactDetail,
+    Element,
+    Identifier,
+    Narrative,
+    Extension,
+    Coding,
+    UsageContext,
+)
 from fhirkit.ChoiceTypeMixin import AbstractChoiceTypeMixin
 
 
 class Meta(BaseModel):
     versionId: Optional[Id]
     lastUpdated: Optional[Instant]
     source: Optional[AnyUrl]
@@ -119,7 +129,25 @@
 
 
 class DomainResource(Resource):
     text: Optional[Narrative] = Field(None, repr=False)
     contained: Sequence[Resource] = Field([], repr=False)
     extension: Sequence[Extension] = Field([], repr=False)
     modifierExtension: Sequence[Extension] = Field([], repr=False)
+
+
+class CanonicalResource(DomainResource):
+    url: Optional[AnyUrl]
+    identifier: Sequence[Identifier] = []
+    version: Optional[str]
+    name: Optional[str]
+    title: Optional[str]
+    status: Code
+    experimental: Optional[bool]
+    date: Optional[dateTime]
+    publisher: Optional[str]
+    contact: Sequence[ContactDetail] = []
+    description: Optional[str]
+    useContext: Sequence[UsageContext] = []
+    jurisdiction: Sequence[CodeableConcept] = []
+    purpose: Optional[str]
+    copyright: Optional[str]
```

### Comparing `FHIRkit-0.0.8/fhirkit/Procedure.py` & `FHIRkit-0.0.9/fhirkit/Procedure.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/snomed/elements.py` & `FHIRkit-0.0.9/fhirkit/snomed/elements.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/snomed/ValueSet.py` & `FHIRkit-0.0.9/fhirkit/snomed/ValueSet.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/snomed/terminology.py` & `FHIRkit-0.0.9/fhirkit/snomed/terminology.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/SimpleFHIRServer.py` & `FHIRkit-0.0.9/fhirkit/SimpleFHIRServer.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.8/fhirkit/Parameter.py` & `FHIRkit-0.0.9/fhirkit/Parameter.py`

 * *Files identical despite different names*

