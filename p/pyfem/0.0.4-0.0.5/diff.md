# Comparing `tmp/pyfem-0.0.4.tar.gz` & `tmp/pyfem-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.4.tar", last modified: Wed May  3 11:06:29 2023, max compression
+gzip compressed data, was "pyfem-0.0.5.tar", last modified: Mon May  8 13:34:44 2023, max compression
```

## Comparing `pyfem-0.0.4.tar` & `pyfem-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.916171 pyfem-0.0.4/
--rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      535 2023-05-03 11:06:29.915675 pyfem-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-05-03 09:58:16.000000 pyfem-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 11:06:29.916667 pyfem-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-05-03 11:05:46.000000 pyfem-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.876407 pyfem-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.888311 pyfem-0.0.4/src/pyfem/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      401 2023-05-03 10:54:29.000000 pyfem-0.0.4/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.898231 pyfem-0.0.4/src/pyfem/assembly/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.899719 pyfem-0.0.4/src/pyfem/elements/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.901704 pyfem-0.0.4/src/pyfem/fem/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/fem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.905175 pyfem-0.0.4/src/pyfem/io/
--rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.4/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-03 05:18:43.000000 pyfem-0.0.4/src/pyfem/io/arguments.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.909228 pyfem-0.0.4/src/pyfem/materials/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/materials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.910714 pyfem-0.0.4/src/pyfem/mesh/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.912203 pyfem-0.0.4/src/pyfem/solvers/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/solvers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.914187 pyfem-0.0.4/src/pyfem/utils/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.4/src/pyfem/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:06:29.896744 pyfem-0.0.4/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      535 2023-05-03 11:06:29.000000 pyfem-0.0.4/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2023-05-03 11:06:29.000000 pyfem-0.0.4/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:06:29.000000 pyfem-0.0.4/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-03 11:06:29.000000 pyfem-0.0.4/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 11:06:29.000000 pyfem-0.0.4/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.496315 pyfem-0.0.5/
+-rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      791 2023-05-08 13:34:44.495819 pyfem-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-04 10:59:11.000000 pyfem-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:34:44.496315 pyfem-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-05-08 13:33:22.000000 pyfem-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.429613 pyfem-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.443500 pyfem-0.0.5/src/pyfem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-05-06 15:26:11.000000 pyfem-0.0.5/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.453917 pyfem-0.0.5/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.455406 pyfem-0.0.5/src/pyfem/elements/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.460861 pyfem-0.0.5/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     2686 2023-05-06 15:26:11.000000 pyfem-0.0.5/src/pyfem/fem/ElementSet.py
+-rw-rw-rw-   0        0        0     3257 2023-05-06 15:26:11.000000 pyfem-0.0.5/src/pyfem/fem/NodeSet.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.478393 pyfem-0.0.5/src/pyfem/io/
+-rw-rw-rw-   0        0        0      572 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0      531 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/Dofs.py
+-rw-rw-rw-   0        0        0      548 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/Domain.py
+-rw-rw-rw-   0        0        0      551 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      501 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      518 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0     7577 2023-05-07 07:31:27.000000 pyfem-0.0.5/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      487 2023-05-07 05:33:53.000000 pyfem-0.0.5/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.5/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1334 2023-05-08 13:34:21.000000 pyfem-0.0.5/src/pyfem/io/arguments.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.481864 pyfem-0.0.5/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     1118 2023-05-07 08:34:39.000000 pyfem-0.0.5/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/materials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.483352 pyfem-0.0.5/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.484839 pyfem-0.0.5/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/solvers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.493835 pyfem-0.0.5/src/pyfem/utils/
+-rw-rw-rw-   0        0        0      450 2023-05-07 05:37:27.000000 pyfem-0.0.5/src/pyfem/utils/Constants.py
+-rw-rw-rw-   0        0        0     2259 2023-05-06 14:58:33.000000 pyfem-0.0.5/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0      311 2023-05-07 07:41:00.000000 pyfem-0.0.5/src/pyfem/utils/SolverStatus.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.5/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0     1516 2023-05-06 15:26:11.000000 pyfem-0.0.5/src/pyfem/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:34:44.451933 pyfem-0.0.5/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      791 2023-05-08 13:34:44.000000 pyfem-0.0.5/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      882 2023-05-08 13:34:44.000000 pyfem-0.0.5/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:34:44.000000 pyfem-0.0.5/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-08 13:34:44.000000 pyfem-0.0.5/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 13:34:44.000000 pyfem-0.0.5/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.4/LICENSE` & `pyfem-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.4/PKG-INFO` & `pyfem-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.4
+Version: 0.0.5
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
- 
+A finite element package in python.
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
```

### Comparing `pyfem-0.0.4/setup.py` & `pyfem-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.4",
+    version="0.0.5",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.0.4/src/pyfem/io/arguments.py` & `pyfem-0.0.5/src/pyfem/io/arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import argparse
 import sys
+from typing import Tuple
 
 
-def get_arguments() -> tuple[str, str, list[str]]:
+def get_arguments() -> Tuple[str, str, str]:
     # 创建一个 argparse 解析器对象
     parser = argparse.ArgumentParser(add_help=False)
 
     # 添加程序输入文件选项
     parser.add_argument('-i', metavar='input', type=str,
-                        help='Identify the input file name.')
+                        help='Identify the input file.')
 
     # 添加程序输出文件选项
     parser.add_argument('-o', metavar='output', type=str,
-                        help='Identify the output file name.')
+                        help='Identify the output file.')
 
     # 添加参数选项
-    parser.add_argument('-p', metavar='parameter', type=str, action='append',
-                        help='Parameters to pass to the program.')
+    parser.add_argument('-p', metavar='parameter', type=str,
+                        help='Parameter to pass to the program.')
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='%(prog)s 0.1')
+                        version='%(prog)s 0.0.5')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('error: the input file is required.')
```

### Comparing `pyfem-0.0.4/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.0.5/src/pyfem.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.4
+Version: 0.0.5
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
- 
+A finite element package in python.
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
```

