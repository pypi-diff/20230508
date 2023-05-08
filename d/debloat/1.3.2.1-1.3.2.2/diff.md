# Comparing `tmp/debloat-1.3.2.1.tar.gz` & `tmp/debloat-1.3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.3.2.1.tar", last modified: Thu Apr 20 03:44:43 2023, max compression
+gzip compressed data, was "debloat-1.3.2.2.tar", last modified: Mon May  8 11:40:06 2023, max compression
```

## Comparing `debloat-1.3.2.1.tar` & `debloat-1.3.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:43.233525 debloat-1.3.2.1/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.3.2.1/LICENSE
--rw-rw-rw-   0        0        0     7407 2023-04-20 03:44:43.234025 debloat-1.3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.3.2.1/README.md
--rw-rw-rw-   0        0        0      790 2023-04-20 03:26:32.000000 debloat-1.3.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-04-20 03:44:43.235525 debloat-1.3.2.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.3.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:43.187027 debloat-1.3.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:43.210024 debloat-1.3.2.1/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-04-20 03:26:52.000000 debloat-1.3.2.1/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.3.2.1/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     3835 2023-04-20 03:29:34.000000 debloat-1.3.2.1/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1564 2023-04-20 03:44:03.000000 debloat-1.3.2.1/src/debloat/main.py
--rw-rw-rw-   0        0        0    19474 2023-04-16 12:04:38.000000 debloat-1.3.2.1/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:43.232523 debloat-1.3.2.1/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7407 2023-04-20 03:44:43.000000 debloat-1.3.2.1/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-04-20 03:44:43.000000 debloat-1.3.2.1/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 03:44:43.000000 debloat-1.3.2.1/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-04-20 03:44:43.000000 debloat-1.3.2.1/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-04-20 03:44:43.000000 debloat-1.3.2.1/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 03:44:43.000000 debloat-1.3.2.1/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.836589 debloat-1.3.2.2/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.3.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7407 2023-05-08 11:40:06.836589 debloat-1.3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.3.2.2/README.md
+-rw-rw-rw-   0        0        0      790 2023-05-08 11:36:50.000000 debloat-1.3.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-05-08 11:40:06.838089 debloat-1.3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.791591 debloat-1.3.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.808590 debloat-1.3.2.2/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:26:52.000000 debloat-1.3.2.2/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.3.2.2/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3835 2023-04-20 03:29:34.000000 debloat-1.3.2.2/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1564 2023-05-05 02:45:32.000000 debloat-1.3.2.2/src/debloat/main.py
+-rw-rw-rw-   0        0        0    19515 2023-05-08 11:29:58.000000 debloat-1.3.2.2/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.835589 debloat-1.3.2.2/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     7407 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.3.2.1/LICENSE` & `debloat-1.3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.1/PKG-INFO` & `debloat-1.3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.3.2.1
+Version: 1.3.2.2
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `debloat-1.3.2.1/README.md` & `debloat-1.3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.1/pyproject.toml` & `debloat-1.3.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.3.2.1"
+version = "1.3.2.2"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.3.2.1/src/debloat/gui.py` & `debloat-1.3.2.2/src/debloat/gui.py`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.1/src/debloat/main.py` & `debloat-1.3.2.2/src/debloat/main.py`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.1/src/debloat/processor.py` & `debloat-1.3.2.2/src/debloat/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 Entropy of section is exteremely low. This is indicative of a bloated section. 
 Removing bloated section... 
 ''', end="", flush=True)
                 # Get the size of the section.
                 section_end = section.PointerToRawData + section.SizeOfRawData
                 # If the entropy is simply 0.00, there is no data to be 
                 # missed, we won't waste CPU and just drop the whole thing.
+                delta_last_non_junk = 0
                 if section_entropy == 0.00:
                     # To play it safe, we will leave 100 bytes in the 
                     # section. And thus mark the end of the binary as 
                     # the beginning of the last section + 100.
                     section_bytes_to_remove = section.SizeOfRawData - 100
                     end_of_real_data = section.PointerToRawData + 100
                 # If the section has low entropy we'll try to determine
```

### Comparing `debloat-1.3.2.1/src/debloat.egg-info/PKG-INFO` & `debloat-1.3.2.2/src/debloat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.3.2.1
+Version: 1.3.2.2
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

