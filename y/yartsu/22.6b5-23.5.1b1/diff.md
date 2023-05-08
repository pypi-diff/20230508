# Comparing `tmp/yartsu-22.6b5.tar.gz` & `tmp/yartsu-23.5.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yartsu-22.6b5.tar", last modified: Sat Jun 18 21:57:23 2022, max compression
+gzip compressed data, was "yartsu-23.5.1b1.tar", last modified: Mon May  8 04:53:45 2023, max compression
```

## Comparing `yartsu-22.6b5.tar` & `yartsu-23.5.1b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1070 2022-06-15 06:40:10.603873 yartsu-22.6b5/LICENSE.txt
--rw-r--r--   0 daylin    (1000) daylin    (1000)     4641 2022-06-18 21:55:13.908275 yartsu-22.6b5/README.md
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1113 2022-06-15 06:07:31.922178 yartsu-22.6b5/pyproject.toml
--rw-r--r--   0 daylin    (1000) daylin    (1000)       34 2022-06-14 21:01:45.894693 yartsu-22.6b5/yartsu/__init__.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1752 2022-06-18 21:52:48.397277 yartsu-22.6b5/yartsu/_export_format.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1874 2022-06-14 22:06:07.201743 yartsu-22.6b5/yartsu/_run_cmd.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)      144 2022-06-14 21:35:42.763819 yartsu-22.6b5/yartsu/_version.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     6004 2022-06-14 23:17:17.341178 yartsu-22.6b5/yartsu/argparse.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     3766 2022-06-16 18:28:36.031173 yartsu-22.6b5/yartsu/cli.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     9380 2022-06-18 21:52:48.397277 yartsu-22.6b5/yartsu/console.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1581 2022-06-14 23:17:17.527846 yartsu-22.6b5/yartsu/term.py
--rw-r--r--   0 daylin    (1000) daylin    (1000)     7378 2022-06-15 18:28:01.120518 yartsu-22.6b5/yartsu/themes.py
--rw-------   0 daylin    (1000) daylin    (1000)     6091 2022-06-18 21:57:23.877062 yartsu-22.6b5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-06-15 06:40:10.603873 yartsu-23.5.1b1/LICENSE.txt
+-rw-r--r--   0        0        0     5053 2022-06-19 20:28:23.781090 yartsu-23.5.1b1/README.md
+-rw-r--r--   0        0        0     1235 2023-05-08 04:38:38.657870 yartsu-23.5.1b1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-08 04:41:33.843492 yartsu-23.5.1b1/yartsu/__init__.py
+-rw-r--r--   0        0        0     1917 2023-05-08 04:40:01.525340 yartsu-23.5.1b1/yartsu/_export_format.py
+-rw-r--r--   0        0        0     1874 2022-06-14 22:06:07.201743 yartsu-23.5.1b1/yartsu/_run_cmd.py
+-rw-r--r--   0        0        0      144 2023-05-08 04:44:17.329555 yartsu-23.5.1b1/yartsu/_version.py
+-rw-r--r--   0        0        0     6055 2023-05-08 04:38:38.707871 yartsu-23.5.1b1/yartsu/argparse.py
+-rw-r--r--   0        0        0     3794 2023-05-08 04:38:38.707871 yartsu-23.5.1b1/yartsu/cli.py
+-rw-r--r--   0        0        0    10080 2023-05-08 04:43:18.898680 yartsu-23.5.1b1/yartsu/console.py
+-rw-r--r--   0        0        0     1580 2023-05-08 04:38:38.707871 yartsu-23.5.1b1/yartsu/term.py
+-rw-r--r--   0        0        0     7378 2022-06-15 18:28:01.120518 yartsu-23.5.1b1/yartsu/themes.py
+-rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 yartsu-23.5.1b1/PKG-INFO
```

### Comparing `yartsu-22.6b5/LICENSE.txt` & `yartsu-23.5.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yartsu-22.6b5/README.md` & `yartsu-23.5.1b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -109,21 +109,25 @@
 Currently `yartsu` loads the `nerd font` patched FiraCode font.
 This should result in general support for emoji's and `nerd font` icons.
 
 <div align="center"><img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/demo.svg" alt="Logo" width=400 ></div>
 
 **Note**: github won't load the font's when displaying on the README. Click on the `svg` to see the `nerd font` icons.
 
+### Differences from [`Rich`](https://github.com/Textualize/rich)
 
-## TODO
+For both practical and stylistic reasons the underlying code used to generate the SVG is slightly different than `rich`'s default `save_svg` method. See [here](https://github.com/daylinmorgan/yartsu/blob/main/docs/rich-diff.md) for the current deviation between the latest releases of each respective release.
+
+
+## TODO (for stable release)
 
-- [ ] add unit tests
 - [x] add support for nerd-fonts
 - [x] add ~~optional~~ shadow
-- [ ] add more themes
+- [ ] add unit tests
+- [ ] setup CI for release/testing
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 [contributors-shield]: https://img.shields.io/github/contributors/daylinmorgan/yartsu.svg?style=flat
 [contributors-url]: https://github.com/daylinmorgan/yartsu/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/daylinmorgan/yartsu.svg?style=flat
 [forks-url]: https://github.com/daylinmorgan/yartsu/network/members
```

#### html2text {}

```diff
@@ -40,20 +40,25 @@
 use the environment variable `YARTSU_THEME`. See [here](https://github.com/
 daylinmorgan/yartsu/blob/main/docs/themes.md) a preview of the available themes
 ### Supported Characters Currently `yartsu` loads the `nerd font` patched
 FiraCode font. This should result in general support for emoji's and `nerd
 font` icons.
                                     [Logo]
 **Note**: github won't load the font's when displaying on the README. Click on
-the `svg` to see the `nerd font` icons. ## TODO - [ ] add unit tests - [x] add
-support for nerd-fonts - [x] add ~~optional~~ shadow - [ ] add more themes
-[contributors-shield]: https://img.shields.io/github/contributors/daylinmorgan/
-yartsu.svg?style=flat [contributors-url]: https://github.com/daylinmorgan/
-yartsu/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
-daylinmorgan/yartsu.svg?style=flat [forks-url]: https://github.com/
-daylinmorgan/yartsu/network/members [stars-shield]: https://img.shields.io/
-github/stars/daylinmorgan/yartsu.svg?style=flat [stars-url]: https://
-github.com/daylinmorgan/yartsu/stargazers [issues-shield]: https://
-img.shields.io/github/issues/daylinmorgan/yartsu.svg?style=flat [issues-url]:
+the `svg` to see the `nerd font` icons. ### Differences from [`Rich`](https://
+github.com/Textualize/rich) For both practical and stylistic reasons the
+underlying code used to generate the SVG is slightly different than `rich`'s
+default `save_svg` method. See [here](https://github.com/daylinmorgan/yartsu/
+blob/main/docs/rich-diff.md) for the current deviation between the latest
+releases of each respective release. ## TODO (for stable release) - [x] add
+support for nerd-fonts - [x] add ~~optional~~ shadow - [ ] add unit tests - [ ]
+setup CI for release/testing  [contributors-shield]: https://img.shields.io/
+github/contributors/daylinmorgan/yartsu.svg?style=flat [contributors-url]:
+https://github.com/daylinmorgan/yartsu/graphs/contributors [forks-shield]:
+https://img.shields.io/github/forks/daylinmorgan/yartsu.svg?style=flat [forks-
+url]: https://github.com/daylinmorgan/yartsu/network/members [stars-shield]:
+https://img.shields.io/github/stars/daylinmorgan/yartsu.svg?style=flat [stars-
+url]: https://github.com/daylinmorgan/yartsu/stargazers [issues-shield]: https:
+//img.shields.io/github/issues/daylinmorgan/yartsu.svg?style=flat [issues-url]:
 https://github.com/daylinmorgan/yartsu/issues [license-shield]: https://
 img.shields.io/github/license/daylinmorgan/yartsu.svg?style=flat [license-url]:
 https://github.com/daylinmorgan/yartsu/blob/main/LICENSE.txt
```

### Comparing `yartsu-22.6b5/pyproject.toml` & `yartsu-23.5.1b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,55 +2,68 @@
 name = "yartsu"
 description = "yartsu, another rich terminal screenshot utility"
 authors = [
     { name = "Daylin Morgan", email = "daylinmorgan@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
-    "rich>=12.3.0",
+    "rich>=13.3.5",
     "importlib-metadata>=4.11.4; python_version < \"3.8\"",
 ]
 requires-python = ">=3.7"
 dynamic = []
-version = "22.6b5"
+version = "23.5.1b1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/daylinmorgan/yartsu"
 Repository = "https://github.com/daylinmorgan/yartsu"
 
 [project.scripts]
 yartsu = "yartsu.cli:main"
 
-[project.optional-dependencies]
-
 [tool.pdm.version]
-use_scm = true
+source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit>=2.18.1",
     "mypy>=0.961",
 ]
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-
 [tool.mypy]
 check_untyped_defs = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 disallow_any_unimported = true
 warn_return_any = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
+[tool.ruff]
+select = [
+    "F",
+    "E",
+    "W",
+    "I001",
+]
+exclude = [
+    "scripts",
+]
+
+[tool.ruff.per-file-ignores]
+"yartsu/_export_format.py" = [
+    "E501",
+]
+"yartsu/console.py" = [
+    "E501",
+]
+
 [build-system]
 requires = [
     "pdm-pep517>=0.12.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `yartsu-22.6b5/yartsu/_export_format.py` & `yartsu-23.5.1b1/yartsu/_export_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 CONSOLE_SVG_FORMAT = """\
 <svg class="rich-terminal shadow" viewBox="0 0 {width} {height}" xmlns="http://www.w3.org/2000/svg">
-    <!-- Generated with Rich https://www.textualize.io -->
+    <!-- Generated with Rich https://www.textualize.io & yartsu https://github.com/daylinmorgan/yartsu -->
     <style>
+
     @font-face {{
         font-family: "Fira Code";
         src: local("FiraCode-Regular"),
-            url("https://cdn.jsdelivr.net/gh/ryanoasis/nerd-fonts@2.1.0/patched-fonts/FiraCode/Regular/complete/Fira%20Code%20Regular%20Nerd%20Font%20Complete.ttf") format("truetype");
+                url("https://cdnjs.cloudflare.com/ajax/libs/firacode/6.2.0/woff2/FiraCode-Regular.woff2") format("woff2"),
+                url("https://cdnjs.cloudflare.com/ajax/libs/firacode/6.2.0/woff/FiraCode-Regular.woff") format("woff");
         font-style: normal;
         font-weight: 400;
     }}
     @font-face {{
         font-family: "Fira Code";
         src: local("FiraCode-Bold"),
-            url("https://cdn.jsdelivr.net/gh/ryanoasis/nerd-fonts@2.1.0/patched-fonts/FiraCode/Bold/complete/Fira%20Code%20Bold%20Nerd%20Font%20Complete.ttf") format("truetype");
+                url("https://cdnjs.cloudflare.com/ajax/libs/firacode/6.2.0/woff2/FiraCode-Bold.woff2") format("woff2"),
+                url("https://cdnjs.cloudflare.com/ajax/libs/firacode/6.2.0/woff/FiraCode-Bold.woff") format("woff");
         font-style: bold;
         font-weight: 700;
     }}
 
     .{unique_id}-matrix {{
         font-family: Fira Code, monospace;
         font-size: {char_height}px;
```

### Comparing `yartsu-22.6b5/yartsu/_run_cmd.py` & `yartsu-23.5.1b1/yartsu/_run_cmd.py`

 * *Files identical despite different names*

### Comparing `yartsu-22.6b5/yartsu/argparse.py` & `yartsu-23.5.1b1/yartsu/argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,18 @@
         if not action.help:
             tup = self._current_indent, "", action_header
             action_header = "%*s%s\n" % tup
 
         # short action name; start on the same line and pad two spaces
         elif action_header_len <= action_width:
             tup = self._current_indent, "", action_width, action_header
-            action_header = f"{' '*self._current_indent}{action_header}{' '*(action_width+2 - action_header_len)}"
+            action_header = (
+                f"{' '*self._current_indent}{action_header}"
+                f"{' '*(action_width+2 - action_header_len)}"
+            )
             indent_first = 0
 
         # long action name; start on the next line
         else:
             tup = self._current_indent, "", action_header
             action_header = "%*s%s\n" % tup
             indent_first = help_position
@@ -110,15 +113,14 @@
         elif action.nargs == ONE_OR_MORE:
             return "%s ..." % get_metavar(1)
         else:
             return super()._format_args(action, default_metavar)
 
     def add_argument(self, action: Action) -> None:
         if action.help is not SUPPRESS:
-
             # find all invocations
             get_invocation = self._format_action_invocation
             invocations = [get_invocation(action)]
             for subaction in self._iter_indented_subactions(action):
                 invocations.append(get_invocation(subaction))
 
             # update the maximum item length accounting for ansi codes from rich
```

### Comparing `yartsu-22.6b5/yartsu/cli.py` & `yartsu-23.5.1b1/yartsu/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 import textwrap
-from argparse import SUPPRESS, FileType, Namespace
+from argparse import SUPPRESS, FileType
 from pathlib import Path
 
 from rich.__main__ import make_test_card
 from rich.text import Text
 
 from ._export_format import CONSOLE_SVG_FORMAT
 from ._run_cmd import run_cmd
@@ -14,16 +14,15 @@
 from .console import Console
 from .term import term
 from .themes import THEMES
 
 DEFAULT_THEME = os.getenv("YARTSU_THEME", "cat-mocha")
 
 
-def get_args() -> Namespace:
-
+def get_parser() -> ArgumentParser:
     parser = ArgumentParser(
         usage=SUPPRESS,
         description=textwrap.dedent(
             r"""
         [header]usage[/]:
 
         convert terminal output to svg
@@ -63,33 +62,35 @@
         type=str,
         default=DEFAULT_THEME,
     )
     parser.add_argument(
         "--list-themes", help="list available themes", action="store_true"
     )
     parser.add_argument("--demo", help=SUPPRESS, action="store_true")
-    return parser.parse_args()
+    return parser
 
 
 def main() -> None:
-    args = get_args()
+    parser = get_parser()
+    args = parser.parse_args()
     console = Console(record=True)
 
     if args.list_themes:
         term.print("Available themes:")
         term.print("\n".join(["  - " + theme for theme in THEMES]))
         sys.exit(0)
 
     if args.cmd and args.input or not (args.cmd or args.input or args.demo):
         term.print(
             "[UsageError]: either use the --input option "
             "OR pipe terminal output to yartsu",
             err=True,
         )
-        term.print("See 'yartsu --help' for more information", err=True)
+        term.print("See below for more information:\n")
+        parser.print_help()
         sys.exit(1)
 
     if args.theme not in THEMES:
         term.print(f"[ThemeError]: {args.theme} is not a valid theme", err=True)
         sys.exit(1)
 
     if args.cmd:
```

### Comparing `yartsu-22.6b5/yartsu/console.py` & `yartsu-23.5.1b1/yartsu/console.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,26 +16,32 @@
     def export_svg(
         self,
         *,
         title: str = "Rich",
         theme: Optional[TerminalTheme] = None,
         clear: bool = True,
         code_format: str = CONSOLE_SVG_FORMAT,
+        font_aspect_ratio: float = 0.61,
+        unique_id: Optional[str] = None,
     ) -> str:
         """
         Generate an SVG from the console contents (requires record=True in Console constructor).
 
         Args:
-            path (str): The path to write the SVG to.
-            title (str): The title of the tab in the output image
+            title (str, optional): The title of the tab in the output image
             theme (TerminalTheme, optional): The ``TerminalTheme`` object to use to style the terminal
             clear (bool, optional): Clear record buffer after exporting. Defaults to ``True``
-            code_format (str): Format string used to generate the SVG. Rich will inject a number of variables
+            code_format (str, optional): Format string used to generate the SVG. Rich will inject a number of variables
                 into the string in order to form the final SVG output. The default template used and the variables
                 injected by Rich can be found by inspecting the ``console.CONSOLE_SVG_FORMAT`` variable.
+            font_aspect_ratio (float, optional): The width to height ratio of the font used in the ``code_format``
+                string. Defaults to 0.61, which is the width to height ratio of Fira Code (the default font).
+                If you aren't specifying a different font inside ``code_format``, you probably don't need this.
+            unique_id (str, optional): unique id that is used as the prefix for various elements (CSS styles, node
+                ids). If not set, this defaults to a computed value based on the recorded content.
         """
 
         from rich.cells import cell_len
 
         style_cache: Dict[Style, str] = {}
 
         def get_svg_style(style: Style) -> str:
@@ -71,15 +77,15 @@
             style_cache[style] = css
             return css
 
         _theme = theme or SVG_EXPORT_THEME
 
         width = self.width
         char_height = 20
-        char_width = char_height * 0.61
+        char_width = char_height * font_aspect_ratio
         line_height = char_height * 1.22
 
         margin_top = 1
         margin_right = char_width * 5 / 6
         margin_bottom = 20 * 5 / 3
         margin_left = char_width * 5 / 6
 
@@ -123,22 +129,24 @@
             )
 
         with self._record_buffer_lock:
             segments = list(Segment.filter_control(self._record_buffer))
             if clear:
                 self._record_buffer.clear()
 
-        unique_id = "terminal-" + str(
-            zlib.adler32(
-                ("".join(segment.text for segment in segments)).encode(
-                    "utf-8", "ignore"
+        if unique_id is None:
+            unique_id = "terminal-" + str(
+                zlib.adler32(
+                    ("".join(repr(segment) for segment in segments)).encode(
+                        "utf-8",
+                        "ignore",
+                    )
+                    + title.encode("utf-8", "ignore")
                 )
-                + title.encode("utf-8", "ignore")
             )
-        )
         y = 0
         for y, line in enumerate(Segment.split_and_crop_lines(segments, length=width)):
             x = 0
             for text, style, _control in line:
                 style = style or Style()
                 rules = get_svg_style(style)
                 if rules not in classes:
```

### Comparing `yartsu-22.6b5/yartsu/term.py` & `yartsu-23.5.1b1/yartsu/term.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 
 theme = Theme({"header": "bold cyan", "option": "yellow", "metavar": "green"})
 
 
 class Term:
     def __init__(self, width: int) -> None:
-
         self.console = Console(highlight=False, theme=theme, width=width)
         self.err_console = Console(
             theme=Theme({"error": "bold red"}, inherit=True),
             stderr=True,
             highlighter=ErrorHighlighter(),
             width=width,
         )
```

### Comparing `yartsu-22.6b5/yartsu/themes.py` & `yartsu-23.5.1b1/yartsu/themes.py`

 * *Files identical despite different names*

### Comparing `yartsu-22.6b5/PKG-INFO` & `yartsu-23.5.1b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,146 +1,151 @@
 Metadata-Version: 2.1
 Name: yartsu
-Version: 22.6b5
+Version: 23.5.1b1
 Summary: yartsu, another rich terminal screenshot utility
 License: MIT
 Author-email: Daylin Morgan <daylinmorgan@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Homepage, https://github.com/daylinmorgan/yartsu
 Project-URL: Repository, https://github.com/daylinmorgan/yartsu
 Description-Content-Type: text/markdown
-Description: # YARTSU
-        
-        
-        <div id="top"></div>
-        
-        <!-- PROJECT LOGO -->
-        <div align="center">
-          <a href="https://github.com/daylinmorgan/yartsu">
-            <img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/logo.svg" alt="Logo" width=600 >
-          </a>
-          <p align="center">
-            yartsu, another rich terminal screenshot utility
-          </p>
-        </div>
-        <br />
-        
-        <!-- PROJECT SHIELDS -->
-        [![Stargazers][stars-shield]][stars-url]
-        [![Issues][issues-shield]][issues-url]
-        [![MIT License][license-shield]][license-url]
-        
-        
-        
-        **NOTE**: this is a currently in a beta release and the API is subject to change (feedback welcome)
-        
-        Inspired by recent commits in the wonderful library [`rich`](https://github.com/Textualize/rich) I decided to write ` yartsu`.
-        
-        I needed to programmatically generate screenshots for documentation purposes. The new `export_svg` methods in `rich` were a godsend.
-        So I wanted to try to make this feature a little more generalizable to program output outside of `rich`/`python`.
-        Hopefully, you find it useful.
-        
-        If you come across anything unexpected please submit an issue.
-        
-        ## Install
-        
-        ```bash
-        pip install yartsu
-        ```
-        
-        There is a standalone binary available for linux in the [releases](https://github.com/daylinmorgan/yartsu/releases).
-        
-        Optionally install with [`eget`](https://github.com/zyedidia/eget):
-        
-        ```bash
-        eget daylinmorgan/yartsu
-        ```
-        
-        Otherwise you can download an extract manually to somewhere on your path.
-        
-        ## Usage
-        
-        <div align="center"><img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/help.svg" alt="Logo" width=600 ></div>
-        
-        Getting a properly formatted output from a terminal screenshot is challenging.
-        
-        There are three options for generating a screenshot.
-        
-        If one of the below option causes you any headaches consider first trying a different option.
-        
-        ### Option 1: Pipes
-        
-        Many tools that color output (i.e. `grep` or `ls`) additionally allow
-        you to force ANSI color codes to be included even when piping output.
-        
-        In these cases you can simply pipe the output directly into `yartsu`
-        
-        ```bash
-        ls --color=always | yartsu -w 50 -o assets/ls_color.svg
-        ```
-        
-        ### Option 2: Subprocess/Pty
-        
-        With this option `yartsu` will deploy a `subprocess` and `pty`
-        to run your command for you in an attempt to preserve ANSI.
-        
-        Note with this option you need to separate
-        the command you want to run with `yartsu` args using `--`.
-        
-        ```bash
-        yartsu -w 50 -o assets/ls_color.svg -- ls --color /
-        ```
-        
-        ### Option 3: Text File
-        
-        Finally, if you neither of the above options work and you can
-        manage to preserve the codes in a plain text file you can pass this as input to `yartsu`.
-        
-        ```bash
-        ls --color > ls.txt
-        yartsu -w 50 -i ls.txt -o assets/ls_color.svg
-        ```
-        
-        By default svgs will be saved at `./capture.svg`.
-        
-        Additionally, for options 1 and 3 you may want to define your own title with `-t/--title`.
-        For option 2 the title will by default be the cmd ran by `yartsu`.
-        
-        ### Themes:
-        
-        There are a number of themes you can use to style output.
-        Use `yartsu --list-themes` to see the available options.
-        Then you can specify the theme you want with `--theme`, i.e. `yartsu --theme rich_default`.
-        You may also use the environment variable `YARTSU_THEME`.
-        
-        See [here](https://github.com/daylinmorgan/yartsu/blob/main/docs/themes.md) a preview of the available themes
-        
-        ### Supported Characters
-        
-        Currently `yartsu` loads the `nerd font` patched FiraCode font.
-        This should result in general support for emoji's and `nerd font` icons.
-        
-        <div align="center"><img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/demo.svg" alt="Logo" width=400 ></div>
-        
-        **Note**: github won't load the font's when displaying on the README. Click on the `svg` to see the `nerd font` icons.
-        
-        
-        ## TODO
-        
-        - [ ] add unit tests
-        - [x] add support for nerd-fonts
-        - [x] add ~~optional~~ shadow
-        - [ ] add more themes
-        
-        
-        <!-- MARKDOWN LINKS & IMAGES -->
-        [contributors-shield]: https://img.shields.io/github/contributors/daylinmorgan/yartsu.svg?style=flat
-        [contributors-url]: https://github.com/daylinmorgan/yartsu/graphs/contributors
-        [forks-shield]: https://img.shields.io/github/forks/daylinmorgan/yartsu.svg?style=flat
-        [forks-url]: https://github.com/daylinmorgan/yartsu/network/members
-        [stars-shield]: https://img.shields.io/github/stars/daylinmorgan/yartsu.svg?style=flat
-        [stars-url]: https://github.com/daylinmorgan/yartsu/stargazers
-        [issues-shield]: https://img.shields.io/github/issues/daylinmorgan/yartsu.svg?style=flat
-        [issues-url]: https://github.com/daylinmorgan/yartsu/issues
-        [license-shield]: https://img.shields.io/github/license/daylinmorgan/yartsu.svg?style=flat
-        [license-url]: https://github.com/daylinmorgan/yartsu/blob/main/LICENSE.txt
+
+# YARTSU
+
+
+<div id="top"></div>
+
+<!-- PROJECT LOGO -->
+<div align="center">
+  <a href="https://github.com/daylinmorgan/yartsu">
+    <img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/logo.svg" alt="Logo" width=600 >
+  </a>
+  <p align="center">
+    yartsu, another rich terminal screenshot utility
+  </p>
+</div>
+<br />
+
+<!-- PROJECT SHIELDS -->
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+
+
+
+**NOTE**: this is a currently in a beta release and the API is subject to change (feedback welcome)
+
+Inspired by recent commits in the wonderful library [`rich`](https://github.com/Textualize/rich) I decided to write ` yartsu`.
+
+I needed to programmatically generate screenshots for documentation purposes. The new `export_svg` methods in `rich` were a godsend.
+So I wanted to try to make this feature a little more generalizable to program output outside of `rich`/`python`.
+Hopefully, you find it useful.
+
+If you come across anything unexpected please submit an issue.
+
+## Install
+
+```bash
+pip install yartsu
+```
+
+There is a standalone binary available for linux in the [releases](https://github.com/daylinmorgan/yartsu/releases).
+
+Optionally install with [`eget`](https://github.com/zyedidia/eget):
+
+```bash
+eget daylinmorgan/yartsu
+```
+
+Otherwise you can download an extract manually to somewhere on your path.
+
+## Usage
+
+<div align="center"><img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/help.svg" alt="Logo" width=600 ></div>
+
+Getting a properly formatted output from a terminal screenshot is challenging.
+
+There are three options for generating a screenshot.
+
+If one of the below option causes you any headaches consider first trying a different option.
+
+### Option 1: Pipes
+
+Many tools that color output (i.e. `grep` or `ls`) additionally allow
+you to force ANSI color codes to be included even when piping output.
+
+In these cases you can simply pipe the output directly into `yartsu`
+
+```bash
+ls --color=always | yartsu -w 50 -o assets/ls_color.svg
+```
+
+### Option 2: Subprocess/Pty
+
+With this option `yartsu` will deploy a `subprocess` and `pty`
+to run your command for you in an attempt to preserve ANSI.
+
+Note with this option you need to separate
+the command you want to run with `yartsu` args using `--`.
+
+```bash
+yartsu -w 50 -o assets/ls_color.svg -- ls --color /
+```
+
+### Option 3: Text File
+
+Finally, if you neither of the above options work and you can
+manage to preserve the codes in a plain text file you can pass this as input to `yartsu`.
+
+```bash
+ls --color > ls.txt
+yartsu -w 50 -i ls.txt -o assets/ls_color.svg
+```
+
+By default svgs will be saved at `./capture.svg`.
+
+Additionally, for options 1 and 3 you may want to define your own title with `-t/--title`.
+For option 2 the title will by default be the cmd ran by `yartsu`.
+
+### Themes:
+
+There are a number of themes you can use to style output.
+Use `yartsu --list-themes` to see the available options.
+Then you can specify the theme you want with `--theme`, i.e. `yartsu --theme rich_default`.
+You may also use the environment variable `YARTSU_THEME`.
+
+See [here](https://github.com/daylinmorgan/yartsu/blob/main/docs/themes.md) a preview of the available themes
+
+### Supported Characters
+
+Currently `yartsu` loads the `nerd font` patched FiraCode font.
+This should result in general support for emoji's and `nerd font` icons.
+
+<div align="center"><img src="https://raw.githubusercontent.com/daylinmorgan/yartsu/main/assets/demo.svg" alt="Logo" width=400 ></div>
+
+**Note**: github won't load the font's when displaying on the README. Click on the `svg` to see the `nerd font` icons.
+
+### Differences from [`Rich`](https://github.com/Textualize/rich)
+
+For both practical and stylistic reasons the underlying code used to generate the SVG is slightly different than `rich`'s default `save_svg` method. See [here](https://github.com/daylinmorgan/yartsu/blob/main/docs/rich-diff.md) for the current deviation between the latest releases of each respective release.
+
+
+## TODO (for stable release)
+
+- [x] add support for nerd-fonts
+- [x] add ~~optional~~ shadow
+- [ ] add unit tests
+- [ ] setup CI for release/testing
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+[contributors-shield]: https://img.shields.io/github/contributors/daylinmorgan/yartsu.svg?style=flat
+[contributors-url]: https://github.com/daylinmorgan/yartsu/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/daylinmorgan/yartsu.svg?style=flat
+[forks-url]: https://github.com/daylinmorgan/yartsu/network/members
+[stars-shield]: https://img.shields.io/github/stars/daylinmorgan/yartsu.svg?style=flat
+[stars-url]: https://github.com/daylinmorgan/yartsu/stargazers
+[issues-shield]: https://img.shields.io/github/issues/daylinmorgan/yartsu.svg?style=flat
+[issues-url]: https://github.com/daylinmorgan/yartsu/issues
+[license-shield]: https://img.shields.io/github/license/daylinmorgan/yartsu.svg?style=flat
+[license-url]: https://github.com/daylinmorgan/yartsu/blob/main/LICENSE.txt
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: yartsu Version: 22.6b5 Summary: yartsu, another
+Metadata-Version: 2.1 Name: yartsu Version: 23.5.1b1 Summary: yartsu, another
 rich terminal screenshot utility License: MIT Author-email: Daylin Morgan
 gmail.com> Requires-Python: >=3.7 Project-URL: Homepage, https://github.com/
 daylinmorgan/yartsu Project-URL: Repository, https://github.com/daylinmorgan/
-yartsu Description-Content-Type: text/markdown Description: # YARTSU
+yartsu Description-Content-Type: text/markdown # YARTSU
                                     [Logo]
                yartsu, another rich terminal screenshot utility
 
  [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-
 url] [![MIT License][license-shield]][license-url] **NOTE**: this is a
 currently in a beta release and the API is subject to change (feedback welcome)
 Inspired by recent commits in the wonderful library [`rich`](https://
@@ -44,20 +44,25 @@
 use the environment variable `YARTSU_THEME`. See [here](https://github.com/
 daylinmorgan/yartsu/blob/main/docs/themes.md) a preview of the available themes
 ### Supported Characters Currently `yartsu` loads the `nerd font` patched
 FiraCode font. This should result in general support for emoji's and `nerd
 font` icons.
                                     [Logo]
 **Note**: github won't load the font's when displaying on the README. Click on
-the `svg` to see the `nerd font` icons. ## TODO - [ ] add unit tests - [x] add
-support for nerd-fonts - [x] add ~~optional~~ shadow - [ ] add more themes
-[contributors-shield]: https://img.shields.io/github/contributors/daylinmorgan/
-yartsu.svg?style=flat [contributors-url]: https://github.com/daylinmorgan/
-yartsu/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
-daylinmorgan/yartsu.svg?style=flat [forks-url]: https://github.com/
-daylinmorgan/yartsu/network/members [stars-shield]: https://img.shields.io/
-github/stars/daylinmorgan/yartsu.svg?style=flat [stars-url]: https://
-github.com/daylinmorgan/yartsu/stargazers [issues-shield]: https://
-img.shields.io/github/issues/daylinmorgan/yartsu.svg?style=flat [issues-url]:
+the `svg` to see the `nerd font` icons. ### Differences from [`Rich`](https://
+github.com/Textualize/rich) For both practical and stylistic reasons the
+underlying code used to generate the SVG is slightly different than `rich`'s
+default `save_svg` method. See [here](https://github.com/daylinmorgan/yartsu/
+blob/main/docs/rich-diff.md) for the current deviation between the latest
+releases of each respective release. ## TODO (for stable release) - [x] add
+support for nerd-fonts - [x] add ~~optional~~ shadow - [ ] add unit tests - [ ]
+setup CI for release/testing  [contributors-shield]: https://img.shields.io/
+github/contributors/daylinmorgan/yartsu.svg?style=flat [contributors-url]:
+https://github.com/daylinmorgan/yartsu/graphs/contributors [forks-shield]:
+https://img.shields.io/github/forks/daylinmorgan/yartsu.svg?style=flat [forks-
+url]: https://github.com/daylinmorgan/yartsu/network/members [stars-shield]:
+https://img.shields.io/github/stars/daylinmorgan/yartsu.svg?style=flat [stars-
+url]: https://github.com/daylinmorgan/yartsu/stargazers [issues-shield]: https:
+//img.shields.io/github/issues/daylinmorgan/yartsu.svg?style=flat [issues-url]:
 https://github.com/daylinmorgan/yartsu/issues [license-shield]: https://
 img.shields.io/github/license/daylinmorgan/yartsu.svg?style=flat [license-url]:
 https://github.com/daylinmorgan/yartsu/blob/main/LICENSE.txt
```

