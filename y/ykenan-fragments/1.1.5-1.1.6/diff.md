# Comparing `tmp/ykenan_fragments-1.1.5.tar.gz` & `tmp/ykenan_fragments-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.1.5.tar", last modified: Sat May  6 12:23:00 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.1.6.tar", last modified: Mon May  8 02:24:18 2023, max compression
```

## Comparing `ykenan_fragments-1.1.5.tar` & `ykenan_fragments-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 12:23:00.378167 ykenan_fragments-1.1.5/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.5/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      964 2023-05-06 12:23:00.378167 ykenan_fragments-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.5/README.md
--rw-rw-rw-   0        0        0      773 2023-05-06 12:22:29.000000 ykenan_fragments-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 12:23:00.378167 ykenan_fragments-1.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 12:23:00.344990 ykenan_fragments-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:23:00.363169 ykenan_fragments-1.1.5/src/ykenan_fragments/
--rw-rw-rw-   0        0        0    32943 2023-05-06 12:22:06.000000 ykenan_fragments-1.1.5/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3185 2023-05-06 09:16:51.000000 ykenan_fragments-1.1.5/src/ykenan_fragments/genome_transformation.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:23:00.376195 ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      964 2023-05-06 12:23:00.000000 ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-05-06 12:23:00.000000 ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 12:23:00.000000 ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-06 12:23:00.000000 ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 12:23:00.000000 ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      964 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.6/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-08 02:23:15.000000 ykenan_fragments-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.680630 ykenan_fragments-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.711881 ykenan_fragments-1.1.6/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0    33129 2023-05-08 02:23:00.000000 ykenan_fragments-1.1.6/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3185 2023-05-06 09:16:51.000000 ykenan_fragments-1.1.6/src/ykenan_fragments/genome_transformation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 02:24:18.727507 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 02:24:18.000000 ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.1.5/LICENSE` & `ykenan_fragments-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.5/PKG-INFO` & `ykenan_fragments-1.1.6/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ykenan_fragments
-Version: 1.1.5
+Name: ykenan-fragments
+Version: 1.1.6
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.1.5/pyproject.toml` & `ykenan_fragments-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.1.5/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.1.6/src/ykenan_fragments/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,16 @@
         if not os.path.exists(fragments_cp_dir):
             self.log.info(f"create folder {fragments_cp_dir}")
             os.makedirs(fragments_cp_dir)
         # copy
         fragments_gz_file = os.path.join(fragments_cp_dir, f"{fragments_file_name}.gz")
         if os.path.exists(fragments_gz_file):
             self.log.warn(f"The file has been compressed into {fragments_gz_file}, Default copy completed")
+        elif os.path.exists(os.path.join(fragments_cp_dir, fragments_file_name)):
+            self.log.warn(f"The file has been copy into {fragments_gz_file}, Default copy completed")
         else:
             self.copy_file(fragments_file, os.path.join(fragments_cp_dir, fragments_file_name))
         self.log.info(f"Copy file to specified path for {key} completed")
 
     def exec_fragments(self):
         # Classify the types and place them in different folders
         source_files: dict = self.handler_source_files()
```

### Comparing `ykenan_fragments-1.1.5/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.1.6/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.5/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ykenan-fragments
-Version: 1.1.5
+Name: ykenan_fragments
+Version: 1.1.6
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

