# Comparing `tmp/pytest-pyreport-1.0.0.tar.gz` & `tmp/pytest-pyreport-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pyreport-1.0.0.tar", last modified: Sun May  7 17:55:10 2023, max compression
+gzip compressed data, was "pytest-pyreport-1.0.1.tar", last modified: Mon May  8 15:21:00 2023, max compression
```

## Comparing `pytest-pyreport-1.0.0.tar` & `pytest-pyreport-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 17:54:59.000000 pytest-pyreport-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-07 17:54:59.000000 pytest-pyreport-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-07 17:54:59.000000 pytest-pyreport-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/src/pyreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 17:54:59.000000 pytest-pyreport-1.0.0/src/pyreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-07 17:54:59.000000 pytest-pyreport-1.0.0/src/pyreport/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/src/pyreport/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-07 17:54:59.000000 pytest-pyreport-1.0.0/src/pyreport/templates/template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:55:10.642433 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-07 17:55:10.000000 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-07 17:55:10.000000 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 17:55:10.000000 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 17:55:10.000000 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 17:55:10.000000 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 17:55:10.000000 pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/pytest_pyreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/src/pytest_pyreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/src/pytest_pyreport/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/pytest_pyreport/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/src/pytest_pyreport/templates/template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/top_level.txt
```

### Comparing `pytest-pyreport-1.0.0/LICENSE` & `pytest-pyreport-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.0.0/PKG-INFO` & `pytest-pyreport-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-pyreport
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report
-Home-page: https://github.com/ToghrulMirzayev/pyreport
+Home-page: https://github.com/ToghrulMirzayev/pytest-pyreport
 Author: Toghrul Mirzayev
 Author-email: togrul.mirzoev@gmail.com
 License: MIT
-Keywords: pyreport,python,pytest,report
+Keywords: pytest_pyreport,python,pytest,report
 Classifier: Framework :: Pytest
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytest-pyreport-1.0.0/README.md` & `pytest-pyreport-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.0.0/setup.py` & `pytest-pyreport-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytest-pyreport',
-    version='1.0.0',
+    version='1.0.1',
     description='PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Toghrul Mirzayev',
     author_email='togrul.mirzoev@gmail.com',
-    url='https://github.com/ToghrulMirzayev/pyreport',
+    url='https://github.com/ToghrulMirzayev/pytest-pyreport',
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     package_data={
-        "pyreport": ["plugin.py", "templates/template.html"],
+        "pytest_pyreport": ["plugin.py", "templates/template.html"],
     },
-    entry_points={"pytest11": ["pyreport = pyreport.plugin"]},
+    entry_points={"pytest11": ["pytest_pyreport = pytest_pyreport.plugin"]},
     classifiers=["Framework :: Pytest",
                  "Operating System :: OS Independent",
                  "License :: OSI Approved :: MIT License",
                  "Programming Language :: Python :: 3",
                  "Topic :: Software Development :: Testing"],
-    keywords='pyreport, python, pytest, report',
+    keywords='pytest_pyreport, python, pytest, report',
     install_requires=[
         'Jinja2>=3.1.2',
         'pytest>=7.3.1',
     ],
     python_requires='>=3.8',
     license='MIT'
 )
```

### Comparing `pytest-pyreport-1.0.0/src/pyreport/plugin.py` & `pytest-pyreport-1.0.1/src/pytest_pyreport/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.0.0/src/pyreport/templates/template.html` & `pytest-pyreport-1.0.1/src/pytest_pyreport/templates/template.html`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.0.0/src/pytest_pyreport.egg-info/PKG-INFO` & `pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-pyreport
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report
-Home-page: https://github.com/ToghrulMirzayev/pyreport
+Home-page: https://github.com/ToghrulMirzayev/pytest-pyreport
 Author: Toghrul Mirzayev
 Author-email: togrul.mirzoev@gmail.com
 License: MIT
-Keywords: pyreport,python,pytest,report
+Keywords: pytest_pyreport,python,pytest,report
 Classifier: Framework :: Pytest
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

