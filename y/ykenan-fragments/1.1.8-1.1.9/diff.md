# Comparing `tmp/ykenan_fragments-1.1.8.tar.gz` & `tmp/ykenan_fragments-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.1.8.tar", last modified: Mon May  8 04:15:03 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.1.9.tar", last modified: Mon May  8 06:17:26 2023, max compression
```

## Comparing `ykenan_fragments-1.1.8.tar` & `ykenan_fragments-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 04:15:03.944393 ykenan_fragments-1.1.8/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      964 2023-05-08 04:15:03.944393 ykenan_fragments-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.8/README.md
--rw-rw-rw-   0        0        0      773 2023-05-08 04:13:56.000000 ykenan_fragments-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 04:15:03.944393 ykenan_fragments-1.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 04:15:03.912685 ykenan_fragments-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 04:15:03.926271 ykenan_fragments-1.1.8/src/ykenan_fragments/
--rw-rw-rw-   0        0        0    33708 2023-05-08 04:13:10.000000 ykenan_fragments-1.1.8/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3186 2023-05-08 04:13:10.000000 ykenan_fragments-1.1.8/src/ykenan_fragments/genome_transformation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 04:15:03.944393 ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      964 2023-05-08 04:15:03.000000 ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-05-08 04:15:03.000000 ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 04:15:03.000000 ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-08 04:15:03.000000 ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 04:15:03.000000 ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 06:17:26.040586 ykenan_fragments-1.1.9/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      964 2023-05-08 06:17:26.040586 ykenan_fragments-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.9/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-08 06:03:48.000000 ykenan_fragments-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:17:26.040586 ykenan_fragments-1.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 06:17:26.002065 ykenan_fragments-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 06:17:26.023586 ykenan_fragments-1.1.9/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0    33896 2023-05-08 06:03:48.000000 ykenan_fragments-1.1.9/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-05-08 06:03:48.000000 ykenan_fragments-1.1.9/src/ykenan_fragments/genome_transformation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:17:26.039585 ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-05-08 06:17:25.000000 ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-08 06:17:25.000000 ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 06:17:25.000000 ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-08 06:17:25.000000 ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 06:17:25.000000 ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.1.8/LICENSE` & `ykenan_fragments-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.8/PKG-INFO` & `ykenan_fragments-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.1.8
+Version: 1.1.9
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.1.8/pyproject.toml` & `ykenan_fragments-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.1.8/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.1.9/src/ykenan_fragments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import itertools
 import os
 import shutil
+from multiprocessing.pool import ThreadPool
 from typing import TextIO
 
 import pandas as pd
 from pandas import DataFrame
 from ykenan_log import Logger
 import ykenan_file as yf
 import gzip
@@ -206,15 +207,15 @@
 
     def fragments_file_name(self, key: str) -> str:
         return f"{key}{self.suffix_fragments}"
 
     def information_file_name(self, key: str) -> str:
         return f"{key}{self.suffix_information}"
 
-    def write_fragments(self, param: str) -> None:
+    def write_fragments(self, param: list) -> None:
         """
         Form fragments file
         :return:
         """
         path: str = param[0]
         key: str = param[1]
         self.log.info(f"Process {key} related files (folders)")
@@ -326,36 +327,38 @@
         # Classify the types and place them in different folders
         source_files: dict = self.handler_source_files()
         no_finish_infor = source_files["no_finish"]
         no_finish_keys = no_finish_infor["key"]
         no_finish_paths = no_finish_infor["path"]
         self.log.info(f"Related file information {no_finish_keys}, {no_finish_paths}")
         # 参数信息
-        write_fragments_param_list = []
+        write_fragments_param_list: list = []
         for key in no_finish_keys:
             write_fragments_param_list.append((no_finish_paths[key], key))
         # 实例化线程对象
-        pool = Pool(10)
+        pool: ThreadPool = Pool(10)
         # Form fragments file
         pool.map(self.write_fragments, write_fragments_param_list)
         pool.close()
+        pool.join()
 
         # All information
         all_infor = source_files["all"]
         all_infor_keys = all_infor["key"]
         all_infor_paths = all_infor["path"]
         # 参数信息
         cp_files_param_list = []
         for key in all_infor_keys:
             cp_files_param_list.append((all_infor_paths[key], key))
         # 实例化线程对象
-        pool = Pool(10)
+        pool: ThreadPool = Pool(10)
         # copy file
         pool.map(self.cp_files, cp_files_param_list)
         pool.close()
+        pool.join()
 
 
 class GetChrSortFragments:
 
     def __init__(self, path: str, cp_path: str, gsm: str, get_fragments_path: str, lift_over_path: str, is_hg19_to_hg38: bool = True, is_exec: bool = True):
         """
         Form an fragments
@@ -551,18 +554,19 @@
             for chr_ in chr_name:
                 position_file: str = os.path.join(position, f"{file}_{chr_}.tsv")
                 position_f_path = dict(itertools.chain(position_f_path.items(), {
                     chr_: position_file
                 }.items()))
                 sort_position_files_core_param_list.append((position, file_dict_path, chr_, file))
             # 实例化线程对象
-            pool = Pool(10)
+            pool: ThreadPool = Pool(10)
             # Form fragments file
             pool.map(self.sort_position_files_core, sort_position_files_core_param_list)
             pool.close()
+            pool.join()
         else:
             for chr_ in chr_name:
                 position_file: str = os.path.join(position, f"{file}_{chr_}.tsv")
                 position_f_path = dict(itertools.chain(position_f_path.items(), {
                     chr_: position_file
                 }.items()))
         return {
@@ -655,18 +659,19 @@
                     self.log.warn(f"{chr_sort_fragments_file_source}. The file already exists, it has been processed by default")
                     continue
 
             # 添加参数
             param_list.append((files_path, file, chr_sort_fragments_file, chr_sort_fragments_file_source))
 
         # 实例化线程对象
-        pool = Pool(10)
+        pool: ThreadPool = Pool(10)
         # Form fragments file
         pool.map(self.chr_sort_fragments_file_core, param_list)
         pool.close()
+        pool.join()
 
 
 class Run:
 
     def __init__(self, path: str, lift_over_path: str = None, is_hg19_to_hg38: bool = True):
         self.base_path: str = os.path.join(path, "handler")
         self.source_path: str = os.path.join(path, "source")
```

### Comparing `ykenan_fragments-1.1.8/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.1.9/src/ykenan_fragments/genome_transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import os.path
 from multiprocessing.dummy import Pool
+from multiprocessing.pool import ThreadPool
+
 import ykenan_file as yf
 from ykenan_log import Logger
 
 
 class Hg19ToHg38:
     """
     该步骤需要去子系统中进入该路径执行进行执行
@@ -67,12 +69,13 @@
         code_list = []
         finish_files = self.file.get_files(path=self.output)
         for input_file in input_files:
             if input_file not in finish_files:
                 code_list.append(self.exec_str(input_file))
 
         # 实例化线程对象
-        pool = Pool(10)
+        pool: ThreadPool = Pool(10)
         # 将 list 的每一个元素传递给 pool_page(page) 处理
         pool.map(self.exec_command, code_list)
         # 关闭线程
         pool.close()
+        pool.join()
```

### Comparing `ykenan_fragments-1.1.8/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.1.9/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.1.8
+Version: 1.1.9
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

