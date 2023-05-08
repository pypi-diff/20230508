# Comparing `tmp/captcha6-0.3.tar.gz` & `tmp/captcha6-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captcha6-0.3.tar", last modified: Sun May  7 19:26:08 2023, max compression
+gzip compressed data, was "captcha6-0.4.tar", last modified: Mon May  8 17:03:50 2023, max compression
```

## Comparing `captcha6-0.3.tar` & `captcha6-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 19:26:08.199348 captcha6-0.3/
--rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 captcha6-0.3/LICENSE
--rw-rw-rw-   0        0        0     1341 2023-05-07 19:26:08.197348 captcha6-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      772 2023-05-07 19:25:47.000000 captcha6-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 19:26:08.130344 captcha6-0.3/captcha6/
--rw-rw-rw-   0        0        0     1185 2023-05-07 18:34:49.000000 captcha6-0.3/captcha6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 19:26:08.194347 captcha6-0.3/captcha6.egg-info/
--rw-rw-rw-   0        0        0     1341 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 19:26:08.200349 captcha6-0.3/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-07 19:25:30.000000 captcha6-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:03:50.771563 captcha6-0.4/
+-rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 captcha6-0.4/LICENSE
+-rw-rw-rw-   0        0        0     1383 2023-05-08 17:03:50.768561 captcha6-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2023-05-08 17:02:17.000000 captcha6-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:03:50.483540 captcha6-0.4/captcha6/
+-rw-rw-rw-   0        0        0     1468 2023-05-08 17:00:44.000000 captcha6-0.4/captcha6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:03:50.765560 captcha6-0.4/captcha6.egg-info/
+-rw-rw-rw-   0        0        0     1383 2023-05-08 17:03:49.000000 captcha6-0.4/captcha6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-08 17:03:49.000000 captcha6-0.4/captcha6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:03:49.000000 captcha6-0.4/captcha6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-08 17:03:49.000000 captcha6-0.4/captcha6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 17:03:49.000000 captcha6-0.4/captcha6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:03:50.772562 captcha6-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-05-08 17:01:00.000000 captcha6-0.4/setup.py
```

### Comparing `captcha6-0.3/PKG-INFO` & `captcha6-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captcha6
-Version: 0.3
+Version: 0.4
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -56,9 +56,10 @@
 
 ----
 ## From here register on the site
 [Link](https://2captcha.io/auth-sign-in.php)
 
 ### The developer of this library
 #### 2captcha.io
+### https://2captcha.io/auth-sign-in.php
```

### Comparing `captcha6-0.3/README.md` & `captcha6-0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,9 +40,10 @@
 
 ----
 ## From here register on the site
 [Link](https://2captcha.io/auth-sign-in.php)
 
 ### The developer of this library
 #### 2captcha.io
+### https://2captcha.io/auth-sign-in.php
```

### Comparing `captcha6-0.3/captcha6.egg-info/PKG-INFO` & `captcha6-0.4/captcha6.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captcha6
-Version: 0.3
+Version: 0.4
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -56,9 +56,10 @@
 
 ----
 ## From here register on the site
 [Link](https://2captcha.io/auth-sign-in.php)
 
 ### The developer of this library
 #### 2captcha.io
+### https://2captcha.io/auth-sign-in.php
```

### Comparing `captcha6-0.3/setup.py` & `captcha6-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 # with open('requirements.txt','r') as fr:
 #     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='captcha6',
-    version="0.3",
+    version="0.4",
     author='omar Style',
     author_email='omarllStyle@gmail.com',
     description='Omar_Style _ 〄🇵🇸',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Omarail1/omarpoop.git',
     packages=['captcha6'],
```

