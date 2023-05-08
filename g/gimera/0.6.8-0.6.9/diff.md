# Comparing `tmp/gimera-0.6.8.tar.gz` & `tmp/gimera-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.6.8.tar", last modified: Fri Jul  8 13:35:54 2022, max compression
+gzip compressed data, was "gimera-0.6.9.tar", last modified: Fri Jul  8 21:48:00 2022, max compression
```

## Comparing `gimera-0.6.8.tar` & `gimera-0.6.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 13:35:54.532995 gimera-0.6.8/
--rw-r--r--   0 marcwimmer   (501) staff       (20)     1068 2021-07-26 15:49:47.000000 gimera-0.6.8/LICENSE.txt
--rw-r--r--   0 marcwimmer   (501) staff       (20)     2317 2022-07-08 13:35:54.533078 gimera-0.6.8/PKG-INFO
--rw-r--r--   0 marcwimmer   (501) staff       (20)     1978 2022-07-05 06:37:51.000000 gimera-0.6.8/README.md
-drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 13:35:54.530357 gimera-0.6.8/gimera/
--rw-r--r--   0 marcwimmer   (501) staff       (20)      112 2022-07-05 17:42:31.000000 gimera-0.6.8/gimera/__init__.py
--rwxr-xr-x   0 marcwimmer   (501) staff       (20)    23207 2022-07-08 13:35:42.000000 gimera-0.6.8/gimera/gimera.py
--rw-r--r--   0 marcwimmer   (501) staff       (20)     4029 2022-07-08 13:35:42.000000 gimera-0.6.8/gimera/gitcommands.py
--rw-r--r--   0 marcwimmer   (501) staff       (20)     8956 2022-07-08 13:35:42.000000 gimera-0.6.8/gimera/repo.py
--rw-r--r--   0 marcwimmer   (501) staff       (20)     1138 2022-07-08 13:35:42.000000 gimera-0.6.8/gimera/tools.py
-drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 13:35:54.532848 gimera-0.6.8/gimera.egg-info/
--rw-r--r--   0 marcwimmer   (501) staff       (20)     2317 2022-07-08 13:35:54.000000 gimera-0.6.8/gimera.egg-info/PKG-INFO
--rw-r--r--   0 marcwimmer   (501) staff       (20)      311 2022-07-08 13:35:54.000000 gimera-0.6.8/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 marcwimmer   (501) staff       (20)        1 2022-07-08 13:35:54.000000 gimera-0.6.8/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 marcwimmer   (501) staff       (20)       45 2022-07-08 13:35:54.000000 gimera-0.6.8/gimera.egg-info/entry_points.txt
--rw-r--r--   0 marcwimmer   (501) staff       (20)       29 2022-07-08 13:35:54.000000 gimera-0.6.8/gimera.egg-info/requires.txt
--rw-r--r--   0 marcwimmer   (501) staff       (20)        7 2022-07-08 13:35:54.000000 gimera-0.6.8/gimera.egg-info/top_level.txt
--rw-r--r--   0 marcwimmer   (501) staff       (20)      396 2022-07-08 13:35:54.533568 gimera-0.6.8/setup.cfg
--rw-r--r--   0 marcwimmer   (501) staff       (20)     3834 2022-07-08 13:35:42.000000 gimera-0.6.8/setup.py
+drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 21:48:00.943252 gimera-0.6.9/
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     1068 2021-07-26 15:49:47.000000 gimera-0.6.9/LICENSE.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     2317 2022-07-08 21:48:00.943340 gimera-0.6.9/PKG-INFO
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     1978 2022-07-05 06:37:51.000000 gimera-0.6.9/README.md
+drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 21:48:00.923126 gimera-0.6.9/gimera/
+-rw-r--r--   0 marcwimmer   (501) staff       (20)      112 2022-07-05 17:42:31.000000 gimera-0.6.9/gimera/__init__.py
+-rwxr-xr-x   0 marcwimmer   (501) staff       (20)    23463 2022-07-08 21:47:57.000000 gimera-0.6.9/gimera/gimera.py
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     4029 2022-07-08 13:35:42.000000 gimera-0.6.9/gimera/gitcommands.py
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     8956 2022-07-08 13:35:42.000000 gimera-0.6.9/gimera/repo.py
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     1138 2022-07-08 13:35:42.000000 gimera-0.6.9/gimera/tools.py
+drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 21:48:00.943026 gimera-0.6.9/gimera.egg-info/
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     2317 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 marcwimmer   (501) staff       (20)      311 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)        1 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)       45 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)       29 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/requires.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)        7 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/top_level.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)      396 2022-07-08 21:48:00.947265 gimera-0.6.9/setup.cfg
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     3834 2022-07-08 13:35:42.000000 gimera-0.6.9/setup.py
```

### Comparing `gimera-0.6.8/LICENSE.txt` & `gimera-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.6.8/PKG-INFO` & `gimera-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.6.8
+Version: 0.6.9
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `gimera-0.6.8/README.md` & `gimera-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.6.8/gimera/gimera.py` & `gimera-0.6.9/gimera/gimera.py`

 * *Files 1% similar despite different names*

```diff
@@ -698,11 +698,20 @@
         existing_submodules = list(
             filter(lambda x: x.equals(repo.path / path), submodules)
         )
         if not existing_submodules:
             _raise_error(f"Error with submodule {path}")
         del existing_submodules
 
+@cli.command
+def completion():
+    shell = os.environ['SHELL'].split("/")[-1]
+    click.secho(
+        "\n\n"
+        f"Insert into ~/.{shell}rc\n\n"
+        f'echo \'eval "$(_GIMERA_COMPLETE={shell}_source gimera)"\' >> ~/.{shell}rc'
+        "\n\n"
+    )
 
 if __name__ == "__main__":
     # _make_sure_in_root()
     gimera()
```

### Comparing `gimera-0.6.8/gimera/gitcommands.py` & `gimera-0.6.9/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.8/gimera/repo.py` & `gimera-0.6.9/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.8/gimera/tools.py` & `gimera-0.6.9/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.8/gimera.egg-info/PKG-INFO` & `gimera-0.6.9/gimera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.6.8
+Version: 0.6.9
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `gimera-0.6.8/setup.py` & `gimera-0.6.9/setup.py`

 * *Files identical despite different names*

