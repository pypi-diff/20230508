# Comparing `tmp/iron_toolbox-1.0.8.tar.gz` & `tmp/iron_toolbox-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iron_toolbox-1.0.8.tar", last modified: Wed Apr 12 18:15:46 2023, max compression
+gzip compressed data, was "iron_toolbox-1.0.9.tar", last modified: Thu Apr 13 17:31:55 2023, max compression
```

## Comparing `iron_toolbox-1.0.8.tar` & `iron_toolbox-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 18:15:46.173829 iron_toolbox-1.0.8/
--rw-rw-rw-   0        0        0     1092 2023-03-16 21:06:41.000000 iron_toolbox-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      649 2023-04-12 18:15:46.173829 iron_toolbox-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-03-17 14:20:36.000000 iron_toolbox-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 18:15:46.164742 iron_toolbox-1.0.8/iron_toolbox/
--rw-rw-rw-   0        0        0      105 2023-03-16 23:27:50.000000 iron_toolbox-1.0.8/iron_toolbox/__init__.py
--rw-rw-rw-   0        0        0    15272 2023-04-05 12:40:46.000000 iron_toolbox-1.0.8/iron_toolbox/aws_functions.py
--rw-rw-rw-   0        0        0     1757 2023-03-16 23:27:50.000000 iron_toolbox-1.0.8/iron_toolbox/domo_functions.py
--rw-rw-rw-   0        0        0    24103 2023-02-23 20:09:35.000000 iron_toolbox-1.0.8/iron_toolbox/iron_functions.py
--rw-rw-rw-   0        0        0    64816 2023-04-12 18:15:15.000000 iron_toolbox-1.0.8/iron_toolbox/mongo_functions.py
--rw-rw-rw-   0        0        0     4325 2023-02-01 20:27:50.000000 iron_toolbox-1.0.8/iron_toolbox/sftp_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:15:46.171829 iron_toolbox-1.0.8/iron_toolbox.egg-info/
--rw-rw-rw-   0        0        0      649 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      222 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-12 18:15:46.175829 iron_toolbox-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1586 2023-04-12 18:15:15.000000 iron_toolbox-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:55.431354 iron_toolbox-1.0.9/
+-rw-rw-rw-   0        0        0     1092 2023-03-16 21:06:41.000000 iron_toolbox-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      649 2023-04-13 17:31:55.431354 iron_toolbox-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-03-17 14:20:36.000000 iron_toolbox-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:55.385443 iron_toolbox-1.0.9/iron_toolbox/
+-rw-rw-rw-   0        0        0      105 2023-03-16 23:27:50.000000 iron_toolbox-1.0.9/iron_toolbox/__init__.py
+-rw-rw-rw-   0        0        0    15272 2023-04-05 12:40:46.000000 iron_toolbox-1.0.9/iron_toolbox/aws_functions.py
+-rw-rw-rw-   0        0        0     1757 2023-03-16 23:27:50.000000 iron_toolbox-1.0.9/iron_toolbox/domo_functions.py
+-rw-rw-rw-   0        0        0    24103 2023-02-23 20:09:35.000000 iron_toolbox-1.0.9/iron_toolbox/iron_functions.py
+-rw-rw-rw-   0        0        0    65142 2023-04-13 17:30:58.000000 iron_toolbox-1.0.9/iron_toolbox/mongo_functions.py
+-rw-rw-rw-   0        0        0     4325 2023-02-01 20:27:50.000000 iron_toolbox-1.0.9/iron_toolbox/sftp_functions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:55.428359 iron_toolbox-1.0.9/iron_toolbox.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-04-13 17:31:54.000000 iron_toolbox-1.0.9/iron_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-04-13 17:31:54.000000 iron_toolbox-1.0.9/iron_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:31:54.000000 iron_toolbox-1.0.9/iron_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2023-04-13 17:31:54.000000 iron_toolbox-1.0.9/iron_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 17:31:54.000000 iron_toolbox-1.0.9/iron_toolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-13 17:31:55.432881 iron_toolbox-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1586 2023-04-13 17:31:07.000000 iron_toolbox-1.0.9/setup.py
```

### Comparing `iron_toolbox-1.0.8/LICENSE.txt` & `iron_toolbox-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.8/PKG-INFO` & `iron_toolbox-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron_toolbox
-Version: 1.0.8
+Version: 1.0.9
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
```

### Comparing `iron_toolbox-1.0.8/iron_toolbox/aws_functions.py` & `iron_toolbox-1.0.9/iron_toolbox/aws_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.8/iron_toolbox/domo_functions.py` & `iron_toolbox-1.0.9/iron_toolbox/domo_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.8/iron_toolbox/iron_functions.py` & `iron_toolbox-1.0.9/iron_toolbox/iron_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.8/iron_toolbox/mongo_functions.py` & `iron_toolbox-1.0.9/iron_toolbox/mongo_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,16 +470,19 @@
                                                                                      'contactChannel': 1,
                                                                                      'status': 1,
                                                                                      'serviceReturn': 1,
                                                                                      'complains': 1,
                                                                                      'orientations': 1,
                                                                                      'exams': 1,
                                                                                      'medicines': 1,
+                                                                                     'outsideAppointments': 1,
                                                                                      'fup': 1,
                                                                                      'illnessAllergies': 1,
+                                                                                     'linkedMedicine': 1,
+                                                                                     'linkedSickNote': 1,
                                                                                      'note': 1}),
                                                 desc="Total itens recebidos:"))
         print(f'Realizando tratamento do Dataset {mongodb_collection}!')
         dbusertelephonecall = dbusertelephonecall.replace({'_p_support': r'^Support\$'}, {'_p_support': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_scheduledAppointments': r'^ScheduledAppointments\$'},
                                                           {'_p_scheduledAppointments': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_staff': r'^Staff\$'}, {'_p_staff': ''}, regex=True)
```

### Comparing `iron_toolbox-1.0.8/iron_toolbox/sftp_functions.py` & `iron_toolbox-1.0.9/iron_toolbox/sftp_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.8/iron_toolbox.egg-info/PKG-INFO` & `iron_toolbox-1.0.9/iron_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron-toolbox
-Version: 1.0.8
+Version: 1.0.9
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
```

### Comparing `iron_toolbox-1.0.8/setup.py` & `iron_toolbox-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # with open('requirements.txt') as f:
 #     required = f.read().splitlines()
     
 setuptools.setup(
     name='iron_toolbox',
     packages=['iron_toolbox'],
-    version='1.0.8',
+    version='1.0.9',
     license='MIT',
     description='Functions to be used by Iron Data Analytics Team',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Luciano Siqueira',
     author_email='lucianosiqueira@iron.fit',
     url='https://github.com/IronTrainers/iron_data_toolbox',
```

