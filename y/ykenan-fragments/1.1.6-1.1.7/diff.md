# Comparing `tmp/ykenan_fragments-1.1.6.tar.gz` & `tmp/ykenan_fragments-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.1.6.tar", last modified: Mon May  8 02:24:18 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.1.7.tar", last modified: Mon May  8 03:12:51 2023, max compression
```

## Comparing `ykenan_fragments-1.1.6.tar` & `ykenan_fragments-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.6/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      964 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.6/README.md
--rw-rw-rw-   0        0        0      773 2023-05-08 02:23:15.000000 ykenan_fragments-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.680630 ykenan_fragments-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.711881 ykenan_fragments-1.1.6/src/ykenan_fragments/
--rw-rw-rw-   0        0        0    33129 2023-05-08 02:23:00.000000 ykenan_fragments-1.1.6/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3185 2023-05-06 09:16:51.000000 ykenan_fragments-1.1.6/src/ykenan_fragments/genome_transformation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      964 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 03:12:51.269986 ykenan_fragments-1.1.7/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      964 2023-05-08 03:12:51.269986 ykenan_fragments-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.7/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-08 03:09:15.000000 ykenan_fragments-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 03:12:51.269986 ykenan_fragments-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 03:12:51.158532 ykenan_fragments-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 03:12:51.255479 ykenan_fragments-1.1.7/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0    33706 2023-05-08 03:09:03.000000 ykenan_fragments-1.1.7/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3185 2023-05-06 09:16:51.000000 ykenan_fragments-1.1.7/src/ykenan_fragments/genome_transformation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 03:12:51.269986 ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-05-08 03:12:51.000000 ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-08 03:12:51.000000 ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 03:12:51.000000 ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-08 03:12:51.000000 ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 03:12:51.000000 ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.1.6/LICENSE` & `ykenan_fragments-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.6/PKG-INFO` & `ykenan_fragments-1.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.1.6
+Version: 1.1.7
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.1.6/pyproject.toml` & `ykenan_fragments-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.1.6/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.1.7/src/ykenan_fragments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -595,14 +595,36 @@
         self.log.info(f"Sorted file information {position_file_dict}")
         self.log.info(f"Sorting {file} group files completed")
         # 合并文件
         self.log.info(f"Start merging {file} grouped files")
         self.merge_chr_files(position_file_dict, fragments_file)
         self.log.info(f"Merge {file} group files completed")
 
+    def chr_sort_fragments_file_core(self, param_list: list):
+        # 参数信息
+        files_path: dict = param_list[0]
+        file: str = param_list[1]
+        chr_sort_fragments_file: dict = param_list[2]
+        chr_sort_fragments_file_source: str = param_list[3]
+
+        self.log.info(f"Start to group {file} files according to chromatin information")
+        chr_file_dict: dict = self.write_chr_file(files_path[file], file)
+        self.log.info(f"File information after grouping {chr_file_dict}")
+        self.log.info(f"Complete file grouping of {file} according to chromatin information")
+
+        # 判断是否需要进行 liftOver
+        if self.lift_over_path:
+            # 进行转化为 hg19 或 hg38
+            genome_transformation_dict: dict = self.genome_transformation(chr_file_dict, file)
+            genome_list: list = list(genome_transformation_dict.keys())
+            for genome in genome_list:
+                self.after_two_step(file, genome_transformation_dict[genome], chr_sort_fragments_file[genome])
+        else:
+            self.after_two_step(file, chr_file_dict, chr_sort_fragments_file_source)
+
     def exec_sort_fragments(self) -> None:
         files_dict: dict = self.get_files()
         files_name: list = files_dict["name"]
         files_path: dict = files_dict["path"]
 
         # 创建文件夹
         cp_input_path_genome_source = os.path.join(self.cp_input_path, self.genome_source)
@@ -610,14 +632,15 @@
         if not cp_input_path_genome_source:
             self.log.info(f"创建 {cp_input_path_genome_source} 文件夹")
             os.makedirs(cp_input_path_genome_source)
         if not cp_input_path_genome_generate:
             self.log.info("")
             self.log.info(f"创建 {cp_input_path_genome_generate} 文件夹")
 
+        param_list: list = []
         for file in files_name:
             # output file
             chr_sort_fragments_file_source: str = os.path.join(cp_input_path_genome_source, file)
             chr_sort_fragments_file_generate: str = os.path.join(cp_input_path_genome_source, file)
             chr_sort_fragments_file: dict = {
                 self.genome_source: cp_input_path_genome_source,
                 self.genome_generate: chr_sort_fragments_file_generate
@@ -628,28 +651,22 @@
                     self.log.warn(f"{chr_sort_fragments_file_source} and {chr_sort_fragments_file_generate}. The files already exists, it has been processed by default")
                     continue
             else:
                 if os.path.exists(chr_sort_fragments_file_source):
                     self.log.warn(f"{chr_sort_fragments_file_source}. The file already exists, it has been processed by default")
                     continue
 
-            self.log.info(f"Start to group {file} files according to chromatin information")
-            chr_file_dict: dict = self.write_chr_file(files_path[file], file)
-            self.log.info(f"File information after grouping {chr_file_dict}")
-            self.log.info(f"Complete file grouping of {file} according to chromatin information")
+            # 添加参数
+            param_list.append((files_path, file, chr_sort_fragments_file, chr_sort_fragments_file_source))
 
-            # 判断是否需要进行 liftOver
-            if self.lift_over_path:
-                # 进行转化为 hg19 或 hg38
-                genome_transformation_dict: dict = self.genome_transformation(chr_file_dict, file)
-                genome_list: list = list(genome_transformation_dict.keys())
-                for genome in genome_list:
-                    self.after_two_step(file, genome_transformation_dict[genome], chr_sort_fragments_file[genome])
-            else:
-                self.after_two_step(file, chr_file_dict, chr_sort_fragments_file_source)
+        # 实例化线程对象
+        pool = Pool(10)
+        # Form fragments file
+        pool.map(self.chr_sort_fragments_file_core, param_list)
+        pool.close()
 
 
 class Run:
 
     def __init__(self, path: str, lift_over_path: str = None, is_hg19_to_hg38: bool = True):
         self.base_path: str = os.path.join(path, "handler")
         self.source_path: str = os.path.join(path, "source")
```

### Comparing `ykenan_fragments-1.1.6/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.1.7/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.1.7/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.1.6
+Version: 1.1.7
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

