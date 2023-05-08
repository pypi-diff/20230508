# Comparing `tmp/transformgpt-0.1.2.tar.gz` & `tmp/transformgpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformgpt-0.1.2.tar", last modified: Sat May  6 22:42:14 2023, max compression
+gzip compressed data, was "transformgpt-0.1.3.tar", last modified: Mon May  8 00:02:44 2023, max compression
```

## Comparing `transformgpt-0.1.2.tar` & `transformgpt-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.853140 transformgpt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-06 22:42:01.000000 transformgpt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-06 22:42:14.853140 transformgpt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-06 22:42:01.000000 transformgpt-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-06 22:42:14.853140 transformgpt-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-06 22:42:01.000000 transformgpt-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.849140 transformgpt-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-06 22:42:01.000000 transformgpt-0.1.2/test/test_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.849140 transformgpt-0.1.2/transformgpt/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/source_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/transformgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.853140 transformgpt-0.1.2/transformgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:02:44.667798 transformgpt-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 00:02:31.000000 transformgpt-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-08 00:02:44.667798 transformgpt-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-08 00:02:31.000000 transformgpt-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 00:02:44.667798 transformgpt-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 00:02:31.000000 transformgpt-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:02:44.663798 transformgpt-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-08 00:02:31.000000 transformgpt-0.1.3/test/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-08 00:02:31.000000 transformgpt-0.1.3/test/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:02:44.663798 transformgpt-0.1.3/transformgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 00:02:31.000000 transformgpt-0.1.3/transformgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-08 00:02:31.000000 transformgpt-0.1.3/transformgpt/classify_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-08 00:02:31.000000 transformgpt-0.1.3/transformgpt/source_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-08 00:02:31.000000 transformgpt-0.1.3/transformgpt/transform_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-08 00:02:31.000000 transformgpt-0.1.3/transformgpt/transformgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:02:44.667798 transformgpt-0.1.3/transformgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-08 00:02:44.000000 transformgpt-0.1.3/transformgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 00:02:44.000000 transformgpt-0.1.3/transformgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:02:44.000000 transformgpt-0.1.3/transformgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 00:02:44.000000 transformgpt-0.1.3/transformgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 00:02:44.000000 transformgpt-0.1.3/transformgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 00:02:44.000000 transformgpt-0.1.3/transformgpt.egg-info/top_level.txt
```

### Comparing `transformgpt-0.1.2/LICENSE` & `transformgpt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.2/PKG-INFO` & `transformgpt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: transformgpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for transforming unstructured text into structured data without context/mappings using ChatGPT.
 Home-page: https://github.com/TSavo/transformgpt
-Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.2
+Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.3
 Author: T Savo
 Author-email: evilgenius@nefariousplan.com
 License: MIT
 Keywords: openai gpt3 chatgpt nlp chatbot transformers structruing text
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `transformgpt-0.1.2/README.md` & `transformgpt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.2/setup.py` & `transformgpt-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-VERSION='0.1.2'
+VERSION='0.1.3'
 setup(
     name='transformgpt',
     version=VERSION,
     packages=['transformgpt'],
     author='T Savo',
     author_email="evilgenius@nefariousplan.com",
     description="A library for transforming unstructured text into structured data without context/mappings using ChatGPT.",
@@ -12,17 +12,19 @@
     requires=["openai"],
     py_modules=['transformgpt'],
     download_url='https://github.com/tsavo/transformgpt/tarball/{}'.format(VERSION),
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=['openai>=0.27.6'],
-    scripts=['transformgpt/main.py'],
+    scripts=['transformgpt/transform_main.py',
+             'transformgpt/classify_main.py'],
     entry_points={
-        'console_scripts': ['transformgpt=transformgpt.main:main'],
+        'console_scripts': ['transformgpt=transformgpt.transform_main:main',
+                            'classifygpt=transformgpt.classify_main:main'],
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Natural Language :: English',
         'Environment :: Console',
```

### Comparing `transformgpt-0.1.2/test/test_interpreter.py` & `transformgpt-0.1.3/test/test_transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 from dataclasses import dataclass
 import dataclasses
 from typing import List, Optional
 import unittest
 import openai
 import os
+import sys
+# add .. to the path so we can import transformgpt
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
 from transformgpt import TransformGPT
 
 
 openai.api_key = os.getenv("OpenAIAPI-Token")
 transformer = TransformGPT(openai.ChatCompletion)
 
 @dataclass
```

### Comparing `transformgpt-0.1.2/transformgpt/main.py` & `transformgpt-0.1.3/transformgpt/transform_main.py`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.2/transformgpt/source_utils.py` & `transformgpt-0.1.3/transformgpt/source_utils.py`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.2/transformgpt.egg-info/PKG-INFO` & `transformgpt-0.1.3/transformgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: transformgpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for transforming unstructured text into structured data without context/mappings using ChatGPT.
 Home-page: https://github.com/TSavo/transformgpt
-Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.2
+Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.3
 Author: T Savo
 Author-email: evilgenius@nefariousplan.com
 License: MIT
 Keywords: openai gpt3 chatgpt nlp chatbot transformers structruing text
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

