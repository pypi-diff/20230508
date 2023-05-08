# Comparing `tmp/robocorp_excel-0.2.0.tar.gz` & `tmp/robocorp_excel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_excel-0.2.0.tar", max compression
+gzip compressed data, was "robocorp_excel-0.3.0.tar", max compression
```

## Comparing `robocorp_excel-0.2.0.tar` & `robocorp_excel-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       25 2023-04-04 11:49:45.059148 robocorp_excel-0.2.0/README.md
--rw-r--r--   0        0        0      615 2023-04-25 10:40:48.282657 robocorp_excel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-25 10:39:03.644567 robocorp_excel-0.2.0/src/robocorp/excel/__init__.py
--rw-r--r--   0        0        0      598 2023-04-25 10:39:03.644677 robocorp_excel-0.2.0/src/robocorp/excel/_types.py
--rw-r--r--   0        0        0    23104 2023-04-25 10:39:03.645036 robocorp_excel-0.2.0/src/robocorp/excel/_workbooks.py
--rw-r--r--   0        0        0     2639 2023-04-25 10:39:03.645269 robocorp_excel-0.2.0/src/robocorp/excel/excel.py
--rw-r--r--   0        0        0    65743 2023-04-25 10:39:03.645757 robocorp_excel-0.2.0/src/robocorp/excel/tables.py
--rw-r--r--   0        0        0     2854 2023-04-25 10:39:03.645940 robocorp_excel-0.2.0/src/robocorp/excel/workbook.py
--rw-r--r--   0        0        0     5425 2023-04-25 10:39:03.646107 robocorp_excel-0.2.0/src/robocorp/excel/worksheet.py
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 robocorp_excel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-04-28 10:50:56.515006 robocorp_excel-0.3.0/README.md
+-rw-r--r--   0        0        0      795 2023-05-08 12:42:11.457457 robocorp_excel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-05-08 08:00:21.916838 robocorp_excel-0.3.0/src/robocorp/excel/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-28 10:50:56.515921 robocorp_excel-0.3.0/src/robocorp/excel/_types.py
+-rw-r--r--   0        0        0    23102 2023-05-08 08:00:22.936249 robocorp_excel-0.3.0/src/robocorp/excel/_workbooks.py
+-rw-r--r--   0        0        0     2638 2023-05-08 08:00:22.944749 robocorp_excel-0.3.0/src/robocorp/excel/excel.py
+-rw-r--r--   0        0        0    65719 2023-05-08 08:00:22.956149 robocorp_excel-0.3.0/src/robocorp/excel/tables.py
+-rw-r--r--   0        0        0     2854 2023-05-08 08:00:22.939148 robocorp_excel-0.3.0/src/robocorp/excel/workbook.py
+-rw-r--r--   0        0        0     5425 2023-05-08 08:00:22.947620 robocorp_excel-0.3.0/src/robocorp/excel/worksheet.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 robocorp_excel-0.3.0/PKG-INFO
```

### Comparing `robocorp_excel-0.2.0/pyproject.toml` & `robocorp_excel-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 [tool.poetry]
 name = "robocorp-excel"
-version = "0.2.0"
+version = "0.3.0"
 description = "Robocorp Excel automation library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
-    "Antero V. <antero@robocorp.com>",
+	"Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pillow = "^9.1.1"
 xlrd = "^2.0.1"
 xlwt = "^1.3.0"
 xlutils = "^2.0.0"
 openpyxl = "^3.0.9"
+typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = ".."}
+black = "^23.1.0"
+ruff = "^0.0.255"
+mypy = "^1.1.1"
+pytest = "^7.2.2"
+pytest-xdist = "^3.2.1"
+pytest-regressions = "1.0.6"
+lazydocs = "^0.4.8"
+pydocstyle = "^6.3.0"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_excel-0.2.0/src/robocorp/excel/_types.py` & `robocorp_excel-0.3.0/src/robocorp/excel/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.2.0/src/robocorp/excel/_workbooks.py` & `robocorp_excel-0.3.0/src/robocorp/excel/_workbooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import logging
 import pathlib
 from collections import defaultdict
 from contextlib import contextmanager
 from io import BytesIO
 from typing import Any, List, Optional, Union
 
-
 import openpyxl
 import xlrd
 import xlwt
-
-from xlutils.copy import copy as xlutils_copy
-from openpyxl.worksheet.cell_range import CellRange
 from openpyxl.utils import get_column_letter
 from openpyxl.utils.exceptions import InvalidFileException
+from openpyxl.worksheet.cell_range import CellRange
+from xlutils.copy import copy as xlutils_copy
 
 from robocorp.excel._types import PathType
 from robocorp.excel.tables import Table
 from robocorp.excel.worksheet import Worksheet
 
 
 def _get_column_index(column: str) -> int:
```

### Comparing `robocorp_excel-0.2.0/src/robocorp/excel/excel.py` & `robocorp_excel-0.3.0/src/robocorp/excel/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Literal, Optional
 
 from robocorp.excel._types import PathType
-
 from robocorp.excel._workbooks import XlsWorkbook, XlsxWorkbook, _load_workbook
 from robocorp.excel.workbook import Workbook
 
 
 def create_workbook(
     fmt: Literal["xlsx", "xls"] = "xlsx",
     sheet_name: Optional[str] = None,
```

### Comparing `robocorp_excel-0.2.0/src/robocorp/excel/tables.py` & `robocorp_excel-0.3.0/src/robocorp/excel/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,30 +4,19 @@
 import re
 from collections import OrderedDict, namedtuple
 from enum import Enum
 from itertools import groupby, zip_longest
 from keyword import iskeyword
 from numbers import Number
 from operator import itemgetter
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generator,
-    Iterable,
-    List,
-    NamedTuple,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import (Any, Callable, Dict, Generator, Iterable, List, NamedTuple,
+                    Optional, Tuple, Union)
 
 from robocorp.excel._types import is_dict_like, is_list_like, is_namedtuple
 
-
 Index = Union[int, str]
 Column = Union[int, str]
 Row = Union[Dict, List, Tuple, NamedTuple, set]
 Data = Optional[Union[Dict[Column, Row], List[Row], "Table"]]
 CellCondition = Callable[[Any], bool]
 RowCondition = Callable[[Union[Index, Row]], bool]
```

### Comparing `robocorp_excel-0.2.0/src/robocorp/excel/workbook.py` & `robocorp_excel-0.3.0/src/robocorp/excel/workbook.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from io import BytesIO
 from typing import Any, List, Optional, Union
 
 from robocorp.excel._types import PathType
-from robocorp.excel.worksheet import Worksheet
 from robocorp.excel._workbooks import XlsWorkbook, XlsxWorkbook
+from robocorp.excel.worksheet import Worksheet
 
 
 class Workbook:
     """Manager class for both .xls and .xlsx Excel files."""
 
     def __init__(self, excel: Union[XlsWorkbook, XlsxWorkbook]):
         # Internal API, for users there is create_ and open_ workbook functions
```

### Comparing `robocorp_excel-0.2.0/src/robocorp/excel/worksheet.py` & `robocorp_excel-0.3.0/src/robocorp/excel/worksheet.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from PIL import Image
-
 from typing import TYPE_CHECKING, Any, List, Optional, Union
+
+from PIL import Image
 from typing_extensions import deprecated
-from robocorp.excel._types import PathType
 
+from robocorp.excel._types import PathType
 from robocorp.excel.tables import Table, Tables
 
 if TYPE_CHECKING:
     from robocorp.excel.workbook import Workbook
 
 
 class Worksheet:
```

### Comparing `robocorp_excel-0.2.0/PKG-INFO` & `robocorp_excel-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: robocorp-excel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Robocorp Excel automation library
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pillow (>=9.1.1,<10.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Requires-Dist: xlutils (>=2.0.0,<3.0.0)
 Requires-Dist: xlwt (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Robocorp excel library
```

