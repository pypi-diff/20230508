# Comparing `tmp/mobie-4.0.2.tar.gz` & `tmp/mobie-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobie-4.0.2.tar", last modified: Sun May  7 13:58:16 2023, max compression
+gzip compressed data, was "mobie-4.0.3.tar", last modified: Mon May  8 08:50:36 2023, max compression
```

## Comparing `mobie-4.0.2.tar` & `mobie-4.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:58:16.579856 mobie-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-07 13:58:14.000000 mobie-4.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-07 13:58:16.579856 mobie-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-07 13:58:14.000000 mobie-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:58:16.579856 mobie-4.0.2/mobie/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-07 13:58:14.000000 mobie-4.0.2/mobie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:58:16.579856 mobie-4.0.2/mobie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 13:58:16.579856 mobie-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-07 13:58:14.000000 mobie-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:36.916808 mobie-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-08 08:50:35.000000 mobie-4.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 08:50:36.916808 mobie-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-08 08:50:35.000000 mobie-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:36.916808 mobie-4.0.3/mobie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-08 08:50:35.000000 mobie-4.0.3/mobie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:36.916808 mobie-4.0.3/mobie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:50:36.916808 mobie-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 08:50:35.000000 mobie-4.0.3/setup.py
```

### Comparing `mobie-4.0.2/LICENSE.txt` & `mobie-4.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mobie-4.0.2/README.md` & `mobie-4.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 ```
 
 ### Test within Java on the command line
 
 1. cd to the main folder of mobie-viewer-fiji
 2. ./install.sh
 3. ./mobie-files -r "/Users/tischer/Documents/mobie/src/test/resources/input/skimage-2d-tiff/" -i "image.tif" -l "segmentation.tif" -t "table.tsv" 
+4. ./mobie-hcs
+
 
 ### Test within python using a local MoBIE build
 
 1. mvn install current version (could be a SNAPSHOT)
 2. hardcode this version in `__init__.py`: e.g., 
    `_artifactVersion         = '3.2.0-SNAPSHOT' #version("mobie")` 
    
@@ -35,14 +37,15 @@
 ### Release a new version
 
 Example for version `3.0.10`:
 
 #### mobie-viewer-fiji repo
 
 Within the mobie Java code update the versions in all command line tools, e.g.:
+
 ```java
 @CommandLine.Command(name = "mobie", mixinStandardHelpOptions = true, version = "3.0.10", description = "Visualise multi-modal big image data, see https://mobie.github.io/")
 ```
 
 Use the below lines to make a maven release:
 
 ```
@@ -52,30 +55,38 @@
 ../scijava-scripts/release-version.sh --skip-version-check --skip-license-update
 # if successful this will say
 # * [new tag]mobie-viewer-fiji-3.0.10 -> mobie-viewer-fiji-3.0.10
 ```
 
 #### mobie-cmd repo
 
-Go to `setup.py` and change the `version` to `3.0.10`
+Within `mobie/__init.py__` ensure that
+`_artifactVersion = version("mobie")`   
+
+Within `setup.py` set `version` to `3.0.10`
 
 ```
 git add setup.py
 git commit -m "Version bump 3.0.10"
 ```
 
 
 #### test locally
 
+TODO: add test data for mobie hcs
+TODO: add test data for mobie table
+
 ```
 mamba activate mobie-dev
 pip install -e .
 mobie --help
 mobie project -p "https://github.com/mobie/platybrowser-project"
 mobie files -r "/Users/tischer/Documents/mobie/src/test/resources/input/skimage-2d-tiff/" -i "image.tif" -l "segmentation.tif" -t "table.tsv"
+mobie hcs
+mobie table
 ```
 
 #### deploy to pypi
 
 ```
 git tag 3.0.10
 git push --tags
```

### Comparing `mobie-4.0.2/mobie/__init__.py` & `mobie-4.0.3/mobie/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     mobie_project = sub.add_parser("table", add_help=False)
     mobie_project.set_defaults(func=partial(launch_mobie, "org.embl.mobie.cmd.TableCmd"))
     mobie_files = sub.add_parser("hcs", add_help=False)
     mobie_files.set_defaults(func=partial(launch_mobie, "org.embl.mobie.cmd.HCSCmd"))
 
     # subparsers don't specify any options, everything is passed to MoBiE
     args, unknown = p.parse_known_args()
-    args.func(mobie_options=unknown)
+    return args.func(mobie_options=unknown)
```

### Comparing `mobie-4.0.2/setup.py` & `mobie-4.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 entry_points = {
     "console_scripts": [
         "mobie=mobie:main",
     ]
 }
 
-version = "4.0.2"
+version = "4.0.3"
 
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 package_urls = {
```

