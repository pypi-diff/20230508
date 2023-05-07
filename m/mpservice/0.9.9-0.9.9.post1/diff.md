# Comparing `tmp/mpservice-0.9.9.tar.gz` & `tmp/mpservice-0.9.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpservice-0.9.9.tar", last modified: Fri Mar 11 05:49:12 2022, max compression
+gzip compressed data, was "mpservice-0.9.9.post1.tar", last modified: Sat Mar 12 07:17:54 2022, max compression
```

## Comparing `mpservice-0.9.9.tar` & `mpservice-0.9.9.post1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1075 2022-01-26 04:20:53.037768 mpservice-0.9.9/LICENSE
--rw-r--r--   0        0        0     1369 2022-01-30 19:08:52.635830 mpservice-0.9.9/README.md
--rw-r--r--   0        0        0     1353 2022-03-11 05:15:19.501306 mpservice-0.9.9/pyproject.toml
--rw-r--r--   0        0        0       22 2022-03-11 05:22:23.916770 mpservice-0.9.9/src/mpservice/__init__.py
--rw-r--r--   0        0        0    17510 2022-03-11 05:20:07.379514 mpservice-0.9.9/src/mpservice/_async_streamer.py
--rw-r--r--   0        0        0    25761 2022-03-11 05:10:54.238652 mpservice-0.9.9/src/mpservice/_streamer.py
--rw-r--r--   0        0        0    10937 2022-01-30 17:47:58.354747 mpservice-0.9.9/src/mpservice/background_task.py
--rw-r--r--   0        0        0     2211 2022-03-11 04:16:45.062068 mpservice-0.9.9/src/mpservice/http_server.py
--rw-r--r--   0        0        0    35951 2022-03-11 05:15:08.545526 mpservice-0.9.9/src/mpservice/mpserver.py
--rw-r--r--   0        0        0        0 2021-05-08 22:58:38.592507 mpservice-0.9.9/src/mpservice/py.typed
--rw-r--r--   0        0        0     3810 2022-02-01 05:55:40.115159 mpservice-0.9.9/src/mpservice/remote_exception.py
--rw-r--r--   0        0        0     2240 2022-02-01 05:56:34.850055 mpservice-0.9.9/src/mpservice/server_process.py
--rw-r--r--   0        0        0      118 2021-11-01 18:35:31.042791 mpservice-0.9.9/src/mpservice/streamer.py
--rw-r--r--   0        0        0     2368 1970-01-01 00:00:00.000000 mpservice-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-01-26 04:20:53.037768 mpservice-0.9.9.post1/LICENSE
+-rw-r--r--   0        0        0     1369 2022-01-30 19:08:52.635830 mpservice-0.9.9.post1/README.md
+-rw-r--r--   0        0        0     1353 2022-03-11 05:15:19.501306 mpservice-0.9.9.post1/pyproject.toml
+-rw-r--r--   0        0        0       28 2022-03-12 07:00:18.111134 mpservice-0.9.9.post1/src/mpservice/__init__.py
+-rw-r--r--   0        0        0    17596 2022-03-12 07:17:28.601952 mpservice-0.9.9.post1/src/mpservice/_async_streamer.py
+-rw-r--r--   0        0        0    25761 2022-03-11 05:10:54.238652 mpservice-0.9.9.post1/src/mpservice/_streamer.py
+-rw-r--r--   0        0        0     1058 2022-03-12 07:02:30.116411 mpservice-0.9.9.post1/src/mpservice/_util.py
+-rw-r--r--   0        0        0    10937 2022-01-30 17:47:58.354747 mpservice-0.9.9.post1/src/mpservice/background_task.py
+-rw-r--r--   0        0        0     2211 2022-03-11 04:16:45.062068 mpservice-0.9.9.post1/src/mpservice/http_server.py
+-rw-r--r--   0        0        0    36623 2022-03-12 07:01:32.265604 mpservice-0.9.9.post1/src/mpservice/mpserver.py
+-rw-r--r--   0        0        0        0 2021-05-08 22:58:38.592507 mpservice-0.9.9.post1/src/mpservice/py.typed
+-rw-r--r--   0        0        0     3810 2022-02-01 05:55:40.115159 mpservice-0.9.9.post1/src/mpservice/remote_exception.py
+-rw-r--r--   0        0        0     2240 2022-02-01 05:56:34.850055 mpservice-0.9.9.post1/src/mpservice/server_process.py
+-rw-r--r--   0        0        0      118 2021-11-01 18:35:31.042791 mpservice-0.9.9.post1/src/mpservice/streamer.py
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 mpservice-0.9.9.post1/PKG-INFO
```

### Comparing `mpservice-0.9.9/LICENSE` & `mpservice-0.9.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/README.md` & `mpservice-0.9.9.post1/README.md`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/pyproject.toml` & `mpservice-0.9.9.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/src/mpservice/_async_streamer.py` & `mpservice-0.9.9.post1/src/mpservice/_async_streamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,16 @@
             except Exception as e:
                 # This should be exception while
                 # getting data from `instream`,
                 # not exception in the current object.
                 self._upstream_err = e
                 await q.put_end()
 
+        # TODO: this causes error
+        #   "Task was destroyed but it is pending!"
         self._task = asyncio.create_task(foo(self._instream, self._q, self._crashed))
 
     async def _get_next(self):
         try:
             return await self._q.__anext__()
         except StopAsyncIteration:
             if self._upstream_err is not None:
```

### Comparing `mpservice-0.9.9/src/mpservice/_streamer.py` & `mpservice-0.9.9.post1/src/mpservice/_streamer.py`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/src/mpservice/background_task.py` & `mpservice-0.9.9.post1/src/mpservice/background_task.py`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/src/mpservice/http_server.py` & `mpservice-0.9.9.post1/src/mpservice/http_server.py`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/src/mpservice/mpserver.py` & `mpservice-0.9.9.post1/src/mpservice/mpserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,33 @@
 Reference: [Service Batching from Scratch, Again](https://zpz.github.io/blog/batched-service-redesign/).
 This article describes roughly version 0.7.2.
 '''
 
 import asyncio
 import concurrent.futures
 import logging
-import multiprocessing as mp
+import multiprocessing
 import queue
 import threading
 import time
 from abc import ABCMeta, abstractmethod
-from multiprocessing import synchronize
+from multiprocessing import synchronize, Queue
 from typing import List, Type, Sequence, Union, Callable
 from uuid import uuid4
 
 import psutil  # type: ignore
 
 from .remote_exception import RemoteException
 from . import streamer
+from ._util import forward_logs, logger_thread
 
 
+# Set level for logs produced by the standard `multiprocessing` module.
+multiprocessing.log_to_stderr(logging.WARNING)
+
 logger = logging.getLogger(__name__)
 
 
 class TimeoutError(Exception):
     pass
 
 
@@ -89,30 +93,32 @@
 
 class Servlet(metaclass=ABCMeta):
     # Typically a subclass needs to enhance
     # `__init__` and implement `call`.
 
     @classmethod
     def run(cls, *,
-            q_in: mp.Queue,
-            q_out: mp.Queue,
-            q_err: mp.Queue,
+            q_in: Queue,
+            q_out: Queue,
+            q_err: Queue,
             q_in_lock: synchronize.Lock,
+            q_log: Queue,
             cpus: Sequence[int] = None,
             **init_kwargs):
         '''
         This classmethod runs in the worker process to construct
         the worker object and start its processing loop.
 
         This function is the parameter `target` to `multiprocessing.Process`
         called by `MPServer` in the main process. As such, elements
         in `init_kwargs` go through pickling, hence they should consist
         mainly of small, native types such as string, number,small dict.
         Be careful about passing custom class objects in `init_kwargs`.
         '''
+        forward_logs(q_log)
         if cpus:
             psutil.Process().cpu_affinity(cpus=cpus)
         obj = cls(**init_kwargs)
         obj.start(q_in=q_in,
                   q_out=q_out,
                   q_err=q_err,
                   q_in_lock=q_in_lock)
@@ -140,15 +146,15 @@
         the intended use case. Beware of this in benchmarking.
 
         Remember to pass in `batch_size` in accordance with the implementation
         of `call`.
 
         If the algorithm can not vectorize the computation, then there is
         no advantage in enabling batching. In that case, the subclass should
-        simple fix `batch_size` to 0 in their `__init__`.
+        simply fix `batch_size` to 0 in their `__init__`.
 
         The `__init__` of a subclass may define additional input parameters;
         they can be passed in through `run`.
         '''
         if batch_size is None or batch_size == 0:
             batch_size = 0
             if batch_wait_time is None:
@@ -164,19 +170,18 @@
             if batch_wait_time is None:
                 batch_wait_time = 0.01
             else:
                 assert batch_wait_time > 0
 
         self.batch_size = batch_size
         self.batch_wait_time = batch_wait_time
-        self.name = f'{self.__class__.__name__}--{mp.current_process().name}'
+        self.name = f'{self.__class__.__name__}--{multiprocessing.current_process().name}'
 
     def start(self, *, q_in, q_out, q_err, q_in_lock):
-        q_err.put('ready')
-        logger.info('%s started', self.name)
+        q_err.put(self.name)
         if self.batch_size > 1:
             self._start_batch(q_in=q_in, q_out=q_out, q_err=q_err,
                               q_in_lock=q_in_lock)
         else:
             self._start_single(q_in=q_in, q_out=q_out, q_err=q_err)
 
     def _start_single(self, *, q_in, q_out, q_err):
@@ -230,17 +235,16 @@
                         # If there is remaining time, wait up to
                         # that long.
                         # Otherwise, get the next item if it is there
                         # right now (i.e. no waiting) even if we
                         # are already over time. That is, if supply
                         # has piled up, then will get up to the
                         # batch capacity.
-                        if time_left > 0:
-                            # Or should we do `if time_left > 0.001`?
-                            uid, x = q_in.get(timeout=max(0.001, time_left))
+                        if time_left > 0.001:
+                            uid, x = q_in.get(timeout=time_left)
                         else:
                             uid, x = q_in.get_nowait()
                     except queue.Empty:
                         break
 
                     batch.append(x)
                     uids.append(uid)
@@ -292,19 +296,23 @@
         # If a subclass fixes `batch_size` in its `__init__` to be
         # 0 or nonzero, make sure the current method is implemented
         # accordingly. If `__init__` has no requirement on the value
         # of `batch_size`, then the current method needs to check
         # `self.batch_size` and act accordingly, because it is up to
         # the uer in `MPServer` to specify a zero or nonzero `batch_size`
         # for this worker.
+        #
+        # In case of exceptions, unless the user has specific things to do,
+        # do not handle them; just let them happen. They will be handled
+        # in `_start_batch` and `_start_single`.
         raise NotImplementedError
 
 
 class MPServer(metaclass=ABCMeta):
-    MP_CLASS = mp.get_context('spawn')
+    MP_CLASS = multiprocessing.get_context('spawn')
     # This class attribute is provided because in some cases
     # one may want to use `torch.multiprocessing`, which is
     # a drop-in replacement for the standard `multiprocessing`
     # with some enhancements related to data sharing between
     # processes.
 
     SLEEP_ENQUEUE = 0.00015
@@ -318,20 +326,22 @@
                  ):
         '''
         `cpus`: specifies the cpu for the "main process",
         i.e. the process in which this server objects resides.
         '''
         self.max_queue_size = max_queue_size or 1024
         self._q_in_lock: List[synchronize.Lock] = []
-        self._q_err: mp.Queue = self.MP_CLASS.Queue(self.max_queue_size)
+        self._q_err: Queue = self.MP_CLASS.Queue(self.max_queue_size)
+        self._q_log: Queue = self.MP_CLASS.Queue()
 
         self._t_gather_output: threading.Thread = None  # type: ignore
         self._t_gather_error: threading.Thread = None  # type: ignore
+        self._t_servlet_log: threading.Thread = None
 
-        self._servlets: List[mp.Process] = []
+        self._servlets: List[multiprocessing.Process] = []
         self._uid_to_futures = {}
 
         self.started = 0
         if cpus:
             # Pin this coordinating thread to the specified CPUs.
             psutil.Process().cpu_affinity(cpus=cpus)
 
@@ -349,44 +359,44 @@
     def start(self, sequential: bool = True):
         assert self._servlets
         self.started += 1
         if self.started > 1:
             # Re-entry.
             return
 
+        self._t_servlet_log = threading.Thread(
+            target=logger_thread, args=(self._q_log,))
+        self._t_servlet_log.start()
+
         if sequential:
             # Start the servlets one by one.
             n = len(self._servlets)
             k = 0
             for m in self._servlets:
-                print('servlet')
-                print(m)
-                print('')
-
+                logger.debug(f"starting servlet in Process {m}")
                 m.start()
-                z = self._q_err.get()
-                assert z == 'ready'
+                name = self._q_err.get()
                 k += 1
-                logger.info(f"servlet processes ready: {k}/{n}")
+                logger.info(f"{k}/{n}: servlet <{name}> is ready")
         else:
             # Start the servlets concurrently.
             # In some situations, concurrent servlet launch
             # may have issues, e.g. all servlets read the same
             # large file on startup, or all servlets download
             # the same dataset on startup.
             n = 0
             for m in self._servlets:
+                logger.debug(f"starting servlet in Process {m}")
                 m.start()
                 n += 1
             k = 0
             while k < n:
-                z = self._q_err.get()
-                assert z == 'ready'
+                name = self._q_err.get()
                 k += 1
-                logger.info(f"servlet processes ready: {k}/{n}")
+                logger.info(f"{k}/{n}: servlet <{name}> is ready")
 
         self._t_gather_output = threading.Thread(
             target=self._gather_output, name='ResultCollector')
         self._t_gather_output.start()
         self._t_gather_error = threading.Thread(
             target=self._gather_error, name='ErrorCollector')
         self._t_gather_error.start()
@@ -404,14 +414,17 @@
         self._t_gather_error = None
 
         for m in self._servlets:
             # if m.is_alive():
             m.terminate()
             m.join()
 
+        self._q_log.put(None)
+        self._t_servlet_log.join()
+
         # Reset CPU affinity.
         psutil.Process().cpu_affinity(cpus=[])
 
     async def async_call(self, x, /, *,
                          enqueue_timeout: Union[int, float] = None,
                          total_timeout: Union[int, float] = None,
                          ):
@@ -606,34 +619,36 @@
                      **init_kwargs):
         # `servlet` is the class object, not instance.
         assert not self.started
 
         q_in_lock = self.MP_CLASS.Lock()
         self._q_in_lock.append(q_in_lock)
         q_err = self._q_err
+        q_log = self._q_log
 
         cpus = self._resolve_cpus(cpus=cpus, workers=workers)
 
         name = name or 'Servlet'
 
         for cpu in cpus:
             # Pinned to the specified cpu core.
-            logger.info('adding servlet %s at CPU %s',
-                        servlet.__name__, cpu)
+            sname = f"{name}-{','.join(map(str, cpu))}"
+            logger.info('adding servlet <%s> at CPU %s', sname, cpu)
 
             self._servlets.append(
                 self.MP_CLASS.Process(
                     target=servlet.run,
-                    name=f"{name}-{','.join(map(str, cpu))}",
+                    name=sname,
                     kwargs={
                         'q_in': q_in,
                         'q_out': q_out,
                         'q_err': q_err,
                         'cpus': cpu,
                         'q_in_lock': q_in_lock,
+                        'q_log': q_log,
                         **init_kwargs,
                     },
                 )
             )
 
     def _resolve_cpus(self, *, cpus: list = None, workers: int = None):
         n_cpus = psutil.cpu_count(logical=True)
@@ -832,20 +847,20 @@
     A sequence of operations performed in order,
     the previous op's result becoming the subsequent
     op's input.
     '''
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self._q_in_out: List[mp.Queue] = [
+        self._q_in_out: List[Queue] = [
             self.MP_CLASS.Queue(self.max_queue_size)]
 
     def add_servlet(self, servlet: Type[Servlet], **kwargs):
         q_in = self._q_in_out[-1]
-        q_out: mp.Queue = self.MP_CLASS.Queue(self.max_queue_size)
+        q_out: Queue = self.MP_CLASS.Queue(self.max_queue_size)
         self._q_in_out.append(q_out)
 
         self._add_servlet(
             servlet,
             q_in=q_in,
             q_out=q_out,
             **kwargs,
@@ -886,20 +901,20 @@
     A number of operations performed on the same input
     in parallel, the list of results gathered and combined
     to form a final result.
     '''
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self._q_in: List[mp.Queue] = []
-        self._q_out: List[mp.Queue] = []
+        self._q_in: List[Queue] = []
+        self._q_out: List[Queue] = []
 
     def add_servlet(self, servlet: Type[Servlet], **kwargs):
-        q_in: mp.Queue = self.MP_CLASS.Queue(self.max_queue_size)
-        q_out: mp.Queue = self.MP_CLASS.Queue(self.max_queue_size)
+        q_in: Queue = self.MP_CLASS.Queue(self.max_queue_size)
+        q_out: Queue = self.MP_CLASS.Queue(self.max_queue_size)
         self._q_in.append(q_in)
         self._q_out.append(q_out)
 
         self._add_servlet(
             servlet,
             q_in=q_in,
             q_out=q_out,
```

### Comparing `mpservice-0.9.9/src/mpservice/remote_exception.py` & `mpservice-0.9.9.post1/src/mpservice/remote_exception.py`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/src/mpservice/server_process.py` & `mpservice-0.9.9.post1/src/mpservice/server_process.py`

 * *Files identical despite different names*

### Comparing `mpservice-0.9.9/PKG-INFO` & `mpservice-0.9.9.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpservice
-Version: 0.9.9
+Version: 0.9.9.post1
 Summary: Serving with asyncio, multiprocessing, and batching
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

