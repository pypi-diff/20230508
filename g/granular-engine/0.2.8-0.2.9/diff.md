# Comparing `tmp/granular_engine-0.2.8.tar.gz` & `tmp/granular_engine-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granular_engine-0.2.8.tar", max compression
+gzip compressed data, was "granular_engine-0.2.9.tar", max compression
```

## Comparing `granular_engine-0.2.8.tar` & `granular_engine-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.8/README.rst
--rwxr-xr-x   0        0        0      210 2023-05-08 21:21:35.106995 granular_engine-0.2.8/engine/__init__.py
--rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.8/engine/cli/__init__.py
--rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.8/engine/cli/auth.py
--rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.8/engine/cli/experiment.py
--rwxr-xr-x   0        0        0    12915 2023-05-08 21:21:28.024867 granular_engine-0.2.8/engine/cli/project.py
--rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.8/engine/connections/__init__.py
--rwxr-xr-x   0        0        0     5202 2023-05-08 21:01:13.100756 granular_engine-0.2.8/engine/connections/callisto.py
--rwxr-xr-x   0        0        0     4350 2023-05-08 08:52:31.363502 granular_engine-0.2.8/engine/connections/dione.py
--rwxr-xr-x   0        0        0     6310 2023-05-08 21:01:13.116774 granular_engine-0.2.8/engine/connections/europa.py
--rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.8/engine/connections/neso.py
--rwxr-xr-x   0        0        0     4754 2023-05-08 08:52:31.383917 granular_engine-0.2.8/engine/grain.py
--rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.8/engine/libs/__init__.py
--rwxr-xr-x   0        0        0    46675 2023-05-08 21:01:13.134631 granular_engine-0.2.8/engine/libs/config.py
--rwxr-xr-x   0        0        0     1453 2023-05-08 21:01:13.150663 granular_engine-0.2.8/engine/libs/inquirer.py
--rwxr-xr-x   0        0        0     4607 2023-05-08 21:01:13.162994 granular_engine-0.2.8/engine/libs/utils.py
--rwxr-xr-x   0        0        0     1252 2023-05-08 21:21:35.099472 granular_engine-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 granular_engine-0.2.8/PKG-INFO
+-rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.9/README.rst
+-rwxr-xr-x   0        0        0      210 2023-05-08 21:25:20.706197 granular_engine-0.2.9/engine/__init__.py
+-rwxr-xr-x   0        0        0      881 2023-05-02 13:15:25.911286 granular_engine-0.2.9/engine/cli/__init__.py
+-rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.9/engine/cli/auth.py
+-rwxr-xr-x   0        0        0     4081 2023-05-07 09:47:59.211514 granular_engine-0.2.9/engine/cli/experiment.py
+-rwxr-xr-x   0        0        0    12907 2023-05-08 21:25:03.574304 granular_engine-0.2.9/engine/cli/project.py
+-rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.9/engine/connections/__init__.py
+-rwxr-xr-x   0        0        0     5202 2023-05-08 21:01:13.100756 granular_engine-0.2.9/engine/connections/callisto.py
+-rwxr-xr-x   0        0        0     4350 2023-05-08 08:52:31.363502 granular_engine-0.2.9/engine/connections/dione.py
+-rwxr-xr-x   0        0        0     6310 2023-05-08 21:01:13.116774 granular_engine-0.2.9/engine/connections/europa.py
+-rwxr-xr-x   0        0        0     1281 2023-05-07 09:47:59.242275 granular_engine-0.2.9/engine/connections/neso.py
+-rwxr-xr-x   0        0        0     4754 2023-05-08 08:52:31.383917 granular_engine-0.2.9/engine/grain.py
+-rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.9/engine/libs/__init__.py
+-rwxr-xr-x   0        0        0    46675 2023-05-08 21:01:13.134631 granular_engine-0.2.9/engine/libs/config.py
+-rwxr-xr-x   0        0        0     1453 2023-05-08 21:01:13.150663 granular_engine-0.2.9/engine/libs/inquirer.py
+-rwxr-xr-x   0        0        0     4607 2023-05-08 21:01:13.162994 granular_engine-0.2.9/engine/libs/utils.py
+-rwxr-xr-x   0        0        0     1252 2023-05-08 21:25:20.699605 granular_engine-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 granular_engine-0.2.9/PKG-INFO
```

### Comparing `granular_engine-0.2.8/README.rst` & `granular_engine-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/cli/__init__.py` & `granular_engine-0.2.9/engine/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/cli/auth.py` & `granular_engine-0.2.9/engine/cli/auth.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/cli/experiment.py` & `granular_engine-0.2.9/engine/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/cli/project.py` & `granular_engine-0.2.9/engine/cli/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
                 with open(save_path, 'w') as fout:
                     fout.write(cfg_string)
                     print ("Saved to " + Fore.GREEN + save_path + Style.RESET_ALL)
 
                 print ()
 
                 print ("You can use the config file using geolibs.")
-                print (Fore.GREEN + f"python geolibs/tools/train.py {save_path}" + Style.RESET_ALL)
+                print (Fore.GREEN + f"python tools/train.py {save_path}" + Style.RESET_ALL)
                 print ("\n")
 
         print ("You can download the dataset using following command. Please make sure it is inside data folder.")
         project_name = project['name'].replace(' ', '_')
         print (Fore.MAGENTA + f"mkdir data data/{project_name}")
         print (f"mkdir data/{project_name}/rasters data/{project_name}/vectors")
         print (f"gsutil -m cp -n -r {project['bucketPath']}/rasters/raw data/{project_name}/rasters/")
```

### Comparing `granular_engine-0.2.8/engine/connections/callisto.py` & `granular_engine-0.2.9/engine/connections/callisto.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/connections/dione.py` & `granular_engine-0.2.9/engine/connections/dione.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/connections/europa.py` & `granular_engine-0.2.9/engine/connections/europa.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/connections/neso.py` & `granular_engine-0.2.9/engine/connections/neso.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/grain.py` & `granular_engine-0.2.9/engine/grain.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/libs/config.py` & `granular_engine-0.2.9/engine/libs/config.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/libs/inquirer.py` & `granular_engine-0.2.9/engine/libs/inquirer.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/engine/libs/utils.py` & `granular_engine-0.2.9/engine/libs/utils.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.8/pyproject.toml` & `granular_engine-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "granular-engine"
-version = "v0.2.8"
+version = "v0.2.9"
 description = "Experiment tracking for GeoSpatial Machine Learning on GeoEngine"
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "engine"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `granular_engine-0.2.8/PKG-INFO` & `granular_engine-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granular-engine
-Version: 0.2.8
+Version: 0.2.9
 Summary: Experiment tracking for GeoSpatial Machine Learning on GeoEngine
 Home-page: https://github.com/granularai/engine
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

