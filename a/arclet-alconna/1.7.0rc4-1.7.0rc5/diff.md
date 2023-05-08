# Comparing `tmp/arclet-alconna-1.7.0rc4.tar.gz` & `tmp/arclet-alconna-1.7.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc4.tar", last modified: Fri Apr 28 08:00:54 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.0rc5.tar", last modified: Mon May  8 11:30:12 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc4.tar` & `arclet-alconna-1.7.0rc5.tar`

### file list

```diff
@@ -1,31 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc4/LICENSE
--rw-r--r--   0        0        0     2731 2023-04-28 07:58:40.959628 arclet-alconna-1.7.0rc4/pyproject.toml
--rw-r--r--   0        0        0     5861 2023-04-27 14:49:51.354435 arclet-alconna-1.7.0rc4/README-EN.md
--rw-r--r--   0        0        0      926 2023-04-28 07:41:36.946430 arclet-alconna-1.7.0rc4/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0     3419 2023-04-09 14:04:25.832070 arclet-alconna-1.7.0rc4/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    13765 2023-04-24 13:50:47.402011 arclet-alconna-1.7.0rc4/src/arclet/alconna/analyser.py
--rw-r--r--   0        0        0    11183 2023-04-27 14:14:53.516769 arclet-alconna-1.7.0rc4/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     7169 2023-04-28 06:02:12.116241 arclet-alconna-1.7.0rc4/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    12616 2023-04-27 14:25:54.921925 arclet-alconna-1.7.0rc4/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0     6745 2023-04-24 14:02:23.257763 arclet-alconna-1.7.0rc4/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     4384 2023-04-17 05:41:18.628904 arclet-alconna-1.7.0rc4/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     3486 2023-04-27 14:49:51.385435 arclet-alconna-1.7.0rc4/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     3455 2023-04-26 09:58:35.085641 arclet-alconna-1.7.0rc4/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14486 2023-04-27 14:34:40.178996 arclet-alconna-1.7.0rc4/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2498 2023-03-31 19:18:40.743939 arclet-alconna-1.7.0rc4/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-03-31 14:01:42.790537 arclet-alconna-1.7.0rc4/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    10341 2023-04-26 10:45:37.334634 arclet-alconna-1.7.0rc4/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0    19181 2023-04-28 07:33:07.099623 arclet-alconna-1.7.0rc4/src/arclet/alconna/handlers.py
--rw-r--r--   0        0        0     6382 2023-04-28 07:17:08.737239 arclet-alconna-1.7.0rc4/src/arclet/alconna/header.py
--rw-r--r--   0        0        0       99 2023-04-24 13:02:08.850723 arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3273 2023-04-26 10:32:37.466006 arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3300 2023-04-26 10:28:23.789467 arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    14530 2023-04-24 14:13:48.282478 arclet-alconna-1.7.0rc4/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1505 2023-04-13 03:35:02.200010 arclet-alconna-1.7.0rc4/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1144 2023-04-12 12:33:00.784350 arclet-alconna-1.7.0rc4/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc4/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-04-08 09:18:05.731268 arclet-alconna-1.7.0rc4/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc4/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     2385 2023-04-26 10:52:37.893474 arclet-alconna-1.7.0rc4/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0      915 2023-04-26 10:51:56.274030 arclet-alconna-1.7.0rc4/src/arclet/alconna/util.py
--rw-r--r--   0        0        0     6555 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc5/LICENSE
+-rw-r--r--   0        0        0     2813 2023-05-07 16:32:54.439874 arclet-alconna-1.7.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-08 08:04:29.409891 arclet-alconna-1.7.0rc5/README-EN.md
+-rw-r--r--   0        0        0     1087 2023-05-08 11:29:49.426377 arclet-alconna-1.7.0rc5/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:29:22.798529 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    18070 2023-05-08 06:36:38.138006 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8361 2023-05-07 16:29:22.799529 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    22923 2023-05-08 08:02:25.512945 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     7811 2023-05-08 06:38:21.959747 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-07 16:29:22.801529 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1785 2023-05-08 05:11:19.754526 arclet-alconna-1.7.0rc5/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14478 2023-05-08 06:44:47.137906 arclet-alconna-1.7.0rc5/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1243 2023-05-07 16:29:22.804526 arclet-alconna-1.7.0rc5/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15913 2023-05-07 16:32:41.201286 arclet-alconna-1.7.0rc5/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    12902 2023-05-08 05:22:02.753182 arclet-alconna-1.7.0rc5/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-08 06:44:58.844442 arclet-alconna-1.7.0rc5/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4868 2023-05-08 06:45:27.372580 arclet-alconna-1.7.0rc5/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4470 2023-05-07 16:32:44.799782 arclet-alconna-1.7.0rc5/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14715 2023-05-07 16:32:45.542456 arclet-alconna-1.7.0rc5/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2615 2023-05-07 16:32:47.490076 arclet-alconna-1.7.0rc5/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1070 2023-05-07 16:32:49.003053 arclet-alconna-1.7.0rc5/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11256 2023-05-07 16:32:49.488876 arclet-alconna-1.7.0rc5/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-07 16:29:22.812601 arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3565 2023-05-07 16:29:22.813522 arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3602 2023-05-07 16:29:22.813850 arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    16838 2023-05-08 06:47:44.520450 arclet-alconna-1.7.0rc5/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1430 2023-05-07 16:32:50.831111 arclet-alconna-1.7.0rc5/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-07 16:32:51.478127 arclet-alconna-1.7.0rc5/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-07 16:32:52.687122 arclet-alconna-1.7.0rc5/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:29:22.816522 arclet-alconna-1.7.0rc5/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5813 2023-05-07 16:32:58.355410 arclet-alconna-1.7.0rc5/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3584 2023-05-07 16:32:58.778521 arclet-alconna-1.7.0rc5/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3254 2023-05-08 06:48:40.755418 arclet-alconna-1.7.0rc5/tests/analyser_test.py
+-rw-r--r--   0        0        0     7223 2023-05-07 16:29:22.820523 arclet-alconna-1.7.0rc5/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-07 16:32:42.508980 arclet-alconna-1.7.0rc5/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-08 06:49:11.411375 arclet-alconna-1.7.0rc5/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-07 16:29:22.822522 arclet-alconna-1.7.0rc5/tests/config_test.py
+-rw-r--r--   0        0        0    23213 2023-05-08 06:49:45.049528 arclet-alconna-1.7.0rc5/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-07 16:29:22.823526 arclet-alconna-1.7.0rc5/tests/util_test.py
+-rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc5/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc4/LICENSE` & `arclet-alconna-1.7.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc4/pyproject.toml` & `arclet-alconna-1.7.0rc5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "nepattern<0.6.0, >=0.5.5",
+    "nepattern<0.6.0, >=0.5.6",
     "tarina>=0.3.3",
 ]
 dynamic = []
 requires-python = ">=3.8"
 readme = "README-EN.md"
 keywords = [
     "command",
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc4"
+version = "1.7.0rc5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
@@ -65,15 +65,15 @@
     "fix-future-annotations>=0.4.0",
     "viztracer>=0.15.6",
 ]
 
 [tool.pdm.scripts]
 test = "python entry_test.py"
 benchmark = "python benchmark.py"
-deps = "pydeps ./src/arclet/alconna"
+deps = "pydeps -o alconna.svg ./src/arclet/alconna --max-bacon=4 --cluster --keep-target-cluster --rmprefix alconna. "
 
 [tool.pdm.version]
 source = "file"
 path = "src/arclet/alconna/__init__.py"
 
 [tool.pylint.BASIC]
 class-const-naming-style = "any"
```

### Comparing `arclet-alconna-1.7.0rc4/README-EN.md` & `arclet-alconna-1.7.0rc5/README-EN.md`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
 * High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
+* Intuitive way to create command components
 * Powerful Automatic Type Parse and Conversion
 * Customizable Help Text Formatter and Control of Command Analyser
 * i18n Support
 * Cache of input command for quick response of repeated command
 * Easy-to-use Construct and Usage of Command Shortcut
 * Can bind callback function to execute after command parsing
 * Can create command completion session to implement multi-round continuous completion prompt
@@ -73,65 +74,99 @@
 
 Example of Callback Executor:
 
 ```python
 # callback.py
 from arclet.alconna import Alconna, Args
 
-alc = Alconna("test", Args["foo", int]["bar", str])
+alc = Alconna("callback", Args["foo", int]["bar", str])
 
 @alc.bind()
 def callback(foo: int, bar: str):
     print(f"foo: {foo}")
     print(f"bar: {bar}")
     print(bar * foo)
     
 if __name__ == "__main__":
     alc()
 ```
 
 ```shell
-$ python callback.py test 3 hello
+$ python callback.py 3 hello
 foo: 3
 bar: hello
 hellohellohello
 ```
 
 
 Example of Type Conversion:
 
 ```python
 from arclet.alconna import Alconna, Args
 from pathlib import Path
 
-read = Alconna(
-    "read", Args["data", bytes], 
-    action=lambda data: print(type(data))
-)
+read = Alconna("read", Args["data", bytes])
+
+@read.bind()
+def cb(data: bytes):
+    print(type(data))
 
 read.parse(["read", b'hello'])
 read.parse("read test_fire.py")
 read.parse(["read", Path("test_fire.py")])
 
 '''
 <class 'bytes'>
 <class 'bytes'>
 <class 'bytes'>
 '''
 ```
 
+Example of Component creation:
+```python
+# component.py
+from arclet.alconna import Alconna, Args, Option, Subcommand, store_true, count, append
+
+alc = Alconna(
+    "component",
+    Args["path", str],
+    Option("--verbose|-v", action=count),
+    Option("-f", Args["flag", str], compact=True, action=append),
+    Subcommand("sub", Option("bar", action=store_true, default=False))
+)
+
+if __name__ == '__main__':
+    res = alc()
+    print(res.query("path"))
+    print(res.query("verbose.value"))
+    print(res.query("f.flag"))
+    print(res.query("sub"))
+```
+
+```shell
+$ python component.py /home/arclet -vvvv -f1 -f2 -f3 sub bar
+/home/arclet
+4
+['1', '2', '3']
+(value=Ellipsis args={} options={'bar': (value=True args={})} subcommands={})
+```
+
 Example of Command Shortcut:
 ```python
 # shortcut.py
 from arclet.alconna import Alconna, Args
 
-alc = Alconna("eval", Args["content", str], action=lambda x: eval(x, {}, {}))
+alc = Alconna("eval", Args["content", str])
 alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
 
-if __name__ == "__main__":
+@alc.bind()
+def cb(content: str):
+    eval(content, {}, {})
+
+if __name__ == '__main__':
     alc()
 ```
 
 ```shell
 $ python shortcut.py eval print(\"hello world\")
 hello world
 $ python shortcut.py echo hello world!
@@ -139,28 +174,28 @@
 ```
 
 Example of Command Completion:
 ```python
 # completion.py
 from arclet.alconna import Alconna, Args, Option
 
-alc = Alconna("test", Args["bar", int]) + Option("foo") + Option("fool")
+alc = Alconna("complete", Args["bar", int]) + Option("foo") + Option("fool")
 
 if __name__ == "__main__":
-    alc.completion()
+    alc()
 ```
 
 ```shell
-$ python completion.py test ?
-next input maybe:
-> foo
-> int
-> -h
-> --help
-> fool
+$ python completion.py ?
+suggest input follows:
+* bar: int
+* --help
+* -h
+* foo
+* fool
 ```
 
 Example of `typing` Support:
 ```python
 from typing import Annotated  # or typing_extensions.Annotated
 from arclet.alconna import Alconna, Args
 
@@ -188,19 +223,14 @@
 ```
 
 ```shell
 $ python fuzzy.py /test_fuzzy foo bar
 /test_fuzy not matched. Are you mean "!test_fuzzy"?
 ```
 
-
-
-
-
-
 ## License
 
 Alconna is licensed under the [MIT License](LICENSE).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
 
 ## Acknowledgement
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/analyser.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/arparma.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,340 +1,418 @@
 from __future__ import annotations
 
-import re
-import traceback
-from re import Match
-from typing import TYPE_CHECKING, Any, Generic, Callable
+from abc import ABCMeta, abstractmethod
+from contextlib import suppress
 from dataclasses import dataclass, field
-from typing_extensions import Self, TypeAlias
-from tarina import lang
+from functools import lru_cache
+from types import MappingProxyType
+from typing import Any, Callable, Generic, Mapping, TypeVar, overload
+from tarina import get_signature, generic_isinstance, Empty, lang
+from typing_extensions import Self
 
-from .manager import command_manager, ShortcutArgs
-from .exceptions import (
-    ParamsUnmatched,
-    ArgumentMissing,
-    FuzzyMatchSuccess,
-    PauseTriggered,
-    SpecialOptionTriggered
-)
-from .args import Args
-from .header import Header
-from .base import Option, Subcommand
-from .completion import comp_ctx
-from .model import Sentence, HeadResult, OptionResult, SubcommandResult
-from .arparma import Arparma
+from .exceptions import BehaveCancelled, OutBoundsBehave
+from .model import HeadResult, OptionResult, SubcommandResult
 from .typing import TDC
-from .config import Namespace
-from .output import output_manager
-from .handlers import (
-    analyse_args, analyse_param, analyse_header, handle_help, handle_shortcut, handle_completion, prompt
-)
-
-if TYPE_CHECKING:
-    from .argv import Argv
-    from .core import Alconna
-
-_SPECIAL = {
-    "help": handle_help,
-    "shortcut": handle_shortcut,
-    "completion": handle_completion
-}
-
-
-def _compile_opts(option: Option, data: dict[str, Sentence | Option | list[Option] | SubAnalyser]):
-    for alias in option.aliases:
-        if li := data.get(alias):
-            if isinstance(li, list):
-                li.append(option)
-            elif isinstance(li, Sentence):
-                data[alias] = option
-                continue
-            else:
-                data[alias] = [li, option]
-            data[alias].sort(key=lambda x: x.priority, reverse=True)
-        else:
-            data[alias] = option
 
+T = TypeVar('T')
+D = TypeVar('D')
+
+
+def _handle_opt(_pf: str, _parts: list[str], _opts: dict[str, OptionResult]):
+    """处理 `options.xxx.yyy.zzz` 形式的参数"""
+    if _pf == "options":
+        _pf = _parts.pop(0)
+    if not _parts:  # options.foo or foo
+        return _opts, _pf
+    elif not (__src := _opts.get(_pf)):  # options.foo.bar or foo.bar
+        return _opts, _pf
+    if (_end := _parts.pop(0)) == "value":
+        return __src, _end
+    if _end == 'args':
+        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
+    return __src.args, _end
+
+
+def _handle_sub(_pf: str, _parts: list[str], _subs: dict[str, SubcommandResult]):
+    """处理 `subcommands.xxx.yyy.zzz` 形式的参数"""
+    if _pf == "subcommands":
+        _pf = _parts.pop(0)
+    if not _parts:
+        return _subs, _pf
+    elif not (__src := _subs.get(_pf)):
+        return _subs, _pf
+    if (_end := _parts.pop(0)) == "value":
+        return __src, _end
+    if _end == 'args':
+        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
+    if _end == "options" and (_end in __src.options or not _parts):
+        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
+    if _end == "options" or _end in __src.options:
+        return _handle_opt(_end, _parts, __src.options)
+    if _end == "subcommands" and (_end in __src.subcommands or not _parts):
+        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
+    if _end == "subcommands" or _end in __src.subcommands:
+        return _handle_sub(_end, _parts, __src.subcommands)
+    return __src.args, _end
+
+
+class Arparma(Generic[TDC]):
+    """承载解析结果与操作数据的接口类
+
+    Attributes:
+        origin (TDC): 原始数据
+        matched (bool): 是否匹配
+        header_match (HeadResult): 命令头匹配结果
+        error_info (type[BaseException] | BaseException | str): 错误信息
+        error_data (list[str | Any]): 错误数据
+        main_args (dict[str, Any]): 主参数匹配结果
+        other_args (dict[str, Any]): 其他参数匹配结果
+        options (dict[str, OptionResult]): 选项匹配结果
+        subcommands (dict[str, SubcommandResult]): 子命令匹配结果
+    """
+    header_match: HeadResult
+    options: dict[str, OptionResult]
+    subcommands: dict[str, SubcommandResult]
 
-def default_compiler(analyser: SubAnalyser, _config: Namespace, pids: set[str]):
-    require_len = 0
-    for opts in analyser.command.options:
-        if isinstance(opts, Option):
-            _compile_opts(opts, analyser.compile_params)  # type: ignore
-            pids.update(opts.aliases)
-        elif isinstance(opts, Subcommand):
-            sub = SubAnalyser(opts)
-            analyser.compile_params[opts.name] = sub
-            pids.add(opts.name)
-            default_compiler(sub, _config, pids)
-        if not set(analyser.command.separators).issuperset(opts.separators):
-            analyser.default_separate &= False
-        if opts.requires:
-            pids.update(opts.requires)
-            require_len = max(len(opts.requires), require_len)
-            for k in opts.requires:
-                analyser.compile_params.setdefault(k, Sentence(name=k))
-    analyser.part_len = range(
-        len(analyser.command.options) + analyser.need_main_args + require_len
-    )
-
-
-@dataclass
-class SubAnalyser(Generic[TDC]):
-    command: Subcommand
-    default_main_only: bool = field(default=False)  # 默认只有主参数
-    part_len: range = field(default=range(0))  # 分段长度
-    need_main_args: bool = field(default=False)  # 是否需要主参数
-    default_separate: bool = field(default=True)
-    compile_params: dict[str, Sentence | Option | list[Option] | SubAnalyser[TDC]] = field(default_factory=dict)
-
-    self_args: Args = field(init=False)  # 自身参数
-    subcommands_result: dict[str, SubcommandResult] = field(init=False)
-    options_result: dict[str, OptionResult] = field(init=False)  # 存放解析到的所有选项
-    args_result: dict[str, Any] = field(init=False)  # 参数的解析结果
-    header_result: HeadResult | None = field(init=False)
-    value_result: Any = field(init=False)
-    sentences: list[str] = field(init=False)  # 存放解析到的所有句子
+    def __init__(
+        self,
+        source: str,
+        origin: TDC,
+        matched: bool = False,
+        header_match: HeadResult | None = None,
+        error_info: type[BaseException] | BaseException | str = '',
+        error_data: list[str | Any] | None = None,
+        main_args: dict[str, Any] | None = None,
+        options: dict[str, OptionResult] | None = None,
+        subcommands: dict[str, SubcommandResult] | None = None,
+    ):
+        """初始化 `Arparma`
+        Args:
+            source (str): 命令源
+            origin (TDC): 原始数据
+            matched (bool, optional): 是否匹配
+            header_match (HeadResult | None, optional): 命令头匹配结果
+            error_info (type[BaseException] | BaseException | str, optional): 错误信息
+            error_data (list[str | Any] | None, optional): 错误数据
+            main_args (dict[str, Any] | None, optional): 主参数匹配结果
+            options (dict[str, OptionResult] | None, optional): 选项匹配结果
+            subcommands (dict[str, SubcommandResult] | None, optional): 子命令匹配结果
+        """
+        self._source = source
+        self.origin = origin
+        self.matched = matched
+        self.header_match = header_match or HeadResult()
+        self.error_info = error_info
+        self.error_data = error_data or []
+        self.main_args = main_args or {}
+        self.other_args = {}
+        self.options = options or {}
+        self.subcommands = subcommands or {}
 
     def _clr(self):
-        self.reset()
         ks = list(self.__dict__.keys())
         for k in ks:
             delattr(self, k)
 
-    def __post_init__(self):
-        self.reset()
-        self.self_args = self.command.args
-        if self.command.nargs > 0 and self.command.nargs > self.self_args.optional_count:
-            self.need_main_args = True  # 如果need_marg那么match的元素里一定得有main_argument
-        _de_count = sum(arg.field.default_gen is not None for arg in self.self_args.argument)
-        if _de_count and _de_count == self.command.nargs:
-            self.default_main_only = True
-
-    def result(self) -> SubcommandResult:
-        res = SubcommandResult(
-            self.value_result, self.args_result.copy(), self.options_result.copy(), self.subcommands_result.copy()
-        )
-        self.reset()
-        return res
-
-    def reset(self):
-        """重置分析器"""
-        self.args_result = {}
-        self.options_result = {}
-        self.subcommands_result = {}
-        self.sentences = []
-        self.value_result = None
-        self.header_result = None
-
-    def process(self, argv: Argv[TDC]) -> Self:
-        sub = argv.context = self.command
-        if sub.requires and self.sentences != sub.requires:
-            raise ParamsUnmatched(f"{sub.name}'s required is not '{' '.join(self.sentences)}'")
-        self.sentences = []
-        if sub.is_compact:
-            name, _ = argv.next()
-            if not name.startswith(sub.name):
-                raise ParamsUnmatched(f"{name} dose not matched with {sub.name}")
-            argv.rollback(name.lstrip(sub.name), replace=True)
-        else:
-            name, _ = argv.next(sub.separators)
-            if name != sub.name:  # 先匹配选项名称
-                raise ParamsUnmatched(f"{name} dose not matched with {sub.name}")
-
-        if self.part_len.stop == 0:
-            self.value_result = Ellipsis
-            return self
-        return self.analyse(argv)
-
-    def analyse(self, argv: Argv[TDC]) -> Self:
-        for _ in self.part_len:
-            analyse_param(self, argv, self.command.separators)
-        if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(argv, self.self_args)
-        if not self.args_result and self.need_main_args:
-            raise ArgumentMissing(lang.require("subcommand", "args_missing").format(name=self.command.dest))
+    @property
+    def source(self):
+        """返回命令源"""
+        from .manager import command_manager
+        return command_manager.get_command(self._source)
+
+    @property
+    def header(self) -> dict[str, Any]:
+        """返回可能解析到的命令头中的组信息"""
+        return self.header_match.groups
+
+    @property
+    def head_matched(self):
+        """返回命令头是否匹配"""
+        return self.header_match.matched
+
+    @property
+    def header_result(self):
+        """返回命令头匹配结果"""
+        return self.header_match.result
+
+    @property
+    def non_component(self) -> bool:
+        """返回是否没有解析到任何组件"""
+        return not self.subcommands and not self.options
+
+    @property
+    def components(self) -> dict[str, OptionResult | SubcommandResult]:
+        """返回解析到的组件"""
+        return {**self.options, **self.subcommands}
+
+    @property
+    def all_matched_args(self) -> dict[str, Any]:
+        """返回 Alconna 中所有 Args 解析到的值"""
+        return {**self.main_args, **self.other_args}
+
+    @property
+    def token(self) -> int:
+        """返回命令的 Token"""
+        from .manager import command_manager
+        return command_manager.get_token(self)
+
+    def _unpack_opts(self, _data):
+        for _v in _data.values():
+            self.other_args = {**self.other_args, **_v.args}
+
+    def _unpack_subs(self, _data):
+        for _v in _data.values():
+            self.other_args = {**self.other_args, **_v.args}
+            if _v.options:
+                self._unpack_opts(_v.options)
+            if _v.subcommands:
+                self._unpack_subs(_v.subcommands)
+
+    def unpack(self) -> None:
+        """处理 `Arparma` 中的数据"""
+        self._unpack_opts(self.options)
+        self._unpack_subs(self.subcommands)
+
+    @staticmethod
+    def behave_cancel():
+        """取消行为器的后续操作"""
+        raise BehaveCancelled
+
+    @staticmethod
+    def behave_fail():
+        """取消行为器的后续操作并抛出 `OutBoundsBehave`"""
+        raise OutBoundsBehave
+
+    def execute(self, behaviors: list[ArparmaBehavior] | None = None) -> Self:
+        """执行行为器
+
+        Args:
+            behaviors (list[ArparmaBehavior] | None, optional): 要执行的行为器列表
+        Returns:
+            Self: 返回自身
+        """
+        if behaviors := (self.source.behaviors + (behaviors or [])):
+            exc_behaviors = []
+            for behavior in behaviors:
+                exc_behaviors.extend(requirement_handler(behavior))
+            for b in exc_behaviors:
+                b.before_operate(self)
+            for b in exc_behaviors:
+                try:
+                    b.operate(self)
+                except BehaveCancelled:
+                    continue
+                except OutBoundsBehave as e:
+                    return self.fail(e)
         return self
 
-    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDC] | None:
-        if target == self.command:
-            return self
-        for param in self.compile_params.values():
-            if isinstance(param, SubAnalyser):
-                return param.get_sub_analyser(target)
-
-
-class Analyser(SubAnalyser[TDC], Generic[TDC]):
-    command: Alconna  # Alconna实例
-    used_tokens: set[int]  # 已使用的token
-    command_header: Header  # 命令头部
-
-    def __init__(self, alconna: Alconna[TDC], compiler: TCompile | None = None):
-        super().__init__(alconna)
-        self.fuzzy_match = alconna.meta.fuzzy_match
-        self.used_tokens = set()
-        self.command_header = Header.generate(alconna.command, alconna.prefixes)
-        compiler = compiler or default_compiler
-        compiler(
-            self,
-            alconna.namespace_config,
-            command_manager.resolve(self.command).param_ids
-        )
+    def call(self, target: Callable[..., T], **additional) -> T:
+        """依据 `Arparma` 中的数据调用函数
 
-    def _clr(self):
-        self.used_tokens.clear()
-        super()._clr()
+        Args:
+            target (Callable[..., T]): 要调用的函数
+            **additional (Any): 附加参数
+        Returns:
+            T: 函数返回值
+        Raises:
+            RuntimeError: 如果 Arparma 未匹配, 则抛出 RuntimeError
+        """
+        if self.matched:
+            names = {p.name for p in get_signature(target)}
+            return target(**{k: v for k, v in {**self.all_matched_args, **additional}.items() if k in names})
+        raise RuntimeError
+
+    def fail(self, exc: type[BaseException] | BaseException | str):
+        """生成一个失败的 `Arparma`"""
+        return Arparma(self._source, self.origin, False, self.header_match, error_info=exc)
+
+    def __require__(self, parts: list[str]) -> tuple[dict[str, Any] | OptionResult | SubcommandResult | None, str]:
+        """如果能够返回, 除开基本信息, 一定返回该path所在的dict"""
+        if len(parts) == 1:
+            part = parts[0]
+            for src in (self.main_args, self.other_args, self.options, self.subcommands):
+                if part in src:
+                    return src, part
+            if part in {"options", "subcommands", "main_args", "other_args"}:
+                return getattr(self, part, {}), ''
+            return (self.all_matched_args, '') if part == "args" else (None, part)
+        prefix = parts.pop(0)  # parts[0]
+        if prefix in {"options", "subcommands"} and prefix in self.components:
+            raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=prefix))
+        if prefix == "options" or prefix in self.options:
+            return _handle_opt(prefix, parts, self.options)
+        if prefix == "subcommands" or prefix in self.subcommands:
+            return _handle_sub(prefix, parts, self.subcommands)
+        prefix = prefix.replace("$main", "main_args").replace("$other", "other_args")
+        if prefix in {"main_args", "other_args"}:
+            return getattr(self, prefix, {}), parts.pop(0)
+        return None, prefix
+
+    @overload
+    def query(self, path: str) -> Mapping[str, Any] | Any | None:
+        ...
+
+    @overload
+    def query(self, path: str, default: T) -> T | Mapping[str, Any] | Any:
+        ...
+
+    def query(self, path: str, default: T | None = None) -> Any | Mapping[str, Any] | T | None:
+        """查询 `Arparma` 中的数据
+
+        Args:
+            path (str): 要查询的路径
+            default (T | None, optional): 如果查询失败, 则返回该值
+        """
+        source, endpoint = self.__require__(path.split('.'))
+        if source is None:
+            return default
+        if isinstance(source, (OptionResult, SubcommandResult)):
+            return getattr(source, endpoint, default) if endpoint else source
+        return source.get(endpoint, default) if endpoint else MappingProxyType(source)
+
+    @overload
+    def query_with(self, arg_type: type[T]) -> T | None:
+        ...
+
+    @overload
+    def query_with(self, arg_type: type[T], path: str) -> T | None:
+        ...
+
+    @overload
+    def query_with(self, arg_type: type[T], *, default: D) -> T | D:
+        ...
+
+    @overload
+    def query_with(self, arg_type: type[T], path: str, default: D) -> T | D:
+        ...
+
+    def query_with(self, arg_type: type[T], path: str | None = None, default: D | None = None) -> T | D | None:
+        """查询 `Arparma` 中的数据并检查类型
+
+        Args:
+            arg_type (type[T]): 要检查的类型
+            path (str | None, optional): 要查询的路径
+            default (D | None, optional): 如果查询失败, 则返回该值
+        """
+        if path:
+            return res if generic_isinstance(res := self.query(path, Empty), arg_type) else default
+        with suppress(StopIteration):
+            return next(v for v in self.all_matched_args.values() if generic_isinstance(v, arg_type))
+        return default
+
+    def find(self, path: str) -> bool:
+        """查询路径是否存在
+
+        Args:
+            path (str): 要查询的路径
+
+        Returns:
+            bool: 是否存在
+        """
+        return self.query(path, Empty) != Empty
+
+    @overload
+    def __getitem__(self, item: type[T]) -> T | None:
+        ...
+
+    @overload
+    def __getitem__(self, item: str) -> Any:
+        ...
+
+    def __getitem__(self, item: str | type[T]) -> T | Any | None:
+        """查询 `Arparma` 中的数据
+
+        Args:
+            item (str | type[T]): 要查询的路径或类型
+        """
+
+        if isinstance(item, str):
+            return self.query(item)
+        if data := self.query_with(item):
+            return data
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__} of {self.command.path}>"
+    def __getattr__(self, item: str):
+        return self.all_matched_args.get(item, self.query(item.replace('_', '.')))
 
-    def shortcut(
-        self,
-        argv: Argv[TDC],
-        data: list[Any], short: Arparma | ShortcutArgs,
-        reg: Match | None
-    ) -> Arparma[TDC]:
-        if isinstance(short, Arparma):
-            return short
-        argv.build(short.get('command', self.command.command or self.command.name))
-        if not short.get('fuzzy') and data:
-            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=data[0]))
-            if self.command.meta.raise_exception:
-                raise exc
-            return self.export(argv, True, exc)
-        data_index = 0
-        for i, unit in enumerate(argv.raw_data):
-            if not data:
-                break
-            if not isinstance(unit, str):
+    def __repr__(self):
+        if self.error_info:
+            attrs = ((s, getattr(self, s, None)) for s in ("matched", "header_match", "error_data", "error_info"))
+            return ", ".join([f"{a}={v}" for a, v in attrs if v is not None])
+        else:
+            attrs = {
+                "matched": self.matched, "header_match": self.header_match,
+                "options": self.options, "subcommands": self.subcommands,
+                "main_args": self.main_args, "other_args": self.other_args
+            }
+            return ", ".join([f"{a}={v}" for a, v in attrs.items() if v])
+
+
+@dataclass(init=True, unsafe_hash=True, repr=True)
+class ArparmaBehavior(metaclass=ABCMeta):
+    """解析结果行为器的基类, 对应一个对解析结果的操作行为
+
+    Attributes:
+        requires (list[ArparmaBehavior]): 该行为器所依赖的行为器
+    """
+    record: dict[int, dict[str, tuple[Any, Any]]] = field(default_factory=dict, init=False, repr=False, hash=False)
+    requires: list[ArparmaBehavior] = field(init=False, hash=False, repr=False)
+
+    def before_operate(self, interface: Arparma):
+        """在操作前调用, 用于准备数据"""
+        if not self.record:
+            return
+        if not (_record := self.record.get(interface.token, None)):
+            return
+        for path, (past, current) in _record.items():
+            source, end = interface.__require__(path.split("."))
+            if source is None:
                 continue
-            if unit == f"{{%{data_index}}}":
-                argv.raw_data[i] = data.pop(0)
-                data_index += 1
-            elif f"{{%{data_index}}}" in unit:
-                argv.raw_data[i] = unit.replace(f"{{%{data_index}}}", str(data.pop(0)))
-                data_index += 1
-            elif mat := re.search(r"\{\*(.*)\}", unit, re.DOTALL):
-                sep = mat[1]
-                argv.raw_data[i] = unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data)))
-                data.clear()
-
-        argv.bak_data = argv.raw_data.copy()
-        argv.addon(*data).addon(*short.get('args', []))
-        if reg:
-            groups: tuple[str, ...] = reg.groups()
-            gdict: dict[str, str] = reg.groupdict()
-            for j, unit in enumerate(argv.raw_data):
-                if not isinstance(unit, str):
-                    continue
-                for i, c in enumerate(groups):
-                    unit = unit.replace(f"{{{i}}}", c)
-                for k, v in gdict.items():
-                    unit = unit.replace(f"{{{k}}}", v)
-                argv.raw_data[j] = unit
-        if argv.message_cache:
-            argv.token = argv.generate_token(argv.raw_data)
-        return self.process(argv)
-
-    def process(self, argv: Argv[TDC]) -> Arparma[TDC]:
-        """主体解析函数, 应针对各种情况进行解析"""
-        if (
-            argv.message_cache and
-            argv.token in self.used_tokens and
-            (res := command_manager.get_record(argv.token))
-        ):
-            return res
-        try:
-            self.header_result = analyse_header(self.command_header, argv)
-        except ParamsUnmatched as e:
-            argv.raw_data = argv.bak_data.copy()
-            argv.current_index = 0
-            try:
-                _res = command_manager.find_shortcut(self.command, argv.next(move=False)[0])
-            except ValueError as exc:
-                if self.command.meta.raise_exception:
-                    raise e from exc
-                return self.export(argv, True, e)
+            if isinstance(source, dict):
+                if past != Empty:
+                    source[end] = past
+                elif source.get(end, Empty) != current:
+                    source.pop(end)
+            elif past != Empty:
+                setattr(source, end, past)
+            elif getattr(source, end, Empty) != current:
+                delattr(source, end)
+        _record.clear()
+
+    @abstractmethod
+    def operate(self, interface: Arparma):
+        """对解析结果进行操作"""
+        ...
+
+    def update(self, interface: Arparma, path: str, value: Any):
+        """更新解析结果
+
+        Args:
+            interface (Arparma): Arparma 实例
+            path (str): 要更新的路径
+            value (Any): 要更新的值
+        """
+        def _update(tkn, src, pth, ep, val):
+            _record = self.record.setdefault(tkn, {})
+            if isinstance(src, dict):
+                _record[pth] = (src.get(ep, Empty), val)
+                src[ep] = val
             else:
-                argv.next()
-                data = argv.release()
-                self.reset()
-                argv.reset()
-                return self.shortcut(argv, data, *_res)
-
-        except FuzzyMatchSuccess as Fuzzy:
-            output_manager.send(self.command.name, lambda: str(Fuzzy))
-            return self.export(argv, True)
-
-        if fail := self.analyse(argv):
-            return fail
-
-        if argv.done and (not self.need_main_args or self.args_result):
-            return self.export(argv)
-
-        rest = argv.release()
-        if len(rest) > 0:
-            if isinstance(rest[-1], str) and rest[-1] in argv.completion_names:
-                last = argv.bak_data[-1]
-                argv.bak_data[-1] = last[:last.rfind(rest[-1])]
-                return handle_completion(self, argv, rest[-2])
-            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=argv.next(move=False)[0]))
-        else:
-            exc = ArgumentMissing(lang.require("analyser", "param_missing"))
-        if isinstance(exc, ArgumentMissing) and comp_ctx.get(None):
-            raise PauseTriggered(prompt(self, argv))
-        if self.command.meta.raise_exception:
-            raise exc
-        return self.export(argv, True, exc)
-
-    def analyse(self, argv: Argv[TDC]) -> Arparma[TDC] | None:
-        for _ in self.part_len:
-            try:
-                analyse_param(self, argv)
-            except FuzzyMatchSuccess as e:
-                output_manager.send(self.command.name, lambda: str(e))
-                return self.export(argv, True)
-            except SpecialOptionTriggered as sot:
-                return _SPECIAL[sot.args[0]](self, argv)
-            except (ParamsUnmatched, ArgumentMissing) as e1:
-                if (rest := argv.release()) and isinstance(rest[-1], str):
-                    if rest[-1] in argv.completion_names:
-                        last = argv.bak_data[-1]
-                        argv.bak_data[-1] = last[:last.rfind(rest[-1])]
-                        return handle_completion(self, argv)
-                    if handler := argv.special.get(rest[-1]):
-                        return _SPECIAL[handler](self, argv)
-                if isinstance(e1, ArgumentMissing) and comp_ctx.get(None):
-                    raise PauseTriggered(prompt(self, argv)) from e1
-                if self.command.meta.raise_exception:
-                    raise
-                return self.export(argv, True, e1)
-            if argv.done:
-                break
-
-        if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(argv, self.self_args)
-
-    def export(
-        self,
-        argv: Argv[TDC],
-        fail: bool = False,
-        exception: BaseException | None = None,
-    ) -> Arparma[TDC]:
-        """创建arpamar, 其一定是一次解析的最后部分"""
-        result = Arparma(self.command.path, argv.origin, not fail, self.header_result)
-        if fail:
-            result.error_info = repr(exception or traceback.format_exc(limit=1))
-            result.error_data = argv.release()
-        else:
-            result.main_args = self.args_result
-            result.options = self.options_result
-            result.subcommands = self.subcommands_result
-            result.unpack()
-            if argv.message_cache:
-                command_manager.record(argv.token, result)
-                self.used_tokens.add(argv.token)
-        self.reset()
-        return result  # type: ignore
-
+                _record[pth] = (getattr(src, ep, Empty), val)
+                setattr(src, ep, val)
 
-TCompile: TypeAlias = "Callable[[SubAnalyser, Namespace, set[str]], None]"
+        source, end = interface.__require__(path.split("."))
+        if source is None:
+            return
+        if end:
+            _update(interface.token, source, path, end, value)
+        elif isinstance(value, dict):
+            for k, v in value.items():
+                _update(interface.token, source, f"{path}.{k}", k, v)
+
+
+@lru_cache(4096)
+def requirement_handler(behavior: ArparmaBehavior) -> list[ArparmaBehavior]:
+    res = []
+    for b in getattr(behavior, 'requires', []):
+        res.extend(requirement_handler(b))
+    res.append(behavior)
+    return res
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/args.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/formatter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,288 +1,283 @@
 from __future__ import annotations
 
-import inspect
-import re
-from copy import deepcopy
-from dataclasses import field as dc_field
-from enum import Enum
-from functools import partial
-from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union, TYPE_CHECKING
-from tarina import Empty, get_signature, lang
-from nepattern import AllParam, AnyOne, BasePattern, UnionPattern, type_parser
-from typing_extensions import Self
+from contextlib import suppress
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any
+from tarina import Empty, lang
+from nepattern import AllParam, BasePattern
 
-from .exceptions import InvalidParam
-from .typing import KeyWordVar, MultiVar
+from .args import Arg, Args
+from .base import Option, Subcommand
 
 if TYPE_CHECKING:
-    from dataclasses import dataclass
-else:
-    from .util import dataclass
-
-_T = TypeVar("_T")
-TAValue = Union[BasePattern, AllParam.__class__, type, str]
-
-
-class ArgFlag(str, Enum):
-    OPTIONAL = '?'
-    HIDDEN = "/"
-    ANTI = "!"
-
-
-@dataclass(slots=True)
-class Field(Generic[_T]):
-    """标识参数单元字段"""
-    default: _T | None = dc_field(default=None)
-    default_factory: Callable[[], _T | None] = dc_field(default=lambda: None)
-    alias: str | None = dc_field(default=None)
-    completion: Callable[[], str | list[str]] | None = dc_field(default=None)
-    display: Any = dc_field(init=False)
-    default_gen: _T | None = dc_field(init=False)
-
-    def __post_init__(self):
-        self.default_gen = self.default if self.default is not None else self.default_factory()
-        self.display = self.alias or self.default_gen
-
-
-@dataclass(init=False, eq=True, unsafe_hash=True, slots=True)
-class Arg:
-    name: str = dc_field(compare=True, hash=True)
-    value: Union[BasePattern, AllParam.__class__] = dc_field(compare=False, hash=True)
-    field: Field[Any] = dc_field(compare=False, hash=False)
-    notice: str | None = dc_field(compare=False, hash=False)
-    flag: set[ArgFlag] = dc_field(compare=False, hash=False)
-    separators: tuple[str, ...] = dc_field(compare=False, hash=False)
-    optional: bool = dc_field(compare=False, hash=False)
-    hidden: bool = dc_field(compare=False, hash=False)
-    anonymous: bool = dc_field(compare=False, hash=False)
-
-    def __init__(
-        self,
-        name: str,
-        value: TAValue | None = None,
-        field: Field[_T] | _T | None = None,
-        seps: str | Iterable[str] = " ",
-        notice: str | None = None,
-        flags: list[ArgFlag] | None = None,
-    ):
-        if not isinstance(name, str) or name.startswith('$'):
-            raise InvalidParam(lang.require("args", "name_error"))
-        if not name.strip():
-            raise InvalidParam(lang.require("args", "name_empty"))
-        self.name = name
-        _value = type_parser(value or name)
-        default = field if isinstance(field, Field) else Field(field)
-        if isinstance(_value, UnionPattern) and _value.optional:
-            default.default = Empty if default.default is None else default.default
-        if default.default == "...":
-            default.default = Empty
-        if _value is Empty:
-            raise InvalidParam(lang.require("args", "value_error").format(target=name))
-        self.value = _value
-        self.field = default
-        self.notice = notice
-        self.separators = (seps,) if isinstance(seps, str) else tuple(seps)
-        flags = flags or []
-        if res := re.match(r"^.+?#(?P<notice>[^;?!/#]+)", name):
-            self.notice = res["notice"]
-            self.name = name.replace(f"#{res['notice']}", "")
-        if res := re.match(r"^.+?;(?P<flag>[?!/]+)", self.name):
-            flags.extend(ArgFlag(c) for c in res["flag"])
-            self.name = self.name.replace(f";{res['flag']}", "")
-        self.flag = set(flags)
-        self.optional = ArgFlag.OPTIONAL in self.flag
-        self.hidden = ArgFlag.HIDDEN in self.flag
-        self.anonymous = self.name.startswith("_key_")
-        if ArgFlag.ANTI in self.flag and self.value not in (AnyOne, AllParam):
-            self.value = deepcopy(self.value).reverse()
-
-    def __repr__(self):
-        return (n if (n := f"'{self.name}'") == (v := str(self.value)) else f"{n}: {v}") + (
-            f" = '{self.field.display}'" if self.field.display is not None else ""
-        )
-
-
-class ArgsMeta(type):
-    """Args 类的元类"""
+    from .core import Alconna
 
-    def __getattr__(self, name):
-        return type("_S", (), {"__getitem__": partial(self.__class__.__getitem__, self, key=name), "__call__": None})()
 
-    def __getitem__(self, item, key: str | None = None):
-        data = item if isinstance(item, tuple) else (item,)
-        if isinstance(data[0], Arg):
-            return self(*data)
-        return self(Arg(key, *data)) if key else self(Arg(*data))
-
-
-class Args(metaclass=ArgsMeta):
-    argument: list[Arg]
-    var_positional: str | None
-    var_keyword: str | None
-    keyword_only: list[str]
-    optional_count: int
-
-    @classmethod
-    def from_callable(cls, target: Callable):
-        """从可调用函数中构造Args"""
-        _args = cls()
-        method = False
-        for param in get_signature(target):
-            name = param.name
-            if name in ["self", "cls"]:
-                method = True
-                continue
-            anno = param.annotation
-            de = param.default
-            NULL = {Empty: None, None: Empty}
-            if anno == inspect.Signature.empty:
-                anno = type(de) if de not in NULL else AnyOne
-            de = NULL.get(de, de)
-            if param.kind == param.KEYWORD_ONLY:
-                if anno == bool:
-                    anno = BasePattern(f"(?:-*no)?-*{name}", 3, bool, lambda _, x: not x.lstrip("-").startswith('no'))
-                    _args.keyword_only.append(name)
+def resolve_requires(options: list[Option | Subcommand]):
+    """Resolve the requires of options."""
+    reqs: dict[str, dict | Option | Subcommand] = {}
+
+    def _u(target, source):
+        for k in source:
+            if k not in target or isinstance(target[k], (Option, Subcommand)):
+                target.update(source)
+                break
+            _u(target[k], source[k])
+
+    for opt in options:
+        if not opt.requires:
+            # reqs.setdefault(opt.name, opt)
+            [reqs.setdefault(i, opt) for i in opt.aliases] if isinstance(opt, Option) else None
+            reqs.setdefault(opt.name, resolve_requires(opt.options)) if isinstance(opt, Subcommand) else None
+        else:
+            _reqs = _cache = {}
+            for req in opt.requires:
+                if not _reqs:
+                    _reqs[req] = {}
+                    _cache = _reqs[req]
                 else:
-                    anno = KeyWordVar(anno, sep=' ')
-            if param.kind == param.VAR_POSITIONAL:
-                anno = MultiVar(anno, "*")
-            if param.kind == param.VAR_KEYWORD:
-                anno = MultiVar(KeyWordVar(anno), "*")
-            _args.add(name, value=anno, default=de)
-        return _args, method
-
-    def __init__(
-        self, *args: Arg, separators: str | Iterable[str] | None = None, **kwargs: TAValue
-    ):
-        """
-        构造一个Args
+                    _cache[req] = {}
+                    _cache = _cache[req]
+            # _cache[opt.name] = opt  # type: ignore
+            [_cache.setdefault(i, opt) for i in opt.aliases] if isinstance(opt, Option) else None  # type: ignore
+            _cache.setdefault(opt.name, resolve_requires(opt.options)) if isinstance(opt, Subcommand) else None
+            _u(reqs, _reqs)
+    return reqs
+
+
+def ensure_node(target: str, options: list[Option | Subcommand]):
+    for opt in options:
+        if isinstance(opt, Option) and target in opt.aliases:
+            return opt
+        if isinstance(opt, Subcommand):
+            return opt if target == opt.name else ensure_node(target, opt.options)
+
+
+@dataclass(eq=True)
+class Trace:
+    """存放命令节点数据的结构
+
+    该结构用于存放命令节点的数据，包括命令节点的头部、参数、分隔符和主体。
+    """
+    head: dict[str, Any]
+    args: Args
+    separators: tuple[str, ...]
+    body: list[Option | Subcommand]
+
+    def union(self, others: list[Trace]):
+        """合并多个 Trace 对象
 
         Args:
-            args: 应传入 slice|tuple, 代表key、value、default
-            extra: 额外类型检查的策略
-            separator: 参数分隔符
-            kwargs: 其他参数
+            others (list[Trace]): 待合并的 Trace 对象列表
+
+        Returns:
+            Trace: 合并后的 Trace 对象
         """
-        self._visit = set()
-        self.var_positional = None
-        self.var_keyword = None
-        self.keyword_only = []
-        self.optional_count = 0
-        self.argument = list(args)
-        self.argument.extend(Arg(k, type_parser(v), Field()) for k, v in kwargs.items())
-        self.__check_vars__()
-        if separators is not None:
-            self.separate(*((separators,) if isinstance(separators, str) else tuple(separators)))
-
-    __slots__ = "var_positional", "var_keyword", "argument", "optional_count", "keyword_only", "_visit"
-
-    def add(self, name: str, *, value: Any, default: Any = None, flags: list[ArgFlag] | None = None) -> Self:
-        """添加一个参数"""
-        if next(filter(lambda x: x.name == name, self.argument), False):
+        if not others:
             return self
-        self.argument.append(Arg(name, value, default, flags=flags))
-        self.__check_vars__()
+        if others[0] == self:
+            return self.union(others[1:])
+        pfs = self.head.copy()
+        pfs['prefix'] = list({*self.head['prefix'], *others[0].head['prefix']})
+        return Trace(pfs, self.args, self.separators, list({*self.body, *others[0].body})).union(others[1:])
+
+
+class TextFormatter:
+    """帮助文档格式化器
+
+    该格式化器负责将传入的命令解析并生成帮助文档字符串
+    """
+
+    def __init__(self):
+        self.data = {}
+        self.ignore_names = set()
+
+    def add(self, base: Alconna):
+        """添加目标命令"""
+        self.ignore_names.update(base.namespace_config.builtin_option_name['help'])
+        self.ignore_names.update(base.namespace_config.builtin_option_name['shortcut'])
+        self.ignore_names.update(base.namespace_config.builtin_option_name['completion'])
+        pfs = base.prefixes.copy()
+        if base.name in pfs:
+            pfs.remove(base.name)  # type: ignore
+        res = Trace(
+            {
+                'name': base.name, 'prefix': pfs or [], 'description': base.meta.description,
+                'usage': base.meta.usage, 'example': base.meta.example
+            },
+            base.args, base.separators, base.options.copy()
+        )
+        self.data.setdefault(base.path, []).append(res)
         return self
 
-    def default(self, **kwargs) -> Self:
-        """设置参数的默认值"""
-        for arg in self.argument:
-            if v := (kwargs.get(arg.name)):
-                if isinstance(v, Field):
-                    arg.field = v
-                else:
-                    arg.field.default = v
-        return self
+    def remove(self, base: Alconna | str):
+        """移除目标命令"""
+        if isinstance(base, str):
+            self.data.pop(base)
+        else:
+            with suppress(ValueError):
+                self.data.get(base.path, []).remove(base)
 
-    def separate(self, *separator: str) -> Self:
-        """设置参数的分隔符"""
-        for arg in self.argument:
-            arg.separators = separator
-        return self
+    def format_node(self, parts: list | None = None):
+        """格式化命令节点
 
-    def __check_vars__(self):
-        _tmp = []
-        _visit = set()
-        for arg in self.argument:
-            if arg.name in _visit:
-                continue
-            _tmp.append(arg)
-            _visit.add(arg.name)
-            if arg.name in self._visit:
-                continue
-            self._visit.add(arg.name)
-            _limit = False
-            if isinstance(arg.value, MultiVar) and not _limit:
-                if isinstance(arg.value.base, KeyWordVar):
-                    if self.var_keyword:
-                        raise InvalidParam(lang.require("args", "duplicate_kwargs"))
-                    self.var_keyword = arg.name
-                elif self.var_positional:
-                    raise InvalidParam(lang.require("args", "duplicate_varargs"))
+        Args:
+            parts (list | None, optional): 可能的节点路径.
+        """
+        def _handle(traces: list[Trace]):
+            trace = traces[0].union(traces[1:])
+            if not parts or parts == ['']:
+                return self.format(trace)
+            _cache = resolve_requires(trace.body)
+            _parts = []
+            for text in parts:
+                if isinstance(_cache, dict) and text in _cache:
+                    _cache = _cache[text]
+                    _parts.append(text)
+            if not _parts:
+                return self.format(trace)
+            if isinstance(_cache, dict):
+                if ensure := ensure_node(_parts[-1], trace.body):
+                    _cache = ensure
                 else:
-                    self.var_positional = arg.name
-                _limit = True
-            if isinstance(arg.value, KeyWordVar):
-                if self.var_keyword or self.var_positional:
-                    raise InvalidParam(lang.require("args", "exclude_mutable_args"))
-                self.keyword_only.append(arg.name)
-                if arg.value.sep in arg.separators:
-                    _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"-*{arg.name}"))
-                    _tmp[-1].value = arg.value.base
-            if ArgFlag.OPTIONAL in arg.flag:
-                if self.var_keyword or self.var_positional:
-                    raise InvalidParam(lang.require("args", "exclude_mutable_args"))
-                self.optional_count += 1
-        self.argument.clear()
-        self.argument.extend(_tmp)
-        del _tmp
-        del _visit
-
-    def __len__(self):
-        return len(self.argument)
-
-    def __getitem__(self, item) -> Self | Arg:
-        if isinstance(item, str) and (res := next(filter(lambda x: x.name == item, self.argument), None)):
-            return res
-        data = item if isinstance(item, tuple) else (item,)
-        if isinstance(data[0], Arg):
-            self.argument.extend(data)  # type: ignore
-        else:
-            self.argument.append(Arg(*data))  # type: ignore
-        self.__check_vars__()
-        return self
+                    _opts, _visited = [], set()
+                    for k, i in _cache.items():
+                        if isinstance(i, dict):
+                            _opts.append(Option(k, requires=_parts))
+                        elif i not in _visited:
+                            _opts.append(i)
+                            _visited.add(i)
+                    return self.format(Trace(
+                        {"name": _parts[-1], 'prefix': [], 'description': _parts[-1]}, Args(), trace.separators,
+                        _opts
+                    ))
+            if isinstance(_cache, Option):
+                return self.format(Trace(
+                    {"name": "", "prefix": list(_cache.aliases), "description": _cache.help_text}, _cache.args,
+                    _cache.separators, []
+                ))
+            if isinstance(_cache, Subcommand):
+                return self.format(Trace(
+                    {"name": _cache.name, "prefix": [], "description": _cache.help_text}, _cache.args,
+                    _cache.separators, _cache.options  # type: ignore
+                ))
+            return self.format(trace)
 
-    def __merge__(self, other) -> Self:
-        if isinstance(other, Args):
-            self.argument.extend(other.argument)
-            self.__check_vars__()
-            self.keyword_only = list(set(self.keyword_only + other.keyword_only))
-            del other
-        elif isinstance(other, Arg):
-            self.argument.append(other)
-            self.__check_vars__()
-        elif isinstance(other, Sequence):
-            self.__getitem__(tuple(other))
-        return self
+        return "\n".join([_handle(v) for v in self.data.values()])
 
-    __add__ = __merge__
-    __iadd__ = __merge__
-    __lshift__ = __merge__
-    __iter__ = lambda self: iter(self.argument)
+    def format(self, trace: Trace) -> str:
+        """帮助文本的生成入口
 
-    def __truediv__(self, other) -> Self:
-        self.separate(*other if isinstance(other, (list, tuple, set)) else other)
-        return self
+        Args:
+            trace (Trace): 命令节点数据
+        """
+        prefix = self.header(trace.head, trace.separators)
+        param = self.parameters(trace.args)
+        body = self.body(trace.body)
+        return prefix % (param, body)
+
+    def param(self, parameter: Arg) -> str:
+        """对单个参数的描述
+
+        Args:
+            parameter (Arg): 参数单元
+        """
+        name = parameter.name
+        arg = f"[{name}" if parameter.optional else f"<{name}"
+        if not parameter.hidden:
+            if parameter.value is AllParam:
+                return f"<...{name}>"
+            if not isinstance(parameter.value, BasePattern) or parameter.value.pattern != name:
+                arg += f": {parameter.value}"
+            if parameter.field.display is Empty:
+                arg += " = None"
+            elif parameter.field.display is not None:
+                arg += f" = {parameter.field.display}"
+        return f"{arg}]" if parameter.optional else f"{arg}>"
 
-    def __eq__(self, other):
-        return self.argument == other.argument
+    def parameters(self, args: Args) -> str:
+        """参数列表的描述
 
-    def __repr__(self):
+        Args:
+            args (Args): 参数列表
+        """
+        res = ""
+        for arg in args.argument:
+            if arg.name.startswith('_key_'):
+                continue
+            if len(arg.separators) == 1:
+                sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
+            else:
+                sep = f"[{'|'.join(arg.separators)!r}]"
+            res += self.param(arg) + sep
+        notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
         return (
-            f"Args({', '.join([f'{arg}' for arg in self.argument if not arg.anonymous])})"
-            if self.argument else "Empty"
+            f"{res}\n## {lang.require('format', 'notice')}\n  " +
+            "\n  ".join([f"{v[0]}: {v[1]}" for v in notice])
+        ) if notice else res
+
+
+    def header(self, root: dict[str, Any], separators: tuple[str, ...]) -> str:
+        """头部节点的描述
+
+        Args:
+            root (dict[str, Any]): 头部节点数据
+            separators (tuple[str, ...]): 分隔符
+        """
+        help_string = f"\n{desc}" if (desc := root.get('description')) else ""
+        usage = f"\n{lang.require('format', 'usage')}:\n{usage}" if (usage := root.get('usage')) else ""
+        example = f"\n{lang.require('format', 'example')}:\n{example}" if (example := root.get('example')) else ""
+        prefixs = f"[{''.join(map(str, prefixs))}]" if (prefixs := root.get('prefix', [])) != [] else ""
+        cmd = f"{prefixs}{root.get('name', '')}"
+        command_string = cmd or (root['name'] + separators[0])
+        return f"{command_string} %s{help_string}{usage}\n\n%s{example}"
+
+    def opt(self, node: Option) -> str:
+        """对单个选项的描述"""
+        alias_text = " ".join(node.requires) + (' ' if node.requires else '') + "|".join(node.aliases)
+        return (
+            f"* {node.help_text}\n"
+            f"  {alias_text}{node.separators[0]}{self.parameters(node.args)}\n"
+        )
+
+    def sub(self, node: Subcommand) -> str:
+        """对单个子命令的描述"""
+        name = " ".join(node.requires) + (' ' if node.requires else '') + node.name
+        opt_string = "".join(
+            [
+                self.opt(opt).replace("\n", "\n  ").replace("# ", "* ")
+                for opt in filter(lambda x: isinstance(x, Option), node.options)
+            ]
         )
+        sub_string = "".join(
+            [
+                self.opt(sub).replace("\n", "\n  ").replace("# ", "* ")  # type: ignore
+                for sub in filter(lambda x: isinstance(x, Subcommand), node.options)
+            ]
+        )
+        opt_help = f"  {lang.require('format', 'subcommands.opts')}:\n  " if opt_string else ""
+        sub_help = f"  {lang.require('format', 'subcommands.subs')}:\n  " if sub_string else ""
+        return (
+            f"* {node.help_text}\n"
+            f"  {name}{tuple(node.separators)[0]}{self.parameters(node.args)}\n"
+            f"{sub_help}{sub_string}"
+            f"{opt_help}{opt_string}"
+        ).rstrip(' ')
+
+    def body(self, parts: list[Option | Subcommand]) -> str:
+        """子节点列表的描述"""
+        option_string = "".join(
+            [
+                self.opt(opt) for opt in filter(lambda x: isinstance(x, Option), parts)
+                if opt.name not in self.ignore_names
+            ]
+        )
+        subcommand_string = "".join(
+            [self.sub(sub) for sub in filter(lambda x: isinstance(x, Subcommand), parts)]
+        )
+        option_help = f"{lang.require('format', 'options')}:\n" if option_string else ""
+        subcommand_help = f"{lang.require('format', 'subcommands')}:\n" if subcommand_string else ""
+        return f"{subcommand_help}{subcommand_string}{option_help}{option_string}"
+
 
-    @property
-    def empty(self) -> bool:
-        return not self.argument
+__all__ = ["TextFormatter", "Trace"]
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,319 +1,345 @@
+"""Alconna 的基础内容相关"""
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
-from contextlib import suppress
-from dataclasses import dataclass, field
-from functools import lru_cache
-from types import MappingProxyType
-from typing import Any, Callable, Generic, Mapping, TypeVar, overload
-from tarina import get_signature, generic_isinstance, Empty, lang
+from functools import reduce
+from typing import Iterable, Sequence, overload, Any
 from typing_extensions import Self
+from tarina import lang
 
-from .exceptions import BehaveCancelled, OutBoundsBehave
-from .model import HeadResult, OptionResult, SubcommandResult
-from .typing import TDC
-
-T = TypeVar('T')
-D = TypeVar('D')
-
-
-def _handle_opt(_pf: str, _parts: list[str], _opts: dict[str, OptionResult]):
-    if _pf == "options":
-        _pf = _parts.pop(0)
-    if not _parts:  # options.foo or foo
-        return _opts, _pf
-    elif not (__src := _opts.get(_pf)):  # options.foo.bar or foo.bar
-        return _opts, _pf
-    if (_end := _parts.pop(0)) == "value":
-        return __src, _end
-    if _end == 'args':
-        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
-    return __src.args, _end
-
-
-def _handle_sub(_pf: str, _parts: list[str], _subs: dict[str, SubcommandResult]):
-    if _pf == "subcommands":
-        _pf = _parts.pop(0)
-    if not _parts:
-        return _subs, _pf
-    elif not (__src := _subs.get(_pf)):
-        return _subs, _pf
-    if (_end := _parts.pop(0)) == "value":
-        return __src, _end
-    if _end == 'args':
-        return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
-    if _end == "options" and (_end in __src.options or not _parts):
-        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
-    if _end == "options" or _end in __src.options:
-        return _handle_opt(_end, _parts, __src.options)
-    if _end == "subcommands" and (_end in __src.subcommands or not _parts):
-        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
-    if _end == "subcommands" or _end in __src.subcommands:
-        return _handle_sub(_end, _parts, __src.subcommands)
-    return __src.args, _end
-
-
-class Arparma(Generic[TDC]):
-    """承载解析结果与操作数据的接口类"""
-    header_match: HeadResult
-    options: dict[str, OptionResult]
-    subcommands: dict[str, SubcommandResult]
+from .action import Action, store
+from .args import Arg, Args
+from .exceptions import InvalidParam
+from .model import OptionResult, SubcommandResult
+
+
+def _handle_default(node: CommandNode):
+    if node.default is None:
+        return
+    act = node.action
+    if isinstance(node.default, (OptionResult, SubcommandResult)):
+        if act.type == 0 and act.value is ...:
+            act.value = node.default.value
+        if act.type == 1:
+            if not isinstance(node.default.value, list):
+                node.default.value = [node.default.value]
+            if act.value[0] is ...:
+                act.value = node.default.value[:]
+        if act.type == 2 and not isinstance(node.default.value, int):
+            node.default.value = 1
+    else:
+        if act.type == 0 and act.value is ...:
+            act.value = node.default
+        if act.type == 1:
+            if not isinstance(node.default, list):
+                node.default = [node.default]
+            if act.value[0] is ...:
+                act.value = node.default[:]
+        if act.type == 2 and not isinstance(node.default, int):
+            node.default = 1
+
+
+class CommandNode:
+    """命令节点基类, 规定基础组件所含属性"""
+
+    name: str
+    """命令节点名称"""
+    dest: str
+    """命令节点目标名称"""
+    default: Any
+    """命令节点默认值"""
+    args: Args
+    """命令节点参数"""
+    separators: tuple[str, ...]
+    """命令节点分隔符"""
+    action: Action
+    """命令节点响应动作"""
+    help_text: str
+    """命令节点帮助信息"""
+    requires: list[str]
+    """命令节点需求前缀"""
 
     def __init__(
-        self,
-        source: str,
-        origin: TDC,
-        matched: bool = False,
-        header_match: HeadResult | None = None,
-        error_info: type[BaseException] | BaseException | str = '',
-        error_data: list[str | Any] | None = None,
-        main_args: dict[str, Any] | None = None,
-        options: dict[str, OptionResult] | None = None,
-        subcommands: dict[str, SubcommandResult] | None = None,
+        self, name: str, args: Arg | Args | None = None,
+        dest: str | None = None, default: Any = None, action: Action | None = None,
+        separators: str | Sequence[str] | set[str] | None = None,
+        help_text: str | None = None,
+        requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
     ):
-        self._source = source
-        self.origin = origin
-        self.matched = matched
-        self.header_match = header_match or HeadResult()
-        self.error_info = error_info
-        self.error_data = error_data or []
-        self.main_args = main_args or {}
-        self.other_args = {}
-        self.options = options or {}
-        self.subcommands = subcommands or {}
-
-    def _clr(self):
-        ks = list(self.__dict__.keys())
-        for k in ks:
-            delattr(self, k)
-
-    @property
-    def source(self):
-        from .manager import command_manager
-        return command_manager.get_command(self._source)
-
-    @property
-    def header(self) -> dict[str, Any]:
-        """返回可能解析到的命令头中的信息"""
-        return self.header_match.groups
-
-    @property
-    def head_matched(self):
-        return self.header_match.matched
-
-    @property
-    def header_result(self):
-        return self.header_match.result
-
-    @property
-    def non_component(self) -> bool:
-        return not self.subcommands and not self.options
-
-    @property
-    def components(self) -> dict[str, OptionResult | SubcommandResult]:
-        return {**self.options, **self.subcommands}
-
-    @property
-    def all_matched_args(self) -> dict[str, Any]:
-        """返回 Alconna 中所有 Args 解析到的值"""
-        return {**self.main_args, **self.other_args}
-
-    @property
-    def token(self) -> int:
-        from .manager import command_manager
-        return command_manager.get_token(self)
-
-    def _unpack_opts(self, _data):
-        for _v in _data.values():
-            self.other_args = {**self.other_args, **_v.args}
-
-    def _unpack_subs(self, _data):
-        for _v in _data.values():
-            self.other_args = {**self.other_args, **_v.args}
-            if _v.options:
-                self._unpack_opts(_v.options)
-            if _v.subcommands:
-                self._unpack_subs(_v.subcommands)
+        """
+        初始化命令节点
 
-    def unpack(
-        self,
-    ) -> None:
-        """处理 Arparma 中的数据"""
-        self._unpack_opts(self.options)
-        self._unpack_subs(self.subcommands)
-
-    @staticmethod
-    def behave_cancel():
-        raise BehaveCancelled
-
-    @staticmethod
-    def behave_fail():
-        raise OutBoundsBehave
-
-    def execute(self, behaviors: list[ArparmaBehavior] | None = None) -> Self:
-        if behaviors := (self.source.behaviors[1:] + (behaviors or [])):
-            exc_behaviors = []
-            for behavior in behaviors:
-                exc_behaviors.extend(requirement_handler(behavior))
-            for b in exc_behaviors:
-                b.before_operate(self)
-            for b in exc_behaviors:
-                try:
-                    b.operate(self)
-                except BehaveCancelled:
-                    continue
-                except OutBoundsBehave as e:
-                    return self.fail(e)
+        Args:
+            name (str): 命令节点名称
+            args (Arg | Args | None, optional): 命令节点参数
+            dest (str | None, optional): 命令节点目标名称
+            default (Any, optional): 命令节点默认值
+            action (Action | None, optional): 命令节点响应动作
+            separators (str | Sequence[str] | Set[str] | None, optional): 命令分隔符
+            help_text (str | None, optional): 命令帮助信息
+            requires (str | list[str] | tuple[str, ...] | set[str] | None, optional): 命令节点需求前缀
+        """
+        if not name:
+            raise InvalidParam(lang.require("common", "name_empty"))
+        _parts = name.split(" ")
+        self.name = _parts[-1]
+        self.requires = ([requires] if isinstance(requires, str) else list(requires)) if requires else []
+        self.requires.extend(_parts[:-1])
+        self.args = Args() + args
+        self.default = default
+        self.action = action or store
+        _handle_default(self)
+        self.separators = (' ',) if separators is None else (
+            (separators,) if isinstance(separators, str) else tuple(separators)
+        )
+        self.nargs = len(self.args.argument)
+        self.dest = (
+            dest or (("_".join(self.requires) + "_") if self.requires else "") + self.name.lstrip('-')
+        ).lstrip('-')
+        self.help_text = help_text or self.dest
+        self._hash = self._calc_hash()
+
+    nargs: int
+    _hash: int
+
+    def separate(self, *separator: str) -> Self:
+        """设置命令分隔符
+
+        Args:
+            *separator(str): 命令分隔符
+
+        Returns:
+            Self: 命令节点本身
+        """
+        self.separators = separator
+        self._hash = self._calc_hash()
         return self
 
-    def call(self, target: Callable[..., T], **additional):
-        if self.matched:
-            names = {p.name for p in get_signature(target)}
-            return target(**{k: v for k, v in {**self.all_matched_args, **additional}.items() if k in names})
-        raise RuntimeError
-
-    def fail(self, exc: type[BaseException] | BaseException | str):
-        return Arparma(self._source, self.origin, False, self.header_match, error_info=exc)
-
-    def __require__(self, parts: list[str]) -> tuple[dict[str, Any] | OptionResult | SubcommandResult | None, str]:
-        """如果能够返回, 除开基本信息, 一定返回该path所在的dict"""
-        if len(parts) == 1:
-            part = parts[0]
-            for src in (self.main_args, self.other_args, self.options, self.subcommands):
-                if part in src:
-                    return src, part
-            if part in {"options", "subcommands", "main_args", "other_args"}:
-                return getattr(self, part, {}), ''
-            return (self.all_matched_args, '') if part == "args" else (None, part)
-        prefix = parts.pop(0)  # parts[0]
-        if prefix in {"options", "subcommands"} and prefix in self.components:
-            raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=prefix))
-        if prefix == "options" or prefix in self.options:
-            return _handle_opt(prefix, parts, self.options)
-        if prefix == "subcommands" or prefix in self.subcommands:
-            return _handle_sub(prefix, parts, self.subcommands)
-        prefix = prefix.replace("$main", "main_args").replace("$other", "other_args")
-        if prefix in {"main_args", "other_args"}:
-            return getattr(self, prefix, {}), parts.pop(0)
-        return None, prefix
+    def __repr__(self):
+        data = {}
+        if not self.args.empty:
+            data["args"] = self.args
+        if self.default is not None:
+            data["default"] = self.default
+        return f"{self.__class__.__name__}({self.dest!r}, {', '.join(f'{k}={v!r}' for k, v in data.items())})"
+
+    def _calc_hash(self):
+        data = vars(self)
+        data.pop("_hash", None)
+        return hash(repr(data))
+
+    def __hash__(self):
+        return self._hash
+
+    def __eq__(self, other):
+        return self.__class__ == other.__class__ and self.__hash__() == other.__hash__()
+
+
+class Option(CommandNode):
+    """命令选项
+
+    相比命令节点, 命令选项可以设置别名, 优先级, 允许名称与后随参数之间无分隔符
+    """
+
+    default: OptionResult | None
+    """命令选项默认值"""
+    aliases: frozenset[str]
+    """命令选项别名"""
+    priority: int
+    """命令选项优先级"""
+    compact: bool
+    "是否允许名称与后随参数之间无分隔符"
+
+    def __init__(
+        self,
+        name: str, args: Arg | Args | None = None, alias: Iterable[str] | None = None,
+        dest: str | None = None, default: Any = None, action: Action | None = None,
+        separators: str | Sequence[str] | set[str] | None = None,
+        help_text: str | None = None,
+        requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
+        compact: bool = False, priority: int = 0,
+    ):
+        """初始化命令选项
+
+        Args:
+            name (str): 命令选项名称
+            args (Arg | Args | None, optional): 命令选项参数
+            alias (Iterable[str] | None, optional): 命令选项别名
+            dest (str | None, optional): 命令选项目标名称
+            default (Any, optional): 命令选项默认值
+            action (Action | None, optional): 命令选项响应动作
+            separators (str | Sequence[str] | Set[str] | None, optional): 命令分隔符
+            help_text (str | None, optional): 命令选项帮助信息
+            requires (str | list[str] | tuple[str, ...] | set[str] | None, optional): 命令选项需求前缀
+            compact (bool, optional): 是否允许名称与后随参数之间无分隔符
+            priority (int, optional): 命令选项优先级
+        """
+        aliases = list(alias or [])
+        _name = name.split(" ")[-1]
+        if "|" in _name:
+            _aliases = _name.split("|")
+            _aliases.sort(key=len, reverse=True)
+            name = name.replace(_name, _aliases[0])
+            _name = _aliases[0]
+            aliases.extend(_aliases[1:])
+        aliases.insert(0, _name)
+        self.aliases = frozenset(aliases)
+        self.priority = priority
+        self.compact = compact
+        default = (
+            None if default is None else
+            default if isinstance(default, OptionResult) else OptionResult(default)
+        )
+        super().__init__(name, args, dest, default, action, separators, help_text, requires)
+        if self.separators == ("",):
+            self.compact = True
+            self.separators = (" ",)
 
     @overload
-    def query(self, path: str) -> Mapping[str, Any] | Any | None:
+    def __add__(self, other: Option) -> Subcommand:
         ...
 
     @overload
-    def query(self, path: str, default: T) -> T | Mapping[str, Any] | Any:
+    def __add__(self, other: Args | Arg) -> Option:
         ...
 
-    def query(self, path: str, default: T | None = None) -> Any | Mapping[str, Any] | T | None:
-        """根据path查询值"""
-        source, endpoint = self.__require__(path.split('.'))
-        if source is None:
-            return default
-        if isinstance(source, (OptionResult, SubcommandResult)):
-            return getattr(source, endpoint, default) if endpoint else source
-        return source.get(endpoint, default) if endpoint else MappingProxyType(source)
+    def __add__(self, other: Option | Args | Arg) -> Self | Subcommand:
+        """连接命令选项与命令节点或命令选项, 生成子命令
 
-    @overload
-    def query_with(self, arg_type: type[T], path: str | None = None) -> T | None: ...
-    @overload
-    def query_with(self, arg_type: type[T], *, default: D) -> T | D: ...
-    @overload
-    def query_with(self, arg_type: type[T], path: str, default: D) -> T | D: ...
-    def query_with(self, arg_type: type[T], path: str | None = None, default: D | None = None) -> T | D | None:
-        """根据类型查询参数"""
-        if path:
-            return res if generic_isinstance(res := self.query(path, Empty), arg_type) else default
-        with suppress(IndexError):
-            return [v for v in self.all_matched_args.values() if generic_isinstance(v, arg_type)][0]
-        return default
-
-    def find(self, path: str) -> bool:
-        """查询路径是否存在"""
-        return self.query(path, Empty) != Empty
+        Args:
+            other (Option | Args | Arg): 命令节点或命令选项
 
-    @overload
-    def __getitem__(self, item: type[T]) -> T | None: ...
-    @overload
-    def __getitem__(self, item: str) -> Any:  ...
-    def __getitem__(self, item: str | type[T]) -> T | Any | None:
-        if isinstance(item, str):
-            return self.query(item)
-        if data := self.query_with(item):
-            return data
+        Returns:
+            Option | Subcommand: 如果other为命令选项, 则返回生成的子命令, 否则返回自己
 
-    def __getattr__(self, item: str):
-        return self.all_matched_args.get(item, self.query(item.replace('_', '.')))
+        Raises:
+            TypeError: 如果other不是命令选项或命令节点, 则抛出此异常
+        """
+        if isinstance(other, Option):
+            return Subcommand(
+                self.name, other, self.args, dest=self.dest,
+                separators=self.separators, help_text=self.help_text, requires=self.requires
+            )
+        if isinstance(other, (Arg, Args)):
+            self.args += other
+            self.nargs = len(self.args)
+            self._hash = self._calc_hash()
+            return self
+        raise TypeError(f"unsupported operand type(s) for +: 'Option' and '{other.__class__.__name__}'")
+
+    def __radd__(self, other: str):
+        """与字符串连接, 生成 `Alconna` 对象
+
+        Args:
+            other (str): 字符串
+
+        Returns:
+            Alconna: Alconna 对象
+
+        Raises:
+            TypeError: 如果other不是字符串, 则抛出此异常
+        """
+        if isinstance(other, str):
+            from .core import Alconna
+            return Alconna(other, self)
+        raise TypeError(f"unsupported operand type(s) for +: '{other.__class__.__name__}' and 'Option'")
 
-    def __repr__(self):
-        if self.error_info:
-            attrs = ((s, getattr(self, s, None)) for s in ("matched", "header_match", "error_data", "error_info"))
-            return ", ".join([f"{a}={v}" for a, v in attrs if v is not None])
-        else:
-            attrs = [(s, getattr(self, s, None)) for s in ("matched", "header_match", "options", "subcommands")]
-            margs = {k: v for k, v in self.main_args.items() if k not in ('$varargs', '$kwargs', '$kwonly')}
-            attrs.append(("main_args", margs))
-            other_args = {k: v for k, v in self.other_args.items() if k not in ('$varargs', '$kwargs', '$kwonly')}
-            attrs.append(("other_args", other_args))
-            return ", ".join([f"{a}={v}" for a, v in attrs if v])
 
+class Subcommand(CommandNode):
+    """子命令, 次于主命令
 
-@dataclass(init=True, unsafe_hash=True, repr=True)
-class ArparmaBehavior(metaclass=ABCMeta):
+    与命令节点不同, 子命令可以包含多个命令选项与相对于自己的子命令
     """
-    解析结果行为器的基类, 对应一个对解析结果的操作行为
-    """
-    record: dict[int, dict[str, tuple[Any, Any]]] = field(default_factory=dict, init=False, repr=False, hash=False)
-    requires: list[ArparmaBehavior] = field(init=False, hash=False, repr=False)
+    default: SubcommandResult | None
+    """子命令默认值"""
+    options: list[Option | Subcommand]
+    """子命令包含的选项与子命令"""
 
-    def before_operate(self, interface: Arparma):
-        if not self.record:
-            return
-        if not (_record := self.record.get(interface.token, None)):
-            return
-        for path, (past, current) in _record.items():
-            source, end = interface.__require__(path.split("."))
-            if source is None:
-                continue
-            if isinstance(source, dict):
-                if past != Empty:
-                    source[end] = past
-                elif source.get(end, Empty) != current:
-                    source.pop(end)
-            elif past != Empty:
-                setattr(source, end, past)
-            elif getattr(source, end, Empty) != current:
-                delattr(source, end)
-        _record.clear()
+    def __init__(
+        self,
+        name: str,
+        *args: Args | Arg | Option | Subcommand | list[Option | Subcommand],
+        dest: str | None = None, default: Any = None,
+        separators: str | Sequence[str] | set[str] | None = None,
+        help_text: str | None = None,
+        requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
+    ):
+        """初始化子命令
+
+        Args:
+            name (str): 子命令名称
+            *args (Args | Arg | Option | Subcommand | list[Option | Subcommand]): 参数, 选项或子命令
+            dest (str | None, optional): 子命令选项目标名称
+            default (Any, optional): 子命令默认值
+            action (Action | None, optional): 子命令选项响应动作
+            separators (str | Sequence[str] | Set[str] | None, optional): 子命令分隔符
+            help_text (str | None, optional): 子命令选项帮助信息
+            requires (str | list[str] | tuple[str, ...] | set[str] | None, optional): 子命令选项需求前缀
+        """
+        self.options = [i for i in args if isinstance(i, (Option, Subcommand))]
+        for li in filter(lambda x: isinstance(x, list), args):
+            self.options.extend(li)
+        default = (
+            None if default is None else
+            default if isinstance(default, SubcommandResult) else SubcommandResult(default)
+        )
+        super().__init__(
+            name,
+            reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
+            dest, default, None, separators, help_text, requires
+        )
+
+    def __add__(self, other: Option | Args | Arg | str) -> Self:
+        """连接子命令与命令选项或命令节点
+
+        Args:
+            other (Option | Args | Arg | str): 命令选项或命令节点
+
+        Returns:
+            Self: 返回子命令自身
+
+        Raises:
+            TypeError: 如果other不是命令选项或命令节点, 则抛出此异常
+        """
+        if isinstance(other, (Option, str)):
+            self.options.append(Option(other) if isinstance(other, str) else other)
+            self._hash = self._calc_hash()
+            return self
+        if isinstance(other, (Arg, Args)):
+            self.args += other
+            self.nargs = len(self.args)
+            self._hash = self._calc_hash()
+            return self
+        raise TypeError(f"unsupported operand type(s) for +: 'Subcommand' and '{other.__class__.__name__}'")
+
+    def __radd__(self, other: str):
+        """与字符串连接, 生成 `Alconna` 对象
+
+        Args:
+            other (str): 字符串
+
+        Returns:
+            Alconna: Alconna 对象
+
+        Raises:
+            TypeError: 如果other不是字符串, 则抛出此异常
+        """
+        if isinstance(other, str):
+            from .core import Alconna
+            return Alconna(other, self)
+        raise TypeError(f"unsupported operand type(s) for +: '{other.__class__.__name__}' and 'Subcommand'")
+
+    def add(self, opt: Option | Subcommand) -> Self:
+        """添加选项或子命令
+
+        Args:
+            opt (Option | Subcommand): 选项或子命令
+
+        Returns:
+            Self: 返回子命令自身
+        """
+        self.options.append(opt)
+        self._hash = self._calc_hash()
+        return self
 
-    @abstractmethod
-    def operate(self, interface: Arparma):
-        ...
 
-    def update(self, interface: Arparma, path: str, value: Any):
-        def _update(tkn, src, pth, ep, val):
-            _record = self.record.setdefault(tkn, {})
-            if isinstance(src, dict):
-                _record[pth] = (src.get(ep, Empty), val)
-                src[ep] = val
-            else:
-                _record[pth] = (getattr(src, ep, Empty), val)
-                setattr(src, ep, val)
-
-        source, end = interface.__require__(path.split("."))
-        if source is None:
-            return
-        if end:
-            _update(interface.token, source, path, end, value)
-        elif isinstance(value, dict):
-            for k, v in value.items():
-                _update(interface.token, source, f"{path}.{k}", k, v)
-
-
-@lru_cache(4096)
-def requirement_handler(behavior: ArparmaBehavior) -> list[ArparmaBehavior]:
-    res = []
-    for b in getattr(behavior, 'requires', []):
-        res.extend(requirement_handler(b))
-    res.append(behavior)
-    return res
+__all__ = ["CommandNode", "Option", "Subcommand"]
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/core.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,61 @@
 """Alconna 主体"""
 from __future__ import annotations
 
 import sys
-from dataclasses import InitVar, dataclass, field
-from functools import reduce, partial
+from dataclasses import dataclass, field
+from functools import partial, reduce
+from pathlib import Path
 from typing import Any, Callable, Generic, Sequence, TypeVar, overload
 
 from tarina import init_spec, lang
 from typing_extensions import Self
 
-from .action import ArgAction, exec_, exec_args
-from .analyser import TCompile, Analyser
+from ._internal._analyser import Analyser, TCompile
 from .args import Arg, Args
 from .arparma import Arparma, ArparmaBehavior
 from .base import Option, Subcommand
 from .config import Namespace, config
 from .duplication import Duplication
-from .exceptions import NullMessage, ExecuteFailed
+from .exceptions import ExecuteFailed, NullMessage
 from .formatter import TextFormatter
 from .manager import ShortcutArgs, command_manager
-from .typing import TDC, TPrefixes
+from .typing import TDC, TPrefixes, DataCollection, CommandMeta
 
 T_Duplication = TypeVar('T_Duplication', bound=Duplication)
 T = TypeVar("T")
+TDC1 = TypeVar("TDC1", bound=DataCollection[Any])
 
 
 @dataclass(init=True, unsafe_hash=True)
 class ArparmaExecutor(Generic[T]):
+    """Arparma 执行器
+
+    Attributes:
+        target(Callable[..., T]): 目标函数
+    """
     target: Callable[..., T]
     binding: Callable[..., list[Arparma]] = field(default=lambda: [], repr=False)
 
     __call__ = lambda self, *args, **kwargs: self.target(*args, **kwargs)
 
     @property
     def result(self) -> T:
+        """执行结果"""
         if not self.binding:
             raise ExecuteFailed(None)
         arps = self.binding()
         if not arps or not arps[0].matched:
             raise ExecuteFailed("Unmatched")
         try:
             return arps[0].call(self.target)
         except Exception as e:
             raise ExecuteFailed(e) from e
 
 
-@dataclass
-class ActionHandler(ArparmaBehavior):
-    source: InitVar[Alconna]
-    main_action: ArgAction | None = field(init=False, default=None)
-    options: dict[str, ArgAction] = field(init=False, default_factory=dict)
-
-    def _step(self, src, prefix=None):
-        for opt in src.options:
-            if opt.action:
-                self.options[(f"{prefix}." if prefix else "") + opt.dest] = opt.action
-            if hasattr(opt, "options"):
-                self._step(opt, (f"{prefix}." if prefix else "") + opt.dest)
-
-    def __post_init__(self, source: Alconna):
-        self.main_action = source.action
-        self._step(source)
-
-    def operate(self, interface: Arparma):
-        self.before_operate(interface)
-        source = interface.source
-        if action := self.main_action:
-            self.update(interface, "main_args", exec_args(interface.main_args, action, source.meta.raise_exception))
-        for path, action in self.options.items():
-            if d := interface.query(path, None):
-                end, value = exec_(d, action, source.meta.raise_exception)  # type: ignore
-                self.update(interface, f"{path}.{end}", value)  # type: ignore
-
-
-@dataclass(unsafe_hash=True)
-class CommandMeta:
-    description: str = field(default="Unknown")
-    usage: str | None = field(default=None)
-    example: str | None = field(default=None)
-    author: str | None = field(default=None)
-    fuzzy_match: bool = field(default=False)
-    raise_exception: bool = field(default=False)
-    hide: bool = field(default=False)
-    keep_crlf: bool = field(default=False)
-
-
 class Alconna(Subcommand, Generic[TDC]):
     """
     更加精确的命令解析
 
     Examples:
 
         >>> from arclet.alconna import Alconna
@@ -102,115 +69,116 @@
         ...         Args["sub_main_args", "sub_main_args"]
         ...     ),
         ...     Args["main_args", "main_args"],
         ...  )
         >>> alc.parse("name opt opt_arg")
     """
     prefixes: TPrefixes
+    """命令前缀"""
     command: str | Any
-    analyser_type: type[Analyser]
+    """命令名"""
     formatter: TextFormatter
+    """文本格式化器"""
     namespace: str
+    """命名空间"""
     meta: CommandMeta
+    """命令元数据"""
     behaviors: list[ArparmaBehavior]
-
-    global_analyser_type: type[Analyser] = Analyser
+    """命令行为器"""
 
     @property
     def compile(self) -> Callable[[TCompile | None], Analyser[TDC]]:
-        return partial(self.analyser_type, self)
-
-    @classmethod
-    def default_analyser(cls, __t: type[Analyser] | None = None):
-        """配置 Alconna 的默认解析器"""
-        if __t is not None:
-            cls.global_analyser_type = __t
-        return cls
+        """编译 `Alconna` 为对应的解析器"""
+        return partial(Analyser, self)
 
     def __init__(
         self,
         *args: Option | Subcommand | str | TPrefixes | Any | Args | Arg,
-        action: ArgAction | Callable | None = None,
         meta: CommandMeta | None = None,
         namespace: str | Namespace | None = None,
         separators: str | set[str] | Sequence[str] | None = None,
-        analyser_type: type[Analyser] | None = None,
         behaviors: list[ArparmaBehavior] | None = None,
         formatter_type: type[TextFormatter] | None = None
     ):
         """
-        以标准形式构造 Alconna
+        以标准形式构造 `Alconna`
 
         Args:
-            args: 命令选项、主参数、命令名称或命令头
-            action: 命令解析后针对主参数的回调函数
-            meta: 命令元信息
-            namespace: 命令命名空间, 默认为 'Alconna'
-            separators: 命令参数分隔符, 默认为空格
-            analyser_type: 命令解析器类型, 默认为 DisorderCommandAnalyser
-            behaviors: 命令解析行为，默认为 None
-            formatter_type: 命令帮助文本格式器类型, 默认为 DefaultHelpTextFormatter
+            *args (Option | Subcommand | str | TPrefixes | Any | Args | Arg): 命令选项、主参数、命令名称或命令头
+            action (ArgAction | Callable | None, optional): 命令解析后针对主参数的回调函数
+            meta (CommandMeta | None, optional): 命令元信息
+            namespace (str | Namespace | None, optional): 命令命名空间, 默认为 'Alconna'
+            separators (str | set[str] | Sequence[str] | None, optional): 命令参数分隔符, 默认为 `' '`
+            behaviors (list[ArparmaBehavior] | None, optional): 命令解析行为器
+            formatter_type (type[TextFormatter] | None, optional): 指定的命令帮助文本格式器类型
         """
         if not namespace:
-            np_config = config.default_namespace
+            ns_config = config.default_namespace
         elif isinstance(namespace, Namespace):
-            np_config = config.namespaces.setdefault(namespace.name, namespace)
+            ns_config = config.namespaces.setdefault(namespace.name, namespace)
         else:
-            np_config = config.namespaces.setdefault(namespace, Namespace(namespace))
-        self.prefixes = next(filter(lambda x: isinstance(x, list), args + (np_config.prefixes.copy(),)))  # type: ignore
+            ns_config = config.namespaces.setdefault(namespace, Namespace(namespace))
+        self.prefixes = next(filter(lambda x: isinstance(x, list), args + (ns_config.prefixes.copy(),)))  # type: ignore
         try:
             self.command = next(filter(lambda x: not isinstance(x, (list, Option, Subcommand, Args, Arg)), args))
         except StopIteration:
-            self.command = "" if self.prefixes else sys.argv[0]
-        self.namespace = np_config.name
-        self.analyser_type = analyser_type or self.__class__.global_analyser_type  # type: ignore
-        self.formatter = (formatter_type or np_config.formatter_type or TextFormatter)()
+            if self.prefixes:
+                self.command = ""
+            else:
+                path = Path(sys.argv[0])
+                self.command = path.parent.stem if str(path.parent) not in (".", "/", "\\") else path.stem
+        self.namespace = ns_config.name
+        self.formatter = (formatter_type or ns_config.formatter_type or TextFormatter)()
         self.meta = meta or CommandMeta()
-        self.meta.fuzzy_match = self.meta.fuzzy_match or np_config.fuzzy_match
-        self.meta.raise_exception = self.meta.raise_exception or np_config.raise_exception
+        self.meta.fuzzy_match = self.meta.fuzzy_match or ns_config.fuzzy_match
+        self.meta.raise_exception = self.meta.raise_exception or ns_config.raise_exception
+        self.meta.compact = self.meta.compact or ns_config.compact
         options = [i for i in args if isinstance(i, (Option, Subcommand))]
         options.append(
-            Option("|".join(np_config.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
+            Option("|".join(ns_config.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
         )
         options.append(
             Option(
-                "|".join(np_config.builtin_option_name['shortcut']),
+                "|".join(ns_config.builtin_option_name['shortcut']),
                 Args["delete;?", "delete"]["name", str]["command", str, "_"],
                 help_text=lang.require("builtin", "option_shortcut")
             )
         )
         options.append(
             Option(
-                "|".join(np_config.builtin_option_name['completion']),
+                "|".join(ns_config.builtin_option_name['completion']),
                 help_text=lang.require("builtin", "option_completion")
             )
         )
         name = f"{self.command or self.prefixes[0]}".replace(command_manager.sign, "")  # type: ignore
         self.path = f"{self.namespace}::{name}"
         super().__init__(
             "ALCONNA::",
             reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
             *options,
             dest=name,
-            action=action,
-            separators=separators or np_config.separators,
+            separators=separators or ns_config.separators,
         )
         self.name = name
         self.behaviors = behaviors or []
-        self.behaviors.insert(0, ActionHandler(self))
         command_manager.register(self)
         self._executors: list[ArparmaExecutor] = []
         self.union = set()
 
     @property
     def namespace_config(self) -> Namespace:
         return config.namespaces[self.namespace]
 
     def reset_namespace(self, namespace: Namespace | str, header: bool = True) -> Self:
-        """重新设置命名空间"""
+        """重新设置命名空间
+
+        Args:
+            namespace (Namespace | str): 命名空间
+            header (bool, optional): 是否保留命令头, 默认为 `True`
+        """
         command_manager.delete(self)
         if isinstance(namespace, str):
             namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
         self.namespace = namespace.name
         self.path = f"{self.namespace}::{self.name}"
         if header:
             self.prefixes = namespace.prefixes.copy()
@@ -229,24 +197,40 @@
         self.meta.fuzzy_match = namespace.fuzzy_match or self.meta.fuzzy_match
         self.meta.raise_exception = namespace.raise_exception or self.meta.raise_exception
         self._hash = self._calc_hash()
         command_manager.register(self)
         return self
 
     def reset_behaviors(self, behaviors: list[ArparmaBehavior]) -> Self:
-        """重新设置解析行为器"""
+        """重新设置解析行为器
+
+        Args:
+            behaviors (list[ArparmaBehavior]): 解析行为器
+        """
         self.behaviors[1:] = behaviors
         return self
 
     def get_help(self) -> str:
         """返回该命令的帮助信息"""
         return self.formatter.format_node()
 
     def shortcut(self, key: str, args: ShortcutArgs[TDC] | None = None, delete: bool = False):
-        """添加快捷命令"""
+        """操作快捷命令
+
+        Args:
+            key (str): 快捷命令名
+            args (ShortcutArgs[TDC] | None, optional): 快捷命令参数, 不传入时则尝试使用最近一次使用的命令
+            delete (bool, optional): 是否删除快捷命令, 默认为 `False`
+
+        Returns:
+            str: 操作结果
+
+        Raises:
+            ValueError: 快捷命令操作失败时抛出
+        """
         try:
             if delete:
                 command_manager.delete_shortcut(self, key)
                 return lang.require("shortcut", "delete_success").format(shortcut=key, target=self.path)
             if args:
                 command_manager.add_shortcut(self, key, args)
                 return lang.require("shortcut", "add_success").format(shortcut=key, target=self.path)
@@ -266,27 +250,36 @@
                 raise e
             return str(e)
 
     def __repr__(self):
         return f"{self.namespace}::{self.name}(args={self.args}, options={self.options})"
 
     def add(self, opt: Option | Subcommand) -> Self:
+        """添加选项或子命令
+
+        Args:
+            opt (Option | Subcommand): 选项或子命令
+
+        Returns:
+            Self: 命令本身
+        """
         command_manager.delete(self)
         self.options.insert(-3, opt)
-        self.behaviors[0] = ActionHandler(self)
         self._hash = self._calc_hash()
         command_manager.register(self)
         return self
 
     @init_spec(Option, True)
     def option(self, opt: Option) -> Self:
+        """添加选项"""
         return self.add(opt)
 
     @init_spec(Subcommand, True)
     def subcommand(self, sub: Subcommand) -> Self:
+        """添加子命令"""
         return self.add(sub)
 
     def _parse(self, message: TDC) -> Arparma[TDC]:
         if self.union:
             for ana, argv in command_manager.requires(*self.union):
                 if (res := ana.process(argv.build(message))).matched:
                     return res
@@ -302,30 +295,43 @@
     @overload
     def parse(self, message, *, duplication: type[T_Duplication]) -> T_Duplication:
         ...
 
     def parse(
         self, message: TDC, *, duplication: type[T_Duplication] | None = None
     ) -> Arparma[TDC] | T_Duplication:
-        """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类"""
+        """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类
+        
+        Args:
+            message (TDC): 命令消息
+            duplication (type[T_Duplication], optional): 指定的`副本`类型
+        Returns:
+            Arparma[TDC] | T_Duplication: 若`duplication`参数为`None`则返回`Arparma`对象, 否则返回`duplication`类型的对象
+        Raises:
+            NullMessage: 传入的消息为空时抛出
+        """
         try:
             arp = self._parse(message)
         except NullMessage as e:
             if self.meta.raise_exception:
                 raise e
             return Arparma(self.path, message, False, error_info=e)
         if arp.matched:
-            self.behaviors[0].operate(arp)
             arp = arp.execute()
             if self._executors:
                 for ext in self._executors:
                     arp.call(ext.target)
         return duplication(arp) if duplication else arp
 
     def bind(self, active: bool = True):
+        """绑定命令执行器
+
+        Args:
+            active (bool, optional): 该执行器是否由 `Alconna` 主动调用, 默认为 `True`
+        """
         def wrapper(target: Callable[..., T]) -> ArparmaExecutor[T]:
             ext = ArparmaExecutor(target, lambda: command_manager.get_result(self))
             if active:
                 self._executors.append(ext)
             return ext
         return wrapper
 
@@ -341,24 +347,33 @@
         elif isinstance(other, Option):
             self.options.append(other)
         elif isinstance(other, Args):
             self.args += other
             self.nargs = len(self.args)
         elif isinstance(other, str):
             self.options.append(Option(other))
-        self.behaviors[0] = ActionHandler(self)
         self._hash = self._calc_hash()
         command_manager.register(self)
         return self
 
     def __or__(self, other: Alconna) -> Self:
         self.union.add(other.path)
         return self
 
     def _calc_hash(self):
         return hash((self.path + str(self.prefixes), self.meta, *self.options, *self.args))
 
     def __call__(self, *args, **kwargs):
-        return self.parse(list(args)) if args else self.parse(sys.argv[1:])
+        if args:
+            return self.parse(list(args))  # type: ignore
+        path = Path(sys.argv[0])
+        head = path.parent.stem if str(path.parent) not in (".", "/", "\\") else path.stem
+        if head != self.command:
+            return self.parse(sys.argv[1:])  # type: ignore
+        return self.parse([head, *sys.argv[1:]])  # type: ignore
+
+    @property
+    def headers(self):
+        return self.prefixes
 
 
-__all__ = ["Alconna", "CommandMeta"]
+__all__ = ["Alconna", "ArparmaExecutor"]
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/duplication.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,42 +5,44 @@
 from tarina import Empty
 
 from .arparma import Arparma
 from .stub import ArgsStub, BaseStub, OptionStub, SubcommandStub
 
 
 class Duplication:
-    """用以更方便的检查、调用解析结果的类。"""
+    """`副本`, 用以更方便的检查、调用解析结果的类。"""
     header: dict[str, str]
 
     def __init__(self, target: Arparma):
         from .base import Option, Subcommand
         self.header = target.header.copy()
         for key, value in self.__annotations__.items():
             if isclass(value) and issubclass(value, BaseStub):
-                if value == ArgsStub:
+                if value is ArgsStub:
                     setattr(self, key, ArgsStub(target.source.args).set_result(target.main_args))
-                elif value == SubcommandStub:
+                elif value is SubcommandStub:
                     for subcommand in filter(lambda x: isinstance(x, Subcommand), target.source.options):
                         if subcommand.dest == key:
                             setattr(self, key, SubcommandStub(subcommand).set_result(target.subcommands.get(key, None)))
-                elif value == OptionStub:
+                elif value is OptionStub:
                     for option in filter(lambda x: isinstance(x, Option), target.source.options):
                         if option.dest == key:
                             setattr(self, key, OptionStub(option).set_result(target.options.get(key, None)))
             elif key != 'header':
                 setattr(self, key, target.all_matched_args.get(key, Empty))
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.__annotations__})'
 
     def option(self, name: str) -> OptionStub | None:
+        """获取指定名称的选项存根。"""
         return cast(OptionStub, getattr(self, name, None))
 
     def subcommand(self, name: str) -> SubcommandStub | None:
+        """获取指定名称的子命令存根。"""
         return cast(SubcommandStub, getattr(self, name, None))
 
 
 def generate_duplication(arp: Arparma) -> Duplication:
     """依据给定的命令生成一个解析结果的检查类。"""
     from .base import Option, Subcommand
     options = filter(lambda x: isinstance(x, Option), arp.source.options)
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,7 +43,11 @@
 
 class PauseTriggered(Exception):
     """解析状态保存触发"""
 
 
 class SpecialOptionTriggered(Exception):
     """内置选项解析触发"""
+
+
+class TerminateLoop(Exception):
+    """终止循环"""
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/handlers.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Iterable
-from tarina import Empty, split_once, lang
-from nepattern import AllParam, BasePattern
+from tarina import Empty, lang
+from nepattern import AllParam, BasePattern, AnyOne, AnyString
 from nepattern.util import TPattern
 
-from .args import Arg, Args
-from .header import Double, Header
-from .base import Option, Subcommand
-from .config import config
-from .completion import Prompt, comp_ctx
-from .exceptions import ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, SpecialOptionTriggered, PauseTriggered
-from .model import OptionResult, Sentence, HeadResult
-from .output import output_manager
-from .typing import KeyWordVar, MultiVar
-from .util import levenshtein_norm
+from ._header import Double, Header
+from ..action import Action
+from ..args import Arg, Args, STRING
+from ..base import Option, Subcommand
+from ..config import config
+from ..completion import Prompt, comp_ctx
+from ..exceptions import (
+    ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, SpecialOptionTriggered, PauseTriggered, TerminateLoop
+)
+from ..model import OptionResult, Sentence, HeadResult
+from ..output import output_manager
+from ..typing import KeyWordVar, MultiVar
+from ._util import levenshtein
 
 if TYPE_CHECKING:
-    from .argv import Argv
-    from .analyser import SubAnalyser, Analyser
+    from ._argv import Argv
+    from ._analyser import SubAnalyser, Analyser
 
 
 def _handle_keyword(
     argv: Argv,
     value: KeyWordVar,
     may_arg: Any,
     seps: tuple[str, ...],
     result_dict: dict[str, Any],
     default_val: Any,
     optional: bool,
     key: str | None = None,
     fuzzy: bool = False,
 ):
+    """处理关键字参数
+
+    Args:
+        argv (Argv): 命令行参数
+        value (KeyWordVar): 关键字参数
+        may_arg (Any): 可能的参数
+        seps (tuple[str, ...]): 分隔符
+        result_dict (dict[str, Any]): 结果字典
+        default_val (Any): 默认值
+        optional (bool): 是否可选
+        key (str | None, optional): 关键字. Defaults to None.
+        fuzzy (bool, optional): 是否模糊匹配. Defaults to False.
+    """
     if _kwarg := re.match(fr'^([^{value.sep}]+){value.sep}(.*?)$', may_arg):
         key = key or _kwarg[1]
         if (_key := _kwarg[1]) != key:
             argv.rollback(may_arg)
-            if fuzzy and levenshtein_norm(_key, key) >= config.fuzzy_threshold:
+            if fuzzy and levenshtein(_key, key) >= config.fuzzy_threshold:
                 raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_key, target=key))
             if default_val is None:
                 raise ParamsUnmatched(lang.require("fuzzy", "matched").format(source=_key, target=key))
             result_dict[_key] = None if default_val is Empty else default_val
             return
         if not (_m_arg := _kwarg[2]):
             _m_arg, _ = argv.next(seps)
@@ -61,14 +77,15 @@
 def _loop_kw(
     argv: Argv,
     _loop: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any
 ):
+    """循环关键字参数"""
     result = {}
     for _ in range(_loop):
         _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
         if _m_str and _m_arg in argv.param_ids:
             argv.rollback(_m_arg)
@@ -88,14 +105,15 @@
     argv: Argv,
     _loop: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any,
     args: Args
 ):
+    """循环参数"""
     kw = args[args.var_keyword].value.base if args.var_keyword else None
     result = []
     for _ in range(_loop):
         _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
         if _m_str and (
@@ -117,18 +135,26 @@
 
 def multi_arg_handler(
     argv: Argv,
     args: Args,
     arg: Arg,
     result_dict: dict[str, Any],
 ):
+    """处理可变参数
+
+    Args:
+        argv (Argv): 命令行参数
+        args (Args): 参数集合
+        arg (Arg): 参数单元
+        result_dict (dict[str, Any]): 结果字典
+    """
     seps = arg.separators
     value = arg.value
     key = arg.name
-    default = arg.field.default_gen
+    default = arg.field.default
     kw = value.base.__class__ == KeyWordVar
     _m_rest_arg = len(args) - len(result_dict)
     _m_rest_all_param_count = len(argv.release(seps))
     if not kw and not args.var_keyword or kw and not args.var_positional:
         loop = _m_rest_all_param_count - _m_rest_arg + 1
     elif not kw:
         loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_keyword].value.flag == "*"))
@@ -136,275 +162,383 @@
         loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_positional].value.flag == "*"))
     if value.length > 0:
         loop = min(loop, value.length)
     result_dict[key] = (
         _loop_kw(argv, loop, seps, value, default) if kw
         else _loop(argv, loop, seps, value, default, args)
     )
+    if kw:
+        kwargs = result_dict[key]
+        if not isinstance(kwargs, dict):
+            kwargs = {key: kwargs}
+        result_dict[key] = kwargs
+    else:
+        varargs = result_dict[key]
+        if not isinstance(varargs, Iterable):
+            varargs = (varargs, )
+        elif not isinstance(varargs, tuple):
+            varargs = tuple(varargs)
+        result_dict[key] = varargs
 
 
 def analyse_args(argv: Argv, args: Args) -> dict[str, Any]:
     """
-    分析 Args 部分
+    分析 `Args` 部分
 
     Args:
-        argv: 使用的分析器
-        args: 目标Args
+        argv (Argv): 命令行参数
+        args (Args): 目标 `Args`
 
     Returns:
-        Dict: 解析结果
+        dict[str, Any]: 解析结果
     """
     result: dict[str, Any] = {}
     for arg in args.argument:
         argv.context = arg
         key = arg.name
         value = arg.value
-        default_val = arg.field.default_gen
+        default_val = arg.field.default
         may_arg, _str = argv.next(arg.separators)
-        if _str and may_arg in argv.special:
-            raise SpecialOptionTriggered(argv.special[may_arg])
+        if _str and may_arg in argv.completion_names:
+            raise SpecialOptionTriggered("completion")
         if not may_arg or (_str and may_arg in argv.param_ids):
             argv.rollback(may_arg)
             if default_val is not None:
                 result[key] = None if default_val is Empty else default_val
             elif value.__class__ is MultiVar and value.flag == '*':
                 result[key] = ()
             elif not arg.optional:
                 raise ArgumentMissing(lang.require("args", "missing").format(key=key))
             continue
         if value.__class__ is MultiVar:
             argv.rollback(may_arg)
             multi_arg_handler(argv, args, arg, result)  # type: ignore
         elif value.__class__ is KeyWordVar:
             _handle_keyword(
-                argv, value, may_arg, arg.separators, result, default_val, arg.optional, key, argv.fuzzy_match  # type: ignore
+                argv, value, may_arg, arg.separators,  # type: ignore
+                result, default_val, arg.optional, key, argv.fuzzy_match  # type: ignore
             )
-        elif value is AllParam:
+        elif value == AllParam:
             argv.rollback(may_arg)
             result[key] = argv.converter(argv.release(arg.separators))
             argv.current_index = argv.ndata
             return result
+        elif value == AnyOne:
+            result[key] = may_arg
+        elif value == AnyString:
+            result[key] = str(may_arg)
+        elif value == STRING and _str:
+            result[key] = may_arg
         else:
             res = (
                 value.invalidate(may_arg, default_val)
                 if value.anti
                 else value.validate(may_arg, default_val)
             )
             if res.flag != 'valid':
                 argv.rollback(may_arg)
             if res.flag == 'error':
                 if arg.optional:
                     continue
                 raise ParamsUnmatched(*res.error.args)
             if not arg.anonymous:
                 result[key] = res._value  # type: ignore
-    if args.var_keyword:
-        kwargs = result[args.var_keyword]
-        if not isinstance(kwargs, dict):
-            kwargs = {args.var_keyword: kwargs}
-        result['$kwargs'] = (kwargs, args.var_keyword)
-    if args.var_positional:
-        varargs = result[args.var_positional]
-        if not isinstance(varargs, Iterable):
-            varargs = [varargs]
-        elif not isinstance(varargs, list):
-            varargs = list(varargs)
-        result['$varargs'] = (varargs, args.var_positional)
-    if args.keyword_only:
-        result['$kwonly'] = {k: v for k, v in result.items() if k in args.keyword_only}
     argv.context = None
     return result
 
 
-def analyse_unmatch_params(analyser: SubAnalyser, argv: Argv, text: str):
-    for _p in analyser.compile_params.values():
-        if isinstance(_p, list):
-            res = []
-            for _o in _p:
-                _may_param, _ = split_once(text, _o.separators)
-                if _may_param in _o.aliases or any(map(_may_param.startswith, _o.aliases)):
-                    analyser.compile_params.setdefault(text, res)
-                    res.append(_o)
-                    continue
-                if argv.fuzzy_match and levenshtein_norm(_may_param, _o.name) >= config.fuzzy_threshold:
-                    raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_o.name))
-            if res:
-                return res
-        elif isinstance(_p, Option):
-            _may_param, _ = split_once(text, _p.separators)
-            if _may_param in _p.aliases or any(map(_may_param.startswith, _p.aliases)):
-                analyser.compile_params.setdefault(text, _p)
-                return _p
-            if argv.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_p.name))
-        elif isinstance(_p, Sentence):
-            if (_may_param := split_once(text, _p.separators)[0]) == _p.name:
-                analyser.compile_params.setdefault(text, _p)
-                return _p
-            if argv.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_p.name))
-        else:
-            _may_param, _ = split_once(text, _p.command.separators)
-            if _may_param == _p.command.name or _may_param.startswith(_p.command.name):
-                analyser.compile_params.setdefault(text, _p)
-                return _p
-            if argv.fuzzy_match and levenshtein_norm(_may_param, _p.command.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_p.command.name))
-
-
-def analyse_option(analyser: SubAnalyser, argv: Argv, param: Option) -> tuple[str, OptionResult]:
+def handle_option(argv: Argv, opt: Option) -> tuple[str, OptionResult]:
     """
-    分析 Option 部分
+    处理 `Option` 部分
 
     Args:
-        analyser: 使用的分析器
-        argv: 使用的分析器
-        param: 目标Option
-    """
-    argv.context = param
-    if param.requires and analyser.sentences != param.requires:
-        raise ParamsUnmatched(f"{param.name}'s required is not '{' '.join(analyser.sentences)}'")
-    analyser.sentences = []
-    if param.is_compact:
-        name, _ = argv.next()
-        for al in param.aliases:
+        argv (Argv): 命令行参数
+        opt (Option): 目标 `Option`
+    """
+    argv.context = opt
+    _cnt = 0
+    error = True
+    name, _ = argv.next(opt.separators)
+    if opt.compact:
+        for al in opt.aliases:
             if mat := re.fullmatch(f"{al}(?P<rest>.*?)", name):
                 argv.rollback(mat.groupdict()['rest'], replace=True)
+                error = False
                 break
-        else:
-            raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
+    elif opt.action.type == 2:
+        for al in opt.aliases:
+            if name.startswith(al) and (cnt := (len(name.lstrip("-")) / len(al.lstrip("-")))).is_integer():
+                _cnt = int(cnt)
+                error = False
+                break
+    elif name in opt.aliases:
+        error = False
+    if error:
+        if argv.fuzzy_match and levenshtein(name, opt.name) >= config.fuzzy_threshold:
+            raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=name, target=opt.name))
+        raise ParamsUnmatched(lang.require("option", "name_error").format(source=opt.name, target=name))
+    name = opt.dest
+    return (
+        (name, OptionResult(None, analyse_args(argv, opt.args)))
+        if opt.nargs
+        else (name, OptionResult(_cnt or opt.action.value))
+    )
+
+
+def handle_action(param: Option, source: OptionResult, target: OptionResult):
+    """处理 `Option` 的 `action`"""
+    if param.action.type == 0:
+        return target
+    if param.action.type == 2:
+        if not param.nargs:
+            source.value += target.value
+            return source
+        return target
+    if not param.nargs:
+        source.value.extend(target.value)
     else:
-        name, _ = argv.next(param.separators)
-        if name not in param.aliases:  # 先匹配选项名称
-            raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
-    name = param.dest
-    if param.nargs == 0:
-        return name, OptionResult()
-    return name, OptionResult(None, analyse_args(argv, param.args))
+        for key, value in target.args.items():
+            if key in source.args:
+                source.args[key].append(value)
+            else:
+                source.args[key] = [value]
+    return source
+
+
+def analyse_option(analyser: SubAnalyser, argv: Argv, opt: Option):
+    """
+    分析 `Option` 部分
+
+    Args:
+        analyser (SubAnalyser): 当前解析器
+        argv (Argv): 命令行参数
+        opt (Option): 目标 `Option`
+    """
+    opt_n, opt_v = handle_option(argv, opt)
+    if opt_n not in analyser.options_result:
+        analyser.options_result[opt_n] = opt_v
+        if opt.action.type == 1 and opt_v.args:
+            for key in list(opt_v.args.keys()):
+                opt_v.args[key] = [opt_v.args[key]]
+    else:
+        analyser.options_result[opt_n] = handle_action(opt, analyser.options_result[opt_n], opt_v)
+
+
+def analyse_compact_params(analyser: SubAnalyser, argv: Argv):
+    """分析紧凑参数
+
+    Args:
+        analyser (SubAnalyser): 当前解析器
+        argv (Argv): 命令行参数
+    """
+    for param in analyser.compact_params:
+        _data, _index = argv.data_set()
+        try:
+            if param.__class__ is Option:
+                if param.requires and analyser.sentences != param.requires:
+                    return lang.require("option", "require_error").format(
+                        source=param.name, target=' '.join(analyser.sentences)
+                    )
+                analyse_option(analyser, argv, param)
+            else:
+                if param.command.requires and analyser.sentences != param.command.requires:
+                    return lang.require("subcommand", "require_error").format(
+                        source=param.command.name, target=' '.join(analyser.sentences)
+                    )
+                analyser.subcommands_result[param.command.dest] = param.process(argv).result()
+            _data.clear()
+            return True
+        except ParamsUnmatched as e:
+            if argv.context.__class__ is Arg:
+                raise e
+            argv.data_reset(_data, _index)
+
+
+def handle_opt_default(defaults: dict[str, tuple[OptionResult, Action]], data: dict[str, OptionResult]):
+    for k, v in defaults.items():
+        if k not in data:
+            data[k] = v[0]
+        if not v[0].args:
+            continue
+        for key, value in v[0].args.items():
+            data[k].args.setdefault(key, [value] if v[1].value == 1 else value)
 
 
 def analyse_param(analyser: SubAnalyser, argv: Argv, seps: tuple[str, ...] | None = None):
+    """处理参数
+
+    Args:
+        analyser (SubAnalyser): 当前解析器
+        argv (Argv): 命令行参数
+        seps (tuple[str, ...], optional): 指定的分隔符.
+    """
     _text, _str = argv.next(seps, move=False)
     if _str and _text in argv.special:
         if _text in argv.completion_names:
             if argv.current_index < argv.ndata:
                 argv.bak_data = argv.bak_data[:argv.current_index+1]
             last = argv.bak_data[-1]
             argv.bak_data[-1] = last[:last.rfind(_text)]
         raise SpecialOptionTriggered(argv.special[_text])
     if not _str or not _text:
         _param = None
     elif _text in analyser.compile_params:
         _param = analyser.compile_params[_text]
+    elif analyser.compact_params and (res := analyse_compact_params(analyser, argv)):
+        if res.__class__ is str:
+            raise ParamsUnmatched(res)
+        argv.context = None
+        return
     else:
-        _param = None if analyser.default_separate else analyse_unmatch_params(analyser, argv, _text)
-    if not _param and not analyser.args_result:
+        _param = None
+    if not _param and analyser.command.nargs and not analyser.args_result:
         analyser.args_result = analyse_args(argv, analyser.self_args)
-    elif _param.__class__ is Option:
-        opt_n, opt_v = analyse_option(analyser, argv, _param)
-        analyser.options_result[opt_n] = opt_v
+        if analyser.args_result:
+            argv.context = None
+            return
+    if _param.__class__ is Sentence:
+        analyser.sentences.append(argv.next()[0])
+        return
+    if _param.__class__ is Option:
+        if _param.requires and analyser.sentences != _param.requires:
+            raise ParamsUnmatched(
+                lang.require("option", "require_error").format(source=_param.name, target=' '.join(analyser.sentences))
+            )
+        analyse_option(analyser, argv, _param)
     elif _param.__class__ is list:
+        exc: Exception | None = None
         for opt in _param:
             _data, _index = argv.data_set()
             try:
-                opt_n, opt_v = analyse_option(analyser, argv, opt)
-                analyser.options_result[opt_n] = opt_v
+                if opt.requires and analyser.sentences != opt.requires:
+                    raise ParamsUnmatched(lang.require("option", "require_error").format(
+                        source=opt.name, target=' '.join(analyser.sentences)
+                    ))
+                analyser.sentences = []
+                analyse_option(analyser, argv, opt)
                 _data.clear()
+                exc = None
                 break
             except Exception as e:
                 exc = e
                 argv.data_reset(_data, _index)
-                continue
-        else:
+        if exc:
             raise exc  # type: ignore  # noqa
-    elif _param.__class__ is Sentence:
-        analyser.sentences.append(argv.next()[0])
     elif _param is not None:
-        _param.process(argv)
-        analyser.subcommands_result.setdefault(_param.command.dest, _param.result())
+        if _param.command.requires and analyser.sentences != _param.command.requires:
+            raise ParamsUnmatched(
+                lang.require("subcommand", "require_error").format(
+                    source=_param.command.name, target=' '.join(analyser.sentences)
+                )
+            )
+        analyser.subcommands_result[_param.command.dest] = _param.process(argv).result()
+    else:
+        raise TerminateLoop(str(_text))
+    analyser.sentences.clear()
     argv.context = None
 
 
 def analyse_header(header: Header, argv: Argv) -> HeadResult:
+    """分析头部
+
+    Args:
+        header (Header): 头部
+        argv (Argv): 命令行参数
+
+    Returns:
+        HeadResult: 分析结果
+    """
     content = header.content
     mapping = header.mapping
     head_text, _str = argv.next()
-    if content.__class__ is TPattern and _str and (mat := content.fullmatch(head_text)):
-        return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
-    elif isinstance(content, BasePattern) and (val := content.exec(head_text, Empty)).success:
-        return HeadResult(head_text, val.value, True, fixes=mapping)
-
-    may_command, _m_str = argv.next()
-    if content.__class__ is list and _m_str:
-        for pair in content:
-            if res := pair.match(head_text, may_command):
-                return HeadResult(*res, fixes=mapping)
-    if content.__class__ is Double and (
-        res := content.match(head_text, may_command, _str, _m_str, argv.rollback)
-    ):
-        return HeadResult(*res, fixes=mapping)
+    if content.__class__ is TPattern and _str:
+        if mat := content.fullmatch(head_text):
+            return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
+        if header.compact and (mat := content.match(head_text)):
+            argv.rollback(head_text[len(mat[0]):], replace=True)
+            return HeadResult(mat[0], mat[0], True, mat.groupdict(), mapping)
+    elif isinstance(content, BasePattern):
+        if (val := content.exec(head_text, Empty)).success:
+            return HeadResult(head_text, val.value, True, fixes=mapping)
+        if header.compact and (val := content.prefixed().exec(head_text, Empty)).success:
+            if _str:
+                argv.rollback(head_text[len(str(val.value)):], replace=True)
+            return HeadResult(val.value, val.value, True, fixes=mapping)
+    else:
+        may_command, _m_str = argv.next()
+        if content.__class__ is list and _m_str:
+            for pair in content:
+                if res := pair.match(head_text, may_command, argv.rollback, header.compact):
+                    return HeadResult(*res, fixes=mapping)
+        if content.__class__ is Double and (
+            res := content.match(head_text, may_command, _str, _m_str, argv.rollback, header.compact)
+        ):
+            return HeadResult(*res, fixes=mapping)
 
     if _str and argv.fuzzy_match:
         command, prefixes = header.origin
         headers_text = []
         if prefixes and prefixes != [""]:
             headers_text.extend(f"{i}{command}" for i in prefixes)
         elif command:
             headers_text.append(str(command))
         if isinstance(content, (TPattern, BasePattern)):
             source = head_text
         else:
-            source = head_text + argv.separators[0] + str(may_command)
+            source = head_text + argv.separators[0] + str(may_command)  # noqa
         if source == command:
             raise ParamsUnmatched(lang.require("header", "error").format(target=head_text))
         for ht in headers_text:
-            if levenshtein_norm(source, ht) >= config.fuzzy_threshold:
+            if levenshtein(source, ht) >= config.fuzzy_threshold:
                 raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(target=source, source=ht))
     raise ParamsUnmatched(lang.require("header", "error").format(target=head_text))
 
 
 def handle_help(analyser: Analyser, argv: Argv):
+    """处理帮助选项触发"""
     _help_param = [str(i) for i in argv.release(recover=True) if str(i) not in argv.special]
     output_manager.send(
         analyser.command.name,
         lambda: analyser.command.formatter.format_node(_help_param),
     )
     return analyser.export(argv, True)
 
 
 _args = Args["delete;?", "delete"]["name", str]["command", str, "_"]
 
 
 def handle_shortcut(analyser: Analyser, argv: Argv):
+    """处理快捷命令触发"""
     argv.next()
-    opt_v = analyse_args(argv, _args)
+    try:
+        opt_v = analyse_args(argv, _args)
+    except SpecialOptionTriggered:
+        return handle_completion(analyser, argv)
     try:
         msg = analyser.command.shortcut(
             opt_v["name"],
             None if opt_v["command"] == "_" else {"command": argv.converter(opt_v["command"])},
             bool(opt_v.get("delete"))
         )
         output_manager.send(analyser.command.name, lambda: msg)
     except Exception as e:
         output_manager.send(analyser.command.name, lambda: str(e))
     return analyser.export(argv, True)
 
 
-def _prompt_unit(argv: Argv, trigger: Arg):
-    if trigger.field.completion:
-        comp = trigger.field.completion()
+def _prompt_unit(analyser: Analyser, argv: Argv, trig: Arg):
+    if trig.field.completion:
+        comp = trig.field.completion()
         if isinstance(comp, str):
             return [Prompt(comp, False)]
         releases = argv.release(recover=True)
         target = str(releases[-1]) or str(releases[-2])
         o = list(filter(lambda x: target in x, comp)) or comp
         return [Prompt(i, False, target) for i in o]
-    default = trigger.field.default_gen
-    o = f"[{trigger.name}]{trigger.value}{'' if default is None else f' default:({None if default is Empty else default})'}"
-    return [Prompt(o, False)]
+    return [Prompt(analyser.command.formatter.param(trig), False)]
 
 
 def _prompt_sentence(analyser: Analyser):
     res: list[str] = []
     s_len = len(stc := analyser.sentences)
     for opt in filter(
         lambda x: len(x.requires) >= s_len and x.requires[s_len - 1] == stc[-1],
@@ -420,54 +554,50 @@
 def _prompt_none(analyser: Analyser, argv: Argv, got: list[str]):
     res: list[Prompt] = []
     if not analyser.args_result and analyser.self_args.argument:
         unit = analyser.self_args.argument[0]
         if gen := unit.field.completion:
             res.extend([Prompt(comp, False)] if isinstance(comp := gen(), str) else [Prompt(i, False) for i in comp])
         else:
-            default = unit.field.default_gen
-            res.append(
-                Prompt(
-                    f"[{unit.name}]{unit.value}{'' if default is None else f' ({None if default is Empty else default})'}",
-                    False
-                )
-            )
+            res.append(Prompt(analyser.command.formatter.param(unit), False))
     for opt in filter(
         lambda x: x.name not in argv.completion_names,
         analyser.command.options,
     ):
         if opt.requires and all(opt.requires[0] not in i for i in got):
             res.append(Prompt(opt.requires[0]))
         elif opt.dest not in got:
             res.extend([Prompt(al) for al in opt.aliases] if isinstance(opt, Option) else [Prompt(opt.name)])
     return res
 
 
 def prompt(analyser: Analyser, argv: Argv, trigger: str | None = None):
-    trigger = trigger or argv.context
+    """获取补全列表"""
+    _trigger = trigger or argv.context
     got = [*analyser.options_result.keys(), *analyser.subcommands_result.keys(), *analyser.sentences]
-    if isinstance(trigger, Arg):
-        return _prompt_unit(argv, trigger)
-    elif isinstance(trigger, Subcommand):
-        return [Prompt(i) for i in analyser.get_sub_analyser(trigger).compile_params]
-    elif isinstance(trigger, str):
-        res = list(filter(lambda x: trigger in x, analyser.compile_params))
+    if isinstance(_trigger, Arg):
+        return _prompt_unit(analyser, argv, _trigger)
+    elif isinstance(_trigger, Subcommand):
+        return [Prompt(i) for i in analyser.get_sub_analyser(_trigger).compile_params]
+    elif isinstance(_trigger, str):
+        res = list(filter(lambda x: _trigger in x, analyser.compile_params))
         if not res:
             return []
         out = [i for i in res if i not in got]
-        return [Prompt(i, True, trigger) for i in (out or res)]
+        return [Prompt(i, True, _trigger) for i in (out or res)]
     releases = argv.release(recover=True)
     target = str(releases[-1]) or str(releases[-2])
     if _res := list(filter(lambda x: target in x and target != x, analyser.compile_params)):
         out = [i for i in _res if i not in got]
         return [Prompt(i, True, target) for i in (out or _res)]
     return _prompt_sentence(analyser) if analyser.sentences else _prompt_none(analyser, argv, got)
 
 
 def handle_completion(analyser: Analyser, argv: Argv, trigger: str | None = None):
+    """处理补全选项触发"""
     if res := prompt(analyser, argv, trigger):
         if comp_ctx.get(None):
             raise PauseTriggered(res)
         output_manager.send(
             analyser.command.name,
             lambda: f"{lang.require('completion', 'node')}\n* " + "\n* ".join([i.text for i in res]),
         )
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/en-US.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925925925925926%*

 * *Differences: {"'option'": "OrderedDict([('name_error', '{target} not matched with option {source}'), "*

 * *             '(\'require_error\', "Option {source}\'s required is not {target}")])',*

 * * "'subcommand'": "{'name_error': '{target} not matched with subcommand {source}', 'require_error': "*

 * *                 '"Subcommand {source}\'s required is not {target}"}'}*

```diff
@@ -65,20 +65,26 @@
         "help_header": "# Following commands are available:",
         "help_pages": "Page {current} of {total}",
         "incorrect_shortcut": "Shortcut {target} cannot be used",
         "target_command_error": "The target command of {shortcut} is not {target}",
         "undefined_command": "Command {target} is not defined",
         "undefined_shortcut": "Shortcut {target} is not defined"
     },
+    "option": {
+        "name_error": "{target} not matched with option {source}",
+        "require_error": "Option {source}'s required is not {target}"
+    },
     "shortcut": {
         "add_success": "Add shortcut: \"{shortcut}\" for {target} successfully",
         "delete_success": "Delete shortcut: \"{shortcut}\" for {target} successfully",
         "no_recent_command": "get recent message failed",
         "recent_command_error": "command {target} is not same as recent message's command {source}"
     },
     "stub": {
         "key_error": "{target} is not supported"
     },
     "subcommand": {
-        "args_missing": "subcommand \"{name}\" missed its args"
+        "args_missing": "subcommand \"{name}\" missed its args",
+        "name_error": "{target} not matched with subcommand {source}",
+        "require_error": "Subcommand {source}'s required is not {target}"
     }
 }
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/zh-CN.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925925925925926%*

 * *Differences: {"'option'": "OrderedDict([('name_error', '{target} 与选项 {source} 不匹配'), ('require_error', '选项 "*

 * *             "{source} 需求的前置文字并非 {target}')])",*

 * * "'subcommand'": "{'name_error': '{target} 与子命令 {source} 不匹配', 'require_error': '子命令 {source} "*

 * *                 "需求的前置文字并非 {target}'}"}*

```diff
@@ -65,19 +65,25 @@
         "help_header": "# \u5f53\u524d\u53ef\u7528\u7684\u547d\u4ee4\u6709:",
         "help_pages": "\u7b2c {current}/{total} \u9875",
         "incorrect_shortcut": "\u5feb\u6377\u547d\u4ee4 {target} \u65e0\u6cd5\u4f7f\u7528",
         "target_command_error": "{shortcut} \u7684\u76ee\u6807\u547d\u4ee4 {target} \u9519\u8bef",
         "undefined_command": "\u547d\u4ee4 {target} \u4e0d\u5b58\u5728",
         "undefined_shortcut": "\u5feb\u6377\u547d\u4ee4 {target} \u4e0d\u5b58\u5728"
     },
+    "option": {
+        "name_error": "{target} \u4e0e\u9009\u9879 {source} \u4e0d\u5339\u914d",
+        "require_error": "\u9009\u9879 {source} \u9700\u6c42\u7684\u524d\u7f6e\u6587\u5b57\u5e76\u975e {target}"
+    },
     "shortcut": {
         "add_success": "{target} \u7684\u5feb\u622a\u6307\u4ee4: \"{shortcut}\" \u6dfb\u52a0\u6210\u529f",
         "delete_success": "{target} \u7684\u5feb\u622a\u6307\u4ee4: \"{shortcut}\" \u5220\u9664\u6210\u529f",
         "recent_command_error": "\u5386\u53f2\u8bb0\u5f55\u5bf9\u5e94\u7684\u547d\u4ee4 {source} \u4e0e \u672c\u547d\u4ee4 {target} \u4e0d\u4e00\u81f4"
     },
     "stub": {
         "key_error": "\u4e0d\u652f\u6301 {target}"
     },
     "subcommand": {
-        "args_missing": "\u5b50\u547d\u4ee4 \"{name}\" \u7f3a\u5c11\u5fc5\u8981\u53c2\u6570"
+        "args_missing": "\u5b50\u547d\u4ee4 \"{name}\" \u7f3a\u5c11\u5fc5\u8981\u53c2\u6570",
+        "name_error": "{target} \u4e0e\u5b50\u547d\u4ee4 {source} \u4e0d\u5339\u914d",
+        "require_error": "\u5b50\u547d\u4ee4 {source} \u9700\u6c42\u7684\u524d\u7f6e\u6587\u5b57\u5e76\u975e {target}"
     }
 }
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,52 @@
 from copy import copy
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload, Generic
 from typing_extensions import NotRequired
 from tarina import LRU, lang
 from weakref import WeakKeyDictionary, WeakValueDictionary
 
-from .argv import Argv
+from .argv import Argv, __argv_type__
 from .arparma import Arparma
 from .config import Namespace, config
 from .exceptions import ExceedMaxCount
-from .typing import DataCollection, TDC
+from .typing import DataCollection, TDC, CommandMeta
 
 
 if TYPE_CHECKING:
-    from .analyser import Analyser
-    from .core import Alconna, CommandMeta
+    from ._internal._analyser import Analyser
+    from .core import Alconna
 
 
     class ShortcutArgs(TypedDict, Generic[TDC]):
+        """快捷指令参数"""
+
         command: NotRequired[TDC]
+        """快捷指令的命令"""
         args: NotRequired[list[Any]]
+        """快捷指令的附带参数"""
         fuzzy: NotRequired[bool]
+        """是否允许命令后随参数"""
 else:
     class ShortcutArgs(TypedDict):
+        """快捷指令参数"""
+
         command: NotRequired[DataCollection[Any]]
+        """快捷指令的命令"""
         args: NotRequired[list[Any]]
+        """快捷指令的附带参数"""
         fuzzy: NotRequired[bool]
+        """是否允许命令后随参数"""
 
 
 class CommandManager:
     """
-    Alconna 命令管理器
+    `Alconna` 命令管理器
 
-    命令管理器负责记录命令, 并存储快捷指令。
+    命令管理器负责记录命令, 存储命令, 命令行参数, 命令解析器, 快捷指令等
     """
 
     sign: str
     current_count: int
     max_count: int
 
     __commands: dict[str, WeakValueDictionary[str, Alconna]]
@@ -61,15 +71,15 @@
         self.current_count = 0
 
         self.__commands = {}
         self.__argv = WeakKeyDictionary()
         self.__analysers = WeakKeyDictionary()
         self.__abandons = []
         self.__shortcuts = {}
-        self.__record = LRU(config.message_max_cache)
+        self.__record = LRU(128)
 
         def _del():
             self.__commands.clear()
             for ana in self.__analysers.values():
                 ana._clr()
             self.__analysers.clear()
             self.__abandons.clear()
@@ -89,15 +99,19 @@
     def dump_cache(self) -> None:
         """保存缓存"""
         with shelve.open(self.cache_path) as db:
             db["shortcuts"] = self.__shortcuts
 
     @property
     def get_loaded_namespaces(self):
-        """获取所有命名空间"""
+        """获取所有命名空间
+
+        Returns:
+            list[str]: 所有命名空间的名称
+        """
         return list(self.__commands.keys())
 
     @staticmethod
     def _command_part(command: str) -> tuple[str, str]:
         """获取命令的组成部分"""
         command_parts = command.split("::", maxsplit=1)[-2:]
         if len(command_parts) != 2:
@@ -110,15 +124,15 @@
         return config.namespaces.get(name)
 
     def register(self, command: Alconna) -> None:
         """注册命令解析器, 会同时记录解析器对应的命令"""
         if self.current_count >= self.max_count:
             raise ExceedMaxCount
         self.__argv.pop(command, None)
-        self.__argv[command] = Argv(
+        self.__argv[command] = __argv_type__(
             command.namespace_config,
             fuzzy_match=command.meta.fuzzy_match,
             to_text=command.namespace_config.to_text,
             converter=command.namespace_config.converter,
             separators=command.separators,
             message_cache=command.namespace_config.enable_message_cache,
             filter_crlf=not command.meta.keep_crlf,
@@ -149,14 +163,15 @@
         try:
             return self.__analysers[command]  # type: ignore
         except KeyError as e:
             namespace, name = self._command_part(command.path)
             raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
 
     def requires(self, *paths: str) -> zip[tuple[Analyser, Argv]]:  # type: ignore
+        """获取多个命令解析器"""
         return zip(
             [v for k, v in self.__analysers.items() if k.path in paths],
             [v for k, v in self.__argv.items() if k.path in paths],
         )
 
     def delete(self, command: Alconna | str) -> None:
         """删除命令"""
@@ -164,36 +179,43 @@
         try:
             base = self.__commands[namespace][name]
             base.formatter.remove(base)
             del self.__argv[base]
             del self.__analysers[base]
             del self.__commands[namespace][name]
             self.current_count -= 1
-        finally:
+        except KeyError:
             if self.__commands.get(namespace) == {}:
                 del self.__commands[namespace]
-            return None
 
     def is_disable(self, command: Alconna) -> bool:
         """判断命令是否被禁用"""
         return command in self.__abandons
 
     def set_enabled(self, command: Alconna | str, enabled: bool):
+        """设置命令是否被禁用"""
         if isinstance(command, str):
             command = self.get_command(command)
         if enabled and command in self.__abandons:
             self.__abandons.remove(command)
         if not enabled and command not in self.__abandons:
             self.__abandons.append(command)
 
-    def add_shortcut(self, target: Alconna, key: str, source: Arparma | ShortcutArgs):
-        """添加快捷命令"""
+    def add_shortcut(self, target: Alconna[TDC], key: str, source: Arparma | ShortcutArgs[TDC]):
+        """添加快捷命令
+
+        Args:
+            target (Alconna): 目标命令
+            key (str): 快捷命令的名称
+            source (Arparma | ShortcutArgs): 快捷命令的参数
+        """
         namespace, name = self._command_part(target.path)
+        argv = self.resolve(target)
         if isinstance(source, dict):
-            source['command'] = source.get('command', target.command or target.name)
+            source['command'] = source.get('command', argv.converter(target.command or target.name))
             source.setdefault('fuzzy', True)
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         elif source.matched:
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         else:
             raise ValueError(lang.require("manager", "incorrect_shortcut").format(target=f"{key}"))
 
@@ -206,27 +228,36 @@
     @overload
     def find_shortcut(
         self, target: Alconna[TDC], query: str
     ) -> tuple[Arparma[TDC] | ShortcutArgs[TDC], Match[str] | None]:
         ...
 
     def find_shortcut(self, target: Alconna[TDC], query: str | None = None):
-        """查找快捷命令"""
+        """查找快捷命令
+
+        Args:
+            target (Alconna): 目标命令
+            query (str, optional): 快捷命令的名称. Defaults to None.
+
+        Returns:
+            list[Union[Arparma, ShortcutArgs]] | tuple[Union[Arparma, ShortcutArgs], Match[str]]: \
+            快捷命令的参数, 若没有 `query` 则返回目标命令的所有快捷命令, 否则返回匹配的快捷命令
+        """
         namespace, name = self._command_part(target.path)
         if query:
             try:
                 return self.__shortcuts[f"{namespace}.{name}::{query}"], None
             except KeyError as e:
-                for k in self.__shortcuts.keys():
+                for k in self.__shortcuts:
                     if mat := re.match(k.split("::")[1], query):
                         return self.__shortcuts[k], mat
                 raise ValueError(
                     lang.require("manager", "target_command_error").format(target=f"{namespace}.{name}", shortcut=query)
                 ) from e
-        return [self.__shortcuts[k] for k in self.__shortcuts.keys() if f"{namespace}.{name}" in k]
+        return [self.__shortcuts[k] for k in self.__shortcuts if f"{namespace}.{name}" in k]
 
     def delete_shortcut(self, target: Alconna, key: str | None = None):
         """删除快捷命令"""
         for res in [self.find_shortcut(target, key)[0]] if key else self.find_shortcut(target):
             with contextlib.suppress(StopIteration):
                 self.__shortcuts.pop(next(filter(lambda x: self.__shortcuts[x] == res, self.__shortcuts)))
 
@@ -243,41 +274,49 @@
             return list(self.__analysers.keys())
         if isinstance(namespace, Namespace):
             namespace = Namespace.name
         if namespace not in self.__commands:
             return []
         return list(self.__commands[namespace].values())
 
-    def broadcast(self, message: TDC, namespace: str | Namespace = '') -> Arparma[TDC] | None:
-        """将一段命令广播给当前空间内的所有命令"""
+    def test(self, message: TDC, namespace: str | Namespace = '') -> Arparma[TDC] | None:
+        """将一段命令给当前空间内的所有命令测试匹配"""
         for cmd in self.get_commands(namespace):
             if (res := cmd.parse(message)) and res.matched:
                 return res
 
+    def broadcast(self, message: TDC, namespace: str | Namespace = '') -> WeakValueDictionary[str, Arparma[TDC]]:
+        """将一段命令给当前空间内的所有命令测试匹配"""
+        data = WeakValueDictionary()
+        for cmd in self.get_commands(namespace):
+            if (res := cmd.parse(message)) and res.matched:
+                data[cmd.path] = res
+        return data
+
     def all_command_help(
         self,
         show_index: bool = False,
         namespace: str | Namespace | None = None,
         header: str | None = None,
         pages: str | None = None,
         footer: str | None = None,
         max_length: int = -1,
         page: int = 1
     ) -> str:
         """
         获取所有命令的帮助信息
 
         Args:
-            show_index: 是否展示索引
-            namespace: 指定的命名空间, 如果为None则选择所有命令
-            header: 帮助信息的页眉
-            pages: 帮助信息的页码
-            footer: 帮助信息的页脚
-            max_length: 单个页面展示的最大长度
-            page: 当前页码
+            show_index (bool, optional): 是否展示索引. Defaults to False.
+            namespace (str | Namespace | None, optional): 指定的命名空间, 如果为None则选择所有命令.
+            header (str | None, optional): 帮助信息的页眉.
+            pages (str | None, optional): 帮助信息的页码.
+            footer (str | None, optional): 帮助信息的页脚.
+            max_length (int, optional): 单个页面展示的最大长度. Defaults to -1.
+            page (int, optional): 当前页码. Defaults to 1.
         """
         pages = pages or lang.require("manager", "help_pages")
         cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
         header = header or lang.require("manager", "help_header")
         if max_length < 1:
             command_string = "\n".join(
                 f" {str(index).rjust(len(str(len(cmds))), '0')} {slot.name} : {slot.meta.description}"
@@ -313,44 +352,56 @@
 
     def command_help(self, command: str) -> str | None:
         """获取单个命令的帮助"""
         if cmd := self.get_command(command):
             return cmd.get_help()
 
     def record(self, token: int, result: Arparma):
+        """记录某个命令的 `token`"""
         self.__record[token] = result
 
     def get_record(self, token: int) -> Arparma | None:
+        """获取某个 `token` 对应的 `Arparma` 对象"""
         if token in self.__record:
             return self.__record[token]
 
     def get_token(self, result: Arparma) -> int:
+        """获取某个命令的 `token`"""
         return next((token for token, res in self.__record.items() if res == result), 0)
 
     def get_result(self, command: Alconna) -> list[Arparma]:
+        """获取某个命令的所有 `Arparma` 对象"""
         return [v for v in self.__record.values() if v.source == command]
 
     @property
     def recent_message(self) -> DataCollection[str | Any] | None:
+        """获取最近一次使用的命令"""
         if rct := self.__record.peek_first_item():
             return rct[1].origin  # type: ignore
 
     @property
     def last_using(self):
+        """获取最近一次使用的 `Alconna` 对象"""
         if rct := self.__record.peek_first_item():
             return rct[1].source  # type: ignore
 
     @property
     def records(self) -> LRU[int, Arparma]:
+        """获取当前记录"""
         return self.__record
 
     def reuse(self, index: int = -1):
+        """获取当前记录中的某个值"""
         key = self.__record.keys()[index]
         return self.__record[key]
 
+    def set_record_size(self, size: int):
+        """设置记录的最大长度"""
+        self.__record.set_size(size)
+
     def __repr__(self):
         return (
             f"Current: {hex(id(self))} in {datetime.now().strftime('%Y/%m/%d %H:%M:%S')}\n" +
             "Commands:\n" +
             f"[{', '.join([cmd.path for cmd in self.get_commands()])}]" +
             "\nShortcuts:\n" +
             "\n".join([f" {k} => {v}" for k, v in self.__shortcuts.items()]) +
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/model.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from dataclasses import dataclass
 _repr_ = lambda self: "(" + " ".join([f"{k}={getattr(self, k, ...)!r}" for k in self.__slots__]) + ")"
 
 
 @dataclass(init=False, eq=True)
 class Sentence:
-    __slots__ = ("name", "separators")
+    __slots__ = ("name")
     __repr__ = _repr_
-    def __init__(self, name, separators=None):
+    def __init__(self, name):
         self.name = name
-        self.separators = separators or (" ",)
 
 
 @dataclass(init=False, eq=True)
 class OptionResult:
     __slots__ = ("value", "args")
     __repr__ = _repr_
     def __init__(self, value=Ellipsis, args=None):
@@ -38,9 +37,9 @@
     def __init__(self, origin=None, result=None, matched=False, groups=None, fixes=None):
         self.origin = origin
         self.result = result
         self.matched = matched
         self.groups = groups or {}
         if fixes:
             self.groups.update(
-                {k: v(self.groups[k])._value for k, v in fixes.items() if k in self.groups}  # noqa
+                {k: v.exec(self.groups[k]).value for k, v in fixes.items() if k in self.groups}  # noqa
             )
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/output.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,80 +4,112 @@
 from dataclasses import dataclass, field
 from typing import Any, Callable
 from weakref import finalize
 
 
 @dataclass(init=True, unsafe_hash=True)
 class Sender:
+    """发送器"""
     action: Callable[..., Any]
+    """发送行为函数"""
     generator: Callable[[], str]
+    """发送内容生成器"""
 
     def __call__(self, *args, **kwargs):
         res = self.generator()
         data = self.action(res)
         return data if data and isinstance(data, dict) else {"output": res}
 
 
 @dataclass
 class OutputManager:
-    """帮助信息"""
+    """命令输出管理器"""
     cache: dict[str, Callable] = field(default_factory=dict)
+    """缓存的输出行为"""
     outputs: dict[str, Sender] = field(default_factory=dict)
+    """输出行为"""
     send_action: Callable[[str], Any] = field(default=lambda x: print(x))
+    """默认的发送行为"""
     _out_cache: dict[str, dict[str, Any]] = field(default_factory=dict, hash=False, init=False)
 
     def __post_init__(self):
         def _clr(mgr: OutputManager):
             mgr.cache.clear()
             mgr.outputs.clear()
             mgr._out_cache.clear()
 
         finalize(self, _clr, self)
 
     def send(self, command: str | None = None, generator: Callable[[], str] | None = None):
-        """调用指定的输出行为"""
+        """调用指定的输出行为
+
+        Args:
+            command (str | None, optional): 输出行为对应的命令名称
+            generator (Callable[[], str] | None, optional): 输出内容生成器
+        """
         if sender := self.get(command):
             if generator:
                 sender.generator = generator
         elif generator:
             sender = self.set(generator, command)
         else:
             raise KeyError(f"Command {command} not found")
         res = sender()
         if command in self._out_cache:
             self._out_cache[command].update(res)
         return res
 
     def get(self, command: str | None = None) -> Sender | None:
-        """获取指定的输出行为"""
+        """获取指定的输出行为
+
+        Args:
+            command (str | None, optional): 输出行为对应的命令名称
+        """
         return self.outputs.get(command or "$global")
 
     def set(self, generator: Callable[[], str], command: str | None = None) -> Sender:
-        """设置指定的输出行为"""
+        """设置指定的输出行为
+
+        Args:
+            generator (Callable[[], str]): 输出内容生成器
+            command (str | None, optional): 输出行为对应的命令名称
+        """
         command = command or "$global"
         if command in self.outputs:
             self.outputs[command].generator = generator
         elif command in self.cache:
             self.outputs[command] = Sender(self.cache.pop(command), generator)
         else:
             self.outputs[command] = Sender(self.send_action, generator)
         return self.outputs[command]
 
     def set_action(self, action: Callable[[str], Any], command: str | None = None):
-        """修改输出行为"""
+        """修改输出行为
+
+        Args:
+            action (Callable[[str], Any]): 输出行为函数
+            command (str | None, optional): 输出行为指定对应的命令名称
+        """
         if command is None or command == "$global":
             self.send_action = action
         elif cmd := self.outputs.get(command):
             cmd.action = action
         else:
             self.cache[command] = action
 
     @contextmanager
     def capture(self, command: str | None = None):
-        """捕获输出"""
+        """捕获输出
+
+        Args:
+            command (str | None, optional): 输出行为指定对应的命令名称
+
+        Yields:
+            dict[str, Any]: 输出内容
+        """
         command = command or "$global"
         _cache = self._out_cache.setdefault(command, {})
         yield _cache
         _cache.clear()
 
 
 output_manager = OutputManager()
```

### Comparing `arclet-alconna-1.7.0rc4/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.0rc5/src/arclet/alconna/stub.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,56 +16,68 @@
 
 
 @dataclass(init=True, eq=True)
 class BaseStub(Generic[T_Origin], metaclass=ABCMeta):
     """基础的命令组件存根"""
 
     _origin: T_Origin
+    """原始的命令组件"""
     _value: Any = field(default=None)
+    """解析结果"""
     available: bool = field(default=False, init=False)
+    """是否可用"""
 
     @property
     def origin(self) -> T_Origin:
+        """原始的命令组件"""
         return self._origin
 
     @abstractmethod
     def set_result(self, result: Any) -> Self:
         """设置解析结果与可用性"""
 
     def __repr__(self):
         return f"{{{', '.join([f'{k}={v}' for k, v in vars(self).items() if v and not k.startswith('_')])}}}"
 
 
 @dataclass(init=True)
 class ArgsStub(BaseStub[Args]):
     """参数存根"""
     _value: dict[str, Any] = field(default_factory=dict)
+    """解析结果"""
 
     def __post_init__(self):
         for arg in self._origin.argument:
             key = arg.name
             if arg.value in (AllParam, AnyOne):
                 self.__annotations__[key] = Any
             elif isinstance(arg.value, BasePattern):
                 self.__annotations__[key] = arg.value.origin
             else:
                 self.__annotations__[key] = arg.value
-            setattr(self, key, arg.field.default_gen)
+            setattr(self, key, arg.field.default)
 
     def set_result(self, result: dict[str, Any]):
         if result:
             self._value = result.copy()
             self.available = True
         return self
 
     @property
     def first(self) -> Any:
+        """第一个参数"""
         return self.__getitem__(0)
 
     def get(self, item: str | type[T], default=None) -> T | Any:
+        """获取参数结果
+
+        Args:
+            item (str | type[T]): 参数名或参数类型
+            default (Any, optional): 默认值. Defaults to None.
+        """
         if isinstance(item, str):
             return self._value.get(item, default)
         for k, v in self.__annotations__.items():
             if isclass(v) and (item == v or issubclass(v, item)):
                 return self._value.get(k, default)
         return default
 
@@ -89,17 +101,21 @@
         return self._value[item]
 
 
 @dataclass(init=True)
 class OptionStub(BaseStub[Option]):
     """选项存根"""
     args: ArgsStub = field(init=False)
+    """选项的参数存根"""
     dest: str = field(init=False)
+    """选项的目标名称"""
     aliases: list[str] = field(init=False)
+    """选项的别名"""
     name: str = field(init=False)
+    """选项的名称"""
 
     def __post_init__(self):
         self.dest = self._origin.dest
         self.aliases = [alias.lstrip('-') for alias in self._origin.aliases]
         self.name = self._origin.name.lstrip('-')
         self.args = ArgsStub(self._origin.args)
 
@@ -111,18 +127,23 @@
         return self
 
 
 @dataclass(init=True)
 class SubcommandStub(BaseStub[Subcommand]):
     """子命令存根"""
     args: ArgsStub = field(init=False)
+    """子命令的参数存根"""
     dest: str = field(init=False)
+    """子命令的目标名称"""
     options: list[OptionStub] = field(init=False)
+    """子命令的子选项存根"""
     subcommands: list[SubcommandStub] = field(init=False)
+    """子命令的子子命令存根"""
     name: str = field(init=False)
+    """子命令的名称"""
 
     def __post_init__(self):
         self.dest = self._origin.dest
         self.name = self._origin.name.lstrip('-')
         self.args = ArgsStub(self._origin.args)
         self.options = [OptionStub(opt) for opt in self._origin.options if isinstance(opt, Option)]
         self.subcommands = [SubcommandStub(sub) for sub in self._origin.options if isinstance(sub, Subcommand)]
@@ -135,8 +156,21 @@
                 option.set_result(result.options.get(option.dest, None))
             for subcommand in self.subcommands:
                 subcommand.set_result(result.subcommands.get(subcommand.dest, None))
             self.available = True
         return self
 
     def option(self, name: str) -> OptionStub:
+        """获取子选项存根
+
+        Args:
+            name (str): 子选项名称
+        """
         return next(opt for opt in self.options if opt.name == name)
+
+    def subcommand(self, name: str) -> SubcommandStub:
+        """获取子子命令存根
+
+        Args:
+            name (str): 子子命令名称
+        """
+        return next(sub for sub in self.subcommands if sub.name == name)
```

### Comparing `arclet-alconna-1.7.0rc4/PKG-INFO` & `arclet-alconna-1.7.0rc5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc4
+Version: 1.7.0rc5
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -79,14 +79,15 @@
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
 * High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
+* Intuitive way to create command components
 * Powerful Automatic Type Parse and Conversion
 * Customizable Help Text Formatter and Control of Command Analyser
 * i18n Support
 * Cache of input command for quick response of repeated command
 * Easy-to-use Construct and Usage of Command Shortcut
 * Can bind callback function to execute after command parsing
 * Can create command completion session to implement multi-round continuous completion prompt
@@ -94,65 +95,99 @@
 
 Example of Callback Executor:
 
 ```python
 # callback.py
 from arclet.alconna import Alconna, Args
 
-alc = Alconna("test", Args["foo", int]["bar", str])
+alc = Alconna("callback", Args["foo", int]["bar", str])
 
 @alc.bind()
 def callback(foo: int, bar: str):
     print(f"foo: {foo}")
     print(f"bar: {bar}")
     print(bar * foo)
     
 if __name__ == "__main__":
     alc()
 ```
 
 ```shell
-$ python callback.py test 3 hello
+$ python callback.py 3 hello
 foo: 3
 bar: hello
 hellohellohello
 ```
 
 
 Example of Type Conversion:
 
 ```python
 from arclet.alconna import Alconna, Args
 from pathlib import Path
 
-read = Alconna(
-    "read", Args["data", bytes], 
-    action=lambda data: print(type(data))
-)
+read = Alconna("read", Args["data", bytes])
+
+@read.bind()
+def cb(data: bytes):
+    print(type(data))
 
 read.parse(["read", b'hello'])
 read.parse("read test_fire.py")
 read.parse(["read", Path("test_fire.py")])
 
 '''
 <class 'bytes'>
 <class 'bytes'>
 <class 'bytes'>
 '''
 ```
 
+Example of Component creation:
+```python
+# component.py
+from arclet.alconna import Alconna, Args, Option, Subcommand, store_true, count, append
+
+alc = Alconna(
+    "component",
+    Args["path", str],
+    Option("--verbose|-v", action=count),
+    Option("-f", Args["flag", str], compact=True, action=append),
+    Subcommand("sub", Option("bar", action=store_true, default=False))
+)
+
+if __name__ == '__main__':
+    res = alc()
+    print(res.query("path"))
+    print(res.query("verbose.value"))
+    print(res.query("f.flag"))
+    print(res.query("sub"))
+```
+
+```shell
+$ python component.py /home/arclet -vvvv -f1 -f2 -f3 sub bar
+/home/arclet
+4
+['1', '2', '3']
+(value=Ellipsis args={} options={'bar': (value=True args={})} subcommands={})
+```
+
 Example of Command Shortcut:
 ```python
 # shortcut.py
 from arclet.alconna import Alconna, Args
 
-alc = Alconna("eval", Args["content", str], action=lambda x: eval(x, {}, {}))
+alc = Alconna("eval", Args["content", str])
 alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
 
-if __name__ == "__main__":
+@alc.bind()
+def cb(content: str):
+    eval(content, {}, {})
+
+if __name__ == '__main__':
     alc()
 ```
 
 ```shell
 $ python shortcut.py eval print(\"hello world\")
 hello world
 $ python shortcut.py echo hello world!
@@ -160,28 +195,28 @@
 ```
 
 Example of Command Completion:
 ```python
 # completion.py
 from arclet.alconna import Alconna, Args, Option
 
-alc = Alconna("test", Args["bar", int]) + Option("foo") + Option("fool")
+alc = Alconna("complete", Args["bar", int]) + Option("foo") + Option("fool")
 
 if __name__ == "__main__":
-    alc.completion()
+    alc()
 ```
 
 ```shell
-$ python completion.py test ?
-next input maybe:
-> foo
-> int
-> -h
-> --help
-> fool
+$ python completion.py ?
+suggest input follows:
+* bar: int
+* --help
+* -h
+* foo
+* fool
 ```
 
 Example of `typing` Support:
 ```python
 from typing import Annotated  # or typing_extensions.Annotated
 from arclet.alconna import Alconna, Args
 
@@ -209,19 +244,14 @@
 ```
 
 ```shell
 $ python fuzzy.py /test_fuzzy foo bar
 /test_fuzy not matched. Are you mean "!test_fuzzy"?
 ```
 
-
-
-
-
-
 ## License
 
 Alconna is licensed under the [MIT License](LICENSE).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
 
 ## Acknowledgement
```

