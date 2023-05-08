# Comparing `tmp/docbuild-0.1.105.tar.gz` & `tmp/docbuild-0.1.106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.105.tar", last modified: Sun Apr 30 11:58:07 2023, max compression
+gzip compressed data, was "docbuild-0.1.106.tar", last modified: Mon May  8 09:08:18 2023, max compression
```

## Comparing `docbuild-0.1.105.tar` & `docbuild-0.1.106.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.555246 docbuild-0.1.105/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-30 11:58:07.554589 docbuild-0.1.105/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.105/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.543852 docbuild-0.1.105/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-30 11:57:46.000000 docbuild-0.1.105/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.105/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.105/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.105/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7054 2023-04-29 18:09:32.000000 docbuild-0.1.105/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.549383 docbuild-0.1.105/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.105/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.105/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.105/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.105/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.105/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     5805 2023-04-30 08:43:31.000000 docbuild-0.1.105/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.105/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.553007 docbuild-0.1.105/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.105/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12923 2023-04-30 11:56:34.000000 docbuild-0.1.105/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.105/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16325 2023-04-30 05:58:58.000000 docbuild-0.1.105/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.546627 docbuild-0.1.105/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-30 11:58:07.555300 docbuild-0.1.105/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-30 11:57:59.000000 docbuild-0.1.105/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.401326 docbuild-0.1.106/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-08 09:08:18.401112 docbuild-0.1.106/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.106/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.394006 docbuild-0.1.106/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-05-08 09:07:48.000000 docbuild-0.1.106/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.106/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.106/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.106/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7054 2023-04-29 18:09:32.000000 docbuild-0.1.106/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.398018 docbuild-0.1.106/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.106/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.106/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.106/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.106/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.106/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6087 2023-05-08 09:07:21.000000 docbuild-0.1.106/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.106/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.400138 docbuild-0.1.106/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.106/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12923 2023-04-30 11:56:34.000000 docbuild-0.1.106/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.106/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16325 2023-04-30 05:58:58.000000 docbuild-0.1.106/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.396395 docbuild-0.1.106/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       83 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-05-08 09:08:18.401377 docbuild-0.1.106/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-05-08 09:08:02.000000 docbuild-0.1.106/setup.py
```

### Comparing `docbuild-0.1.105/PKG-INFO` & `docbuild-0.1.106/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.105
+Version: 0.1.106
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.105/docbuild/graph.py` & `docbuild-0.1.106/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/hocr_parser.py` & `docbuild-0.1.106/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/page_creator.py` & `docbuild-0.1.106/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.106/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.106/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.106/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/textract_parser.py` & `docbuild-0.1.106/docbuild/textract_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from docstruct import BoundingBox, TextBlock, Word, Line
 from .constants import LINE, WORD
-
+import logging
 
 
 class TextractParser:
     def __init__(self, textract_response: dict):
         self.textract_response = textract_response
         self.validate_args()
         self.words: list[dict] = []
@@ -51,15 +51,21 @@
         """
         return any(char.isspace() for char in word.text)
 
     def get_non_space_slices(self, word: Word) -> list[slice]:
         space_indexes = [i for i, char in enumerate(word.text) if char.isspace()]
         space_indexes.insert(0, -1)
         space_indexes.append(len(word.text))
-        non_space_slices = [slice(space_indexes[i]+1, space_indexes[i+1]) for i in range(len(space_indexes) -1)]
+        non_space_slices = []
+        for i in range(len(space_indexes) - 1):
+            if space_indexes[i+1] == space_indexes[i] + 1:
+                continue
+            current_slice = slice(space_indexes[i]+1, space_indexes[i+1])
+            non_space_slices.append(current_slice)
+
         return non_space_slices
 
     def split_word_by_space(self, word: Word) -> list[Word]:
         """
         Split a word by space
         """
         non_space_slices = self.get_non_space_slices(word)
@@ -146,16 +152,19 @@
 
     def parse_lines(self, lines_dict: list[dict]) -> list[Line]:
         """
         Parse the lines
         """
         lines = []
         for line_dict in lines_dict:
-            line = self.get_line(line_dict)
-            lines.append(line)
+            try:
+                line = self.get_line(line_dict)
+                lines.append(line)
+            except Exception as e:
+                logging.error(e)
         return lines
 
     def parse_response(self) -> list[Line]:
         """
         Parse the textract response and return the page object
         """
         self.words, self.lines = self.split_blocks_by_type(self.textract_response)
```

### Comparing `docbuild-0.1.105/docbuild/utils.py` & `docbuild-0.1.106/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.106/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.106/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.106/docbuild.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.105
+Version: 0.1.106
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.105/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.106/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.105/setup.py` & `docbuild-0.1.106/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.105",
+    version="0.1.106",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

