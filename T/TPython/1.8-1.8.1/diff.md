# Comparing `tmp/TPython-1.8-py2.py3-none-any.whl.zip` & `tmp/TPython-1.8.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7532 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       66 b- defN 23-Feb-20 16:26 tpy/__init__.py
--rw-rw-rw-  2.0 fat       29 b- defN 23-Feb-10 13:59 tpy/__main__.py
--rw-rw-rw-  2.0 fat     3961 b- defN 23-Feb-19 13:13 tpy/config.py
--rw-rw-rw-  2.0 fat      476 b- defN 23-Feb-16 13:56 tpy/jsonc.py
--rw-rw-rw-  2.0 fat     9430 b- defN 23-Feb-20 16:26 tpy/tpy.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Feb-20 17:01 TPython-1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2480 b- defN 23-Feb-20 17:01 TPython-1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Feb-20 17:01 TPython-1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       37 b- defN 23-Feb-20 17:01 TPython-1.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Feb-20 17:01 TPython-1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      814 b- defN 23-Feb-20 17:01 TPython-1.8.dist-info/RECORD
-11 files, 18469 bytes uncompressed, 6170 bytes compressed:  66.6%
+Zip file size: 8490 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       68 b- defN 23-May-08 16:50 tpy/__init__.py
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Feb-20 17:02 tpy/__main__.py
+-rw-rw-rw-  2.0 fat     3961 b- defN 23-May-07 11:56 tpy/config.py
+-rw-rw-rw-  2.0 fat      903 b- defN 23-May-07 11:40 tpy/jsonc.py
+-rw-rw-rw-  2.0 fat    12048 b- defN 23-May-08 16:50 tpy/tpy.py
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2482 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       37 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      827 b- defN 23-May-08 16:51 TPython-1.8.1.dist-info/RECORD
+11 files, 21533 bytes uncompressed, 7104 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tpy/jsonc.py
 Comment: 
 
 Filename: tpy/tpy.py
 Comment: 
 
-Filename: TPython-1.8.dist-info/LICENSE
+Filename: TPython-1.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: TPython-1.8.dist-info/METADATA
+Filename: TPython-1.8.1.dist-info/METADATA
 Comment: 
 
-Filename: TPython-1.8.dist-info/WHEEL
+Filename: TPython-1.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: TPython-1.8.dist-info/entry_points.txt
+Filename: TPython-1.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: TPython-1.8.dist-info/top_level.txt
+Filename: TPython-1.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: TPython-1.8.dist-info/RECORD
+Filename: TPython-1.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpy/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .tpy import main
 
-__version__ = '1.8'
 __all__ = ['main']
+__version__ = '1.8.1'
```

## tpy/__main__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
 from . import tpy
-tpy.main()
+tpy.main()
```

## tpy/config.py

```diff
@@ -10,15 +10,15 @@
     from colorama import Fore, init
     init(autoreset=True)
 except ModuleNotFoundError:
     sys.exit('Module not found: colorama')
 
 # Defualt Vars
 #  It's just the defualt configuration dict, Consider reading https://github.com/Techlord210/TPython/blob/main/config.jsonc instead.
-CONFIG = {'version': '1.1', 'config': {'notify_updates': True, 'welcome_msg': True, 'exit_msg': True, 'crash_msg': True}, 'colors': {'update': {'text_color': Fore.LIGHTCYAN_EX, 'version_color': Fore.LIGHTGREEN_EX}, 'welcome': {'text_color': Fore.LIGHTCYAN_EX, 'padding_color': Fore.LIGHTCYAN_EX}, 'exit': {'success': {'text_color': Fore.LIGHTCYAN_EX, 'padding_color': Fore.LIGHTCYAN_EX}, 'crash': {'text_color': Fore.LIGHTYELLOW_EX, 'padding_color': Fore.LIGHTYELLOW_EX}}, 'promot': {'default': {'sq_brackets': Fore.LIGHTGREEN_EX, 'number': {'normal': Fore.LIGHTWHITE_EX, 'error': Fore.LIGHTRED_EX}, 'dash': Fore.LIGHTGREEN_EX,'arrow': Fore.LIGHTCYAN_EX, 'indent': {'number_replace': Fore.LIGHTYELLOW_EX, 'sq_brackets': Fore.LIGHTGREEN_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTYELLOW_EX}}, 'timeit': {'sq_brackets': Fore.LIGHTGREEN_EX, 'text_color': Fore.LIGHTWHITE_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTWHITE_EX, 'time_text': {'text_color': Fore.LIGHTGREEN_EX, 'time_color': Fore.LIGHTYELLOW_EX}, 'indent': {'number_replace': Fore.LIGHTWHITE_EX, 'sq_brackets': Fore.LIGHTGREEN_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTWHITE_EX}}}}}
+config = {'version': '1.1', 'config': {'notify_updates': True, 'welcome_msg': True, 'exit_msg': True, 'crash_msg': True}, 'colors': {'update': {'text_color': Fore.LIGHTCYAN_EX, 'version_color': Fore.LIGHTGREEN_EX}, 'welcome': {'text_color': Fore.LIGHTCYAN_EX, 'padding_color': Fore.LIGHTCYAN_EX}, 'exit': {'success': {'text_color': Fore.LIGHTCYAN_EX, 'padding_color': Fore.LIGHTCYAN_EX}, 'crash': {'text_color': Fore.LIGHTYELLOW_EX, 'padding_color': Fore.LIGHTYELLOW_EX}}, 'promot': {'default': {'sq_brackets': Fore.LIGHTGREEN_EX, 'number': {'normal': Fore.LIGHTWHITE_EX, 'error': Fore.LIGHTRED_EX}, 'dash': Fore.LIGHTGREEN_EX,'arrow': Fore.LIGHTCYAN_EX, 'indent': {'number_replace': Fore.LIGHTYELLOW_EX, 'sq_brackets': Fore.LIGHTGREEN_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTYELLOW_EX}}, 'timeit': {'sq_brackets': Fore.LIGHTGREEN_EX, 'text_color': Fore.LIGHTWHITE_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTWHITE_EX, 'time_text': {'text_color': Fore.LIGHTGREEN_EX, 'time_color': Fore.LIGHTYELLOW_EX}, 'indent': {'number_replace': Fore.LIGHTWHITE_EX, 'sq_brackets': Fore.LIGHTGREEN_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTWHITE_EX}}}}}
 CONFIG_PATH: str = os.path.abspath(os.path.expanduser('~/.TPython/config.jsonc'))
 READER_VERSION: str = '1.1'
 READ_FILE: bool = False
 
 # Decoder Error
 class JSONCDecodeError(Exception):
     def __init__(self, msg: str) -> None:
@@ -48,20 +48,20 @@
 
     except Exception:
         tpy.tpy.exc()
         return {}
 
 if os.path.isfile(CONFIG_PATH):
     try:
-        CONFIG = parse_file(CONFIG_PATH)
+        config = parse_file(CONFIG_PATH)
         READ_FILE = True
     except:
         tpy.tpy.exc()
 
-if CONFIG['version'] == READER_VERSION:
+if config['version'] == READER_VERSION:
     if READ_FILE:
         COLORS = {
             "cyan": Fore.LIGHTCYAN_EX,
             "green": Fore.LIGHTGREEN_EX,
             "red": Fore.LIGHTRED_EX,
             "yellow": Fore.LIGHTYELLOW_EX,
             "white": Fore.LIGHTWHITE_EX,
@@ -73,15 +73,15 @@
         def color_to_code(config: dict) -> dict:
             for key, val in config.items():
                 if type(val) == dict:
                     color_to_code(config[key])
                 else:
                     config[key] = COLORS.get(val, Fore.WHITE)
             return config
-        color_to_code(CONFIG['colors'])
+        color_to_code(config['colors'])
 else:
-    sys.exit(f"{Fore.LIGHTRED_EX}config file version '{Fore.LIGHTYELLOW_EX}{CONFIG['version']}{Fore.LIGHTRED_EX}' don't match with reader '{Fore.LIGHTYELLOW_EX}{READER_VERSION}{Fore.LIGHTRED_EX}'")
+    sys.exit(f"{Fore.LIGHTRED_EX}config file version '{Fore.LIGHTYELLOW_EX}{config['version']}{Fore.LIGHTRED_EX}' don't match with reader '{Fore.LIGHTYELLOW_EX}{READER_VERSION}{Fore.LIGHTRED_EX}'")
 
-INP_COLORS = CONFIG['colors']['promot']['default']
-INP_COLORS_INDENT = CONFIG['colors']['promot']['default']['indent']
-TNP_COLORS = CONFIG['colors']['promot']['timeit']
-TNP_COLORS_INDENT = CONFIG['colors']['promot']['timeit']['indent']
+INP_COLORS = config['colors']['promot']['default']
+INP_COLORS_INDENT = config['colors']['promot']['default']['indent']
+TNP_COLORS = config['colors']['promot']['timeit']
+TNP_COLORS_INDENT = config['colors']['promot']['timeit']['indent']
```

## tpy/jsonc.py

```diff
@@ -1,16 +1,29 @@
 # Import Libs
 import json
 import re
+from typing import List
 
-# Parser
-def parse(filepath: str) -> dict:
-    # Define the regular expression to match both comment styles
-    comment_pattern = r'(\/\/[^\n]*)|(/\*[\s\S]*?\*/)'
+# Decoder Error
+class JSONCDecodeError(Exception):
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
 
+# Parser
+def parse_file(file: str) -> dict:
     # Read the contents of the file into a string
-    with open(filepath, 'r', encoding='utf-8') as f:
-        contents = f.read()
+    with open(file, 'r') as f:
+        content:str = f.read()
 
     # Remove the comments from the string
-    json_dict = json.loads(re.sub(comment_pattern, '', contents))
-    return json_dict
+    json_str: str = re.sub(r'(\/\/[^\n]*)|(/\*[\s\S]*?\*/)', '', content)
+
+    # Check for broken comments
+    tmp_list: List[str] = re.sub(r'"([^"]*)"', '', json_str).splitlines()
+
+    for line_no, element in enumerate(tmp_list, 1):
+        if '*/' in element:
+            raise JSONCDecodeError(f"expected '/*' before '*/', line {line_no}")
+        elif '/*' in element:
+            raise JSONCDecodeError(f"expected '*/' after '/*', line {line_no}")
+    
+    return json.loads(json_str)
```

## tpy/tpy.py

```diff
@@ -1,94 +1,139 @@
 # Import libs
 import ast
+import builtins as __builtins__
 import json
 import os
 import sys
 import traceback
 import urllib.error
 import urllib.request
 from threading import Thread
 from timeit import timeit
 
-import tpy.config
+from . import jsonc
 
 try:
     from colorama import Fore, init
     init(autoreset=True)
 except ModuleNotFoundError:
     sys.exit('Module not found: colorama')
 
 # Vars
 cell_number: int = 1
 err: bool = False
 ind: bool = False
-namespace: dict = {}
+namespace: dict = {'__builtins__': __builtins__, '__name__': '__main__', '__doc__': 'Automatically created module for TPython interactive environment', '__package__': None, '__loader__': None, '__spec__': None, '__annotations__': {}}
 VERSION: str = '1.8'
 
 # Exception prettifier
 def exc() -> None:
     name, value = sys.exc_info()[0:2] # type: ignore
     name: str = name.__name__ # type: ignore
     top_bar = "----------------------------------------------------------------------" if os.get_terminal_size().columns > 70 else "-"*os.get_terminal_size().columns
     if name == 'SyntaxError':
         line: str = value.args[1][3] # type: ignore
         err_highlight: str = ' '*(value.offset - 1) + ('^'*(value.end_offset - value.offset) if value.end_offset - value.offset != 0 else '^') # type: ignore
-        value: str = value.args[0] # type: ignore
+        value: = value.args[0] # type: ignore
         if line.endswith('\n'):
             line = line.removesuffix('\n')
         exc: str = f'{Fore.LIGHTGREEN_EX}{top_bar}\n{Fore.LIGHTRED_EX}{name} {Fore.LIGHTGREEN_EX}in Cell {Fore.GREEN}{cell_number}\n{Fore.RESET}{line}\n{err_highlight}\n\n{Fore.LIGHTRED_EX}{name}{Fore.RESET}: {value}'
     else:
         exc: str = f'{Fore.LIGHTGREEN_EX}{top_bar}\n{Fore.LIGHTRED_EX}{name} {Fore.LIGHTGREEN_EX}in Cell {Fore.GREEN}{cell_number}{(len(top_bar)-len(name)-len(str(cell_number))-42)*" "}Traceback (most recent call last)\n\n{Fore.LIGHTRED_EX}{name}{Fore.RESET}: {value}'
     print(exc)
 
+# Load Config
+# Defualt Vars
+CONFIG_PATH: str = os.path.abspath(os.path.expanduser('~/.TPython/config.jsonc'))
+READER_VERSION: str = '1.1'
+_read: bool = False
+## Consider reading https://github.com/Techlord210/TPython/blob/main/jsonc instead.
+config = {'version': '1.1', 'config': {'notify_updates': True, 'welcome_msg': True, 'exit_msg': True, 'crash_msg': True}, 'colors': {'update': {'text_color': Fore.LIGHTCYAN_EX, 'version_color': Fore.LIGHTGREEN_EX}, 'welcome': {'text_color': Fore.LIGHTCYAN_EX, 'padding_color': Fore.LIGHTCYAN_EX}, 'exit': {'success': {'text_color': Fore.LIGHTCYAN_EX, 'padding_color': Fore.LIGHTCYAN_EX}, 'crash': {'text_color': Fore.LIGHTYELLOW_EX, 'padding_color': Fore.LIGHTYELLOW_EX}}, 'promot': {'default': {'sq_brackets': Fore.LIGHTGREEN_EX, 'number': {'normal': Fore.LIGHTWHITE_EX, 'error': Fore.LIGHTRED_EX}, 'dash': Fore.LIGHTGREEN_EX,'arrow': Fore.LIGHTCYAN_EX, 'indent': {'number_replace': Fore.LIGHTYELLOW_EX, 'sq_brackets': Fore.LIGHTGREEN_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTYELLOW_EX}}, 'timeit': {'sq_brackets': Fore.LIGHTGREEN_EX, 'text_color': Fore.LIGHTWHITE_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTWHITE_EX, 'time_text': {'text_color': Fore.LIGHTGREEN_EX, 'time_color': Fore.LIGHTYELLOW_EX}, 'indent': {'number_replace': Fore.LIGHTWHITE_EX, 'sq_brackets': Fore.LIGHTGREEN_EX, 'dash': Fore.LIGHTGREEN_EX, 'arrow': Fore.LIGHTWHITE_EX}}}}}
+
+if os.path.isfile(CONFIG_PATH):
+    try:
+        config = jsonc.parse_file(CONFIG_PATH)
+        _read = True
+    except Exception:
+        exc()
+
+if config['version'] == READER_VERSION:
+    if _read:
+        COLORS = {
+            "cyan": Fore.LIGHTCYAN_EX,
+            "green": Fore.LIGHTGREEN_EX,
+            "red": Fore.LIGHTRED_EX,
+            "yellow": Fore.LIGHTYELLOW_EX,
+            "white": Fore.LIGHTWHITE_EX,
+            "blue": Fore.LIGHTBLUE_EX,
+            "black": Fore.LIGHTBLACK_EX,
+            "magenta": Fore.LIGHTMAGENTA_EX
+        }
+
+        def color_to_code(config: dict) -> dict:
+            for key, val in config.items():
+                if type(val) == dict:
+                    color_to_code(config[key])
+                else:
+                    config[key] = COLORS.get(val, Fore.WHITE)
+            return config
+        color_to_code(config['colors'])
+else:
+    sys.exit(f"{Fore.LIGHTRED_EX}config file version '{Fore.LIGHTYELLOW_EX}{config['version']}{Fore.LIGHTRED_EX}' don't match with reader '{Fore.LIGHTYELLOW_EX}{READER_VERSION}{Fore.LIGHTRED_EX}'")
+
+INP_COLORS = config['colors']['promot']['default']
+INP_COLORS_INDENT = config['colors']['promot']['default']['indent']
+TNP_COLORS = config['colors']['promot']['timeit']
+TNP_COLORS_INDENT = config['colors']['promot']['timeit']['indent']
+
 # Update notifier
-if tpy.config.CONFIG['config']['notify_updates']:
+if config['config']['notify_updates']:
     def update_checker() -> None:
         try:
             response = urllib.request.urlopen('https://pypi.org/pypi/TPython/json')
             pypi_json = json.load(response)
             pypi_version = pypi_json['info']['version']
             if pypi_version != VERSION:
-                print(f'{tpy.config.CONFIG["colors"]["update"]["text_color"]}Newer version of TPython is available: {tpy.config.CONFIG["colors"]["update"]["version_color"]}{pypi_version}')
+                print(f'{config["colors"]["update"]["text_color"]}Newer version of TPython is available: {config["colors"]["update"]["version_color"]}{pypi_version}')
         except urllib.error.URLError:
             pass
         return
     Thread(target=update_checker).run()
 
 # Entry point
 def main() -> None:
     global cell_number, err, ind
 
     # Exit function
     def ext(crash_m: str = '', crash: bool = False) -> None:
         columns = os.get_terminal_size().columns
         success_m = 'Process Completed Successfully'
         if crash:
-            if tpy.config.CONFIG['config']['crash_msg']:
+            if config['config']['crash_msg']:
                 msg = crash_m
                 for i in range((columns-len(crash_m))//2):
-                    msg = f'{tpy.config.CONFIG["colors"]["exit"]["crash"]["padding_color"]}-{tpy.config.CONFIG["colors"]["exit"]["crash"]["text_color"]}{msg}{tpy.config.CONFIG["colors"]["exit"]["crash"]["padding_color"]}-'
+                    msg = f'{config["colors"]["exit"]["crash"]["padding_color"]}-{config["colors"]["exit"]["crash"]["text_color"]}{msg}{config["colors"]["exit"]["crash"]["padding_color"]}-'
                 sys.exit(f'{msg}')
         else:
-            if tpy.config.CONFIG['config']['exit_msg']:
+            if config['config']['exit_msg']:
                 msg = success_m
                 for i in range((columns-len(success_m))//2):
-                    msg = f'{tpy.config.CONFIG["colors"]["exit"]["success"]["padding_color"]}-{tpy.config.CONFIG["colors"]["exit"]["success"]["text_color"]}{msg}{tpy.config.CONFIG["colors"]["exit"]["success"]["padding_color"]}-'
+                    msg = f'{config["colors"]["exit"]["success"]["padding_color"]}-{config["colors"]["exit"]["success"]["text_color"]}{msg}{config["colors"]["exit"]["success"]["padding_color"]}-'
                 print(f'{msg}')
             sys.exit()
 
     try:
         # Execute function
         def execute(code: str, timeit_b: bool = False) -> None:
             global err, cell_number
             run = False
             if timeit_b:
                 try:
                     time = timeit(code, globals=namespace, number=1)
-                    print(f'{tpy.config.TNP_COLORS["time_text"]["text_color"]}Execution time: {tpy.config.TNP_COLORS["time_text"]["time_color"]}{time}')
+                    print(f'{TNP_COLORS["time_text"]["text_color"]}Execution time: {TNP_COLORS["time_text"]["time_color"]}{time}')
                 except Exception:
                     exc()
                     err = True
             else:
                 try:
                     eval_return = eval(code, namespace)
                     if eval_return != None:
@@ -102,52 +147,52 @@
                         err = False
                     except Exception:
                         exc()
                         err = True
             cell_number += 1
 
         # Welcome message
-        if tpy.config.CONFIG['config']['welcome_msg']:
+        if config['config']['welcome_msg']:
             columns = os.get_terminal_size().columns
             msg = 'TPython'
             columns -= 7
             for i in range(columns//2):
-                msg = f'{tpy.config.CONFIG["colors"]["welcome"]["padding_color"]}-{tpy.config.CONFIG["colors"]["welcome"]["text_color"]}{msg}{tpy.config.CONFIG["colors"]["welcome"]["padding_color"]}-'
+                msg = f'{config["colors"]["welcome"]["padding_color"]}-{config["colors"]["welcome"]["text_color"]}{msg}{config["colors"]["welcome"]["padding_color"]}-'
             print(f'{msg}')
 
         # Input
         while True:
             try:
                 indent = False
                 indent_t = False
-                inp = input(f'{tpy.config.INP_COLORS["sq_brackets"]}[{tpy.config.INP_COLORS["number"]["error" if err else "normal"]}{cell_number}{tpy.config.INP_COLORS["sq_brackets"]}]{tpy.config.INP_COLORS["dash"]}-{tpy.config.INP_COLORS["arrow"]}> {Fore.LIGHTWHITE_EX}')
+                inp = input(f'{INP_COLORS["sq_brackets"]}[{INP_COLORS["number"]["error" if err else "normal"]}{cell_number}{INP_COLORS["sq_brackets"]}]{INP_COLORS["dash"]}-{INP_COLORS["arrow"]}> {Fore.LIGHTWHITE_EX}')
                 if not (inp.isspace() or inp == ''):
                     inp = inp.strip()
                     # Exit command
                     if inp in ('exit', 'quit', 'close'):
                         ext()
                     elif inp in ('clear', 'cls') and not ('clear' in namespace or 'cls' in namespace):
                         os.system('cls' if os.name == 'nt' else 'clear')
                         err = False
                     # Version command
                     elif inp == 'version' and not 'version' in namespace:
                         print(f'{Fore.LIGHTCYAN_EX}{VERSION} {Fore.LIGHTGREEN_EX}from {Fore.LIGHTCYAN_EX}Python {Fore.LIGHTCYAN_EX}{sys.version_info.major}.{sys.version_info.minor}')
                     # TimeIt command
                     elif inp == 'timeit' and not 'timeit' in namespace:
                         while True:
-                            tnp = input(f'{tpy.config.TNP_COLORS["sq_brackets"]}[{tpy.config.TNP_COLORS["text_color"]}TimeIt{tpy.config.TNP_COLORS["sq_brackets"]}]{tpy.config.TNP_COLORS["dash"]}-{tpy.config.TNP_COLORS["arrow"]}> {Fore.LIGHTWHITE_EX}').strip()
+                            tnp = input(f'{TNP_COLORS["sq_brackets"]}[{TNP_COLORS["text_color"]}TimeIt{TNP_COLORS["sq_brackets"]}]{TNP_COLORS["dash"]}-{TNP_COLORS["arrow"]}> {Fore.LIGHTWHITE_EX}').strip()
                             # Check for SyntaxError, if there is it will give indent promote
                             try:
                                 ast.parse(inp)
                             except SyntaxError:
                                 indent_t = True
                             if indent_t:
                                 # Indenting
                                 while True:
-                                    indent = input(f'{tpy.config.TNP_COLORS_INDENT["sq_brackets"]}[{tpy.config.TNP_COLORS_INDENT["text_replace"]}------{tpy.config.TNP_COLORS_INDENT["sq_brackets"]}]{tpy.config.TNP_COLORS_INDENT["dash"]}-{tpy.config.TNP_COLORS_INDENT["arrow"]}> {Fore.LIGHTWHITE_EX}')
+                                    indent = input(f'{TNP_COLORS_INDENT["sq_brackets"]}[{TNP_COLORS_INDENT["text_replace"]}------{TNP_COLORS_INDENT["sq_brackets"]}]{TNP_COLORS_INDENT["dash"]}-{TNP_COLORS_INDENT["arrow"]}> {Fore.LIGHTWHITE_EX}')
                                     if indent.strip() == '':
                                         if not ind:
                                             ind = True
                                         else:
                                             break
                                     else:
                                         tnp += f'\n{indent}'
@@ -162,15 +207,15 @@
                         try:
                             ast.parse(inp)
                         except SyntaxError:
                             indent = True
                         if indent:
                             # Indenting
                             while True:
-                                indent = input(f'{tpy.config.INP_COLORS_INDENT["sq_brackets"]}[{tpy.config.INP_COLORS_INDENT["number_replace"]}{":"*len(str(cell_number))}{tpy.config.INP_COLORS_INDENT["sq_brackets"]}]{tpy.config.INP_COLORS_INDENT["dash"]}-{tpy.config.INP_COLORS_INDENT["arrow"]}> {Fore.LIGHTWHITE_EX}')
+                                indent = input(f'{INP_COLORS_INDENT["sq_brackets"]}[{INP_COLORS_INDENT["number_replace"]}{":"*len(str(cell_number))}{INP_COLORS_INDENT["sq_brackets"]}]{INP_COLORS_INDENT["dash"]}-{INP_COLORS_INDENT["arrow"]}> {Fore.LIGHTWHITE_EX}')
                                 if indent.strip() == '':
                                     if not ind:
                                         ind = True
                                     else:
                                         break
                                 else:
                                     inp += f'\n{indent}'
@@ -181,8 +226,8 @@
             except KeyboardInterrupt:
                 print(f'\n{Fore.LIGHTYELLOW_EX}KeyboardInterrupt')
                 err = True
     except EOFError:
         sys.exit(f'{Fore.LIGHTYELLOW_EX}EOFError')
     except Exception as e:
         print(traceback.format_exc())
-        ext(e.__name__, True) # type: ignore
+        ext(e.__name__, True) # type: ignore
```

## Comparing `TPython-1.8.dist-info/LICENSE` & `TPython-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `TPython-1.8.dist-info/METADATA` & `TPython-1.8.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TPython
-Version: 1.8
+Version: 1.8.1
 Summary: A better python REPL
 Home-page: https://github.com/Techlord210/TPython
 Author: Techlord210
 Author-email: techlord210@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `TPython-1.8.dist-info/RECORD` & `TPython-1.8.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-tpy/__init__.py,sha256=Qh0utrGVAeYxurq-CPaPCHXAAy41SClkXyoaHM94eyg,66
-tpy/__main__.py,sha256=25fwvr4p_iqO65WKaDu9AKdDdCZmwO4BlURigB_6Boo,29
-tpy/config.py,sha256=MMrNMhZXouZM-WvFFscdpe0dxlvkTkaxA3LEoIxKQ1E,3961
-tpy/jsonc.py,sha256=GbEqRZWGshgyxU4y6uHKPhWUXCHcZlbEhhy8w2niPl0,476
-tpy/tpy.py,sha256=BKneo19rEuwFoo1GnUSyPfTeEF-MVLJt1rzTujmRMrU,9430
-TPython-1.8.dist-info/LICENSE,sha256=GS5TToSs_EOk0Tj2Fo-HHCkZ6eygTyWO3XS14FejHhA,1062
-TPython-1.8.dist-info/METADATA,sha256=zq_uaeYP7nKUpHtYgQWKdSAVixB43L1zYZG6ALE3rRw,2480
-TPython-1.8.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-TPython-1.8.dist-info/entry_points.txt,sha256=q8DvqvZcK998v2-nIBxk1_8YN9-8q7ExjaLMAD3wSMg,37
-TPython-1.8.dist-info/top_level.txt,sha256=m1dzcLsLqF1dBEAhsMlZKNTPyKhkLCeR0pVUn0kiSVw,4
-TPython-1.8.dist-info/RECORD,,
+tpy/__init__.py,sha256=mb-GatMZXxfPlMSBVT4X8FsRDAZWLI9XWPS7uMUFDtY,68
+tpy/__main__.py,sha256=ltgbchgFToyekZWa2vYf0Pu5T-wy5zQ8_b7flye0uvU,31
+tpy/config.py,sha256=wVEvEKF8Go-KIsiaDvOD01XKOBTX2E_KtS_rlv3ylL0,3961
+tpy/jsonc.py,sha256=DPdbBaLfje_05VtWpYU9C_7CnmNBmv2-I8S23LOEsI4,903
+tpy/tpy.py,sha256=JLIwA_4pUM1o1lVhHXcSRhbSbUIUtQ88f2udxqv6oUA,12048
+TPython-1.8.1.dist-info/LICENSE,sha256=GS5TToSs_EOk0Tj2Fo-HHCkZ6eygTyWO3XS14FejHhA,1062
+TPython-1.8.1.dist-info/METADATA,sha256=03I46Hf_KA_W_PKcjGw5AUSx64SbmqVxf84ev6xZjCA,2482
+TPython-1.8.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+TPython-1.8.1.dist-info/entry_points.txt,sha256=q8DvqvZcK998v2-nIBxk1_8YN9-8q7ExjaLMAD3wSMg,37
+TPython-1.8.1.dist-info/top_level.txt,sha256=m1dzcLsLqF1dBEAhsMlZKNTPyKhkLCeR0pVUn0kiSVw,4
+TPython-1.8.1.dist-info/RECORD,,
```

