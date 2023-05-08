# Comparing `tmp/SqlAlchemy_Tools-0.1.1b0.tar.gz` & `tmp/SqlAlchemy_Tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SqlAlchemy_Tools-0.1.1b0.tar", last modified: Sat Feb 13 22:55:58 2021, max compression
+gzip compressed data, was "SqlAlchemy_Tools-0.2.0.tar", last modified: Mon May  8 10:10:57 2023, max compression
```

## Comparing `SqlAlchemy_Tools-0.1.1b0.tar` & `SqlAlchemy_Tools-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.116411 SqlAlchemy_Tools-0.1.1b0/
--rw-rw-rw-   0        0        0     1082 2021-02-13 22:00:59.000000 SqlAlchemy_Tools-0.1.1b0/LICENSE
--rw-rw-rw-   0        0        0       62 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/MANIFEST.in
--rw-rw-rw-   0        0        0     9974 2021-02-13 22:55:58.113413 SqlAlchemy_Tools-0.1.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     7375 2021-02-13 22:41:36.000000 SqlAlchemy_Tools-0.1.1b0/README.md
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.027463 SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/
--rw-rw-rw-   0        0        0     9974 2021-02-13 22:55:57.000000 SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2021-02-13 22:55:57.000000 SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-13 22:55:57.000000 SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2021-02-13 22:55:57.000000 SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2021-02-13 22:55:57.000000 SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-02-13 22:55:58.119409 SqlAlchemy_Tools-0.1.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1364 2021-02-13 22:55:37.000000 SqlAlchemy_Tools-0.1.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.044454 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/
--rw-rw-rw-   0        0        0      206 2021-02-13 22:55:37.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.077433 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/
--rw-rw-rw-   0        0        0       89 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/__init__.py
--rw-rw-rw-   0        0        0     5415 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/model.py
--rw-rw-rw-   0        0        0     1697 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/query.py
--rw-rw-rw-   0        0        0     2029 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/repr.py
--rw-rw-rw-   0        0        0     8223 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/database.py
--rw-rw-rw-   0        0        0      348 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/forms.py
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.081431 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/
--rw-rw-rw-   0        0        0    20101 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:57.979490 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.094424 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/
--rw-rw-rw-   0        0        0       38 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/README
--rw-rw-rw-   0        0        0      815 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/alembic.ini.mako
--rw-rw-rw-   0        0        0     3030 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/env.py
--rw-rw-rw-   0        0        0      518 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/script.py.mako
--rw-rw-rw-   0        0        0       47 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/mixins.py
-drwxrwxrwx   0        0        0        0 2021-02-13 22:55:58.105417 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/pagination/
--rw-rw-rw-   0        0        0       34 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/pagination/__init__.py
--rw-rw-rw-   0        0        0     4947 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/pagination/paginator.py
--rw-rw-rw-   0        0        0      634 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/pagination/test_paginator.py
--rw-rw-rw-   0        0        0      715 2021-02-13 22:01:25.000000 SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:57.147608 SqlAlchemy_Tools-0.2.0/
+-rw-rw-rw-   0        0        0     1082 2021-02-13 22:00:59.000000 SqlAlchemy_Tools-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       62 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7905 2023-05-08 10:10:57.139603 SqlAlchemy_Tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7375 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:56.961606 SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/
+-rw-rw-rw-   0        0        0     7905 2023-05-08 10:10:56.000000 SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-05-08 10:10:56.000000 SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:10:56.000000 SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      290 2023-05-08 10:10:56.000000 SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 10:10:56.000000 SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:10:57.147608 SqlAlchemy_Tools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-05-08 10:09:53.000000 SqlAlchemy_Tools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:56.992604 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/
+-rw-rw-rw-   0        0        0      203 2023-05-08 10:09:53.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:57.039603 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/
+-rw-rw-rw-   0        0        0       89 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/__init__.py
+-rw-rw-rw-   0        0        0     5415 2023-05-07 12:59:59.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/model.py
+-rw-rw-rw-   0        0        0     1697 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/query.py
+-rw-rw-rw-   0        0        0     2029 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/repr.py
+-rw-rw-rw-   0        0        0     8223 2023-05-07 12:59:59.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/database.py
+-rw-rw-rw-   0        0        0      348 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:57.053601 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/
+-rw-rw-rw-   0        0        0    20102 2023-05-08 09:57:15.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:57.079606 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/manager/
+-rw-rw-rw-   0        0        0    14579 2023-05-08 09:57:35.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/manager/__init__.py
+-rw-rw-rw-   0        0        0    14792 2023-05-07 10:57:51.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/manager/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:56.893604 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:57.110604 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/
+-rw-rw-rw-   0        0        0       38 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/README
+-rw-rw-rw-   0        0        0      815 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/alembic.ini.mako
+-rw-rw-rw-   0        0        0     3030 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/env.py
+-rw-rw-rw-   0        0        0      518 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/script.py.mako
+-rw-rw-rw-   0        0        0       47 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/mixins.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:10:57.132599 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/pagination/
+-rw-rw-rw-   0        0        0       34 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/pagination/__init__.py
+-rw-rw-rw-   0        0        0     4947 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/pagination/paginator.py
+-rw-rw-rw-   0        0        0      634 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/pagination/test_paginator.py
+-rw-rw-rw-   0        0        0      715 2021-02-13 22:59:19.000000 SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/validator.py
```

### Comparing `SqlAlchemy_Tools-0.1.1b0/LICENSE` & `SqlAlchemy_Tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/README.md` & `SqlAlchemy_Tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/SqlAlchemy_Tools.egg-info/SOURCES.txt` & `SqlAlchemy_Tools-0.2.0/SqlAlchemy_Tools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 sqlalchemy_tools/mixins.py
 sqlalchemy_tools/validator.py
 sqlalchemy_tools/base/__init__.py
 sqlalchemy_tools/base/model.py
 sqlalchemy_tools/base/query.py
 sqlalchemy_tools/base/repr.py
 sqlalchemy_tools/migration/__init__.py
+sqlalchemy_tools/migration/manager/__init__.py
+sqlalchemy_tools/migration/manager/cli.py
 sqlalchemy_tools/migration/templates/default/README
 sqlalchemy_tools/migration/templates/default/alembic.ini.mako
 sqlalchemy_tools/migration/templates/default/env.py
 sqlalchemy_tools/migration/templates/default/script.py.mako
 sqlalchemy_tools/pagination/__init__.py
 sqlalchemy_tools/pagination/paginator.py
 sqlalchemy_tools/pagination/test_paginator.py
```

### Comparing `SqlAlchemy_Tools-0.1.1b0/setup.py` & `SqlAlchemy_Tools-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="SqlAlchemy_Tools",
-    version="0.1.1-b0",
+    version="0.2.0",
     packages=find_packages(),
     include_package_data=True,
 
     install_requires=[
         "alembic>=1.5.4",
         "arrow>=0.17.0",
         "flask-wtf>=0.14.3",
@@ -21,16 +21,16 @@
         "inflection>=0.5.1",
         "graphviz>=0.16",
         "manage.py>=0.2.10",
         "pandas>=1.2.2",
         "pymysql>=1.0.2",
         "pg8000>=1.17.0",
         "sadisplay>=0.4.9",
-        "sqlalchemy>=1.3.23",
-        "sqlalchemy-mixins>=1.2.1",
+        "sqlalchemy>=1.3.23,<=1.4.48",
+        "sqlalchemy-mixins>=1.2.1,<=1.5.3",
         "sqlalchemy-repr>=0.0.2",
         "wtforms_alchemy>=0.17.0",
     ],
 
     author="Andy Everitt",
     author_email="andreweveritt@e3d-online.com",
     description="SqlAlchemyTools provides similar functionality to Flask-SqlAlchemy & Flask-Migrate without being dependant on Flask.",
```

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/model.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/model.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/query.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/query.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/base/repr.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/base/repr.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/database.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/database.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/__init__.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import graphviz
 import sadisplay.reflect
 from alembic import __version__ as __alembic_version__
 from alembic import command
 from alembic.config import Config as AlembicConfig
 from alembic.util import CommandError
 from flask import current_app
-from manager import Manager
+from .manager import Manager
 
 alembic_version = tuple([int(v) for v in __alembic_version__.split('.')[0:3]])
 log = logging.getLogger(__name__)
 
 
 class _MigrateConfig(object):
     def __init__(self, migrate, db, **kwargs):
```

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/alembic.ini.mako` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/env.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/migration/templates/default/script.py.mako` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/migration/templates/default/script.py.mako`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/pagination/paginator.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/pagination/test_paginator.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/pagination/test_paginator.py`

 * *Files identical despite different names*

### Comparing `SqlAlchemy_Tools-0.1.1b0/sqlalchemy_tools/validator.py` & `SqlAlchemy_Tools-0.2.0/sqlalchemy_tools/validator.py`

 * *Files identical despite different names*

