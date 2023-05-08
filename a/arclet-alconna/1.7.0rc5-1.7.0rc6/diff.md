# Comparing `tmp/arclet-alconna-1.7.0rc5.tar.gz` & `tmp/arclet-alconna-1.7.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc5.tar", last modified: Mon May  8 11:30:12 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.0rc6.tar", last modified: Mon May  8 16:34:17 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc5.tar` & `arclet-alconna-1.7.0rc6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc5/LICENSE
--rw-r--r--   0        0        0     2813 2023-05-07 16:32:54.439874 arclet-alconna-1.7.0rc5/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-08 08:04:29.409891 arclet-alconna-1.7.0rc5/README-EN.md
--rw-r--r--   0        0        0     1087 2023-05-08 11:29:49.426377 arclet-alconna-1.7.0rc5/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 16:29:22.798529 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    18070 2023-05-08 06:36:38.138006 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8361 2023-05-07 16:29:22.799529 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    22923 2023-05-08 08:02:25.512945 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     7811 2023-05-08 06:38:21.959747 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-07 16:29:22.801529 arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1785 2023-05-08 05:11:19.754526 arclet-alconna-1.7.0rc5/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14478 2023-05-08 06:44:47.137906 arclet-alconna-1.7.0rc5/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1243 2023-05-07 16:29:22.804526 arclet-alconna-1.7.0rc5/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15913 2023-05-07 16:32:41.201286 arclet-alconna-1.7.0rc5/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    12902 2023-05-08 05:22:02.753182 arclet-alconna-1.7.0rc5/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-08 06:44:58.844442 arclet-alconna-1.7.0rc5/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4868 2023-05-08 06:45:27.372580 arclet-alconna-1.7.0rc5/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4470 2023-05-07 16:32:44.799782 arclet-alconna-1.7.0rc5/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14715 2023-05-07 16:32:45.542456 arclet-alconna-1.7.0rc5/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2615 2023-05-07 16:32:47.490076 arclet-alconna-1.7.0rc5/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1070 2023-05-07 16:32:49.003053 arclet-alconna-1.7.0rc5/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11256 2023-05-07 16:32:49.488876 arclet-alconna-1.7.0rc5/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-07 16:29:22.812601 arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3565 2023-05-07 16:29:22.813522 arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3602 2023-05-07 16:29:22.813850 arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    16838 2023-05-08 06:47:44.520450 arclet-alconna-1.7.0rc5/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1430 2023-05-07 16:32:50.831111 arclet-alconna-1.7.0rc5/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-07 16:32:51.478127 arclet-alconna-1.7.0rc5/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-07 16:32:52.687122 arclet-alconna-1.7.0rc5/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-07 16:29:22.816522 arclet-alconna-1.7.0rc5/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5813 2023-05-07 16:32:58.355410 arclet-alconna-1.7.0rc5/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3584 2023-05-07 16:32:58.778521 arclet-alconna-1.7.0rc5/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3254 2023-05-08 06:48:40.755418 arclet-alconna-1.7.0rc5/tests/analyser_test.py
--rw-r--r--   0        0        0     7223 2023-05-07 16:29:22.820523 arclet-alconna-1.7.0rc5/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-07 16:32:42.508980 arclet-alconna-1.7.0rc5/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-08 06:49:11.411375 arclet-alconna-1.7.0rc5/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-07 16:29:22.822522 arclet-alconna-1.7.0rc5/tests/config_test.py
--rw-r--r--   0        0        0    23213 2023-05-08 06:49:45.049528 arclet-alconna-1.7.0rc5/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-07 16:29:22.823526 arclet-alconna-1.7.0rc5/tests/util_test.py
--rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc6/LICENSE
+-rw-r--r--   0        0        0     2813 2023-05-07 16:32:54.439874 arclet-alconna-1.7.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-08 08:04:29.409891 arclet-alconna-1.7.0rc6/README-EN.md
+-rw-r--r--   0        0        0     1087 2023-05-08 16:32:38.530616 arclet-alconna-1.7.0rc6/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:29:22.798529 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    18070 2023-05-08 06:36:38.138006 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8361 2023-05-07 16:29:22.799529 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    22923 2023-05-08 08:02:25.512945 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     7811 2023-05-08 06:38:21.959747 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-07 16:29:22.801529 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1785 2023-05-08 05:11:19.754526 arclet-alconna-1.7.0rc6/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14478 2023-05-08 06:44:47.137906 arclet-alconna-1.7.0rc6/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1243 2023-05-07 16:29:22.804526 arclet-alconna-1.7.0rc6/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15913 2023-05-07 16:32:41.201286 arclet-alconna-1.7.0rc6/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    12902 2023-05-08 05:22:02.753182 arclet-alconna-1.7.0rc6/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-08 06:44:58.844442 arclet-alconna-1.7.0rc6/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4868 2023-05-08 06:45:27.372580 arclet-alconna-1.7.0rc6/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4463 2023-05-08 15:45:12.657524 arclet-alconna-1.7.0rc6/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14858 2023-05-08 12:05:48.939938 arclet-alconna-1.7.0rc6/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2615 2023-05-07 16:32:47.490076 arclet-alconna-1.7.0rc6/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1070 2023-05-07 16:32:49.003053 arclet-alconna-1.7.0rc6/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11252 2023-05-08 16:28:22.675096 arclet-alconna-1.7.0rc6/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-07 16:29:22.812601 arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3565 2023-05-07 16:29:22.813522 arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3602 2023-05-07 16:29:22.813850 arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    16838 2023-05-08 06:47:44.520450 arclet-alconna-1.7.0rc6/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1430 2023-05-07 16:32:50.831111 arclet-alconna-1.7.0rc6/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-07 16:32:51.478127 arclet-alconna-1.7.0rc6/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-07 16:32:52.687122 arclet-alconna-1.7.0rc6/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:29:22.816522 arclet-alconna-1.7.0rc6/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5813 2023-05-07 16:32:58.355410 arclet-alconna-1.7.0rc6/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3584 2023-05-07 16:32:58.778521 arclet-alconna-1.7.0rc6/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3254 2023-05-08 06:48:40.755418 arclet-alconna-1.7.0rc6/tests/analyser_test.py
+-rw-r--r--   0        0        0     7223 2023-05-07 16:29:22.820523 arclet-alconna-1.7.0rc6/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-07 16:32:42.508980 arclet-alconna-1.7.0rc6/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-08 06:49:11.411375 arclet-alconna-1.7.0rc6/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-07 16:29:22.822522 arclet-alconna-1.7.0rc6/tests/config_test.py
+-rw-r--r--   0        0        0    23213 2023-05-08 06:49:45.049528 arclet-alconna-1.7.0rc6/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-07 16:29:22.823526 arclet-alconna-1.7.0rc6/tests/util_test.py
+-rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc6/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc5/LICENSE` & `arclet-alconna-1.7.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/pyproject.toml` & `arclet-alconna-1.7.0rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc5"
+version = "1.7.0rc6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.0rc5/README-EN.md` & `arclet-alconna-1.7.0rc6/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.0rc5"
+__version__ = "1.7.0rc6"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_analyser.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_handlers.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/action.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/args.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/args.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/arparma.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/base.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/config.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """默认是否抛出异常"""
     enable_message_cache: bool = field(default=True)
     """默认是否启用消息缓存"""
     builtin_option_name: OptionNames = field(
         default_factory=lambda: {
             "help": {"--help", "-h"},
             "shortcut": {"--shortcut", "-sct"},
-            "completion": {"--comp", "-cp", "?", "？"},
+            "completion": {"--comp", "-cp", "?"},
         }
     )
     """默认的内置选项名称"""
     to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
     """默认的选项转文本函数"""
     checker: Callable[[Any], bool] | None = field(default=None)
     """默认的传入命令检查"""
```

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/core.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,16 @@
                 self.command = ""
             else:
                 path = Path(sys.argv[0])
                 self.command = path.parent.stem if str(path.parent) not in (".", "/", "\\") else path.stem
         self.namespace = ns_config.name
         self.formatter = (formatter_type or ns_config.formatter_type or TextFormatter)()
         self.meta = meta or CommandMeta()
+        if self.meta.example:
+            self.meta.example = self.meta.example.replace("$", str(self.prefixes[0]) if self.prefixes else "")
         self.meta.fuzzy_match = self.meta.fuzzy_match or ns_config.fuzzy_match
         self.meta.raise_exception = self.meta.raise_exception or ns_config.raise_exception
         self.meta.compact = self.meta.compact or ns_config.compact
         options = [i for i in args if isinstance(i, (Option, Subcommand))]
         options.append(
             Option("|".join(ns_config.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
         )
```

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,15 @@
         return self
 
     def remove(self, base: Alconna | str):
         """移除目标命令"""
         if isinstance(base, str):
             self.data.pop(base)
         else:
-            with suppress(ValueError):
-                self.data.get(base.path, []).remove(base)
+            self.data.pop(base.path)
 
     def format_node(self, parts: list | None = None):
         """格式化命令节点
 
         Args:
             parts (list | None, optional): 可能的节点路径.
         """
@@ -179,24 +178,26 @@
     def param(self, parameter: Arg) -> str:
         """对单个参数的描述
 
         Args:
             parameter (Arg): 参数单元
         """
         name = parameter.name
+        if str(parameter.value).strip("'\"") == name:
+            return f"[{name}]" if parameter.optional else name
+        if parameter.hidden:
+            return f"[{name}]" if parameter.optional else f"<{name}>"
+        if parameter.value is AllParam:
+            return f"<...{name}>"
         arg = f"[{name}" if parameter.optional else f"<{name}"
-        if not parameter.hidden:
-            if parameter.value is AllParam:
-                return f"<...{name}>"
-            if not isinstance(parameter.value, BasePattern) or parameter.value.pattern != name:
-                arg += f": {parameter.value}"
-            if parameter.field.display is Empty:
-                arg += " = None"
-            elif parameter.field.display is not None:
-                arg += f" = {parameter.field.display}"
+        arg += f": {parameter.value}"
+        if parameter.field.display is Empty:
+            arg += " = None"
+        elif parameter.field.display is not None:
+            arg += f" = {parameter.field.display}"
         return f"{arg}]" if parameter.optional else f"{arg}>"
 
     def parameters(self, args: Args) -> str:
         """参数列表的描述
 
         Args:
             args (Args): 参数列表
```

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/manager.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/model.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/output.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.0rc6/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/tests/analyser_test.py` & `arclet-alconna-1.7.0rc6/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/tests/args_test.py` & `arclet-alconna-1.7.0rc6/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/tests/base_test.py` & `arclet-alconna-1.7.0rc6/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/tests/components_test.py` & `arclet-alconna-1.7.0rc6/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/tests/config_test.py` & `arclet-alconna-1.7.0rc6/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/tests/core_test.py` & `arclet-alconna-1.7.0rc6/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc5/PKG-INFO` & `arclet-alconna-1.7.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc5
+Version: 1.7.0rc6
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

