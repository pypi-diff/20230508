# Comparing `tmp/varbox-1.2.tar.gz` & `tmp/varbox-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varbox-1.2.tar", last modified: Mon May  8 16:30:01 2023, max compression
+gzip compressed data, was "varbox-2.0.tar", last modified: Mon May  8 16:36:17 2023, max compression
```

## Comparing `varbox-1.2.tar` & `varbox-2.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 16:30:01.537179 varbox-1.2/
--rw-rw-rw-   0        0        0      438 2023-05-08 16:30:01.537179 varbox-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 16:30:01.537179 varbox-1.2/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-05-08 16:29:38.000000 varbox-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:30:01.483777 varbox-1.2/varbox/
--rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-1.2/varbox/cipher.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:30:01.490289 varbox-1.2/varbox/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:25:32.000000 varbox-1.2/varbox/constants/__init__.py
--rw-rw-rw-   0        0        0       53 2023-04-21 16:13:39.000000 varbox-1.2/varbox/constants/encryptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:30:01.505935 varbox-1.2/varbox/encryption/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:19:17.000000 varbox-1.2/varbox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1161 2023-04-21 16:56:55.000000 varbox-1.2/varbox/encryption/aes_encryption.py
--rw-rw-rw-   0        0        0      947 2023-04-21 16:33:26.000000 varbox-1.2/varbox/encryption/arc4_encryption.py
--rw-rw-rw-   0        0        0     1472 2023-04-21 16:56:55.000000 varbox-1.2/varbox/encryption/blowfish_encryption.py
--rw-rw-rw-   0        0        0      314 2023-05-08 15:53:32.000000 varbox-1.2/varbox/test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:30:01.521557 varbox-1.2/varbox/varbox.egg-info/
--rw-rw-rw-   0        0        0      438 2023-05-08 16:30:01.000000 varbox-1.2/varbox/varbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-05-08 16:30:01.000000 varbox-1.2/varbox/varbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 16:30:01.000000 varbox-1.2/varbox/varbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 16:29:39.000000 varbox-1.2/varbox/varbox.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-05-08 16:30:01.000000 varbox-1.2/varbox/varbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       57 2023-05-08 16:30:01.000000 varbox-1.2/varbox/varbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4271 2023-05-08 14:37:36.000000 varbox-1.2/varbox/varbox.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:30:01.521557 varbox-1.2/varbox/varboxexceptions/
--rw-rw-rw-   0        0        0        0 2023-04-20 18:53:13.000000 varbox-1.2/varbox/varboxexceptions/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-20 18:58:12.000000 varbox-1.2/varbox/varboxexceptions/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:36:17.472262 varbox-2.0/
+-rw-rw-rw-   0        0        0      438 2023-05-08 16:36:17.456637 varbox-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:36:17.472262 varbox-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-05-08 16:35:57.000000 varbox-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:36:17.425337 varbox-2.0/varbox/
+-rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-2.0/varbox/cipher.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:36:17.425337 varbox-2.0/varbox/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 14:25:32.000000 varbox-2.0/varbox/constants/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-04-21 16:13:39.000000 varbox-2.0/varbox/constants/encryptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:36:17.441041 varbox-2.0/varbox/encryption/
+-rw-rw-rw-   0        0        0        0 2023-04-21 14:19:17.000000 varbox-2.0/varbox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1161 2023-04-21 16:56:55.000000 varbox-2.0/varbox/encryption/aes_encryption.py
+-rw-rw-rw-   0        0        0      947 2023-04-21 16:33:26.000000 varbox-2.0/varbox/encryption/arc4_encryption.py
+-rw-rw-rw-   0        0        0     1472 2023-04-21 16:56:55.000000 varbox-2.0/varbox/encryption/blowfish_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:36:17.456637 varbox-2.0/varbox/varbox.egg-info/
+-rw-rw-rw-   0        0        0      438 2023-05-08 16:36:17.000000 varbox-2.0/varbox/varbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-05-08 16:36:17.000000 varbox-2.0/varbox/varbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:36:17.000000 varbox-2.0/varbox/varbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 16:35:58.000000 varbox-2.0/varbox/varbox.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-05-08 16:36:17.000000 varbox-2.0/varbox/varbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       52 2023-05-08 16:36:17.000000 varbox-2.0/varbox/varbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4282 2023-05-08 16:33:32.000000 varbox-2.0/varbox/varbox.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:36:17.456637 varbox-2.0/varbox/varboxexceptions/
+-rw-rw-rw-   0        0        0        0 2023-04-20 18:53:13.000000 varbox-2.0/varbox/varboxexceptions/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-20 18:58:12.000000 varbox-2.0/varbox/varboxexceptions/exception.py
```

### Comparing `varbox-1.2/setup.py` & `varbox-2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 import setuptools
 
 setup(
     name='varbox',
-    version='1.2',
+    version='2.0',
     description='varbox package can be used to dump and load multiple variables through local file and can also be used as encryption vault',
     author= 'Aman Anand',
     author_email='amananandofficials@gmail.com',
     keywords=['varbox dump', 'varbox load', 'varbox pickle load', 'varbox pickle dump','varbox','variable dump','encryption',"encryptor"],
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.8.8',
-    py_modules=['cipher','varbox','test'],
+    py_modules=['cipher','varbox'],
     package_dir={'':'varbox'},
     packages=['constants','encryption','varboxexceptions'],
     install_requires = [
         "pycryptodome==3.17"
     ],
     include_package_data=True,
     zip_safe=False
```

### Comparing `varbox-1.2/varbox/cipher.py` & `varbox-2.0/varbox/cipher.py`

 * *Files identical despite different names*

### Comparing `varbox-1.2/varbox/encryption/aes_encryption.py` & `varbox-2.0/varbox/encryption/aes_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-1.2/varbox/encryption/arc4_encryption.py` & `varbox-2.0/varbox/encryption/arc4_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-1.2/varbox/encryption/blowfish_encryption.py` & `varbox-2.0/varbox/encryption/blowfish_encryption.py`

 * *Files identical despite different names*

### Comparing `varbox-1.2/varbox/varbox.egg-info/SOURCES.txt` & `varbox-2.0/varbox/varbox.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 setup.py
 varbox/cipher.py
-varbox/test.py
 varbox/varbox.py
 varbox/constants/__init__.py
 varbox/constants/encryptions.py
 varbox/encryption/__init__.py
 varbox/encryption/aes_encryption.py
 varbox/encryption/arc4_encryption.py
 varbox/encryption/blowfish_encryption.py
```

### Comparing `varbox-1.2/varbox/varbox.py` & `varbox-2.0/varbox/varbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,10 +118,10 @@
     def set_amount(self,a):
         self.amount = a
     def get_amount(self):
         return self.amount
 
 g = Glass()
 varbox.dump(1, 2, 3, g, filepath="var_file_path", varnames=["a", "b", "c", "g"])
-k = varbox.load("ss")
+k = varbox.load("var_file_path")
 print(k["g"].amount)
 '''
```

