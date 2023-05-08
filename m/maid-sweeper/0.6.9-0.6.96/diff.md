# Comparing `tmp/maid-sweeper-0.6.9.tar.gz` & `tmp/maid-sweeper-0.6.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maid-sweeper-0.6.9.tar", last modified: Sun May  7 20:22:16 2023, max compression
+gzip compressed data, was "maid-sweeper-0.6.96.tar", last modified: Mon May  8 03:33:40 2023, max compression
```

## Comparing `maid-sweeper-0.6.9.tar` & `maid-sweeper-0.6.96.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:16.113524 maid-sweeper-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-07 20:22:16.113524 maid-sweeper-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:22:16.113524 maid-sweeper-0.6.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:16.109523 maid-sweeper-0.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:16.109523 maid-sweeper-0.6.9/src/maid_sweeper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:16.109523 maid-sweeper-0.6.9/src/maid_sweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/common/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/common/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:16.113524 maid-sweeper-0.6.9/src/maid_sweeper/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/dispatchers/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/dispatchers/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/dispatchers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/dispatchers/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-07 20:22:05.000000 maid-sweeper-0.6.9/src/maid_sweeper/maid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:16.109523 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-07 20:22:16.000000 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-07 20:22:16.000000 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:22:16.000000 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 20:22:16.000000 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 20:22:16.000000 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 20:22:16.000000 maid-sweeper-0.6.9/src/maid_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:33:40.470452 maid-sweeper-0.6.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-08 03:33:40.470452 maid-sweeper-0.6.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:33:40.470452 maid-sweeper-0.6.96/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:33:40.466452 maid-sweeper-0.6.96/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:33:40.466452 maid-sweeper-0.6.96/src/maid_sweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/src/maid_sweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/src/maid_sweeper/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/src/maid_sweeper/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/src/maid_sweeper/maid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-08 03:33:29.000000 maid-sweeper-0.6.96/src/maid_sweeper/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:33:40.470452 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-08 03:33:40.000000 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-08 03:33:40.000000 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:33:40.000000 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 03:33:40.000000 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 03:33:40.000000 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 03:33:40.000000 maid-sweeper-0.6.96/src/maid_sweeper.egg-info/top_level.txt
```

### Comparing `maid-sweeper-0.6.9/LICENSE` & `maid-sweeper-0.6.96/LICENSE`

 * *Files identical despite different names*

### Comparing `maid-sweeper-0.6.9/PKG-INFO` & `maid-sweeper-0.6.96/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 Metadata-Version: 2.1
 Name: maid-sweeper
-Version: 0.6.9
+Version: 0.6.96
 Summary: A maid that sweeps your files
 Author-email: noirgif <nomaru@outlook.com>
 Project-URL: Homepage, https://github.com/noirgif/maid-sweeper
 Project-URL: Bug Tracker, https://github.com/noirgif/maid-sweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Maid Sweeper for files
 
 Instead of cleaning the unused files, it calls a maid to label them and sweep them under the rug accordingly.
 
 However, the maid can practice Danshari given permission. For example, she can [sell your unused iPad for money](https://comic-days.com/episode/3269754496647364302).
 
+Like Toki, she has two modes:
+
+`tag`: Label the files/directories automatically, based on their types and names.
+
+- code projects and application directories are labeled, and their children are not scanned
+- others are labeled based on the extensions
+
+`sweep`: Carry out actions based on the labels`.
+
 ## Feature
 
-* Asyncio
-* MongoDB
-* Not scanning every single file inside code and program directories, saving time
-    * Avoid accessing metadata
+* AsyncIO, so all operations are in parallel
+* MongoDB for fast indexing
+* Save time by not scanning every single file inside code and program directories and not checking the metadata
 * Kyoufu
 
 ## Installation
 
-1. Have Python 3.11 (as it used some fancy type hints that is incompatible with <3.11).
-2. Install the requirements by running `pip install .`.
+1. Have Python 3.10.
+2. Install by running `pip install maid-sweeper`.
 
 ## Usage
 
 1. Start a MongoDB instance.
-2. Run `python maid.py tag D:\Study`, then you can find tagged entries in Database 'sweep_maid' Collection 'file_metadata'. Then it can be used for further processing.
-3. Run `python maid.py sweep video,game rm -rf {}`, the maid is going to remove all 'video' or 'game' tagged files and directories.
-    * As `fire` is used, it is about the best we can get, without custom deserializer 
-
-## TO-DO
-
-- [ ] Remove type hints
-- [ ] Better readme
-- [ ] Tag based on time
+2. Run `maid-sweeper tag D:\Study`, then you can find tagged entries in the database. Sweeping works on all directories tagged.
+3. Run `maid-sweeper sweep -t video game -x del \q \f {}`, and the maid is going to remove all 'video' or 'game' tagged files and directories.
+    * Any other commands is OK as well
+    * By default the maid will do a sweep -- remove all those files. Kyoufu!
+
+## Ideas
+
+- Multithreading
+- Remove type hints
+- Tags based on time
     * How does it affect other tags? If not why bother?
     * Maybe not tag, but just metadata
     * There will be IO cost
-- [ ] Group similar named files
-- [x] Automatically carry out actions based on the tags, like Dan, Sha and Ri, etc.
-- [ ] Understand human language so they can toss away garbage
-
-- [x] Better command line interface
-    * have to escape {} for fire
-- [ ] Optionally clean up the database after sweeping.
-- [ ] Single line mode: do the tag, sweep, and clean up database entries with a single command.
+- Group similarly named files: 01.jpg, 02.jpg, etc.
+- Understand human language so they can toss away garbage
+- Optionally clean up the database after sweeping.
+- Single line mode: do the tag, sweep, and clean up database entries with a single command.
+- Allow users to specify tags
```

### Comparing `maid-sweeper-0.6.9/README.md` & `maid-sweeper-0.6.96/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 # Maid Sweeper for files
 
 Instead of cleaning the unused files, it calls a maid to label them and sweep them under the rug accordingly.
 
 However, the maid can practice Danshari given permission. For example, she can [sell your unused iPad for money](https://comic-days.com/episode/3269754496647364302).
 
+Like Toki, she has two modes:
+
+`tag`: Label the files/directories automatically, based on their types and names.
+
+- code projects and application directories are labeled, and their children are not scanned
+- others are labeled based on the extensions
+
+`sweep`: Carry out actions based on the labels`.
+
 ## Feature
 
-* Asyncio
-* MongoDB
-* Not scanning every single file inside code and program directories, saving time
-    * Avoid accessing metadata
+* AsyncIO, so all operations are in parallel
+* MongoDB for fast indexing
+* Save time by not scanning every single file inside code and program directories and not checking the metadata
 * Kyoufu
 
 ## Installation
 
-1. Have Python 3.11 (as it used some fancy type hints that is incompatible with <3.11).
-2. Install the requirements by running `pip install .`.
+1. Have Python 3.10.
+2. Install by running `pip install maid-sweeper`.
 
 ## Usage
 
 1. Start a MongoDB instance.
-2. Run `python maid.py tag D:\Study`, then you can find tagged entries in Database 'sweep_maid' Collection 'file_metadata'. Then it can be used for further processing.
-3. Run `python maid.py sweep video,game rm -rf {}`, the maid is going to remove all 'video' or 'game' tagged files and directories.
-    * As `fire` is used, it is about the best we can get, without custom deserializer 
-
-## TO-DO
-
-- [ ] Remove type hints
-- [ ] Better readme
-- [ ] Tag based on time
+2. Run `maid-sweeper tag D:\Study`, then you can find tagged entries in the database. Sweeping works on all directories tagged.
+3. Run `maid-sweeper sweep -t video game -x del \q \f {}`, and the maid is going to remove all 'video' or 'game' tagged files and directories.
+    * Any other commands is OK as well
+    * By default the maid will do a sweep -- remove all those files. Kyoufu!
+
+## Ideas
+
+- Multithreading
+- Remove type hints
+- Tags based on time
     * How does it affect other tags? If not why bother?
     * Maybe not tag, but just metadata
     * There will be IO cost
-- [ ] Group similar named files
-- [x] Automatically carry out actions based on the tags, like Dan, Sha and Ri, etc.
-- [ ] Understand human language so they can toss away garbage
-
-- [x] Better command line interface
-    * have to escape {} for fire
-- [ ] Optionally clean up the database after sweeping.
-- [ ] Single line mode: do the tag, sweep, and clean up database entries with a single command.
+- Group similarly named files: 01.jpg, 02.jpg, etc.
+- Understand human language so they can toss away garbage
+- Optionally clean up the database after sweeping.
+- Single line mode: do the tag, sweep, and clean up database entries with a single command.
+- Allow users to specify tags
```

### Comparing `maid-sweeper-0.6.9/pyproject.toml` & `maid-sweeper-0.6.96/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maid-sweeper"
-version = "0.6.9"
+version = "0.6.96"
 authors = [
   { name="noirgif", email="nomaru@outlook.com" },
 ]
 description = "A maid that sweeps your files"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'nest-asyncio',
-    'pymongo',
+    'motor',
+    'certifi'
 ]
 
 [project.scripts]
 maid-sweeper = "maid_sweeper.maid:main"
 
 [project.urls]
 "Homepage" = "https://github.com/noirgif/maid-sweeper"
```

### Comparing `maid-sweeper-0.6.9/src/maid_sweeper/common/patterns.py` & `maid-sweeper-0.6.96/src/maid_sweeper/patterns.py`

 * *Files identical despite different names*

### Comparing `maid-sweeper-0.6.9/src/maid_sweeper/maid.py` & `maid-sweeper-0.6.96/src/maid_sweeper/maid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,157 @@
 import argparse
 import asyncio
-from concurrent.futures import ThreadPoolExecutor
 import logging
-from pathlib import Path
 import sys
 import tracemalloc
+from concurrent.futures import ThreadPoolExecutor
+from pathlib import Path
 from typing import Awaitable, Callable, ParamSpec, TypeVar
-import motor.motor_asyncio
+
 import nest_asyncio
 from pymongo import ASCENDING
-from maid_sweeper.common import patterns
-from maid_sweeper.common.context import Context
-from maid_sweeper.dispatchers.directory import Directory
-from maid_sweeper.dispatchers.exec import Exec
+
+from maid_sweeper import dispatcher, patterns
+from maid_sweeper.context import ThreadMotorContext
 
 P = ParamSpec("P")
 R = TypeVar('R')
 
 
 class MaidSweeper:
-    def __init__(self, mongodb_url='mongodb://localhost:27017', database_name='sweep_maid', max_workers=24, debug_mode=False) -> None:
+    def __init__(self, args: argparse.Namespace) -> None:
         nest_asyncio.apply()
-        self.client = motor.motor_asyncio.AsyncIOMotorClient(
-            mongodb_url)
-        db: motor.motor_asyncio.AsyncIOMotorDatabase = self.client[database_name]
-        loop = asyncio.get_event_loop()
-        self.context = Context(
-            db=db,
-            loop=loop,
-            executor=ThreadPoolExecutor(max_workers=max_workers),
-            debug=debug_mode
-        )
-        self.debug = debug_mode
-
-    def _debug_async(self, func: Callable[P, Awaitable[R]], *args: P.args, **kwargs: P.kwargs) -> Awaitable[R]:
-        """
-        Run an async command with optional asyncio debugging"""
-        if self.debug:
+        if args.debug:
+            import os
             tracemalloc.start()
             logging.basicConfig(level=logging.DEBUG)
+            os.environ["PYTHONASYNCIODEBUG"] = "1"
             if not sys.warnoptions:
-                import os
                 import warnings
                 # Change the filter in this process
                 warnings.simplefilter("default")
-                # Also affect subprocesses]
+                # Also affect subprocesses
                 os.environ["PYTHONWARNINGS"] = "default"
-        result = func(*args, **kwargs)
 
+        self.context = ThreadMotorContext(
+            executor=ThreadPoolExecutor(max_workers=args.max_workers),
+            database_name=args.database_name,
+            debug=args.debug,
+            host=args.mongodb_host,
+            port=args.mongodb_port,
+        )
+
+    def _debug_async(self, func: Callable[P, Awaitable[R]], *args: P.args, **kwargs: P.kwargs) -> Awaitable[R]:
+        """Run an async command with optional asyncio debugging"""
+        result = func(*args, **kwargs)
         # stop tracemalloc after the result is realized
-        if self.debug:
+        if self.context.is_debug():
             async def _inner(x: Awaitable[R]) -> R:
                 res = await x
                 tracemalloc.stop()
                 return res
 
             result = _inner(result)
 
         return result
 
-    async def _sweep(self, keywords: tuple[str], args: tuple[str]):
-        exec_dispatch = Exec()
+    async def _sweep(self, keywords: list[str], args: list[str]):
+        exec_dispatch = dispatcher.Exec()
         # replace synonyms with the actual keywords
         new_keywords = []
         for keyword in keywords:
             if keyword in patterns.SYNONYMS:
                 new_keywords.extend(patterns.SYNONYMS[keyword])
 
         cursor = self.context.db.file_metadata.find(
-            {"tags": {'$in': keywords}})
+            {"tags": {'$in': new_keywords}})
         async for document in cursor:
             path = Path(document['path'])
-            await self.context.dispatch(exec_dispatch, path, args)
+            await exec_dispatch(self.context, path, args)
 
-    async def _tag(self, path: Path):
-        await self.context.dispatch(Directory(), path)
-        self.context.db.file_metadata.create_index([("tags", ASCENDING)])
+    async def _tag(self, paths: list[str]):
+        tasks = []
+        for path in paths:
+            if self.context.is_debug():
+                print(f"Tagging {path}")
+            tasks.append(dispatcher.Directory().dispatch_thread(self.context, Path(path)))
+        await asyncio.gather(*tasks)
+        await self.context.db.file_metadata.create_index([("tags", ASCENDING)])
 
-    def sweep(self, keywords: tuple[str], *exec_args: str):
+    def sweep(self, keywords: list[str], exec_args: list[str]):
         """Sweep the database for files with the given keywords and run the given function on them.
         Args:
             keywords: The comma separated list of keywords to specify the documents.
             exec_args: The command to run on the files. Use placeholders like {} as in find -exec or fd -x.
         """
         print(
             f"Running sweep with keywords {keywords} and command {exec_args}, sure? (y/n)")
         if input() != 'y':
             return
         coro = self._debug_async(self._sweep, keywords, exec_args)
-        self.context.loop.run_until_complete(coro)
+        asyncio.get_event_loop().run_until_complete(coro)
 
-    def tag(self, path: str):
+    def tag(self, paths: list[str]):
         """Tag a file or directory.
 
         Args:
             path: The path to the file or directory to tag.
         """
-        coro = self._debug_async(self._tag, Path(path))
-        self.context.loop.run_until_complete(coro)
+        coro = self._debug_async(self._tag, paths)
+        asyncio.get_event_loop().run_until_complete(coro)
 
 
 def main():
     parser = argparse.ArgumentParser(description='Sweep maid')
 
-    parser.add_argument('--mongodb-url', type=str, default='mongodb://localhost:27017',
+    parser.add_argument('--mongodb-host', type=str, default='mongodb://localhost:27017',
+                        help='The url to the mongodb instance to use.')
+    parser.add_argument('--mongodb-port', type=int, default=27017,
                         help='The url to the mongodb instance to use.')
     parser.add_argument('--database-name', type=str,
                         default='sweep_maid', help='The name of the database to use.')
     parser.add_argument('--max-workers', type=int, default=24,
                         help='The maximum number of workers to use.')
-
     parser.add_argument('--debug', action='store_true',
                         help='Enable debug mode.')
 
     command_parser = parser.add_subparsers(
         dest='command', help='The command to run.')
 
+    tag_parser = command_parser.add_parser(
+        'tag', help='Tag a file or directory.')
+    tag_parser.add_argument(
+        'paths', nargs='+', metavar='path', type=str, help='The root directories to tag.')
+
     sweep_parser = command_parser.add_parser(
         'sweep', help='Sweep the database for files with the given keywords and run the given function on them.')
     sweep_parser.add_argument(
-        'keywords', type=str, help='A comma separated list of keywords to specify the documents. E.g. `sweep game,video` passes `[\'game\',\'video\']` to the maid.')
-    sweep_parser.add_argument('exec_args', type=str, nargs='+',
-                              help='The command to run on the files. Use placeholders like {} as in find -exec or fd -x.')
+        '-t', '--tag', type=str, nargs='*', action='extend', help='A list of tags to specify the documents. E.g. `sweep game,video` passes `[\'game\',\'video\']` to the maid.')
 
-    tag_parser = command_parser.add_parser(
-        'tag', help='Tag a file or directory.')
-    tag_parser.add_argument(
-        'path', type=str, help='The path to the file or directory to tag.')
+    sweep_parser.add_argument('-x', '--exec', type=str, nargs='+', dest='exec_args',
+                              help='The command to run on the files. Use placeholders like {} as in find -exec or fd -x. Defaults to Danshari -- removing all of the files/directories  with the specified tags.')
 
     args = parser.parse_args()
 
-    maid = MaidSweeper(args.mongodb_url, args.database_name,
-                       args.max_workers, args.debug)
+    # set to Danshari mode if no exec args are given
+    if sys.platform == 'win32':
+        danshari = ['del', '/F', '/P', '{}']
+    else:
+        danshari = ['rm', '-r', '{}']
+    if args.command == 'sweep' and args.exec_args is None:
+        print(
+            f"No exec args given, using default {danshari}. Sure? (yes/no)")
+        if input() == 'yes':
+            args.exec_args = danshari
+        else:
+            return
 
+    maid = MaidSweeper(args)
     if args.command == 'sweep':
-        maid.sweep(tuple(args.keywords.split(',')), *args.exec_args)
+        maid.sweep(args.tag, args.exec_args)
     elif args.command == 'tag':
-        maid.tag(args.path)
+        maid = MaidSweeper(args)
+        maid.tag(args.paths)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `maid-sweeper-0.6.9/src/maid_sweeper.egg-info/PKG-INFO` & `maid-sweeper-0.6.96/src/maid_sweeper.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 Metadata-Version: 2.1
 Name: maid-sweeper
-Version: 0.6.9
+Version: 0.6.96
 Summary: A maid that sweeps your files
 Author-email: noirgif <nomaru@outlook.com>
 Project-URL: Homepage, https://github.com/noirgif/maid-sweeper
 Project-URL: Bug Tracker, https://github.com/noirgif/maid-sweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Maid Sweeper for files
 
 Instead of cleaning the unused files, it calls a maid to label them and sweep them under the rug accordingly.
 
 However, the maid can practice Danshari given permission. For example, she can [sell your unused iPad for money](https://comic-days.com/episode/3269754496647364302).
 
+Like Toki, she has two modes:
+
+`tag`: Label the files/directories automatically, based on their types and names.
+
+- code projects and application directories are labeled, and their children are not scanned
+- others are labeled based on the extensions
+
+`sweep`: Carry out actions based on the labels`.
+
 ## Feature
 
-* Asyncio
-* MongoDB
-* Not scanning every single file inside code and program directories, saving time
-    * Avoid accessing metadata
+* AsyncIO, so all operations are in parallel
+* MongoDB for fast indexing
+* Save time by not scanning every single file inside code and program directories and not checking the metadata
 * Kyoufu
 
 ## Installation
 
-1. Have Python 3.11 (as it used some fancy type hints that is incompatible with <3.11).
-2. Install the requirements by running `pip install .`.
+1. Have Python 3.10.
+2. Install by running `pip install maid-sweeper`.
 
 ## Usage
 
 1. Start a MongoDB instance.
-2. Run `python maid.py tag D:\Study`, then you can find tagged entries in Database 'sweep_maid' Collection 'file_metadata'. Then it can be used for further processing.
-3. Run `python maid.py sweep video,game rm -rf {}`, the maid is going to remove all 'video' or 'game' tagged files and directories.
-    * As `fire` is used, it is about the best we can get, without custom deserializer 
-
-## TO-DO
-
-- [ ] Remove type hints
-- [ ] Better readme
-- [ ] Tag based on time
+2. Run `maid-sweeper tag D:\Study`, then you can find tagged entries in the database. Sweeping works on all directories tagged.
+3. Run `maid-sweeper sweep -t video game -x del \q \f {}`, and the maid is going to remove all 'video' or 'game' tagged files and directories.
+    * Any other commands is OK as well
+    * By default the maid will do a sweep -- remove all those files. Kyoufu!
+
+## Ideas
+
+- Multithreading
+- Remove type hints
+- Tags based on time
     * How does it affect other tags? If not why bother?
     * Maybe not tag, but just metadata
     * There will be IO cost
-- [ ] Group similar named files
-- [x] Automatically carry out actions based on the tags, like Dan, Sha and Ri, etc.
-- [ ] Understand human language so they can toss away garbage
-
-- [x] Better command line interface
-    * have to escape {} for fire
-- [ ] Optionally clean up the database after sweeping.
-- [ ] Single line mode: do the tag, sweep, and clean up database entries with a single command.
+- Group similarly named files: 01.jpg, 02.jpg, etc.
+- Understand human language so they can toss away garbage
+- Optionally clean up the database after sweeping.
+- Single line mode: do the tag, sweep, and clean up database entries with a single command.
+- Allow users to specify tags
```

