# Comparing `tmp/toml-sort-0.8.0.tar.gz` & `tmp/toml-sort-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml-sort-0.8.0.tar", last modified: Thu Aug  8 19:54:23 2019, max compression
+gzip compressed data, was "toml-sort-0.9.0.tar", last modified: Mon Aug 12 22:19:37 2019, max compression
```

## Comparing `toml-sort-0.8.0.tar` & `toml-sort-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2019-08-06 17:10:57.179862 toml-sort-0.8.0/LICENSE
--rw-r--r--   0        0        0     1766 2019-08-08 19:54:10.928915 toml-sort-0.8.0/README.md
--rw-r--r--   0        0        0     1766 2019-08-08 19:54:10.928915 toml-sort-0.8.0/README.md
--rw-r--r--   0        0        0     1302 2019-08-08 19:54:10.928915 toml-sort-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       87 2019-08-08 17:24:46.726390 toml-sort-0.8.0/toml_sort/__init__.py
--rw-r--r--   0        0        0     1587 2019-08-08 17:24:46.726390 toml-sort-0.8.0/toml_sort/cli.py
--rw-r--r--   0        0        0        0 2019-08-06 17:10:57.179862 toml-sort-0.8.0/toml_sort/py.typed
--rw-r--r--   0        0        0     4232 2019-08-08 19:54:10.928915 toml-sort-0.8.0/toml_sort/tomlsort.py
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 toml-sort-0.8.0/setup.py
--rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 toml-sort-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2019-08-05 12:39:54.925097 toml-sort-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1766 2019-08-12 22:16:41.528471 toml-sort-0.9.0/README.md
+-rw-r--r--   0        0        0     1766 2019-08-12 22:16:41.528471 toml-sort-0.9.0/README.md
+-rw-r--r--   0        0        0     1302 2019-08-12 22:18:22.768471 toml-sort-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2019-08-07 15:14:11.812911 toml-sort-0.9.0/toml_sort/__init__.py
+-rw-r--r--   0        0        0     1621 2019-08-12 22:16:02.776471 toml-sort-0.9.0/toml_sort/cli.py
+-rw-r--r--   0        0        0        0 2019-08-04 17:06:04.663993 toml-sort-0.9.0/toml_sort/py.typed
+-rw-r--r--   0        0        0     4232 2019-08-12 22:16:41.528471 toml-sort-0.9.0/toml_sort/tomlsort.py
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 toml-sort-0.9.0/setup.py
+-rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 toml-sort-0.9.0/PKG-INFO
```

### Comparing `toml-sort-0.8.0/LICENSE` & `toml-sort-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toml-sort-0.8.0/README.md` & `toml-sort-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `toml-sort-0.8.0/pyproject.toml` & `toml-sort-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry]
 name = "toml-sort"
-version = "0.8.0"
+version = "0.9.0"
 description = "Toml sorting library"
 authors = ["Sam Roeca <samuel.roeca@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/pappasam/toml-sort"
 repository = "https://github.com/pappasam/toml-sort"
 keywords = ["toml", "sort", "cli", "unix", "utility"]
 classifiers = [
```

### Comparing `toml-sort-0.8.0/toml_sort/cli.py` & `toml-sort-0.9.0/toml_sort/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,22 +19,26 @@
     "--output",
     type=click.File("w"),
     default="-",
     show_default=True,
     help="The output filepath. Choose stdout with '-'.",
 )
 @click.option(
-    "-i",
-    "--ignore-non-tables",
+    "-a",
+    "--all",
+    "_all",
     is_flag=True,
-    help="Only sort top-level Tables / Arrays of Tables",
+    help=(
+        "Sort all keys. "
+        "Default is to only sort non-inline 'tables and arrays of tables'."
+    ),
 )
 @click.argument("filename", type=click.File("r"), default="-")
 @click.version_option()
-def cli(output, ignore_non_tables, filename) -> None:
+def cli(output, _all, filename) -> None:
     """Sort toml file FILENAME, saving results to a file, or stdout (default)
 
     FILENAME a filepath or standard input (-)
 
     Examples:
 
         Read from stdin, write to stdout:
@@ -49,19 +53,18 @@
 
             toml-sort input.toml
 
         Read from stdin, write to file on disk
 
             cat input.toml | toml-sort -o output.toml
 
-        Only sort the top-level tables / arrays of tables
+        Sort all keys, not just top-level / table keys
 
-            cat input.toml | toml-sort -i
+            cat input.toml | toml-sort -a
     """
     if filename.isatty():
         click.echo(get_help())
         return
-
-    only_sort_tables = bool(ignore_non_tables)
+    only_sort_tables = not bool(_all)
     toml_content = filename.read()
     sorted_toml = TomlSort(toml_content, only_sort_tables).sorted()
     output.write(sorted_toml)
```

### Comparing `toml-sort-0.8.0/toml_sort/tomlsort.py` & `toml-sort-0.9.0/toml_sort/tomlsort.py`

 * *Files identical despite different names*

### Comparing `toml-sort-0.8.0/setup.py` & `toml-sort-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=7.0,<8.0', 'tomlkit>=0.5.5']
 
 entry_points = \
 {'console_scripts': ['toml-sort = toml_sort.cli:cli']}
 
 setup_kwargs = {
     'name': 'toml-sort',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Toml sorting library',
     'long_description': '# toml-sort\n\nA command line utility to sort your toml files. Requires Python 3.6 or greater.\n\n## Motivation\n\nI wrote this library because I couldn\'t find any "good" sorting utilities for TOML files. This library strives to sort TOML files by providing the following features:\n\n* Preserve inline comments\n* Sort tables / arrays of Tables\n* Option to sort table keys, or not\n* Standardize top-level whitespace and indentation (generally removes it; this library is opinionated here)\n* Preserve top-level comments (in progress; really hard and maybe unachievable)\n\n## Installation\n\n```bash\npip install toml-sort\n```\n\n## Usage\n\nThis project can be used as either a Python library or a command line utility. I will document the Python library interface in the future when it stabilizes. The command line interface should remain fairly stable.\n\n### Command line interface\n\nRead from stdin, write to stdout:\n\n    cat input.toml | toml-sort\n\nRead from file on disk, write to file on disk:\n\n    toml-sort -o output.toml input.toml\n\nRead from file on disk, write to stdout\n\n    toml-sort input.toml\n\nRead from stdin, write to file on disk\n\n    cat input.toml | toml-sort -o output.toml\n\nOnly sort the top-level tables / arrays of tables\n\n    cat input.toml | toml-sort -i\n    cat input.toml | toml-sort --ignore-non-tables\n\n## Local Development\n\nLocal development for this project is quite simple.\n\n**Dependencies**\n\nInstall the following tools manually.\n\n* [Poetry](https://github.com/sdispater/poetry#installation)\n* [GNU Make](https://www.gnu.org/software/make/)\n\n*Recommended*\n\n* [pyenv](https://github.com/pyenv/pyenv)\n\n**Set up development environment**\n\n```bash\nmake setup\n```\n\n**Run Tests**\n\n```bash\nmake test\n```\n\n## Written by\n\nSamuel Roeca *samuel.roeca@gmail.com*\n',
     'author': 'Sam Roeca',
     'author_email': 'samuel.roeca@gmail.com',
     'url': 'https://github.com/pappasam/toml-sort',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `toml-sort-0.8.0/PKG-INFO` & `toml-sort-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml-sort
-Version: 0.8.0
+Version: 0.9.0
 Summary: Toml sorting library
 Home-page: https://github.com/pappasam/toml-sort
 License: MIT
 Keywords: toml,sort,cli,unix,utility
 Author: Sam Roeca
 Author-email: samuel.roeca@gmail.com
 Requires-Python: >=3.6,<4.0
```

