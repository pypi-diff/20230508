# Comparing `tmp/mecha-0.9.1.tar.gz` & `tmp/mecha-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecha-0.9.1.tar", last modified: Tue Nov 16 02:15:47 2021, max compression
+gzip compressed data, was "mecha-0.9.2.tar", last modified: Tue Nov 16 02:58:46 2021, max compression
```

## Comparing `mecha-0.9.1.tar` & `mecha-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2021-11-16 02:15:18.886854 mecha-0.9.1/LICENSE
--rw-r--r--   0        0        0     3927 2021-11-16 02:15:18.890854 mecha-0.9.1/README.md
--rw-r--r--   0        0        0      317 2021-11-16 02:15:44.960615 mecha-0.9.1/mecha/__init__.py
--rw-r--r--   0        0        0    14085 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/api.py
--rw-r--r--   0        0        0    15458 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/ast.py
--rw-r--r--   0        0        0     4662 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/config.py
--rw-r--r--   0        0        0        0 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/contrib/__init__.py
--rw-r--r--   0        0        0     1373 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/contrib/annotate_diagnostics.py
--rw-r--r--   0        0        0      178 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/contrib/clear_diagnostics.py
--rw-r--r--   0        0        0     2749 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/contrib/lint_basic.py
--rw-r--r--   0        0        0     2862 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/contrib/messages.py
--rw-r--r--   0        0        0     1562 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/contrib/relative_location.py
--rw-r--r--   0        0        0     2641 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/database.py
--rw-r--r--   0        0        0     5405 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/diagnostic.py
--rw-r--r--   0        0        0    10180 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/dispatch.py
--rw-r--r--   0        0        0      106 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/error.py
--rw-r--r--   0        0        0    59200 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/parse.py
--rw-r--r--   0        0        0      195 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/plugin.py
--rw-r--r--   0        0        0      960 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/prototype.py
--rw-r--r--   0        0        0        0 2021-11-16 02:15:18.890854 mecha-0.9.1/mecha/py.typed
--rw-r--r--   0        0        0   257142 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/1_16.json
--rw-r--r--   0        0        0   266016 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/1_17.json
--rw-r--r--   0        0        0   266263 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/1_18.json
--rw-r--r--   0        0        0      630 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/__init__.py
--rw-r--r--   0        0        0    12112 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/argument_examples.json
--rw-r--r--   0        0        0     6069 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/command_examples.mcfunction
--rw-r--r--   0        0        0     1948 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/resources/multiline_command_examples.mcfunction
--rw-r--r--   0        0        0     7501 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/serialize.py
--rw-r--r--   0        0        0     3181 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/spec.py
--rw-r--r--   0        0        0     5421 2021-11-16 02:15:18.894854 mecha-0.9.1/mecha/utils.py
--rw-r--r--   0        0        0     1263 2021-11-16 02:15:44.968615 mecha-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4734 2021-11-16 02:15:47.150541 mecha-0.9.1/setup.py
--rw-r--r--   0        0        0     4662 2021-11-16 02:15:47.151382 mecha-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-11-16 02:58:02.485801 mecha-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3927 2021-11-16 02:58:02.485801 mecha-0.9.2/README.md
+-rw-r--r--   0        0        0      317 2021-11-16 02:58:44.386274 mecha-0.9.2/mecha/__init__.py
+-rw-r--r--   0        0        0    14085 2021-11-16 02:58:02.485801 mecha-0.9.2/mecha/api.py
+-rw-r--r--   0        0        0    15458 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/ast.py
+-rw-r--r--   0        0        0     4662 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/config.py
+-rw-r--r--   0        0        0        0 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/contrib/__init__.py
+-rw-r--r--   0        0        0     1430 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/contrib/annotate_diagnostics.py
+-rw-r--r--   0        0        0      178 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/contrib/clear_diagnostics.py
+-rw-r--r--   0        0        0     2749 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/contrib/lint_basic.py
+-rw-r--r--   0        0        0     2862 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/contrib/messages.py
+-rw-r--r--   0        0        0     1562 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/contrib/relative_location.py
+-rw-r--r--   0        0        0     2641 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/database.py
+-rw-r--r--   0        0        0     5405 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/diagnostic.py
+-rw-r--r--   0        0        0    10180 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/dispatch.py
+-rw-r--r--   0        0        0      106 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/error.py
+-rw-r--r--   0        0        0    59200 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/parse.py
+-rw-r--r--   0        0        0      195 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/plugin.py
+-rw-r--r--   0        0        0      960 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/prototype.py
+-rw-r--r--   0        0        0        0 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/py.typed
+-rw-r--r--   0        0        0   257142 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/resources/1_16.json
+-rw-r--r--   0        0        0   266016 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/resources/1_17.json
+-rw-r--r--   0        0        0   266263 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/resources/1_18.json
+-rw-r--r--   0        0        0      630 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/resources/__init__.py
+-rw-r--r--   0        0        0    12112 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/resources/argument_examples.json
+-rw-r--r--   0        0        0     6069 2021-11-16 02:58:02.489801 mecha-0.9.2/mecha/resources/command_examples.mcfunction
+-rw-r--r--   0        0        0     1948 2021-11-16 02:58:02.493801 mecha-0.9.2/mecha/resources/multiline_command_examples.mcfunction
+-rw-r--r--   0        0        0     7501 2021-11-16 02:58:02.493801 mecha-0.9.2/mecha/serialize.py
+-rw-r--r--   0        0        0     3181 2021-11-16 02:58:02.493801 mecha-0.9.2/mecha/spec.py
+-rw-r--r--   0        0        0     5421 2021-11-16 02:58:02.493801 mecha-0.9.2/mecha/utils.py
+-rw-r--r--   0        0        0     1263 2021-11-16 02:58:44.394275 mecha-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4734 2021-11-16 02:58:46.508991 mecha-0.9.2/setup.py
+-rw-r--r--   0        0        0     4662 2021-11-16 02:58:46.509791 mecha-0.9.2/PKG-INFO
```

### Comparing `mecha-0.9.1/LICENSE` & `mecha-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/README.md` & `mecha-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/api.py` & `mecha-0.9.2/mecha/api.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/ast.py` & `mecha-0.9.2/mecha/ast.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/config.py` & `mecha-0.9.2/mecha/config.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/contrib/annotate_diagnostics.py` & `mecha-0.9.2/mecha/contrib/annotate_diagnostics.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 def beet_default(ctx: Context):
     mc = ctx.inject(Mecha)
 
     annotations: Dict[TextFileBase[Any], List[Tuple[int, int, List[str]]]] = {}
 
     for diagnostic in mc.diagnostics.exceptions:
-        message = f"{diagnostic.level:<7}{diagnostic.format_message()}\n{diagnostic.format_location()}"
+        message = f"{diagnostic.level.upper():<7}{diagnostic.format_message()}\n{diagnostic.format_location()}"
 
         if diagnostic.file and not diagnostic.location.unknown:
             if source := mc.database[diagnostic.file].source:
                 if code := diagnostic.format_code(source):
                     message += f"\n{code}"
 
             comments = [f"# {line}" for line in message.splitlines()]
+            comments[0] = "#>" + comments[0][2:]
             rendered = annotations.setdefault(diagnostic.file, [])
             line_index = diagnostic.location.lineno - 1
 
             heappush(rendered, (line_index, len(rendered), comments))
 
     for function, rendered in annotations.items():
         lines = function.text.splitlines()
```

### Comparing `mecha-0.9.1/mecha/contrib/lint_basic.py` & `mecha-0.9.2/mecha/contrib/lint_basic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/contrib/messages.py` & `mecha-0.9.2/mecha/contrib/messages.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/contrib/relative_location.py` & `mecha-0.9.2/mecha/contrib/relative_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/database.py` & `mecha-0.9.2/mecha/database.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/diagnostic.py` & `mecha-0.9.2/mecha/diagnostic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/dispatch.py` & `mecha-0.9.2/mecha/dispatch.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/parse.py` & `mecha-0.9.2/mecha/parse.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/prototype.py` & `mecha-0.9.2/mecha/prototype.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/1_16.json` & `mecha-0.9.2/mecha/resources/1_16.json`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/1_17.json` & `mecha-0.9.2/mecha/resources/1_17.json`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/1_18.json` & `mecha-0.9.2/mecha/resources/1_18.json`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/__init__.py` & `mecha-0.9.2/mecha/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/argument_examples.json` & `mecha-0.9.2/mecha/resources/argument_examples.json`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/command_examples.mcfunction` & `mecha-0.9.2/mecha/resources/command_examples.mcfunction`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/resources/multiline_command_examples.mcfunction` & `mecha-0.9.2/mecha/resources/multiline_command_examples.mcfunction`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/serialize.py` & `mecha-0.9.2/mecha/serialize.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/spec.py` & `mecha-0.9.2/mecha/spec.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/mecha/utils.py` & `mecha-0.9.2/mecha/utils.py`

 * *Files identical despite different names*

### Comparing `mecha-0.9.1/pyproject.toml` & `mecha-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecha"
-version = "0.9.1"
+version = "0.9.2"
 description = "A powerful Minecraft command library"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/mecha"
 repository = "https://github.com/mcbeet/mecha"
 documentation = "https://github.com/mcbeet/mecha"
@@ -29,15 +29,15 @@
 [tool.poetry.dev-dependencies]
 black = "^21.10b0"
 rope = "^0.20.1"
 pytest = "^6.2.5"
 isort = "^5.10.0"
 python-semantic-release = "^7.19.2"
 pytest-insta = "^0.1.10"
-lectern = "^0.17.1"
+lectern = "^0.18.0"
 
 [tool.black]
 target-version = ["py38"]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
```

### Comparing `mecha-0.9.1/setup.py` & `mecha-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['beet>=0.44.5', 'tokenstream>=1.2.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'mecha',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'A powerful Minecraft command library',
     'long_description': '<img align="right" src="https://raw.githubusercontent.com/mcbeet/mecha/main/logo.png" alt="logo" width="76">\n\n# Mecha\n\n[![GitHub Actions](https://github.com/mcbeet/mecha/workflows/CI/badge.svg)](https://github.com/mcbeet/mecha/actions)\n[![PyPI](https://img.shields.io/pypi/v/mecha.svg)](https://pypi.org/project/mecha/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mecha.svg)](https://pypi.org/project/mecha/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Discord](https://img.shields.io/discord/900530660677156924?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/98MdSGMm8j)\n\n> A powerful Minecraft command library.\n\n```python\nfrom mecha import Mecha\n\nmc = Mecha()\n\nfunction = """\n    execute\n        as @a                        # For each "player",\n        at @s                        # start at their feet.\n        anchored eyes                # Looking through their eyes,\n        facing 0 0 0                 # face perfectly at the target\n        anchored feet                # (go back to the feet)\n        positioned ^ ^ ^1            # and move one block forward.\n        rotated as @s                # Face the direction the player\n                                     # is actually facing,\n        positioned ^ ^ ^-1           # and move one block back.\n        if entity @s[distance=..0.6] # Check if we\'re close to the\n                                     # player\'s feet.\n        run\n            say I\'m facing the target!\n"""\n\nast = mc.parse(function, multiline=True)\nprint(mc.serialize(ast))  # execute as @a at @s anchored eyes facing ...\n```\n\n## Introduction\n\nThis package provides everything you need for working with Minecraft commands in Python, whether you\'re looking to process commands or build abstractions on top.\n\n### Features\n\n- Extensible and version-agnostic `mcfunction` parser\n- Clean, immutable and hashable abstract syntax tree with source location\n- Command config resolver that flattens and enumerates all the valid command prototypes\n- Powerful rule dispatcher for processing specific ast nodes\n- Composable ast visitors and reducers\n- Execute arbitrary compilation passes in your [`beet`](https://github.com/mcbeet/beet) pipeline\n- _(soon)_ Expressive command API for writing commands in Python\n\n## Credits\n\n- [A few test cases are adapted from `SPYGlass`](https://github.com/SPYGlassMC/SPYGlass)\n- [Multiline example by `AjaxGb` (MCC discord)](https://discord.com/channels/154777837382008833/157097006500806656/539318174466703361)\n- [Multiline syntax derived from the `hangman` plugin](https://github.com/mcbeet/beet/blob/main/beet/contrib/hangman.py)\n- [Partially inspired by `Trident`](https://energyxxer.com/trident/)\n\n## Installation\n\nThe package can be installed with `pip`.\n\n```bash\n$ pip install mecha\n```\n\n## Contributing\n\nContributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org/).\n\n```bash\n$ poetry install\n```\n\nYou can run the tests with `poetry run pytest`.\n\n```bash\n$ poetry run pytest\n```\n\nThe project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you\'re using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.\n\n```bash\n$ npm run watch\n$ npm run check\n```\n\nThe code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).\n\n```bash\n$ poetry run isort mecha tests\n$ poetry run black mecha tests\n$ poetry run black --check mecha tests\n```\n\n---\n\nLicense - [MIT](https://github.com/mcbeet/mecha/blob/main/LICENSE)\n',
     'author': 'Valentin Berlier',
     'author_email': 'berlier.v@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mcbeet/mecha',
```

### Comparing `mecha-0.9.1/PKG-INFO` & `mecha-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecha
-Version: 0.9.1
+Version: 0.9.2
 Summary: A powerful Minecraft command library
 Home-page: https://github.com/mcbeet/mecha
 License: MIT
 Keywords: beet,minecraft,datapack,minecraft-commands,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.8,<4.0
```

