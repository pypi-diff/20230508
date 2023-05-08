# Comparing `tmp/click_extra-3.8.3.tar.gz` & `tmp/click_extra-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-3.8.3.tar", max compression
+gzip compressed data, was "click_extra-3.9.0.tar", max compression
```

## Comparing `click_extra-3.8.3.tar` & `click_extra-3.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3223 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/__init__.py
--rw-r--r--   0        0        0    22624 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/colorize.py
--rw-r--r--   0        0        0     9399 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/commands.py
--rw-r--r--   0        0        0    29859 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/config.py
--rw-r--r--   0        0        0     6593 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/docs_update.py
--rw-r--r--   0        0        0     4035 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/logging.py
--rw-r--r--   0        0        0     1143 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/parameters.py
--rw-r--r--   0        0        0     3240 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/platform.py
--rw-r--r--   0        0        0    14730 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/py.typed
--rw-r--r--   0        0        0     7749 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/pygments.py
--rw-r--r--   0        0        0     4140 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/run.py
--rw-r--r--   0        0        0     5462 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/sphinx.py
--rw-r--r--   0        0        0     4937 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tabulate.py
--rw-r--r--   0        0        0      770 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    13503 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    15200 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0     8675 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    18915 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     3665 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0     9733 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8707 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0     7041 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_run.py
--rw-r--r--   0        0        0    14173 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     4062 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     8458 2023-02-25 08:27:42.335711 click_extra-3.8.3/click_extra/version.py
--rw-r--r--   0        0        0     6177 2023-02-25 08:27:42.343711 click_extra-3.8.3/pyproject.toml
--rw-r--r--   0        0        0     5392 2023-02-25 08:27:42.343711 click_extra-3.8.3/readme.md
--rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 click_extra-3.8.3/setup.py
--rw-r--r--   0        0        0     8651 1970-01-01 00:00:00.000000 click_extra-3.8.3/PKG-INFO
+-rw-r--r--   0        0        0     4064 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    22415 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/colorize.py
+-rw-r--r--   0        0        0     7826 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/commands.py
+-rw-r--r--   0        0        0    29656 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/config.py
+-rw-r--r--   0        0        0     7448 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6376 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0     3898 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/logging.py
+-rw-r--r--   0        0        0     1143 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/parameters.py
+-rw-r--r--   0        0        0     3240 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/platform.py
+-rw-r--r--   0        0        0    14730 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7749 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     4140 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/run.py
+-rw-r--r--   0        0        0     5460 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     4806 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0      770 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    14075 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    16393 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    10655 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    20375 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     3789 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0     9733 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8707 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0     7041 2023-04-01 06:43:41.500460 click_extra-3.9.0/click_extra/tests/test_run.py
+-rw-r--r--   0        0        0    14287 2023-04-01 06:43:41.504460 click_extra-3.9.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     4604 2023-04-01 06:43:41.504460 click_extra-3.9.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     8327 2023-04-01 06:43:41.504460 click_extra-3.9.0/click_extra/version.py
+-rw-r--r--   0        0        0     6171 2023-04-01 06:43:41.508460 click_extra-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5392 2023-04-01 06:43:41.508460 click_extra-3.9.0/readme.md
+-rw-r--r--   0        0        0     8700 1970-01-01 00:00:00.000000 click_extra-3.9.0/PKG-INFO
```

### Comparing `click_extra-3.8.3/click_extra/__init__.py` & `click_extra-3.9.0/click_extra/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 """Expose package-wide elements."""
 
 from __future__ import annotations
 
-__version__ = "3.8.3"
+__version__ = "3.9.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
@@ -34,81 +34,128 @@
 # Import all click's module-level content to allow for drop-in replacement.
 # XXX Star import is really badly supported by mypy for now and leads to lots of
 # "Module 'XXX' has no attribute 'YYY'". See: https://github.com/python/mypy/issues/4930
 from click import *  # noqa: E402, F403
 from click.core import ParameterSource  # noqa: E402
 
 # Overrides some of click helpers with cloup's.
-from cloup import (  # type: ignore # noqa: E402
+from cloup import (  # noqa: E402
     Argument,
     Command,
     Group,
     HelpFormatter,
     HelpTheme,
     Option,
     Style,
     argument,
-    command,  # noqa: E402
-    group,  # noqa: E402
     option,
     option_group,
 )
 
-# Replace some of click defaults with click-extra variant.
-from .colorize import (  # noqa: I001, E402
-    ColorOption,
-    HelpOption,
+from .colorize import ColorOption, HelpOption  # noqa: I001, E402
+from .commands import TimerOption  # noqa: I001, E402
+from .config import ConfigOption, ShowParamsOption  # noqa: I001, E402
+from .decorators import (  # type: ignore # noqa: I001, E402
     color_option,
-    help_option,
-)
-
-# Import last to avoid circular dependencies.
-from .commands import (  # noqa: I001, E402
-    TimerOption,
+    command,  # noqa: E402
+    config_option,
     extra_command,
     extra_group,
-    timer_option,
-)
-from .config import (  # noqa: I001, E402
-    ConfigOption,
-    ShowParamsOption,
-    config_option,
+    group,  # noqa: E402
+    help_option,
     show_params_option,
+    table_format_option,
+    timer_option,
+    verbosity_option,
+    version_option,
 )
-from .logging import VerbosityOption, verbosity_option  # noqa: I001, E402
+from .logging import VerbosityOption  # noqa: I001, E402
 from .parameters import ExtraOption  # noqa: I001, E402
-from .tabulate import table_format_option  # noqa: I001, E402
-from .version import VersionOption, version_option  # noqa: I001, E402
+from .version import VersionOption  # noqa: I001, E402
 
-__all__ = [
+__all__ = [  # noqa: F405
+    "Abort",
     "Argument",
     "argument",
+    "BadArgumentUsage",
+    "BadOptionUsage",
+    "BadParameter",
+    "BaseCommand",
+    "BOOL",
+    "Choice",
+    "clear",
+    "ClickException",
     "color_option",
     "ColorOption",
-    "Command",
     "command",
+    "Command",
+    "CommandCollection",
     "config_option",
     "ConfigOption",
+    "confirm",
+    "confirmation_option",
+    "Context",
+    "DateTime",
+    "echo",
+    "echo_via_pager",
+    "edit",
     "extra_command",
     "extra_group",
     "ExtraOption",
+    "File",
+    "FileError",
+    "FLOAT",
+    "FloatRange",
+    "format_filename",
+    "get_app_dir",
+    "get_binary_stream",
+    "get_current_context",
+    "get_text_stream",
+    "getchar",
     "group",
     "Group",
     "help_option",
     "HelpFormatter",
     "HelpOption",
     "HelpTheme",
-    "Option",
+    "INT",
+    "IntRange",
+    "launch",
+    "make_pass_decorator",
+    "MissingParameter",
+    "MultiCommand",
+    "NoSuchOption",
+    "open_file",
     "option",
+    "Option",
     "option_group",
+    "OptionParser",
+    "Parameter",
     "ParameterSource",
+    "ParamType",
+    "pass_context",
+    "pass_obj",
+    "password_option",
+    "Path",
+    "pause",
+    "progressbar",
+    "prompt",
+    "secho",
     "show_params_option",
     "ShowParamsOption",
+    "STRING",
+    "style",
     "Style",
     "table_format_option",
     "timer_option",
     "TimerOption",
+    "Tuple",
+    "UNPROCESSED",
+    "unstyle",
+    "UsageError",
+    "UUID",
     "verbosity_option",
     "VerbosityOption",
     "version_option",
     "VersionOption",
+    "wrap_text",
 ]
```

### Comparing `click_extra-3.8.3/click_extra/colorize.py` & `click_extra-3.9.0/click_extra/colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 """Helpers and utilities to apply ANSI coloring to terminal content."""
 
 from __future__ import annotations
 
 import os
 import re
 from configparser import RawConfigParser
-from functools import partial
 from gettext import gettext as _
 from operator import getitem
 from typing import NamedTuple
 
 import regex as re3
 from boltons.strutils import complement_int_list, int_ranges_from_int_list
 from click import Parameter, echo, get_current_context
 from click.core import ParameterSource
-from cloup import Choice, Context, HelpFormatter, Style, option
+from cloup import Choice, Context, HelpFormatter, Style
 from cloup._util import identity
 from cloup.styling import IStyle
 
 from .parameters import ExtraOption
 
 
 class HelpExtraTheme(NamedTuple):
@@ -255,18 +254,14 @@
             is_eager=is_eager,
             expose_value=expose_value,
             help=help,
             **kwargs,
         )
 
 
-color_option = partial(option, cls=ColorOption)
-"""Decorator for ``ColorOption``."""
-
-
 class HelpOption(ExtraOption):
     @staticmethod
     def print_help(ctx: Context, param: Parameter, value: bool) -> None:
         """Prints help text and exits."""
         if not value or ctx.resilient_parsing:
             return
 
@@ -293,18 +288,14 @@
             expose_value=expose_value,
             is_eager=is_eager,
             help=help,
             **kwargs,
         )
 
 
-help_option = partial(option, cls=HelpOption)
-"""Decorator for ``HelpOption``."""
-
-
 class ExtraHelpColorsMixin:
     """Adds extra-keywords highlighting to Click commands.
 
     This mixin for `click.core.Command`-like classes intercepts the top-level helper-
     generation method to initialize the formatter with dynamic settings.
 
     This is implemented here to get access to the global context.
```

### Comparing `click_extra-3.8.3/click_extra/commands.py` & `click_extra-3.9.0/click_extra/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 
 The collection of pre-defined decorators here present good and common defaults. You can
 still mix'n'match the mixins below to build your own custom variants.
 """
 
 from __future__ import annotations
 
-from functools import partial
 from gettext import gettext as _
 from logging import getLevelName
 from time import perf_counter
-from typing import Any
+from typing import (
+    Any,
+)
 
 from click import Context as ClickContext
 from click import echo
-from cloup import Command, Group, command, group, option
+from cloup import Command, Group
 from cloup import Context as CloupContext
 
-from .colorize import ColorOption, ExtraHelpColorsMixin, HelpOption
-from .config import ConfigOption, ShowParamsOption
-from .logging import VerbosityOption, logger
+from .colorize import ExtraHelpColorsMixin
+from .logging import logger
 from .parameters import ExtraOption
 from .version import VersionOption
 
 
 class TimerOption(ExtraOption):
     """A pre-configured option that is adding a ``--time``/``--no-time`` flag to print
     elapsed time at the end of CLI execution."""
@@ -82,18 +82,14 @@
             default=default,
             expose_value=expose_value,
             help=help,
             **kwargs,
         )
 
 
-timer_option = partial(option, cls=TimerOption)
-"""Decorator for ``TimerOption``."""
-
-
 class ExtraContext(CloupContext):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
     ``meta`` property at instanciation."""
 
     _extra_meta: dict[str, Any] = {}
 
     def __init__(self, *args, meta: dict[str, Any] = {}, **kwargs) -> None:
@@ -214,53 +210,7 @@
 
 
 class ExtraGroup(ExtraCommand, Group):
     """Same as ``cloup.group``, but with sane defaults and extra help screen
     colorization."""
 
     pass
-
-
-def default_extra_params():
-    """Default additional options added to ``extra_command`` and ``extra_group``:
-
-    #. ``--time`` / ``--no-time``
-    #. ``--color``, ``--ansi`` / ``--no-color``, ``--no-ansi``
-    #. ``-C``, ``--config CONFIG_PATH``
-    #. ``--show-params``
-    #. ``-v``, ``--verbosity LEVEL``
-    #. ``--version``
-    #. ``-h``, ``--help``
-
-    Order is important to let options at the top have influence on those below.
-
-    .. note::
-
-        This default set is a list wrapped in a method, as a workaround for unittests,
-        in which option instances seems to be reused in unrelated commands and mess with
-        test isolation.
-    """
-    return [
-        TimerOption(),
-        ColorOption(),
-        ConfigOption(),
-        ShowParamsOption(),
-        VerbosityOption(),
-        VersionOption(print_env_info=True),
-        HelpOption(),
-    ]
-
-
-extra_command = partial(command, cls=ExtraCommand, params=default_extra_params())
-"""Augment default ``cloup.command`` with additional options.
-
-See :py:func:`click_extra.commands.default_extra_params` for the list of default
-options.
-"""
-
-
-extra_group = partial(group, cls=ExtraGroup, params=default_extra_params())
-"""Augment default ``cloup.group`` with additional options.
-
-See :py:func:`click_extra.commands.default_extra_params` for the list of default
-options.
-"""
```

### Comparing `click_extra-3.8.3/click_extra/config.py` & `click_extra-3.9.0/click_extra/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from __future__ import annotations
 
 import os
 import sys
 from collections.abc import MutableMapping
 from configparser import ConfigParser, ExtendedInterpolation
 from enum import Enum
-from functools import partial, reduce
+from functools import reduce
 from gettext import gettext as _
 from operator import getitem, methodcaller
 from pathlib import Path
 from typing import Any, Iterable, Sequence
 from unittest.mock import patch
 
 if sys.version_info >= (3, 8):
@@ -41,17 +41,16 @@
     import tomli as tomllib  # type: ignore[import]
 
 import commentjson as json
 import requests
 import xmltodict
 import yaml
 from boltons.iterutils import flatten, remap
-from boltons.urlutils import URL
 from boltons.pathutils import shrinkuser
-
+from boltons.urlutils import URL
 from click import (
     BOOL,
     FLOAT,
     INT,
     STRING,
     UNPROCESSED,
     UUID,
@@ -59,15 +58,15 @@
     Parameter,
     echo,
     get_app_dir,
     get_current_context,
 )
 from click import Path as ClickPath
 from click.core import ParameterSource
-from cloup import Choice, DateTime, File, FloatRange, IntRange, Style, option
+from cloup import Choice, DateTime, File, FloatRange, IntRange, Style
 from cloup import Tuple as CloupTuple
 from mergedeep import merge
 from tabulate import tabulate
 from wcmatch.glob import (
     BRACE,
     DOTGLOB,
     FOLLOW,
@@ -209,16 +208,16 @@
 
                 for p in cmd.params:
                     yield (cli.name, cmd_id, p.name), p
 
     def get_param_type(self, param):
         """Get the Python type of a Click parameter.
 
-        See the list of `custom types provided by Click
-        <https://click.palletsprojects.com/en/8.1.x/api/?highlight=intrange#types>`_.
+        See the list of
+        `custom types provided by Click <https://click.palletsprojects.com/en/8.1.x/api/?highlight=intrange#types>`_.
         """
         if param.multiple or param.nargs != 1:
             return list
 
         if hasattr(param, "is_bool_flag") and getattr(param, "is_bool_flag"):
             return bool
 
@@ -615,17 +614,17 @@
         clean_conf = remap(valid_conf, visit=visit)
         return clean_conf
 
     def load_conf(self, ctx, param, path_pattern):
         """Fetch parameters values from configuration file and merge them with the
         defaults.
 
-        User configuration is `merged to the context default_map as Click does
-        <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
-
+        User configuration is
+        `merged to the context default_map as Click does <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
+        
         This allow user's config to only overrides defaults. Values sets from direct
         command line parameters, environment variables or interactive prompts, takes
         precedence over any values from the config file.
         """
         explicit_conf = ctx.get_parameter_source("config") in (
             ParameterSource.COMMANDLINE,
             ParameterSource.ENVIRONMENT,
@@ -827,15 +826,7 @@
             sorted(table, key=sort_by_depth),
             headers=header_labels,
             tablefmt="rounded_outline",
             disable_numparse=True,
         )
         echo(output, color=ctx.color)
         ctx.exit()
-
-
-show_params_option = partial(option, cls=ShowParamsOption)
-"""Decorator for ``ShowParamsOption``."""
-
-
-config_option = partial(option, cls=ConfigOption)
-"""Decorator for ``ConfigOption``."""
```

### Comparing `click_extra-3.8.3/click_extra/docs_update.py` & `click_extra-3.9.0/click_extra/docs_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,24 +132,17 @@
                 "\n" + indent("\n".join(sorted(nodes)), INDENT) + "\nend"
             )
         )
 
     # Wrap the Mermaid code into a MyST block.
     return "\n".join(
         (
-            "```{mermaid}",
-            # XXX Titles are not supported by sphinxcontrib-mermaid yet:
-            # https://github.com/mgaitan/sphinxcontrib-mermaid/issues/108
-            #
-            # "---",
-            # (
-            #     f"title: click_extra.platforms.{graph_id} - {description}"
-            #     f" (Click Extra v{__version__})"
-            # ),
-            # "---",
+            # Use attributes blocks extension to add a title.
+            ('{caption="' f"`click_extra.platforms.{graph_id}` - {description}" '"}'),
+            "```mermaid",
             "flowchart",
             indent("\n".join(sorted(subgraphs)), INDENT),
             "```",
         )
     )
```

### Comparing `click_extra-3.8.3/click_extra/logging.py` & `click_extra-3.9.0/click_extra/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 """Logging utilities."""
 
 from __future__ import annotations
 
 import logging
-from functools import partial
 from gettext import gettext as _
 
 from click_log import basic_config
-from cloup import Choice, option
+from cloup import Choice
 
 from .parameters import ExtraOption
 
 LOG_LEVELS = {
     name: value
     for value, name in sorted(logging._levelToName.items(), reverse=True)
     if name != "NOTSET"
@@ -120,11 +119,7 @@
             metavar=metavar,
             type=type,
             expose_value=expose_value,
             help=help,
             is_eager=is_eager,
             **kwargs,
         )
-
-
-verbosity_option = partial(option, cls=VerbosityOption)
-"""Decorator for ``VerbosityOption``."""
```

### Comparing `click_extra-3.8.3/click_extra/parameters.py` & `click_extra-3.9.0/click_extra/parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/platform.py` & `click_extra-3.9.0/click_extra/platform.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/platforms.py` & `click_extra-3.9.0/click_extra/platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     return sys.platform.startswith("GNU")
 
 
 @cache
 def is_linux() -> bool:
     """Return `True` only if current platform is of the Linux family.
 
-    Excludes WSL1 and WSL2 from this check to `avoid false positives
-    <https://github.com/kdeldycke/meta-package-manager/issues/944>`_.
+    Excludes WSL1 and WSL2 from this check to
+    `avoid false positives <https://github.com/kdeldycke/meta-package-manager/issues/944>`_.
     """
     return sys.platform.startswith("linux") and not is_wsl1() and not is_wsl2()
 
 
 @cache
 def is_macos() -> bool:
     """Return `True` only if current platform is of the macOS family."""
```

### Comparing `click_extra-3.8.3/click_extra/pygments.py` & `click_extra-3.9.0/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/run.py` & `click_extra-3.9.0/click_extra/run.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/sphinx.py` & `click_extra-3.9.0/click_extra/sphinx.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     MyST:
 
     .. code-block:: markdown
 
         ```{click-example}
         from click_extra import echo, extra_command, option, style
 
-        @extra_command()
+        @extra_command
         @option("--name", prompt="Your name", help="The person to greet.")
         def hello_world(name):
             "Simple program that greets NAME."
             echo(f"Hello, {style(name, fg='red')}!")
         ```
 
     .. code-block:: markdown
```

### Comparing `click_extra-3.8.3/click_extra/tabulate.py` & `click_extra-3.9.0/click_extra/tabulate.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import csv
 from functools import partial
 from gettext import gettext as _
 from io import StringIO
 
 import tabulate
 from click import Choice, echo
-from cloup import option
 
 from .parameters import ExtraOption
 
 tabulate.MIN_PADDING = 0
 """Neutralize spurious double-spacing in table rendering."""
 
 
@@ -133,11 +132,7 @@
             param_decls=param_decls,
             type=type,
             default=default,
             expose_value=expose_value,
             help=help,
             **kwargs,
         )
-
-
-table_format_option = partial(option, cls=TableFormatOption)
-"""Decorator for ``TableFormatOption``."""
```

### Comparing `click_extra-3.8.3/click_extra/tests/__init__.py` & `click_extra-3.9.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/tests/conftest.py` & `click_extra-3.9.0/click_extra/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import cloup
 import pytest
 from boltons.strutils import strip_ansi
 from boltons.tbutils import ExceptionInfo
 from click.core import BaseCommand
 from click.testing import CliRunner, Result
 
-from ..commands import extra_command, extra_group
+from ..decorators import command, extra_command, extra_group, group
 from ..platforms import is_linux, is_macos, is_windows
 from ..run import EnvVars, args_cleanup, print_cli_output
 
 DESTRUCTIVE_MODE = bool(
     os.environ.get("DESTRUCTIVE_TESTS", False) not in {True, 1, "True", "true", "1"}
 )
 """Pre-computed boolean flag indicating if destructive mode is activated by the presence
@@ -194,14 +194,15 @@
 
 
 def command_decorators(
     no_commands=False,
     no_groups=False,
     no_click=False,
     no_cloup=False,
+    no_redefined=False,
     no_extra=False,
     with_types=False,
 ):
     """Returns collection of Pytest parameters to test all forms of click/cloup/click-
     extra command-like decorators."""
     params = []
 
@@ -218,22 +219,30 @@
             params.extend(
                 [
                     (cloup.command, {"cloup", "command"}, "cloup.command", skip_naked),
                     (cloup.command(), {"cloup", "command"}, "cloup.command()", ()),
                 ]
             )
 
+        if not no_redefined:
+            params.extend(
+                [
+                    (command, {"redefined", "command"}, "click_extra.command", ()),
+                    (command(), {"redefined", "command"}, "click_extra.command()", ()),
+                ]
+            )
+
         if not no_extra:
             params.extend(
                 [
                     (
                         extra_command,
                         {"extra", "command"},
                         "click_extra.extra_command",
-                        skip_naked,
+                        (),
                     ),
                     (
                         extra_command(),
                         {"extra", "command"},
                         "click_extra.extra_command()",
                         (),
                     ),
@@ -253,22 +262,30 @@
             params.extend(
                 [
                     (cloup.group, {"cloup", "group"}, "cloup.group", skip_naked),
                     (cloup.group(), {"cloup", "group"}, "cloup.group()", ()),
                 ]
             )
 
+        if not no_redefined:
+            params.extend(
+                [
+                    (group, {"redefined", "group"}, "click_extra.group", ()),
+                    (group(), {"redefined", "group"}, "click_extra.group()", ()),
+                ]
+            )
+
         if not no_extra:
             params.extend(
                 [
                     (
                         extra_group,
                         {"extra", "group"},
                         "click_extra.extra_group",
-                        skip_naked,
+                        (),
                     ),
                     (
                         extra_group(),
                         {"extra", "group"},
                         "click_extra.extra_group()",
                         (),
                     ),
```

### Comparing `click_extra-3.8.3/click_extra/tests/test_colorize.py` & `click_extra-3.9.0/click_extra/tests/test_colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,34 @@
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
 from boltons.strutils import strip_ansi
 from click import echo, secho, style
-from cloup import HelpTheme, Style, argument, command, option, option_group
+from cloup import HelpTheme, Style, argument, option, option_group
+from pytest_cases import parametrize
 
 from ..colorize import (
     HelpExtraFormatter,
     HelpExtraTheme,
-    color_option,
     default_theme,
     highlight,
 )
-from ..commands import extra_command, extra_group
-from ..logging import LOG_LEVELS, logger, verbosity_option
+from ..decorators import (
+    color_option,
+    command,
+    extra_command,
+    extra_group,
+    help_option,
+    verbosity_option,
+)
+from ..logging import LOG_LEVELS, logger
 from .conftest import (
+    command_decorators,
     default_debug_colored_log,
     default_debug_uncolored_log,
     default_options_colored_help,
     skip_windows_colors,
 )
 
 
@@ -104,15 +112,15 @@
     # Make sure no highlighting occurred
     assert strip_ansi(output) == output
 
 
 @skip_windows_colors
 def test_keyword_collection(invoke):
     # Create a dummy Click CLI.
-    @extra_group()
+    @extra_group
     @option_group(
         "Group 1",
         option("-a", "--o1"),
         option("-b", "--o2"),
     )
     @cloup.option_group(
         "Group 2",
@@ -238,56 +246,57 @@
               -h, --help  Show this message and exit.
             """
         )
         assert not result.stderr
 
 
 @skip_windows_colors
+@parametrize("option_decorator", (color_option, color_option()))
 @pytest.mark.parametrize(
     "param,expecting_colors",
     (
         ("--color", True),
         ("--no-color", False),
         ("--ansi", True),
         ("--no-ansi", False),
         (None, True),
     ),
 )
-def test_standalone_color_option(invoke, param, expecting_colors):
+def test_standalone_color_option(invoke, option_decorator, param, expecting_colors):
     """Check color option values, defaults and effects on all things colored, including
     verbosity option."""
 
     @click.command
-    @verbosity_option()
-    @color_option()
-    def color_cli5():
+    @verbosity_option
+    @option_decorator
+    def standalone_color():
         echo(Style(fg="yellow")("It works!"))
         echo("\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m")
         echo(style("Run command.", fg="magenta"))
         logger.warning("Processing...")
         print(style("print() bypass Click.", fg="blue"))
         secho("Done.", fg="green")
 
-    result = invoke(color_cli5, param, "--verbosity", "DEBUG", color=True)
+    result = invoke(standalone_color, param, "--verbosity", "DEBUG", color=True)
     assert result.exit_code == 0
 
     if expecting_colors:
-        assert result.output == (
+        assert result.stdout == (
             "\x1b[33mIt works!\x1b[0m\n"
             "\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m\n"
             "\x1b[35mRun command.\x1b[0m\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "\x1b[32mDone.\x1b[0m\n"
         )
         assert result.stderr == (
             "\x1b[34mdebug: \x1b[0mVerbosity set to DEBUG.\n"
             "\x1b[33mwarning: \x1b[0mProcessing...\n"
         )
     else:
-        assert result.output == (
+        assert result.stdout == (
             "It works!\n"
             "Art\n"
             "Run command.\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "Done.\n"
         )
         assert result.stderr == (
@@ -318,15 +327,15 @@
         (None, True),
     ),
 )
 def test_no_color_env_convention(
     invoke, env, env_expect_colors, param, param_expect_colors
 ):
     @click.command
-    @color_option()
+    @color_option
     def color_cli7():
         echo(Style(fg="yellow")("It works!"))
 
     result = invoke(color_cli7, param, color=True, env=env)
     assert result.exit_code == 0
     assert not result.stderr
 
@@ -349,15 +358,15 @@
         ("--no-color", False),
         ("--ansi", True),
         ("--no-ansi", False),
         (None, True),
     ),
 )
 def test_integrated_color_option(invoke, param, expecting_colors):
-    @extra_group()
+    @extra_group
     def color_cli8():
         echo(Style(fg="yellow")("It works!"))
         echo("\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m")
 
     @color_cli8.command()
     def command1():
         echo(style("Run command #1.", fg="magenta"))
@@ -456,7 +465,43 @@
     result = highlight(
         "Hey-xx-xxx-heY-xXxXxxxxx-hey",
         substrings,
         styling_method=default_theme.success,
         ignore_case=ignore_case,
     )
     assert result == expected
+
+
+@parametrize(
+    "cmd_decorator, cmd_type",
+    # Skip click extra's commands, as help option is already part of the default.
+    command_decorators(no_extra=True, with_types=True),
+)
+@parametrize("option_decorator", (help_option, help_option()))
+def test_standalone_help_option(invoke, cmd_decorator, cmd_type, option_decorator):
+    @cmd_decorator
+    @option_decorator
+    def standalone_help():
+        echo("It works!")
+
+    result = invoke(standalone_help, "--help")
+    assert result.exit_code == 0
+    assert not result.stderr
+
+    if "group" in cmd_type:
+        assert result.stdout == dedent(
+            """\
+            Usage: standalone-help [OPTIONS] COMMAND [ARGS]...
+
+            Options:
+              -h, --help  Show this message and exit.
+            """
+        )
+    else:
+        assert result.stdout == dedent(
+            """\
+            Usage: standalone-help [OPTIONS]
+
+            Options:
+              -h, --help  Show this message and exit.
+            """
+        )
```

### Comparing `click_extra-3.8.3/click_extra/tests/test_commands.py` & `click_extra-3.9.0/click_extra/tests/test_commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,32 +22,37 @@
 import re
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
 from click import echo
-from cloup import command, option, option_group
-from pytest_cases import fixture
+from cloup import option, option_group
+from pytest_cases import fixture, parametrize
 
-from ..commands import extra_command, extra_group, timer_option
-from .conftest import default_debug_uncolored_log, default_options_uncolored_help
+from ..decorators import extra_command, extra_group, timer_option
+from .conftest import (
+    command_decorators,
+    default_debug_uncolored_log,
+    default_options_uncolored_help,
+)
 
 
 @fixture
 def all_command_cli():
+    """A CLI that used all variations and flavors of subcommands."""
     @extra_group(version="2021.10.08")
     def command_cli1():
         echo("It works!")
 
     @command_cli1.command()
     def default_subcommand():
         echo("Run default subcommand...")
 
-    @extra_command()
+    @extra_command
     def click_extra_subcommand():
         echo("Run click-extra subcommand...")
 
     @cloup.command()
     def cloup_subcommand():
         echo("Run cloup subcommand...")
 
@@ -208,50 +213,122 @@
 
     regex_output = r"command-cli1, version 2021.10.08\n{'.+'}\n"
     assert re.fullmatch(regex_output, result.output)
 
     assert not result.stderr
 
 
-def test_standalone_time_option(invoke):
-    @command()
-    @timer_option()
-    def standalone_time():
+@parametrize(
+    "cmd_decorator",
+    # Skip click extra's commands, as timer option is already part of the default.
+    command_decorators(no_groups=True, no_extra=True),
+)
+@parametrize("option_decorator", (timer_option, timer_option()))
+def test_standalone_timer_option(invoke, cmd_decorator, option_decorator):
+    @cmd_decorator
+    @option_decorator
+    def standalone_timer():
         echo("It works!")
 
-    result = invoke(standalone_time, "--help")
+    result = invoke(standalone_timer, "--help")
     assert result.exit_code == 0
+    assert not result.stderr
     assert result.stdout == dedent(
         """\
-        Usage: standalone-time [OPTIONS]
+        Usage: standalone-timer [OPTIONS]
 
         Options:
           --time / --no-time  Measure and print elapsed execution time.
           --help              Show this message and exit.
         """
     )
-    assert not result.stderr
 
-    result = invoke(standalone_time, "--time")
+    result = invoke(standalone_timer, "--time")
     assert result.exit_code == 0
+    assert not result.stderr
     assert re.fullmatch(
         r"It works!\nExecution time: [0-9.]+ seconds.\n",
         result.output,
     )
-    assert not result.stderr
 
-    result = invoke(standalone_time, "--no-time")
+    result = invoke(standalone_timer, "--no-time")
     assert result.exit_code == 0
+    assert not result.stderr
     assert result.output == "It works!\n"
+
+
+def test_no_option_leaks_between_subcommands(invoke):
+    """As reported in https://github.com/kdeldycke/click-extra/issues/489."""
+    @click.group
+    def cli():
+        echo("Run cli...")
+
+    @extra_command
+    @click.option("--one")
+    def foo():
+        echo("Run foo...")
+
+    @extra_command(short_help="Bar subcommand.")
+    @click.option("--two")
+    def bar():
+        echo("Run bar...")
+
+    cli.add_command(foo)
+    cli.add_command(bar)
+
+    result = invoke(cli, "--help", color=False)
+    assert result.exit_code == 0
+    assert result.output == dedent(
+        """\
+        Usage: cli [OPTIONS] COMMAND [ARGS]...
+
+        Options:
+          --help  Show this message and exit.
+
+        Commands:
+          bar  Bar subcommand.
+          foo
+        """
+    )
+    assert not result.stderr
+
+    result = invoke(cli, "foo", "--help", color=False)
+    assert result.exit_code == 0
+    assert re.fullmatch(
+        (
+            r"Run cli\.\.\.\n"
+            r"Usage: cli foo \[OPTIONS\]\n"
+            r"\n"
+            r"Options:\n"
+            r"  --one TEXT\n"
+            rf"{default_options_uncolored_help}"
+        ),
+        result.stdout,
+    )
+    assert not result.stderr
+
+    result = invoke(cli, "bar", "--help", color=False)
+    assert result.exit_code == 0
+    assert re.fullmatch(
+        (
+            r"Run cli\.\.\.\n"
+            r"Usage: cli bar \[OPTIONS\]\n"
+            r"\n"
+            r"Options:\n"
+            r"  --two TEXT\n"
+            rf"{default_options_uncolored_help}"
+        ),
+        result.stdout,
+    )
     assert not result.stderr
 
 
 def test_option_group_integration(invoke):
     # Mix regular and grouped options
-    @extra_group()
+    @extra_group
     @option_group(
         "Group 1",
         click.option("-a", "--opt1"),
         option("-b", "--opt2"),
     )
     @click.option("-c", "--opt3")
     @option("-d", "--opt4")
```

### Comparing `click_extra-3.8.3/click_extra/tests/test_config.py` & `click_extra-3.9.0/click_extra/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import re
 from os.path import sep
 from pathlib import Path
 
 import click
 import pytest
+from boltons.pathutils import shrinkuser
 from click import (
     BOOL,
     FLOAT,
     INT,
     STRING,
     UNPROCESSED,
     UUID,
@@ -36,21 +37,24 @@
     IntRange,
     Tuple,
     echo,
     get_app_dir,
 )
 from click import Path as ClickPath
 from cloup import argument, option
+from pytest_cases import parametrize
 from tabulate import tabulate
-from boltons.pathutils import shrinkuser
 
 from ..colorize import escape_for_help_sceen
-from ..commands import extra_command, extra_group
-from ..config import ConfigOption, ShowParamsOption, config_option
-from .conftest import default_debug_uncolored_log
+from ..config import ConfigOption, ShowParamsOption
+from ..decorators import config_option, extra_command, extra_group, show_params_option
+from .conftest import (
+    command_decorators,
+    default_debug_uncolored_log,
+)
 
 DUMMY_TOML_FILE = """
     # Comment
 
     top_level_param             = "to_ignore"
 
     [config-cli1]
@@ -188,15 +192,15 @@
             ("ini", DUMMY_INI_FILE),
             ("xml", DUMMY_XML_FILE),
         )
     ),
 )
 
 
-@extra_group()
+@extra_group
 @option("--dummy-flag/--no-flag")
 @option("--my-list", multiple=True)
 def config_cli1(dummy_flag, my_list):
     echo(f"dummy_flag = {dummy_flag!r}")
     echo(f"my_list = {my_list!r}")
 
 
@@ -258,16 +262,21 @@
     assert not result.output
     assert result.stderr == (
         f"Load configuration matching {conf_path}\n"
         f"critical: No configuration file found.\n"
     )
 
 
-def test_conf_auto_types(invoke, create_config):
-    """Check the conf type and structure is properly derived from CLI options."""
+@parametrize("option_decorator", (config_option, config_option()))
+def test_conf_auto_types(invoke, create_config, option_decorator):
+    """Check the conf type and structure is properly derived from CLI options.
+
+    Also covers the tests of the standalone ``@config_option`` decorator in all its
+    flavors.
+    """
     @click.command
     @option("--flag1/--no-flag1")
     @option("--flag2", is_flag=True)
     @option("--str-param1", type=str)
     @option("--str-param2", type=STRING)
     @option("--int-param1", type=int)
     @option("--int-param2", type=INT)
@@ -284,15 +293,15 @@
     @option("--count-param", count=True)  # See issue #170.
     @option("--float-range-param", type=FloatRange())
     @option("--datetime-param", type=DateTime())
     @option("--tuple1", nargs=2, type=Tuple([str, int]))
     @option("--list1", multiple=True)
     @argument("file_arg1", type=File("w"))
     @argument("file_arg2", type=File("w"), nargs=-1)
-    @config_option()
+    @option_decorator
     def config_cli2(
         flag1,
         flag2,
         str_param1,
         str_param2,
         int_param1,
         int_param2,
@@ -516,16 +525,59 @@
         assert result.exit_code == 0
         assert result.output == (
             "dummy_flag = False\nmy_list = ('super', 'wow')\nint_parameter = 15\n"
         )
         assert result.stderr == f"Load configuration matching {conf_path.resolve()}\n"
 
 
-def test_show_params_option(invoke, create_config):
-    @extra_command()
+@parametrize(
+    "cmd_decorator",
+    # Skip click extra's commands, as show_params option is already part of the default.
+    command_decorators(no_groups=True, no_extra=True),
+)
+@parametrize("option_decorator", (show_params_option, show_params_option()))
+def test_standalone_show_params_option(invoke, cmd_decorator, option_decorator):
+    @cmd_decorator
+    @option_decorator
+    def show_params():
+        echo("It works!")
+
+    result = invoke(show_params, "--show-params")
+    assert result.exit_code == 0
+
+    table = [
+        (
+            "show-params.show_params",
+            "click_extra.config.ShowParamsOption",
+            "--show-params",
+            "bool",
+            "",
+            "✘",
+            "",
+            False,
+            "",
+            "COMMANDLINE",
+        ),
+    ]
+    output = tabulate(
+        table,
+        headers=ShowParamsOption.TABLE_HEADERS,
+        tablefmt="rounded_outline",
+        disable_numparse=True,
+    )
+    assert result.output == f"{output}\n"
+
+    assert result.stderr == (
+        "warning: Cannot extract parameters values: "
+        "<Command show-params> does not inherits from ExtraCommand.\n"
+    )
+
+
+def test_integrated_show_params_option(invoke, create_config):
+    @extra_command
     @option("--int-param1", type=int, default=10)
     @option("--int-param2", type=int, default=555)
     def show_params_cli(int_param1, int_param2):
         echo(f"int_param1 is {int_param1!r}")
         echo(f"int_param2 is {int_param2!r}")
 
     conf_file = """
```

### Comparing `click_extra-3.8.3/click_extra/tests/test_logging.py` & `click_extra-3.9.0/click_extra/tests/test_logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 
 from __future__ import annotations
 
 import re
 
 import pytest
 from click import echo
+from pytest_cases import parametrize
 
-from ..commands import extra_command
-from ..logging import LOG_LEVELS, logger, verbosity_option
+from ..decorators import extra_command, verbosity_option
+from ..logging import LOG_LEVELS, logger
 from .conftest import command_decorators, default_debug_colored_log, skip_windows_colors
 
 
 @pytest.mark.parametrize("cmd_decorator, cmd_type", command_decorators(with_types=True))
 def test_unrecognized_verbosity(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
-    @verbosity_option()
+    @verbosity_option
     def logging_cli1():
         echo("It works!")
 
     result = invoke(logging_cli1, "--verbosity", "random")
     assert result.exit_code == 2
     assert not result.output
 
@@ -47,22 +48,23 @@
         "Error: Invalid value for '--verbosity' / '-v': "
         "'random' is not one of 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG'.\n"
     )
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
-    # Skip click extra's commands, as verbosity option is already part of the default.
     "cmd_decorator",
+    # Skip click extra's commands, as verbosity option is already part of the default.
     command_decorators(no_groups=True, no_extra=True),
 )
+@parametrize("option_decorator", (verbosity_option, verbosity_option()))
 @pytest.mark.parametrize("level", LOG_LEVELS.keys())
-def test_standalone_verbosity_option(invoke, cmd_decorator, level):
+def test_standalone_verbosity_option(invoke, cmd_decorator, option_decorator, level):
     @cmd_decorator
-    @verbosity_option()
+    @option_decorator
     def logging_cli2():
         echo("It works!")
         logger.debug("my debug message.")
         logger.info("my info message.")
         logger.warning("my warning message.")
         logger.error("my error message.")
         logger.critical("my critical message.")
@@ -84,15 +86,15 @@
     assert result.stderr == log_records
 
 
 @skip_windows_colors
 @pytest.mark.parametrize("level", LOG_LEVELS.keys())
 # TODO: test extra_group
 def test_integrated_verbosity_option(invoke, level):
-    @extra_command()
+    @extra_command
     def logging_cli3():
         echo("It works!")
 
     result = invoke(logging_cli3, "--verbosity", level, color=True)
     assert result.exit_code == 0
     assert result.output == "It works!\n"
     if level == "DEBUG":
```

### Comparing `click_extra-3.8.3/click_extra/tests/test_platforms.py` & `click_extra-3.9.0/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/tests/test_pygments.py` & `click_extra-3.9.0/click_extra/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/tests/test_run.py` & `click_extra-3.9.0/click_extra/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `click_extra-3.8.3/click_extra/tests/test_tabulate.py` & `click_extra-3.9.0/click_extra/tests/test_tabulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 import pytest
 import tabulate
 
 # We use vanilla click primitives here to demonstrate the full-compatibility.
 from click import echo, pass_context
 from pytest_cases import fixture, parametrize
 
+from ..decorators import table_format_option
 from ..platforms import is_windows
-from ..tabulate import output_formats, table_format_option
+from ..tabulate import output_formats
 from .conftest import command_decorators
 
 
 @pytest.mark.parametrize("cmd_decorator, cmd_type", command_decorators(with_types=True))
 def test_unrecognized_format(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
-    @table_format_option()
+    @table_format_option
     def tabulate_cli1():
         echo("It works!")
 
     result = invoke(tabulate_cli1, "--table-format", "random")
     assert result.exit_code == 2
     assert not result.output
 
@@ -511,17 +512,18 @@
 
     assert len(output_formats) == len(expected_renderings.keys())
     assert set(output_formats) == set(expected_renderings.keys())
 
 
 @fixture
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
-def table_cli(cmd_decorator):
+@parametrize("option_decorator", (table_format_option, table_format_option()))
+def table_cli(cmd_decorator, option_decorator):
     @cmd_decorator
-    @table_format_option()
+    @option_decorator
     @pass_context
     def tabulate_cli2(ctx):
         data = ((1, 87), (2, 80), (3, 79))
         headers = ("day", "temperature")
         ctx.print_table(data, headers)
 
     return tabulate_cli2
```

### Comparing `click_extra-3.8.3/click_extra/tests/test_version.py` & `click_extra-3.9.0/click_extra/tests/test_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,37 @@
 
 import click
 import pytest
 from click import echo
 from cloup import Style
 from pytest_cases import parametrize
 
-from ..colorize import color_option
-from ..commands import extra_group
-from ..version import version_option
+from ..decorators import color_option, extra_group, version_option
 from .conftest import command_decorators, skip_windows_colors
 
 
 @skip_windows_colors
+@parametrize("cmd_decorator", command_decorators())
+@parametrize("option_decorator", (version_option, version_option()))
+def test_standalone_version_option(invoke, cmd_decorator, option_decorator):
+    @cmd_decorator
+    @option_decorator
+    def standalone_option():
+        echo("It works!")
+
+    result = invoke(standalone_option, "--version", color=True)
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert re.fullmatch(
+        r"\x1b\[97mstandalone-option\x1b\[0m, version \x1b\[32m\d+.\d+.\d+\x1b\[0m\n",
+        result.output,
+    )
+
+
+@skip_windows_colors
 def test_standalone_version_option_with_env_info(invoke):
     @click.group
     @version_option(version="1.2.3.4", print_env_info=True)
     def color_cli2():
         echo("It works!")
 
     # Test default colouring.
@@ -104,15 +120,15 @@
     ..todo:
 
         Maybe have the possibility to tweak CLI callback evaluation order so we can
         let the user to have the NO_COLOR env set to allow for color-less ``--version``
         output.
     """
     @click.command
-    @color_option()
+    @color_option
     @version_option(version="2.1.9")
     def color_cli6():
         echo(Style(fg="yellow")("It works!"))
 
     result = invoke(color_cli6, "--no-color", "--version", "command1", color=True)
     assert result.exit_code == 0
     assert result.output == "color-cli6, version 2.1.9\n"
```

### Comparing `click_extra-3.8.3/click_extra/version.py` & `click_extra-3.9.0/click_extra/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 """Extraction of CLI's version and its printing."""
 
 from __future__ import annotations
 
 import inspect
 import re
 import sys
-from functools import partial
 from gettext import gettext as _
 from typing import Iterable
 
 if sys.version_info >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata  # type: ignore[import]
 
 from boltons.ecoutils import get_profile
 from click import Parameter, echo
-from cloup import Context, Style, option
+from cloup import Context, Style
 
 from .colorize import default_theme
 from .parameters import ExtraOption
 
 
 class VersionOption(ExtraOption):
     """Prints the colored version of the CLI.
@@ -222,11 +221,7 @@
             param_decls=param_decls,
             is_flag=is_flag,
             expose_value=expose_value,
             is_eager=is_eager,
             help=help,
             **kwargs,
         )
-
-
-version_option = partial(option, cls=VersionOption)
-"""Decorator for ``VersionOption``."""
```

### Comparing `click_extra-3.8.3/pyproject.toml` & `click_extra-3.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "3.8.3"
+version = "3.9.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -72,50 +72,50 @@
 # https://en.wikipedia.org/wiki/History_of_Python#Support
 python = "^3.7"
 boltons = "^23.0.0"
 click = "^8.1.1"
 click-log = "^0.4.0"
 cloup = "^2.0.0.post1"
 commentjson = "^0.9.0"
+furo = "^2023.03.27"
 importlib-metadata = { version = ">= 1.4", python = "< 3.8" }
 mergedeep = "^1.3.4"
 Pallets-Sphinx-Themes = "^2.0.2"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
 pygments = "^2.14.0"
-pygments-ansi-color = ">=0.0.6,<0.2.1"
+pygments-ansi-color = "^0.2.0"
 pyyaml = "^6.0.0"
 regex = "^2022.3.15"
 requests = "^2.27.1"
 sphinx = "^5.3.0"
 tabulate = { extras = ["widechars"], version = "^0.9.0" }
 tomli = { version = "^2.0.1", python = "< 3.11" }
 wcmatch = "^8.4"
-xmltodict = ">=0.12,<0.14"
+xmltodict = "^0.13.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
 coverage = { extras = ["toml"], version = "^7.2" }
-furo = "^2022.9.15"
-mypy = "^1.0"
-myst-parser = "^0.18.0"
-pytest = "^7.2.1"
+mypy = "^1.1"
+myst-parser = "^1.0.0"
+pytest = "^7.2.2"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cases = "^3.6.14"
 pytest-cov = "^4.0.0"
 pytest-httpserver = "^1.0.6"
 pytest-randomly = "^3.12.0"
 sphinx-autodoc-typehints = "^1.22"
 sphinx-copybutton = "^0.5.1"
 sphinx-design = "^0.3.0"
 sphinx-issues = "^3.0.1"
 sphinxext-opengraph = "^0.7.5"
-sphinxcontrib-mermaid = "^0.8"
+sphinxcontrib-mermaid = "^0.8.1"
 types-Pygments = "^2.14.0"
 types-PyYAML = "^6.0.12"
-types-regex = "^2022.10.31.6"
+types-regex = "^2023.3.23.1"
 types-requests = "^2.28.11"
 types-tabulate = "^0.9.0"
 types-xmltodict = "^0.13.0"
 
 [tool.poetry.plugins."pygments.lexers"]
 # The name of the entrypoint values doesn’t really matter, Pygments extracts required metadata from the class definition.
 # Source: https://pygments.org/docs/plugins/#defining-plugins-through-entrypoints
```

### Comparing `click_extra-3.8.3/readme.md` & `click_extra-3.9.0/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
   <a href="https://github.com/kdeldycke/click-extra/">
-    <img src="https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/images/logo-banner.svg" alt="Click Extra">
+    <img src="https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/assets/logo-banner.svg" alt="Click Extra">
   </a>
 </p>
 
 [![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
 [![Python versions](https://img.shields.io/pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
 [![Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml?query=branch%3Amain)
 [![Documentation status](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml?query=branch%3Amain)
@@ -21,19 +21,19 @@
 [workarounds and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
 reached upstream yet (or are unlikely to).
 
 ## Example
 
 It can transform this vanilla `click` CLI:
 
-![click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/images/click-help-screen.png)
+![click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-help-screen.png)
 
 Into this:
 
-![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/images/click-extra-screen.png)
+![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
 
 To undestrand how we ended up with the result above, go [read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).
 
 ## Features
 
 - Configuration file loader for:
   - `TOML`
```

#### html2text {}

```diff
@@ -14,16 +14,16 @@
 Click Extra? A collection of helpers and utilities for [Click](https://
 click.palletsprojects.com), the Python CLI framework. It is a drop-in
 replacement with good defaults that saves lots of boilerplate code and
 frustration. It also comes with [workarounds and patches](https://
 kdeldycke.github.io/click-extra/issues.html) that have not reached upstream yet
 (or are unlikely to). ## Example It can transform this vanilla `click` CLI: !
 [click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
-images/click-help-screen.png) Into this: ![click-extra CLI help screen](https:/
-/github.com/kdeldycke/click-extra/raw/main/docs/images/click-extra-screen.png)
+assets/click-help-screen.png) Into this: ![click-extra CLI help screen](https:/
+/github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
 To undestrand how we ended up with the result above, go [read the tutorial]
 (https://kdeldycke.github.io/click-extra/tutorial.html). ## Features -
 Configuration file loader for: - `TOML` - `YAML` - `JSON`, with inline and
 block comments (Python-style `#` and Javascript-style `//`) - `INI`, with
 extended interpolation, multi-level sections and non-native types (`list`,
 `set`, â¦) - `XML` - Download configuration from remote URLs - Optional strict
 validation of configuration - Search of configuration file from default user
```

### Comparing `click_extra-3.8.3/setup.py` & `click_extra-3.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,161 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: click-extra
+Version: 3.9.0
+Summary: 🌈 Extra colorization and configuration loading for Click.
+Home-page: https://github.com/kdeldycke/click-extra
+License: GPL-2.0-or-later
+Keywords: ansi-colors,cli,cli-helper,click-help-color,click-log,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
+Author: Kevin Deldycke
+Author-email: kevin@deldycke.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Plugins
+Classifier: Framework :: Pytest
+Classifier: Framework :: Sphinx
+Classifier: Framework :: Sphinx :: Extension
+Classifier: Framework :: Sphinx :: Theme
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Classifier: Topic :: Text Processing :: Filters
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Topic :: Text Processing :: Markup :: reStructuredText
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: Pallets-Sphinx-Themes (>=2.0.2,<3.0.0)
+Requires-Dist: boltons (>=23.0.0,<24.0.0)
+Requires-Dist: click (>=8.1.1,<9.0.0)
+Requires-Dist: click-log (>=0.4.0,<0.5.0)
+Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
+Requires-Dist: commentjson (>=0.9.0,<0.10.0)
+Requires-Dist: furo (>=2023.03.27,<2024.0.0)
+Requires-Dist: importlib-metadata (>=1.4) ; python_version < "3.8"
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
+Requires-Dist: pygments (>=2.14.0,<3.0.0)
+Requires-Dist: pygments-ansi-color (>=0.2.0,<0.3.0)
+Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
+Requires-Dist: regex (>=2022.3.15,<2023.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: sphinx (>=5.3.0,<6.0.0)
+Requires-Dist: tabulate[widechars] (>=0.9.0,<0.10.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Requires-Dist: wcmatch (>=8.4,<9.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Project-URL: Changelog, https://kdeldycke.github.io/click-extra/changelog.html
+Project-URL: Documentation, https://kdeldycke.github.io/click-extra
+Project-URL: Funding, https://github.com/sponsors/kdeldycke
+Project-URL: Issues, https://github.com/kdeldycke/click-extra/issues
+Project-URL: Repository, https://github.com/kdeldycke/click-extra
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <a href="https://github.com/kdeldycke/click-extra/">
+    <img src="https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/assets/logo-banner.svg" alt="Click Extra">
+  </a>
+</p>
+
+[![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
+[![Python versions](https://img.shields.io/pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
+[![Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml?query=branch%3Amain)
+[![Documentation status](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml?query=branch%3Amain)
+[![Coverage status](https://codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://codecov.io/gh/kdeldycke/click-extra/branch/main)
+[![DOI](https://zenodo.org/badge/418402236.svg)](https://zenodo.org/badge/latestdoi/418402236)
+
+## What is Click Extra?
+
+A collection of helpers and utilities for
+[Click](https://click.palletsprojects.com), the Python CLI framework.
+
+It is a drop-in replacement with good defaults that saves lots of boilerplate code and frustration.
+It also comes with
+[workarounds and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
+reached upstream yet (or are unlikely to).
+
+## Example
+
+It can transform this vanilla `click` CLI:
+
+![click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-help-screen.png)
+
+Into this:
+
+![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
+
+To undestrand how we ended up with the result above, go [read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).
+
+## Features
+
+- Configuration file loader for:
+  - `TOML`
+  - `YAML`
+  - `JSON`, with inline and block comments (Python-style `#` and Javascript-style `//`)
+  - `INI`, with extended interpolation, multi-level sections and non-native types (`list`, `set`, …)
+  - `XML`
+- Download configuration from remote URLs
+- Optional strict validation of configuration
+- Search of configuration file from default user folder and glob patterns
+- Respect of `CLI` > `Configuration` > `Environment` > `Defaults` precedence
+- `--show-params` option to debug parameters defaults, values, environment variables and provenance
+- Colorization of help screens
+- `-h`/`--help` option names (see [rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/))
+- `--color`/`--no-color` option flag
+- Recognize the `NO_COLOR` environment variable convention from [`no-color.org`](https://no-color.org)
+- Colored `--version` option
+- Colored `--verbosity` option and logs
+- `--time`/`--no-time` flag to measure duration of command execution
+- Platform recognition utilities (macOS, Linux and Windows)
+- New conditional markers for `pytest`:
+  - `@skip_linux`, `@skip_macos` and `@skip_windows`
+  - `@unless_linux`, `@unless_macos` and `@unless_windows`
+  - `@destructive` and `@non_destructive`
+- [`.. click:example::` and `.. click:run::` Sphinx extensions](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
+- [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
+- Pygments styles and filters for ANSI rendering
+- [Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
+- Rely on [`cloup`](https://github.com/janluke/cloup) to add:
+  - option groups
+  - constraints
+  - subcommands sections
+  - aliases
+  - command suggestion (`Did you mean <subcommand>?`)
+
+## Used in
+
+Check these projects to get real-life examples of `click-extra` usage:
+
+- ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://github.com/kdeldycke/meta-package-manager#readme)
+  \- A unifying CLI for multiple package managers.
+- ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A
+  CLI to deduplicate similar emails.
+- ![GitHub stars](https://img.shields.io/github/stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox tool.
+- ![GitHub stars](https://img.shields.io/github/stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/hugolundin/badger#readme) - An mDNS-based reverse
+  proxy for naming services on a local network.
+- ![GitHub stars](https://img.shields.io/github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme)
+
+Feel free to send a PR to add your project in this list if you are relying on Click Extra in any way.
+
+## Development
+
+[Development guidelines](https://kdeldycke.github.io/meta-package-manager/development.html)
+are the same as
+[parent project `mpm`](https://github.com/kdeldycke/meta-package-manager), from
+which `click-extra` originated.
 
-packages = \
-['click_extra', 'click_extra.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pallets-Sphinx-Themes>=2.0.2,<3.0.0',
- 'boltons>=23.0.0,<24.0.0',
- 'click-log>=0.4.0,<0.5.0',
- 'click>=8.1.1,<9.0.0',
- 'cloup>=2.0.0.post1,<3.0.0',
- 'commentjson>=0.9.0,<0.10.0',
- 'mergedeep>=1.3.4,<2.0.0',
- 'pygments-ansi-color>=0.0.6,<0.2.1',
- 'pygments>=2.14.0,<3.0.0',
- 'pyyaml>=6.0.0,<7.0.0',
- 'regex>=2022.3.15,<2023.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'sphinx>=5.3.0,<6.0.0',
- 'tabulate[widechars]>=0.9.0,<0.10.0',
- 'wcmatch>=8.4,<9.0',
- 'xmltodict>=0.12,<0.14']
-
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0'],
- ':python_version < "3.8"': ['importlib-metadata>=1.4']}
-
-entry_points = \
-{'pygments.filters': ['ansi-filter = click_extra.pygments:AnsiFilter'],
- 'pygments.formatters': ['ansi-html-formatter = '
-                         'click_extra.pygments:AnsiHtmlFormatter'],
- 'pygments.lexers': ['ansi-bash-session = '
-                     'click_extra.pygments:AnsiBashSessionLexer',
-                     'ansi-dylan-console = '
-                     'click_extra.pygments:AnsiDylanConsoleLexer',
-                     'ansi-elixir-console = '
-                     'click_extra.pygments:AnsiElixirConsoleLexer',
-                     'ansi-erlang-shell = '
-                     'click_extra.pygments:AnsiErlangShellLexer',
-                     'ansi-gap-console = '
-                     'click_extra.pygments:AnsiGAPConsoleLexer',
-                     'ansi-julia-console = '
-                     'click_extra.pygments:AnsiJuliaConsoleLexer',
-                     'ansi-matlab-session = '
-                     'click_extra.pygments:AnsiMatlabSessionLexer',
-                     'ansi-msdos-session = '
-                     'click_extra.pygments:AnsiMSDOSSessionLexer',
-                     'ansi-output = click_extra.pygments:AnsiOutputLexer',
-                     'ansi-postgres-console = '
-                     'click_extra.pygments:AnsiPostgresConsoleLexer',
-                     'ansi-power-shell-session = '
-                     'click_extra.pygments:AnsiPowerShellSessionLexer',
-                     'ansi-psysh-console = '
-                     'click_extra.pygments:AnsiPsyshConsoleLexer',
-                     'ansi-python-console = '
-                     'click_extra.pygments:AnsiPythonConsoleLexer',
-                     'ansi-r-console = click_extra.pygments:AnsiRConsoleLexer',
-                     'ansi-ruby-console = '
-                     'click_extra.pygments:AnsiRubyConsoleLexer',
-                     'ansi-sqlite-console = '
-                     'click_extra.pygments:AnsiSqliteConsoleLexer',
-                     'ansi-tcsh-session = '
-                     'click_extra.pygments:AnsiTcshSessionLexer'],
- 'pygments.styles': ['ansi-click-extra-furo-style = '
-                     'click_extra.pygments:AnsiClickExtraFuroStyle']}
-
-setup_kwargs = {
-    'name': 'click-extra',
-    'version': '3.8.3',
-    'description': '🌈 Extra colorization and configuration loading for Click.',
-    'long_description': '<p align="center">\n  <a href="https://github.com/kdeldycke/click-extra/">\n    <img src="https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/images/logo-banner.svg" alt="Click Extra">\n  </a>\n</p>\n\n[![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://pypi.python.org/pypi/click-extra)\n[![Python versions](https://img.shields.io/pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra)\n[![Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml?query=branch%3Amain)\n[![Documentation status](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml?query=branch%3Amain)\n[![Coverage status](https://codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://codecov.io/gh/kdeldycke/click-extra/branch/main)\n[![DOI](https://zenodo.org/badge/418402236.svg)](https://zenodo.org/badge/latestdoi/418402236)\n\n## What is Click Extra?\n\nA collection of helpers and utilities for\n[Click](https://click.palletsprojects.com), the Python CLI framework.\n\nIt is a drop-in replacement with good defaults that saves lots of boilerplate code and frustration.\nIt also comes with\n[workarounds and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not\nreached upstream yet (or are unlikely to).\n\n## Example\n\nIt can transform this vanilla `click` CLI:\n\n![click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/images/click-help-screen.png)\n\nInto this:\n\n![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/images/click-extra-screen.png)\n\nTo undestrand how we ended up with the result above, go [read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).\n\n## Features\n\n- Configuration file loader for:\n  - `TOML`\n  - `YAML`\n  - `JSON`, with inline and block comments (Python-style `#` and Javascript-style `//`)\n  - `INI`, with extended interpolation, multi-level sections and non-native types (`list`, `set`, …)\n  - `XML`\n- Download configuration from remote URLs\n- Optional strict validation of configuration\n- Search of configuration file from default user folder and glob patterns\n- Respect of `CLI` > `Configuration` > `Environment` > `Defaults` precedence\n- `--show-params` option to debug parameters defaults, values, environment variables and provenance\n- Colorization of help screens\n- `-h`/`--help` option names (see [rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/))\n- `--color`/`--no-color` option flag\n- Recognize the `NO_COLOR` environment variable convention from [`no-color.org`](https://no-color.org)\n- Colored `--version` option\n- Colored `--verbosity` option and logs\n- `--time`/`--no-time` flag to measure duration of command execution\n- Platform recognition utilities (macOS, Linux and Windows)\n- New conditional markers for `pytest`:\n  - `@skip_linux`, `@skip_macos` and `@skip_windows`\n  - `@unless_linux`, `@unless_macos` and `@unless_windows`\n  - `@destructive` and `@non_destructive`\n- [`.. click:example::` and `.. click:run::` Sphinx extensions](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution\n- [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output\n- Pygments styles and filters for ANSI rendering\n- [Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects\n- Rely on [`cloup`](https://github.com/janluke/cloup) to add:\n  - option groups\n  - constraints\n  - subcommands sections\n  - aliases\n  - command suggestion (`Did you mean <subcommand>?`)\n\n## Used in\n\nCheck these projects to get real-life examples of `click-extra` usage:\n\n- ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://github.com/kdeldycke/meta-package-manager#readme)\n  \\- A unifying CLI for multiple package managers.\n- ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A\n  CLI to deduplicate similar emails.\n- ![GitHub stars](https://img.shields.io/github/stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox tool.\n- ![GitHub stars](https://img.shields.io/github/stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/hugolundin/badger#readme) - An mDNS-based reverse\n  proxy for naming services on a local network.\n- ![GitHub stars](https://img.shields.io/github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme)\n\nFeel free to send a PR to add your project in this list if you are relying on Click Extra in any way.\n\n## Development\n\n[Development guidelines](https://kdeldycke.github.io/meta-package-manager/development.html)\nare the same as\n[parent project `mpm`](https://github.com/kdeldycke/meta-package-manager), from\nwhich `click-extra` originated.\n',
-    'author': 'Kevin Deldycke',
-    'author_email': 'kevin@deldycke.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kdeldycke/click-extra',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,111 +1,114 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['click_extra', 'click_extra.tests'] package_data = \ {'': ['*']}
-install_requires = \ ['Pallets-Sphinx-Themes>=2.0.2,<3.0.0',
-'boltons>=23.0.0,<24.0.0', 'click-log>=0.4.0,<0.5.0', 'click>=8.1.1,<9.0.0',
-'cloup>=2.0.0.post1,<3.0.0', 'commentjson>=0.9.0,<0.10.0',
-'mergedeep>=1.3.4,<2.0.0', 'pygments-ansi-color>=0.0.6,<0.2.1',
-'pygments>=2.14.0,<3.0.0', 'pyyaml>=6.0.0,<7.0.0',
-'regex>=2022.3.15,<2023.0.0', 'requests>=2.27.1,<3.0.0',
-'sphinx>=5.3.0,<6.0.0', 'tabulate[widechars]>=0.9.0,<0.10.0',
-'wcmatch>=8.4,<9.0', 'xmltodict>=0.12,<0.14'] extras_require = \ {':
-python_version < "3.11"': ['tomli>=2.0.1,<3.0.0'], ':python_version < "3.8"':
-['importlib-metadata>=1.4']} entry_points = \ {'pygments.filters': ['ansi-
-filter = click_extra.pygments:AnsiFilter'], 'pygments.formatters': ['ansi-html-
-formatter = ' 'click_extra.pygments:AnsiHtmlFormatter'], 'pygments.lexers':
-['ansi-bash-session = ' 'click_extra.pygments:AnsiBashSessionLexer', 'ansi-
-dylan-console = ' 'click_extra.pygments:AnsiDylanConsoleLexer', 'ansi-elixir-
-console = ' 'click_extra.pygments:AnsiElixirConsoleLexer', 'ansi-erlang-shell =
-' 'click_extra.pygments:AnsiErlangShellLexer', 'ansi-gap-console = '
-'click_extra.pygments:AnsiGAPConsoleLexer', 'ansi-julia-console = '
-'click_extra.pygments:AnsiJuliaConsoleLexer', 'ansi-matlab-session = '
-'click_extra.pygments:AnsiMatlabSessionLexer', 'ansi-msdos-session = '
-'click_extra.pygments:AnsiMSDOSSessionLexer', 'ansi-output =
-click_extra.pygments:AnsiOutputLexer', 'ansi-postgres-console = '
-'click_extra.pygments:AnsiPostgresConsoleLexer', 'ansi-power-shell-session = '
-'click_extra.pygments:AnsiPowerShellSessionLexer', 'ansi-psysh-console = '
-'click_extra.pygments:AnsiPsyshConsoleLexer', 'ansi-python-console = '
-'click_extra.pygments:AnsiPythonConsoleLexer', 'ansi-r-console =
-click_extra.pygments:AnsiRConsoleLexer', 'ansi-ruby-console = '
-'click_extra.pygments:AnsiRubyConsoleLexer', 'ansi-sqlite-console = '
-'click_extra.pygments:AnsiSqliteConsoleLexer', 'ansi-tcsh-session = '
-'click_extra.pygments:AnsiTcshSessionLexer'], 'pygments.styles': ['ansi-click-
-extra-furo-style = ' 'click_extra.pygments:AnsiClickExtraFuroStyle']}
-setup_kwargs = { 'name': 'click-extra', 'version': '3.8.3', 'description':
-'ð Extra colorization and configuration loading for Click.',
-'long_description': '
-                            \n \n_[Click_Extra]\n\n
-\n\n[![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://
-pypi.python.org/pypi/click-extra)\n[![Python versions](https://img.shields.io/
-pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra)\n[!
+Metadata-Version: 2.1 Name: click-extra Version: 3.9.0 Summary: ð Extra
+colorization and configuration loading for Click. Home-page: https://
+github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
+colors,cli,cli-helper,click-help-color,click-
+log,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
+tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
+kevin@deldycke.com Requires-Python: >=3.7,<4.0 Classifier: Development Status
+:: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
+Sphinx Classifier: Framework :: Sphinx :: Extension Classifier: Framework ::
+Sphinx :: Theme Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: GNU General Public License v2 or later (GPLv2+) Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier: Topic
+:: Documentation :: Sphinx Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development :: User
+Interfaces Classifier: Topic :: System :: Logging Classifier: Topic :: System
+:: Shells Classifier: Topic :: Terminals Classifier: Topic :: Text Processing
+:: Filters Classifier: Topic :: Text Processing :: Markup :: HTML Classifier:
+Topic :: Text Processing :: Markup :: Markdown Classifier: Topic :: Text
+Processing :: Markup :: XML Classifier: Topic :: Text Processing :: Markup ::
+reStructuredText Classifier: Topic :: Utilities Classifier: Typing :: Typed
+Requires-Dist: Pallets-Sphinx-Themes (>=2.0.2,<3.0.0) Requires-Dist: boltons
+(>=23.0.0,<24.0.0) Requires-Dist: click (>=8.1.1,<9.0.0) Requires-Dist: click-
+log (>=0.4.0,<0.5.0) Requires-Dist: cloup (>=2.0.0.post1,<3.0.0) Requires-Dist:
+commentjson (>=0.9.0,<0.10.0) Requires-Dist: furo (>=2023.03.27,<2024.0.0)
+Requires-Dist: importlib-metadata (>=1.4) ; python_version < "3.8" Requires-
+Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pygments (>=2.14.0,<3.0.0)
+Requires-Dist: pygments-ansi-color (>=0.2.0,<0.3.0) Requires-Dist: pyyaml
+(>=6.0.0,<7.0.0) Requires-Dist: regex (>=2022.3.15,<2023.0.0) Requires-Dist:
+requests (>=2.27.1,<3.0.0) Requires-Dist: sphinx (>=5.3.0,<6.0.0) Requires-
+Dist: tabulate[widechars] (>=0.9.0,<0.10.0) Requires-Dist: tomli
+(>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist: wcmatch (>=8.4,<9.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Changelog, https://
+kdeldycke.github.io/click-extra/changelog.html Project-URL: Documentation,
+https://kdeldycke.github.io/click-extra Project-URL: Funding, https://
+github.com/sponsors/kdeldycke Project-URL: Issues, https://github.com/
+kdeldycke/click-extra/issues Project-URL: Repository, https://github.com/
+kdeldycke/click-extra Description-Content-Type: text/markdown
+                                 [Click_Extra]
+[![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://
+pypi.python.org/pypi/click-extra) [![Python versions](https://img.shields.io/
+pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra) [!
 [Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/
-actions/workflows/tests.yaml?query=branch%3Amain)\n[![Documentation status]
+actions/workflows/tests.yaml?query=branch%3Amain) [![Documentation status]
 (https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/
 badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/
-workflows/docs.yaml?query=branch%3Amain)\n[![Coverage status](https://
+workflows/docs.yaml?query=branch%3Amain) [![Coverage status](https://
 codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://
-codecov.io/gh/kdeldycke/click-extra/branch/main)\n[![DOI](https://zenodo.org/
-badge/418402236.svg)](https://zenodo.org/badge/latestdoi/418402236)\n\n## What
-is Click Extra?\n\nA collection of helpers and utilities for\n[Click](https://
-click.palletsprojects.com), the Python CLI framework.\n\nIt is a drop-in
+codecov.io/gh/kdeldycke/click-extra/branch/main) [![DOI](https://zenodo.org/
+badge/418402236.svg)](https://zenodo.org/badge/latestdoi/418402236) ## What is
+Click Extra? A collection of helpers and utilities for [Click](https://
+click.palletsprojects.com), the Python CLI framework. It is a drop-in
 replacement with good defaults that saves lots of boilerplate code and
-frustration.\nIt also comes with\n[workarounds and patches](https://
-kdeldycke.github.io/click-extra/issues.html) that have not\nreached upstream
-yet (or are unlikely to).\n\n## Example\n\nIt can transform this vanilla
-`click` CLI:\n\n![click CLI help screen](https://github.com/kdeldycke/click-
-extra/raw/main/docs/images/click-help-screen.png)\n\nInto this:\n\n![click-
-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
-images/click-extra-screen.png)\n\nTo undestrand how we ended up with the result
-above, go [read the tutorial](https://kdeldycke.github.io/click-extra/
-tutorial.html).\n\n## Features\n\n- Configuration file loader for:\n - `TOML`\n
-- `YAML`\n - `JSON`, with inline and block comments (Python-style `#` and
-Javascript-style `//`)\n - `INI`, with extended interpolation, multi-level
-sections and non-native types (`list`, `set`, â¦)\n - `XML`\n- Download
-configuration from remote URLs\n- Optional strict validation of
-configuration\n- Search of configuration file from default user folder and glob
-patterns\n- Respect of `CLI` > `Configuration` > `Environment` > `Defaults`
-precedence\n- `--show-params` option to debug parameters defaults, values,
-environment variables and provenance\n- Colorization of help screens\n- `-h`/`-
--help` option names (see [rant on other inconsistencies](https://
-blog.craftyguy.net/cmdline-help/))\n- `--color`/`--no-color` option flag\n-
+frustration. It also comes with [workarounds and patches](https://
+kdeldycke.github.io/click-extra/issues.html) that have not reached upstream yet
+(or are unlikely to). ## Example It can transform this vanilla `click` CLI: !
+[click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
+assets/click-help-screen.png) Into this: ![click-extra CLI help screen](https:/
+/github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
+To undestrand how we ended up with the result above, go [read the tutorial]
+(https://kdeldycke.github.io/click-extra/tutorial.html). ## Features -
+Configuration file loader for: - `TOML` - `YAML` - `JSON`, with inline and
+block comments (Python-style `#` and Javascript-style `//`) - `INI`, with
+extended interpolation, multi-level sections and non-native types (`list`,
+`set`, â¦) - `XML` - Download configuration from remote URLs - Optional strict
+validation of configuration - Search of configuration file from default user
+folder and glob patterns - Respect of `CLI` > `Configuration` > `Environment` >
+`Defaults` precedence - `--show-params` option to debug parameters defaults,
+values, environment variables and provenance - Colorization of help screens -
+`-h`/`--help` option names (see [rant on other inconsistencies](https://
+blog.craftyguy.net/cmdline-help/)) - `--color`/`--no-color` option flag -
 Recognize the `NO_COLOR` environment variable convention from [`no-color.org`]
-(https://no-color.org)\n- Colored `--version` option\n- Colored `--verbosity`
-option and logs\n- `--time`/`--no-time` flag to measure duration of command
-execution\n- Platform recognition utilities (macOS, Linux and Windows)\n- New
-conditional markers for `pytest`:\n - `@skip_linux`, `@skip_macos` and
-`@skip_windows`\n - `@unless_linux`, `@unless_macos` and `@unless_windows`\n -
-`@destructive` and `@non_destructive`\n- [`.. click:example::` and `.. click:
+(https://no-color.org) - Colored `--version` option - Colored `--verbosity`
+option and logs - `--time`/`--no-time` flag to measure duration of command
+execution - Platform recognition utilities (macOS, Linux and Windows) - New
+conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
+`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
+`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
 run::` Sphinx extensions](https://kdeldycke.github.io/click-extra/sphinx.html)
-to document CLI source code and their execution\n- [ANSI-capable Pygments
+to document CLI source code and their execution - [ANSI-capable Pygments
 lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell
-session and console output\n- Pygments styles and filters for ANSI rendering\n-
+session and console output - Pygments styles and filters for ANSI rendering -
 [Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from
-other Click-related projects\n- Rely on [`cloup`](https://github.com/janluke/
-cloup) to add:\n - option groups\n - constraints\n - subcommands sections\n -
-aliases\n - command suggestion (`Did you mean ?`)\n\n## Used in\n\nCheck these
-projects to get real-life examples of `click-extra` usage:\n\n- ![GitHub stars]
-(https://img.shields.io/github/stars/kdeldycke/meta-package-
+other Click-related projects - Rely on [`cloup`](https://github.com/janluke/
+cloup) to add: - option groups - constraints - subcommands sections - aliases -
+command suggestion (`Did you mean ?`) ## Used in Check these projects to get
+real-life examples of `click-extra` usage: - ![GitHub stars](https://
+img.shields.io/github/stars/kdeldycke/meta-package-
 manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://
-github.com/kdeldycke/meta-package-manager#readme)\n \\- A unifying CLI for
-multiple package managers.\n- ![GitHub stars](https://img.shields.io/github/
+github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI for
+multiple package managers. - ![GitHub stars](https://img.shields.io/github/
 stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
-Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A\n CLI to
-deduplicate similar emails.\n- ![GitHub stars](https://img.shields.io/github/
+Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
+deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
 stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
 [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
-rewrite of the fireprox tool.\n- ![GitHub stars](https://img.shields.io/github/
+rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
 stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
-(https://github.com/hugolundin/badger#readme) - An mDNS-based reverse\n proxy
-for naming services on a local network.\n- ![GitHub stars](https://
-img.shields.io/github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square)
-[Molecular Dynamics Trajectory Analysis](https://github.com/tclick/
-mdstab#readme)\n\nFeel free to send a PR to add your project in this list if
-you are relying on Click Extra in any way.\n\n## Development\n\n[Development
-guidelines](https://kdeldycke.github.io/meta-package-manager/
-development.html)\nare the same as\n[parent project `mpm`](https://github.com/
-kdeldycke/meta-package-manager), from\nwhich `click-extra` originated.\n',
-'author': 'Kevin Deldycke', 'author_email': 'kevin@deldycke.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/kdeldycke/click-
-extra', 'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'entry_points':
-entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+(https://github.com/hugolundin/badger#readme) - An mDNS-based reverse proxy for
+naming services on a local network. - ![GitHub stars](https://img.shields.io/
+github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular
+Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme) Feel
+free to send a PR to add your project in this list if you are relying on Click
+Extra in any way. ## Development [Development guidelines](https://
+kdeldycke.github.io/meta-package-manager/development.html) are the same as
+[parent project `mpm`](https://github.com/kdeldycke/meta-package-manager), from
+which `click-extra` originated.
```

