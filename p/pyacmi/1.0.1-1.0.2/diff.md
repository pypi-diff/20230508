# Comparing `tmp/pyacmi-1.0.1.tar.gz` & `tmp/pyacmi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.0.1.tar", last modified: Mon May  8 11:38:52 2023, max compression
+gzip compressed data, was "pyacmi-1.0.2.tar", last modified: Mon May  8 16:14:16 2023, max compression
```

## Comparing `pyacmi-1.0.1.tar` & `pyacmi-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:38:52.213270 pyacmi-1.0.1/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 10:54:45.000000 pyacmi-1.0.1/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     1116 2023-05-08 11:38:52.213145 pyacmi-1.0.1/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      438 2023-05-08 11:36:11.000000 pyacmi-1.0.1/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:38:52.212327 pyacmi-1.0.1/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 09:42:33.000000 pyacmi-1.0.1/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    17604 2023-05-08 10:59:36.000000 pyacmi-1.0.1/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 11:38:52.212967 pyacmi-1.0.1/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     1116 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-08 11:38:52.000000 pyacmi-1.0.1/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-08 11:38:52.213315 pyacmi-1.0.1/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-08 11:38:32.000000 pyacmi-1.0.1/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 16:14:16.938254 pyacmi-1.0.2/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 10:54:45.000000 pyacmi-1.0.2/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-08 16:14:16.938110 pyacmi-1.0.2/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      729 2023-05-08 16:11:33.000000 pyacmi-1.0.2/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 16:14:16.934492 pyacmi-1.0.2/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 09:42:33.000000 pyacmi-1.0.2/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    17604 2023-05-08 10:59:36.000000 pyacmi-1.0.2/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 16:14:16.937109 pyacmi-1.0.2/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-08 16:14:16.938743 pyacmi-1.0.2/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-08 16:12:09.000000 pyacmi-1.0.2/setup.py
```

### Comparing `pyacmi-1.0.1/LICENSE` & `pyacmi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.0.1/PKG-INFO` & `pyacmi-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.0.1
+Version: 1.0.2
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -16,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyacmi: TacView ACMI FileParser
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pyacmi.svg)](https://pypi.org/project/pyacmi/)
+[![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
+[![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
-借鉴了[https://github.com/rp-/acmi](https://github.com/rp-/acmi)
+The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
 ## Install
 
 ```shell
 
 pip install pyacmi
 
@@ -39,7 +41,11 @@
 
 from pyacmi import *
 
 acmi = Acmi('test.acmi')
 print(acmi)
 
 ```
+
+## Credits
+
+- [https://github.com/rp-/acmi](https://github.com/rp-/acmi)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyacmi-1.0.1/pyacmi/acmi.py` & `pyacmi-1.0.2/pyacmi/acmi.py`

 * *Files identical despite different names*

### Comparing `pyacmi-1.0.1/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.0.2/pyacmi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.0.1
+Version: 1.0.2
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -16,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyacmi: TacView ACMI FileParser
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pyacmi.svg)](https://pypi.org/project/pyacmi/)
+[![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
+[![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
-借鉴了[https://github.com/rp-/acmi](https://github.com/rp-/acmi)
+The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
 ## Install
 
 ```shell
 
 pip install pyacmi
 
@@ -39,7 +41,11 @@
 
 from pyacmi import *
 
 acmi = Acmi('test.acmi')
 print(acmi)
 
 ```
+
+## Credits
+
+- [https://github.com/rp-/acmi](https://github.com/rp-/acmi)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyacmi-1.0.1/setup.py` & `pyacmi-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.0.1',
+        version='1.0.2',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

