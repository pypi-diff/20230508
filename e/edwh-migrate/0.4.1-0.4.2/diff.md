# Comparing `tmp/edwh_migrate-0.4.1.tar.gz` & `tmp/edwh_migrate-0.4.2.tar.gz`

## Comparing `edwh_migrate-0.4.1.tar` & `edwh_migrate-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,16 @@
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/migrations.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/.gitignore
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/dataSources.xml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/migrate.iml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/vcs.xml
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/workspace.xml
--rw-r--r--   0        0        0    47176 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/dataSources/21da014d-6e3f-42ea-8c44-aedba5c52d26.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/tests/test_basics.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/tests/sqlite_empty/empty_sqlite.db
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/tests/sqlite_empty/just_implemented_features.db
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/tests/sqlite_empty/just_implemented_features.sql
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/README.md
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 edwh_migrate-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/migrations.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/requirements.txt
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/test_basics.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/README.md
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.4.2/PKG-INFO
```

### Comparing `edwh_migrate-0.4.1/CHANGELOG.md` & `edwh_migrate-0.4.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.2 (2023-05-04)
+### Documentation
+* **migrate:** Changed package name from '-' to edwh-migrate and added extra's dev dependencies ([`ae3eef6`](https://github.com/educationwarehouse/migrate/commit/ae3eef6a1e2db47d03fcd60a57d768d79b7f4a32))
+
 ## v0.4.1 (2023-05-04)
 ### Fix
 * Better troubleshooting support for the sys.argv[1] argument ([`8a21505`](https://github.com/educationwarehouse/migrate/commit/8a21505307618a45d993b772f1ea40e0c4b3343f))
 
 ## v0.4.0 (2023-05-04)
 ### Feature
 * Support for argv[1] as a path to a python file, or to the folder where `migrations.py` is stored. ([`7d0aba6`](https://github.com/educationwarehouse/migrate/commit/7d0aba641907ca4100a10a3fba67e3286ab8f5c6))
```

### Comparing `edwh_migrate-0.4.1/migrations.py` & `edwh_migrate-0.4.2/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/requirements.txt` & `edwh_migrate-0.4.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/src/edwh_migrate/__init__.py` & `edwh_migrate-0.4.2/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/src/edwh_migrate/migrate.py` & `edwh_migrate-0.4.2/src/edwh_migrate/migrate.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/tests/test_basics.py` & `edwh_migrate-0.4.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/tests/sqlite_empty/empty_sqlite.db` & `edwh_migrate-0.4.2/tests/sqlite_empty/empty_sqlite.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/tests/sqlite_empty/just_implemented_features.db` & `edwh_migrate-0.4.2/tests/sqlite_empty/just_implemented_features.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/.gitignore` & `edwh_migrate-0.4.2/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -153,8 +153,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
```

### Comparing `edwh_migrate-0.4.1/LICENSE.txt` & `edwh_migrate-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.1/README.md` & `edwh_migrate-0.4.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Educationwarehouse's Migrate
 
-[![PyPI - Version](https://img.shields.io/pypi/v/-.svg)](https://pypi.org/project/-)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/-.svg)](https://pypi.org/project/-)
+[![PyPI - Version](https://img.shields.io/pypi/v/edwh-migrate.svg)](https://pypi.org/project/edwh-migrate)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-migrate.svg)](https://pypi.org/project/edwh-migrate)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Documentation](#documentation)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install edwh-migrate
 ```
@@ -25,8 +26,8 @@
 * `MIGRATE_CAT_COMMAND`: for unsupported compression formats, this command decompresses the file and produces sql on the stdout. 
 * `SCHEMA_VERSION`: Used in case of schema versioning. Set by another process.
 * `REDIS_HOST`: If set, all keys of the redis database 0 will be removed. 
 
 
 ## License
 
-`-` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`edwh-migrate` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `edwh_migrate-0.4.1/pyproject.toml` & `edwh_migrate-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,29 @@
 ]
 dependencies = [
   "pydal>=20221110.1",
   'plumbum',
   'psycopg2-binary',
   'redis',
 ]
+
+[project.optional-dependencies]
+dev = [
+    "hatch",
+    "python-semantic-release",
+    "black",
+]
+
 [project.scripts]
 migrate = "edwh_migrate.migrate:console_hook"
 
 [project.urls]
-Documentation = "https://github.com/unknown/-#readme"
-Issues = "https://github.com/unknown/-/issues"
-Source = "https://github.com/unknown/-"
+Documentation = "https://github.com/educationwarehouse/migrate#readme"
+Issues = "https://github.com/educationwarehouse/migrate/issues"
+Source = "https://github.com/educationwarehouse/migrate"
 
 [tool.semantic_release]
 branch = "main"
 version_variable = "src/edwh_migrate/__about__.py:__version__"
 change_log = "CHANGELOG.md"
 upload_to_repository = false
 upload_to_release = false
```

### Comparing `edwh_migrate-0.4.1/PKG-INFO` & `edwh_migrate-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: edwh-migrate
-Version: 0.4.1
+Version: 0.4.2
 Summary: Helps migrating database schema changes using pydal. 
-Project-URL: Documentation, https://github.com/unknown/-#readme
-Project-URL: Issues, https://github.com/unknown/-/issues
-Project-URL: Source, https://github.com/unknown/-
+Project-URL: Documentation, https://github.com/educationwarehouse/migrate#readme
+Project-URL: Issues, https://github.com/educationwarehouse/migrate/issues
+Project-URL: Source, https://github.com/educationwarehouse/migrate
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: database-migration,migrate,postgresql,pydal,schema-change
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
@@ -16,26 +16,31 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: plumbum
 Requires-Dist: psycopg2-binary
 Requires-Dist: pydal>=20221110.1
 Requires-Dist: redis
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: python-semantic-release; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Educationwarehouse's Migrate
 
-[![PyPI - Version](https://img.shields.io/pypi/v/-.svg)](https://pypi.org/project/-)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/-.svg)](https://pypi.org/project/-)
+[![PyPI - Version](https://img.shields.io/pypi/v/edwh-migrate.svg)](https://pypi.org/project/edwh-migrate)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-migrate.svg)](https://pypi.org/project/edwh-migrate)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Documentation](#documentation)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install edwh-migrate
 ```
@@ -49,8 +54,8 @@
 * `MIGRATE_CAT_COMMAND`: for unsupported compression formats, this command decompresses the file and produces sql on the stdout. 
 * `SCHEMA_VERSION`: Used in case of schema versioning. Set by another process.
 * `REDIS_HOST`: If set, all keys of the redis database 0 will be removed. 
 
 
 ## License
 
-`-` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`edwh-migrate` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

