# Comparing `tmp/perfectoai-1.0.36.tar.gz` & `tmp/perfectoai-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfectoai-1.0.36.tar", last modified: Mon May  8 14:08:29 2023, max compression
+gzip compressed data, was "perfectoai-1.0.37.tar", last modified: Mon May  8 15:38:05 2023, max compression
```

## Comparing `perfectoai-1.0.36.tar` & `perfectoai-1.0.37.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 genesis.thomas   (502) staff       (20)        0 2023-05-08 14:08:29.430269 perfectoai-1.0.36/
--rw-r--r--   0 genesis.thomas   (502) staff       (20)     1821 2023-05-08 12:39:51.000000 perfectoai-1.0.36/CHANGELOG.md
--rw-r--r--   0 genesis.thomas   (502) staff       (20)       20 2023-05-08 14:08:12.000000 perfectoai-1.0.36/MANIFEST.in
--rw-r--r--   0 genesis.thomas   (502) staff       (20)     2224 2023-05-08 14:08:29.423019 perfectoai-1.0.36/PKG-INFO
--rw-r--r--   0 genesis.thomas   (502) staff       (20)      997 2023-05-08 06:59:09.000000 perfectoai-1.0.36/README.md
-drwxr-xr-x   0 genesis.thomas   (502) staff       (20)        0 2023-05-08 14:08:29.400255 perfectoai-1.0.36/perfecto/
-drwxr-xr-x   0 genesis.thomas   (502) staff       (20)        0 2023-05-08 14:08:29.422408 perfectoai-1.0.36/perfecto/perfectoai.egg-info/
--rw-r--r--   0 genesis.thomas   (502) staff       (20)     2224 2023-05-08 14:08:29.000000 perfectoai-1.0.36/perfecto/perfectoai.egg-info/PKG-INFO
--rw-r--r--   0 genesis.thomas   (502) staff       (20)      303 2023-05-08 14:08:29.000000 perfectoai-1.0.36/perfecto/perfectoai.egg-info/SOURCES.txt
--rw-r--r--   0 genesis.thomas   (502) staff       (20)        1 2023-05-08 14:08:29.000000 perfectoai-1.0.36/perfecto/perfectoai.egg-info/dependency_links.txt
--rw-r--r--   0 genesis.thomas   (502) staff       (20)       56 2023-05-08 14:08:29.000000 perfectoai-1.0.36/perfecto/perfectoai.egg-info/entry_points.txt
--rw-r--r--   0 genesis.thomas   (502) staff       (20)      272 2023-05-08 14:08:29.000000 perfectoai-1.0.36/perfecto/perfectoai.egg-info/requires.txt
--rw-r--r--   0 genesis.thomas   (502) staff       (20)        1 2023-05-08 14:08:29.000000 perfectoai-1.0.36/perfecto/perfectoai.egg-info/top_level.txt
--rw-r--r--   0 genesis.thomas   (502) staff       (20)       38 2023-05-08 14:08:29.430420 perfectoai-1.0.36/setup.cfg
--rw-r--r--   0 genesis.thomas   (502) staff       (20)     1414 2023-05-08 14:08:17.000000 perfectoai-1.0.36/setup.py
+drwxr-xr-x   0 genesis.thomas   (502) staff       (20)        0 2023-05-08 15:38:05.803142 perfectoai-1.0.37/
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)     1821 2023-05-08 15:37:20.000000 perfectoai-1.0.37/CHANGELOG.md
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)       20 2023-05-08 14:08:12.000000 perfectoai-1.0.37/MANIFEST.in
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)     2224 2023-05-08 15:38:05.802540 perfectoai-1.0.37/PKG-INFO
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)     1123 2023-05-08 15:12:56.000000 perfectoai-1.0.37/README.md
+drwxr-xr-x   0 genesis.thomas   (502) staff       (20)        0 2023-05-08 15:38:05.796849 perfectoai-1.0.37/perfecto/
+drwxr-xr-x   0 genesis.thomas   (502) staff       (20)        0 2023-05-08 15:38:05.802055 perfectoai-1.0.37/perfecto/perfectoai.egg-info/
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)     2224 2023-05-08 15:38:05.000000 perfectoai-1.0.37/perfecto/perfectoai.egg-info/PKG-INFO
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)      303 2023-05-08 15:38:05.000000 perfectoai-1.0.37/perfecto/perfectoai.egg-info/SOURCES.txt
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)        1 2023-05-08 15:38:05.000000 perfectoai-1.0.37/perfecto/perfectoai.egg-info/dependency_links.txt
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)       56 2023-05-08 15:38:05.000000 perfectoai-1.0.37/perfecto/perfectoai.egg-info/entry_points.txt
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)      288 2023-05-08 15:38:05.000000 perfectoai-1.0.37/perfecto/perfectoai.egg-info/requires.txt
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)        1 2023-05-08 15:38:05.000000 perfectoai-1.0.37/perfecto/perfectoai.egg-info/top_level.txt
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)       38 2023-05-08 15:38:05.803231 perfectoai-1.0.37/setup.cfg
+-rw-r--r--   0 genesis.thomas   (502) staff       (20)     1452 2023-05-08 15:37:28.000000 perfectoai-1.0.37/setup.py
```

### Comparing `perfectoai-1.0.36/CHANGELOG.md` & `perfectoai-1.0.37/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 PerfectoAI is an automated emailable analytics tool along with AI graphs & predictions specially designed for Perfecto's Smart Reports. Kindly reach out to Perfecto's Professional Services if interested.</br>
 [![Downloads](https://pepy.tech/badge/perfectoai)](https://pepy.tech/project/perfectoai)
 
 CHANGES
 =======
-1.0.36:
+1.0.37:
 -------
 - Handled if no CI jobs ran before
 - Removed unnecessary warnings related to timezone converions. 
 - UI upgrades
 
 1.0.34:
 -------
```

### Comparing `perfectoai-1.0.36/PKG-INFO` & `perfectoai-1.0.37/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: perfectoai
-Version: 1.0.36
+Version: 1.0.37
 Summary: PerfectoAI is an automated emailable analytics tool along with AI graphs & predictions
 Author: Genesis Thomas
 Author-email: gthomas@perforce.com
 Keywords: Perfecto,appium,selenium,testing,api,automation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 PerfectoAI is an automated emailable analytics tool along with AI graphs & predictions specially designed for Perfecto's Smart Reports. Kindly reach out to Perfecto's Professional Services if interested.</br>
 [![Downloads](https://pepy.tech/badge/perfectoai)](https://pepy.tech/project/perfectoai)
 
 CHANGES
 =======
-1.0.36:
+1.0.37:
 -------
 - Handled if no CI jobs ran before
 - Removed unnecessary warnings related to timezone converions. 
 - UI upgrades
 
 1.0.34:
 -------
```

### Comparing `perfectoai-1.0.36/README.md` & `perfectoai-1.0.37/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 
   3. Install [npm](https://nodejs.org/en/)
 
   4. Install Anaconda
     
   4. Run the following commands from conda power shell - Windows:
         pip uninstall fbprophet
+        pip install cython
         pip install psutil
         npm install -g electron@1.8.4 orca --unsafe-perm=true
         pip install pystan==2.19.1.1
+        pip install prophet==1.0.1
         pip install perfectoai -U
     
     mac:
         pip3 uninstall fbprophet
+        pip3 install cython
         pip3 install psutil
         sudo npm install -g electron@1.8.4 orca --unsafe-perm=true
         pip3 install pystan==2.19.1.1
+        pip3 install prophet==1.0.1
         pip3 install perfectoai -U
```

### Comparing `perfectoai-1.0.36/perfecto/perfectoai.egg-info/PKG-INFO` & `perfectoai-1.0.37/perfecto/perfectoai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: perfectoai
-Version: 1.0.36
+Version: 1.0.37
 Summary: PerfectoAI is an automated emailable analytics tool along with AI graphs & predictions
 Author: Genesis Thomas
 Author-email: gthomas@perforce.com
 Keywords: Perfecto,appium,selenium,testing,api,automation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 PerfectoAI is an automated emailable analytics tool along with AI graphs & predictions specially designed for Perfecto's Smart Reports. Kindly reach out to Perfecto's Professional Services if interested.</br>
 [![Downloads](https://pepy.tech/badge/perfectoai)](https://pepy.tech/project/perfectoai)
 
 CHANGES
 =======
-1.0.36:
+1.0.37:
 -------
 - Handled if no CI jobs ran before
 - Removed unnecessary warnings related to timezone converions. 
 - UI upgrades
 
 1.0.34:
 -------
```

### Comparing `perfectoai-1.0.36/setup.py` & `perfectoai-1.0.37/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 OPTIONS = {}
 mainscript = 'perfecto/perfectoai.py'
 with open("CHANGELOG.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='perfectoai',
-    #   version='1.0.36', #testpypi
-    version='1.0.36',
+    #   version='1.0.37', #testpypi
+    version='1.0.37',
     author="Genesis Thomas",
     author_email="gthomas@perforce.com",
     description="PerfectoAI is an automated emailable analytics tool along with AI graphs & predictions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['Perfecto', 'appium', 'selenium',
               'testing', 'api', 'automation'],
     install_requires=[
-            'json2html', 'jenkinsapi', 'requests', 'numpy', 'cython', 'pandas==1.2.4', 'retrying', 'ephem', 'pymeeus', 'easydict', 'psutil', 'korean-lunar-calendar', 'MarkupSafe', 'jinja2', 'colorama', 'LunarCalendar', 'holidays', 'cmdstanpy==0.9.68', 'convertdate', 'openpyxl', 'wheel', 'pystan==2.19.1.1', 'xlrd', 'jinja2', 'tzlocal', 'plotly', 'prophet==1.0.1'
-    ],
+            'json2html', 'kaleido', 'urllib3', 'jenkinsapi', 'requests', 'numpy', 'cython', 'pandas==1.5.3', 'retrying', 'ephem', 'pymeeus', 'easydict', 'psutil', 'korean-lunar-calendar', 'MarkupSafe', 'jinja2', 'colorama', 'LunarCalendar', 'holidays', 'cmdstanpy==0.9.68', 'convertdate', 'openpyxl', 'wheel', 'pystan==2.19.1.1', 'xlrd', 'jinja2', 'tzlocal', 'plotly', 'prophet==1.0.1'
+    ], # pandas==1.2.4
     package_dir={'': "perfecto"},
     packages=find_packages("perfecto"),
     include_package_data=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent'
     ],
```

