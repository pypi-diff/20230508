# Comparing `tmp/security_scanner-0.0.2.tar.gz` & `tmp/security_scanner-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security_scanner-0.0.2.tar", last modified: Mon May  8 17:58:16 2023, max compression
+gzip compressed data, was "security_scanner-0.1.0.tar", last modified: Mon May  8 18:17:25 2023, max compression
```

## Comparing `security_scanner-0.0.2.tar` & `security_scanner-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.327546 security_scanner-0.0.2/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.0.2/LICENSE
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 17:58:16.327425 security_scanner-0.0.2/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.0.2/README.md
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.325640 security_scanner-0.0.2/app/
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.326367 security_scanner-0.0.2/app/security_scanner/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.0.2/app/security_scanner/__init__.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.327216 security_scanner-0.0.2/app/security_scanner/src/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.0.2/app/security_scanner/src/__init__.py
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3945 2023-05-08 15:56:12.000000 security_scanner-0.0.2/app/security_scanner/src/security_scanner.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.326991 security_scanner-0.0.2/app/security_scanner.egg-info/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/requires.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/top_level.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 17:58:16.327592 security_scanner-0.0.2/setup.cfg
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 17:57:51.000000 security_scanner-0.0.2/setup.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.309876 security_scanner-0.1.0/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.1.0/LICENSE
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 18:17:25.309750 security_scanner-0.1.0/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.1.0/README.md
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.307878 security_scanner-0.1.0/app/
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.308631 security_scanner-0.1.0/app/security_scanner/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.1.0/app/security_scanner/__init__.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.309529 security_scanner-0.1.0/app/security_scanner/src/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.1.0/app/security_scanner/src/__init__.py
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3927 2023-05-08 18:16:00.000000 security_scanner-0.1.0/app/security_scanner/src/security_scanner.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.309298 security_scanner-0.1.0/app/security_scanner.egg-info/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/requires.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/top_level.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 18:17:25.309918 security_scanner-0.1.0/setup.cfg
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 18:17:20.000000 security_scanner-0.1.0/setup.py
```

### Comparing `security_scanner-0.0.2/LICENSE` & `security_scanner-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `security_scanner-0.0.2/PKG-INFO` & `security_scanner-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security_scanner
-Version: 0.0.2
+Version: 0.1.0
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `security_scanner-0.0.2/app/security_scanner/src/security_scanner.py` & `security_scanner-0.1.0/app/security_scanner/src/security_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Password/passphrase strength and health checker
 """
 
 import datetime
 import getpass
 import hashlib
+import string
 import subprocess
 
 import httpx
 
 
 def check_password_strength(password: str) -> bool:
     """Check password strength.
@@ -31,16 +32,15 @@
         return False
 
     # Password should contain at least one digit
     if not any(char.isdigit() for char in password):
         return False
 
     # Password should contain at least one special character
-    special_chars = "!@#$%^&*()_+-="
-    if not any(char in special_chars for char in password):
+    if not any(char in string.punctuation for char in password):
         return False
 
     # Password is strong
     return True
 
 
 def check_uniqueness(password: str) -> bool:
```

### Comparing `security_scanner-0.0.2/app/security_scanner.egg-info/PKG-INFO` & `security_scanner-0.1.0/app/security_scanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security-scanner
-Version: 0.0.2
+Version: 0.1.0
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `security_scanner-0.0.2/setup.py` & `security_scanner-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="security_scanner",
-    version="0.0.2",
+    version="0.1.0",
     description="Password/passphrase strength and health checker",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheNewThinkTank/security-scanner",
     author="TheNewThinkTank",
```

