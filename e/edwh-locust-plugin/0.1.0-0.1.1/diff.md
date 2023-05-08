# Comparing `tmp/edwh_locust_plugin-0.1.0.tar.gz` & `tmp/edwh_locust_plugin-0.1.1.tar.gz`

## Comparing `edwh_locust_plugin-0.1.0.tar` & `edwh_locust_plugin-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/src/edwh_locust_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/src/edwh_locust_plugin/__init__.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/src/edwh_locust_plugin/locust_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/src/edwh_locust_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/src/edwh_locust_plugin/__init__.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/src/edwh_locust_plugin/locust_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 edwh_locust_plugin-0.1.1/PKG-INFO
```

### Comparing `edwh_locust_plugin-0.1.0/src/edwh_locust_plugin/locust_plugin.py` & `edwh_locust_plugin-0.1.1/src/edwh_locust_plugin/locust_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_locust_plugin-0.1.0/LICENSE.txt` & `edwh_locust_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_locust_plugin-0.1.0/README.md` & `edwh_locust_plugin-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
-## USING THIS TEMPLATE REPOSITORY
-1. remove this markdown section;
-2. replace 'locust' in README.md, pyproject.toml and the name of the plugin in `src` to your actual plugin name;
-3. (add your actual plugin code of course);
-4. run `semantic-release publish`, `hatch build -c` and `hatch publish`.
-
 ## Installation
 
 ```console
 pip install edwh-locust-plugin
 ```
 
 But probably you want to install the whole edwh package:
```

### Comparing `edwh_locust_plugin-0.1.0/pyproject.toml` & `edwh_locust_plugin-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_locust_plugin-0.1.0/PKG-INFO` & `edwh_locust_plugin-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-locust-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: locust project with a plugin to be discovered from the edwh package
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-locust-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-locust-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-locust-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -30,20 +30,14 @@
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
-## USING THIS TEMPLATE REPOSITORY
-1. remove this markdown section;
-2. replace 'locust' in README.md, pyproject.toml and the name of the plugin in `src` to your actual plugin name;
-3. (add your actual plugin code of course);
-4. run `semantic-release publish`, `hatch build -c` and `hatch publish`.
-
 ## Installation
 
 ```console
 pip install edwh-locust-plugin
 ```
 
 But probably you want to install the whole edwh package:
```

