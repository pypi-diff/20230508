# Comparing `tmp/pylovelace-2023.2.0-py3-none-any.whl.zip` & `tmp/pylovelace-2023.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 18072 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      228 b- defN 23-May-07 16:52 pylovelace/__init__.py
+Zip file size: 18082 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      228 b- defN 23-May-07 23:28 pylovelace/__init__.py
 -rw-rw-rw-  2.0 fat     8086 b- defN 23-Apr-19 05:09 pylovelace/__main__.py
 -rw-rw-rw-  2.0 fat     4552 b- defN 23-May-07 16:51 pylovelace/protect.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1805 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      753 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/RECORD
-9 files, 50732 bytes uncompressed, 16766 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-May-07 23:28 pylovelace-2023.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1833 b- defN 23-May-07 23:28 pylovelace-2023.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 23:28 pylovelace-2023.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-May-07 23:28 pylovelace-2023.2.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-07 23:28 pylovelace-2023.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      753 b- defN 23-May-07 23:28 pylovelace-2023.2.1.dist-info/RECORD
+9 files, 50760 bytes uncompressed, 16776 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pylovelace/__main__.py
 Comment: 
 
 Filename: pylovelace/protect.py
 Comment: 
 
-Filename: pylovelace-2023.2.0.dist-info/LICENSE
+Filename: pylovelace-2023.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: pylovelace-2023.2.0.dist-info/METADATA
+Filename: pylovelace-2023.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace-2023.2.0.dist-info/WHEEL
+Filename: pylovelace-2023.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace-2023.2.0.dist-info/entry_points.txt
+Filename: pylovelace-2023.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylovelace-2023.2.0.dist-info/top_level.txt
+Filename: pylovelace-2023.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace-2023.2.0.dist-info/RECORD
+Filename: pylovelace-2023.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/__init__.py

```diff
@@ -4,9 +4,9 @@
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 
-__version__ = "2023.2.0"
+__version__ = "2023.2.1"
 __description__ = "Python code protection/obfuscation tool"
```

## Comparing `pylovelace-2023.2.0.dist-info/LICENSE` & `pylovelace-2023.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylovelace-2023.2.0.dist-info/METADATA` & `pylovelace-2023.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylovelace
-Version: 2023.2.0
+Version: 2023.2.1
 Summary: Python code protection/obfuscation tool
 Home-page: https://github.com/pylovelace/pylovelace
 Author: nshout
 Keywords: obfuscate obfuscation distribute production tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10, <3.13
 License-File: LICENSE
-Requires-Dist: pylovelace.kernel (>=2023.2.0)
+Requires-Dist: pylovelace.kernel (>=2023.3.0)
 
 PyLovelace Python protection tool.
 ===================================
 
 PyLovelace is a Python protection tool that can be used to protect
 Python source code from being reverse engineered.
 
@@ -44,8 +44,8 @@
 PyLovelace supports Python 3.11 with 3.10 and 3.12 support coming soon.
 Windows only for now.
 
 More information
 ----------------
 - PyLovelace on PyPI: https://pypi.org/project/pylovelace/
 - PyLovelace on GitHub: https://github.com/pylovelace/pylovelace
-- PyLovelace documentation: https://pylovelace.com/docs/
+- PyLovelace documentation: https://pylovelace.com/docs/getting-started/introduction
```

