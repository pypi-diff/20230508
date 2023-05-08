# Comparing `tmp/pydumpck-1.6.168.tar.gz` & `tmp/pydumpck-1.7.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydumpck-1.6.168.tar", last modified: Sun May 29 07:48:44 2022, max compression
+gzip compressed data, was "pydumpck-1.7.62.tar", last modified: Wed Jun  8 11:38:16 2022, max compression
```

## Comparing `pydumpck-1.6.168.tar` & `pydumpck-1.7.62.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-29 07:48:30.000000 pydumpck-1.6.168/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6763 2022-05-29 07:48:44.166589 pydumpck-1.6.168/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-05-29 07:48:30.000000 pydumpck-1.6.168/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7837 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/archive_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/configuration/res_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/py_common_dump/
--rw-r--r--   0 runner    (1001) docker     (121)     6669 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/py_common_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/py_package/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/py_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/py_package/package_description/
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/py_package/package_description/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/py_package/package_struct/
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/py_package/package_struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/pyc_checker/
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/build.py
--rw-r--r--   0 runner    (1001) docker     (121)   216576 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/pycdc.exe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/src/
--rw-r--r--   0 runner    (1001) docker     (121)  1305342 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/src/pycdc.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/pyc_checker/lib_uncompyle6/
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/lib_uncompyle6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/lib_uncompyle6/requirement_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    15143 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/py_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/OpCode/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/OpCode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/OpCode/py3.10.4.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/magic_code/
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/pyc/magic_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3273 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyc_checker/pyz_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/pyinstaller_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/utils/banner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.166589 pydumpck-1.6.168/pydumpck/utils/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/utils/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-29 07:48:30.000000 pydumpck-1.6.168/pydumpck/utils/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 07:48:44.162589 pydumpck-1.6.168/pydumpck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6763 2022-05-29 07:48:43.000000 pydumpck-1.6.168/pydumpck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-05-29 07:48:44.000000 pydumpck-1.6.168/pydumpck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 07:48:43.000000 pydumpck-1.6.168/pydumpck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-29 07:48:43.000000 pydumpck-1.6.168/pydumpck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 07:48:43.000000 pydumpck-1.6.168/pydumpck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-29 07:48:44.000000 pydumpck-1.6.168/pydumpck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-29 07:48:44.000000 pydumpck-1.6.168/pydumpck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-05-29 07:48:30.000000 pydumpck-1.6.168/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 07:48:44.166589 pydumpck-1.6.168/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-05-29 07:48:30.000000 pydumpck-1.6.168/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.898833 pydumpck-1.7.62/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-06-08 11:38:00.000000 pydumpck-1.7.62/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6894 2022-06-08 11:38:16.898833 pydumpck-1.7.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5505 2022-06-08 11:38:00.000000 pydumpck-1.7.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.890833 pydumpck-1.7.62/pydumpck/
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7867 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/archive_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.890833 pydumpck-1.7.62/pydumpck/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/configuration/res_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/py_common_dump/
+-rw-r--r--   0 runner    (1001) docker     (121)     6718 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/py_common_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/py_package/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/py_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/py_package/package_description/
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/py_package/package_description/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/py_package/package_struct/
+-rw-r--r--   0 runner    (1001) docker     (121)     5383 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/py_package/package_struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/
+-rw-r--r--   0 runner    (1001) docker     (121)     4649 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)   216576 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/pycdc.exe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/src/
+-rw-r--r--   0 runner    (1001) docker     (121)  1305342 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/src/pycdc.zip
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/lib_uncompyle6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/lib_uncompyle6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/lib_uncompyle6/requirement_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15159 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/py_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/OpCode/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/OpCode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/OpCode/py3.10.4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.894833 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/magic_code/
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/pyc/magic_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyc_checker/pyz_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/pyinstaller_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.898833 pydumpck-1.7.62/pydumpck/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/utils/banner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.898833 pydumpck-1.7.62/pydumpck/utils/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/utils/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-08 11:38:00.000000 pydumpck-1.7.62/pydumpck/utils/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 11:38:16.890833 pydumpck-1.7.62/pydumpck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6894 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-08 11:38:16.000000 pydumpck-1.7.62/pydumpck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-08 11:38:00.000000 pydumpck-1.7.62/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 11:38:16.898833 pydumpck-1.7.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-06-08 11:38:00.000000 pydumpck-1.7.62/setup.py
```

### Comparing `pydumpck-1.6.168/PKG-INFO` & `pydumpck-1.7.62/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydumpck
-Version: 1.6.168
+Version: 1.7.62
 Summary: pydumpck is a multi-threads tool for decompile exe,elf,pyz,pyc packed by python which is base on pycdc and uncompyle6.sometimes its py-file result not exactly right ,maybe could use uncompyle6.
 Home-page: https://github.com/serfend/pydumpck
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: pydumpck,decomplier,pe,elf,pyc,pyz
 Platform: any
@@ -139,7 +139,13 @@
 ## Notice
 
 > `pycdc` speed is more than 10 times faster than `uncompyle6` , and `uncompyle6` is not support for python that version above 3.8.
 >
 > however `pycdc` sometimes return a not precisely right result.
 >
 > in pydumpck , you can use `--plugin uncompyle6` for single-use or `--plugin pycdc uncompyle6` for both-use.
+
+
+
+## Status
+
+![Alt](https://repobeats.axiom.co/api/embed/013759c6315338178a2643de0bca01826fb39a14.svg "Repobeats analytics image")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydumpck Version: 1.6.168 Summary: pydumpck is a
+Metadata-Version: 2.1 Name: pydumpck Version: 1.7.62 Summary: pydumpck is a
 multi-threads tool for decompile exe,elf,pyz,pyc packed by python which is base
 on pycdc and uncompyle6.sometimes its py-file result not exactly right ,maybe
 could use uncompyle6. Home-page: https://github.com/serfend/pydumpck Author:
 serfend Author-email: serfend@foxmail.com License: MIT Licence Keywords:
 pydumpck,decomplier,pe,elf,pyc,pyz Platform: any Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
@@ -64,8 +64,10 @@
 lib_base64 secert` for targets `main.py` and `lib_base64.py` and `secert.py` ##
 Demo - pyc with header been tampered with - (Warning:gif with size 5MB)![pyc-
 fix_header-demo](https://raw.githubusercontent.com/serfend/res.image.reference/
 main/pyc-fix_header-demo.gif) ## Notice > `pycdc` speed is more than 10 times
 faster than `uncompyle6` , and `uncompyle6` is not support for python that
 version above 3.8. > > however `pycdc` sometimes return a not precisely right
 result. > > in pydumpck , you can use `--plugin uncompyle6` for single-use or
-`--plugin pycdc uncompyle6` for both-use.
+`--plugin pycdc uncompyle6` for both-use. ## Status ![Alt](https://
+repobeats.axiom.co/api/embed/013759c6315338178a2643de0bca01826fb39a14.svg
+"Repobeats analytics image")
```

### Comparing `pydumpck-1.6.168/README.md` & `pydumpck-1.7.62/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,7 +109,13 @@
 ## Notice
 
 > `pycdc` speed is more than 10 times faster than `uncompyle6` , and `uncompyle6` is not support for python that version above 3.8.
 >
 > however `pycdc` sometimes return a not precisely right result.
 >
 > in pydumpck , you can use `--plugin uncompyle6` for single-use or `--plugin pycdc uncompyle6` for both-use.
+
+
+
+## Status
+
+![Alt](https://repobeats.axiom.co/api/embed/013759c6315338178a2643de0bca01826fb39a14.svg "Repobeats analytics image")
```

#### html2text {}

```diff
@@ -46,8 +46,10 @@
 lib_base64 secert` for targets `main.py` and `lib_base64.py` and `secert.py` ##
 Demo - pyc with header been tampered with - (Warning:gif with size 5MB)![pyc-
 fix_header-demo](https://raw.githubusercontent.com/serfend/res.image.reference/
 main/pyc-fix_header-demo.gif) ## Notice > `pycdc` speed is more than 10 times
 faster than `uncompyle6` , and `uncompyle6` is not support for python that
 version above 3.8. > > however `pycdc` sometimes return a not precisely right
 result. > > in pydumpck , you can use `--plugin uncompyle6` for single-use or
-`--plugin pycdc uncompyle6` for both-use.
+`--plugin pycdc uncompyle6` for both-use. ## Status ![Alt](https://
+repobeats.axiom.co/api/embed/013759c6315338178a2643de0bca01826fb39a14.svg
+"Repobeats analytics image")
```

### Comparing `pydumpck-1.6.168/pydumpck/__init__.py` & `pydumpck-1.7.62/pydumpck/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 want that, trust us) you should upgrade to python 3. It's like getting your
 vaccinations. It hurts a little bit initially but in the end it's worth it.
 
 For more information, see here: https://github.com/serfend/pydumpck
 
 Good luck!
 """)
-
+from sgtpyutils.logger import logger
 import sys
 import os
 src_path = os.path.realpath(__file__)
 src_dir = os.path.dirname(src_path)
 sys.path.append(src_dir)
 from pydumpck.pyinstaller_dump import run
```

### Comparing `pydumpck-1.6.168/pydumpck/archive_viewer.py` & `pydumpck-1.7.62/pydumpck/archive_viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-#-----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
 # Copyright (c) 2013-2022, PyInstaller Development Team.
 #
 # Distributed under the terms of the GNU General Public License (version 2
 # or later) with exception for distributing the bootloader.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 #
 # SPDX-License-Identifier: (GPL-2.0-or-later WITH Bootloader-exception)
-#-----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
 """
 Viewer for archives packaged by archive.py.
 """
 
+from . import logger
 import argparse
 import os
 import pprint
 import sys
 import tempfile
 import zlib
 
@@ -27,31 +28,29 @@
 cleanup = []
 
 
 def main(name, brief, debug, rec_debug, **unused_options):
     global stack
 
     if not os.path.isfile(name):
-        print(name, "is an invalid file name!", file=sys.stderr)
+        logger.error(f'[{name}] is an invalid file name!')
         return 1
 
     arch = get_archive(name)
     stack.append((name, arch))
     if debug or brief:
         show_log(arch, rec_debug, brief)
         raise SystemExit(0)
     else:
         show(name, arch)
 
     while 1:
         try:
             toks = stdin_input('? ').split(None, 1)
         except EOFError:
-            # Ctrl-D
-            print(file=sys.stderr)  # Clear line.
             break
         if not toks:
             usage()
             continue
         if len(toks) == 1:
             cmd = toks[0]
             arg = ''
@@ -67,32 +66,32 @@
         elif cmd == 'O':
             if not arg:
                 arg = stdin_input('open name? ')
             arg = arg.strip()
             try:
                 arch = get_archive(arg)
             except NotAnArchiveError as e:
-                print(e, file=sys.stderr)
+                logger.error(e)
                 continue
             if arch is None:
-                print(arg, "not found", file=sys.stderr)
+                logger.error(f"{arg} not found")
                 continue
             stack.append((arg, arch))
             show(arg, arch)
         elif cmd == 'X':
             if not arg:
                 arg = stdin_input('extract name? ')
             arg = arg.strip()
             data = get_data(arg, arch)
             if data is None:
-                print("Not found", file=sys.stderr)
+                logger.error("Not found")
                 continue
             filename = stdin_input('to filename? ')
             if not filename:
-                print(repr(data))
+                logger.error(repr(data))
             else:
                 with open(filename, 'wb') as fp:
                     fp.write(data)
         elif cmd == 'Q':
             break
         else:
             usage()
@@ -102,23 +101,23 @@
 def do_cleanup():
     global stack, cleanup
     stack = []
     for filename in cleanup:
         try:
             os.remove(filename)
         except Exception as e:
-            print("could not delete", filename, e.args, file=sys.stderr)
+            logger.error(f"could not delete {filename} , {e.args}")
     cleanup = []
 
 
 def usage():
-    print("U: go up one level", file=sys.stderr)
-    print("O <name>: open embedded archive name", file=sys.stderr)
-    print("X <name>: extract name", file=sys.stderr)
-    print("Q: quit", file=sys.stderr)
+    logger.debug("U: go up one level")
+    logger.debug("O <name>: open embedded archive name")
+    logger.debug("X <name>: extract name")
+    logger.debug("Q: quit")
 
 
 def get_archive(name):
     if not stack:
         if name[-4:].lower() == '.pyz':
             return ZlibArchive(name)
         return CArchiveReader(name)
@@ -153,20 +152,20 @@
     dpos, dlen, ulen, flag, typcd, name = arch.toc[ndx]
     x, data = arch.extract(ndx)
     return data
 
 
 def show(name, arch):
     if isinstance(arch.toc, dict):
-        print(" Name: (ispkg, pos, len)")
+        logger.debug(" Name: (ispkg, pos, len)")
         toc = arch.toc
     else:
-        print(" pos, length, uncompressed, iscompressed, type, name")
+        logger.debug(" pos, length, uncompressed, iscompressed, type, name")
         toc = arch.toc.data
-    pprint.pprint(toc)
+    logger.debug(f'\n'.join([f'{x} : {toc[x]}' for x in toc]))
 
 
 def get_content(arch, recursive, brief, output):
     if isinstance(arch.toc, dict):
         toc = arch.toc
         if brief:
             for name, _ in toc.items():
@@ -188,18 +187,19 @@
 
 def show_log(arch, recursive, brief):
     output = []
     get_content(arch, recursive, brief, output)
     # first print all TOCs
     for out in output:
         if isinstance(out, dict):
-            pprint.pprint(out)
-    # then print the other entries
-    pprint.pprint([out for out in output if not isinstance(out, dict)])
+            logger.debug(f'\n'.join([f'{x} : {out[x]}' for x in out]))
 
+    # then print the other entries
+    [logger.debug(f'\n'.join([f'{x} : {out[x]}' for x in out])) for out in output if not isinstance(out, dict)]
+    
 
 def get_archive_content(filename):
     """
     Get a list of the (recursive) content of archive `filename`.
 
     This function is primary meant to be used by runtests.
     """
@@ -215,17 +215,18 @@
     def checkmagic(self):
         """
         Overridable.
         Check to see if the file object self.lib actually has a file we understand.
         """
         self.lib.seek(self.start)  # default - magic is at start of file.
         if self.lib.read(len(self.MAGIC)) != self.MAGIC:
-            raise RuntimeError("%s is not a valid %s archive file" % (self.path, self.__class__.__name__))
+            raise RuntimeError("%s is not a valid %s archive file" %
+                               (self.path, self.__class__.__name__))
         if self.lib.read(len(self.pymagic)) != self.pymagic:
-            print("Warning: pyz is from a different Python version", file=sys.stderr)
+            logger.warn("pyz is from a different Python version")
         self.lib.read(4)
 
 
 def run():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '-l',
```

### Comparing `pydumpck-1.6.168/pydumpck/py_common_dump/__init__.py` & `pydumpck-1.7.62/pydumpck/py_common_dump/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from .. import logger
 import math
 import os
 import shutil
 import time
 from typing import List
 from .. import configuration, pyc_checker
 from ..pyc_checker.pyc import PycHandler
@@ -32,15 +32,15 @@
             'pe': 'arch',
             'elf': 'arch',
             'pyz': 'arch',
             'pyc': 'pyc',
         }
 
     def handle_nofile(self, target_file: str):
-        print(target_file, "[-] is an invalid file name!")
+        logger.error(f'is an invalid file name! {target_file}')
         return -1
 
     @staticmethod
     def build_output_dir(clear=True):
         output_dir = configuration.thread_output_directory
         if clear and os.path.exists(output_dir):
             shutil.rmtree(output_dir)
@@ -66,39 +66,39 @@
         self.any_invalid_plugin = False
         p_prefix = 'plugin_decompiler_enable_'
 
         def filter_plugin(p):
             n = f'{p_prefix}{p}'
             if n not in configuration.__dict__:
                 self.any_invalid_plugin = True
-                print(f'[!] no plugin named {p}')
+                logger.error(f'no plugin named {p}')
                 return None
             return [p, n]
         plugin = [filter_plugin(x) for x in plugin]
         plugin_paths = [x[1] for x in plugin if x]
         if self.any_invalid_plugin:
             keys = list(configuration.__dict__)
             all_valid_plugins = filter(lambda x: x.startswith(p_prefix), keys)
             all_valid_plugins = [x.replace(p_prefix, '')
                                  for x in all_valid_plugins]
-            print(f'[*] all valid plugins:{all_valid_plugins}')
+            logger.debug(f'all valid plugins:{all_valid_plugins}')
             time.sleep(5)
-        print('[*] plugins loaded with', [x[0] for x in plugin if x])
+        logger.debug(f'plugins loaded with {[x[0] for x in plugin if x]}')
         [setattr(configuration, x, True) for x in plugin_paths]
 
         if configuration.plugin_decompiler_enable_uncompyle6 and configuration.decompile_file == None:
-            print('[!] attention! when use uncompyle6 , you should use --decompile_file specified which file to decompile for faster task.')
+            logger.error('attention! when use uncompyle6 , you should use --decompile_file specified which file to decompile for faster task.')
             time.sleep(3)
 
     def statistics_status(self, is_end: bool = False):
         if is_end:
             g = self.global_start_time
             cost = time.time() - g
             cost = math.ceil(cost*1e3)
-            print(f'[+] completed,cost {cost}ms', f'with result:{self.result}')
+            logger.info(f'completed,cost {cost}ms with result:{self.result}')
             return
         self.global_start_time = time.time()
 
     def main(self, target_file: str, output_directory: str, thread: int = 0, timeout: int = 10, target_file_type: str = None, session_timeout: int = 120, plugin: List = [], decompile_file: List = None, struct_headers: str = None, **args):
         self.statistics_status()
         print_banner()
         if struct_headers:
@@ -109,31 +109,31 @@
         configuration.thread_timeout = timeout
         configuration.thread_output_directory = output_directory
         configuration.progress_session_timeout = session_timeout
         configuration.decompile_file = dict(
             zip(decompile_file, [True for x in decompile_file])) if decompile_file else None
         self.load_plugins(plugin)
         if not target_file:
-            print('[!] target_file is required')
+            logger.error('target_file is required')
             return
         os.chdir(os.path.dirname(target_file))
-        print(f'[*] target file input:{target_file}\nto:{output_directory}')
+        logger.debug(f'target file input:{target_file}\nto:{output_directory}')
 
         if os.path.exists(output_directory):
-            print(f'[+] removing output_directory')
+            logger.info(f'removing output_directory')
             try:
                 shutil.rmtree(output_directory)
             except:
                 pass
         file_type = target_file_type or self.get_filetype(target_file)
         dispatch_to = self.action_map.get(file_type, None)
         if not dispatch_to in self.action_dispatch:
             self.result = f'unkonwn file-type:{file_type}->{dispatch_to}'
         else:
-            print(f'[*] start dump target file.')
+            logger.debug(f'start dump target file.')
             time.sleep(3)
             self.result = self.action_dispatch[dispatch_to](target_file)
 
         self.statistics_status(True)
         return self.result
 
     @staticmethod
```

### Comparing `pydumpck-1.6.168/pydumpck/py_package/package_description/__init__.py` & `pydumpck-1.7.62/pydumpck/py_package/package_description/__init__.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/py_package/package_struct/__init__.py` & `pydumpck-1.7.62/pydumpck/py_package/package_struct/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from ... import configuration, pyc_checker
+from ... import configuration, pyc_checker, logger
 from ...pyc_checker import extensions
 from concurrent.futures import ThreadPoolExecutor
 import multiprocessing
 import time
 
 
 class PackageStruct:
@@ -31,19 +31,22 @@
     @staticmethod
     def decompile_pyc(file: str):
         # TODO log error from dump
         try:
             t = configuration.thread_timeout
             code, err = pyc_checker.dump_pyc(file, file, t)
             if code:
-                print('[+] decompile bytecode', file, len(code))
+                logger.info(
+                    f'decompile bytecode on file:{file},length:{len(code)}')
             else:
-                print('[!] fail to decompile bytecode', file, err)
+                logger.warning(
+                    f'fail to decompile bytecode on file:{file},with error:{err}')
         except Exception as e:
-            print('[!] Exception on decompile bytecode', file, e)
+            logger.warning(
+                f'Exception on decompile bytecode file:{file},with error:{err}')
 
     def callback_pyc_decompile(self, f: str):
         PackageStruct.decompile_pyc(f)
         self.handle_count += 1
 
     def progress_check_pyc_decompile(self):
         files = self.pyc_files
@@ -84,23 +87,23 @@
         if self.total_count == 0:
             return
         self.handle_count = 0
         self.start_pyz_handle()
         return self.progress_waitter('dumping pyz files')
 
     def progress_check(self):
-        print('\nexport pyc')
+        logger.debug('\nexport pyc')
         self.progress_check_dumping_file()  # export pyc
-        print('\ndecompile pyc')
+        logger.debug('\ndecompile pyc')
         self.progress_check_pyc_decompile()  # decompile pyc
-        print('\nextract pyz')
+        logger.debug('\nextract pyz')
         self.progress_check_extract_pyz()  # extract pyz
-        print('\ndecompile pyc for `extract pyz`')
+        logger.debug('\ndecompile pyc for `extract pyz`')
         self.progress_check_pyc_decompile()  # decompile pyc for `extract pyz`
-        print('\nprogress_check completed')
+        logger.debug('\nprogress_check completed')
         pass
 
     def start_pyz_handle(self):
         if self.encrypt_key_file:
             src_file = extensions.get_pycdc_path(
                 self.encrypt_key_file)
             if not os.path.exists(src_file):
@@ -126,18 +129,18 @@
         package.parent = self
         self.packages.append(package)
         if package.name == 'struct':
             data = package.dump_raw_file()
             if data:
                 self.struct_data = data[0:data.find(b'\xe3')]
                 pyc_checker.default_pyc.file_header = self.struct_data
-                print('[+] struct file found', self.struct_data)
+                logger.info(f'struct file found:{self.struct_data}')
         elif package.name == pyc_checker.pyimod00_crypto_key:
             self.encrypt_key_file = package.out_file
-            print('[+] encrypt_file found', self.encrypt_key_file)
+            logger.info(f'encrypt_file found:{self.encrypt_key_file}')
 
     def dump(self):
         packages = self.packages
         self.packages = []
         self.total_count = len(packages)
         self.handle_count = 0
         [self.pool.submit(self.handle_single, p) for p in packages]
```

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/__init__.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .. import configuration
+from .. import configuration, logger
 from . import extensions, lib_pycdc, lib_uncompyle6
 from .pyc import default_pyc, PycHandler
 import os
 import subprocess
 pyimod00_crypto_key = 'pyimod00_crypto_key'
 
 
@@ -40,63 +40,68 @@
 
 
 def exec_pycdc(structed_pyc_file: str, target_file: str, timeout: int = 10):
     if not lib_pycdc.tool_pycdc:
         if configuration.plugin_decompiler_enable_pycdc:
             lib_pycdc.use_pycdc()
             return exec_pycdc(structed_pyc_file, target_file, timeout)
-        return (None, '[*] pycdc not initilized')
+        return (None, 'pycdc not initilized')
     try:
         p = subprocess.run([lib_pycdc.tool_pycdc, structed_pyc_file],
                            stdout=subprocess.PIPE, stderr=subprocess.PIPE, timeout=timeout)
         content = p.stdout.decode('utf-8')
         err, warning = split_warning_error(p.stderr.decode('utf-8'))
         if warning:
-            print(f'[!] warning:\n{warning}\non exec_pycdc:{structed_pyc_file}')
+            logger.warning(
+                f'\n{warning}\non exec_pycdc:{structed_pyc_file}')
         if not err:
             err = None
         result = (remove_pycdc_banner(content), err)
         if content:
-            print('[+] decompile bytecode by pycdc success',
-                  target_file, len(result[0]))
+            logger.info(
+                f'decompile bytecode by pycdc success on file:{target_file},length:{len(result[0])}')
             with open(extensions.get_pycdc_path(target_file), 'wb') as f:
                 f.write(result[0].encode('utf-8'))
         else:
-            print('[!] decompile bytecode by pycdc fail', target_file, err)
+            logger.warning(
+                f'decompile bytecode by pycdc fail,file:{target_file},with error:{e}')
         return result
     except Exception as e:
-        print('[!] decompile bytecode by pycdc fail', target_file, e)
+        logger.warning(
+            f'decompile bytecode by pycdc fail,file:{target_file},with error:{e}')
         return (None, e)
 
 
 def exec_uncompyle6(structed_pyc_file: str, target_file: str, timeout: int = 10):
     if not lib_uncompyle6.tool_uncompyle6:
         if configuration.plugin_decompiler_enable_uncompyle6:
             lib_uncompyle6.use_uncompyle6()
             return exec_uncompyle6(structed_pyc_file, target_file, timeout)
-        return (None, '[*] uncompyle6 not initilized')
+        return (None, 'uncompyle6 not initilized')
     try:
         # TODO use asyncio,support timeout check
         r = lib_uncompyle6.tool_uncompyle6.decompile_to_file(
             pyc_file=structed_pyc_file,
             target_file=f'{target_file}.up6.py')
         r = remove_pyuncompyle6_banner(r)
-        print('[+] decompile bytecode by uncompyle6 success', target_file, len(r))
+        logger.info(
+            f'decompile bytecode by uncompyle6 success file:{target_file},length:{len(r)}')
         return (r, None)
     except Exception as e:
-        print('[!] decompile bytecode by uncompyle6 fail', target_file, e)
+        logger.error(
+            f'decompile bytecode by uncompyle6 fail file:{target_file} ,with error :{e}')
         return (None, e)
 
 
 def dump(data: bytes, target_file: str, structed_pyc_file: str, timeout: int = 10, use_attach_header: bool = True):
     if use_attach_header:
         same, data = default_pyc.attach_pyc_struct(data, structed_pyc_file)
     filename = extensions.get_filename(structed_pyc_file)
     if configuration.decompile_file != None and filename not in configuration.decompile_file and pyimod00_crypto_key != filename:
-        return (None, f'[*] not in decompile files:{filename}')
+        return (None, f'not in decompile files:{filename}')
     content_cdc, err_cdc = exec_pycdc(structed_pyc_file, target_file, timeout)
     content_uncompyle6, err_uncompyle6 = exec_uncompyle6(
         structed_pyc_file, target_file, timeout)
     # TODO log error info
     content = content_cdc or content_uncompyle6
     err = err_cdc or err_uncompyle6
     err = Exception(
```

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/extensions.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/extensions.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/__init__.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ... import logger
 import os
 import shutil
 import time
 package_dir = os.path.dirname(os.path.realpath(__file__))
 tool_pycdc: str = None
 
 
@@ -13,22 +14,22 @@
     build_flag: bool = False
     bin_path = get_bin_path()
     if os.name == 'nt':
         pycdc_file = f'{bin_path}.exe'
     else:
         pycdc_file = bin_path
         if not os.path.exists(pycdc_file):
-            print('[!] pycdc_file not exist , trying build it...')
+            logger.error('pycdc_file not exist , trying build it...')
             time.sleep(5)
             from . import build
             build_file, build_flag = build.build(pycdc_file)
-            print('get compile file path', build_file, build_flag)
+            logger.info(f'get compile file path:{build_file},is_build:{build_flag}')
                 
 
     if os.stat(pycdc_file).st_mode != 0o100777:
-        print(f'[*] detect pycdc_file not executable,try auth:{pycdc_file}')
+        logger.debug(f'detect pycdc_file not executable,try auth:{pycdc_file}')
         os.chmod(pycdc_file, 0o100777)
     if not os.path.isfile(pycdc_file):
-        raise Exception(f'[!] required binary file is not exist:{pycdc_file}')
+        raise Exception(f'required binary file is not exist:{pycdc_file}')
     global tool_pycdc
     tool_pycdc = pycdc_file
     return build_flag
```

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/build.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from .. import logger
 from typing import Tuple
 import zipfile
 import os
 import shutil
 import time
 import threading
 import shutil
 g_lock = threading.Lock()
 build_cache: str = None
 
-
 def get_self_path():
     return os.path.realpath(os.path.dirname(__file__))
 
 
 def get_src_path():
     f = get_self_path()
     zip_file_path = os.path.join(f, 'src')
@@ -44,29 +44,29 @@
     '''
     global build_cache
     global g_lock
     g_lock.acquire(True)
     if build_cache:
         g_lock.release()
         return build_cache, False
-    print('[*] no cache exist , start build')
+    logger.debug('no cache exist , start build')
     export_file = f'{__build()}{os.path.sep}pycdc'
     if move_to:
         build_cache = move_to
     else:
         build_cache = os.path.join(get_self_path(), 'pycdc_cache')
-    print('[*] moving pycdc file', export_file, build_cache)
+    logger.debug(f'moving pycdc file {export_file} , has cache:{build_cache}')
     try:
         shutil.move(export_file, build_cache)
         clear()
         os.chmod(build_cache, 0o100777)
     except Exception as e:
-        print('[!] error on migrating..', e)
+        logger.error(f'error on migrating..{e}')
     g_lock.release()
-    print('[*] completed built')
+    logger.debug('completed built')
     return build_cache, True
 
 
 def clear():
     zip_file, src_path = get_src_path()
     if os.path.exists(src_path):
         shutil.rmtree(src_path)
```

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/pycdc.exe` & `pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/pycdc.exe`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/lib_pycdc/src/pycdc.zip` & `pydumpck-1.7.62/pydumpck/pyc_checker/lib_pycdc/src/pycdc.zip`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/lib_uncompyle6/__init__.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/lib_uncompyle6/__init__.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/py_extract.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/py_extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 Version 2.0 (March 26, 2020)
 -------------------------------------------------
 - Project migrated to github
 - Supports pyinstaller 3.6
 - Added support for Python 3.7, 3.8
 - The header of all extracted pyc's are now automatically fixed
 """
-
+from .. import logger
 from __future__ import print_function
 import os
 import struct
 import marshal
 import zlib
 import sys
 from uuid import uuid4 as uniquename
@@ -102,35 +102,35 @@
 
 
     def open(self):
         try:
             self.fPtr = open(self.filePath, 'rb')
             self.fileSize = os.stat(self.filePath).st_size
         except:
-            print('[!] Error: Could not open {0}'.format(self.filePath))
+            logger.error('Error: Could not open {0}'.format(self.filePath))
             return False
         return True
 
 
     def close(self):
         try:
             self.fPtr.close()
         except:
             pass
 
 
     def checkFile(self):
-        print('[+] Processing {0}'.format(self.filePath))
+        logger.info('Processing {0}'.format(self.filePath))
 
         searchChunkSize = 8192
         endPos = self.fileSize
         self.cookiePos = -1
 
         if endPos < len(self.MAGIC):
-            print('[!] Error : File is too short or truncated')
+            logger.error('Error : File is too short or truncated')
             return False
 
         while True:
             startPos = endPos - searchChunkSize if endPos >= searchChunkSize else 0
             chunkSize = endPos - startPos
 
             if chunkSize < len(self.MAGIC):
@@ -147,25 +147,25 @@
 
             endPos = startPos + len(self.MAGIC) - 1
 
             if startPos == 0:
                 break
 
         if self.cookiePos == -1:
-            print('[!] Error : Missing cookie, unsupported pyinstaller version or not a pyinstaller archive')
+            logger.error('Error : Missing cookie, unsupported pyinstaller version or not a pyinstaller archive')
             return False
 
         self.fPtr.seek(self.cookiePos + self.PYINST20_COOKIE_SIZE, os.SEEK_SET)
 
         if b'python' in self.fPtr.read(64):
-            print('[+] Pyinstaller version: 2.1+')
+            logger.info('Pyinstaller version: 2.1+')
             self.pyinstVer = 21     # pyinstaller 2.1+
         else:
             self.pyinstVer = 20     # pyinstaller 2.0
-            print('[+] Pyinstaller version: 2.0')
+            logger.info('Pyinstaller version: 2.0')
 
         return True
 
 
     def getCArchiveInfo(self):
         try:
             if self.pyinstVer == 20:
@@ -179,29 +179,29 @@
                 self.fPtr.seek(self.cookiePos, os.SEEK_SET)
 
                 # Read CArchive cookie
                 (magic, lengthofPackage, toc, tocLen, self.pyver, pylibname) = \
                 struct.unpack('!8siiii64s', self.fPtr.read(self.PYINST21_COOKIE_SIZE))
 
         except:
-            print('[!] Error : The file is not a pyinstaller archive')
+            logger.error('Error : The file is not a pyinstaller archive')
             return False
 
-        print('[+] Python version: {0}'.format(self.pyver))
+        logger.info('Python version: {0}'.format(self.pyver))
 
         # Additional data after the cookie
         tailBytes = self.fileSize - self.cookiePos - (self.PYINST20_COOKIE_SIZE if self.pyinstVer == 20 else self.PYINST21_COOKIE_SIZE)
         
         # Overlay is the data appended at the end of the PE
         self.overlaySize = lengthofPackage + tailBytes
         self.overlayPos = self.fileSize - self.overlaySize
         self.tableOfContentsPos = self.overlayPos + toc
         self.tableOfContentsSize = tocLen
 
-        print('[+] Length of package: {0} bytes'.format(lengthofPackage))
+        logger.info('Length of package: {0} bytes'.format(lengthofPackage))
         return True
 
 
     def parseTOC(self):
         # Go to the table of contents
         self.fPtr.seek(self.tableOfContentsPos, os.SEEK_SET)
 
@@ -217,42 +217,42 @@
             struct.unpack( \
                 '!iiiBc{0}s'.format(entrySize - nameLen), \
                 self.fPtr.read(entrySize - 4))
 
             name = name.decode('utf-8').rstrip('\0')
             if len(name) == 0:
                 name = str(uniquename())
-                print('[!] Warning: Found an unamed file in CArchive. Using random name {0}'.format(name))
+                logger.error('Warning: Found an unamed file in CArchive. Using random name {0}'.format(name))
 
             self.tocList.append( \
                                 CTOCEntry(                      \
                                     self.overlayPos + entryPos, \
                                     cmprsdDataSize,             \
                                     uncmprsdDataSize,           \
                                     cmprsFlag,                  \
                                     typeCmprsData,              \
                                     name                        \
                                 ))
 
             parsedLen += entrySize
-        print('[+] Found {0} files in CArchive'.format(len(self.tocList)))
+        logger.info('Found {0} files in CArchive'.format(len(self.tocList)))
 
 
     def _writeRawData(self, filepath, data):
         nm = filepath.replace('\\', os.path.sep).replace('/', os.path.sep).replace('..', '__')
         nmDir = os.path.dirname(nm)
         if nmDir != '' and not os.path.exists(nmDir): # Check if path exists, create if not
             os.makedirs(nmDir)
 
         with open(nm, 'wb') as f:
             f.write(data)
 
 
     def extractFiles(self):
-        print('[+] Beginning extraction...please standby')
+        logger.info('Beginning extraction...please standby')
         extractionDir = os.path.join(os.getcwd(), os.path.basename(self.filePath) + '_extracted')
 
         if not os.path.exists(extractionDir):
             os.mkdir(extractionDir)
 
         os.chdir(extractionDir)
 
@@ -277,15 +277,15 @@
                 # Check if path exists, create if not
                 if not os.path.exists(basePath):
                     os.makedirs(basePath)
 
             if entry.typeCmprsData == b's':
                 # s -> ARCHIVE_ITEM_PYSOURCE
                 # Entry point are expected to be python scripts
-                print('[+] Possible entry point: {0}.pyc'.format(entry.name))
+                logger.info('Possible entry point: {0}.pyc'.format(entry.name))
                 self._writePyc(entry.name + '.pyc', data)
 
             elif entry.typeCmprsData == b'M' or entry.typeCmprsData == b'm':
                 # M -> ARCHIVE_ITEM_PYPACKAGE
                 # m -> ARCHIVE_ITEM_PYMODULE
                 # packages and modules are pyc files with their header's intact
                 self._writeRawData(entry.name + '.pyc', data)
@@ -323,29 +323,29 @@
             pyzMagic = f.read(4)
             assert pyzMagic == b'PYZ\0' # Sanity Check
 
             pycHeader = f.read(4) # Python magic value
 
             # Skip PYZ extraction if not running under the same python version
             if pyc_magic != pycHeader:
-                print('[!] Warning: This script is running in a different Python version than the one used to build the executable.')
-                print('[!] Please run this script in Python{0} to prevent extraction errors during unmarshalling'.format(self.pyver))
-                print('[!] Skipping pyz extraction')
+                logger.error('Warning: This script is running in a different Python version than the one used to build the executable.')
+                logger.error('Please run this script in Python{0} to prevent extraction errors during unmarshalling'.format(self.pyver))
+                logger.error('Skipping pyz extraction')
                 return
 
             (tocPosition, ) = struct.unpack('!i', f.read(4))
             f.seek(tocPosition, os.SEEK_SET)
 
             try:
                 toc = marshal.load(f)
             except:
-                print('[!] Unmarshalling FAILED. Cannot extract {0}. Extracting remaining files.'.format(name))
+                logger.error('Unmarshalling FAILED. Cannot extract {0}. Extracting remaining files.'.format(name))
                 return
 
-            print('[+] Found {0} files in PYZ archive'.format(len(toc)))
+            logger.info('Found {0} files in PYZ archive'.format(len(toc)))
 
             # From pyinstaller 3.1+ toc is a list of tuples
             if type(toc) == list:
                 toc = dict(toc)
 
             for key in toc.keys():
                 (ispkg, pos, length) = toc[key]
@@ -371,35 +371,33 @@
                 if not os.path.exists(fileDir):
                     os.makedirs(fileDir)
 
                 try:
                     data = f.read(length)
                     data = zlib.decompress(data)
                 except:
-                    print('[!] Error: Failed to decompress {0}, probably encrypted. Extracting as is.'.format(filePath))
+                    logger.error('Error: Failed to decompress {0}, probably encrypted. Extracting as is.'.format(filePath))
                     open(filePath + '.encrypted', 'wb').write(data)
                 else:
                     self._writePyc(filePath, data)
 
 
 def main():
     if len(sys.argv) < 2:
-        print('[+] Usage: pyinstxtractor.py <filename>')
+        logger.info('Usage: pyinstxtractor.py <filename>')
 
     else:
         arch = PyInstArchive(sys.argv[1])
         if arch.open():
             if arch.checkFile():
                 if arch.getCArchiveInfo():
                     arch.parseTOC()
                     arch.extractFiles()
                     arch.close()
-                    print('[+] Successfully extracted pyinstaller archive: {0}'.format(sys.argv[1]))
-                    print('')
-                    print('You can now use a python decompiler on the pyc files within the extracted directory')
+                    logger.info('Successfully extracted pyinstaller archive: {0}\nYou can now use a python decompiler on the pyc files within the extracted directory''.format(sys.argv[1]))
                     return
 
             arch.close()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/pyc/__init__.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/pyc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import xdis.unmarshal
 from typing import List, Tuple
+from .. import logger
 from ...configuration.res_lock import check_directory
 from . import headers, magic_code
 import os
 import io
 
 
 class PycHandler():
@@ -33,15 +34,15 @@
                 success_version_mode = i
                 break
             except Exception as e:
                 pass
             fp.seek(0)
         if success_version_mode:
             v, magic, demo_header = success_version_mode
-            print(f'[+] find suitable python-version:{v},magic:{magic}')
+            logger.info(f'find suitable python-version:{v},magic:{magic}')
             return bytes(demo_header)
         return None
 
     def get_e3(self, data: bytes):
         pos = data.find(b'\xe3')
         return pos, data[pos:]
```

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/OpCode/py3.10.4.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/OpCode/py3.10.4.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/pyc/headers/__init__.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/pyc/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/pyc/magic_code/__init__.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/pyc/magic_code/__init__.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/pyc_checker/pyz_extract.py` & `pydumpck-1.7.62/pydumpck/pyc_checker/pyz_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .. import logger
 from typing import List
 from io import BufferedReader
 import os
 import zlib
 import sys
 import struct
 import marshal
@@ -40,27 +41,27 @@
     pyzMagic = f.read(4)
     assert pyzMagic == b'PYZ\0'  # Sanity Check
 
     pycHeader = f.read(4)  # Python magic value
 
     # Skip PYZ extraction if not running under the same python version
     if pyc_magic != pycHeader:
-        print('[!] Warning: This script is running in a different Python version than the one used to build the executable.')
+        logger.error('Warning: This script is running in a different Python version than the one used to build the executable.')
 
     (tocPosition, ) = struct.unpack('!i', f.read(4))
     f.seek(tocPosition, os.SEEK_SET)
 
     try:
         toc = marshal.load(f)
     except:
-        print(
-            '[!] Unmarshalling FAILED. Cannot extract {0}. Extracting remaining files.'.format(dirName))
+        logger.warning(
+            'Unmarshalling FAILED. Cannot extract {0}. Extracting remaining files.'.format(dirName))
         return
 
-    print('[+] Found {0} files in PYZ archive'.format(len(toc)))
+    logger.info('Found {0} files in PYZ archive'.format(len(toc)))
 
     # From pyinstaller 3.1+ toc is a list of tuples
     if type(toc) == list:
         toc = dict(toc)
 
     def handle_single(key: str):
         (ispkg, pos, length) = toc[key]
```

### Comparing `pydumpck-1.6.168/pydumpck/pyinstaller_dump.py` & `pydumpck-1.7.62/pydumpck/pyinstaller_dump.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import logger
 import argparse
 from typing import List
 import pydumpck.__version__ as __version__
 from pydumpck.py_common_dump import CommonDump
 import pydumpck.utils.paths
 import time
 
@@ -90,19 +91,19 @@
         nargs=argparse.ZERO_OR_MORE,
         dest='plugin',
         help='enable decompiler plugins,split by space .example: `--plugin pycdc uncompyle6` (default: %(default)s).available:pycdc,uncompyle6',
     )
     args = parser.parse_args()
     if not args.show_version == False:
         v = __version__.__version__
-        print(v)
+        logger.debug(v)
         return v
-    print(parser.description)
-    print('-' * 20)
-    print(f'[+] pydumpck initilizing with {__version__.__version__}')
+    desc = parser.description + '\n' + '-' * 20
+    content = f'pydumpck initilizing with {__version__.__version__}'
+    logger.info(f'{desc}\n{content}')
     try:
         dmp = CommonDump()
         return dmp.main(**vars(args))
     except KeyboardInterrupt:
         raise SystemExit("Aborted by user request.")
```

### Comparing `pydumpck-1.6.168/pydumpck/utils/banner.py` & `pydumpck-1.7.62/pydumpck/utils/banner.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck/utils/extensions/__init__.py` & `pydumpck-1.7.62/pydumpck/utils/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/pydumpck.egg-info/PKG-INFO` & `pydumpck-1.7.62/pydumpck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydumpck
-Version: 1.6.168
+Version: 1.7.62
 Summary: pydumpck is a multi-threads tool for decompile exe,elf,pyz,pyc packed by python which is base on pycdc and uncompyle6.sometimes its py-file result not exactly right ,maybe could use uncompyle6.
 Home-page: https://github.com/serfend/pydumpck
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: pydumpck,decomplier,pe,elf,pyc,pyz
 Platform: any
@@ -139,7 +139,13 @@
 ## Notice
 
 > `pycdc` speed is more than 10 times faster than `uncompyle6` , and `uncompyle6` is not support for python that version above 3.8.
 >
 > however `pycdc` sometimes return a not precisely right result.
 >
 > in pydumpck , you can use `--plugin uncompyle6` for single-use or `--plugin pycdc uncompyle6` for both-use.
+
+
+
+## Status
+
+![Alt](https://repobeats.axiom.co/api/embed/013759c6315338178a2643de0bca01826fb39a14.svg "Repobeats analytics image")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydumpck Version: 1.6.168 Summary: pydumpck is a
+Metadata-Version: 2.1 Name: pydumpck Version: 1.7.62 Summary: pydumpck is a
 multi-threads tool for decompile exe,elf,pyz,pyc packed by python which is base
 on pycdc and uncompyle6.sometimes its py-file result not exactly right ,maybe
 could use uncompyle6. Home-page: https://github.com/serfend/pydumpck Author:
 serfend Author-email: serfend@foxmail.com License: MIT Licence Keywords:
 pydumpck,decomplier,pe,elf,pyc,pyz Platform: any Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
@@ -64,8 +64,10 @@
 lib_base64 secert` for targets `main.py` and `lib_base64.py` and `secert.py` ##
 Demo - pyc with header been tampered with - (Warning:gif with size 5MB)![pyc-
 fix_header-demo](https://raw.githubusercontent.com/serfend/res.image.reference/
 main/pyc-fix_header-demo.gif) ## Notice > `pycdc` speed is more than 10 times
 faster than `uncompyle6` , and `uncompyle6` is not support for python that
 version above 3.8. > > however `pycdc` sometimes return a not precisely right
 result. > > in pydumpck , you can use `--plugin uncompyle6` for single-use or
-`--plugin pycdc uncompyle6` for both-use.
+`--plugin pycdc uncompyle6` for both-use. ## Status ![Alt](https://
+repobeats.axiom.co/api/embed/013759c6315338178a2643de0bca01826fb39a14.svg
+"Repobeats analytics image")
```

### Comparing `pydumpck-1.6.168/pydumpck.egg-info/SOURCES.txt` & `pydumpck-1.7.62/pydumpck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydumpck-1.6.168/setup.py` & `pydumpck-1.7.62/setup.py`

 * *Files identical despite different names*

