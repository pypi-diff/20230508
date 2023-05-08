# Comparing `tmp/xknxproject-3.0.0.tar.gz` & `tmp/xknxproject-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xknxproject-3.0.0.tar", last modified: Tue Apr 25 21:17:44 2023, max compression
+gzip compressed data, was "xknxproject-3.1.0.tar", last modified: Mon May  8 19:58:19 2023, max compression
```

## Comparing `xknxproject-3.0.0.tar` & `xknxproject-3.1.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-25 21:17:26.000000 xknxproject-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 21:17:26.000000 xknxproject-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-04-25 21:17:44.387534 xknxproject-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-25 21:17:26.000000 xknxproject-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 21:17:26.000000 xknxproject-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-25 21:17:44.387534 xknxproject-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.383534 xknxproject-3.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 21:17:26.000000 xknxproject-3.0.0/test/test_knxproj.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 21:17:26.000000 xknxproject-3.0.0/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.383534 xknxproject-3.0.0/xknxproject/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/application_program_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/hardware_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/knx_master_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/loader/project_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/models/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/knxproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/models/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/xknxproj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/xml/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/xml/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.387534 xknxproject-3.0.0/xknxproject/zip/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-25 21:17:26.000000 xknxproject-3.0.0/xknxproject/zip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:17:44.383534 xknxproject-3.0.0/xknxproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-04-25 21:17:43.000000 xknxproject-3.0.0/xknxproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-25 21:17:44.000000 xknxproject-3.0.0/xknxproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:17:43.000000 xknxproject-3.0.0/xknxproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 21:17:44.000000 xknxproject-3.0.0/xknxproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 21:17:44.000000 xknxproject-3.0.0/xknxproject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-08 19:58:00.000000 xknxproject-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 19:58:00.000000 xknxproject-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-05-08 19:58:19.546286 xknxproject-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-08 19:58:00.000000 xknxproject-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-08 19:58:00.000000 xknxproject-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 19:58:19.546286 xknxproject-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 19:58:00.000000 xknxproject-3.1.0/test/test_knxproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 19:58:00.000000 xknxproject-3.1.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/combination/combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/application_program_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/hardware_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/knx_master_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/project_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/knxproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/xknxproj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/xml/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/zip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-05-08 19:58:18.000000 xknxproject-3.1.0/xknxproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 19:58:19.000000 xknxproject-3.1.0/xknxproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:58:18.000000 xknxproject-3.1.0/xknxproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 19:58:19.000000 xknxproject-3.1.0/xknxproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 19:58:19.000000 xknxproject-3.1.0/xknxproject.egg-info/top_level.txt
```

### Comparing `xknxproject-3.0.0/LICENSE` & `xknxproject-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/PKG-INFO` & `xknxproject-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.0.0
+Version: 3.1.0
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.0.0/README.md` & `xknxproject-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/pyproject.toml` & `xknxproject-3.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -113,7 +113,29 @@
 [tool.pylint.reports]
 score = "no"
 output-format = "colorized"
 
 
 [tool.pytest.ini_options]
 testpaths = "test"
+
+[tool.ruff]
+target-version = "py39"
+select = [
+  "C4",  # comprehensions
+  "D",   # pydocstyle
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "RUF", # ruff specific
+  "T20", # print
+  "UP",  # pyupgrade
+  "W",   # pydocstyle warning
+]
+ignore = [
+  "D202",
+  "D203",
+  "D212",
+  "E501", # line too long
+]
+extend-exclude = [
+  "script",
+]
```

### Comparing `xknxproject-3.0.0/test/test_knxproj.py` & `xknxproject-3.1.0/test/test_knxproj.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test parsing ETS projects."""
+
 from xknxproject import XKNXProj
 
 from . import RESOURCES_PATH
 from .conftest import assert_stub
 
 
 def test_parse_project_ets5():
```

### Comparing `xknxproject-3.0.0/test/test_util.py` & `xknxproject-3.1.0/test/test_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 """Test utilities."""
 import pytest
 
-from xknxproject.util import parse_dpt_type
+from xknxproject.util import get_dpt_type, parse_dpt_types
 
 
 @pytest.mark.parametrize(
     ("dpt_string", "expected"),
     [
         ("DPT-1", {"main": 1, "sub": None}),
-        ("DPT-1 DPST-1-1", {"main": 1, "sub": 1}),
-        ("DPT-7 DPST-7-1", {"main": 7, "sub": 1}),
+        ("DPT-1 DPST-1-1", {"main": 1, "sub": None}),
+        ("DPT-7 DPST-7-1", {"main": 7, "sub": None}),
         ("DPST-5-1", {"main": 5, "sub": 1}),
-        ("DPT-1 DPT-5", {"main": 5, "sub": None}),
-        ("DPT-14 DPST-14-1", {"main": 14, "sub": 1}),
+        ("DPT-1 DPT-5", {"main": 1, "sub": None}),
+        ("DPT-14 DPST-14-1", {"main": 14, "sub": None}),
         ("DPST-6-10", {"main": 6, "sub": 10}),
         ("Wrong", None),
         ("DPT-Wrong", None),
         ("DPST-1-Wrong", None),
         ("DPST-5", None),
         ([], None),
         (None, None),
     ],
 )
-def test_parse_dpt_type(dpt_string, expected):
-    """Test parsing of DPT from ETS project."""
-    assert parse_dpt_type(dpt_string) == expected
+def test_get_dpt_type(dpt_string, expected):
+    """Test parsing single DPT from ETS project."""
+    assert get_dpt_type(dpt_string) == expected
+
+
+@pytest.mark.parametrize(
+    ("dpt_string", "expected"),
+    [
+        ("DPT-1", [{"main": 1, "sub": None}]),
+        ("DPT-1 DPST-1-1", [{"main": 1, "sub": None}, {"main": 1, "sub": 1}]),
+        ("DPT-7 DPST-7-1", [{"main": 7, "sub": None}, {"main": 7, "sub": 1}]),
+        ("DPST-5-1", [{"main": 5, "sub": 1}]),
+        ("DPT-1 DPT-5", [{"main": 1, "sub": None}, {"main": 5, "sub": None}]),
+        ("DPT-14 DPST-14-1", [{"main": 14, "sub": None}, {"main": 14, "sub": 1}]),
+        ("DPST-6-10", [{"main": 6, "sub": 10}]),
+        ("Wrong", []),
+        ("DPT-Wrong", []),
+        ("DPST-1-Wrong", []),
+        ("DPST-5", []),
+        ([], []),
+        (None, []),
+    ],
+)
+def test_parse_dpt_types(dpt_string, expected):
+    """Test parsing list of DPT from ETS project."""
+    assert parse_dpt_types(dpt_string) == expected
```

### Comparing `xknxproject-3.0.0/xknxproject/loader/application_program_loader.py` & `xknxproject-3.1.0/xknxproject/loader/application_program_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Iterator
 import logging
 from typing import Any
 from xml.etree import ElementTree
 from zipfile import Path
 
 from xknxproject.models import ComObject, ComObjectRef, DeviceInstance
-from xknxproject.util import parse_dpt_type, parse_xml_flag
+from xknxproject.util import parse_dpt_types, parse_xml_flag
 
 _LOGGER = logging.getLogger("xknxproject.log")
 
 
 class ApplicationProgramLoader:
     """Load the application program from KNX XML."""
 
@@ -135,15 +135,15 @@
             object_size=elem.get("ObjectSize"),  # type: ignore[arg-type]
             read_flag=parse_xml_flag(elem.get("ReadFlag"), False),
             write_flag=parse_xml_flag(elem.get("WriteFlag"), False),
             communication_flag=parse_xml_flag(elem.get("CommunicationFlag"), False),
             transmit_flag=parse_xml_flag(elem.get("TransmitFlag"), False),
             update_flag=parse_xml_flag(elem.get("UpdateFlag"), False),
             read_on_init_flag=parse_xml_flag(elem.get("ReadOnInitFlag"), False),
-            datapoint_type=parse_dpt_type(elem.get("DatapointType")),
+            datapoint_types=parse_dpt_types(elem.get("DatapointType")),
         )
 
     @staticmethod
     def parse_com_object_ref(
         elem: ElementTree.Element,
         identifier: str,
     ) -> ComObjectRef:
@@ -157,15 +157,15 @@
             object_size=elem.get("ObjectSize"),
             read_flag=parse_xml_flag(elem.get("ReadFlag")),
             write_flag=parse_xml_flag(elem.get("WriteFlag")),
             communication_flag=parse_xml_flag(elem.get("CommunicationFlag")),
             transmit_flag=parse_xml_flag(elem.get("TransmitFlag")),
             update_flag=parse_xml_flag(elem.get("UpdateFlag")),
             read_on_init_flag=parse_xml_flag(elem.get("ReadOnInitFlag")),
-            datapoint_type=parse_dpt_type(elem.get("DatapointType")),
+            datapoint_types=parse_dpt_types(elem.get("DatapointType")),
         )
 
     @staticmethod
     def apply_translations(
         com_objects: dict[str, ComObject] | dict[str, ComObjectRef],
         translation_map: dict[str, dict[str, str]],
     ) -> None:
```

### Comparing `xknxproject-3.0.0/xknxproject/loader/hardware_loader.py` & `xknxproject-3.1.0/xknxproject/loader/hardware_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/xknxproject/loader/knx_master_loader.py` & `xknxproject-3.1.0/xknxproject/loader/knx_master_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/xknxproject/loader/project_loader.py` & `xknxproject-3.1.0/xknxproject/loader/project_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     SpaceType,
     XMLArea,
     XMLGroupAddress,
     XMLLine,
     XMLProjectInformation,
     XMLSpace,
 )
-from xknxproject.util import parse_dpt_type, parse_xml_flag
+from xknxproject.util import get_dpt_type, parse_dpt_types, parse_xml_flag
 from xknxproject.zip import KNXProjContents
 
 
 class ProjectLoader:
     """Load Project file."""
 
     @staticmethod
@@ -81,15 +81,15 @@
 
         return XMLGroupAddress(
             name=group_address_element.get("Name", ""),
             identifier=group_address_element.get("Id", ""),
             address=group_address_element.get("Address", ""),
             project_uid=int(group_address_element.get("Puid")),  # type: ignore[arg-type]
             description=group_address_element.get("Description", ""),
-            dpt=parse_dpt_type(group_address_element.get("DatapointType")),
+            dpt=get_dpt_type(group_address_element.get("DatapointType")),
         )
 
 
 class _TopologyLoader:
     """Load topology from KNX XML."""
 
     @staticmethod
@@ -187,15 +187,15 @@
             function_text=com_object.get("FunctionText"),
             read_flag=parse_xml_flag(com_object.get("ReadFlag")),
             write_flag=parse_xml_flag(com_object.get("WriteFlag")),
             communication_flag=parse_xml_flag(com_object.get("CommunicationFlag")),
             transmit_flag=parse_xml_flag(com_object.get("TransmitFlag")),
             update_flag=parse_xml_flag(com_object.get("UpdateFlag")),
             read_on_init_flag=parse_xml_flag(com_object.get("ReadOnInitFlag")),
-            datapoint_type=parse_dpt_type(com_object.get("DatapointType")),
+            datapoint_types=parse_dpt_types(com_object.get("DatapointType")),
             description=com_object.get("Description"),
             links=links.split(" "),
         )
 
 
 class _LocationLoader:
     """Load location infos from KNX XML."""
```

### Comparing `xknxproject-3.0.0/xknxproject/models/__init__.py` & `xknxproject-3.1.0/xknxproject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/xknxproject/models/knxproject.py` & `xknxproject-3.1.0/xknxproject/models/knxproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     name: str
     number: int
     text: str
     function_text: str
     description: str
     device_address: str
-    dpt: DPTType | None
+    dpts: list[DPTType]
     object_size: str
     group_address_links: list[str]
     flags: Flags
 
 
 class Device(TypedDict):
     """Devices dictionary."""
```

### Comparing `xknxproject-3.0.0/xknxproject/models/models.py` & `xknxproject-3.1.0/xknxproject/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Handles Group adresses."""
+"""Define internally used data structures."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 import re
 
 from xknxproject.models.knxproject import DPTType
 from xknxproject.models.static import SpaceType
@@ -132,29 +132,29 @@
     function_text: str | None  # "FunctionText"
     read_flag: bool | None  # "ReadFlag" - knx:Enable_t
     write_flag: bool | None  # "WriteFlag" - knx:Enable_t
     communication_flag: bool | None  # "CommunicationFlag" - knx:Enable_t
     transmit_flag: bool | None  # "TransmitFlag" - knx:Enable_t
     update_flag: bool | None  # "UpdateFlag" - knx:Enable_t
     read_on_init_flag: bool | None  # "ReadOnInitFlag" - knx:Enable_t
-    datapoint_type: DPTType | None  # "DataPointType" - knx:IDREFS
+    datapoint_types: list[DPTType]  # "DataPointType" - knx:IDREFS
     description: str | None  # "Description" - language dependent
     links: list[str] | None  # "Links" - knx:RELIDREFS
 
     # resolved via Hardware.xml from the containing DeviceInstance
     com_object_ref_id: str | None = None
 
     # only available form ComObject and ComObjectRef
     name: str | None = None
     number: int | None = None
     object_size: str | None = None
 
     def resolve_com_object_ref_id(self, application_program_ref: str) -> None:
         """Prepend the ref_id with the application program ref."""
-        # Remove module and ModuleInstance occurence as they will not be in the application program directly
+        # Remove module and ModuleInstance occurrence as they will not be in the application program directly
         ref_id = re.sub(r"(M-\d+?_MI-\d+?_)", "", self.ref_id)
         self.com_object_ref_id = f"{application_program_ref}_{ref_id}"
 
     def merge_from_application(self, com_object: ComObject | ComObjectRef) -> None:
         """Fill missing information with information parsed from the application program."""
         if self.name is None:
             self.name = com_object.name
@@ -172,16 +172,16 @@
             self.communication_flag = com_object.communication_flag
         if self.transmit_flag is None:
             self.transmit_flag = com_object.transmit_flag
         if self.update_flag is None:
             self.update_flag = com_object.update_flag
         if self.read_on_init_flag is None:
             self.read_on_init_flag = com_object.read_on_init_flag
-        if self.datapoint_type is None:
-            self.datapoint_type = com_object.datapoint_type
+        if not self.datapoint_types:
+            self.datapoint_types = com_object.datapoint_types
         if isinstance(com_object, ComObject):
             self.number = com_object.number
 
 
 @dataclass
 class ComObject:
     """Class that represents a ComObject instance."""
@@ -195,15 +195,15 @@
         "object_size",
         "read_flag",
         "write_flag",
         "communication_flag",
         "transmit_flag",
         "update_flag",
         "read_on_init_flag",
-        "datapoint_type",
+        "datapoint_types",
     )
 
     # all items required in the XML
     identifier: str  # "Id" - xs:ID
     name: str  # "Name"
     text: str  # "Text" - language dependent
     number: int  # "Number" - xs:unsignedInt
@@ -211,15 +211,15 @@
     object_size: str  # "ObjectSize" - knx:ComObjectSize_t
     read_flag: bool  # "ReadFlag" - knx:Enable_t
     write_flag: bool  # "WriteFlag" - knx:Enable_t
     communication_flag: bool  # "CommunicationFlag" - knx:Enable_t
     transmit_flag: bool  # "TransmitFlag" - knx:Enable_t
     update_flag: bool  # "UpdateFlag" - knx:Enable_t
     read_on_init_flag: bool  # "ReadOnInitFlag" - knx:Enable_t
-    datapoint_type: DPTType | None  # "DataPointType" - knx:IDREFS - optional
+    datapoint_types: list[DPTType]  # "DataPointType" - knx:IDREFS - optional
 
 
 @dataclass
 class ComObjectRef:
     """Class that represents a ComObjectRef instance."""
 
     __slots__ = (
@@ -231,30 +231,30 @@
         "object_size",
         "read_flag",
         "write_flag",
         "communication_flag",
         "transmit_flag",
         "update_flag",
         "read_on_init_flag",
-        "datapoint_type",
+        "datapoint_types",
     )
 
     identifier: str  # "Id" - xs:ID - required
     ref_id: str  # "RefId" - knx:IDREF - required - points to a ComObject Id
     name: str | None  # "Name"
     text: str | None  # "Text" - language dependent
     function_text: str | None  # "FunctionText" - language dependent
     object_size: str | None  # "ObjectSize" - knx:ComObjectSize_t
     read_flag: bool | None  # "ReadFlag" - knx:Enable_t
     write_flag: bool | None  # "WriteFlag" - knx:Enable_t
     communication_flag: bool | None  # "CommunicationFlag" - knx:Enable_t
     transmit_flag: bool | None  # "TransmitFlag" - knx:Enable_t
     update_flag: bool | None  # "UpdateFlag" - knx:Enable_t
     read_on_init_flag: bool | None  # "ReadOnInitFlag" - knx:Enable_t
-    datapoint_type: DPTType | None  # "DataPointType" - knx:IDREFS
+    datapoint_types: list[DPTType]  # "DataPointType" - knx:IDREFS
 
 
 @dataclass
 class XMLSpace:
     """A space in the location XML."""
 
     identifier: str
```

### Comparing `xknxproject-3.0.0/xknxproject/models/static.py` & `xknxproject-3.1.0/xknxproject/models/static.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/xknxproject/xknxproj.py` & `xknxproject-3.1.0/xknxproject/xknxproj.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 import time
 
 from xknxproject.__version__ import __version__
+from xknxproject.combination import combine_project
 from xknxproject.models import KNXProject
 from xknxproject.xml import XMLParser
 from xknxproject.zip.extractor import extract
 
 _LOGGER = logging.getLogger("xknxproject.log")
 
 
@@ -23,26 +24,29 @@
         language: str | None = None,
     ):
         """Initialize a KNXProjParser."""
         self.path = Path(path)
         self.password = password
         self.language = language
 
-    def parse(self) -> KNXProject:
+    def parse(self, combine: bool = True) -> KNXProject:
         """Parse the KNX project."""
         _LOGGER.info(
             'Xknxproject version %s parsing "%s" with%s password...',
             __version__,
             self.path,
             "" if self.password else "out",
         )
         _start = time.time()
         with extract(self.path, self.password) as knx_project_content:
             project = XMLParser(knx_project_content).parse(self.language)
 
+        if combine:
+            project = combine_project(project)
+
         _LOGGER.info("Parsing took %s seconds", time.time() - _start)
         _LOGGER.info(
             "Found %s group addresses, %s devices and %s used communication objects",
             len(project["group_addresses"]),
             len(project["devices"]),
             len(project["communication_objects"]),
         )
```

### Comparing `xknxproject-3.0.0/xknxproject/xml/parser.py` & `xknxproject-3.1.0/xknxproject/xml/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                     communication_objects[com_object_key] = CommunicationObject(
                         name=com_object.name,  # type: ignore[typeddict-item]
                         number=com_object.number,  # type: ignore[typeddict-item]
                         text=com_object.text,  # type: ignore[typeddict-item]
                         function_text=com_object.function_text,  # type: ignore[typeddict-item]
                         description=com_object.description or "",
                         device_address=device.individual_address,
-                        dpt=com_object.datapoint_type,
+                        dpts=com_object.datapoint_types,
                         object_size=com_object.object_size,  # type: ignore[typeddict-item]
                         flags=Flags(
                             read=com_object.read_flag,  # type: ignore[typeddict-item]
                             write=com_object.write_flag,  # type: ignore[typeddict-item]
                             communication=com_object.communication_flag,  # type: ignore[typeddict-item]
                             update=com_object.update_flag,  # type: ignore[typeddict-item]
                             read_on_init=com_object.read_on_init_flag,  # type: ignore[typeddict-item]
```

### Comparing `xknxproject-3.0.0/xknxproject/zip/extractor.py` & `xknxproject-3.1.0/xknxproject/zip/extractor.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.0.0/xknxproject.egg-info/PKG-INFO` & `xknxproject-3.1.0/xknxproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.0.0
+Version: 3.1.0
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.0.0/xknxproject.egg-info/SOURCES.txt` & `xknxproject-3.1.0/xknxproject.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 xknxproject/util.py
 xknxproject/xknxproj.py
 xknxproject.egg-info/PKG-INFO
 xknxproject.egg-info/SOURCES.txt
 xknxproject.egg-info/dependency_links.txt
 xknxproject.egg-info/requires.txt
 xknxproject.egg-info/top_level.txt
+xknxproject/combination/__init__.py
+xknxproject/combination/combination.py
 xknxproject/exceptions/__init__.py
 xknxproject/exceptions/exceptions.py
 xknxproject/loader/__init__.py
 xknxproject/loader/application_program_loader.py
 xknxproject/loader/hardware_loader.py
 xknxproject/loader/knx_master_loader.py
 xknxproject/loader/project_loader.py
```

