# Comparing `tmp/tybase-0.0.4.tar.gz` & `tmp/tybase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.0.4.tar", last modified: Mon May  8 08:47:49 2023, max compression
+gzip compressed data, was "tybase-0.0.5.tar", last modified: Mon May  8 08:52:20 2023, max compression
```

## Comparing `tybase-0.0.4.tar` & `tybase-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:47:49.845551 tybase-0.0.4/
--rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.4/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      624 2023-05-08 08:47:49.845273 tybase-0.0.4/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.0.4/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-08 08:47:49.845718 tybase-0.0.4/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)      793 2023-05-08 08:47:07.000000 tybase-0.0.4/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:47:49.817137 tybase-0.0.4/tybase/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.4/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:47:49.826736 tybase-0.0.4/tybase/baidu/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.0.4/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4126 2023-05-05 10:37:20.000000 tybase-0.0.4/tybase/baidu/kw_tool.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.4/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:47:49.837145 tybase-0.0.4/tybase/lc/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.0.4/tybase/lc/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2421 2023-05-08 08:46:18.000000 tybase-0.0.4/tybase/lc/eg1.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.4/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:47:49.826017 tybase-0.0.4/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      624 2023-05-08 08:47:48.000000 tybase-0.0.4/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      323 2023-05-08 08:47:49.000000 tybase-0.0.4/tybase.egg-info/SOURCES.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-05-08 08:47:48.000000 tybase-0.0.4/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)       20 2023-05-08 08:47:49.000000 tybase-0.0.4/tybase.egg-info/requires.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-05-08 08:47:49.000000 tybase-0.0.4/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.863182 tybase-0.0.5/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.5/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      624 2023-05-08 08:52:20.862877 tybase-0.0.5/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.0.5/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-08 08:52:20.863308 tybase-0.0.5/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      793 2023-05-08 08:52:12.000000 tybase-0.0.5/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.836342 tybase-0.0.5/tybase/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.5/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.839189 tybase-0.0.5/tybase/baidu/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.0.5/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4126 2023-05-05 10:37:20.000000 tybase-0.0.5/tybase/baidu/kw_tool.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.5/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.854578 tybase-0.0.5/tybase/lc/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.0.5/tybase/lc/__init__.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2421 2023-05-08 08:46:18.000000 tybase-0.0.5/tybase/lc/eg1.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.5/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-08 08:52:20.838543 tybase-0.0.5/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      624 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      323 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       20 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/requires.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-05-08 08:52:20.000000 tybase-0.0.5/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.0.4/PKG-INFO` & `tybase-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.0.4
+Version: 0.0.5
 Summary: 新增lc.eg1,用于协助llm生成prompt
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tybase-0.0.4/setup.py` & `tybase-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.0.4',
+    version='0.0.5',
     include_package_data=True,
     description='新增lc.eg1,用于协助llm生成prompt',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
```

### Comparing `tybase-0.0.4/tybase/baidu/kw_tool.py` & `tybase-0.0.5/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.0.4/tybase/lc/eg1.py` & `tybase-0.0.5/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.0.4/tybase.egg-info/PKG-INFO` & `tybase-0.0.5/tybase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.0.4
+Version: 0.0.5
 Summary: 新增lc.eg1,用于协助llm生成prompt
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

