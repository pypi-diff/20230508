# Comparing `tmp/ftdz_from_fyh1-1.0.0.tar.gz` & `tmp/ftdz_from_fyh1-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ftdz_from_fyh1-1.0.0.tar", last modified: Sun May  7 01:48:59 2023, max compression
+gzip compressed data, was "dist\ftdz_from_fyh1-1.0.1.tar", last modified: Mon May  8 11:46:19 2023, max compression
```

## Comparing `ftdz_from_fyh1-1.0.0.tar` & `ftdz_from_fyh1-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/
--rw-rw-rw-   0        0        0      408 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_from_fyh1-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1/
--rw-rw-rw-   0        0        0     9788 2023-05-07 01:45:03.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1/__init__.py
--rw-rw-rw-   0        0        0    22195 2023-04-23 11:38:18.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1/main.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1.egg-info/
--rw-rw-rw-   0        0        0      408 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/ftdz_from_fyh1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 01:48:59.000000 ftdz_from_fyh1-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      518 2023-05-07 01:48:05.000000 ftdz_from_fyh1-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/
+-rw-rw-rw-   0        0        0      408 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_from_fyh1-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/
+-rw-rw-rw-   0        0        0     9803 2023-05-08 11:44:53.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/__init__.py
+-rw-rw-rw-   0        0        0    22195 2023-04-23 11:38:18.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      518 2023-05-08 11:45:19.000000 ftdz_from_fyh1-1.0.1/setup.py
```

### Comparing `ftdz_from_fyh1-1.0.0/ftdz_from_fyh1/__init__.py` & `ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,8 +189,8 @@
     res = requests.get(url, headers=head)
     with open("关.png", "wb") as file:
     #TODO 修改要写入的内容
         file.write(res.content)
     print("下载完毕")
     time.sleep(3)
 finally:
-    import main
+    import ftdz_from_fyh1.main
```

### Comparing `ftdz_from_fyh1-1.0.0/ftdz_from_fyh1/main.py` & `ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/main.py`

 * *Files identical despite different names*

### Comparing `ftdz_from_fyh1-1.0.0/setup.py` & `ftdz_from_fyh1-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
     name='ftdz_from_fyh1',
-    version='1.0.0',
+    version='1.0.1',
     author='bob',
     author_email='56141537@qq.com',
     description='A game.',
     long_description_content_type="""text/markdown""",
     url='https://www.github.com/',
     packages=['ftdz_from_fyh1'],
     install_requires=['pygame','requests'],
```

