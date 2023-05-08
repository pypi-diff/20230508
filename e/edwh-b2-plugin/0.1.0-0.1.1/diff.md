# Comparing `tmp/edwh_b2_plugin-0.1.0.tar.gz` & `tmp/edwh_b2_plugin-0.1.1.tar.gz`

## Comparing `edwh_b2_plugin-0.1.0.tar` & `edwh_b2_plugin-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/src/edwh_b2_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/src/edwh_b2_plugin/__init__.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/src/edwh_b2_plugin/b2_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/src/edwh_b2_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/src/edwh_b2_plugin/__init__.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/src/edwh_b2_plugin/b2_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 edwh_b2_plugin-0.1.1/PKG-INFO
```

### Comparing `edwh_b2_plugin-0.1.0/src/edwh_b2_plugin/b2_plugin.py` & `edwh_b2_plugin-0.1.1/src/edwh_b2_plugin/b2_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_b2_plugin-0.1.0/LICENSE.txt` & `edwh_b2_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_b2_plugin-0.1.0/README.md` & `edwh_b2_plugin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_b2_plugin-0.1.0/pyproject.toml` & `edwh_b2_plugin-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 dev = [
     "hatch",
     # "python-semantic-release",
     "black",
 ]
 
 [project.urls]
-Documentation = "https://github.com/remcoboerma/edwh-b2-plugin#readme"
-Issues = "https://github.com/remcoboerma/edwh-b2-plugin/issues"
-Source = "https://github.com/remcoboerma/edwh-b2-plugin"
+Documentation = "https://github.com/educationwarehouse/edwh-b2-plugin#readme"
+Issues = "https://github.com/educationwarehouse/edwh-b2-plugin/issues"
+Source = "https://github.com/educationwarehouse/edwh-b2-plugin"
 
 # https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/#using-package-metadata
 [project.entry-points."edwh.tasks"]
 b2 = "edwh_b2_plugin.b2_plugin"
 
 [tool.hatch.version]
 path = "src/edwh_b2_plugin/__about__.py"
```

### Comparing `edwh_b2_plugin-0.1.0/PKG-INFO` & `edwh_b2_plugin-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: edwh-b2-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plugin for `edwh` with b2 functionality
-Project-URL: Documentation, https://github.com/remcoboerma/edwh-b2-plugin#readme
-Project-URL: Issues, https://github.com/remcoboerma/edwh-b2-plugin/issues
-Project-URL: Source, https://github.com/remcoboerma/edwh-b2-plugin
+Project-URL: Documentation, https://github.com/educationwarehouse/edwh-b2-plugin#readme
+Project-URL: Issues, https://github.com/educationwarehouse/edwh-b2-plugin/issues
+Project-URL: Source, https://github.com/educationwarehouse/edwh-b2-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

