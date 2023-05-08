# Comparing `tmp/TCLR-1.6.0.tar.gz` & `tmp/TCLR-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCLR-1.6.0.tar", last modified: Mon May  8 04:09:51 2023, max compression
+gzip compressed data, was "TCLR-1.7.0.tar", last modified: Mon May  8 04:12:29 2023, max compression
```

## Comparing `TCLR-1.6.0.tar` & `TCLR-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:09:51.186305 TCLR-1.6.0/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:09:51.186183 TCLR-1.6.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.6.0/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:09:51.185430 TCLR-1.6.0/TCLR/
--rw-r-----   0 jacob      (501) staff       (20)    34848 2023-05-08 04:07:47.000000 TCLR-1.6.0/TCLR/TCLRalgorithm.py
--rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.6.0/TCLR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:09:51.186014 TCLR-1.6.0/TCLR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-08 04:09:51.186347 TCLR-1.6.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-08 04:09:04.000000 TCLR-1.6.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:12:29.833837 TCLR-1.7.0/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:12:29.833691 TCLR-1.7.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.7.0/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:12:29.832704 TCLR-1.7.0/TCLR/
+-rw-r-----   0 jacob      (501) staff       (20)    34868 2023-05-08 04:12:08.000000 TCLR-1.7.0/TCLR/TCLRalgorithm.py
+-rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.7.0/TCLR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:12:29.833507 TCLR-1.7.0/TCLR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-08 04:12:29.833879 TCLR-1.7.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-08 04:12:23.000000 TCLR-1.7.0/setup.py
```

### Comparing `TCLR-1.6.0/PKG-INFO` & `TCLR-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.6.0
+Version: 1.7.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.6.0/README.md` & `TCLR-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `TCLR-1.6.0/TCLR/TCLRalgorithm.py` & `TCLR-1.7.0/TCLR/TCLRalgorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -762,13 +762,13 @@
         newRb = R2(subDataSetB[:, -2], subDataSetB[:, -1])
   
 
     if weight == False:
         R = (newRa + newRb) / 2
         return R
     elif weight == True:
-        weightRa = len(subDataSetA[:, -1]) / (subDataSetA[:, -1] + subDataSetB[:, -1])
-        weightRb = len(subDataSetB[:, -1]) / (subDataSetA[:, -1] + subDataSetB[:, -1])
+        weightRa = len(subDataSetA[:, -1]) / (len(subDataSetA[:, -1]) + len(subDataSetB[:, -1]))
+        weightRb = len(subDataSetB[:, -1]) / (len(subDataSetA[:, -1]) + len(subDataSetB[:, -1]))
         R = weightRa * newRa + weightRb * newRb
         return R
     else:
         print('Parameter error | weight')
```

### Comparing `TCLR-1.6.0/TCLR/__init__.py` & `TCLR-1.7.0/TCLR/__init__.py`

 * *Files identical despite different names*

### Comparing `TCLR-1.6.0/TCLR.egg-info/PKG-INFO` & `TCLR-1.7.0/TCLR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.6.0
+Version: 1.7.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.6.0/setup.py` & `TCLR-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='TCLR',  # 包名
-    version='1.6.0',  # 版本
+    version='1.7.0',  # 版本
     description="Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

