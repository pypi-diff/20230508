# Comparing `tmp/arclet-alconna-tools-0.5.0.tar.gz` & `tmp/arclet-alconna-tools-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.5.0.tar", last modified: Sun Feb 19 16:06:05 2023, max compression
+gzip compressed data, was "arclet-alconna-tools-0.6.0rc1.tar", last modified: Mon May  8 16:36:19 2023, max compression
```

## Comparing `arclet-alconna-tools-0.5.0.tar` & `arclet-alconna-tools-0.6.0rc1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.5.0/LICENSE
--rw-r--r--   0        0        0     1067 2023-02-19 15:59:12.368160 arclet-alconna-tools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       53 2022-09-16 06:41:48.807371 arclet-alconna-tools-0.5.0/README.md
--rw-r--r--   0        0        0      348 2023-02-19 15:26:05.939282 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2334 2023-02-19 14:12:27.994720 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0     1122 2023-02-19 15:41:06.683894 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0    33228 2023-02-19 15:36:34.759395 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     3893 2023-02-18 14:11:04.424398 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    16075 2023-02-19 15:27:54.964272 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0     4234 2023-02-19 15:33:34.291501 arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      277 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     1081 2023-05-08 16:35:08.337284 arclet-alconna-tools-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-09-16 06:41:48.807371 arclet-alconna-tools-0.6.0rc1/README.md
+-rw-r--r--   0        0        0      391 2023-05-08 11:53:03.576121 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    27100 2023-05-08 15:07:41.119518 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    17495 2023-05-08 16:19:03.896293 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.0rc1/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.5.0/LICENSE` & `arclet-alconna-tools-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.5.0/pyproject.toml` & `arclet-alconna-tools-0.6.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.5.0"
+version = "0.6.0rc1"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "nepattern>=0.4.2",
-    "arclet-alconna>=1.6.1",
+    "nepattern<0.6.0, >=0.5.0",
+    "arclet-alconna>=1.7.0rc6",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/actions.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Alconna ArgAction相关"""
 
 from datetime import datetime
+from tarina import lang
 from typing import Literal
 from dataclasses import dataclass, field
 from arclet.alconna.exceptions import OutBoundsBehave
-from arclet.alconna.config import config
 from arclet.alconna.arparma import Arparma, ArparmaBehavior
 
 
 def exclusion(target_path: str, other_path: str):
     """
     当设置的两个路径同时存在时, 抛出异常
 
@@ -17,15 +17,15 @@
         other_path: 其他路径
     """
 
     class _EXCLUSION(ArparmaBehavior):
         def operate(self, interface: "Arparma"):
             if interface.query(target_path) and interface.query(other_path):
                 raise OutBoundsBehave(
-                    config.lang.behavior_exclude_matched.format(target=target_path, other=other_path)
+                    lang.require("tools", "actions.exclusion").format(left=target_path, right=other_path)
                 )
 
     return _EXCLUSION()
 
 
 def cool_down(seconds: float):
     """
@@ -38,15 +38,15 @@
     @dataclass(unsafe_hash=True)
     class _CoolDown(ArparmaBehavior):
         last_time: datetime = field(default_factory=lambda: datetime.now())
 
         def operate(self, interface: "Arparma"):
             current_time = datetime.now()
             if (current_time - self.last_time).total_seconds() < seconds:
-                raise OutBoundsBehave(config.lang.behavior_cooldown_matched)
+                raise OutBoundsBehave(lang.require("tools", "actions.cooldown"))
             else:
                 self.last_time = current_time
 
     return _CoolDown()
 
 
 def inclusion(*targets: str, flag: Literal["any", "all"] = "any"):
@@ -59,13 +59,13 @@
     """
 
     class _Inclusion(ArparmaBehavior):
         def operate(self, interface: "Arparma"):
             if flag == "all":
                 for target in targets:
                     if not interface.query(target):
-                        raise OutBoundsBehave(config.lang.behavior_inclusion_matched)
+                        raise OutBoundsBehave(lang.require("tools", "actions.inclusion").format(target=target))
             else:
                 all_count = len(targets) - sum(1 for target in targets if interface.query(target))
                 if all_count > 0:
-                    raise OutBoundsBehave(config.lang.behavior_inclusion_matched)
+                    raise OutBoundsBehave(lang.require("tools", "actions.inclusion"))
     return _Inclusion()
```

### Comparing `arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/checker.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/checker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from functools import wraps
 from typing import Callable, Optional, TypeVar
 
 from arclet.alconna import Alconna, CommandMeta, Args
-from arclet.alconna.action import ArgAction
 from typing_extensions import ParamSpec
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def simple_type(raise_exception: bool = False):
     def deco(func: Callable[P, T]) -> Callable[P, Optional[T]]:
-        def inner(*args: P.args, **kwargs: P.kwargs):
-            return {"$func": func(*args, **kwargs)}
         name: str = f"{id(func)}"
         _cmd = Alconna(
             name, Args.from_callable(func)[0],
-            action=ArgAction(inner), meta=CommandMeta(raise_exception=raise_exception)
+            meta=CommandMeta(raise_exception=raise_exception)
         )
 
         @wraps(func)
         def __wrapper__(*args: P.args, **kwargs: P.kwargs):
             param = [name, *args]
             for k, v in kwargs.items():
                 param.extend([f"{k}=", v])
-            return (
-                result.main_args.get("$func", None)
-                if (result := _cmd.parse(param)).matched
-                else None
-            )
+            res = _cmd.parse(param)
+            return res.call(func) if res.matched else None
 
         return __wrapper__
 
     return deco
```

### Comparing `arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/debug.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/debug.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 from collections import namedtuple
 from typing import Any
 import traceback
 
-from arclet.alconna.analyser import Analyser, default_params_parser
-from arclet.alconna.container import DataCollectionContainer
-from arclet.alconna.handlers import analyse_args as ala, analyse_header as alh, analyse_option as alo
+from arclet.alconna._internal._analyser import Analyser, default_compiler
+from arclet.alconna.argv import Argv
+from arclet.alconna._internal._handlers import analyse_args as ala, analyse_header as alh, analyse_option as alo
+from arclet.alconna._internal._header import Header
 from arclet.alconna.typing import DataCollection
 from arclet.alconna.base import Option, Subcommand
 from arclet.alconna.args import Args
 from arclet.alconna.config import config
 
+
 class AnalyseError(Exception):
     """分析时发生错误"""
 
 
 class _DummyAnalyser(Analyser):
     filter_out = []
 
@@ -23,83 +25,84 @@
         options = []
         meta = namedtuple("Meta", ["keep_crlf", "fuzzy_match"])(False, False)
         namespace_config = config.default_namespace
 
     def __new__(cls, *args, **kwargs):
         cls.command = cls._DummyALC()  # type: ignore
         cls.compile_params = {}
-        cls.container = DataCollectionContainer(message_cache=False, filter_crlf=True)
-        cls.special = {}
-        for i in config.default_namespace.builtin_option_name.values():
-            cls.special.fromkeys(i, True)  # noqa  # type: ignore
+        cls.compact_params = []
         return super().__new__(cls)
 
 
-def analyse_args(args: Args, command: DataCollection[str | Any], raise_exception: bool = True):
-    _analyser = _DummyAnalyser.__new__(_DummyAnalyser)
-    _analyser.reset()
-    _analyser.need_main_args = True
-    _analyser.raise_exception = True
+def analyse_args(args: Args, command: list[str | Any], raise_exception: bool = True):
+    argv = Argv(config.default_namespace, message_cache=False, filter_crlf=True)
     try:
-        _analyser.container.build(command)
-        return ala(_analyser, args, len(args))
+        argv.build(["test"] + command)
+        argv.next()
+        return ala(argv, args)
     except Exception as e:
         if raise_exception:
             traceback.print_exception(AnalyseError, e, e.__traceback__)
         return
 
 
 def analyse_header(
     headers: list[str | Any] | list[tuple[Any, str]],
     command_name: str,
     command: DataCollection[str | Any],
     sep: str = " ",
+    compact: bool = False,
     raise_exception: bool = True
 ):
-    _analyser = _DummyAnalyser.__new__(_DummyAnalyser)
-    _analyser.reset()
-    _analyser.container.separators = (sep, )
-    _analyser.need_main_args = False
-    _analyser.__init_header__(command_name, headers)
+    argv = Argv(
+        config.default_namespace,
+        message_cache=False,
+        filter_crlf=True,
+        separators=(sep, )
+    )
+    command_header = Header.generate(command_name, headers, compact=compact)
     try:
-        _analyser.container.build(command)
-        return alh(_analyser)
+        argv.build(command)
+        return alh(command_header, argv)
     except Exception as e:
         if raise_exception:
             traceback.print_exception(AnalyseError, e, e.__traceback__)
         return
 
 
 def analyse_option(option: Option, command: DataCollection[str | Any], raise_exception: bool = True):
+    argv = Argv(config.default_namespace, message_cache=False, filter_crlf=True)
     _analyser = _DummyAnalyser.__new__(_DummyAnalyser)
     _analyser.reset()
-    _analyser.container.separators = (" ", )
+    _analyser.command.separators = (" ",)
     _analyser.need_main_args = False
     _analyser.raise_exception = True
     _analyser.command.options.append(option)
-    default_params_parser(_analyser, _analyser.command.namespace_config)
+    default_compiler(_analyser, _analyser.command.namespace_config, argv.param_ids)
     _analyser.command.options.clear()
     try:
-        _analyser.container.build(command)
-        return alo(_analyser, option)
+        argv.build(command)
+        alo(_analyser, argv, option)
+        return _analyser.options_result[option.dest]
     except Exception as e:
         if raise_exception:
             traceback.print_exception(AnalyseError, e, e.__traceback__)
         return
 
 
 def analyse_subcommand(subcommand: Subcommand, command: DataCollection[str | Any], raise_exception: bool = True):
+    argv = Argv(config.default_namespace, message_cache=False, filter_crlf=True)
     _analyser = _DummyAnalyser.__new__(_DummyAnalyser)
     _analyser.reset()
-    _analyser.container.separators = (" ", )
+    _analyser.command.separators = (" ", )
     _analyser.need_main_args = False
     _analyser.raise_exception = True
     _analyser.command.options.append(subcommand)
-    default_params_parser(_analyser, _analyser.command.namespace_config)
+    default_compiler(_analyser, _analyser.command.namespace_config, argv.param_ids)
     _analyser.command.options.clear()
     try:
-        _analyser.container.build(command)
-        return _analyser.compile_params[subcommand.name].process().export()  # type: ignore
+        argv.build(command)
+        return _analyser.compile_params[subcommand.name].process(argv).result()  # type: ignore
     except Exception as e:
         if raise_exception:
             traceback.print_exception(AnalyseError, e, e.__traceback__)
-        return
+        return
```

### Comparing `arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/formatter.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/formatter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict, Any, Union, Tuple, Optional
-from nepattern import Empty, AllParam, BasePattern
-
+from nepattern import Empty, AllParam
+from tarina import lang
 from arclet.alconna.args import Args, Arg
 from arclet.alconna.base import Subcommand, Option
 from arclet.alconna.formatter import TextFormatter, Trace
 
 
 class ArgParserTextFormatter(TextFormatter):
     """
@@ -13,63 +13,63 @@
 
     def format(self, trace: Trace) -> str:
         parts = trace.body  # type: ignore
         sub_names = [i.name for i in filter(lambda x: isinstance(x, Subcommand), parts)]
         opt_names = [min(i.aliases, key=len) for i in filter(lambda x: isinstance(x, Option), parts)]
         sub_names = f"{{{','.join(sub_names)}}}" if sub_names else ""
         opt_names = (" ".join(f"[{i}]" for i in opt_names)) if opt_names else ""
-        topic = f"命令: {trace.head['name']} {opt_names}\n {sub_names}"
+        topic = f"{lang.require('tools', 'format.ap.title')}: {trace.head['name']} {opt_names}\n {sub_names}"
         header = self.header(trace.head, trace.separators)
         param = self.parameters(trace.args)
         body = self.body(parts)
         return f"{topic}\n{header % (param, body)}"
 
     def param(self, parameter: Arg) -> str:
         name = parameter.name
+        if str(parameter.value).strip("'\"") == name:
+            return f"[{name}]" if parameter.optional else name
+        if parameter.hidden:
+            return f"[{name.upper()}]" if parameter.optional else name.upper()
+        if parameter.value is AllParam:
+            return f"{name.upper()}..."
         arg = f"[{name.upper()}" if parameter.optional else name.upper()
-        if not parameter.hidden:
-            if parameter.value is AllParam:
-                return f"{name.upper()}..."
-            if isinstance(parameter.value, BasePattern):
-                arg += f":{parameter.value}"
-            if parameter.field.display is Empty:
-                arg += "=None"
-            elif parameter.field.display is not None:
-                arg += f"={parameter.field.display}"
+        arg += f":{parameter.value}"
+        if parameter.field.display is Empty:
+            arg += "=None"
+        elif parameter.field.display is not None:
+            arg += f"={parameter.field.display}"
         return f"{arg}]" if parameter.optional else arg
 
     def parameters(self, args: Args) -> str:
         res = ""
         for arg in args.argument:
             if arg.name.startswith('_key_'):
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        return f"{res}\n  内容:\n  " + "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
+        return f"{res}\n  {lang.require('tools', 'format.ap.notice')}:\n  " + \
+            "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
 
     def header(self, root: Dict[str, Any], separators: Tuple[str, ...]) -> str:
-        help_string = f"\n描述: {desc}\n" if (desc := root.get("description")) else ""
-        usage = f"\n用法: {usage}\n" if (usage := root.get("usage")) else ""
-        example = f"\n样例: {example}\n" if (example := root.get("example")) else ""
+        help_string = f"\n{lang.require('tools', 'format.ap.desc')}: {desc}\n" if (desc := root.get("description")) else ""
+        usage = f"\n{lang.require('tools', 'format.ap.usage')}: {usage}\n" if (usage := root.get("usage")) else ""
+        example = f"\n{lang.require('tools', 'format.ap.example')}: {example}\n" if (example := root.get("example")) else ""
         header_text = (
             f"[{''.join(map(str, headers))}]"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{header_text}{root.get('name', '')}"
         sep = separators[0]
         command_string = (cmd or root["name"]) + sep
-        return f"\n{command_string}%s{help_string}{usage}%s{example}"
-
-    def part(self, node: Union[Subcommand, Option]) -> str:
-        ...
+        return f"\n{command_string}%s{help_string}{usage}\n%s{example}"
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         options = []
         opt_description = []
         max_len = 1
         for opt in filter(
             lambda x: isinstance(x, Option) and (x.name not in self.ignore_names or not x.nargs), parts
@@ -98,68 +98,71 @@
             max_len = max(max(map(lambda x: len(x), subcommands)), max_len)
         option_string = "\n".join(
             f"{i.ljust(max_len)}    {j}" for i, j in zip(options, opt_description)
         )
         subcommand_string = "\n".join(
             f"{i.ljust(max_len)}    {j}" for i, j in zip(subcommands, sub_description)
         )
-        option_help = "选项:\n" if option_string else ""
-        subcommand_help = "子命令:\n" if subcommand_string else ""
+        option_help = f"{lang.require('tools', 'format.ap.opt')}:\n" if option_string else ""
+        subcommand_help = f"{lang.require('tools', 'format.ap.sub')}:\n" if subcommand_string else ""
         return f"{subcommand_help}{subcommand_string}\n{option_help}{option_string}\n"
 
 
 class MarkdownTextFormatter(TextFormatter):
     def format(self, trace: Trace) -> str:
         """help text的生成入口"""
         """头部节点的描述"""
         root, separators = trace.head, trace.separators
         params, notice = self.parameters(trace.args)
-        notice_text = ("### 注释:\n```\n" + "\n".join(notice) + "\n```") if notice else ""
+        notice_text = (
+            f"### {lang.require('format', 'notice')}:\n```\n" + "\n".join(notice) + "\n```"
+        ) if notice else ""
         help_string = f"{desc}" if (desc := root.get("description")) else ""
         usage = f"\n{usage}" if (usage := root.get("usage")) else ""
         example = (
-            f"\n## 使用示例:\n```shell\n{example}\n```"
+            f"\n## {lang.require('format', 'example')}:\n```shell\n{example}\n```"
             if (example := root.get("example"))
             else ""
         )
 
         headers = (
             f"&#91;{''.join(map(str, headers))}&#93;"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{headers}{root.get('name', '')}"
         command_string = (cmd or root["name"]) + (
             tuple(separators)[0] if params else ""
         )
         body = self.body(trace.body)
-
         return (
             f"## {help_string}\n\n"
-            f"指令: \n\n"
+            f"{lang.require('tools', 'format.md.title')}: \n\n"
             f"**{command_string}{params}**\n"
             f"{notice_text}"
             f"{usage}\n\n"
             f"{body}"
             f"{example}"
         )
 
     def param(self, parameter: Arg) -> str:
         """对单个参数的描述"""
         name = parameter.name
+        if str(parameter.value).strip("'\"") == name:
+            return f"&#91;{name}&#93;" if parameter.optional else name
+        if parameter.hidden:
+            return f"&#91;{name}&#93;" if parameter.optional else f"&lt;{name}&gt;"
+        if parameter.value is AllParam:
+            return f"&lt;...{name}&gt;"
         arg = f"&#91;{name}" if parameter.optional else f"&lt;{name}"
-        if not parameter.hidden:
-            if parameter.value is AllParam:
-                return f"&lt;...{name}&gt;"
-            if not isinstance(parameter.value, BasePattern) or parameter.value.pattern != name:
-                arg += f":{parameter.value}"
-            if parameter.field.display is Empty:
-                arg += " = None"
-            elif parameter.field.display is not None:
-                arg += f" = {parameter.field.display} "
+        arg += f": {parameter.value}"
+        if parameter.field.display is Empty:
+            arg += " = None"
+        elif parameter.field.display is not None:
+            arg += f" = {parameter.field.display}"
         return f"{arg}&#93;" if parameter.optional else f"{arg}&gt;"
 
     def parameters(self, args: Args) -> Tuple[str, Optional[List[str]]]:
         """参数列表的描述"""
         res = ""
         for arg in args.argument:
             if arg.name.startswith('_key_'):
@@ -168,68 +171,77 @@
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
         return (res[:-1], [f"{v[0]}: {v[1]}" for v in notice]) if notice else (res[:-1], None)
 
-    def part(self, node: Union[Subcommand, Option]) -> str:
-        """每个子节点的描述"""
-        if isinstance(node, Subcommand):
-            name = " ".join(node.requires) + (" " if node.requires else "") + node.name
-            option_string = "\n".join(self.part(i) for i in node.options)
-            option_help = "### 该子命令内可用的选项有:\n " if option_string else ""
-            param, notice = self.parameters(node.args)
-            help_text = "> Unknown" if node.help_text == node.dest else f"> {node.help_text}"
-            notice_text = (
-                (f"\n>\n> #### 注释:\n> " + "\n> ".join(notice)) if notice else ""
-            )
-            return (
-                f"- **{name + (tuple(node.separators)[0] if param else '')}"
-                f"{param}**\n"
-                f"{help_text}"
-                f"{notice_text}\n"
-                f"{option_help}{option_string}"
+    def opt(self, node: Option) -> str:
+        alias_text = (
+            " ".join(node.requires)
+            + (" " if node.requires else "")
+            + (
+                f"&#91;{'|'.join(node.aliases)}&#93;"
+                if len(node.aliases) >= 2
+                else node.name
             )
-        elif isinstance(node, Option):
-            alias_text = (
-                " ".join(node.requires)
-                + (" " if node.requires else "")
-                + (
-                    f"&#91;{'|'.join(node.aliases)}&#93;"
-                    if len(node.aliases) >= 2
-                    else "".join(node.aliases)
-                )
-            )
-            help_text = "> Unknown" if node.help_text == node.dest else f"> {node.help_text}"
-            param, notice = self.parameters(node.args)
-            notice_text = (
-                (f"\n>\n> #### 注释:\n> " + "\n> ".join(notice)) if notice else ""
-            )
-            return (
-                f"- **{alias_text + (tuple(node.separators)[0] if param else '')}"
-                f"{param.strip(' ')}**\n"
-                f"{help_text}"
-                f"{notice_text}\n"
-            )
-        else:
-            raise TypeError(f"{node} is not a valid node")
+        )
+        help_text = "> Unknown" if node.help_text == node.dest else f"> {node.help_text}"
+        param, notice = self.parameters(node.args)
+        notice_text = (
+            (f"\n>\n> #### {lang.require('format', 'notice')}:\n> " + "\n> ".join(notice)) if notice else ""
+        )
+        return (
+            f"- **{alias_text + (tuple(node.separators)[0] if param else '')}"
+            f"{param.strip(' ')}**\n"
+            f"{help_text}"
+            f"{notice_text}\n"
+        )
+
+    def sub(self, node: Subcommand) -> str:
+        """对单个子命令的描述"""
+        name = " ".join(node.requires) + (" " if node.requires else "") + node.name
+        opt_string = "\n".join(
+            [self.opt(opt) for opt in filter(lambda x: isinstance(x, Option), node.options)]
+        )
+        sub_string = "".join(
+            [
+                self.opt(sub) # type: ignore
+                for sub in filter(lambda x: isinstance(x, Subcommand), node.options)
+            ]
+        )
+        opt_help = f"### {lang.require('format', 'subcommands.opts')}:\n" if opt_string else ""
+        sub_help = f"### {lang.require('format', 'subcommands.subs')}:\n" if sub_string else ""
+        param, notice = self.parameters(node.args)
+        help_text = "> Unknown" if node.help_text == node.dest else f"> {node.help_text}"
+        notice_text = (
+            (f"\n>\n> #### {lang.require('format', 'notice')}:\n> " + "\n> ".join(notice)) if notice else ""
+        )
+        return (
+            f"- **{name + (tuple(node.separators)[0] if param else '')}"
+            f"{param}**\n"
+            f"{help_text}"
+            f"{notice_text}\n"
+            f"{sub_help}{sub_string}"
+            f"{opt_help}{opt_string}"
+        )
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         """子节点列表的描述"""
         option_string = "\n".join(
-            self.part(opt)
-            for opt in filter(lambda x: isinstance(x, Option), parts)
-            if opt.name not in self.ignore_names
+            [
+                self.opt(opt) for opt in filter(lambda x: isinstance(x, Option), parts)
+                if opt.name not in self.ignore_names
+            ]
         )
         subcommand_string = "\n".join(
-            self.part(sub) for sub in filter(lambda x: isinstance(x, Subcommand), parts)
+            [self.sub(sub) for sub in filter(lambda x: isinstance(x, Subcommand), parts)]
         )
-        option_help = "## 可用的选项有:\n" if option_string else ""
-        subcommand_help = "## 可用的子命令有:\n" if subcommand_string else ""
+        option_help = f"## {lang.require('format', 'options')}:\n" if option_string else ""
+        subcommand_help = f"## {lang.require('format', 'subcommands')}:\n" if subcommand_string else ""
         return f"{subcommand_help}{subcommand_string}{option_help}{option_string}"
 
 
 color_theme = {
     "msg": ("magenta", "35"),
     "warn": ("yellow", "33"),
     "info": ("blue", "34"),
@@ -253,25 +265,31 @@
         return f"[{color_theme[style][0]}]{content}[/]"
     def format(self, trace: Trace) -> str:
         parts = trace.body  # type: ignore
         sub_names = [i.name for i in filter(lambda x: isinstance(x, Subcommand), parts)]
         opt_names = [min(i.aliases, key=len) for i in filter(lambda x: isinstance(x, Option), parts)]
         sub_names = self._convert(f"{{{','.join(sub_names)}}}\n", "info") if sub_names else ""
         opt_names = self._convert((" ".join(f"[{i}]" for i in opt_names)), 'info') if opt_names else ""
-        topic = f"{self._convert('命令:', 'warn')} {self._convert(trace.head['name'], 'msg')} {opt_names}\n {sub_names}"
+        title = f"{lang.require('tools', 'format.ap.title')}:"
+        topic = f"{self._convert(title, 'warn')} {self._convert(trace.head['name'], 'msg')} {opt_names}\n {sub_names}"
         header = self.header(trace.head, trace.separators)
         param = self._convert(self.parameters(trace.args), "success")
         body = self.body(parts)
         return f"{topic}{header % (param, body)}"
 
     def param(self, parameter: Arg) -> str:
         name = parameter.name
-        arg = f"[{name.upper()}" if parameter.optional else name.upper()
+        if str(parameter.value).strip("'\"") == name:
+            return f"[{name}]" if parameter.optional else name
+        if parameter.hidden:
+            return f"[{name.upper()}]" if parameter.optional else name.upper()
         if parameter.value is AllParam:
             return f"{name.upper()}..."
+        arg = f"[{name.upper()}" if parameter.optional else name.upper()
+        arg += f":{parameter.value}"
         if parameter.field.display is Empty:
             arg += "=None"
         elif parameter.field.display is not None:
             arg += f"={parameter.field.display}"
         return f"{arg}]" if parameter.optional else arg
 
     def parameters(self, args: Args) -> str:
@@ -281,29 +299,34 @@
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        return f"{res}\n  内容:\n  " + "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
+        return f"{res}\n  {lang.require('tools', 'format.ap.notice')}:\n  " + \
+            "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
+
 
     def header(self, root: Dict[str, Any], separators: Tuple[str, ...]) -> str:
-        help_string = f"\n{self._convert('描述:', 'warn')} {desc}\n" if (desc := root.get("description")) else ""
-        usage = f"\n{self._convert('用法:', 'warn')} {usage}\n" if (usage := root.get("usage")) else ""
-        example = f"\n{self._convert('样例:', 'warn')} {example}\n" if (example := root.get("example")) else ""
+        _desc = f"{lang.require('tools', 'format.ap.desc')}:"
+        _usage = f"{lang.require('tools', 'format.ap.usage')}:"
+        _example = f"{lang.require('tools', 'format.ap.example')}:"
+        help_string = f"\n{self._convert(_desc, 'warn')} {desc}\n" if (desc := root.get("description")) else ""
+        usage = f"\n{self._convert(_usage, 'warn')} {usage}\n" if (usage := root.get("usage")) else ""
+        example = f"\n{self._convert(_example, 'warn')} {example}\n" if (example := root.get("example")) else ""
         header_text = (
             f"[{''.join(map(str, headers))}]"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{header_text}{root.get('name', '')}"
         sep = separators[0]
         command_string = self._convert((cmd or root["name"]) + sep, "success")
-        return f"\n{command_string}%s{help_string}{usage}%s{example}"
+        return f"\n{command_string}%s{help_string}{usage}\n%s{example}"
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         options = []
         opt_description = []
         max_len = 1
         for opt in filter(
             lambda x: isinstance(x, Option) and (x.name not in self.ignore_names or not x.nargs), parts
@@ -338,16 +361,18 @@
             max_len = max(max(map(lambda x: len(x), subcommands)), max_len)
         option_string = "\n".join(
             f"{i.ljust(max_len)}    {j}" for i, j in zip(options, opt_description)
         )
         subcommand_string = "\n".join(
             f"{i.ljust(max_len)}    {j}" for i, j in zip(subcommands, sub_description)
         )
-        option_help = f"{self._convert('选项:', 'warn')}\n" if option_string else ""
-        subcommand_help = f"{self._convert('子命令:', 'warn')}\n" if subcommand_string else ""
+        _opt = f"{lang.require('tools', 'format.ap.opt')}:"
+        _sub = f"{lang.require('tools', 'format.ap.sub')}:"
+        option_help = f"{self._convert(_opt, 'warn')}\n" if option_string else ""
+        subcommand_help = f"{self._convert(_sub, 'warn')}\n" if subcommand_string else ""
         return f"{subcommand_help}{subcommand_string}\n{option_help}{option_string}\n"
 
 class RichTextFormatter(_RichTextFormatter):
     """argparser 风格的帮助文本格式化器, 增加 rich 的颜色标记，可用 rich.console 打印"""
     csl_code = False
 
 class RichConsoleFormatter(_RichTextFormatter):
```

### Comparing `arclet-alconna-tools-0.5.0/src/arclet/alconna/tools/pattern.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/pattern.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 from arclet.alconna import Args, config
 from nepattern import (
     BasePattern,
     Empty,
     MatchFailed,
     PatternModel,
-    lang,
-    pattern_map,
-    set_converter,
+    all_patterns,
 )
-
+from nepattern.context import global_patterns
+from tarina import lang
 from .debug import analyse_args
 
 TOrigin = TypeVar("TOrigin")
 
 
 class ObjectPattern(BasePattern):
     def __init__(
@@ -24,33 +23,34 @@
         origin: Type[TOrigin],
         limit: Tuple[str, ...] = (),
         flag: Literal["urlget", "part", "json", "space"] = "part",
         **suppliers: Callable,
     ):
         self._args = Args()
         self._names = []
+        pmap = all_patterns()
         for param in inspect.signature(origin.__init__).parameters.values():
             name = param.name
             anno = param.annotation
             default = param.default
             if name in ("self", "cls"):
                 continue
             if limit and name not in limit:
                 continue
             if param.kind in (
                 inspect.Parameter.VAR_POSITIONAL,
                 inspect.Parameter.VAR_KEYWORD,
             ):
                 continue
             if anno is Empty:
-                anno = pattern_map[str]
+                anno = pmap[str]
             elif inspect.isclass(anno) and issubclass(anno, str):
-                anno = pattern_map[str]
+                anno = pmap[str]
             elif inspect.isclass(anno) and issubclass(anno, int):
-                anno = pattern_map[int]
+                anno = pmap[int]
             if name in suppliers and inspect.isclass(anno):
                 _s_sig = inspect.signature(suppliers[name])
                 if len(_s_sig.parameters) == 1 or (
                     len(_s_sig.parameters) == 2 and inspect.ismethod(suppliers[name])
                 ):
                     anno = BasePattern(
                         model=PatternModel.TYPE_CONVERT,
@@ -89,25 +89,28 @@
                 + "}"
             )
         else:
             raise TypeError(config.lang.types_type_error.format(target=flag))
         super().__init__(
             model=PatternModel.TYPE_CONVERT, origin=origin, alias=origin.__name__
         )
-        set_converter(self)
+        global_patterns().set(self)
 
     def match(self, input_: Union[str, Any]) -> TOrigin:
         if isinstance(input_, self.origin):
             return input_  # type: ignore
         elif not isinstance(input_, str):
-            raise MatchFailed(lang.type_error.format(target=input_.__class__))
+            raise MatchFailed(lang.require("nepattern", "type_error").format(target=input_.__class__))
         if not (mat := self._re_pattern.fullmatch(input_)):
-            raise MatchFailed(lang.content_error.format(target=input_))
+            raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_))
         if res := analyse_args(
             self._args, list(mat.groupdict().values()), raise_exception=False
         ):
             return self.origin(**res)
         else:
-            raise MatchFailed(lang.content_error.format(target=input_))
+            raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_))
+
+    def __call__(self, *args, **kwargs):
+        return self.origin(*args, **kwargs)
 
     def __eq__(self, other):
         return isinstance(other, ObjectPattern) and self.origin == other.origin
```

