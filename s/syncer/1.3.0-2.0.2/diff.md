# Comparing `tmp/syncer-1.3.0.tar.gz` & `tmp/syncer-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syncer-1.3.0.tar", last modified: Sat Jun  3 10:14:49 2017, max compression
+gzip compressed data, was "syncer-2.0.2.tar", last modified: Mon May  8 07:44:27 2023, max compression
```

## Comparing `syncer-1.3.0.tar` & `syncer-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 takagi    (1000) takagi    (1000)        0 2017-06-03 10:14:49.000000 syncer-1.3.0/
-drwxrwxr-x   0 takagi    (1000) takagi    (1000)        0 2017-06-03 10:14:49.000000 syncer-1.3.0/tests/
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     3356 2017-06-03 10:13:11.000000 syncer-1.3.0/tests/test_py34.py
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     2291 2017-06-03 10:13:11.000000 syncer-1.3.0/tests/test_py35.py
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     2725 2016-03-24 11:58:24.000000 syncer-1.3.0/README.rst
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     1082 2016-03-23 15:05:20.000000 syncer-1.3.0/LICENSE
--rw-rw-r--   0 takagi    (1000) takagi    (1000)      179 2016-03-23 15:05:20.000000 syncer-1.3.0/MANIFEST.in
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     1286 2017-06-03 10:13:11.000000 syncer-1.3.0/syncer.py
--rwxrwxr-x   0 takagi    (1000) takagi    (1000)     1279 2017-06-03 10:14:10.000000 syncer-1.3.0/setup.py
-drwxrwxr-x   0 takagi    (1000) takagi    (1000)        0 2017-06-03 10:14:49.000000 syncer-1.3.0/syncer.egg-info/
--rw-rw-r--   0 takagi    (1000) takagi    (1000)        1 2017-06-03 10:14:49.000000 syncer-1.3.0/syncer.egg-info/not-zip-safe
--rw-rw-r--   0 takagi    (1000) takagi    (1000)        1 2017-06-03 10:14:49.000000 syncer-1.3.0/syncer.egg-info/dependency_links.txt
--rw-rw-r--   0 takagi    (1000) takagi    (1000)        7 2017-06-03 10:14:49.000000 syncer-1.3.0/syncer.egg-info/top_level.txt
--rw-rw-r--   0 takagi    (1000) takagi    (1000)      302 2017-06-03 10:14:49.000000 syncer-1.3.0/syncer.egg-info/SOURCES.txt
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     4180 2017-06-03 10:14:49.000000 syncer-1.3.0/syncer.egg-info/PKG-INFO
--rw-rw-r--   0 takagi    (1000) takagi    (1000)      212 2017-06-03 10:14:49.000000 syncer-1.3.0/setup.cfg
-drwxrwxr-x   0 takagi    (1000) takagi    (1000)        0 2017-06-03 10:14:49.000000 syncer-1.3.0/docs/
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     6762 2016-03-23 15:05:20.000000 syncer-1.3.0/docs/Makefile
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     9198 2017-06-03 10:14:10.000000 syncer-1.3.0/docs/conf.py
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     6459 2016-03-23 15:05:20.000000 syncer-1.3.0/docs/make.bat
--rw-rw-r--   0 takagi    (1000) takagi    (1000)      299 2016-03-23 15:05:20.000000 syncer-1.3.0/docs/index.rst
--rw-rw-r--   0 takagi    (1000) takagi    (1000)     4180 2017-06-03 10:14:49.000000 syncer-1.3.0/PKG-INFO
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/
+-rw-r--r--   0 takagi    (1000) users      (985)     1082 2023-05-08 07:34:27.000000 syncer-2.0.2/LICENSE
+-rw-r--r--   0 takagi    (1000) users      (985)      179 2023-05-08 07:34:27.000000 syncer-2.0.2/MANIFEST.in
+-rw-r--r--   0 takagi    (1000) users      (985)     3123 2023-05-08 07:44:27.526271 syncer-2.0.2/PKG-INFO
+-rw-r--r--   0 takagi    (1000) users      (985)     2385 2023-05-08 07:36:46.000000 syncer-2.0.2/README.rst
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/docs/
+-rw-r--r--   0 takagi    (1000) users      (985)     6762 2023-05-08 07:34:27.000000 syncer-2.0.2/docs/Makefile
+-rw-r--r--   0 takagi    (1000) users      (985)     9198 2023-05-08 07:41:53.000000 syncer-2.0.2/docs/conf.py
+-rw-r--r--   0 takagi    (1000) users      (985)      299 2023-05-08 07:34:27.000000 syncer-2.0.2/docs/index.rst
+-rw-r--r--   0 takagi    (1000) users      (985)     6459 2023-05-08 07:34:27.000000 syncer-2.0.2/docs/make.bat
+-rw-r--r--   0 takagi    (1000) users      (985)      212 2023-05-08 07:44:27.526271 syncer-2.0.2/setup.cfg
+-rwxr-xr-x   0 takagi    (1000) users      (985)     1220 2023-05-08 07:41:53.000000 syncer-2.0.2/setup.py
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/syncer.egg-info/
+-rwxr-xr-x   0 takagi    (1000) users      (985)     3123 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/PKG-INFO
+-rwxr-xr-x   0 takagi    (1000) users      (985)      303 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/SOURCES.txt
+-rwxr-xr-x   0 takagi    (1000) users      (985)        1 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/dependency_links.txt
+-rwxr-xr-x   0 takagi    (1000) users      (985)        1 2018-02-15 06:26:26.000000 syncer-2.0.2/syncer.egg-info/not-zip-safe
+-rwxr-xr-x   0 takagi    (1000) users      (985)        7 2023-05-08 07:44:27.000000 syncer-2.0.2/syncer.egg-info/top_level.txt
+-rw-r--r--   0 takagi    (1000) users      (985)     1007 2023-05-08 07:34:27.000000 syncer-2.0.2/syncer.py
+drwxr-xr-x   0 takagi    (1000) users      (985)        0 2023-05-08 07:44:27.526271 syncer-2.0.2/tests/
+-rw-r--r--   0 takagi    (1000) users      (985)        0 2023-05-08 07:34:27.000000 syncer-2.0.2/tests/__init__.py
+-rw-r--r--   0 takagi    (1000) users      (985)     2291 2023-05-08 07:34:27.000000 syncer-2.0.2/tests/test_syncer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `syncer-1.3.0/tests/test_py35.py` & `syncer-2.0.2/tests/test_syncer.py`

 * *Files identical despite different names*

### Comparing `syncer-1.3.0/README.rst` & `syncer-2.0.2/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,14 @@
 
 .. image:: https://img.shields.io/pypi/v/syncer.svg
         :target: https://pypi.python.org/pypi/syncer
 
 .. image:: https://img.shields.io/pypi/pyversions/syncer.svg
         :target: https://pypi.python.org/pypi/syncer
 
-.. image:: https://img.shields.io/travis/miyakogi/syncer.svg
-        :target: https://travis-ci.org/miyakogi/syncer
-
-.. image:: https://codecov.io/github/miyakogi/syncer/coverage.svg?branch=master
-    :target: https://codecov.io/github/miyakogi/syncer?branch=master
-
 
 Syncer is an async-to-sync converter for python.
 
 * PyPI: https://pypi.python.org/pypi/syncer/
 * Documentation: https://miyakogi.github.io/syncer/
 * Source code: https://github.com/miyakogi/syncer/
 
@@ -25,17 +19,16 @@
 
 Sometimes (mainly in test) we need to convert asynchronous functions to normal,
 synchronous functions and run them synchronously. It can be done by
 ``ayncio.get_event_loop().run_until_complete()``, but it's quite long...
 
 Syncer makes this conversion easy.
 
-* Convert coroutine-function (defined by ``aync def``) to normal (synchronous) function
-* Run coroutines synchronously
-* Support both ``async def`` and decorator (``@asyncio.coroutine``) style
+* Convert async-function (defined by ``aync def``) to normal (synchronous) function
+* Evaluate coroutines synchronously
 
 Install
 =======
 
 At the command line::
 
     $ pip install syncer
```

### Comparing `syncer-1.3.0/LICENSE` & `syncer-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syncer-1.3.0/syncer.py` & `syncer-2.0.2/syncer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import sys
 from functools import singledispatch, wraps
 import asyncio
 import inspect
 import types
 from typing import Any, Callable, Generator
 
 
-PY35 = sys.version_info >= (3, 5)
-
-
-def _is_awaitable(co: Generator[Any, None, Any]) -> bool:
-    if PY35:
-        return inspect.isawaitable(co)
-    else:
-        return (isinstance(co, types.GeneratorType) or
-                isinstance(co, asyncio.Future))
-
-
 @singledispatch
 def sync(co: Any):
     raise TypeError('Called with unsupported argument: {}'.format(co))
 
 
 @sync.register(asyncio.Future)
 @sync.register(types.GeneratorType)
 def sync_co(co: Generator[Any, None, Any]) -> Any:
-    if not _is_awaitable(co):
+    if not inspect.isawaitable(co):
         raise TypeError('Called with unsupported argument: {}'.format(co))
     return asyncio.get_event_loop().run_until_complete(co)
 
 
 @sync.register(types.FunctionType)
 @sync.register(types.MethodType)
 def sync_fu(f: Callable[..., Any]) -> Callable[..., Any]:
@@ -41,9 +29,8 @@
 
     @wraps(f)
     def run(*args, **kwargs):
         return asyncio.get_event_loop().run_until_complete(f(*args, **kwargs))
     return run
 
 
-if PY35:
-    sync.register(types.CoroutineType)(sync_co)
+sync.register(types.CoroutineType)(sync_co)
```

### Comparing `syncer-1.3.0/setup.py` & `syncer-2.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import sys
 from os import path
 
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
+from setuptools import setup
 
 readme_file = path.join(path.dirname(path.abspath(__file__)), 'README.rst')
 with open(readme_file) as readme_file:
     readme = readme_file.read()
 
-install_requires = ['typing'] if sys.version_info < (3, 6) else []
+test_requirements = ['xfail']
 
 setup(
     name='syncer',
-    version='1.3.0',
+    version='2.0.2',
     description='Async to sync converter',
     long_description=readme,
     author='Hiroyuki Takagi',
     author_email='miyako.dev@gmail.com',
     url='https://github.com/miyakogi/syncer',
     py_modules=['syncer'],
     include_package_data=True,
@@ -31,14 +28,16 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    test_suite='test_syncer',
-    install_requires=install_requires,
+    test_suite='tests',
+    tests_require=test_requirements,
+
 )
```

### Comparing `syncer-1.3.0/docs/Makefile` & `syncer-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `syncer-1.3.0/docs/conf.py` & `syncer-2.0.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 copyright = '2016, Hiroyuki Takagi'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '1.3.0'
+version = '2.0.2'
 # The full version, including alpha/beta/rc tags.
-release = '1.3.0'
+release = '2.0.2'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
```

### Comparing `syncer-1.3.0/docs/make.bat` & `syncer-2.0.2/docs/make.bat`

 * *Files identical despite different names*

