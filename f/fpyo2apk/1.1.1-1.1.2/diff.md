# Comparing `tmp/fpyo2apk-1.1.1.tar.gz` & `tmp/fpyo2apk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpyo2apk-1.1.1.tar", last modified: Sun May  7 21:22:53 2023, max compression
+gzip compressed data, was "fpyo2apk-1.1.2.tar", last modified: Sun May  7 21:32:56 2023, max compression
```

## Comparing `fpyo2apk-1.1.1.tar` & `fpyo2apk-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/Tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/check_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/check_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/unzip_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   495603 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/assets/fpyo2apkdist.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/edit_beeware_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_app_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_localhost_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:56.460885 fpyo2apk-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-07 21:32:56.460885 fpyo2apk-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:56.456885 fpyo2apk-1.1.2/fpyo2apk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:56.456885 fpyo2apk-1.1.2/fpyo2apk/Tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/Tools/check_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/Tools/check_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/Tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:56.456885 fpyo2apk-1.1.2/fpyo2apk/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   495603 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/assets/fpyo2apkdist.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:56.460885 fpyo2apk-1.1.2/fpyo2apk/beeware_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/beeware_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/beeware_tools/edit_beeware_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/beeware_tools/the_app_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/beeware_tools/the_localhost_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/fpyo2apk/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:32:56.456885 fpyo2apk-1.1.2/fpyo2apk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-07 21:32:56.000000 fpyo2apk-1.1.2/fpyo2apk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-07 21:32:56.000000 fpyo2apk-1.1.2/fpyo2apk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:32:56.000000 fpyo2apk-1.1.2/fpyo2apk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:32:56.000000 fpyo2apk-1.1.2/fpyo2apk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 21:32:56.000000 fpyo2apk-1.1.2/fpyo2apk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:32:56.460885 fpyo2apk-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 21:32:45.000000 fpyo2apk-1.1.2/setup.py
```

### Comparing `fpyo2apk-1.1.1/LICENSE` & `fpyo2apk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/fpyo2apk/Tools/unzip_assets.py` & `fpyo2apk-1.1.2/fpyo2apk/Tools/unzip_assets.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/fpyo2apk/assets/fpyo2apkdist.zip` & `fpyo2apk-1.1.2/fpyo2apk/assets/fpyo2apkdist.zip`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/fpyo2apk/beeware_tools/edit_beeware_project.py` & `fpyo2apk-1.1.2/fpyo2apk/beeware_tools/edit_beeware_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,22 @@
 
     print("start edit the 'app.py' file")
     open(f"{project_name}/src/fpyo2apk/app.py", "w+", encoding="utf-8").write(The_app_py_script)
 
     print("start creating/editing the 'localhost.py' file")
     open(f"{project_name}/src/fpyo2apk/localhost.py", "w+", encoding="utf-8").write(The_localhost_py_script)
 
-    print("Your app is being built and then opened on the iOS simulator..\nThis Usually take two minutes to finish, please wait..")
+    print("Your app is being built and then can open it on the android simulator..\nThis Usually take two minutes to finish, please wait..")
     process = subprocess.Popen(["cd fpyo2apkdist\nbriefcase create Android\nbriefcase build Android\n"], stdin=subprocess.PIPE, stdout=subprocess.PIPE, shell=True)
     output, error = process.communicate()
     if error != None:
         sys.exit(f"\nExit with Error: {error}")
     
     print("""
 
 All work done!
-Your app is in the `fpyo2apkdist/build/fpyo2apkdist/Android/`!
+Your app is in the `fpyo2apkdist/build/fpyo2apkdist/android/`!
 To run a simulator, use:
-$ cd pyo2ipadist
+$ cd fpyo2apkdist
 $ briefcase run Android
 
     """)
```

### Comparing `fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_app_py.py` & `fpyo2apk-1.1.2/fpyo2apk/beeware_tools/the_app_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_localhost_py.py` & `fpyo2apk-1.1.2/fpyo2apk/beeware_tools/the_localhost_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/fpyo2apk/build.py` & `fpyo2apk-1.1.2/fpyo2apk/build.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/fpyo2apk.egg-info/SOURCES.txt` & `fpyo2apk-1.1.2/fpyo2apk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.1/setup.py` & `fpyo2apk-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fpyo2apk',
-    version='1.1.1',
+    version='1.1.2',
     author='SKbarbon',
     description='A package tool that allow you to built a python Android apps with flet-pyodide dist.',
     long_description="https://github.com/SKbarbon/fpyo2apk",
     url='https://github.com/SKbarbon/fpyo2apk',
     install_requires=["briefcase==0.3.14"],
     include_package_data=True,
     packages=find_packages(),
```

