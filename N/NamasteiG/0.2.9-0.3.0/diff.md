# Comparing `tmp/NamasteiG-0.2.9.tar.gz` & `tmp/NamasteiG-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.2.9.tar", last modified: Mon May  8 08:02:45 2023, max compression
+gzip compressed data, was "NamasteiG-0.3.0.tar", last modified: Mon May  8 08:33:00 2023, max compression
```

## Comparing `NamasteiG-0.2.9.tar` & `NamasteiG-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.598854 NamasteiG-0.2.9/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      838 2023-05-08 08:02:45.598854 NamasteiG-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.9/README.md
--rw-rw-rw-   0        0        0      593 2023-05-08 07:59:00.000000 NamasteiG-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 08:02:45.599831 NamasteiG-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.578437 NamasteiG-0.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.589321 NamasteiG-0.2.9/src/NamasteiG/
--rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.2.9/src/NamasteiG/VerifyData.py
--rw-rw-rw-   0        0        0    27949 2023-05-08 07:58:45.000000 NamasteiG-0.2.9/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      501 2023-04-21 14:30:38.000000 NamasteiG-0.2.9/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:02:45.596832 NamasteiG-0.2.9/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-08 08:02:45.000000 NamasteiG-0.2.9/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.391506 NamasteiG-0.3.0/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-05-08 08:33:00.391506 NamasteiG-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.3.0/README.md
+-rw-rw-rw-   0        0        0      593 2023-05-08 08:32:44.000000 NamasteiG-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:33:00.393010 NamasteiG-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.376439 NamasteiG-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.383986 NamasteiG-0.3.0/src/NamasteiG/
+-rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.3.0/src/NamasteiG/VerifyData.py
+-rw-rw-rw-   0        0        0    27983 2023-05-08 08:32:23.000000 NamasteiG-0.3.0/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-04-21 14:30:38.000000 NamasteiG-0.3.0/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.390409 NamasteiG-0.3.0/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.2.9/LICENSE` & `NamasteiG-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.9/PKG-INFO` & `NamasteiG-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.9
+Version: 0.3.0
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.2.9/pyproject.toml` & `NamasteiG-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.2.9"
+version = "0.3.0"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.2.9/src/NamasteiG/VerifyData.py` & `NamasteiG-0.3.0/src/NamasteiG/VerifyData.py`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.9/src/NamasteiG/__init__.py` & `NamasteiG-0.3.0/src/NamasteiG/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,16 +374,17 @@
                     "IgDeviceId": self.IgDeviceId,
                     "IgFamilyDeviceId": self.IgFamilyDeviceId,
                     "AndroidID": self.AndroidID,
                     'UserAgent': self.UserAgent,
                     'BlockVersion': self.Blockversion
                 }
                 return value
-            except ConnectionError :
-                pass
+            except Exception as E :
+                print(E)
+                time.sleep(4)
     def head(self):
 
 
         headers = {
             'Host': 'i.instagram.com',
             'X-Ig-App-Locale': 'en_US',
             'X-Ig-Device-Locale': 'en_US',
```

### Comparing `NamasteiG-0.2.9/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.3.0/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.9
+Version: 0.3.0
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

