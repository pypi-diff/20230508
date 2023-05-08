# Comparing `tmp/varbox-2.3.tar.gz` & `tmp/varbox-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varbox-2.3.tar", last modified: Mon May  8 17:25:32 2023, max compression
+gzip compressed data, was "varbox-3.0.tar", last modified: Mon May  8 17:34:46 2023, max compression
```

## Comparing `varbox-2.3.tar` & `varbox-3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:25:32.468075 varbox-2.3/
--rw-rw-rw-   0        0        0      479 2023-05-08 17:25:32.468075 varbox-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2023-05-08 17:24:27.000000 varbox-2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 17:25:32.468075 varbox-2.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-05-08 17:25:15.000000 varbox-2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:25:32.425320 varbox-2.3/varbox/
--rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-2.3/varbox/cipher.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:25:32.440932 varbox-2.3/varbox/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:25:32.000000 varbox-2.3/varbox/constants/__init__.py
--rw-rw-rw-   0        0        0       53 2023-04-21 16:13:39.000000 varbox-2.3/varbox/constants/encryptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:25:32.440932 varbox-2.3/varbox/encryption/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:19:17.000000 varbox-2.3/varbox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1161 2023-04-21 16:56:55.000000 varbox-2.3/varbox/encryption/aes_encryption.py
--rw-rw-rw-   0        0        0      947 2023-04-21 16:33:26.000000 varbox-2.3/varbox/encryption/arc4_encryption.py
--rw-rw-rw-   0        0        0     1472 2023-04-21 16:56:55.000000 varbox-2.3/varbox/encryption/blowfish_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:25:32.456559 varbox-2.3/varbox/varbox.egg-info/
--rw-rw-rw-   0        0        0      479 2023-05-08 17:25:32.000000 varbox-2.3/varbox/varbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-05-08 17:25:32.000000 varbox-2.3/varbox/varbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:25:32.000000 varbox-2.3/varbox/varbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 17:25:16.000000 varbox-2.3/varbox/varbox.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-05-08 17:25:32.000000 varbox-2.3/varbox/varbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       52 2023-05-08 17:25:32.000000 varbox-2.3/varbox/varbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4282 2023-05-08 16:33:32.000000 varbox-2.3/varbox/varbox.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:25:32.456559 varbox-2.3/varbox/varboxexceptions/
--rw-rw-rw-   0        0        0        0 2023-04-20 18:53:13.000000 varbox-2.3/varbox/varboxexceptions/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-20 18:58:12.000000 varbox-2.3/varbox/varboxexceptions/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:34:46.228789 varbox-3.0/
+-rw-rw-rw-   0        0        0     2738 2023-05-08 17:34:46.228789 varbox-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2023-05-08 17:24:27.000000 varbox-3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:34:46.228789 varbox-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-05-08 17:34:09.000000 varbox-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:34:46.197542 varbox-3.0/varbox/
+-rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-3.0/varbox/cipher.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:34:46.197542 varbox-3.0/varbox/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 14:25:32.000000 varbox-3.0/varbox/constants/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-04-21 16:13:39.000000 varbox-3.0/varbox/constants/encryptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:34:46.213166 varbox-3.0/varbox/encryption/
+-rw-rw-rw-   0        0        0        0 2023-04-21 14:19:17.000000 varbox-3.0/varbox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1161 2023-04-21 16:56:55.000000 varbox-3.0/varbox/encryption/aes_encryption.py
+-rw-rw-rw-   0        0        0      947 2023-04-21 16:33:26.000000 varbox-3.0/varbox/encryption/arc4_encryption.py
+-rw-rw-rw-   0        0        0     1472 2023-04-21 16:56:55.000000 varbox-3.0/varbox/encryption/blowfish_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:34:46.228789 varbox-3.0/varbox/varbox.egg-info/
+-rw-rw-rw-   0        0        0     2738 2023-05-08 17:34:45.000000 varbox-3.0/varbox/varbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-05-08 17:34:46.000000 varbox-3.0/varbox/varbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:34:45.000000 varbox-3.0/varbox/varbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 17:34:25.000000 varbox-3.0/varbox/varbox.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-05-08 17:34:45.000000 varbox-3.0/varbox/varbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       52 2023-05-08 17:34:45.000000 varbox-3.0/varbox/varbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4282 2023-05-08 16:33:32.000000 varbox-3.0/varbox/varbox.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:34:46.228789 varbox-3.0/varbox/varboxexceptions/
+-rw-rw-rw-   0        0        0        0 2023-04-20 18:53:13.000000 varbox-3.0/varbox/varboxexceptions/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-20 18:58:12.000000 varbox-3.0/varbox/varboxexceptions/exception.py
```

### Comparing `varbox-2.3/README.md` & `varbox-3.0/README.md`

 * *Files identical despite different names*

### Comparing `varbox-2.3/setup.py` & `varbox-3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='varbox',
-    version='2.3',
+    version='3.0',
     description='varbox package can be used to dump and load multiple variables through local file and can also be used as encryption vault',
     author= 'Aman Anand',
+    long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='amananandofficials@gmail.com',
     keywords=['varbox dump', 'varbox load', 'varbox pickle load', 'varbox pickle dump','varbox','variable dump','encryption',"encryptor"],
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.8.8',
```

### Comparing `varbox-2.3/varbox/cipher.py` & `varbox-3.0/varbox/cipher.py`

 * *Files identical despite different names*

### Comparing `varbox-2.3/varbox/encryption/aes_encryption.py` & `varbox-3.0/varbox/encryption/aes_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-2.3/varbox/encryption/arc4_encryption.py` & `varbox-3.0/varbox/encryption/arc4_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-2.3/varbox/encryption/blowfish_encryption.py` & `varbox-3.0/varbox/encryption/blowfish_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-2.3/varbox/varbox.egg-info/SOURCES.txt` & `varbox-3.0/varbox/varbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `varbox-2.3/varbox/varbox.py` & `varbox-3.0/varbox/varbox.py`

 * *Files identical despite different names*

