# Comparing `tmp/get_all_files-0.1.0.tar.gz` & `tmp/get_all_files-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_all_files-0.1.0.tar", max compression
+gzip compressed data, was "get_all_files-0.2.0.tar", max compression
```

## Comparing `get_all_files-0.1.0.tar` & `get_all_files-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-05-01 03:49:13.250535 get_all_files-0.1.0/LICENSE
--rw-r--r--   0        0        0     1877 2023-05-01 03:49:13.250535 get_all_files-0.1.0/README.md
--rw-r--r--   0        0        0      198 2023-05-01 03:49:13.250535 get_all_files-0.1.0/get_all_files/__init__.py
--rw-r--r--   0        0        0     2925 2023-05-01 03:49:13.250535 get_all_files-0.1.0/get_all_files/_get_all_files.py
--rw-r--r--   0        0        0      644 2023-05-01 03:49:13.250535 get_all_files-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 get_all_files-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-08 01:12:21.808449 get_all_files-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2149 2023-05-08 01:12:21.808449 get_all_files-0.2.0/README.md
+-rw-r--r--   0        0        0      198 2023-05-08 01:12:21.808449 get_all_files-0.2.0/get_all_files/__init__.py
+-rw-r--r--   0        0        0     2958 2023-05-08 01:12:21.808449 get_all_files-0.2.0/get_all_files/_get_all_files.py
+-rw-r--r--   0        0        0      644 2023-05-08 01:12:21.808449 get_all_files-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 get_all_files-0.2.0/PKG-INFO
```

### Comparing `get_all_files-0.1.0/LICENSE` & `get_all_files-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `get_all_files-0.1.0/README.md` & `get_all_files-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # READ ME
 
 ![tests](https://github.com/bwheelz36/get_all_files/actions/workflows/run_tests.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/get_all_files.svg)](https://badge.fury.io/py/get_all_files)
 [![codecov](https://codecov.io/gh/bwheelz36/get_all_files/branch/main/graph/badge.svg?token=CCVB5BAR8W)](https://codecov.io/gh/bwheelz36/get_all_files)
 
 
-This is a very simple package which simply gets all the files with extension matching a list of extensions in a given
+This is a very simple package which is basically a wrapper around glob; it simply gets all the files with extension matching a list of extensions in a given
 directory. I found that I was including functionality like this in so many other projects I might as well just make
-it a package. Plus I wanted to play with poetry.
+it a package. Plus I wanted to play with poetry. 
 
 ## install 
 
 ```bash
 pip install get_all_files
 ```
 
@@ -31,14 +31,23 @@
 from get_all_files import get_all_files
 from pathlib import Path
 
 home_dir = Path('~').expanduser()
 jpg_files = get_all_files(home_dir, ['jpg', 'png'])
 ```
 
+**get all jpg files starting with 'a' in home directory**
+```python
+from get_all_files import get_all_files
+from pathlib import Path
+
+home_dir = Path('~').expanduser()
+jpg_files = get_all_files(home_dir, 'jpg', file_name='a*')
+```
+
 **get absolute file paths instead of file names**
 ```python
 from get_all_files import get_all_files
 from pathlib import Path
 
 home_dir = Path('~').expanduser()
 jpg_files = get_all_files(home_dir, ['jpg', 'png'], return_absolute_filepath=True)
```

### Comparing `get_all_files-0.1.0/get_all_files/_get_all_files.py` & `get_all_files-0.2.0/get_all_files/_get_all_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,51 +28,51 @@
     if not isinstance(file_extensions, list):
         raise TypeError(f'file_extensions must be type str or list, not {type(file_extensions)}')
     processed_extensions = []
     for extension in file_extensions:
         if not file_extensions[0] == '.':
             # handles the case where the user entered 'jpg' instead of '.jpg'
             extension = '.' + extension
-        # add wildcard
-        extension = '*' + extension
-        # verify that this is now in the format we require
-        if not extension[0:2] == '*.':
-            # don't think it's possible to get here but just in case
-            raise Exception('please enter the file_extensions parameter like this : file_extensions = "jpg"')
         processed_extensions.append(extension)
     return processed_extensions
 
 
-def _get_all_files(path_to_data: (Path, str), file_extensions: (str, list),
+def _get_all_files(path_to_data: (Path, str),
+                   file_extensions: (str, list),
+                   file_name: str = '*',
                    return_absolute_filepath: bool = False) -> list:
     """
-    quick script to just collect all the files in the Analysis path
+    quick script to just collect all the files in the Analysis path. Basically a wrapper around glob with (for me)
+    easier to use syntax.
 
     :param path_to_data: folder where the files are
     :type path_to_data: pathlib.Path, string
     :param file_extensions: extension of files to return, e.g. 'dcm'
     :type file_extensions: str, list
+    :param file_name: string to match files to; defaults to '*' which gives all files matching the extensions. set to
+        e.g. 'a*' to get all files starting with a
     :param return_absolute_filepath: if False (default) file names are returned; if True absolute file names returned
     :returns Files: list of all found files
     """
     # process input path:
     path_to_data = _process_input_path(path_to_data)
 
     # process extensions:
     file_extensions = _process_extensions(file_extensions)
 
     Files = []
     for extension in file_extensions:
+        search_string = file_name + extension
         # find the files matching this extension
-        AllFiles = glob.glob(str(path_to_data / extension))
+        AllFiles = glob.glob(str(path_to_data / search_string))
         # process all found files into desired format
         for file in AllFiles:
             if return_absolute_filepath:
                 Files.append(file)
             else:
                 head, tail = os.path.split(file)
                 Files.append(tail)
 
         if not Files:
-            warnings.warn(f'no {extension} files in {path_to_data}')
+            warnings.warn(f'\nno files matching {search_string} in {path_to_data}\n')
 
     return Files
```

### Comparing `get_all_files-0.1.0/pyproject.toml` & `get_all_files-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get-all-files"
-version = "0.1.0"
+version = "0.2.0"
 description = "a simple package to get all files with given file extension in a directory"
 authors = ["brendan whelan <bwheelz360@gmail.com>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "get_all_files"}]
 
 [tool.poetry.dependencies]
```

### Comparing `get_all_files-0.1.0/PKG-INFO` & `get_all_files-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-all-files
-Version: 0.1.0
+Version: 0.2.0
 Summary: a simple package to get all files with given file extension in a directory
 License: LICENSE
 Author: brendan whelan
 Author-email: bwheelz360@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -17,17 +17,17 @@
 # READ ME
 
 ![tests](https://github.com/bwheelz36/get_all_files/actions/workflows/run_tests.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/get_all_files.svg)](https://badge.fury.io/py/get_all_files)
 [![codecov](https://codecov.io/gh/bwheelz36/get_all_files/branch/main/graph/badge.svg?token=CCVB5BAR8W)](https://codecov.io/gh/bwheelz36/get_all_files)
 
 
-This is a very simple package which simply gets all the files with extension matching a list of extensions in a given
+This is a very simple package which is basically a wrapper around glob; it simply gets all the files with extension matching a list of extensions in a given
 directory. I found that I was including functionality like this in so many other projects I might as well just make
-it a package. Plus I wanted to play with poetry.
+it a package. Plus I wanted to play with poetry. 
 
 ## install 
 
 ```bash
 pip install get_all_files
 ```
 
@@ -47,14 +47,23 @@
 from get_all_files import get_all_files
 from pathlib import Path
 
 home_dir = Path('~').expanduser()
 jpg_files = get_all_files(home_dir, ['jpg', 'png'])
 ```
 
+**get all jpg files starting with 'a' in home directory**
+```python
+from get_all_files import get_all_files
+from pathlib import Path
+
+home_dir = Path('~').expanduser()
+jpg_files = get_all_files(home_dir, 'jpg', file_name='a*')
+```
+
 **get absolute file paths instead of file names**
 ```python
 from get_all_files import get_all_files
 from pathlib import Path
 
 home_dir = Path('~').expanduser()
 jpg_files = get_all_files(home_dir, ['jpg', 'png'], return_absolute_filepath=True)
```

