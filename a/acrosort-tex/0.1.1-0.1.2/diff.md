# Comparing `tmp/acrosort_tex-0.1.1.tar.gz` & `tmp/acrosort_tex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrosort_tex-0.1.1.tar", max compression
+gzip compressed data, was "acrosort_tex-0.1.2.tar", max compression
```

## Comparing `acrosort_tex-0.1.1.tar` & `acrosort_tex-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2023-05-07 19:44:22.877485 acrosort_tex-0.1.1/acrosort_tex/__init__.py
--rw-r--r--   0        0        0     5894 2023-05-07 19:43:08.130277 acrosort_tex-0.1.1/acrosort_tex/sorter.py
--rw-r--r--   0        0        0     1075 2023-05-07 19:13:48.202423 acrosort_tex-0.1.1/LICENSE
--rw-r--r--   0        0        0      885 2023-05-07 19:44:35.974039 acrosort_tex-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1021 2023-05-07 19:31:22.038473 acrosort_tex-0.1.1/README.md
--rw-r--r--   0        0        0     1773 2023-05-07 19:44:58.913328 acrosort_tex-0.1.1/setup.py
--rw-r--r--   0        0        0     1862 2023-05-07 19:44:58.913328 acrosort_tex-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-08 14:42:11.062374 acrosort_tex-0.1.2/acrosort_tex/__init__.py
+-rw-r--r--   0        0        0     4821 2023-05-08 14:41:57.183944 acrosort_tex-0.1.2/acrosort_tex/sorter.py
+-rw-r--r--   0        0        0     1075 2023-05-07 19:13:48.202423 acrosort_tex-0.1.2/LICENSE
+-rw-r--r--   0        0        0      885 2023-05-08 14:42:06.938767 acrosort_tex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1028 2023-05-08 14:43:02.793482 acrosort_tex-0.1.2/README.md
+-rw-r--r--   0        0        0     1780 2023-05-08 14:43:12.802080 acrosort_tex-0.1.2/setup.py
+-rw-r--r--   0        0        0     1869 2023-05-08 14:43:12.803105 acrosort_tex-0.1.2/PKG-INFO
```

### Comparing `acrosort_tex-0.1.1/acrosort_tex/sorter.py` & `acrosort_tex-0.1.2/acrosort_tex/sorter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import re
 
 from rich.console import Console
 
 
+# TODO: NamedTuple, If key_2 not available use key_1
 def _load_file(filename: str) -> list:
     """
     Load .tex file with abbreviations and return a list of lines.
 
     Args:
         filename (str): .tex file path
 
@@ -24,77 +25,42 @@
     Find the start and end of the acronym block in the .tex file and find the longest shortform key.
     Longest shortform key is needed to set the width of the shortform column in the acronym block.
 
     Args:
         tex_lines (list): List of all lines in the .tex file
 
     Returns:
-        tuple: (Index of Start Block of Acronyms, Index of End Block of Acronyms, Longest Shortform Key)
+        tuple: (Index of Start Block of Acronyms, Index of End Block of Acronyms, Longest Shortform Key, Acronyms)
     """
     acronym_block_start = None
     acronym_block_end = None
     longest_shortform_key = None
     longest_shortform_len = 0
+    acronyms = {}
 
     for i, line in enumerate(tex_lines):
         if "\\begin{acronym}" in line:
             acronym_block_start = i
             longest_shortform_key = re.findall(r"\[([^\]]+)\]", line)[0]
         elif "\\end{acronym}" in line:
             acronym_block_end = i
             break
         else:
             match = re.search(r"\\acro\{(.+?)\}\[(.+?)\]\{(.+?)\}", line)
             if match:
-                shortform_len = len(match.group(2))
+                key = match.group(1)
+                key_in_file = match.group(2)
+                long_form = match.group(3)
+                acronyms[key] = (key_in_file, long_form)
+                shortform_len = len(key_in_file)
                 if shortform_len > longest_shortform_len:
-                    longest_shortform_key = match.group(1)
+                    longest_shortform_key = key
                     longest_shortform_len = shortform_len
 
-    return acronym_block_start, acronym_block_end, longest_shortform_key
-
-
-def _extract_acronym_lines(
-    acronym_block_start: int, acronym_block_end: int, tex_lines: list
-) -> list:
-    """
-    Extract only the acronym block.
-
-    Args:
-        acronym_block_start (int): Index of Start Block of Acronyms
-        acronym_block_end (int): Index of End Block of Acronyms
-        tex_lines (list):
-
-    Returns:
-        list: List of all lines in the .tex file
-    """
-    acronym_lines = tex_lines[acronym_block_start : acronym_block_end + 1]
-    acronym_lines = [line.strip() for line in acronym_lines]
-    return acronym_lines
-
-
-def _extract_acronyms(acronym_lines: list) -> dict:
-    """
-    Extract all acronyms from block
-
-    Args:
-        acronym_lines (list): List of all acronym lines.
-
-    Returns:
-        dict: Key-Value Pair of acronyms. Key is the shortform, Value is a tuple of (key_in_file, long_form)
-    """
-    acronyms = {}
-    for line in acronym_lines:
-        match = re.search(r"\\acro\{(.+?)\}\[(.+?)\]\{(.+?)\}", line)
-        if match:
-            key = match.group(1)
-            key_in_file = match.group(2)
-            long_form = match.group(3)
-            acronyms[key] = (key_in_file, long_form)
-    return acronyms
+    return acronym_block_start, acronym_block_end, longest_shortform_key, acronyms
 
 
 def _sort_acronyms(acronyms: dict) -> list:
     """
     Sort acronyms by their shortform in ascending order.
 
     Args:
@@ -124,15 +90,15 @@
         longest_shortform_key (str): Longest shortform key to set the width of the shortform column in the acronym block
 
     Returns:
         list: All lines with the new acronym block
     """
     new_acronym_lines = [f"\\begin{{acronym}}[{longest_shortform_key}]\n"]
     for key, (key_in_file, long_form) in sorted_acronyms:
-        new_line = f"\\acro{{{key}}}[{key_in_file}]{{{long_form}}}\n"
+        new_line = f"\t\\acro{{{key}}}[{key_in_file}]{{{long_form}}}\n"
         new_acronym_lines.append(new_line)
     new_acronym_lines.append("\\end{acronym}\n")
 
     tex_lines = (
         tex_lines[:acronym_block_start]
         + new_acronym_lines
         + tex_lines[acronym_block_end + 1 :]
@@ -160,23 +126,20 @@
     )
     parser.add_argument("output_file", type=str, help="filename of your output file")
 
     args = parser.parse_args()
 
     tex_lines = _load_file(args.input_file)
 
-    acronym_block_start, acronym_block_end, longest_shortform_key = _find_acronym_block(
-        tex_lines
-    )
-
-    acronym_lines = _extract_acronym_lines(
-        acronym_block_start, acronym_block_end, tex_lines
-    )
-
-    acronyms = _extract_acronyms(acronym_lines)
+    (
+        acronym_block_start,
+        acronym_block_end,
+        longest_shortform_key,
+        acronyms,
+    ) = _find_acronym_block(tex_lines)
 
     acronyms = _sort_acronyms(acronyms)
 
     tex_lines = _replace_old_acronym_block_with_new_one(
         acronym_block_start,
         acronym_block_end,
         tex_lines,
```

### Comparing `acrosort_tex-0.1.1/LICENSE` & `acrosort_tex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acrosort_tex-0.1.1/pyproject.toml` & `acrosort_tex-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acrosort_tex"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["baniasbaabe <banias@hotmail.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/baniasbaabe/acrosort-tex/tree/main"
 repository = "https://github.com/baniasbaabe/acrosort-tex/tree/main"
 keywords = ["latex", "acronyms", "sorting"]
```

### Comparing `acrosort_tex-0.1.1/README.md` & `acrosort_tex-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```bash
 acrosort <input_file.tex> <output_file.tex>
 ```
 
 For example:
 
 ```bash
-acrosort examples/List_Of_Abbreviations.tex acronyms.tex
+acrosort examples/List_Of_Abbreviations.tex sorted_acronyms.tex
 ```
 
 This will create a new `.tex` file called `sorted_acronyms.tex` with the sorted acronyms, while everything else isn't touched.
 
 It will also find the longest key to set the width of the shortform column in the acronym block.
 
 ## License
```

### Comparing `acrosort_tex-0.1.1/setup.py` & `acrosort_tex-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['rich>=13.3.5,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['acrosort = acrosort_tex.sorter:main']}
 
 setup_kwargs = {
     'name': 'acrosort-tex',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
-    'long_description': "# acrosort-tex\n\n`acrosort-tex` is a Python Command Line App to sort your acronyms in your `.tex` by their shortform.\n\n## Installation\n\nYou can install acrosort-tex using pip (note the underscore):\n\n```bash\npip install acrosort_tex\n```\n\n## Usage\n\nTo use `acrosort-tex`, you first need to create a `.tex` file with a list of acronyms (see in `examples` for an example file).\n\nIt doesn't matter if there are other TeX commands before or after the `acronym` block.\n\nTo sort the acronyms, run the following command:\n\n```bash\nacrosort <input_file.tex> <output_file.tex>\n```\n\nFor example:\n\n```bash\nacrosort examples/List_Of_Abbreviations.tex acronyms.tex\n```\n\nThis will create a new `.tex` file called `sorted_acronyms.tex` with the sorted acronyms, while everything else isn't touched.\n\nIt will also find the longest key to set the width of the shortform column in the acronym block.\n\n## License\n\n`acrosort_tex` is licensed under the MIT License. See the LICENSE file for more information.\n",
+    'long_description': "# acrosort-tex\n\n`acrosort-tex` is a Python Command Line App to sort your acronyms in your `.tex` by their shortform.\n\n## Installation\n\nYou can install acrosort-tex using pip (note the underscore):\n\n```bash\npip install acrosort_tex\n```\n\n## Usage\n\nTo use `acrosort-tex`, you first need to create a `.tex` file with a list of acronyms (see in `examples` for an example file).\n\nIt doesn't matter if there are other TeX commands before or after the `acronym` block.\n\nTo sort the acronyms, run the following command:\n\n```bash\nacrosort <input_file.tex> <output_file.tex>\n```\n\nFor example:\n\n```bash\nacrosort examples/List_Of_Abbreviations.tex sorted_acronyms.tex\n```\n\nThis will create a new `.tex` file called `sorted_acronyms.tex` with the sorted acronyms, while everything else isn't touched.\n\nIt will also find the longest key to set the width of the shortform column in the acronym block.\n\n## License\n\n`acrosort_tex` is licensed under the MIT License. See the LICENSE file for more information.\n",
     'author': 'baniasbaabe',
     'author_email': 'banias@hotmail.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/baniasbaabe/acrosort-tex/tree/main',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `acrosort_tex-0.1.1/PKG-INFO` & `acrosort_tex-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrosort-tex
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/baniasbaabe/acrosort-tex/tree/main
 License: MIT
 Keywords: latex,acronyms,sorting
 Author: baniasbaabe
 Author-email: banias@hotmail.de
 Requires-Python: >=3.8,<4.0
@@ -44,15 +44,15 @@
 ```bash
 acrosort <input_file.tex> <output_file.tex>
 ```
 
 For example:
 
 ```bash
-acrosort examples/List_Of_Abbreviations.tex acronyms.tex
+acrosort examples/List_Of_Abbreviations.tex sorted_acronyms.tex
 ```
 
 This will create a new `.tex` file called `sorted_acronyms.tex` with the sorted acronyms, while everything else isn't touched.
 
 It will also find the longest key to set the width of the shortform column in the acronym block.
 
 ## License
```

