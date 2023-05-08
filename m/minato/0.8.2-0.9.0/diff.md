# Comparing `tmp/minato-0.8.2.tar.gz` & `tmp/minato-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minato-0.8.2.tar", max compression
+gzip compressed data, was "minato-0.9.0.tar", max compression
```

## Comparing `minato-0.8.2.tar` & `minato-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1064 2022-02-24 10:31:08.804870 minato-0.8.2/LICENSE
--rw-r--r--   0        0        0     1855 2022-02-24 10:31:08.804870 minato-0.8.2/README.md
--rw-r--r--   0        0        0     4236 2022-02-24 10:31:08.804870 minato-0.8.2/minato/__init__.py
--rw-r--r--   0        0        0      443 2022-02-24 10:31:08.808870 minato-0.8.2/minato/__main__.py
--rw-r--r--   0        0        0     9451 2022-02-24 10:31:08.808870 minato-0.8.2/minato/cache.py
--rw-r--r--   0        0        0      748 2022-02-24 10:31:08.808870 minato-0.8.2/minato/commands/__init__.py
--rw-r--r--   0        0        0     2225 2022-02-24 10:31:08.808870 minato-0.8.2/minato/commands/cache.py
--rw-r--r--   0        0        0     3892 2022-02-24 10:31:08.808870 minato-0.8.2/minato/commands/list.py
--rw-r--r--   0        0        0     2335 2022-02-24 10:31:08.808870 minato-0.8.2/minato/commands/remove.py
--rw-r--r--   0        0        0     3724 2022-02-24 10:31:08.808870 minato-0.8.2/minato/commands/subcommand.py
--rw-r--r--   0        0        0     3291 2022-02-24 10:31:08.808870 minato-0.8.2/minato/commands/update.py
--rw-r--r--   0        0        0     1851 2022-02-24 10:31:08.808870 minato-0.8.2/minato/config.py
--rw-r--r--   0        0        0      356 2022-02-24 10:31:08.808870 minato-0.8.2/minato/exceptions.py
--rw-r--r--   0        0        0     1056 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filelock.py
--rw-r--r--   0        0        0      410 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filesystems/__init__.py
--rw-r--r--   0        0        0     5029 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filesystems/filesystem.py
--rw-r--r--   0        0        0     7772 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filesystems/gcs.py
--rw-r--r--   0        0        0     3589 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filesystems/http.py
--rw-r--r--   0        0        0     2574 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filesystems/osfs.py
--rw-r--r--   0        0        0     8354 2022-02-24 10:31:08.808870 minato-0.8.2/minato/filesystems/s3.py
--rw-r--r--   0        0        0    10305 2022-02-24 10:31:08.808870 minato-0.8.2/minato/minato.py
--rw-r--r--   0        0        0        0 2022-02-24 10:31:08.808870 minato-0.8.2/minato/py.typed
--rw-r--r--   0        0        0     3660 2022-02-24 10:31:08.808870 minato-0.8.2/minato/table.py
--rw-r--r--   0        0        0     1204 2022-02-24 10:31:08.808870 minato-0.8.2/minato/url.py
--rw-r--r--   0        0        0     4961 2022-02-24 10:31:08.808870 minato-0.8.2/minato/util.py
--rw-r--r--   0        0        0     1987 2022-02-24 10:31:08.808870 minato-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2960 2022-02-24 10:31:48.589511 minato-0.8.2/setup.py
--rw-r--r--   0        0        0     2741 2022-02-24 10:31:48.589941 minato-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-07-02 04:06:11.293516 minato-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1855 2022-07-02 04:06:11.293516 minato-0.9.0/README.md
+-rw-r--r--   0        0        0     4090 2022-07-02 04:06:11.293516 minato-0.9.0/minato/__init__.py
+-rw-r--r--   0        0        0      443 2022-07-02 04:06:11.293516 minato-0.9.0/minato/__main__.py
+-rw-r--r--   0        0        0     9451 2022-07-02 04:06:11.293516 minato-0.9.0/minato/cache.py
+-rw-r--r--   0        0        0      750 2022-07-02 04:06:11.293516 minato-0.9.0/minato/commands/__init__.py
+-rw-r--r--   0        0        0     2225 2022-07-02 04:06:11.293516 minato-0.9.0/minato/commands/cache.py
+-rw-r--r--   0        0        0     3892 2022-07-02 04:06:11.293516 minato-0.9.0/minato/commands/list.py
+-rw-r--r--   0        0        0     2335 2022-07-02 04:06:11.293516 minato-0.9.0/minato/commands/remove.py
+-rw-r--r--   0        0        0     3649 2022-07-02 04:06:11.293516 minato-0.9.0/minato/commands/subcommand.py
+-rw-r--r--   0        0        0     3291 2022-07-02 04:06:11.293516 minato-0.9.0/minato/commands/update.py
+-rw-r--r--   0        0        0     1780 2022-07-02 04:06:11.293516 minato-0.9.0/minato/config.py
+-rw-r--r--   0        0        0      356 2022-07-02 04:06:11.297516 minato-0.9.0/minato/exceptions.py
+-rw-r--r--   0        0        0     1021 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filelock.py
+-rw-r--r--   0        0        0      410 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filesystems/__init__.py
+-rw-r--r--   0        0        0     4812 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filesystems/filesystem.py
+-rw-r--r--   0        0        0     7684 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filesystems/gcs.py
+-rw-r--r--   0        0        0     3513 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filesystems/http.py
+-rw-r--r--   0        0        0     2492 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filesystems/osfs.py
+-rw-r--r--   0        0        0     8266 2022-07-02 04:06:11.297516 minato-0.9.0/minato/filesystems/s3.py
+-rw-r--r--   0        0        0    10233 2022-07-02 04:06:11.297516 minato-0.9.0/minato/minato.py
+-rw-r--r--   0        0        0        0 2022-07-02 04:06:11.297516 minato-0.9.0/minato/py.typed
+-rw-r--r--   0        0        0     3658 2022-07-02 04:06:11.297516 minato-0.9.0/minato/table.py
+-rw-r--r--   0        0        0     1188 2022-07-02 04:06:11.297516 minato-0.9.0/minato/url.py
+-rw-r--r--   0        0        0     4942 2022-07-02 04:06:11.297516 minato-0.9.0/minato/util.py
+-rw-r--r--   0        0        0     2094 2022-07-02 04:06:11.297516 minato-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2961 2022-07-02 04:06:48.106109 minato-0.9.0/setup.py
+-rw-r--r--   0        0        0     2742 2022-07-02 04:06:48.106653 minato-0.9.0/PKG-INFO
```

### Comparing `minato-0.8.2/LICENSE` & `minato-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/README.md` & `minato-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/minato/__init__.py` & `minato-0.9.0/minato/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 from importlib.metadata import version
 from os import PathLike
 from pathlib import Path
-from typing import IO, Any, BinaryIO, ContextManager, Optional, TextIO, Union, overload
+from typing import IO, Any, BinaryIO, ContextManager, TextIO, overload
 
 from minato.cache import Cache
 from minato.config import Config
 from minato.filesystems import FileSystem
 from minato.minato import Minato
 from minato.util import OpenBinaryMode, OpenTextMode
 
@@ -21,90 +23,90 @@
     "open",
     "upload",
 ]
 
 
 @overload
 def open(
-    url_or_filename: Union[str, PathLike],
+    url_or_filename: str | PathLike,
     mode: OpenTextMode = ...,
     buffering: int = ...,
-    encoding: Optional[str] = ...,
-    errors: Optional[str] = ...,
-    newline: Optional[str] = ...,
+    encoding: str | None = ...,
+    errors: str | None = ...,
+    newline: str | None = ...,
     *,
     extract: bool = ...,
-    auto_update: Optional[bool] = ...,
+    auto_update: bool | None = ...,
     use_cache: bool = ...,
     force_download: bool = ...,
     force_extract: bool = ...,
-    cache_root: Optional[Union[str, PathLike]] = ...,
-    expire_days: Optional[int] = ...,
+    cache_root: str | PathLike | None = ...,
+    expire_days: int | None = ...,
     retry: bool = ...,
 ) -> ContextManager[TextIO]:
     ...
 
 
 @overload
 def open(
-    url_or_filename: Union[str, PathLike],
+    url_or_filename: str | PathLike,
     mode: OpenBinaryMode,
     buffering: int = ...,
-    encoding: Optional[str] = ...,
-    errors: Optional[str] = ...,
-    newline: Optional[str] = ...,
+    encoding: str | None = ...,
+    errors: str | None = ...,
+    newline: str | None = ...,
     *,
     extract: bool = ...,
-    auto_update: Optional[bool] = ...,
+    auto_update: bool | None = ...,
     use_cache: bool = ...,
     force_download: bool = ...,
     force_extract: bool = ...,
-    cache_root: Optional[Union[str, PathLike]] = ...,
-    expire_days: Optional[int] = ...,
+    cache_root: str | PathLike | None = ...,
+    expire_days: int | None = ...,
     retry: bool = ...,
 ) -> ContextManager[BinaryIO]:
     ...
 
 
 @overload
 def open(
-    url_or_filename: Union[str, PathLike],
+    url_or_filename: str | PathLike,
     mode: str,
     buffering: int = ...,
-    encoding: Optional[str] = ...,
-    errors: Optional[str] = ...,
-    newline: Optional[str] = ...,
+    encoding: str | None = ...,
+    errors: str | None = ...,
+    newline: str | None = ...,
     *,
     extract: bool = ...,
-    auto_update: Optional[bool] = ...,
+    auto_update: bool | None = ...,
     use_cache: bool = ...,
     force_download: bool = ...,
     force_extract: bool = ...,
-    cache_root: Optional[Union[str, PathLike]] = ...,
-    expire_days: Optional[int] = ...,
+    cache_root: str | PathLike | None = ...,
+    expire_days: int | None = ...,
     retry: bool = ...,
 ) -> ContextManager[IO[Any]]:
     ...
 
 
 def open(
-    url_or_filename: Union[str, PathLike],
+    url_or_filename: str | PathLike,
     mode: str = "r",
     buffering: int = -1,
-    encoding: Optional[str] = None,
-    errors: Optional[str] = None,
-    newline: Optional[str] = None,
+    encoding: str | None = None,
+    errors: str | None = None,
+    newline: str | None = None,
     *,
     extract: bool = False,
-    auto_update: Optional[bool] = None,
+    auto_update: bool | None = None,
     use_cache: bool = True,
     force_download: bool = False,
     force_extract: bool = False,
-    cache_root: Optional[Union[str, PathLike]] = None,
-    expire_days: Optional[int] = None,
+    cache_root: str | PathLike | None = None,
+    expire_days: int | None = None,
     retry: bool = True,
 ) -> ContextManager[IO[Any]]:
     config = Config.load(
         cache_root=cache_root,
     )
 
     return Minato(config).open(
@@ -121,22 +123,22 @@
         force_extract=force_extract,
         expire_days=expire_days,
         retry=retry,
     )
 
 
 def cached_path(
-    url_or_filename: Union[str, PathLike],
+    url_or_filename: str | PathLike,
     extract: bool = False,
-    auto_update: Optional[bool] = None,
+    auto_update: bool | None = None,
     force_download: bool = False,
     force_extract: bool = False,
     retry: bool = True,
-    cache_root: Optional[Union[str, PathLike]] = None,
-    expire_days: Optional[int] = None,
+    cache_root: str | PathLike | None = None,
+    expire_days: int | None = None,
 ) -> Path:
     config = Config.load(
         cache_root=cache_root,
     )
 
     return Minato(config).cached_path(
         url_or_filename,
@@ -145,23 +147,23 @@
         force_download=force_download,
         force_extract=force_extract,
         expire_days=expire_days,
         retry=retry,
     )
 
 
-def download(url: str, filename: Union[str, PathLike]) -> None:
+def download(url: str, filename: str | PathLike) -> None:
     filename = Path(filename)
     Minato.download(url, filename)
 
 
-def upload(filename: Union[str, PathLike], url: str) -> None:
+def upload(filename: str | PathLike, url: str) -> None:
     filename = Path(filename)
     Minato.upload(filename, url)
 
 
-def delete(url_or_filename: Union[str, PathLike]) -> None:
+def delete(url_or_filename: str | PathLike) -> None:
     Minato.delete(url_or_filename)
 
 
-def exists(url_or_filename: Union[str, PathLike]) -> bool:
+def exists(url_or_filename: str | PathLike) -> bool:
     return Minato.exists(url_or_filename)
```

### Comparing `minato-0.8.2/minato/cache.py` & `minato-0.9.0/minato/cache.py`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/minato/commands/__init__.py` & `minato-0.9.0/minato/commands/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+from __future__ import annotations
+
 import argparse
-from typing import Optional
 
 from minato import __version__
 from minato.commands.cache import CacheCommand  # noqa: F401
 from minato.commands.list import ListCommand  # noqa: F401
 from minato.commands.remove import RemoveCommand  # noqa: F401
 from minato.commands.subcommand import Subcommand
 from minato.commands.update import UpdateCommand  # noqa: F401
 
 
-def create_subcommand(prog: Optional[str] = None) -> Subcommand:
+def create_subcommand(prog: str | None = None) -> Subcommand:
     parser = argparse.ArgumentParser(usage="%(prog)s", prog=prog)
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
     )
     return Subcommand(parser)
 
 
-def main(prog: Optional[str] = None) -> None:
+def main(prog: str | None = None) -> None:
     app = create_subcommand(prog)
     app()
```

### Comparing `minato-0.8.2/minato/commands/cache.py` & `minato-0.9.0/minato/commands/cache.py`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/minato/commands/list.py` & `minato-0.9.0/minato/commands/list.py`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/minato/commands/remove.py` & `minato-0.9.0/minato/commands/remove.py`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/minato/commands/subcommand.py` & `minato-0.9.0/minato/commands/subcommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,37 @@
+from __future__ import annotations
+
 import argparse
 import re
 from collections import defaultdict
-from typing import (
-    Callable,
-    ClassVar,
-    Dict,
-    NamedTuple,
-    Optional,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import Callable, ClassVar, Dict, NamedTuple, Optional, Type, TypeVar, cast
 
 Subclass = TypeVar("Subclass", bound="Subcommand")
 Registry = Dict[Type["Subcommand"], Dict[str, Type["Subcommand"]]]
 
 
 class SubcommandInfo(NamedTuple):
     name: str
-    usage: Optional[str] = None
-    description: Optional[str] = None
-    epilog: Optional[str] = None
+    usage: str | None = None
+    description: str | None = None
+    epilog: str | None = None
 
 
 class Subcommand:
     _registry: ClassVar[Registry] = defaultdict(dict)
     _func_key: ClassVar[str] = "__func"
     _cmd_info: ClassVar[SubcommandInfo]
 
     @classmethod
     def register(
         cls,
-        name: Optional[str] = None,
-        usage: Optional[str] = None,
-        description: Optional[str] = None,
-        epilog: Optional[str] = None,
+        name: str | None = None,
+        usage: str | None = None,
+        description: str | None = None,
+        epilog: str | None = None,
         exist_ok: bool = False,
     ) -> Callable[[Type[Subclass]], Type[Subclass]]:
         registry = Subcommand._registry[cls]
 
         def wrapper(subclass: Type[Subclass]) -> Type[Subclass]:
             info = SubcommandInfo(
                 name=name or cls.camel_to_snake(subclass.__name__),
@@ -69,20 +61,18 @@
     @staticmethod
     def camel_to_snake(text: str) -> str:
         underscored = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", text)
         return re.sub("([a-z0-9])([A-Z])", r"\1_\2", underscored).lower()
 
     def __init__(
         self,
-        parser_or_subparsers: Union[
-            argparse.ArgumentParser,
-            argparse._SubParsersAction,
-            None,
-        ] = None,
-        subcommand_info: Optional[SubcommandInfo] = None,
+        parser_or_subparsers: argparse.ArgumentParser
+        | argparse._SubParsersAction
+        | None = None,
+        subcommand_info: SubcommandInfo | None = None,
     ) -> None:
         cls = type(self)
         info = subcommand_info or self.get_info()
 
         if isinstance(parser_or_subparsers, argparse.ArgumentParser):
             self._parser = parser_or_subparsers
         elif isinstance(parser_or_subparsers, argparse._SubParsersAction):
@@ -100,15 +90,15 @@
 
         registry = Subcommand._registry[cls]
         if registry:
             subparsers = self.parser.add_subparsers()
             for subclass in registry.values():
                 subclass(subparsers)
 
-    def __call__(self, args: Optional[argparse.Namespace] = None) -> None:
+    def __call__(self, args: argparse.Namespace | None = None) -> None:
         if not args:
             args = self.parser.parse_args()
 
         func = cast(
             Optional[Callable[[argparse.Namespace], None]],
             getattr(args, self._func_key, None),
         )
```

### Comparing `minato-0.8.2/minato/commands/update.py` & `minato-0.9.0/minato/commands/update.py`

 * *Files identical despite different names*

### Comparing `minato-0.8.2/minato/config.py` & `minato-0.9.0/minato/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 from configparser import ConfigParser
 from os import PathLike
 from pathlib import Path
-from typing import List, Optional, Union
 
 MINATO_ROOT = Path.home() / ".minato"
 DEFAULT_CACHE_ROOT = MINATO_ROOT / "cache"
 ROOT_CONFIG_PATH = MINATO_ROOT / "config.ini"
 LOCAL_CONFIG_PATH = Path.cwd() / "minato.ini"
 
 
@@ -17,18 +16,18 @@
     cache_root: Path = DEFAULT_CACHE_ROOT
     expire_days: int = -1
     auto_update: bool = True
 
     @classmethod
     def load(
         cls,
-        cache_root: Optional[Union[str, PathLike]] = None,
-        expire_days: Optional[int] = None,
-        auto_update: Optional[bool] = None,
-        files: Optional[List[Union[str, PathLike]]] = None,
+        cache_root: str | PathLike | None = None,
+        expire_days: int | None = None,
+        auto_update: bool | None = None,
+        files: list[str | PathLike] | None = None,
     ) -> Config:
         if files is None:
             files = [ROOT_CONFIG_PATH, LOCAL_CONFIG_PATH]
 
         config = cls()
         config.read_files(files)
         if cache_root is not None:
@@ -36,15 +35,15 @@
         if expire_days is not None:
             config.expire_days = expire_days
         if auto_update is not None:
             config.auto_update = auto_update
 
         return config
 
-    def read_files(self, files: List[Union[str, PathLike]]) -> None:
+    def read_files(self, files: list[str | PathLike]) -> None:
         parser = ConfigParser()
         parser.read([str(path) for path in files])
         self._update_from_configparser(parser)
 
     def _update_from_configparser(self, parser: ConfigParser) -> None:
         if parser.has_section("cache"):
             section = parser["cache"]
```

### Comparing `minato-0.8.2/minato/filesystems/gcs.py` & `minato-0.9.0/minato/filesystems/gcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,17 @@
+from __future__ import annotations
+
 import logging
 import os
 import re
 import tempfile
 from contextlib import contextmanager
 from os import PathLike
 from pathlib import Path
-from typing import (
-    IO,
-    Any,
-    BinaryIO,
-    ContextManager,
-    Iterator,
-    Optional,
-    TextIO,
-    Union,
-    overload,
-)
+from typing import IO, Any, BinaryIO, ContextManager, Iterator, TextIO, overload
 
 from tqdm import tqdm
 
 from minato.filesystems.filesystem import FileSystem
 from minato.util import OpenBinaryMode, OpenTextMode
 
 try:
@@ -31,15 +23,15 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 @FileSystem.register(["gs", "gcs"])
 class GCSFileSystem(FileSystem):
-    def __init__(self, url_or_filename: Union[str, PathLike]) -> None:
+    def __init__(self, url_or_filename: str | PathLike) -> None:
         if gcs is None:
             raise ModuleNotFoundError(
                 "GCSFileSystem is not available. Please make sure that "
                 "google-cloud-storage is successfully installed."
             )
 
         super().__init__(url_or_filename)
@@ -73,15 +65,15 @@
 
     def exists(self) -> bool:
         client = self._client
         bucket = client.bucket(self._bucket_name)
         blobs = list(bucket.list_blobs(prefix=self._key))
         return len(blobs) > 0
 
-    def download(self, path: Union[str, PathLike]) -> None:
+    def download(self, path: str | PathLike) -> None:
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         if not isinstance(path, Path):
             path = Path(path)
 
         client = self._client
@@ -106,15 +98,15 @@
             for blob in blobs:
                 relpath = os.path.relpath(blob.name, self._key)
                 file_path = path / relpath
                 os.makedirs(file_path.parent, exist_ok=True)
                 blob.download_to_filename(str(file_path))
                 progress.update(blob.size or 0)
 
-    def upload(self, path: Union[str, PathLike]) -> None:
+    def upload(self, path: str | PathLike) -> None:
         path = Path(path)
 
         if not path.exists():
             raise FileNotFoundError(path)
 
         prefix = self._key
         if prefix.endswith("/"):
@@ -159,15 +151,15 @@
 
         client = self._client
         bucket = client.bucket(self._bucket_name)
         blobs = list(bucket.list_blobs(prefix=self._key))
         for blob in blobs:
             blob.delete()
 
-    def get_version(self) -> Optional[str]:
+    def get_version(self) -> str | None:
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         client = self._client
         bucket = client.bucket(self._bucket_name)
         blobs = list(bucket.list_blobs(prefix=self._key))
         hashes = [
@@ -178,57 +170,57 @@
         return ".".join(sorted(hashes)) if hashes else None
 
     @overload
     def open_file(
         self,
         mode: OpenTextMode = ...,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[TextIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: OpenBinaryMode,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[BinaryIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: str,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[IO[Any]]:
         ...
 
     def open_file(
         self,
         mode: str = "r",
         buffering: int = -1,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
     ) -> ContextManager[IO[Any]]:
         @contextmanager
         def _open(
             mode: str,
             buffering: int,
-            encoding: Optional[str],
-            errors: Optional[str],
-            newline: Optional[str],
+            encoding: str | None,
+            errors: str | None,
+            newline: str | None,
         ) -> Iterator[IO[Any]]:
             if "x" in mode and self.exists():
                 raise FileExistsError(self._url.raw)
 
             local_file = tempfile.NamedTemporaryFile(delete=False)
             try:
                 if "r" in mode or "a" in mode or "+" in mode:
```

### Comparing `minato-0.8.2/minato/filesystems/http.py` & `minato-0.9.0/minato/filesystems/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,39 @@
+from __future__ import annotations
+
 import os
 import tempfile
 from contextlib import contextmanager
 from os import PathLike
-from typing import (
-    IO,
-    Any,
-    BinaryIO,
-    ContextManager,
-    Iterator,
-    Optional,
-    TextIO,
-    Union,
-    overload,
-)
+from typing import IO, Any, BinaryIO, ContextManager, Iterator, TextIO, overload
 
 import requests
 
 from minato.filesystems.filesystem import FileSystem
 from minato.util import OpenBinaryMode, OpenTextMode, _session_with_backoff, http_get
 
 
 @FileSystem.register(["http", "https"])
 class HttpFileSystem(FileSystem):
     def exists(self) -> bool:
         response = requests.head(self._url.raw, allow_redirects=True)
         status_code = response.status_code
         return status_code == 200
 
-    def download(self, path: Union[str, PathLike]) -> None:
+    def download(self, path: str | PathLike) -> None:
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         with open(path, "w+b") as fp:
             http_get(self._url.raw, fp)
 
     def delete(self) -> None:
         raise OSError("HttpFileSystem cannot delete files or directories.")
 
-    def get_version(self) -> Optional[str]:
+    def get_version(self) -> str | None:
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         with _session_with_backoff() as session:
             response = session.head(self._url.raw, allow_redirects=True)
         if response.status_code != 200:
             raise OSError(
@@ -52,57 +44,57 @@
         return response.headers.get("ETag")
 
     @overload
     def open_file(
         self,
         mode: OpenTextMode = ...,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[TextIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: OpenBinaryMode,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[BinaryIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: str,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[IO[Any]]:
         ...
 
     def open_file(
         self,
         mode: str = "r",
         buffering: int = -1,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
     ) -> ContextManager[IO[Any]]:
         @contextmanager
         def _open(
             mode: str,
             buffering: int,
-            encoding: Optional[str],
-            errors: Optional[str],
-            newline: Optional[str],
+            encoding: str | None,
+            errors: str | None,
+            newline: str | None,
         ) -> Iterator[IO[Any]]:
             if not self.exists():
                 raise FileNotFoundError(self._url.raw)
 
             if "a" in mode or "w" in mode or "+" in mode or "x" in mode:
                 raise ValueError("HttpFileSystem is not writable.")
```

### Comparing `minato-0.8.2/minato/filesystems/osfs.py` & `minato-0.9.0/minato/filesystems/osfs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,87 @@
+from __future__ import annotations
+
 import shutil
 from contextlib import contextmanager
 from os import PathLike
 from pathlib import Path
-from typing import (
-    IO,
-    Any,
-    BinaryIO,
-    ContextManager,
-    Iterator,
-    Optional,
-    TextIO,
-    Union,
-    overload,
-)
+from typing import IO, Any, BinaryIO, ContextManager, Iterator, TextIO, overload
 
 from minato.filesystems.filesystem import FileSystem
 from minato.util import OpenBinaryMode, OpenTextMode, remove_file_or_directory
 
 
 @FileSystem.register(["file", "osfs", ""])
 class OSFileSystem(FileSystem):
-    def __init__(self, url_or_filename: Union[str, PathLike]) -> None:
+    def __init__(self, url_or_filename: str | PathLike) -> None:
         super().__init__(url_or_filename)
         self._path = Path(self._url.path)
 
     def exists(self) -> bool:
         return self._path.exists()
 
-    def download(self, path: Union[str, PathLike]) -> None:
+    def download(self, path: str | PathLike) -> None:
         shutil.copy(self._path, path)
 
     def delete(self) -> None:
         if not self._path.exists():
             raise FileNotFoundError(self._path)
         remove_file_or_directory(self._path)
 
-    def get_version(self) -> Optional[str]:
+    def get_version(self) -> str | None:
         return None
 
     @overload
     def open_file(
         self,
         mode: OpenTextMode = ...,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[TextIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: OpenBinaryMode,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[BinaryIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: str,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[IO[Any]]:
         ...
 
     def open_file(
         self,
         mode: str = "r",
         buffering: int = -1,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
     ) -> ContextManager[IO[Any]]:
         @contextmanager
         def _open(
             mode: str,
             buffering: int,
-            encoding: Optional[str],
-            errors: Optional[str],
-            newline: Optional[str],
+            encoding: str | None,
+            errors: str | None,
+            newline: str | None,
         ) -> Iterator[IO[Any]]:
             with self._path.open(
                 mode=mode,
                 buffering=buffering,
                 encoding=encoding,
                 errors=errors,
                 newline=newline,
```

### Comparing `minato-0.8.2/minato/filesystems/s3.py` & `minato-0.9.0/minato/filesystems/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,18 @@
+from __future__ import annotations
+
 import logging
 import os
 import re
 import tempfile
 import threading
 from contextlib import contextmanager
 from os import PathLike
 from pathlib import Path
-from typing import (
-    IO,
-    Any,
-    BinaryIO,
-    ContextManager,
-    Iterator,
-    Optional,
-    TextIO,
-    Union,
-    overload,
-)
+from typing import IO, Any, BinaryIO, ContextManager, Iterator, TextIO, overload
 
 from tqdm import tqdm
 
 from minato.filesystems.filesystem import FileSystem
 from minato.util import OpenBinaryMode, OpenTextMode
 
 try:
@@ -30,15 +22,15 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 @FileSystem.register(["s3"])
 class S3FileSystem(FileSystem):
-    def __init__(self, url_or_filename: Union[str, PathLike]) -> None:
+    def __init__(self, url_or_filename: str | PathLike) -> None:
         if boto3 is None:
             raise ModuleNotFoundError(
                 "S3FileSystem is not available. Please make sure that "
                 "boto3 is successfully installed."
             )
 
         super().__init__(url_or_filename)
@@ -88,15 +80,15 @@
 
     def exists(self) -> bool:
         resource = self._get_resource()  # type: ignore
         bucket = resource.Bucket(self._bucket_name)
         objects = list(bucket.objects.filter(Prefix=self._key))
         return len(objects) > 0
 
-    def download(self, path: Union[str, PathLike]) -> None:
+    def download(self, path: str | PathLike) -> None:
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         path = Path(path)
 
         resource = self._get_resource()  # type: ignore
         bucket = resource.Bucket(self._bucket_name)
@@ -122,15 +114,15 @@
         ) as progress:
             for obj in objects:
                 relprefix = os.path.relpath(obj.key, self._key)
                 file_path = path / relprefix
                 os.makedirs(file_path.parent, exist_ok=True)
                 bucket.download_file(obj.key, str(file_path), Callback=progress.update)
 
-    def upload(self, path: Union[str, PathLike]) -> None:
+    def upload(self, path: str | PathLike) -> None:
         path = Path(str(path)).absolute()
 
         prefix = self._key
         if prefix.endswith("/"):
             prefix = os.path.join(prefix, path.name)
 
         filenames = (
@@ -167,72 +159,72 @@
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         resource = self._get_resource()  # type: ignore
         bucket = resource.Bucket(self._bucket_name)
         bucket.objects.filter(Prefix=self._key).delete()
 
-    def get_version(self) -> Optional[str]:
+    def get_version(self) -> str | None:
         if not self.exists():
             raise FileNotFoundError(self._url.raw)
 
         resource = self._get_resource()  # type: ignore
         bucket = resource.Bucket(self._bucket_name)
         objects = list(bucket.objects.filter(Prefix=self._key))
         etags = [str(obj.e_tag).strip('"') for obj in objects if obj.e_tag]
         return ".".join(sorted(etags)) if etags else None
 
     @overload
     def open_file(
         self,
         mode: OpenTextMode = ...,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[TextIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: OpenBinaryMode,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[BinaryIO]:
         ...
 
     @overload
     def open_file(
         self,
         mode: str,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> ContextManager[IO[Any]]:
         ...
 
     def open_file(
         self,
         mode: str = "r",
         buffering: int = -1,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
     ) -> ContextManager[IO[Any]]:
         @contextmanager
         def _open(
             mode: str,
             buffering: int,
-            encoding: Optional[str],
-            errors: Optional[str],
-            newline: Optional[str],
+            encoding: str | None,
+            errors: str | None,
+            newline: str | None,
         ) -> Iterator[IO[Any]]:
             if "x" in mode and self.exists():
                 raise FileExistsError(self._url.raw)
 
             local_file = tempfile.NamedTemporaryFile(delete=False)
 
             try:
```

### Comparing `minato-0.8.2/minato/minato.py` & `minato-0.9.0/minato/minato.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import logging
 from os import PathLike
 from pathlib import Path
-from typing import IO, Any, BinaryIO, ContextManager, Optional, TextIO, Union, overload
+from typing import IO, Any, BinaryIO, ContextManager, TextIO, overload
 
 from minato.cache import Cache, CacheStatus
 from minato.config import Config
 from minato.exceptions import CacheNotFoundError, InvalidCacheStatus
 from minato.filesystems import delete, download, exists, get_version, open_file, upload
 from minato.util import (
     OpenBinaryMode,
@@ -17,98 +19,98 @@
     remove_file_or_directory,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Minato:
-    def __init__(self, config: Optional[Config] = None) -> None:
+    def __init__(self, config: Config | None = None) -> None:
         self._config = config or Config.load()
         self._cache = Cache(
             root=self._config.cache_root,
             default_expire_days=self._config.expire_days,
             default_auto_update=self._config.auto_update,
         )
 
     @property
     def cache(self) -> Cache:
         return self._cache
 
     @overload
     def open(
         self,
-        url_or_filename: Union[str, PathLike],
+        url_or_filename: str | PathLike,
         mode: OpenTextMode = ...,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
         *,
         extract: bool = ...,
-        auto_update: Optional[bool] = ...,
-        expire_days: Optional[int] = ...,
+        auto_update: bool | None = ...,
+        expire_days: int | None = ...,
         use_cache: bool = ...,
         force_download: bool = ...,
         force_extract: bool = ...,
         retry: bool = ...,
     ) -> ContextManager[TextIO]:
         ...
 
     @overload
     def open(
         self,
-        url_or_filename: Union[str, PathLike],
+        url_or_filename: str | PathLike,
         mode: OpenBinaryMode,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
         *,
         extract: bool = ...,
-        auto_update: Optional[bool] = ...,
-        expire_days: Optional[int] = ...,
+        auto_update: bool | None = ...,
+        expire_days: int | None = ...,
         use_cache: bool = ...,
         force_download: bool = ...,
         force_extract: bool = ...,
         retry: bool = ...,
     ) -> ContextManager[BinaryIO]:
         ...
 
     @overload
     def open(
         self,
-        url_or_filename: Union[str, PathLike],
+        url_or_filename: str | PathLike,
         mode: str,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
         *,
         extract: bool = ...,
-        auto_update: Optional[bool] = ...,
-        expire_days: Optional[int] = ...,
+        auto_update: bool | None = ...,
+        expire_days: int | None = ...,
         use_cache: bool = ...,
         force_download: bool = ...,
         force_extract: bool = ...,
         retry: bool = ...,
     ) -> ContextManager[IO[Any]]:
         ...
 
     def open(
         self,
-        url_or_filename: Union[str, PathLike],
+        url_or_filename: str | PathLike,
         mode: str = "r",
         buffering: int = -1,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
         *,
         extract: bool = False,
-        auto_update: Optional[bool] = None,
-        expire_days: Optional[int] = None,
+        auto_update: bool | None = None,
+        expire_days: int | None = None,
         use_cache: bool = True,
         force_download: bool = False,
         force_extract: bool = False,
         retry: bool = True,
     ) -> ContextManager[IO[Any]]:
         if not ("a" in mode or "w" in mode or "x" in mode or "+" in mode) and use_cache:
             logger.debug("Open cached file of %s.", url_or_filename)
@@ -118,22 +120,22 @@
                 auto_update=auto_update,
                 expire_days=expire_days,
                 force_download=force_download,
                 force_extract=force_extract,
                 retry=retry,
             )
 
-        return open_file(url_or_filename, mode)
+        return open_file(url_or_filename, mode, buffering, encoding, errors, newline)
 
     def cached_path(
         self,
-        url_or_filename: Union[str, PathLike],
+        url_or_filename: str | PathLike,
         extract: bool = False,
-        auto_update: Optional[bool] = None,
-        expire_days: Optional[int] = None,
+        auto_update: bool | None = None,
+        expire_days: int | None = None,
         force_download: bool = False,
         force_extract: bool = False,
         retry: bool = True,
     ) -> Path:
         url_or_filename = str(url_or_filename)
 
         if "!" in url_or_filename:
@@ -263,31 +265,31 @@
             raise FileNotFoundError(cached_file.local_path)
         if cached_file.status != CacheStatus.COMPLETED:
             raise InvalidCacheStatus(
                 f"Cached path status is not completed: status={cached_file.status}"
             )
         return cached_file.local_path
 
-    def available_update(self, url_or_filename: Union[str, PathLike]) -> bool:
+    def available_update(self, url_or_filename: str | PathLike) -> bool:
         if is_local(url_or_filename):
             return False
 
         url = str(url_or_filename)
         cached_file = self._cache.by_url(url)
         current_version = get_version(url)
         return cached_file.version != current_version
 
     @staticmethod
-    def download(url: str, filename: Union[str, PathLike]) -> None:
+    def download(url: str, filename: str | PathLike) -> None:
         download(url, filename)
 
     @staticmethod
-    def upload(filename: Union[str, PathLike], url: str) -> None:
+    def upload(filename: str | PathLike, url: str) -> None:
         upload(filename, url)
 
     @staticmethod
-    def delete(url_or_filename: Union[str, PathLike]) -> None:
+    def delete(url_or_filename: str | PathLike) -> None:
         delete(url_or_filename)
 
     @staticmethod
-    def exists(url_or_filename: Union[str, PathLike]) -> bool:
+    def exists(url_or_filename: str | PathLike) -> bool:
         return exists(url_or_filename)
```

### Comparing `minato-0.8.2/minato/table.py` & `minato-0.9.0/minato/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 import os
 import sys
-from typing import Any, Dict, List, Optional, TextIO, Union
+from typing import Any, TextIO
 
 
 class Table:
     MIN_COLUMN_WIDTH = 2
 
-    def __init__(self, columns: List[str], shrink: bool = True) -> None:
+    def __init__(self, columns: list[str], shrink: bool = True) -> None:
         self._columns = columns
-        self._items: List[Dict[str, Any]] = []
+        self._items: list[dict[str, Any]] = []
         self._shrink = shrink
 
-    def __getitem__(self, columns: List[str]) -> "Table":
+    def __getitem__(self, columns: list[str]) -> "Table":
         table = Table(columns=columns)
         for item in self._items:
             table.add(item)
         return table
 
     @staticmethod
     def _get_padded_column_value(value: str, width: int) -> str:
@@ -26,16 +28,16 @@
 
     @staticmethod
     def _get_column_value_str(value: Any) -> str:
         if isinstance(value, str):
             return repr(value)[1:-1]
         return repr(value)
 
-    def _get_column_widths(self) -> Dict[str, int]:
-        column_widths: Dict[str, int] = {}
+    def _get_column_widths(self) -> dict[str, int]:
+        column_widths: dict[str, int] = {}
         for col in self.columns:
             column_values = [x[col] for x in self._items]
             column_value_strings = [
                 self._get_column_value_str(x) for x in column_values
             ]
 
             column_width = max(len(x) for x in column_value_strings + [col])
@@ -58,38 +60,38 @@
             )
             column_widths[column] = max(width - 1, Table.MIN_COLUMN_WIDTH)
             previous_width = total_column_width
             total_column_width = num_columns + sum(column_widths.values()) - 1
         return column_widths
 
     @property
-    def columns(self) -> List[str]:
+    def columns(self) -> list[str]:
         return self._columns
 
-    def add(self, item: Dict[str, Any]) -> None:
+    def add(self, item: dict[str, Any]) -> None:
         self._items.append({col: item[col] for col in self.columns})
 
     def sort(self, column: str, desc: bool = False) -> None:
-        def _key(item: Dict[str, Any]) -> Any:
+        def _key(item: dict[str, Any]) -> Any:
             return item[column]
 
         self._items = sorted(self._items, key=_key, reverse=desc)
 
-    def filter(self, query: Union[str, Dict[str, str]]) -> "Table":
+    def filter(self, query: str | dict[str, str]) -> "Table":
         if isinstance(query, str):
             query = {col: query for col in self.columns}
         table = Table(columns=self.columns)
         for item in self._items:
             for c, q in query.items():
                 if q in item[c]:
                     table.add(item)
                     break
         return table
 
-    def show(self, output: Optional[TextIO] = None) -> None:
+    def show(self, output: TextIO | None = None) -> None:
         if output is None:
             output = sys.stdout
 
         column_widths = self._get_column_widths()
 
         output.write(
             " ".join(
```

### Comparing `minato-0.8.2/minato/url.py` & `minato-0.9.0/minato/url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List, Optional
+from __future__ import annotations
+
 from urllib.parse import parse_qs, urlparse
 
 
 class URL:
     def __init__(self, url: str) -> None:
         self._raw = url
 
@@ -21,30 +22,30 @@
         return self._parse_result.path
 
     @property
     def scheme(self) -> str:
         return self._parse_result.scheme
 
     @property
-    def username(self) -> Optional[str]:
+    def username(self) -> str | None:
         return self._parse_result.username
 
     @property
-    def password(self) -> Optional[str]:
+    def password(self) -> str | None:
         return self._parse_result.password
 
     @property
-    def hostname(self) -> Optional[str]:
+    def hostname(self) -> str | None:
         return self._parse_result.hostname
 
     @property
-    def netloc(self) -> Optional[str]:
+    def netloc(self) -> str | None:
         return self._parse_result.netloc
 
-    def get_queries(self, key: str) -> Optional[List[str]]:
+    def get_queries(self, key: str) -> list[str] | None:
         return self._queries.get(key)
 
-    def get_query(self, key: str) -> Optional[str]:
+    def get_query(self, key: str) -> str | None:
         values = self.get_queries(key)
         if not values:
             return None
         return values[0]
```

### Comparing `minato-0.8.2/minato/util.py` & `minato-0.9.0/minato/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import logging
 import os
 import shutil
 import tarfile
 import tempfile
 from os import PathLike
 from pathlib import Path
-from typing import IO, Any, Literal, Tuple, Union
+from typing import IO, Any, Literal, Union
 from urllib.parse import urlparse
 from zipfile import ZipFile, is_zipfile
 
 import requests
 from requests.adapters import HTTPAdapter
 from tqdm import tqdm
 from urllib3.util.retry import Retry
@@ -122,62 +124,62 @@
     "Ubr",
 ]
 OpenBinaryMode = Union[
     OpenBinaryModeUpdating, OpenBinaryModeReading, OpenBinaryModeWriting
 ]
 
 
-def remove_file_or_directory(path: Union[str, PathLike]) -> None:
+def remove_file_or_directory(path: str | PathLike) -> None:
     try:
         path = Path(path)
         if path.is_dir():
             shutil.rmtree(path)
         else:
             os.remove(path)
     except FileNotFoundError:
         pass
 
 
-def is_archive_file(filename: Union[str, PathLike]) -> bool:
+def is_archive_file(filename: str | PathLike) -> bool:
     if not Path(filename).is_file():
         return False
     return is_zipfile(filename) or tarfile.is_tarfile(filename)
 
 
 def extract_archive_file(
-    source_path: Union[str, PathLike],
-    target_path: Union[str, PathLike],
+    source_path: str | PathLike,
+    target_path: str | PathLike,
 ) -> None:
     with tempfile.TemporaryDirectory() as temp_dir:
         if is_zipfile(source_path):
             with ZipFile(source_path, "r") as zip_file:
                 zip_file.extractall(temp_dir)
         elif tarfile.is_tarfile(source_path):
             with tarfile.open(source_path) as tar_file:
                 tar_file.extractall(temp_dir)
         os.replace(temp_dir, target_path)
 
 
-def extract_path(filename: Union[str, PathLike]) -> str:
+def extract_path(filename: str | PathLike) -> str:
     parsed = urlparse(str(filename))
     return parsed.path
 
 
-def is_local(url_or_filename: Union[str, PathLike]) -> bool:
+def is_local(url_or_filename: str | PathLike) -> bool:
     if isinstance(url_or_filename, Path):
         return True
 
     parsed = urlparse(str(url_or_filename))
     if parsed.scheme in ("", "file", "osfs"):
         return True
 
     return False
 
 
-def get_parent_path_and_filename(path: Union[str, PathLike]) -> Tuple[str, str]:
+def get_parent_path_and_filename(path: str | PathLike) -> tuple[str, str]:
     if isinstance(path, Path):
         parent = str(path.parent)
         name = str(path.name)
         return parent, name
 
     path = str(path)
     parsed_url = urlparse(path)
@@ -194,15 +196,15 @@
 
     if scheme and netloc:
         parent = f"{scheme}://{netloc}/{parent}"
 
     return parent, name
 
 
-def sizeof_fmt(num: Union[int, float], suffix: str = "B") -> str:
+def sizeof_fmt(num: int | float, suffix: str = "B") -> str:
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return "%3.1f %s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f %s%s" % (num, "Yi", suffix)
```

### Comparing `minato-0.8.2/pyproject.toml` & `minato-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "minato"
-version = "0.8.2"
+version = "0.9.0"
 description = "Cached file system for online resources"
 authors = ["Yasuhiro Yamaguchi <altescy@fastmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/altescy/minato"
 keywords=["python", "cache", "s3", "google-cloud-storage"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.11"
 requests = "^2.25.1"
 tqdm = "^4.60.0"
 boto3 = { version = "^1.17.97", optional = true }
 google-cloud-storage = { version = "^1.39.0", optional = true }
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^7.1.2"
 python-language-server = "^0.36.2"
 pysen = "^0.10.1"
-black = "^22.1.0"
+black = "^22.3.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
-mypy = "^0.931"
+mypy = "^0.950"
 types-requests = "^2.27.8"
 moto = {version = "^2.0.9", extras = ["s3"]}
 boto3-stubs = {version = "^1.19.12", extras = ["s3"]}
 
 [tool.poetry.extras]
 s3=["boto3"]
 gcs=["google-cloud-storage"]
@@ -53,18 +53,20 @@
   paths = ["."]
 
 [tool.pysen.lint.source]
   includes = ["."]
   excludes = [".venv/"]
 
 [tool.black] # automatically generated by pysen
+# pysen ignores and overwrites any modifications
 line-length = 88
 target-version = ["py38"]
 
 [tool.isort] # automatically generated by pysen
+# pysen ignores and overwrites any modifications
 default_section = "THIRDPARTY"
 ensure_newline_before_comments = true
 force_grid_wrap = 0
 force_single_line = false
 include_trailing_comma = true
 line_length = 88
 multi_line_output = 3
```

### Comparing `minato-0.8.2/setup.py` & `minato-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
  's3': ['boto3>=1.17.97,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['minato = minato.__main__:run']}
 
 setup_kwargs = {
     'name': 'minato',
-    'version': '0.8.2',
+    'version': '0.9.0',
     'description': 'Cached file system for online resources',
     'long_description': 'Minato\n======\n\n[![Actions Status](https://github.com/altescy/minato/workflows/CI/badge.svg)](https://github.com/altescy/minato/actions/workflows/ci.yml)\n[![Python version](https://img.shields.io/pypi/pyversions/minato)](https://github.com/altescy/minato)\n[![License](https://img.shields.io/github/license/altescy/minato)](https://github.com/altescy/minato/blob/master/LICENSE)\n[![pypi version](https://img.shields.io/pypi/v/minato)](https://pypi.org/project/minato/)\n\nCache & file system for online resources in Python\n\n\n## Features\n\nMinato enables you to:\n- Download & cache online recsources\n  - minato supports the following protocols: HTTP(S) / AWS S3 / Google Cloud Storage\n  - You can manage cached files via command line interface\n- Automatically update cached files based on ETag\n  - minato downloads new versions if available when you access cached files\n- Open online files super easily\n  - By using `minato.open`, you can read/write online resources like the built-in `open` method\n\n## Installation\n\n```\npip install minato[all]\n```\n\n## Usage\n\n### Python\n\n```python\nimport minato\n\n# Read / write files on online storage\nwith minato.open("s3://your_bucket/path/to/file", "w") as f:\n    f.write("Create a new file on AWS S3!")\n\n# Cache & manage online resources in local storage\nlocal_filename = minato.cached_path("http://example.com/path/to/archive.zip!inner/path/to/file")\n```\n\n### CLI\n\n```\n❯ poetry run minato --help\nusage: minato\n\npositional arguments:\n  {cache,list,remove,update}\n    cache               cache remote file and return cached local file path\n    list                show list of cached files\n    remove              remove cached files\n    update              update cached files\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --version             show program\'s version number and exit\n```\n',
     'author': 'Yasuhiro Yamaguchi',
     'author_email': 'altescy@fastmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/altescy/minato',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `minato-0.8.2/PKG-INFO` & `minato-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: minato
-Version: 0.8.2
+Version: 0.9.0
 Summary: Cached file system for online resources
 Home-page: https://github.com/altescy/minato
 License: MIT
 Keywords: python,cache,s3,google-cloud-storage
 Author: Yasuhiro Yamaguchi
 Author-email: altescy@fastmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: all
 Provides-Extra: gcs
```

