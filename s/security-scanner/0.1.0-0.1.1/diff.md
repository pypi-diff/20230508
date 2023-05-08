# Comparing `tmp/security_scanner-0.1.0.tar.gz` & `tmp/security_scanner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security_scanner-0.1.0.tar", last modified: Mon May  8 18:17:25 2023, max compression
+gzip compressed data, was "security_scanner-0.1.1.tar", last modified: Mon May  8 18:26:29 2023, max compression
```

## Comparing `security_scanner-0.1.0.tar` & `security_scanner-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.309876 security_scanner-0.1.0/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.1.0/LICENSE
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 18:17:25.309750 security_scanner-0.1.0/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.1.0/README.md
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.307878 security_scanner-0.1.0/app/
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.308631 security_scanner-0.1.0/app/security_scanner/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.1.0/app/security_scanner/__init__.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.309529 security_scanner-0.1.0/app/security_scanner/src/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.1.0/app/security_scanner/src/__init__.py
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3927 2023-05-08 18:16:00.000000 security_scanner-0.1.0/app/security_scanner/src/security_scanner.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:17:25.309298 security_scanner-0.1.0/app/security_scanner.egg-info/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/requires.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 18:17:25.000000 security_scanner-0.1.0/app/security_scanner.egg-info/top_level.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 18:17:25.309918 security_scanner-0.1.0/setup.cfg
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 18:17:20.000000 security_scanner-0.1.0/setup.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:26:29.362445 security_scanner-0.1.1/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.1.1/LICENSE
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1379 2023-05-08 18:26:29.362321 security_scanner-0.1.1/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.1.1/README.md
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:26:29.360494 security_scanner-0.1.1/app/
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:26:29.361265 security_scanner-0.1.1/app/security_scanner/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.1.1/app/security_scanner/__init__.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:26:29.362155 security_scanner-0.1.1/app/security_scanner/src/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.1.1/app/security_scanner/src/__init__.py
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3927 2023-05-08 18:16:00.000000 security_scanner-0.1.1/app/security_scanner/src/security_scanner.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:26:29.361925 security_scanner-0.1.1/app/security_scanner.egg-info/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1379 2023-05-08 18:26:29.000000 security_scanner-0.1.1/app/security_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 18:26:29.000000 security_scanner-0.1.1/app/security_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 18:26:29.000000 security_scanner-0.1.1/app/security_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 18:26:29.000000 security_scanner-0.1.1/app/security_scanner.egg-info/requires.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 18:26:29.000000 security_scanner-0.1.1/app/security_scanner.egg-info/top_level.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 18:26:29.362484 security_scanner-0.1.1/setup.cfg
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 18:26:07.000000 security_scanner-0.1.1/setup.py
```

### Comparing `security_scanner-0.1.0/LICENSE` & `security_scanner-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `security_scanner-0.1.0/PKG-INFO` & `security_scanner-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: security_scanner
-Version: 0.1.0
+Version: 0.1.1
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Security Scanner
-A package used to check the health of strength Password/passphrase.
+# Security Scanner
 
-How to use
+A package used to check the health and strength of passwords/passphrases.
+
+# How to use
 After installing the package use following import:
 
-from security_scanner import check_password_strength, check_uniqueness, check_membership_in_rainbow_tables, check_rotation_activated
+```Python
+from security_scanner import (check_password_strength, check_uniqueness, check_membership_in_rainbow_tables, check_rotation_activated)
+```
 
 Then use following commands:
 
 ```Python
 password = getpass.getpass(prompt='Enter password: ')
 
 if not check_password_strength(password):
```

### Comparing `security_scanner-0.1.0/app/security_scanner/src/security_scanner.py` & `security_scanner-0.1.1/app/security_scanner/src/security_scanner.py`

 * *Files identical despite different names*

### Comparing `security_scanner-0.1.0/app/security_scanner.egg-info/PKG-INFO` & `security_scanner-0.1.1/app/security_scanner.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: security-scanner
-Version: 0.1.0
+Version: 0.1.1
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Security Scanner
-A package used to check the health of strength Password/passphrase.
+# Security Scanner
 
-How to use
+A package used to check the health and strength of passwords/passphrases.
+
+# How to use
 After installing the package use following import:
 
-from security_scanner import check_password_strength, check_uniqueness, check_membership_in_rainbow_tables, check_rotation_activated
+```Python
+from security_scanner import (check_password_strength, check_uniqueness, check_membership_in_rainbow_tables, check_rotation_activated)
+```
 
 Then use following commands:
 
 ```Python
 password = getpass.getpass(prompt='Enter password: ')
 
 if not check_password_strength(password):
```

### Comparing `security_scanner-0.1.0/setup.py` & `security_scanner-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="security_scanner",
-    version="0.1.0",
+    version="0.1.1",
     description="Password/passphrase strength and health checker",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheNewThinkTank/security-scanner",
     author="TheNewThinkTank",
```

