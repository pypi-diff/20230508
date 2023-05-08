# Comparing `tmp/alphabetize-0.0.7.tar.gz` & `tmp/alphabetize-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphabetize-0.0.7.tar", last modified: Mon May  8 17:57:20 2023, max compression
+gzip compressed data, was "alphabetize-0.0.8.tar", last modified: Mon May  8 18:28:47 2023, max compression
```

## Comparing `alphabetize-0.0.7.tar` & `alphabetize-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:57:20.738034 alphabetize-0.0.7/
--rw-rw-rw-   0        0        0       94 2023-05-08 10:10:51.000000 alphabetize-0.0.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1087 2023-05-08 10:43:11.000000 alphabetize-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       42 2023-05-08 12:05:31.000000 alphabetize-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5320 2023-05-08 17:57:20.738034 alphabetize-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4117 2023-05-08 17:31:18.000000 alphabetize-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 17:57:20.731986 alphabetize-0.0.7/alphabetize.egg-info/
--rw-rw-rw-   0        0        0     5320 2023-05-08 17:57:20.000000 alphabetize-0.0.7/alphabetize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-08 17:57:20.000000 alphabetize-0.0.7/alphabetize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:57:20.000000 alphabetize-0.0.7/alphabetize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-08 17:57:20.000000 alphabetize-0.0.7/alphabetize.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 17:57:20.000000 alphabetize-0.0.7/alphabetize.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-08 17:57:20.000000 alphabetize-0.0.7/alphabetize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-05-08 10:27:09.000000 alphabetize-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1210 2023-05-08 17:57:20.744802 alphabetize-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1612 2023-05-08 17:54:49.000000 alphabetize-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:57:20.737036 alphabetize-0.0.7/src/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:45:55.000000 alphabetize-0.0.7/src/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-08 17:51:29.000000 alphabetize-0.0.7/src/__main__.py
--rw-rw-rw-   0        0        0     2682 2023-05-08 10:50:08.000000 alphabetize-0.0.7/src/alphabetize.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:28:47.269535 alphabetize-0.0.8/
+-rw-rw-rw-   0        0        0       94 2023-05-08 10:10:51.000000 alphabetize-0.0.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1087 2023-05-08 10:43:11.000000 alphabetize-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:05:31.000000 alphabetize-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5320 2023-05-08 18:28:47.269535 alphabetize-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-05-08 17:31:18.000000 alphabetize-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 18:28:47.263515 alphabetize-0.0.8/alphabetize.egg-info/
+-rw-rw-rw-   0        0        0     5320 2023-05-08 18:28:47.000000 alphabetize-0.0.8/alphabetize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-08 18:28:47.000000 alphabetize-0.0.8/alphabetize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 18:28:47.000000 alphabetize-0.0.8/alphabetize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-08 18:28:47.000000 alphabetize-0.0.8/alphabetize.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 18:28:47.000000 alphabetize-0.0.8/alphabetize.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-08 18:28:47.000000 alphabetize-0.0.8/alphabetize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-05-08 10:27:09.000000 alphabetize-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1210 2023-05-08 18:28:47.271502 alphabetize-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1612 2023-05-08 18:26:46.000000 alphabetize-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:28:47.268507 alphabetize-0.0.8/src/
+-rw-rw-rw-   0        0        0        0 2023-05-08 10:45:55.000000 alphabetize-0.0.8/src/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-08 17:51:29.000000 alphabetize-0.0.8/src/__main__.py
+-rw-rw-rw-   0        0        0     2765 2023-05-08 18:25:13.000000 alphabetize-0.0.8/src/alphabetize.py
```

### Comparing `alphabetize-0.0.7/LICENSE` & `alphabetize-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alphabetize-0.0.7/PKG-INFO` & `alphabetize-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabetize
-Version: 0.0.7
+Version: 0.0.8
 Summary: Alphabetize variables within your files
 Home-page: https://github.com/JakeAdey/alphabetize
 Author: Jake Adey
 Author-email: jakespenceradey@gmail.com
 License: MIT
 Keywords: variable-sorting
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alphabetize-0.0.7/README.md` & `alphabetize-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alphabetize-0.0.7/alphabetize.egg-info/PKG-INFO` & `alphabetize-0.0.8/alphabetize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabetize
-Version: 0.0.7
+Version: 0.0.8
 Summary: Alphabetize variables within your files
 Home-page: https://github.com/JakeAdey/alphabetize
 Author: Jake Adey
 Author-email: jakespenceradey@gmail.com
 License: MIT
 Keywords: variable-sorting
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alphabetize-0.0.7/setup.cfg` & `alphabetize-0.0.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alphabetize
-version = 0.0.7
+version = 0.0.8
 description = Alphabetize variables within your files
 long_description = long_description
 keywords = variable-sorting
 author = Jake Adey
 author_email = jakespenceradey@gmail.com
 url = https://github.com/JakeAdey/alphabetize
 license = MIT
```

### Comparing `alphabetize-0.0.7/setup.py` & `alphabetize-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f1:
     long_description = f1.read()
 
 setup(
     name='alphabetize',
-    version='0.0.7',
+    version='0.0.8',
     description='Alphabetize variables within your files',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="variable-sorting",
     author="Jake Adey",
     author_email="jakespenceradey@gmail.com",
     url="https://github.com/JakeAdey/alphabetize",
```

### Comparing `alphabetize-0.0.7/src/alphabetize.py` & `alphabetize-0.0.8/src/alphabetize.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             else:
                 variable_lines.sort()
                 for ordered_line in variable_lines:
                     updated_file += ordered_line + '\n'
                 updated_file += line + '\n'
                 variable_names = []
                 variable_lines = []
+        # Remove final newline created
+        updated_file = updated_file[0:-1]
         # Wipe file contents and write ordered contents
         file.seek(0)
         file.truncate()
         file.write(updated_file)
 
 
 def parse_args():
```

