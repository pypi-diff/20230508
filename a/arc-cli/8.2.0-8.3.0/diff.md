# Comparing `tmp/arc_cli-8.2.0.tar.gz` & `tmp/arc_cli-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.2.0.tar", max compression
+gzip compressed data, was "arc_cli-8.3.0.tar", max compression
```

## Comparing `arc_cli-8.2.0.tar` & `arc_cli-8.3.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0      944 2023-04-24 02:20:30.375199 arc_cli-8.2.0/README.md
--rw-r--r--   0        0        0      719 2023-05-04 02:59:16.987114 arc_cli-8.2.0/arc/__init__.py
--rw-r--r--   0        0        0     1449 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/api.py
--rw-r--r--   0        0        0     6902 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/autocompletions.py
--rw-r--r--   0        0        0     2189 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/autoload.py
--rw-r--r--   0        0        0      114 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/color.py
--rw-r--r--   0        0        0     5732 2023-05-04 02:54:46.601724 arc_cli-8.2.0/arc/config.py
--rw-r--r--   0        0        0      385 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/constants.py
--rw-r--r--   0        0        0      121 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/__init__.py
--rw-r--r--   0        0        0     1379 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/alias.py
--rw-r--r--   0        0        0     1768 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/classful.py
--rw-r--r--   0        0        0    17181 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/command.py
--rw-r--r--   0        0        0     3118 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/documentation.py
--rw-r--r--   0        0        0      219 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/param/__init__.py
--rw-r--r--   0        0        0     8036 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/param/constructors.py
--rw-r--r--   0        0        0     3499 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/groups.py
--rw-r--r--   0        0        0     8706 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param.py
--rw-r--r--   0        0        0     8549 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param_definition.py
--rw-r--r--   0        0        0     3388 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param_mixin.py
--rw-r--r--   0        0        0     1889 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param_tree.py
--rw-r--r--   0        0        0     6314 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/errors.py
--rw-r--r--   0        0        0     1070 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/logging.py
--rw-r--r--   0        0        0    16336 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/parser.py
--rw-r--r--   0        0        0      402 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/__init__.py
--rw-r--r--   0        0        0     6168 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/ansi.py
--rw-r--r--   0        0        0     4681 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/box.py
--rw-r--r--   0        0        0     5319 2023-05-04 02:58:09.317495 arc_cli-8.2.0/arc/present/console.py
--rw-r--r--   0        0        0      187 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/data.py
--rw-r--r--   0        0        0     2126 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/drawing.py
--rw-r--r--   0        0        0     2748 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/formatters.py
--rw-r--r--   0        0        0     9078 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/help_formatter.py
--rw-r--r--   0        0        0     3024 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/joiner.py
--rw-r--r--   0        0        0       54 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/markdown/__init__.py
--rw-r--r--   0        0        0     6614 2023-05-04 02:56:40.521271 arc_cli-8.2.0/arc/present/markdown/markdown_parser.py
--rw-r--r--   0        0        0     3894 2023-05-04 02:54:24.375128 arc_cli-8.2.0/arc/present/markdown/nodes.py
--rw-r--r--   0        0        0     1632 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/out.py
--rw-r--r--   0        0        0      987 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/pager.py
--rw-r--r--   0        0        0     9825 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/table.py
--rw-r--r--   0        0        0     5182 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/wrap.py
--rw-r--r--   0        0        0      288 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/prompt/__init__.py
--rw-r--r--   0        0        0     3722 2023-04-30 19:31:15.828580 arc_cli-8.2.0/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5926 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/prompt/prompt.py
--rw-r--r--   0        0        0      812 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/prompt/prompts.py
--rw-r--r--   0        0        0     7019 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/prompt/questions.py
--rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.2.0/arc/py.typed
--rw-r--r--   0        0        0      306 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/__init__.py
--rw-r--r--   0        0        0     2970 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/app.py
--rw-r--r--   0        0        0     2678 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/context.py
--rw-r--r--   0        0        0    12517 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/exec.py
--rw-r--r--   0        0        0     8240 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/init.py
--rw-r--r--   0        0        0     7402 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/middleware.py
--rw-r--r--   0        0        0      382 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/safe.py
--rw-r--r--   0        0        0     1866 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/suggest.py
--rw-r--r--   0        0        0      362 2023-04-30 19:42:21.213131 arc_cli-8.2.0/arc/types/__init__.py
--rw-r--r--   0        0        0    13898 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/aliases.py
--rw-r--r--   0        0        0      670 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/convert.py
--rw-r--r--   0        0        0      545 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/default.py
--rw-r--r--   0        0        0     4422 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/file.py
--rw-r--r--   0        0        0       79 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/__init__.py
--rw-r--r--   0        0        0     1403 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/observers.py
--rw-r--r--   0        0        0     2630 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/transformers.py
--rw-r--r--   0        0        0     4042 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/validators.py
--rw-r--r--   0        0        0     3486 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/network.py
--rw-r--r--   0        0        0      854 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/numbers.py
--rw-r--r--   0        0        0      860 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/path.py
--rw-r--r--   0        0        0     6881 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/semver.py
--rw-r--r--   0        0        0      877 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/state.py
--rw-r--r--   0        0        0     1921 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/strings.py
--rw-r--r--   0        0        0     2155 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/type_arg.py
--rw-r--r--   0        0        0     2718 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/type_info.py
--rw-r--r--   0        0        0     3176 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/users.py
--rw-r--r--   0        0        0     2257 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/typing.py
--rw-r--r--   0        0        0     1021 2023-05-04 02:59:17.663776 arc_cli-8.2.0/pyproject.toml
--rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 arc_cli-8.2.0/setup.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 arc_cli-8.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-05-04 03:31:42.938647 arc_cli-8.3.0/README.md
+-rw-r--r--   0        0        0      737 2023-05-08 17:17:44.700548 arc_cli-8.3.0/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-05-04 03:31:42.938647 arc_cli-8.3.0/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-05-04 03:31:42.938647 arc_cli-8.3.0/arc/autocompletions.py
+-rw-r--r--   0        0        0     2189 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/autoload.py
+-rw-r--r--   0        0        0      114 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/color.py
+-rw-r--r--   0        0        0     6534 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/config.py
+-rw-r--r--   0        0        0      385 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/classful.py
+-rw-r--r--   0        0        0    16932 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/define/command.py
+-rw-r--r--   0        0        0     3101 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3499 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8706 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/box.py
+-rw-r--r--   0        0        0     5319 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/formatters.py
+-rw-r--r--   0        0        0     9376 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6614 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3894 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3722 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7019 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/py.typed
+-rw-r--r--   0        0        0      304 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/app.py
+-rw-r--r--   0        0        0     2678 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/runtime/context.py
+-rw-r--r--   0        0        0    12517 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/runtime/exec.py
+-rw-r--r--   0        0        0     8933 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/init.py
+-rw-r--r--   0        0        0     7409 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/middleware.py
+-rw-r--r--   0        0        0     3097 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/plugin.py
+-rw-r--r--   0        0        0      382 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/suggest.py
+-rw-r--r--   0        0        0      362 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/types/__init__.py
+-rw-r--r--   0        0        0    13898 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/convert.py
+-rw-r--r--   0        0        0      545 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/default.py
+-rw-r--r--   0        0        0     4422 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1403 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4042 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/state.py
+-rw-r--r--   0        0        0     1921 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/strings.py
+-rw-r--r--   0        0        0     2155 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-05-04 03:31:42.955314 arc_cli-8.3.0/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-05-04 03:31:42.955314 arc_cli-8.3.0/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-05-04 03:31:42.955314 arc_cli-8.3.0/arc/typing.py
+-rw-r--r--   0        0        0     1116 2023-05-08 17:17:45.363876 arc_cli-8.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 arc_cli-8.3.0/setup.py
+-rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 arc_cli-8.3.0/PKG-INFO
```

### Comparing `arc_cli-8.2.0/README.md` & `arc_cli-8.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 # ARC Features
 - Command line arguments based on python type hints
 - Arbitrary command nesting
 - Automatic `--help` documentation
 - Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...
 
-# [Docs](http://arc.seanrcollings.com)
+# Links
+- [Docs](https://arc.seancollings.dev)
+- [Playground](https://playground.arc.seancollings.dev)
+- [PyPi](https://pypi.org/project/arc-cli/)
+
 
 # Quick Start
 
 ```py
 import arc
 
 @arc.command
```

### Comparing `arc_cli-8.2.0/arc/__init__.py` & `arc_cli-8.3.0/arc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-__version__ = "8.2.0"
+__version__ = "8.3.0"
 
 from arc import types, prompt, present, errors
 from arc.config import (
     ColorConfig,
     Config,
     LinksConfig,
     SuggestionConfig,
     PresentConfig,
+    PluginConfig,
     configure,
 )
 from arc.constants import MISSING
 from arc.define import (
     Param,
     Argument,
     Command,
```

### Comparing `arc_cli-8.2.0/arc/api.py` & `arc_cli-8.3.0/arc/api.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/autocompletions.py` & `arc_cli-8.3.0/arc/autocompletions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/autoload.py` & `arc_cli-8.3.0/arc/autoload.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/config.py` & `arc_cli-8.3.0/arc/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import dataclass, field
 
 import arc.typing as at
 
+from arc.present.help_formatter import HelpFormatter, DefaultHelpFormatter
 from arc.color import fg
 from arc.prompt import Prompt
 
 if t.TYPE_CHECKING:
     from arc.types.semver import SemVer
     from arc import Context
 
@@ -22,42 +23,27 @@
 
     error: str = fg.RED
     highlight: str = fg.YELLOW
     accent: str = fg.ARC_BLUE
     subtle: str = fg.GREY
 
 
-# MarkdownFormat = t.Union[str, t.Callable[[str, "PresentConfig"], str]]
-
-
-# @dataclass
-# class MarkdownConfig:
-#     """Configures Markdown presentation for the application"""
-
-#     header: MarkdownFormat = nodes.Heading.default_format
-#     link: MarkdownFormat = nodes.Link.default_format
-
-#     def apply(self, fmt: MarkdownFormat, value: str, config: PresentConfig) -> str:
-#         if isinstance(fmt, str):
-#             return fmt.format(value)
-#         return fmt(value, config)
-
-
 @dataclass
 class PresentConfig:
     """Configures the presentation of the application"""
 
     indent: str = " " * 4
     """The indent to use for each level of indentation"""
     width: int = 80
     """The default width to present content at. This is used
     for wrapping text. Will be ignored if the terminal width is smaller"""
     color: ColorConfig = field(default_factory=ColorConfig)
     """The color configuration for the application"""
-    # md: MarkdownConfig = field(default_factory=MarkdownConfig)
+    formatter: type[HelpFormatter] = DefaultHelpFormatter
+    """Class to use when formatting help messages"""
 
 
 @dataclass
 class LinksConfig:
     """Configures Links for the application"""
 
     bug: str | None = None
@@ -69,14 +55,40 @@
 
     commands: bool = True
     params: bool = True
     distance: int = 2
 
 
 @dataclass
+class PluginConfig:
+    """Configures Plugins locations for the application"""
+
+    paths: list[str] = field(default_factory=list)
+    """List of paths to search for plugins. These paths will be searched
+    for python  modules that contain a `plugin` function. If the file does
+    not exist, or the function is not found, it will be ignored
+
+    The paths provided can be to a specific file, or a directory. If a directory
+    is provided, all files in that directory will be searched for plugins.
+    """
+
+    groups: list[str] = field(default_factory=lambda: ["arc.plugins"])
+    """List of entrypoint groups to search for plugins. The entrypoint's value must be
+    a callable that accepts a single argument, the `Context` object.
+
+    Defaults to using the `arc.plugins` entrypoint group
+    """
+
+    entrypoints: list[str] = field(default_factory=list)
+    """List of explicit entrypoints to search for plugins. The entrypoint's value must be
+    a callable that accepts a single argument, the `Context` object.
+    """
+
+
+@dataclass
 class Config:
     """arc's Config object. A single global instance
     of this class is created, then used where it is needed"""
 
     environment: at.Env = "production"
     transform_snake_case: bool = True
     env_prefix: str = ""
@@ -85,14 +97,15 @@
     allow_unrecognized_args: bool = False
     autoload_overwrite: bool = True
     debug: bool = False
     prompt: Prompt = field(default_factory=Prompt)
     suggest: SuggestionConfig = field(default_factory=SuggestionConfig)
     links: LinksConfig = field(default_factory=LinksConfig)
     present: PresentConfig = field(default_factory=PresentConfig)
+    plugins: PluginConfig = field(default_factory=PluginConfig)
 
     @classmethod
     def load(cls) -> "Config":
         """Access the Global `Config` instance"""
         global _config
 
         if not _config:
@@ -120,14 +133,15 @@
     prompt: Prompt | None = None,
     autocomplete: bool | None = None,
     allow_unrecognized_args: bool | None = None,
     autoload_overwrite: bool | None = None,
     debug: bool | None = None,
     links: LinksConfig | None = None,
     present: PresentConfig | None = None,
+    plugins: PluginConfig | None = None,
 ) -> None:
     """Function for updating global `arc` configuration
 
     Args:
         version (str | SemVer, optional): Version string to display with `--version`
 
         environment (str, optional): The current environment, either `production` or `development`.
@@ -171,11 +185,12 @@
         "prompt": prompt,
         "autocomplete": autocomplete,
         "allow_unrecognized_args": allow_unrecognized_args,
         "autoload_overwrite": autoload_overwrite,
         "debug": debug,
         "links": links,
         "present": present,
+        "plugins": plugins,
     }
 
     config = Config.load()
     config.update(**data)
```

### Comparing `arc_cli-8.2.0/arc/define/alias.py` & `arc_cli-8.3.0/arc/define/alias.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/classful.py` & `arc_cli-8.3.0/arc/define/classful.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/command.py` & `arc_cli-8.3.0/arc/define/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,65 +7,62 @@
 import typing as t
 
 import arc
 from arc.config import Config
 import arc.typing as at
 from arc import api, color, errors
 from arc.autocompletions import Completion, CompletionInfo, get_completions
-from arc.autoload import Autoload
 from arc.define import classful
 from arc.define.alias import AliasDict
 from arc.define.documentation import Documentation
 from arc.define.param import ParamMixin
 from arc.present.joiner import Join
-from arc.runtime import App, ExecMiddleware, MiddlewareContainer, MiddlewareStack
+from arc.runtime import App, ExecMiddleware, MiddlewareManager, MiddlewareStack
 from arc.runtime import Context
 
 if t.TYPE_CHECKING:
     from .param import ParamDefinition
 
 
-class Command(ParamMixin, MiddlewareContainer):
+class Command(ParamMixin, MiddlewareManager):
     name: str
     parent: Command | None
     config: Config
     subcommands: AliasDict[str, Command]
     param_def: ParamDefinition
     doc: Documentation
     explicit_name: bool
-    _autoload: bool
     data: dict[str, t.Any]
 
     def __init__(
         self,
         callback: at.CommandCallback,
+        config: Config,
         name: str | None = None,
         description: str | None = None,
-        config: Config | None = None,
         parent: Command | None = None,
         explicit_name: bool = True,
         autoload: bool = False,
         **kwargs: t.Any,
     ) -> None:
         ParamMixin.__init__(self)
-        MiddlewareContainer.__init__(self, [])
+        MiddlewareManager.__init__(self, [])
         if inspect.isclass(callback):
             self.callback = self.wrap_class_callback(
                 t.cast(type[at.ClassCallback], callback)
             )
         else:
             self.callback = callback
 
-        self.config = config or Config.load()
+        self.config = config
         self.name = name or callback.__name__
         self.parent = parent
         self.subcommands = AliasDict()
         self.doc = Documentation(self, self.config.present, description)
         self.explicit_name = explicit_name
-        self._autoload = autoload
         self.data = kwargs
 
     __repr__ = api.display("name")
 
     def __call__(
         self, input_args: at.InputArgs = None, state: dict[str, t.Any] = None
     ) -> t.Any:
@@ -217,15 +214,15 @@
             diff = datetime.now() - start_time
             ctx.logger.debug(f"Executing: {self} ({diff.total_seconds():.4f}s)")
         else:
             ctx.logger.debug(f"Executing: {self}")
 
         stack = MiddlewareStack()
         for command in self.command_chain:
-            stack.extend(command.stack)
+            stack.extend(command._stack)
 
         ctx = stack.start(ctx)
         if "arc.args" not in ctx:
             raise errors.InternalError(
                 "The command's arguments were not set during execution "
                 "(ctx['arc.args] is not set). This likely means there "
                 "is a problem with your middleware stack"
@@ -348,15 +345,15 @@
             )
 
         self.subcommands[command.name] = command
 
         if command.parent is None:
             command.parent = self
             for m in ExecMiddleware.all():
-                command.stack.try_remove(m)
+                command._stack.try_remove(m)
 
         if aliases:
             self.subcommands.add_aliases(command.name, *aliases)
 
         return command
 
     def add_commands(self, *commands: Command) -> list[Command]:
@@ -429,17 +426,14 @@
             return inner
 
         raise errors.ParamError(
             f"No parameter with name: {param_name}",
             Join.with_space(self.doc.fullname),
         )
 
-    def autoload(self, *paths: str) -> None:
-        Autoload(paths, self, self.config.autoload_overwrite).load()
-
     @staticmethod
     def wrap_class_callback(cls: type[at.ClassCallback]) -> at.CommandCallback:
         if not hasattr(cls, "handle"):
             raise errors.CommandError("class-style commands require a handle() method")
 
         def wrapper(**kwargs: t.Any) -> t.Any:
             inst = cls()
@@ -494,27 +488,24 @@
         config (Config | None, optional): Configuration object to apply
             to this command. If one is not provided, the default is used
     """
 
     name = None
 
     def inner(callback: at.CommandCallback) -> Command:
+        cmdconfig = config or Config.load()
         command_name = Command.get_canonical_subcommand_name(
-            callback,
-            name,
-            config.transform_snake_case
-            if config
-            else Config.load().transform_snake_case,
+            callback, name, cmdconfig.transform_snake_case
         )
 
         command = Command(
             callback=callback,
+            config=cmdconfig,
             name=command_name,
             description=desc,
-            config=config,
             parent=None,
             explicit_name=bool(name),
             autoload=True,
             **kwargs,
         )
         command.use(ExecMiddleware.all())
         return command
@@ -547,19 +538,21 @@
     Args:
         name (str): Name of the command
         desc (str | None, optional): Description for the command.
 
     Returns:
         command: A command object without a callback associated with it
     """
+    config = config or Config.load()
+
     command = Command(
         callback=namespace_callback,
+        config=config,
         name=name,
         description=desc,
-        config=config,
         parent=None,
         autoload=True,
         **kwargs,
     )
     command.use(ExecMiddleware.all())
     return command
```

### Comparing `arc_cli-8.2.0/arc/define/documentation.py` & `arc_cli-8.3.0/arc/define/documentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 import typing as t
 from functools import cached_property
 import textwrap
-from arc.config import PresentConfig
 
 import arc.typing as at
 from arc.define.param import param
-from arc.present.help_formatter import HelpFormatter
 
 if t.TYPE_CHECKING:
+    from arc.present.help_formatter import HelpFormatter
     from arc.define.command import Command
     from arc.config import PresentConfig
 
 ParamKinds = t.Literal["argument", "option", "flag"]
 
 KIND_MAPPING: dict[type[param.Param[t.Any]], ParamKinds] = {
     param.ArgumentParam: "argument",
@@ -40,19 +39,19 @@
     ):
         self.command = command
         self.config = config
         self._description = description
         self.docstring = self._get_docstring()
 
     def help(self) -> str:
-        formatter = HelpFormatter(self, self.config)
+        formatter = self.config.formatter(self, self.config)
         return formatter.format_help()
 
     def usage(self) -> str:
-        formatter = HelpFormatter(self, self.config)
+        formatter = self.config.formatter(self, self.config)
         return formatter.format_usage()
 
     @property
     def fullname(self) -> list[str]:
         return list(c.name for c in self.command.command_chain)[1:]
 
     @property
```

### Comparing `arc_cli-8.2.0/arc/define/param/constructors.py` & `arc_cli-8.3.0/arc/define/param/constructors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/param/groups.py` & `arc_cli-8.3.0/arc/define/param/groups.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/param/param.py` & `arc_cli-8.3.0/arc/define/param/param.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/param/param_definition.py` & `arc_cli-8.3.0/arc/define/param/param_definition.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/param/param_mixin.py` & `arc_cli-8.3.0/arc/define/param/param_mixin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/define/param/param_tree.py` & `arc_cli-8.3.0/arc/define/param/param_tree.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/errors.py` & `arc_cli-8.3.0/arc/errors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/logging.py` & `arc_cli-8.3.0/arc/logging.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/parser.py` & `arc_cli-8.3.0/arc/parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/ansi.py` & `arc_cli-8.3.0/arc/present/ansi.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/box.py` & `arc_cli-8.3.0/arc/present/box.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/console.py` & `arc_cli-8.3.0/arc/present/console.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/drawing.py` & `arc_cli-8.3.0/arc/present/drawing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/formatters.py` & `arc_cli-8.3.0/arc/present/formatters.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/help_formatter.py` & `arc_cli-8.3.0/arc/present/help_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,43 @@
 
 import textwrap
 import typing as t
 from itertools import repeat
 
 from arc import constants
 from arc.color import colorize, fx
-from arc.config import PresentConfig
 from arc.present.ansi import Ansi
 from arc.present.formatters import TextFormatter
 from arc.present.joiner import Join
 from arc.present.markdown import MarkdownParser
 
 if t.TYPE_CHECKING:
     from arc.define.command import Command
     from arc.define.documentation import Documentation, ParamDoc
+    from arc.config import PresentConfig
 
 
-class HelpFormatter(TextFormatter):
+class HelpFormatter(t.Protocol):
+    def __init__(
+        self,
+        doc: Documentation,
+        config: PresentConfig,
+        *args: t.Any,
+        **kwargs: t.Any,
+    ):
+        ...
+
+    def format_help(self) -> str:
+        ...
+
+    def format_usage(self) -> str:
+        ...
+
+
+class DefaultHelpFormatter(TextFormatter):
     _longest_intro: int = 0
 
     def __init__(
         self,
         doc: Documentation,
         config: PresentConfig,
         *args: t.Any,
```

### Comparing `arc_cli-8.2.0/arc/present/joiner.py` & `arc_cli-8.3.0/arc/present/joiner.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/markdown/markdown_parser.py` & `arc_cli-8.3.0/arc/present/markdown/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/markdown/nodes.py` & `arc_cli-8.3.0/arc/present/markdown/nodes.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/out.py` & `arc_cli-8.3.0/arc/present/out.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/pager.py` & `arc_cli-8.3.0/arc/present/pager.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/table.py` & `arc_cli-8.3.0/arc/present/table.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/present/wrap.py` & `arc_cli-8.3.0/arc/present/wrap.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/prompt/helpers.py` & `arc_cli-8.3.0/arc/prompt/helpers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/prompt/prompt.py` & `arc_cli-8.3.0/arc/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/prompt/prompts.py` & `arc_cli-8.3.0/arc/prompt/prompts.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/prompt/questions.py` & `arc_cli-8.3.0/arc/prompt/questions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/runtime/app.py` & `arc_cli-8.3.0/arc/runtime/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,57 +5,58 @@
 import typing as t
 
 import arc
 import arc.typing as at
 from arc import errors
 from arc.logging import WARNING, logger, mode_map, DEBUG
 from arc.runtime.init import InitMiddleware
-from arc.runtime.middleware import Middleware, MiddlewareContainer
-
+from arc.runtime.middleware import Middleware, MiddlewareManager
+from arc.runtime.plugin import PluginManager
 
 if t.TYPE_CHECKING:
     from arc.define import Command
 
 
-class App(MiddlewareContainer):
+class App(MiddlewareManager):
     def __init__(
         self,
         root: Command,
         init_middlewares: t.Sequence[Middleware] = None,
         state: dict[str, t.Any] = None,
         ctx: dict[str, t.Any] = None,
     ) -> None:
         super().__init__(init_middlewares or InitMiddleware.all())
         self.root = root
         self.provided_ctx = ctx or {}
         self.state = state or {}
         self.config = root.config
+        self.plugins = PluginManager()
 
     def __call__(self, input: at.InputArgs = None) -> t.Any:
         self._handle_dynamic_name()
         self._setup_logger()
         ctx = self._create_ctx({"arc.input": input})
         try:
             try:
-                ctx = self.stack.start(ctx)
+                ctx = self._stack.start(ctx)
                 if "arc.command" not in ctx:
                     raise errors.CommandError(
                         "The command was not decided upon during initialization "
                         "(ctx['arc.command'] is not set). This likely means there "
                         "is a problem with the middleware stack"
                     )
 
                 command: Command = ctx["arc.command"]
                 res = None
                 res = command.run(ctx)
             except Exception as e:
                 res = None
-                self.stack.throw(e)
+                self._stack.throw(e)
             else:
-                res = self.stack.close(res)
+                res = self._stack.close(res)
         except errors.ArcError as exc:
             if self.config.environment == "production":
                 arc.info(exc.fmt(ctx))
                 arc.exit(1)
 
             raise
         except errors.Exit as exc:
@@ -74,14 +75,15 @@
             {
                 "arc.root": self.root,
                 "arc.config": self.config,
                 "arc.errors": [],
                 "arc.app": self,
                 "arc.state": self.state,
                 "arc.logger": logger,
+                "arc.plugins": self.plugins,
             }
             | self.provided_ctx
             | (data or {})
         )
 
     def _handle_dynamic_name(self) -> None:
         if not self.root.explicit_name:
```

### Comparing `arc_cli-8.2.0/arc/runtime/context.py` & `arc_cli-8.3.0/arc/runtime/context.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/runtime/exec.py` & `arc_cli-8.3.0/arc/runtime/exec.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/runtime/init.py` & `arc_cli-8.3.0/arc/runtime/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Contains all of the middlewares used during initialization of a command"""
 from __future__ import annotations
+import typing as t
 from datetime import datetime
-
 import shlex
 import sys
-import typing as t
 
 from arc import autocompletions, errors
 from arc import typing as at
 from arc.define.param.param import FlagParam, OptionParam
 from arc.parser import CustomAutocompleteAction, CustomVersionAction, Parser
 from arc.runtime import Context
 from arc.runtime.middleware import (
@@ -42,14 +41,30 @@
         finally:
             end = datetime.now()
             ctx["arc.debug.end"] = end
             diff = end - start
             ctx.logger.debug(f"Execution took: {diff.total_seconds():.4f}s")
 
 
+class LoadPluginsMiddleware(MiddlewareBase):
+    def __call__(self, ctx: Context) -> t.Any:
+        ctx.logger.debug("Loading plugins...")
+        app = ctx.app
+        app.plugins.paths(*ctx.config.plugins.paths)
+        app.plugins.groups(*ctx.config.plugins.groups)
+        app.plugins.entrypoints(*ctx.config.plugins.entrypoints)
+
+        if app.plugins:
+            ctx.logger.debug("Plugins loaded: %s", ", ".join(app.plugins))
+            ctx.logger.debug("Calling plugin hooks...")
+            for name, p in app.plugins.items():
+                ctx.logger.debug("  Calling plugin hook: %s", name)
+                p(ctx)
+
+
 class PerformDevChecksMiddleware(MiddlewareBase):
     """A utility middleware that performs some development checks.
     Will be disabled in production mode.
 
     # Context Dependencies
     - `arc.root` - Root Command object to start checks from
     - `arc.concig` - Checks Configuration for enviroment
@@ -249,24 +264,26 @@
 
     app()
     ```
 
     """
 
     StartTime = StartTimeMiddleware()
+    LoadPlugins = LoadPluginsMiddleware()
     PerformDevChecks = PerformDevChecksMiddleware()
     AddRuntimeParms = AddRuntimeParmsMiddleware()
     AddUsageErrorInfo = AddUsageErrorInfoMiddleware()
     NormalizeInput = NormalizeInputMiddleware()
     CommandFinder = CommandFinderMiddleware()
     Parser = ArgParseMiddleware()
     CheckParseResult = CheckParseResultsMiddleware()
 
     _list: list[Middleware] = [
         StartTime,
+        LoadPlugins,
         PerformDevChecks,
         AddRuntimeParms,
         AddUsageErrorInfo,
         NormalizeInput,
         CommandFinder,
         Parser,
         CheckParseResult,
```

### Comparing `arc_cli-8.2.0/arc/runtime/middleware.py` & `arc_cli-8.3.0/arc/runtime/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,17 @@
     def try_remove(self, m: Middleware) -> None:
         try:
             self.remove(m)
         except ValueError:
             ...
 
 
-class MiddlewareContainer:
+class MiddlewareManager:
     def __init__(self, middlewares: t.Sequence[Middleware]):
-        self.stack = MiddlewareStack(middlewares)
+        self._stack = MiddlewareStack(middlewares)
 
     @t.overload
     def use(
         self,
         handler: None = None,
         *,
         pos: int | None = None,
@@ -165,26 +165,26 @@
                 raise errors.InternalError(
                     "Cannot provide multiple operations for a single middleware"
                 )
 
         def inner(handler: Middleware) -> Middleware:
             ensure_single_operation()
             if pos is not None:
-                self.stack.insert(pos, handler)
+                self._stack.insert(pos, handler)
             elif replace:
-                idx = self.stack.index(replace)
-                self.stack[idx] = handler
+                idx = self._stack.index(replace)
+                self._stack[idx] = handler
             elif before:
-                idx = self.stack.index(before)
-                self.stack.insert(idx - 1, handler)
+                idx = self._stack.index(before)
+                self._stack.insert(idx - 1, handler)
             elif after:
-                idx = self.stack.index(after)
-                self.stack.insert(idx + 1, handler)
+                idx = self._stack.index(after)
+                self._stack.insert(idx + 1, handler)
             else:
-                self.stack.append(handler)
+                self._stack.append(handler)
 
             return handler
 
         if handler:
             if callable(handler):
                 return inner(handler)
             else:
```

### Comparing `arc_cli-8.2.0/arc/suggest.py` & `arc_cli-8.3.0/arc/suggest.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/aliases.py` & `arc_cli-8.3.0/arc/types/aliases.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/convert.py` & `arc_cli-8.3.0/arc/types/convert.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/default.py` & `arc_cli-8.3.0/arc/types/default.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/file.py` & `arc_cli-8.3.0/arc/types/file.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/middleware/observers.py` & `arc_cli-8.3.0/arc/types/middleware/observers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/middleware/transformers.py` & `arc_cli-8.3.0/arc/types/middleware/transformers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/middleware/validators.py` & `arc_cli-8.3.0/arc/types/middleware/validators.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/network.py` & `arc_cli-8.3.0/arc/types/network.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/numbers.py` & `arc_cli-8.3.0/arc/types/numbers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/path.py` & `arc_cli-8.3.0/arc/types/path.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/semver.py` & `arc_cli-8.3.0/arc/types/semver.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/state.py` & `arc_cli-8.3.0/arc/types/state.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/strings.py` & `arc_cli-8.3.0/arc/types/strings.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/type_arg.py` & `arc_cli-8.3.0/arc/types/type_arg.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/type_info.py` & `arc_cli-8.3.0/arc/types/type_info.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/types/users.py` & `arc_cli-8.3.0/arc/types/users.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/arc/typing.py` & `arc_cli-8.3.0/arc/typing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.2.0/pyproject.toml` & `arc_cli-8.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.2.0"
+version = "8.3.0"
 description = "A Regular CLI"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
 documentation = "https://arc.seanrcollings.com"
 keywords = ["CLI", "extendable", "easy", "arc"]
 classifiers= [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
+    "Typing :: Typed"
 ]
 packages=[{ include = "arc" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
@@ -30,10 +31,13 @@
 types-PyYAML = "^6.0.1"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 Jinja2 = "3.0.3"
 mkdocs-awesome-pages-plugin = "^2.8.0"
 hypothesis = "^6.68.2"
 pygithub = "^1.58.1"
 
+# [tool.poetry.plugins."arc.plugins"]
+# "test_plugin" = "plugin:plugin"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arc_cli-8.2.0/setup.py` & `arc_cli-8.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'arc.types.middleware']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.2.0',
+    'version': '8.3.0',
     'description': 'A Regular CLI',
-    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
+    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# Links\n- [Docs](https://arc.seancollings.dev)\n- [Playground](https://playground.arc.seancollings.dev)\n- [PyPi](https://pypi.org/project/arc-cli/)\n\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `arc_cli-8.2.0/PKG-INFO` & `arc_cli-8.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.2.0
+Version: 8.3.0
 Summary: A Regular CLI
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
 Keywords: CLI,extendable,easy,arc
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Typing :: Typed
 Project-URL: Documentation, https://arc.seanrcollings.com
 Description-Content-Type: text/markdown
 
 # ARC: A Regular CLI
 A tool for building declarative, and highly extendable CLI systems for Python 3.9
 
 # ARC Features
 - Command line arguments based on python type hints
 - Arbitrary command nesting
 - Automatic `--help` documentation
 - Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...
 
-# [Docs](http://arc.seanrcollings.com)
+# Links
+- [Docs](https://arc.seancollings.dev)
+- [Playground](https://playground.arc.seancollings.dev)
+- [PyPi](https://pypi.org/project/arc-cli/)
+
 
 # Quick Start
 
 ```py
 import arc
 
 @arc.command
```

