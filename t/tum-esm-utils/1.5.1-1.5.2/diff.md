# Comparing `tmp/tum_esm_utils-1.5.1.tar.gz` & `tmp/tum_esm_utils-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-1.5.1.tar", max compression
+gzip compressed data, was "tum_esm_utils-1.5.2.tar", max compression
```

## Comparing `tum_esm_utils-1.5.1.tar` & `tum_esm_utils-1.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.5.1/LICENSE
--rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.5.1/README.md
--rw-r--r--   0        0        0     1308 2023-05-03 12:50:51.133586 tum_esm_utils-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      337 2023-05-03 12:46:16.731010 tum_esm_utils-1.5.1/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0      580 2023-05-03 12:45:06.065729 tum_esm_utils-1.5.1/tum_esm_utils/context.py
--rw-r--r--   0        0        0     3177 2023-04-15 14:16:07.544110 tum_esm_utils-1.5.1/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1094 2023-05-03 12:45:35.585219 tum_esm_utils-1.5.1/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     3672 2023-05-03 12:37:22.874116 tum_esm_utils-1.5.1/tum_esm_utils/files.py
--rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.5.1/tum_esm_utils/github.py
--rw-r--r--   0        0        0       64 2023-04-25 03:34:37.353328 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-04-25 03:08:42.468142 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-04-25 02:57:45.344815 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0     4437 2023-04-25 03:34:11.213272 tum_esm_utils-1.5.1/tum_esm_utils/interferograms.py
--rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.5.1/tum_esm_utils/logger.py
--rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.5.1/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.5.1/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.5.1/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     2856 2023-05-03 12:02:45.055012 tum_esm_utils-1.5.1/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.5.1/tum_esm_utils/system.py
--rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.5.1/tum_esm_utils/testing.py
--rw-r--r--   0        0        0     3129 2023-04-17 17:44:42.149505 tum_esm_utils-1.5.1/tum_esm_utils/text.py
--rw-r--r--   0        0        0     6777 2023-04-17 17:41:44.557063 tum_esm_utils-1.5.1/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.1/setup.py
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1480 2023-05-08 20:48:53.107394 tum_esm_utils-1.5.2/README.md
+-rw-r--r--   0        0        0     1405 2023-05-08 20:50:40.883720 tum_esm_utils-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      484 2023-05-08 20:20:03.808107 tum_esm_utils-1.5.2/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0      661 2023-05-08 20:26:45.351232 tum_esm_utils-1.5.2/tum_esm_utils/context.py
+-rw-r--r--   0        0        0     3252 2023-05-08 20:27:26.142823 tum_esm_utils-1.5.2/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1174 2023-05-08 20:28:19.090171 tum_esm_utils-1.5.2/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     3877 2023-05-08 20:30:33.784545 tum_esm_utils-1.5.2/tum_esm_utils/files.py
+-rw-r--r--   0        0        0      717 2023-05-08 20:35:56.495234 tum_esm_utils-1.5.2/tum_esm_utils/github.py
+-rw-r--r--   0        0        0       64 2023-04-25 03:34:37.353328 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/.gitignore
+-rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
+-rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_prepro4.F90
+-rw-r--r--   0        0        0    28408 2023-04-25 03:08:42.468142 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.F90
+-rw-r--r--   0        0        0      758 2023-04-25 02:57:45.344815 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.template.inp
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec.dat
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec2.dat
+-rw-r--r--   0        0        0     4860 2023-05-08 20:38:33.304237 tum_esm_utils-1.5.2/tum_esm_utils/interferograms.py
+-rw-r--r--   0        0        0     7975 2023-05-08 20:39:29.079052 tum_esm_utils-1.5.2/tum_esm_utils/logger.py
+-rw-r--r--   0        0        0      380 2023-05-08 20:39:43.895368 tum_esm_utils-1.5.2/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0     1696 2023-05-08 20:40:10.752208 tum_esm_utils-1.5.2/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.5.2/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     3098 2023-05-08 20:41:20.520764 tum_esm_utils-1.5.2/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1465 2023-05-08 20:42:11.004755 tum_esm_utils-1.5.2/tum_esm_utils/system.py
+-rw-r--r--   0        0        0     1276 2023-05-08 20:43:17.097835 tum_esm_utils-1.5.2/tum_esm_utils/testing.py
+-rw-r--r--   0        0        0     3362 2023-05-08 20:45:20.705055 tum_esm_utils-1.5.2/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     6912 2023-05-08 20:46:28.696498 tum_esm_utils-1.5.2/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.2/setup.py
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.2/PKG-INFO
```

### Comparing `tum_esm_utils-1.5.1/LICENSE` & `tum_esm_utils-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/pyproject.toml` & `tum_esm_utils-1.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_utils"
-version = "1.5.1"
+version = "1.5.2"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = ["Moritz Makowski <moritz.makowski@tum.de>"]
 readme = "README.md"
 packages = [
     {include = "tum_esm_utils"},
     {include = "tum_esm_utils/py.typed"}
 ]
@@ -50,10 +50,17 @@
 ]
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 no_warn_unused_ignores = true
 
+[[tool.mypy.overrides]]
+module = [
+    "pendulum",
+    "polars"
+]
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/context.py` & `tum_esm_utils-1.5.2/tum_esm_utils/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Context managers for common tasks.
+
+Implements: `ensure_section_duration`"""
+
 from contextlib import contextmanager
 import time
 from typing import Generator
 
 
 @contextmanager
 def ensure_section_duration(duration: float) -> Generator[None, None, None]:
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/datastructures.py` & `tum_esm_utils-1.5.2/tum_esm_utils/datastructures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Datastructures not in the standard library.
+
+Implements: `RingList`"""
+
 from typing import Any
 
 
 class RingList:
     def __init__(self, max_size: int):
         assert max_size > 0, "a max_size of zero doesn't make any sense"
         self._max_size: int = max_size
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/decorators.py` & `tum_esm_utils-1.5.2/tum_esm_utils/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Decorators that can be used wrap functions.
+
+Implements: `with_filelock`"""
+
 import filelock
 from typing import Any, Callable, TypeVar, cast
 from functools import wraps
 
 # typing of higher level decorators:
 # https://github.com/python/mypy/issues/1551#issuecomment-253978622
 F = TypeVar("F", bound=Callable[..., Any])
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/files.py` & `tum_esm_utils-1.5.2/tum_esm_utils/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""File-related utility functions.
+
+Implements: `load_file`, `dump_file`, `load_json_file`,
+`dump_json_file`, `get_parent_dir_path`, `get_dir_checksum`,
+`get_file_checksum`, `load_raw_proffast_output`"""
+
 import hashlib
 import json
 import os
 from typing import Any, Optional
 import polars as pl
 import tum_esm_utils
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_OPUSparms.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_prepro4.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp` & `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.template.inp`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/interferograms.py` & `tum_esm_utils-1.5.2/tum_esm_utils/interferograms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Functions for interacting with interferograms.
+
+Implements: `detect_corrupt_ifgs`"""
+
 import os
 import re
 import subprocess
 from typing import Literal
 
 from filelock import FileLock
 import tum_esm_utils
@@ -44,15 +48,22 @@
 
 def detect_corrupt_ifgs(
     ifg_directory: str,
     silent: bool = True,
     fortran_compiler: Literal["gfortran", "gfortran-9"] = "gfortran",
 ) -> dict[str, list[str]]:
     """Returns dict[filename, list[error_messages]] for all
-    corrupt interferograms in the given directory."""
+    corrupt interferograms in the given directory.
+
+    It will compile the fortran code using a given compiler
+    to perform this task. The fortran code is derived from
+    the preprocess source code of Proffast 2
+    (https://www.imk-asf.kit.edu/english/3225.php). We use
+    it because the retrieval using Proffast 2 will fail if
+    there are corrupt interferograms in the input."""
 
     # compiling fortran code
     _compile_fortran_code(silent=silent, fortran_compiler=fortran_compiler)
 
     # generate input file
     ifgs = [f"{ifg_directory}/{x}" for x in os.listdir(ifg_directory)]
     ifgs = list(sorted(list(filter(os.path.isfile, ifgs))))
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/logger.py` & `tum_esm_utils-1.5.2/tum_esm_utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implements custom logging functionality, because the
+standard logging module is hard to configure for special
+cases.
+
+Implements: `Logger`"""
+
 import os
 import sys
 import traceback
 from datetime import datetime, timedelta
 from typing import Literal, Optional
 import filelock
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/processes.py` & `tum_esm_utils-1.5.2/tum_esm_utils/processes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""Functions to start and terminate background processes.
+
+Implements: `get_process_pids`, `start_background_process`,
+`terminate_process`"""
+
 import os
 import time
 import psutil
 
 
 def get_process_pids(script_path: str) -> list[int]:
     """Return a list of PIDs that have the given script as their entrypoint"""
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/shell.py` & `tum_esm_utils-1.5.2/tum_esm_utils/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implements custom logging functionality, because the
+standard logging module is hard to configure for special
+cases.
+
+Implements: `run_shell_command`, `CommandLineException`,
+`get_hostname`, `get_commit_sha`, `change_file_permissions`"""
+
 import os
 import re
 import subprocess
 from typing import Callable, Optional
 
 
 class CommandLineException(Exception):
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/text.py` & `tum_esm_utils-1.5.2/tum_esm_utils/text.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Functions used for text manipulation/processing.
+
+Implements: `get_random_string`, `pad_string`, `is_date_string`,
+`date_range`, `is_datetime_string`, `is_rfc3339_datetime_string`,
+`date_is_too_recent`, `insert_replacements`."""
+
 from datetime import datetime
 import random
 import string
 from typing import Literal
 import pendulum
```

### Comparing `tum_esm_utils-1.5.1/tum_esm_utils/validators.py` & `tum_esm_utils-1.5.2/tum_esm_utils/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from datetime import datetime
+"""Implements validator functions for use with pydantic models.
+
+Implements: `validate_bool`, `validate_float`, `validate_int`,
+`validate_str`, `validate_list`"""
+
+
 import os
 import re
 from typing import Any, Callable, Optional, TypeVar
 
 import pendulum
```

