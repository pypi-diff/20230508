# Comparing `tmp/security_scanner-0.1.2.tar.gz` & `tmp/security_scanner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security_scanner-0.1.2.tar", last modified: Mon May  8 18:30:37 2023, max compression
+gzip compressed data, was "security_scanner-0.1.3.tar", last modified: Mon May  8 18:36:42 2023, max compression
```

## Comparing `security_scanner-0.1.2.tar` & `security_scanner-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:30:37.072932 security_scanner-0.1.2/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.1.2/LICENSE
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1401 2023-05-08 18:30:37.072810 security_scanner-0.1.2/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.1.2/README.md
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:30:37.070913 security_scanner-0.1.2/app/
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:30:37.071725 security_scanner-0.1.2/app/security_scanner/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.1.2/app/security_scanner/__init__.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:30:37.072590 security_scanner-0.1.2/app/security_scanner/src/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.1.2/app/security_scanner/src/__init__.py
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3927 2023-05-08 18:16:00.000000 security_scanner-0.1.2/app/security_scanner/src/security_scanner.py
-drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:30:37.072355 security_scanner-0.1.2/app/security_scanner.egg-info/
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1401 2023-05-08 18:30:37.000000 security_scanner-0.1.2/app/security_scanner.egg-info/PKG-INFO
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 18:30:37.000000 security_scanner-0.1.2/app/security_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 18:30:37.000000 security_scanner-0.1.2/app/security_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 18:30:37.000000 security_scanner-0.1.2/app/security_scanner.egg-info/requires.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 18:30:37.000000 security_scanner-0.1.2/app/security_scanner.egg-info/top_level.txt
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 18:30:37.072984 security_scanner-0.1.2/setup.cfg
--rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 18:30:28.000000 security_scanner-0.1.2/setup.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:36:42.348328 security_scanner-0.1.3/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1073 2023-05-08 15:57:53.000000 security_scanner-0.1.3/LICENSE
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1401 2023-05-08 18:36:42.348188 security_scanner-0.1.3/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       67 2023-05-08 15:57:53.000000 security_scanner-0.1.3/README.md
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:36:42.345342 security_scanner-0.1.3/app/
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:36:42.346063 security_scanner-0.1.3/app/security_scanner/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      158 2023-05-08 16:45:55.000000 security_scanner-0.1.3/app/security_scanner/__init__.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:36:42.347946 security_scanner-0.1.3/app/security_scanner/src/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 16:46:53.000000 security_scanner-0.1.3/app/security_scanner/src/__init__.py
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     3848 2023-05-08 18:35:12.000000 security_scanner-0.1.3/app/security_scanner/src/security_scanner.py
+drwxr-xr-x   0 gustavcollinrasmussen   (501) staff       (20)        0 2023-05-08 18:36:42.347711 security_scanner-0.1.3/app/security_scanner.egg-info/
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)     1401 2023-05-08 18:36:42.000000 security_scanner-0.1.3/app/security_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      360 2023-05-08 18:36:42.000000 security_scanner-0.1.3/app/security_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)        1 2023-05-08 18:36:42.000000 security_scanner-0.1.3/app/security_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       45 2023-05-08 18:36:42.000000 security_scanner-0.1.3/app/security_scanner.egg-info/requires.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       17 2023-05-08 18:36:42.000000 security_scanner-0.1.3/app/security_scanner.egg-info/top_level.txt
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)       38 2023-05-08 18:36:42.348376 security_scanner-0.1.3/setup.cfg
+-rw-r--r--   0 gustavcollinrasmussen   (501) staff       (20)      870 2023-05-08 18:36:25.000000 security_scanner-0.1.3/setup.py
```

### Comparing `security_scanner-0.1.2/LICENSE` & `security_scanner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `security_scanner-0.1.2/PKG-INFO` & `security_scanner-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security_scanner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `security_scanner-0.1.2/app/security_scanner/src/security_scanner.py` & `security_scanner-0.1.3/app/security_scanner/src/security_scanner.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     :return: _description_
     :rtype: bool
     """
 
     sha1_password = hashlib.sha1(password.encode("utf-8")).hexdigest().upper()
     prefix, suffix = sha1_password[:5], sha1_password[5:]
     url = f"https://api.pwnedpasswords.com/range/{prefix}"
-    response = httpx.get(url)  # requests.get(url)
+    response = httpx.get(url)
     if response.status_code == 200:
         hashes = (line.split(":") for line in response.text.splitlines())
         count = next((int(count) for suffix_hash, count in hashes if suffix_hash == suffix), 0)
         if count > 0:
             return False
     
     # Password is unique
@@ -112,20 +112,19 @@
     else:
         # Password rotation is not activated
         return False
 
 
 if __name__ == "__main__":
 
-    # password = input("Enter password: ")
     password = getpass.getpass(prompt='Enter password: ')
 
     if not check_password_strength(password):
         print("Password is weak")
-    # elif not check_uniqueness(password):
-    #     print("Password is not unique")
+    elif not check_uniqueness(password):
+        print("Password is not unique")
     # elif not check_membership_in_rainbow_tables(password):
     #     print("Password is in rainbow tables")
-    # elif not check_rotation_activated(datetime.date(2023, 4, 7), 32):
-    #     print("Screen rotation is not activated")
+    elif not check_rotation_activated(datetime.date(2023, 4, 7), 32):
+        print("rotation is not activated")
     else:
         print("Password is strong and unique, and screen rotation is activated")
```

### Comparing `security_scanner-0.1.2/app/security_scanner.egg-info/PKG-INFO` & `security_scanner-0.1.3/app/security_scanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security-scanner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Password/passphrase strength and health checker
 Home-page: https://github.com/TheNewThinkTank/security-scanner
 Author: TheNewThinkTank
 Author-email: gcr84@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `security_scanner-0.1.2/setup.py` & `security_scanner-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="security_scanner",
-    version="0.1.2",
+    version="0.1.3",
     description="Password/passphrase strength and health checker",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheNewThinkTank/security-scanner",
     author="TheNewThinkTank",
```

