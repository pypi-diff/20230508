# Comparing `tmp/varbox-2.1.tar.gz` & `tmp/varbox-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varbox-2.1.tar", last modified: Mon May  8 17:10:53 2023, max compression
+gzip compressed data, was "varbox-2.2.tar", last modified: Mon May  8 17:21:03 2023, max compression
```

## Comparing `varbox-2.1.tar` & `varbox-2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:10:53.342642 varbox-2.1/
--rw-rw-rw-   0        0        0      479 2023-05-08 17:10:53.342642 varbox-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1958 2023-05-08 17:07:15.000000 varbox-2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 17:10:53.342642 varbox-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-05-08 17:10:09.000000 varbox-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:10:53.311381 varbox-2.1/varbox/
--rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-2.1/varbox/cipher.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:10:53.311381 varbox-2.1/varbox/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:25:32.000000 varbox-2.1/varbox/constants/__init__.py
--rw-rw-rw-   0        0        0       53 2023-04-21 16:13:39.000000 varbox-2.1/varbox/constants/encryptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:10:53.311381 varbox-2.1/varbox/encryption/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:19:17.000000 varbox-2.1/varbox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1161 2023-04-21 16:56:55.000000 varbox-2.1/varbox/encryption/aes_encryption.py
--rw-rw-rw-   0        0        0      947 2023-04-21 16:33:26.000000 varbox-2.1/varbox/encryption/arc4_encryption.py
--rw-rw-rw-   0        0        0     1472 2023-04-21 16:56:55.000000 varbox-2.1/varbox/encryption/blowfish_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:10:53.327016 varbox-2.1/varbox/varbox.egg-info/
--rw-rw-rw-   0        0        0      479 2023-05-08 17:10:53.000000 varbox-2.1/varbox/varbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-05-08 17:10:53.000000 varbox-2.1/varbox/varbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:10:53.000000 varbox-2.1/varbox/varbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 17:10:36.000000 varbox-2.1/varbox/varbox.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-05-08 17:10:53.000000 varbox-2.1/varbox/varbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       52 2023-05-08 17:10:53.000000 varbox-2.1/varbox/varbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4282 2023-05-08 16:33:32.000000 varbox-2.1/varbox/varbox.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:10:53.327016 varbox-2.1/varbox/varboxexceptions/
--rw-rw-rw-   0        0        0        0 2023-04-20 18:53:13.000000 varbox-2.1/varbox/varboxexceptions/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-20 18:58:12.000000 varbox-2.1/varbox/varboxexceptions/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:21:03.669666 varbox-2.2/
+-rw-rw-rw-   0        0        0      479 2023-05-08 17:21:03.669666 varbox-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2023-05-08 17:20:22.000000 varbox-2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:21:03.669666 varbox-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2023-05-08 17:20:34.000000 varbox-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:21:03.636273 varbox-2.2/varbox/
+-rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-2.2/varbox/cipher.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:21:03.638404 varbox-2.2/varbox/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 14:25:32.000000 varbox-2.2/varbox/constants/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-04-21 16:13:39.000000 varbox-2.2/varbox/constants/encryptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:21:03.638404 varbox-2.2/varbox/encryption/
+-rw-rw-rw-   0        0        0        0 2023-04-21 14:19:17.000000 varbox-2.2/varbox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1161 2023-04-21 16:56:55.000000 varbox-2.2/varbox/encryption/aes_encryption.py
+-rw-rw-rw-   0        0        0      947 2023-04-21 16:33:26.000000 varbox-2.2/varbox/encryption/arc4_encryption.py
+-rw-rw-rw-   0        0        0     1472 2023-04-21 16:56:55.000000 varbox-2.2/varbox/encryption/blowfish_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:21:03.669666 varbox-2.2/varbox/varbox.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-05-08 17:21:03.000000 varbox-2.2/varbox/varbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-05-08 17:21:03.000000 varbox-2.2/varbox/varbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:21:03.000000 varbox-2.2/varbox/varbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 17:10:36.000000 varbox-2.2/varbox/varbox.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-05-08 17:21:03.000000 varbox-2.2/varbox/varbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       52 2023-05-08 17:21:03.000000 varbox-2.2/varbox/varbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4282 2023-05-08 16:33:32.000000 varbox-2.2/varbox/varbox.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:21:03.669666 varbox-2.2/varbox/varboxexceptions/
+-rw-rw-rw-   0        0        0        0 2023-04-20 18:53:13.000000 varbox-2.2/varbox/varboxexceptions/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-20 18:58:12.000000 varbox-2.2/varbox/varboxexceptions/exception.py
```

### Comparing `varbox-2.1/README.md` & `varbox-2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Variable dumpper/encryptor 
+
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
+[![Python 3.8.8](https://img.shields.io/badge/python-3.8.8-blue.svg)](https://www.python.org/downloads/release/python-388/) 
+
 ## Example 1
 
  ```
 # test.py
 import varbox
 class Glass:
     def __init__(self):
```

### Comparing `varbox-2.1/setup.py` & `varbox-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='varbox',
-    version='2.1',
+    version='2.2',
     description='varbox package can be used to dump and load multiple variables through local file and can also be used as encryption vault',
     author= 'Aman Anand',
     long_description_content_type="text/markdown",
     author_email='amananandofficials@gmail.com',
     keywords=['varbox dump', 'varbox load', 'varbox pickle load', 'varbox pickle dump','varbox','variable dump','encryption',"encryptor"],
     classifiers=[
         "Programming Language :: Python :: 3"
```

### Comparing `varbox-2.1/varbox/cipher.py` & `varbox-2.2/varbox/cipher.py`

 * *Files identical despite different names*

### Comparing `varbox-2.1/varbox/encryption/aes_encryption.py` & `varbox-2.2/varbox/encryption/aes_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-2.1/varbox/encryption/arc4_encryption.py` & `varbox-2.2/varbox/encryption/arc4_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-2.1/varbox/encryption/blowfish_encryption.py` & `varbox-2.2/varbox/encryption/blowfish_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-2.1/varbox/varbox.egg-info/SOURCES.txt` & `varbox-2.2/varbox/varbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `varbox-2.1/varbox/varbox.py` & `varbox-2.2/varbox/varbox.py`

 * *Files identical despite different names*

