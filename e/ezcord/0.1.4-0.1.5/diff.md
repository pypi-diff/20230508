# Comparing `tmp/ezcord-0.1.4.tar.gz` & `tmp/ezcord-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.1.4.tar", last modified: Thu Apr 27 14:25:08 2023, max compression
+gzip compressed data, was "ezcord-0.1.5.tar", last modified: Mon May  8 19:19:30 2023, max compression
```

## Comparing `ezcord-0.1.4.tar` & `ezcord-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.178108 ezcord-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 14:24:54.000000 ezcord-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-27 14:25:08.178108 ezcord-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-27 14:24:54.000000 ezcord-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 14:24:54.000000 ezcord-0.1.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.174108 ezcord-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 14:24:54.000000 ezcord-0.1.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 14:24:54.000000 ezcord-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 14:24:54.000000 ezcord-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:25:08.178108 ezcord-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.174108 ezcord-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.174108 ezcord-0.1.4/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.178108 ezcord-0.1.4/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.178108 ezcord-0.1.4/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.608173 ezcord-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 19:19:18.000000 ezcord-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-08 19:19:30.608173 ezcord-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-08 19:19:18.000000 ezcord-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 19:19:18.000000 ezcord-0.1.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 19:19:18.000000 ezcord-0.1.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 19:19:18.000000 ezcord-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 19:19:18.000000 ezcord-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:19:30.608173 ezcord-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.608173 ezcord-0.1.5/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/funcutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.1.4/LICENSE` & `ezcord-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.4/PKG-INFO` & `ezcord-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.4
+Version: 0.1.5
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # EzCord
 [![](https://img.shields.io/discord/1010915072694046794?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/zfvbjTEzv6)
 [![](https://img.shields.io/pypi/v/ezcord.svg?style=for-the-badge&logo=pypi&color=yellow&logoColor=white)](https://pypi.org/project/ezcord/)
 [![](https://img.shields.io/pypi/l/ezcord?style=for-the-badge)]()
 [![](https://aschey.tech/tokei/github/tibue99/ezcord?style=for-the-badge)](https://github.com/tibue99/ezcord)
 
 An easy-to-use extension for the [Pycord](https://github.com/Pycord-Development/pycord) library with some utility functions.
 
 ## Installing
-Python 3.8 or higher is required.
+Python 3.9 or higher is required.
 ```
 pip install ezcord
 ```
 You can also install the latest version from GitHub. Note that this version may be unstable
 and requires [git](https://git-scm.com/downloads) to be installed.
 ```
 pip install git+https://github.com/tibue99/ezcord
```

### Comparing `ezcord-0.1.4/README.md` & `ezcord-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![](https://img.shields.io/pypi/v/ezcord.svg?style=for-the-badge&logo=pypi&color=yellow&logoColor=white)](https://pypi.org/project/ezcord/)
 [![](https://img.shields.io/pypi/l/ezcord?style=for-the-badge)]()
 [![](https://aschey.tech/tokei/github/tibue99/ezcord?style=for-the-badge)](https://github.com/tibue99/ezcord)
 
 An easy-to-use extension for the [Pycord](https://github.com/Pycord-Development/pycord) library with some utility functions.
 
 ## Installing
-Python 3.8 or higher is required.
+Python 3.9 or higher is required.
 ```
 pip install ezcord
 ```
 You can also install the latest version from GitHub. Note that this version may be unstable
 and requires [git](https://git-scm.com/downloads) to be installed.
 ```
 pip install git+https://github.com/tibue99/ezcord
```

### Comparing `ezcord-0.1.4/pyproject.toml` & `ezcord-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [project]
 name = "ezcord"
 description = "An easy-to-use extension for the Pycord library"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {text = "MIT"}
 keywords = ["discord", "pycord", "py-cord"]
 authors = [
     { name = "tibue99" }
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["dependencies", "optional-dependencies", "version"]
 
 [tool.setuptools.dynamic]
```

### Comparing `ezcord-0.1.4/src/ezcord/bot.py` & `ezcord-0.1.5/src/ezcord/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 from typing import Any, Literal
 
 import aiohttp
 import discord
 from discord.ext import commands
 
 from .emb import error as error_emb
-from .internal.translation import set_lang, t
+from .enums import ReadyEvent
+from .internal import print_ready, set_lang, t
 from .logs import DEFAULT_LOG, custom_log, set_log
 from .times import dc_timestamp
 
 
 class Bot(discord.Bot):
-    """Bot class that extends from :class:`discord.Bot`.
+    """The EzCord bot class. This is a subclass of :class:`discord.Bot`.
+
+    .. hint::
+
+        As this class extends from :class:`discord.Bot`, only slash commands are supported.
+        If you want to use prefix commands, use :class:`PrefixBot` instead.
 
     Parameters
     ----------
     intents:
         The intents to use for the bot. Defaults to :meth:`discord.Intents.default()`.
     debug:
         Enable debug logs. Defaults to ``True``.
@@ -36,26 +42,32 @@
     ignored_errors:
         A list of error types to ignore. Defaults to ``None``.
     full_error_traceback:
         Whether to send the full error traceback. If this is ``False``,
         only the most recent traceback will be sent. Defaults to ``False``.
     language:
         The language to use for the bot. Defaults to ``en``.
+    ready_event:
+        The style for :meth:`on_ready_event`. Defaults to :attr:`.ReadyEvent.default`.
+        If this is ``None``, the event will be disabled.
+    **kwargs:
+        Additional keyword arguments for :class:`discord.Bot`.
     """
 
     def __init__(
         self,
         intents: discord.Intents = discord.Intents.default(),
         *,
         debug: bool = True,
         error_handler: bool = True,
         error_webhook_url: str | None = None,
         ignored_errors: list[Any] | None = None,
         full_error_traceback: bool = False,
         language: Literal["en", "de"] = "en",
+        ready_event: ReadyEvent | None = ReadyEvent.default,
         **kwargs,
     ):
         super().__init__(intents=intents, **kwargs)
 
         if debug:
             self.logger = set_log(DEFAULT_LOG)
         else:
@@ -68,30 +80,32 @@
         set_lang(language)
 
         if error_handler:
             self.add_listener(self._error_event, "on_application_command_error")
         elif error_webhook_url:
             warnings.warn("You need to enable the error handler for the webhook to work.")
 
-        self.add_listener(self.ready_event, "on_ready")
+        self.ready_event = ready_event
+        if ready_event:
+            self.add_listener(self.on_ready_event, "on_ready")
 
     def load_cogs(
         self,
         *directories: str,
         subdirectories: bool = False,
         ignored_cogs: list[str] | None = None,
         custom_logs: bool | str = True,
     ):
         """Load all cogs in the given directories.
 
         Parameters
         ----------
         *directories:
             Names of the directories to load cogs from.
-            Defaults to ``cogs``.
+            Defaults to ``"cogs"``.
         subdirectories:
             Whether to load cogs from subdirectories.
             Defaults to ``False``.
         ignored_cogs:
             A list of cogs to ignore. Defaults to ``None``.
         custom_logs:
             Whether to use a custom log format for cogs. Defaults to ``True``.
@@ -128,34 +142,17 @@
                                     f"Loaded {element.name}.{name}",
                                     color=custom_logs,
                                     level=logging.DEBUG,
                                 )
                             else:
                                 self.logger.debug(f"Loaded {element.name}.{name}")
 
-    async def ready_event(self):
+    async def on_ready_event(self):
         """Prints the bot's information when it's ready."""
-        infos = [
-            f"User:     {self.user}",
-            f"ID:       {self.user.id}",
-            f"Pycord:   {discord.__version__}",
-            f"Commands: {len(self.commands):,}",
-            f"Guilds:   {len(self.guilds):,}",
-            f"Latency:  {round(self.latency * 1000):,}ms",
-        ]
-
-        longest = max([str(i) for i in infos], key=len)
-        formatter = f"<{len(longest)}"
-
-        start_txt = "Bot is online!"
-        start_txt += f"\n╔{(len(longest) + 2) * '═'}╗\n"
-        for thing in infos:
-            start_txt += f"║ {thing:{formatter}} ║\n"
-        start_txt += f"╚{(len(longest) + 2) * '═'}╝"
-        self.logger.info(start_txt)
+        print_ready(self, self.ready_event)
 
     async def _error_event(self, ctx: discord.ApplicationContext, error: discord.DiscordException):
         """The event that handles application command errors."""
         if type(error) in self.ignored_errors:
             return
 
         if isinstance(error, commands.CommandOnCooldown):
@@ -220,7 +217,17 @@
                         webhook_sent = True
 
             self.logger.exception(
                 f"Error while executing **/{ctx.command.qualified_name}** ```{error_msg}```",
                 exc_info=error,
                 extra={"webhook_sent": webhook_sent},
             )
+
+
+class PrefixBot(Bot, commands.Bot):
+    """A subclass of :class:`discord.ext.commands.Bot` that implements the :class:`Bot` class.
+
+    This class can be used if you want to use EzCord with prefix commands.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ezcord-0.1.4/src/ezcord/emb.py` & `ezcord-0.1.5/src/ezcord/emb.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         await emb.success(ctx, "Success!")
 """
 
 from __future__ import annotations
 
 import discord
 
-from .internal.embed_templates import load_embed, save_embeds
+from .internal import copy_kwargs, load_embed, save_embeds
 
 
 def set_embed_templates(
     *,
     error_embed: discord.Embed | None = None,
     success_embed: discord.Embed | None = None,
     warn_embed: discord.Embed | None = None,
@@ -97,136 +97,162 @@
         await target.send(embed=embed, **kwargs)
 
 
 async def _process_message(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     embed: discord.Embed,
     txt: str,
+    title: str | None,
     ephemeral: bool,
-    *,
-    title: str | None = None,
     **kwargs,
 ):
     """Adds embed attributes to the embed before sending it.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
         The text to send.
+    title:
+        The title of the embed. Defaults to ``None``.
     ephemeral:
         Whether the message should be ephemeral.
     """
     embed.description = txt
     if title is not None:
         embed.title = title
 
     await _send_embed(target, embed, ephemeral, **kwargs)
 
 
+@copy_kwargs(discord.InteractionResponse.send_message)
 async def error(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str,
+    *,
+    title: str | None = None,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send an error message. By default, this is a red embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
-        The text to send.
+        The text for the embed description.
+    title:
+        The title of the embed. Defaults to ``None``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("error_embed")
-    await _process_message(target, embed, txt, ephemeral, **kwargs)
+    await _process_message(target, embed.copy(), txt, title, ephemeral, **kwargs)
 
 
+@copy_kwargs(discord.abc.Messageable.send)
 async def success(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str,
+    *,
+    title: str | None = None,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send a success message. By default, this is a green embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
-        The text to send.
+        The text for the embed description.
+    title:
+        The title of the embed. Defaults to ``None``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("success_embed")
-    await _process_message(target, embed, txt, ephemeral, **kwargs)
+    await _process_message(target, embed.copy(), txt, title, ephemeral, **kwargs)
 
 
+@copy_kwargs(discord.abc.Messageable.send)
 async def warn(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str,
+    *,
+    title: str | None = None,
     ephemeral: bool = True,
     **kwargs,
 ):
-    """Send a warning message. By default, this is an orange embed.
+    """Send a warning message. By default, this is a golden embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
-        The text to send.
+        The text for the embed description.
+    title:
+        The title of the embed. Defaults to ``None``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("warn_embed")
-    await _process_message(target, embed, txt, ephemeral, **kwargs)
+    await _process_message(target, embed.copy(), txt, title, ephemeral, **kwargs)
 
 
+@copy_kwargs(discord.abc.Messageable.send)
 async def info(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str,
+    *,
+    title: str | None = None,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send an info message. By default, this is a blue embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
         The text to send.
+    title:
+        The title of the embed. Defaults to ``None``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("info_embed")
-    await _process_message(target, embed, txt, ephemeral, **kwargs)
+    await _process_message(target, embed.copy(), txt, title, ephemeral, **kwargs)
 
 
+@copy_kwargs(discord.abc.Messageable.send)
 async def send(
     template: str,
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str,
+    *,
+    title: str | None = None,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send a custom embed template. This needs to be set up with :func:`set_embed_templates`.
 
     Parameters
     ----------
     template:
         The name of the template that was used in :func:`set_embed_templates`.
     target:
         The target to send the message to.
     txt:
         The text to send.
+    title:
+        The title of the embed. Defaults to ``None``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed(template)
-    await _process_message(target, embed, txt, ephemeral, **kwargs)
+    await _process_message(target, embed.copy(), txt, title, ephemeral, **kwargs)
```

### Comparing `ezcord-0.1.4/src/ezcord/internal/colors.py` & `ezcord-0.1.5/src/ezcord/internal/colors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.4/src/ezcord/internal/embed_templates.py` & `ezcord-0.1.5/src/ezcord/internal/embed_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import json
 import os
 from functools import cache
 from pathlib import Path
-from typing import Dict
 
 from discord import Color, Embed
 
-TEMPLATES: Dict[str, Embed] = {
+_TEMPLATES: dict[str, Embed] = {
     "success_embed": Embed(color=Color.green()),
     "error_embed": Embed(color=Color.red()),
     "warn_embed": Embed(color=Color.gold()),
     "info_embed": Embed(color=Color.blue()),
 }
 
 
 def save_embeds(**kwargs: Embed):
     """Save multiple embeds to a JSON file.
 
     If one of the default values is not included, a default template will be saved.
     """
     embeds = {}
-    overrides = TEMPLATES if len(kwargs) == 0 else kwargs
+    overrides = _TEMPLATES if len(kwargs) == 0 else kwargs
 
     for name, embed in overrides.items():
         if embed is None:
-            embeds[name] = TEMPLATES[name].to_dict()
+            embeds[name] = _TEMPLATES[name].to_dict()
         else:
             embeds[name] = embed.to_dict()
 
     parent = Path(__file__).parent.absolute()
     with open(os.path.join(parent, "embeds.json"), "w") as file:
         json.dump(embeds, file, indent=2)
 
@@ -43,12 +42,12 @@
 
     with open(os.path.join(parent, "embeds.json")) as file:
         embeds = json.load(file)
 
     try:
         return Embed.from_dict(embeds[name])
     except KeyError:
-        if name in TEMPLATES.keys():
+        if name in _TEMPLATES.keys():
             save_embeds()
             return load_embed()
         else:
             raise ValueError(f"Embed template '{name}' not found.")
```

### Comparing `ezcord-0.1.4/src/ezcord/internal/languages.py` & `ezcord-0.1.5/src/ezcord/internal/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.4/src/ezcord/internal/translation.py` & `ezcord-0.1.5/src/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.4/src/ezcord/logs.py` & `ezcord-0.1.5/src/ezcord/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,21 +43,21 @@
     color = get_escape_code(color)
     logging.getLogger(DEFAULT_LOG).log(level, message, extra={"key": key, "color": color})
 
 
 def _format_log_colors(log_format: str, file: bool, final_colors: dict[int, str]) -> dict[int, str]:
     """Checks if the is sent to a file and formats the colors accordingly."""
     color_formats = {}
-    if "{color_start}" in log_format and "{color_end}" in log_format:
+    if "{color}" in log_format and "{color_end}" in log_format:
         for level in final_colors:
             if file:
-                color_formats[level] = log_format.format(color_start="", color_end="")
+                color_formats[level] = log_format.format(color="", color_end="")
             else:
                 color_formats[level] = log_format.format(
-                    color_start=final_colors[level], color_end=Fore.RESET
+                    color=final_colors[level], color_end=Fore.RESET
                 )
     else:
         for level in final_colors:
             color_formats[level] = final_colors[level] + log_format + Fore.RESET
 
     return color_formats
 
@@ -141,14 +141,22 @@
 
         log_format = color_log_formats.get(record.levelno)
         if "key" in record.__dict__ and log_format:
             log_format = log_format.replace("%(levelname)s", record.__dict__["key"])
 
         current_level_color = color_formats.get(record.levelno)
         new_record = logging.makeLogRecord(record.__dict__)
+
+        # color new lines
+        if isinstance(log_format, str) and log_format.endswith("//"):
+            log_format = log_format.replace("//", "")
+            split = new_record.msg.split("\n", 1)
+            if len(split) > 1:
+                new_record.msg = split[0] + "\n**" + split[1] + "**"
+
         new_record.msg = replace_dc_format(new_record.msg, current_level_color)
 
         formatter = logging.Formatter(log_format, self.TIME_FORMAT)
         return formatter.format(new_record)
 
 
 class _DiscordHandler(logging.Handler):
@@ -198,14 +206,15 @@
         except discord.HTTPException:
             log.error(
                 "Error while sending log message to webhook. Please check if the URL is correct."
             )
 
 
 def _discord_filter(record):
+    """A filter that blocks logs that have already been sent to a Discord webhook."""
     if "webhook_sent" in record.__dict__:
         return not record.__dict__["webhook_sent"]
     return True
 
 
 def set_log(
     name: str = DEFAULT_LOG,
@@ -222,19 +231,19 @@
     """Creates a logger. If this logger already exists, it will return the existing logger.
 
     Parameters
     ----------
     name:
         The name of the logger.
     log_level:
-        Whether to enable debug logs. Defaults to ``logging.INFO``.
+        The log level for default log messages ``logging.DEBUG``.
     file:
         Whether to log to a file. Defaults to ``False``.
     log_format:
-        The log format. Defaults to :attr:`LogFormat.default`.
+        The log format. Defaults to :attr:`.LogFormat.default`.
     time_format:
         The time format. Defaults to ``%Y-%m-%d %H:%M:%S``.
     discord_log_level:
         The log level for discord log messages. Defaults to ``logging.WARNING``.
 
         .. note::
             For discord log messages, ``webhook_url`` is required.
```

### Comparing `ezcord-0.1.4/src/ezcord/times.py` & `ezcord-0.1.5/src/ezcord/times.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 from datetime import datetime, timedelta, timezone
 from typing import Literal
 
 from discord.utils import format_dt, utcnow
 
-from .internal.translation import tp
+from .internal import tp
 
 
 def set_utc(dt: datetime) -> datetime:
     """Set the timezone of a datetime object to UTC.
 
     Parameters
     ----------
@@ -97,15 +97,15 @@
     :class:`str`
         A Discord timestamp.
     """
     dt = utcnow() + timedelta(seconds=seconds)
     return format_dt(dt, style)
 
 
-def convert_to_seconds(s: str):
+def convert_to_seconds(s: str) -> int:
     """Convert a string to seconds.
 
     Parameters
     ----------
     s:
         The string to convert.
```

### Comparing `ezcord-0.1.4/src/ezcord/utils.py` & `ezcord-0.1.5/src/ezcord/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Some utility functions for Pycord and Python."""
 
 import io
 import json
-from typing import Dict
 
 import discord
 
 
-def create_json_file(dictionary: Dict, filename: str = "data.json", **kwargs):
+def create_json_file(dictionary: dict, filename: str = "data.json", **kwargs) -> discord.File:
     """Create a :class:`discord.File` object from a dictionary.
 
     Parameters
     ----------
     dictionary:
         The dictionary to convert to a JSON file.
     filename:
@@ -23,15 +22,15 @@
     -------
     :class:`discord.File`
     """
     content = json.dumps(dictionary, indent=2).encode()
     return discord.File(io.BytesIO(content), filename=filename, **kwargs)
 
 
-def create_text_file(text: str, filename: str = "data.txt", **kwargs):
+def create_text_file(text: str, filename: str = "data.txt", **kwargs) -> discord.File:
     """Create a :class:`discord.File` object from a string.
 
     Parameters
     ----------
     text:
         The string to convert to a text file.
     filename:
```

### Comparing `ezcord-0.1.4/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.1.5/src/ezcord.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.4
+Version: 0.1.5
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # EzCord
 [![](https://img.shields.io/discord/1010915072694046794?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/zfvbjTEzv6)
 [![](https://img.shields.io/pypi/v/ezcord.svg?style=for-the-badge&logo=pypi&color=yellow&logoColor=white)](https://pypi.org/project/ezcord/)
 [![](https://img.shields.io/pypi/l/ezcord?style=for-the-badge)]()
 [![](https://aschey.tech/tokei/github/tibue99/ezcord?style=for-the-badge)](https://github.com/tibue99/ezcord)
 
 An easy-to-use extension for the [Pycord](https://github.com/Pycord-Development/pycord) library with some utility functions.
 
 ## Installing
-Python 3.8 or higher is required.
+Python 3.9 or higher is required.
 ```
 pip install ezcord
 ```
 You can also install the latest version from GitHub. Note that this version may be unstable
 and requires [git](https://git-scm.com/downloads) to be installed.
 ```
 pip install git+https://github.com/tibue99/ezcord
```

