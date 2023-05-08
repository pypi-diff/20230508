# Comparing `tmp/koil-0.2.8.tar.gz` & `tmp/koil-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koil-0.2.8.tar", max compression
+gzip compressed data, was "koil-0.2.9.tar", max compression
```

## Comparing `koil-0.2.8.tar` & `koil-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3475 2022-03-02 12:09:12.548451 koil-0.2.8/README.md
--rw-r--r--   0        0        0      359 2022-04-12 08:39:04.407565 koil-0.2.8/koil/__init__.py
--rw-r--r--   0        0        0       57 2022-03-22 16:49:57.666297 koil-0.2.8/koil/composition/__init__.py
--rw-r--r--   0        0        0     2758 2022-10-11 11:58:58.915576 koil-0.2.8/koil/composition/base.py
--rw-r--r--   0        0        0     1272 2022-10-11 11:58:56.071566 koil-0.2.8/koil/composition/qt.py
--rw-r--r--   0        0        0      771 2022-07-24 13:29:13.040184 koil-0.2.8/koil/context.py
--rw-r--r--   0        0        0     2686 2022-07-05 13:55:50.386734 koil-0.2.8/koil/decorators.py
--rw-r--r--   0        0        0      601 2022-03-11 14:32:53.133337 koil-0.2.8/koil/errors.py
--rw-r--r--   0        0        0     8748 2022-09-24 10:15:45.875563 koil-0.2.8/koil/helpers.py
--rw-r--r--   0        0        0     5240 2022-07-05 13:40:38.547315 koil-0.2.8/koil/koil.py
--rw-r--r--   0        0        0     9275 2022-09-05 09:40:58.394654 koil-0.2.8/koil/qt.py
--rw-r--r--   0        0        0     4460 2022-09-23 09:20:43.931844 koil-0.2.8/koil/task.py
--rw-r--r--   0        0        0      391 2022-03-28 11:51:32.994673 koil-0.2.8/koil/types.py
--rw-r--r--   0        0        0     6824 2022-03-25 16:39:20.667020 koil-0.2.8/koil/utils.py
--rw-r--r--   0        0        0      394 2022-09-23 09:20:43.927844 koil-0.2.8/koil/vars.py
--rw-r--r--   0        0        0      946 2022-10-11 11:59:25.491670 koil-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 koil-0.2.8/setup.py
--rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 koil-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     3475 2022-03-02 12:09:12.548451 koil-0.2.9/README.md
+-rw-r--r--   0        0        0      359 2022-04-12 08:39:04.407565 koil-0.2.9/koil/__init__.py
+-rw-r--r--   0        0        0       88 2022-11-21 11:45:08.012098 koil-0.2.9/koil/composition/__init__.py
+-rw-r--r--   0        0        0     2726 2022-11-21 11:44:34.180046 koil-0.2.9/koil/composition/base.py
+-rw-r--r--   0        0        0     1052 2022-11-21 11:44:34.168046 koil-0.2.9/koil/composition/qt.py
+-rw-r--r--   0        0        0      752 2022-11-21 11:44:34.168046 koil-0.2.9/koil/context.py
+-rw-r--r--   0        0        0     2662 2022-11-21 11:44:34.176046 koil-0.2.9/koil/decorators.py
+-rw-r--r--   0        0        0      574 2022-11-21 11:44:34.164046 koil-0.2.9/koil/errors.py
+-rw-r--r--   0        0        0     8711 2022-11-21 11:44:34.196046 koil-0.2.9/koil/helpers.py
+-rw-r--r--   0        0        0     5142 2022-11-21 11:44:34.180046 koil-0.2.9/koil/koil.py
+-rw-r--r--   0        0        0     9127 2022-11-21 11:44:34.196046 koil-0.2.9/koil/qt.py
+-rw-r--r--   0        0        0     4501 2022-11-21 11:44:34.184046 koil-0.2.9/koil/task.py
+-rw-r--r--   0        0        0      391 2022-03-28 11:51:32.994673 koil-0.2.9/koil/types.py
+-rw-r--r--   0        0        0     6824 2022-03-25 16:39:20.667020 koil-0.2.9/koil/utils.py
+-rw-r--r--   0        0        0      394 2022-09-23 09:20:43.927844 koil-0.2.9/koil/vars.py
+-rw-r--r--   0        0        0      938 2022-11-21 11:46:09.980194 koil-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 koil-0.2.9/setup.py
+-rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 koil-0.2.9/PKG-INFO
```

### Comparing `koil-0.2.8/README.md` & `koil-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `koil-0.2.8/koil/composition/base.py` & `koil-0.2.9/koil/composition/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 from pydantic import BaseModel, Field, root_validator
-from pydantic.dataclasses import dataclass
 
 from koil.decorators import koilable
-from typing import Optional, Type, TypeVar
+from typing import Optional, TypeVar
 from koil.vars import *
 from koil.errors import *
 from koil.koil import *
 
 T = TypeVar("T")
 
 
@@ -20,14 +19,15 @@
     grant_sync = True
     sync_in_async = False
 
     _token = None
     _loop = None
 
     @root_validator()
+    @classmethod
     def check_not_running_in_koil(cls, values):
         if current_loop.get() is not None:
             raise ValueError(
                 f"You are already running in a Koil Loop. You cannot run a Koil Loop inside another Koil Loop. {current_loop.get()}"
             )
         try:
             asyncio.get_running_loop()
```

### Comparing `koil-0.2.8/koil/composition/qt.py` & `koil-0.2.9/koil/composition/qt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from inflection import underscore
-from pydantic import Field, dataclasses, root_validator
-from pydantic.dataclasses import dataclass
+from pydantic import Field
 from koil.composition.base import PedanticKoil
-from typing import Optional, Type, TypeVar
-from koil.koil import KoilMixin
+from typing import Optional
 
-from koil.qt import QtFuture, QtGeneratorRunner, QtKoilMixin, QtRunner, WrappedObject
+from koil.qt import QtFuture, QtKoilMixin, QtRunner
 from qtpy import QtWidgets, QtCore
 import logging
 
-from koil.task import KoilFuture
 
 logger = logging.getLogger(__name__)
 
 
 class QtPedanticKoil(PedanticKoil, QtKoilMixin):
     parent: Optional[QtWidgets.QWidget] = Field(exclude=True)
```

### Comparing `koil-0.2.8/koil/context.py` & `koil-0.2.9/koil/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from contextvars import ContextVar
 
 
-import contextvars
 
 
 class Context:
     def __init__(self, value):
         self.__value: ContextVar = value
 
     def set(self, value):
```

### Comparing `koil-0.2.8/koil/decorators.py` & `koil-0.2.9/koil/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from operator import ge
 from koil.helpers import unkoil
 from koil.koil import Koil
 import inspect
 from typing import Callable, Type, TypeVar
 from koil.vars import current_loop
 import logging
```

### Comparing `koil-0.2.8/koil/errors.py` & `koil-0.2.9/koil/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 class KoilError(Exception):
     pass
 
 
 class KoilStopIteration(Exception):
     """Wrapper around StopIteration as it interacts badly with Futures"""
 
-    pass
 
 
 class ContextError(KoilError):
     pass
 
 
 class ThreadCancelledError(KoilError):
     """Mimics ayncio.CancelledError for threads if they accept cancellation. This should only
     be raised from within a thread that was spawned by koil."""
 
-    pass
 
 
 class CancelledError(KoilError):
     """Mimics ayncio.CancelledError for futures that are living in a koiled loop. Catch this
     as if you would catch asyncio.CancelledError."""
 
-    pass
```

### Comparing `koil-0.2.8/koil/helpers.py` & `koil-0.2.9/koil/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import threading
 
 import janus
 from koil.errors import (
-    CancelledError,
     KoilError,
     KoilStopIteration,
     ThreadCancelledError,
 )
 from koil.task import KoilFuture, KoilRunner
 from koil.utils import run_threaded_with_context
 from koil.vars import *
@@ -186,15 +185,14 @@
     except asyncio.CancelledError as e:
         cancel_event.set()
 
         try:
             await asyncio.wait_for(f, timeout=cancel_timeout)
         except ThreadCancelledError:
             logging.info("Future in another thread was sucessfully cancelled")
-            pass
         except asyncio.TimeoutError as te:
             raise KoilError(
                 f"We could not successfully cancel the future {f} another thread. Make sure you are not blocking the thread with a long running task and check if you check_cancelled every now and then"
             ) from te
 
         raise e
```

### Comparing `koil-0.2.8/koil/koil.py` & `koil-0.2.9/koil/koil.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import asyncio
 from contextlib import contextmanager
 from dataclasses import dataclass
 import os
 import sys
 import threading
-from typing import Any, Optional, Type
+from typing import Any, Optional
 
-from pydantic import BaseModel, Field
 from koil.errors import ContextError
 from koil.vars import *
-from koil.task import KoilFuture, KoilRunner
 import time
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 try:
@@ -173,8 +171,7 @@
     uvify: bool = False
     """Shoul we spawn a new thread for each task?"""
 
     name: str = "KoilLoop"
     """How would you like to name this loop"""
 
     force_lonely: bool = False
-    pass
```

### Comparing `koil-0.2.8/koil/qt.py` & `koil-0.2.9/koil/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import asyncio
 import contextvars
 import inspect
 import logging
 import threading
-import uuid
-from asyncio.futures import Future
-from concurrent import futures
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import Callable, Generic, TypeVar
 
-from qtpy import QtCore, QtGui, QtWidgets
-from qtpy.QtCore import QObject, QThread, Signal
-from typing_extensions import ParamSpec, final
+from qtpy import QtCore, QtWidgets
+from typing_extensions import ParamSpec
 
 from koil.koil import Koil, KoilMixin
 from koil.task import KoilFuture, KoilGeneratorRunner, KoilRunner, KoilYieldFuture
 from koil.utils import (
     iterate_threaded_with_context_and_signals,
     run_threaded_with_context_and_signals,
 )
```

### Comparing `koil-0.2.8/koil/task.py` & `koil-0.2.9/koil/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import contextvars
 import logging
-import asyncio
 import threading
-import time
-from typing import AsyncIterator, Awaitable, Callable, Coroutine, Generic, TypeVar
+from typing import AsyncIterator, Awaitable, Callable, Generic, TypeVar
 from koil.errors import CancelledError
 from koil.vars import current_cancel_event, current_loop
 import inspect
 from .utils import run_threaded_with_context
-from typing_extensions import ParamSpec, final
+from typing_extensions import ParamSpec
 import concurrent.futures
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
@@ -114,14 +111,15 @@
         assert inspect.iscoroutinefunction(coro), "Task is not a coroutine"
 
     def run(self, *args: P.args, **kwargs: P.kwargs):
         args = self.args + args
         kwargs = {**self.kwargs, **kwargs}
 
         loop = current_loop.get()
+        assert loop is not None, "No loop found"
         assert loop.is_running(), "Loop is not running"
         assert not loop.is_closed(), "Loop is closed"
         cancel_event = threading.Event()
         future = run_threaded_with_context(
             self.coro, loop, cancel_event, *args, **kwargs
         )
         return KoilFuture(future, cancel_event, self)
@@ -139,13 +137,14 @@
         self.args = args
         self.kwargs = kwargs
         self.task = None
         assert inspect.isasyncgenfunction(iterator), "Task is not a async iterator"
 
     def run(self, *args: P.args, **kwargs: P.kwargs):
         loop = current_loop.get()
+        assert loop is not None, "No koiled loop found"
         assert loop.is_running(), "Loop is not running"
         assert not loop.is_closed(), "Loop is closed"
         ait = self.iterator(*self.args, **self.kwargs).__aiter__()
         res = [False, False]
         cancel_event = current_cancel_event.get()
         raise NotImplementedError("No design decision was taken")
```

### Comparing `koil-0.2.8/koil/utils.py` & `koil-0.2.9/koil/utils.py`

 * *Files identical despite different names*

### Comparing `koil-0.2.8/setup.py` & `koil-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['janus>=1.0.0,<2.0.0']
 
 extras_require = \
 {'uvloop': ['uvloop>=0.16.0,<0.17.0']}
 
 setup_kwargs = {
     'name': 'koil',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Async for a sync world',
     'long_description': '# koil\n\n[![codecov](https://codecov.io/gh/jhnnsrs/koil/branch/master/graph/badge.svg?token=UGXEA2THBV)](https://codecov.io/gh/jhnnsrs/koil)\n[![PyPI version](https://badge.fury.io/py/koil.svg)](https://pypi.org/project/koil/)\n![Maintainer](https://img.shields.io/badge/maintainer-jhnnsrs-blue)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/koil.svg)](https://pypi.python.org/pypi/koil/)\n[![PyPI status](https://img.shields.io/pypi/status/koil.svg)](https://pypi.python.org/pypi/koil/)\n[![PyPI download day](https://img.shields.io/pypi/dm/koil.svg)](https://pypi.python.org/pypi/koil/)\n\n### DEVELOPMENT\n\n# Quick Start\n\nLet\'s discover **Koil in less than 5 minutes**.\n\n### Inspiration\n\nkoil is an abstraction layer for threaded asyncio to enable "sensible defaults" for\nprogrammers working with frameworks that are barely compatible with asyncio (originally developped to get around pyqt5)\n\n### Main Concept\n\nAsync libraries are amazing, and its an ecosystem rapidly increasing, however in some contexts it still doesn\'t seem like\nthe way to go and the burden of learning these concepts might be to high. However you developed a wonderful async api\nthat you want to share with the world.\n\n```python\nclass AmazingAsyncAPI:\n    def __init__(self) -> None:\n        pass\n\n    async def sleep(self):\n        await asyncio.sleep(0.01)\n        return "the-glory-of-async"\n\n    async def __aenter__(self):\n        # amazing connection logic\n        return self\n\n    async def __aexit__(self, *args, **kwargs):\n        # amazing tear down logic\n        return self\n\n```\n\nHowever if somebody wants to use this api in sync environment they are in for a good one, as a call to asyncio.run() just wont do the trick.\n\n```python\nfrom koil import koilable, unkoilable\n\n@koilable()\nclass AmazingAsyncAPI:\n    def __init__(self) -> None:\n        pass\n\n    @unkoilable()\n    async def sleep(self):\n        await asyncio.sleep(0.01)\n        return "the-glory-of-async"\n\n    async def __aenter__(self):\n        # amazing connection logic\n        return self\n\n    async def __aexit__(self, *args, **kwargs):\n        # amazing tear down logic\n        return self\n\n```\n\nAnd now it works. Just use your Api with a normal context manager.\n\n```python\nwith AmazingAsyncAPI as e:\n  print(e.sleep())\n```\n\nKoil under the hood spawns a new event loop in another thread, calls functions that are marked with unkoilable\nthreadsafe in that loop and returns the result, when exiting it shuts down the loop in the other thread.\n\nIf you have multiple context managers or tasks that you would just like to run in another thread, you can\nalso create a loop in another thread\n\n```python\n\nasync def task(arg):\n       x = await ...\n       return x\n\nwith Koil(): # creates a threaded loop\n\n    x = unkoil(task, 1)\n\n    with AmazingAsyncAPI as e:\n       print(e.sleep())\n\n```\n\nMoreover koil also is able to be used with generators\n\n```python\nimport asyncio\nfrom koil import unkoil_gen\n\nasync def task(arg):\n    for i in range(0,20)\n      await asyncio.sleep(1)\n      yield arg\n\n\nwith Koil(): # creates a threaded loop\n\n    for x in unkoil_gen(task, 1):\n        print(x)\n\n```\n\nAnd finally koil is able to create task like objects,\n\n```python\nasync def task(arg):\n    await asyncio.sleep(2)\n    return arg\n\nwith Koil():\n\n  x = unkoil(task, 1, as_task=True)\n\n  # do other stuff\n\n  if x.done():\n      print(x)\n\n```\n\n## PyQt Support\n\n... Documentation coming soon...\n\n### Installation\n\n```bash\npip install koil\n```\n',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `koil-0.2.8/PKG-INFO` & `koil-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koil
-Version: 0.2.8
+Version: 0.2.9
 Summary: Async for a sync world
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

