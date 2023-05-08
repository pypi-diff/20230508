# Comparing `tmp/security_scanner-0.0.1.tar.gz` & `tmp/security_scanner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security_scanner-0.0.1.tar", last modified: Mon May  8 17:49:43 2023, max compression
+gzip compressed data, was "security_scanner-0.0.2.tar", last modified: Mon May  8 17:58:16 2023, max compression
```

## Comparing `security_scanner-0.0.1.tar` & `security_scanner-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:49:43.169124 security_scanner-0.0.1/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.0.1/LICENSE
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1337 2023-05-08 17:49:43.169004 security_scanner-0.0.1/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.0.1/README.md
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:49:43.167159 security_scanner-0.0.1/app/
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:49:43.167867 security_scanner-0.0.1/app/security_scanner/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.0.1/app/security_scanner/__init__.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:49:43.168782 security_scanner-0.0.1/app/security_scanner/src/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.0.1/app/security_scanner/src/__init__.py
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3945 2023-05-08 15:56:12.000000 security_scanner-0.0.1/app/security_scanner/src/security_scanner.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:49:43.168525 security_scanner-0.0.1/app/security_scanner.egg-info/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1337 2023-05-08 17:49:43.000000 security_scanner-0.0.1/app/security_scanner.egg-info/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 17:49:43.000000 security_scanner-0.0.1/app/security_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 17:49:43.000000 security_scanner-0.0.1/app/security_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 17:49:43.000000 security_scanner-0.0.1/app/security_scanner.egg-info/requires.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 17:49:43.000000 security_scanner-0.0.1/app/security_scanner.egg-info/top_level.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 17:49:43.169163 security_scanner-0.0.1/setup.cfg
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 17:35:36.000000 security_scanner-0.0.1/setup.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.327546 security_scanner-0.0.2/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.0.2/LICENSE
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 17:58:16.327425 security_scanner-0.0.2/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.0.2/README.md
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.325640 security_scanner-0.0.2/app/
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.326367 security_scanner-0.0.2/app/security_scanner/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.0.2/app/security_scanner/__init__.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.327216 security_scanner-0.0.2/app/security_scanner/src/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.0.2/app/security_scanner/src/__init__.py
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3945 2023-05-08 15:56:12.000000 security_scanner-0.0.2/app/security_scanner/src/security_scanner.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 17:58:16.326991 security_scanner-0.0.2/app/security_scanner.egg-info/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1352 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/requires.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 17:58:16.000000 security_scanner-0.0.2/app/security_scanner.egg-info/top_level.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 17:58:16.327592 security_scanner-0.0.2/setup.cfg
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 17:57:51.000000 security_scanner-0.0.2/setup.py
```

### Comparing `security_scanner-0.0.1/LICENSE` & `security_scanner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `security_scanner-0.0.1/PKG-INFO` & `security_scanner-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security_scanner
-Version: 0.0.1
+Version: 0.0.2
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -20,19 +20,21 @@
 How to use
 After installing the package use following import:
 
 from security_scanner import check_password_strength, check_uniqueness, check_membership_in_rainbow_tables, check_rotation_activated
 
 Then use following commands:
 
+```Python
 password = getpass.getpass(prompt='Enter password: ')
 
 if not check_password_strength(password):
     print("Password is weak")
 elif not check_uniqueness(password):
     print("Password is not unique")
 elif not check_membership_in_rainbow_tables(password):
     print("Password is in rainbow tables")
 elif not check_rotation_activated(datetime.date(YEAR, MONTH, DAY), rotation_interval_days):
     print("Screen rotation is not activated")
 else:
     print("Password is strong and unique, and screen rotation is activated")
+````
```

### Comparing `security_scanner-0.0.1/app/security_scanner/src/security_scanner.py` & `security_scanner-0.0.2/app/security_scanner/src/security_scanner.py`

 * *Files identical despite different names*

### Comparing `security_scanner-0.0.1/app/security_scanner.egg-info/PKG-INFO` & `security_scanner-0.0.2/app/security_scanner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security-scanner
-Version: 0.0.1
+Version: 0.0.2
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -20,19 +20,21 @@
 How to use
 After installing the package use following import:
 
 from security_scanner import check_password_strength, check_uniqueness, check_membership_in_rainbow_tables, check_rotation_activated
 
 Then use following commands:
 
+```Python
 password = getpass.getpass(prompt='Enter password: ')
 
 if not check_password_strength(password):
     print("Password is weak")
 elif not check_uniqueness(password):
     print("Password is not unique")
 elif not check_membership_in_rainbow_tables(password):
     print("Password is in rainbow tables")
 elif not check_rotation_activated(datetime.date(YEAR, MONTH, DAY), rotation_interval_days):
     print("Screen rotation is not activated")
 else:
     print("Password is strong and unique, and screen rotation is activated")
+````
```

### Comparing `security_scanner-0.0.1/setup.py` & `security_scanner-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="security_scanner",
-    version="0.0.1",
+    version="0.0.2",
     description="Password/passphrase strength and health checker",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheNewThinkTank/security-scanner",
     author="TheNewThinkTank",
```

