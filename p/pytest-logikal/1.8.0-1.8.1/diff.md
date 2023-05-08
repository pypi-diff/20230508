# Comparing `tmp/pytest-logikal-1.8.0.tar.gz` & `tmp/pytest-logikal-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-logikal-1.8.0.tar", last modified: Fri May  5 11:07:40 2023, max compression
+gzip compressed data, was "pytest-logikal-1.8.1.tar", last modified: Mon May  8 20:10:03 2023, max compression
```

## Comparing `pytest-logikal-1.8.0.tar` & `pytest-logikal-1.8.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/compose.yml
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.669005 pytest-logikal-1.8.0/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.669005 pytest-logikal-1.8.0/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2890 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 20:10:03.611939 pytest-logikal-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-08 20:10:03.611939 pytest-logikal-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 20:10:03.607939 pytest-logikal-1.8.1/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 20:10:03.607939 pytest-logikal-1.8.1/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-08 20:10:03.000000 pytest-logikal-1.8.1/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-08 20:10:03.000000 pytest-logikal-1.8.1/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 20:10:03.000000 pytest-logikal-1.8.1/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-08 20:10:03.000000 pytest-logikal-1.8.1/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-08 20:10:03.000000 pytest-logikal-1.8.1/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-08 20:10:03.000000 pytest-logikal-1.8.1/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 20:10:03.607939 pytest-logikal-1.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 20:10:03.607939 pytest-logikal-1.8.1/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-08 20:09:34.000000 pytest-logikal-1.8.1/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 20:10:03.611939 pytest-logikal-1.8.1/setup.cfg
```

### Comparing `pytest-logikal-1.8.0/LICENSE.txt` & `pytest-logikal-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/PKG-INFO` & `pytest-logikal-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.0
+Version: 1.8.1
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.0/entry_points.ini` & `pytest-logikal-1.8.1/entry_points.ini`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pyproject.toml` & `pytest-logikal-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/bandit.py` & `pytest-logikal-1.8.1/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/browser.py` & `pytest-logikal-1.8.1/pytest_logikal/browser.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/build.py` & `pytest-logikal-1.8.1/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/core.py` & `pytest-logikal-1.8.1/pytest_logikal/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     'django': ['django', 'html', 'css', 'svg', 'js'],
 }
 DEFAULT_INI_OPTIONS: Dict[str, Any] = {
     'max_line_length': {'value': 99, 'help': 'the maximum line length to use'},
     'max_complexity': {'value': 10, 'help': 'the maximum complexity to allow'},
     'cov_fail_under': {'value': 100, 'help': 'target coverage percentage'},
 }
+EXTRAS = {
+    'browser': bool(find_spec('selenium')),
+    'django': bool(find_spec('pytest_django')),
+}
 
 ReportInfoType = Tuple[Union[os.PathLike, str], Optional[int], str]
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup('logikal')
     group.addoption('--live', action='store_true', help='run live tests')
@@ -44,30 +48,31 @@
     group.addoption('--no-build', action='store_true', help='do not run build checks')
     group.addoption('--no-docs', action='store_true', help='do not run documentation checks')
     group.addoption('--no-isort', action='store_true', help='do not use isort')
     group.addoption('--no-licenses', action='store_true', help='do not check licenses')
     group.addoption('--no-pylint', action='store_true', help='do not use pylint')
     group.addoption('--no-requirements', action='store_true', help='do not check requirements')
     group.addoption('--no-style', action='store_true', help='do not use pycodestyle & pydocstyle')
-    group.addoption('--no-django', action='store_true', help='do not run django migration checks')
-    group.addoption('--no-html', action='store_true', help='do not run html template checks')
-    group.addoption('--no-css', action='store_true', help='do not run css checks')
-    group.addoption('--no-svg', action='store_true', help='do not run svg checks')
-    group.addoption('--no-js', action='store_true', help='do not run js checks')
-    group.addoption('--no-install', action='store_true', help='do not install packages')
+    if EXTRAS['django']:
+        group.addoption('--no-django', action='store_true', help='do not run django checks')
+        group.addoption('--no-html', action='store_true', help='do not run html template checks')
+        group.addoption('--no-css', action='store_true', help='do not run css checks')
+        group.addoption('--no-svg', action='store_true', help='do not run svg checks')
+        group.addoption('--no-js', action='store_true', help='do not run js checks')
+        group.addoption('--no-install', action='store_true', help='do not install packages')
+
     for option, entry in DEFAULT_INI_OPTIONS.items():
         parser.addini(option, default=str(entry['value']), help=entry['help'])
 
 
 def pytest_addhooks(pluginmanager: pytest.PytestPluginManager) -> None:
-    if not find_spec('selenium'):
-        pluginmanager.set_blocked('logikal_browser')
-    if not find_spec('pytest_django'):
-        for plugin in PLUGINS['django']:
-            pluginmanager.set_blocked(f'logikal_{plugin}')
+    for extra, installed in EXTRAS.items():
+        if not installed:
+            for plugin in PLUGINS.get(extra, [extra]):
+                pluginmanager.set_blocked(f'logikal_{plugin}')
 
 
 # Untyped decorator (see https://github.com/pytest-dev/pytest/issues/7469)
 @pytest.hookimpl(hookwrapper=True)  # type: ignore[misc]
 def pytest_load_initial_conftests(early_config: pytest.Config, args: List[str]) -> Iterator[None]:
     if '--no-defaults' in args:
         yield
@@ -82,15 +87,15 @@
         args.append('--cache-clear')
         namespace.cacheclear = True
     if '-r' not in args:
         args.extend(['-r', 'fExX'])
     if '-n' not in args:
         args.extend(['-n', 'auto' if '--live' not in args else '0'])
         namespace.dist = 'load' if '--live' not in args else 'no'
-    for plugin in chain.from_iterable(PLUGINS.values()):
+    for plugin in chain(*(plugins for name, plugins in PLUGINS.items() if EXTRAS.get(name, True))):
         if '--fast' not in args and f'--no-{plugin}' not in args:
             args.append(f'--{plugin}')
             setattr(namespace, plugin, True)
     if all(arg not in args for arg in ['--cov', '--no-cov', '--live', '--fast']):
         args.extend(['--cov', '--no-cov-on-fail'])
         namespace.no_cov_on_fail = True
 
@@ -122,40 +127,38 @@
         print(colored('Installing Node.js packages', attrs=['bold']))
         command = ['npm', 'install', '--no-save', '--prefix', str(node_prefix)]
         subprocess.run(command, text=True, check=True)  # nosec: secure, not using untrusted input
 
 
 def pytest_configure(config: pytest.Config) -> None:
     # Installing Node.js packages
-    if find_spec('pytest_django') and not config.getoption('no_install'):
+    if EXTRAS['django'] and not config.getoption('no_install'):
         install_packages()
 
     # Clearing cache
     if config.getoption('clear'):
         print(colored('Clearing cache', 'yellow', attrs=['bold']))
         Path('.coverage').unlink(missing_ok=True)
         shutil.rmtree('.pytest_cache', ignore_errors=True)
         shutil.rmtree('.mypy_cache', ignore_errors=True)
 
-    # Hiding overly verbose debug and info log messages
+    # Hiding information
     if not config.getoption('verbose'):
+        # Hiding overly verbose debug and info log messages
+        logging.getLogger('django_migration_linter').setLevel(logging.WARNING)
+        logging.getLogger('docker').setLevel(logging.INFO)
         logging.getLogger('faker').setLevel(logging.INFO)
         logging.getLogger('filelock').setLevel(logging.WARNING)
+        logging.getLogger('matplotlib').setLevel(logging.INFO)
         logging.getLogger('PIL').setLevel(logging.INFO)
         logging.getLogger('pydocstyle').setLevel(logging.WARNING)
-        logging.getLogger('matplotlib').setLevel(logging.INFO)
-        logging.getLogger('django_migration_linter').setLevel(logging.WARNING)
-
-        # Hiding validator log messages
-        logging.getLogger('docker').setLevel(logging.INFO)
-        logging.getLogger('urllib3').setLevel(logging.INFO)
         logging.getLogger('pytest_logikal.validator').setLevel(logging.INFO)
+        logging.getLogger('urllib3').setLevel(logging.INFO)
 
-    # Hiding worker information lines
-    if not config.getoption('verbose'):
+        # Hiding worker information lines
         config.pluginmanager.get_plugin('reports').getworkerinfoline = lambda *_args, **_kwargs: ''
 
     # Configuring mypy
     mypy = config.pluginmanager.get_plugin('mypy')
     mypy.mypy_argv = [
         '--no-error-summary',
         '--strict',
```

### Comparing `pytest-logikal-1.8.0/pytest_logikal/css.py` & `pytest-logikal-1.8.1/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/css_config.yml` & `pytest-logikal-1.8.1/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/django.py` & `pytest-logikal-1.8.1/pytest_logikal/django.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/docker.py` & `pytest-logikal-1.8.1/pytest_logikal/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/docs.py` & `pytest-logikal-1.8.1/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/file_checker.py` & `pytest-logikal-1.8.1/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/html.py` & `pytest-logikal-1.8.1/pytest_logikal/html.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/isort.py` & `pytest-logikal-1.8.1/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/js.py` & `pytest-logikal-1.8.1/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/js_config.yml` & `pytest-logikal-1.8.1/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/licenses.py` & `pytest-logikal-1.8.1/pytest_logikal/licenses.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/package-lock.json` & `pytest-logikal-1.8.1/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/plugin.py` & `pytest-logikal-1.8.1/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/pylint.py` & `pytest-logikal-1.8.1/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/requirements.py` & `pytest-logikal-1.8.1/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/style.py` & `pytest-logikal-1.8.1/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/svg.py` & `pytest-logikal-1.8.1/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/utils.py` & `pytest-logikal-1.8.1/pytest_logikal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal/validator.py` & `pytest-logikal-1.8.1/pytest_logikal/validator.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal.egg-info/PKG-INFO` & `pytest-logikal-1.8.1/pytest_logikal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.0
+Version: 1.8.1
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.0/pytest_logikal.egg-info/SOURCES.txt` & `pytest-logikal-1.8.1/pytest_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal.egg-info/entry_points.txt` & `pytest-logikal-1.8.1/pytest_logikal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/pytest_logikal.egg-info/requires.txt` & `pytest-logikal-1.8.1/pytest_logikal.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 bandit==1.7.5
 coverage[toml]==7.2.5
 isort[colors]==5.12.0
 mypy==1.2.0
-pip-licenses==4.3.0
+pip-licenses==4.3.1
 pycodestyle==2.10.0
 pydocstyle[toml]==6.3.0
-pylint==2.17.3
+pylint==2.17.4
 pytest==7.3.1
 pytest-cov==4.0.0
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
 pytest-xdist[psutil]==3.2.1
 Pillow~=9.4
 Pygments~=2.15
+docker~=6.1
 pyorbs~=2.0
 termcolor~=2.3
 tomli~=2.0
 
 [browser]
-selenium==4.9.0
+selenium==4.9.1
 
 [django]
 Django~=4.2
 django-stubs~=4.2
 django-migration-linter~=4.1
-djlint==1.25.0
+djlint==1.25.1
 pylint-django==2.5.3
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
-docker~=6.0
 requests~=2.28
 types-requests~=2.28
```

### Comparing `pytest-logikal-1.8.0/requirements/build.txt.lock` & `pytest-logikal-1.8.1/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.0/requirements/dev.txt.lock` & `pytest-logikal-1.8.1/requirements/dev.txt.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 123e0923c12ca1679b00a6caddf9ddb565dc2ff87aef5e10a2dd2bcb172f2024
+##  Requirements hash: 2134406769d7050fa4ae6847b899158b56f34fa84fc3e5ecc4643794e28391da
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.6.0
 astroid==2.15.4
 async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 bleach==6.0.0
 build==0.10.0
-certifi==2022.12.7
+certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.5
 cryptography==40.0.2
 cssbeautifier==1.14.7
 dill==0.3.6
 Django==4.2.1
 django-migration-linter==4.1.0
 django-stubs==4.2.0
 django-stubs-ext==4.2.0
-djlint==1.25.0
-docker==6.0.1
+djlint==1.25.1
+docker==6.1.1
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
-Faker==18.6.2
+Faker==18.7.0
 filelock==3.12.0
 gitdb==4.0.10
 GitPython==3.1.31
 h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 idna==3.4
@@ -52,14 +52,15 @@
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
 jaraco.classes==3.2.3
 jeepney==0.8.0
 Jinja2==3.1.2
 jsbeautifier==1.14.7
+json5==0.9.11
 keyring==23.13.1
 lazy-object-proxy==1.9.0
 logikal-docs==1.1.3
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mccabe==0.7.0
 mdurl==0.1.2
@@ -68,25 +69,25 @@
 mypy-extensions==1.0.0
 outcome==1.2.0
 packaging==23.1
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
-pip-licenses==4.3.0
+pip-licenses==4.3.1
 pkginfo==1.9.6
 platformdirs==3.5.0
 pluggy==1.0.0
 prettytable==3.7.0
 psutil==5.9.5
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 Pygments==2.15.1
-pylint==2.17.3
+pylint==2.17.4
 pylint-django==2.5.3
 pylint-plugin-utils==0.7
 pyorbs==2.0.0
 pyproject_hooks==1.0.0
 PySocks==1.7.1
 pytest==7.3.1
 pytest-cov==4.0.0
@@ -101,15 +102,15 @@
 readme-renderer==37.3
 regex==2023.5.5
 requests==2.30.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.3.5
 SecretStorage==3.3.3
-selenium==4.9.0
+selenium==4.9.1
 setuptools==67.7.2
 six==1.16.0
 smmap==5.0.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==5.3.0
@@ -128,18 +129,18 @@
 tomlkit==0.11.8
 tqdm==4.65.0
 trio==0.22.0
 trio-websocket==0.10.2
 twine==4.0.2
 types-pytz==2023.3.0.0
 types-PyYAML==6.0.12.9
-types-requests==2.29.0.0
+types-requests==2.30.0.0
 types-urllib3==1.26.25.12
 typing_extensions==4.5.0
-urllib3==1.26.15
+urllib3==2.0.2
 wcwidth==0.2.6
 webencodings==0.5.1
 websocket-client==1.5.1
 wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
 zipp==3.15.0
```

### Comparing `pytest-logikal-1.8.0/requirements/docs.txt.lock` & `pytest-logikal-1.8.1/requirements/docs.txt.lock`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,128 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: bec45cef2a84abf1e23a4c575600549fc6d8ff56c4bf8627cf1c3dd1a58a25f9
+##  Requirements hash: 0e866b1bea523e49e31423bce6ea72139b00106fcba40e86d373d7074e56c7ba
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
+appdirs==1.4.4
+asgiref==3.6.0
 astroid==2.15.4
 async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
+backports.zoneinfo==0.2.1
 bandit==1.7.5
-certifi==2022.12.7
+certifi==2023.5.7
 charset-normalizer==3.1.0
+click==8.1.3
 colorama==0.4.6
 coverage==7.2.5
+cssbeautifier==1.14.7
 dill==0.3.6
+Django==4.2.1
+django-migration-linter==4.1.0
+django-stubs==4.2.0
+django-stubs-ext==4.2.0
+djlint==1.25.1
+docker==6.1.1
 docutils==0.17.1
+EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
+factory-boy==3.2.1
+Faker==18.7.0
 filelock==3.12.0
 gitdb==4.0.10
 GitPython==3.1.31
 h11==0.14.0
+html-tag-names==0.1.2
+html-void-elements==0.1.0
 idna==3.4
 imagesize==1.4.1
 importlib-metadata==6.6.0
+inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
 Jinja2==3.1.2
+jsbeautifier==1.14.7
+json5==0.9.11
 lazy-object-proxy==1.9.0
 logikal-docs==1.1.3
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mccabe==0.7.0
 mdurl==0.1.2
 mypy==1.2.0
 mypy-extensions==1.0.0
 outcome==1.2.0
 packaging==23.1
+pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
-pip-licenses==4.3.0
+pip-licenses==4.3.1
 platformdirs==3.5.0
 pluggy==1.0.0
 prettytable==3.7.0
 psutil==5.9.5
 pycodestyle==2.10.0
 pydocstyle==6.3.0
 Pygments==2.15.1
-pylint==2.17.3
+pylint==2.17.4
+pylint-django==2.5.3
+pylint-plugin-utils==0.7
 pyorbs==2.0.0
 PySocks==1.7.1
 pytest==7.3.1
 pytest-cov==4.0.0
+pytest-django==4.5.2
+pytest-factoryboy==2.5.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
 pytest-xdist==3.2.1
+python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
+regex==2023.5.5
 requests==2.30.0
 rich==13.3.5
-selenium==4.9.0
+selenium==4.9.1
 setuptools==67.7.2
+six==1.16.0
 smmap==5.0.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
+sqlparse==0.4.4
 stevedore==5.0.0
 termcolor==2.3.0
+toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.8
+tqdm==4.65.0
 trio==0.22.0
 trio-websocket==0.10.2
+types-pytz==2023.3.0.0
+types-PyYAML==6.0.12.9
+types-requests==2.30.0.0
+types-urllib3==1.26.25.12
 typing_extensions==4.5.0
-urllib3==1.26.15
+urllib3==2.0.2
 wcwidth==0.2.6
+websocket-client==1.5.1
 wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
 zipp==3.15.0
```

