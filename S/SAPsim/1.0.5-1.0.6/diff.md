# Comparing `tmp/SAPsim-1.0.5.tar.gz` & `tmp/SAPsim-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.5.tar", last modified: Mon May  1 02:38:25 2023, max compression
+gzip compressed data, was "SAPsim-1.0.6.tar", last modified: Mon May  8 03:02:07 2023, max compression
```

## Comparing `SAPsim-1.0.5.tar` & `SAPsim-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-01 02:38:17.000000 SAPsim-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-01 02:38:25.953122 SAPsim-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-01 02:38:17.000000 SAPsim-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.949122 SAPsim-1.0.5/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-01 02:38:17.000000 SAPsim-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:38:25.953122 SAPsim-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-01 02:38:17.000000 SAPsim-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 03:01:58.000000 SAPsim-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:02:07.307944 SAPsim-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-08 03:01:58.000000 SAPsim-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.303944 SAPsim-1.0.6/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-08 03:01:58.000000 SAPsim-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:02:07.307944 SAPsim-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-08 03:01:58.000000 SAPsim-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_run.py
```

### Comparing `SAPsim-1.0.5/LICENSE` & `SAPsim-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/PKG-INFO` & `SAPsim-1.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -14,21 +14,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SAPsim
+[![tests GitHub action](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml)
+[![documentation badge](https://readthedocs.org/projects/sapsim/badge/?version=latest)](https://SAPsim.readthedocs.io/en/latest/)
 
-![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
+# SAPsim
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/SAPsim_demo.gif" alt="SAPsim demo">
 </p>
 
 ## Install
 
@@ -41,31 +40,35 @@
 ## Usage
 
 Write a SAP program in the CSV file format shown below.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/ex1.jpg" alt="Screenshot of ex1.csv in Excel">
 </p>
-<p align="center"><a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a></p>
+<p align="center">
+    <a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a>
+</p>
 
-You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension.
+You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension. For a blank template, see [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
 
 Open a Python terminal. Import SAPsim's `run()` function, and pass the path to your SAP program as an argument.
 
 ```py
 >>> from SAPsim import run
->>> run("ex1.csv")                 # run ex1.csv at full speed (default)
+>>> run("ex1.csv")                 # Run ex1.csv at full speed (default)
 ...
->>> run("ex1.csv", debug=True)     # run ex1.csv in debug (step) mode
+>>> run("ex1.csv", debug=True)     # Run ex1.csv in debug (step) mode
 ...
 ```
 
 **Note**: There is a debug (step) mode, as shown above.
 
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
+## Settings
+
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed table format).
 
 ## Rules
 
 It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
```

#### html2text {}

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.5 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.6 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE # SAPsim ![Test badge](https://github.com/jesse-wei/SAPsim/actions/
-workflows/tests.yml/badge.svg) ![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg) ![Python](https://img.shields.io/badge/
-python-3670A0?style=plastic&logo=python&logoColor=ffdd54) > Simulation of [SAP
-(Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from
-COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+LICENSE [![tests GitHub action](https://github.com/jesse-wei/SAPsim/actions/
+workflows/tests.yml/badge.svg)](https://github.com/jesse-wei/SAPsim/actions/
+workflows/tests.yml) [![documentation badge](https://readthedocs.org/projects/
+sapsim/badge/?version=latest)](https://SAPsim.readthedocs.io/en/latest/) #
+SAPsim Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/
+img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://
+unc.edu).
                                  [SAPsim demo]
 ## Install `pip install SAPsim` Your Python version needs to be 3.9+. Check
 with `python --version`. If `python` doesn't work, try `python3`. If `pip`
 doesn't work, try `pip3`. ## Usage Write a SAP program in the CSV file format
 shown below.
                        [Screenshot of ex1.csv in Excel]
                                     ex1.csv
 You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets,
-etc.), as long as you preserve the `.csv` extension. Open a Python terminal.
-Import SAPsim's `run()` function, and pass the path to your SAP program as an
-argument. ```py >>> from SAPsim import run >>> run("ex1.csv") # run ex1.csv at
-full speed (default) ... >>> run("ex1.csv", debug=True) # run ex1.csv in debug
-(step) mode ... ``` **Note**: There is a debug (step) mode, as shown above.
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/
-#settings) (e.g., table format). ## Rules It's easy to just mimic the [example
-programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but
-if you need it, here's the list of [rules for SAPsim programs](https://
-SAPsim.readthedocs.io/en/latest/rules.html). ## SAP instruction set
+etc.), as long as you preserve the `.csv` extension. For a blank template, see
+[template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
+Open a Python terminal. Import SAPsim's `run()` function, and pass the path to
+your SAP program as an argument. ```py >>> from SAPsim import run >>> run
+("ex1.csv") # Run ex1.csv at full speed (default) ... >>> run("ex1.csv",
+debug=True) # Run ex1.csv in debug (step) mode ... ``` **Note**: There is a
+debug (step) mode, as shown above. ## Settings Here's a list of [additional
+settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed
+table format). ## Rules It's easy to just mimic the [example programs](https://
+github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it,
+here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/
+en/latest/rules.html). ## SAP instruction set
                              [SAP instruction set]
 ## Documentation [https://SAPsim.readthedocs.io](https://SAPsim.readthedocs.io/
 en/latest/)
```

### Comparing `SAPsim-1.0.5/README.md` & `SAPsim-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# SAPsim
+[![tests GitHub action](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml)
+[![documentation badge](https://readthedocs.org/projects/sapsim/badge/?version=latest)](https://SAPsim.readthedocs.io/en/latest/)
 
-![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
+# SAPsim
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/SAPsim_demo.gif" alt="SAPsim demo">
 </p>
 
 ## Install
 
@@ -21,31 +20,35 @@
 ## Usage
 
 Write a SAP program in the CSV file format shown below.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/ex1.jpg" alt="Screenshot of ex1.csv in Excel">
 </p>
-<p align="center"><a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a></p>
+<p align="center">
+    <a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a>
+</p>
 
-You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension.
+You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension. For a blank template, see [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
 
 Open a Python terminal. Import SAPsim's `run()` function, and pass the path to your SAP program as an argument.
 
 ```py
 >>> from SAPsim import run
->>> run("ex1.csv")                 # run ex1.csv at full speed (default)
+>>> run("ex1.csv")                 # Run ex1.csv at full speed (default)
 ...
->>> run("ex1.csv", debug=True)     # run ex1.csv in debug (step) mode
+>>> run("ex1.csv", debug=True)     # Run ex1.csv in debug (step) mode
 ...
 ```
 
 **Note**: There is a debug (step) mode, as shown above.
 
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
+## Settings
+
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed table format).
 
 ## Rules
 
 It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
-# SAPsim ![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/
-tests.yml/badge.svg) ![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg) ![Python](https://img.shields.io/badge/python-
-3670A0?style=plastic&logo=python&logoColor=ffdd54) > Simulation of [SAP (Simple
-As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311
-(Computer Organization) @ [UNC](https://unc.edu).
+[![tests GitHub action](https://github.com/jesse-wei/SAPsim/actions/workflows/
+tests.yml/badge.svg)](https://github.com/jesse-wei/SAPsim/actions/workflows/
+tests.yml) [![documentation badge](https://readthedocs.org/projects/sapsim/
+badge/?version=latest)](https://SAPsim.readthedocs.io/en/latest/) # SAPsim
+Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/
+sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://
+unc.edu).
                                  [SAPsim demo]
 ## Install `pip install SAPsim` Your Python version needs to be 3.9+. Check
 with `python --version`. If `python` doesn't work, try `python3`. If `pip`
 doesn't work, try `pip3`. ## Usage Write a SAP program in the CSV file format
 shown below.
                        [Screenshot of ex1.csv in Excel]
                                     ex1.csv
 You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets,
-etc.), as long as you preserve the `.csv` extension. Open a Python terminal.
-Import SAPsim's `run()` function, and pass the path to your SAP program as an
-argument. ```py >>> from SAPsim import run >>> run("ex1.csv") # run ex1.csv at
-full speed (default) ... >>> run("ex1.csv", debug=True) # run ex1.csv in debug
-(step) mode ... ``` **Note**: There is a debug (step) mode, as shown above.
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/
-#settings) (e.g., table format). ## Rules It's easy to just mimic the [example
-programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but
-if you need it, here's the list of [rules for SAPsim programs](https://
-SAPsim.readthedocs.io/en/latest/rules.html). ## SAP instruction set
+etc.), as long as you preserve the `.csv` extension. For a blank template, see
+[template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
+Open a Python terminal. Import SAPsim's `run()` function, and pass the path to
+your SAP program as an argument. ```py >>> from SAPsim import run >>> run
+("ex1.csv") # Run ex1.csv at full speed (default) ... >>> run("ex1.csv",
+debug=True) # Run ex1.csv in debug (step) mode ... ``` **Note**: There is a
+debug (step) mode, as shown above. ## Settings Here's a list of [additional
+settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed
+table format). ## Rules It's easy to just mimic the [example programs](https://
+github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it,
+here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/
+en/latest/rules.html). ## SAP instruction set
                              [SAP instruction set]
 ## Documentation [https://SAPsim.readthedocs.io](https://SAPsim.readthedocs.io/
 en/latest/)
```

### Comparing `SAPsim-1.0.5/SAPsim/__init__.py` & `SAPsim-1.0.6/SAPsim/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-from typing import Any
 from SAPsim.utils.helpers import is_documented_by
 import SAPsim.utils.execute as execute
 
 
 # Weird glitch, passing in the function doesn't actually get its docstring? Just append then
 @is_documented_by(execute.run, 0, "", execute.run.__doc__)
 def run(prog_path: str, **kwargs) -> None:
     execute.run(prog_path, **kwargs)
 
 
-# Weird glitch, passing in the function doesn't actually get its docstring? Just append then
-@is_documented_by(
-    execute.run_and_return_state, 0, "", execute.run_and_return_state.__doc__
-)
-def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
-    return execute.run_and_return_state(prog_path, **kwargs)
-
-
 def create_template() -> None:
     r"""
     Create blank ``template.csv`` file in SAPsim format in current directory.
     """
     # This will rarely be used so doesn't need to be imported at top level
     import csv
```

### Comparing `SAPsim-1.0.5/SAPsim/utils/exceptions.py` & `SAPsim-1.0.6/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/SAPsim/utils/execute.py` & `SAPsim-1.0.6/SAPsim/utils/execute.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Execute instructions in RAM."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from pathlib import Path
-from typing import Any
+from typing import Any, Union
 import SAPsim.utils.global_vars as global_vars
 import SAPsim.utils.instructions as instructions
 import SAPsim.utils.helpers as helpers
 from SAPsim.utils.helpers import is_documented_by
 import SAPsim.utils.exceptions as exceptions
 import SAPsim.utils.parser as parser
 
@@ -45,74 +45,84 @@
             global_vars.PC += 1
         else:
             instructions.OPCODE_TO_INSTR_PROCEDURE[
                 helpers.parse_opcode(global_vars.RAM[global_vars.PC])
             ](helpers.parse_arg(global_vars.RAM[global_vars.PC]))
 
 
-def run(prog_path: str, **kwargs) -> None:
+def run(prog_path: str, **kwargs) -> Union[None, dict[str, Any]]:
     r"""Run given .csv program in SAPsim format.
 
     :param prog_path:
         .csv file in SAPsim format.
     :type prog_path: ``str``
     :param \**kwargs:
         See below
 
     :Keyword Arguments:
         * *debug* (``bool``) --
             * Whether to run in debug mode (True) or at full speed (False)
             * Default is full speed
         * *change* (``str``) --
-            * Comma-separated list of changes to RAM
+            * Comma-separated list of hardcoded changes to RAM
             * Format: <addr>:<base-10 value>,<addr>:<base-10 value>,...
             * The value at each address will be overwritten to that base-10 value
-            * Useful for debugging programs (edit a value without changing CSV)
-            * Also useful for autograding programs (overwrite a reserved instruction/data value)
+            * Useful for debugging programs (edit a value without changing the CSV)
+            * Useful for autograding programs (overwrite a reserved instruction/data value)
         * *table_format* (``str``) --
-            * Table format
+            * Printed table format
             * Options: https://github.com/astanin/python-tabulate#table-format
             * Default value in ``global_vars`` is ``"simple_outline"``
-        * *bits* (``int``) --
-            * Number of bits in unsigned registers
-            * Default value in ``global_vars`` is 8
-        * *non_blocking* (``bool``) --
-            * This is used to unit test debug mode of ``run()``, you likely don't have a need for this
-            * If ``True``, then ``run()`` won't block on input
-            * ``input()`` won't be called in debug mode (i.e., don't have to press enter to continue execution)
-            * If this is ``True``, then debug mode will be on even if ``debug`` isn't in kwargs
-        * *no_print* (``bool``) --
-            * This is used to save computation time during unit testing
-            * If ``True``, then ``print()`` won't be called, except for error messages
+        * The rest of the parameters are pretty much exclusively for unit testing, and you should not use these
+            * *return_state* (``bool``) --
+                * If ``True``, then program state will be returned
+                * See ``utils.helpers.get_state()``
+            * *non_blocking* (``bool``) --
+                * This is used to unit test debug mode of ``run()``, you likely don't have a need for this
+                * If ``True``, then ``run()`` won't block on input
+                * ``input()`` won't be called in debug mode (i.e., don't have to press enter to continue execution)
+                * If this is ``True``, then debug mode will be on even if ``debug`` isn't in kwargs
+            * *no_print* (``bool``) --
+                * This is used to save computation time during unit testing
+                * If ``True``, then ``print()`` won't be called, except for error messages
+            * *bits* (``int``) --
+                * Number of bits in unsigned registers
+                * Default value in ``global_vars`` is 8
 
-    :return: ``None``
+    :return: ``None`` or program state if ``return_state``
+    :rtype: Union[None, dict[str, Any]]
     """
     if not isinstance(prog_path, str):
         raise TypeError("Required parameter prog_path must be a str.")
     if "debug" in kwargs and not isinstance(kwargs["debug"], bool):
         raise TypeError("Keyword argument debug must be a bool.")
     if "change" in kwargs and not isinstance(kwargs["change"], str):
         raise TypeError("Keyword argument change must be a str.")
     if "table_format" in kwargs and not isinstance(kwargs["table_format"], str):
         raise TypeError("Keyword argument table_format must be a str.")
-    if "bits" in kwargs and not isinstance(kwargs["bits"], int):
-        raise TypeError("Keyword argument bits must be an int.")
+    if "return_state" in kwargs and not isinstance(kwargs["return_state"], bool):
+        raise TypeError("Keyword argument return_state must be a bool.")
     if "non_blocking" in kwargs and not isinstance(kwargs["non_blocking"], bool):
         raise TypeError("Keyword argument non_blocking must be a bool.")
+    if "no_print" in kwargs and not isinstance(kwargs["no_print"], bool):
+        raise TypeError("Keyword argument no_print must be a bool.")
+    if "bits" in kwargs and not isinstance(kwargs["bits"], int):
+        raise TypeError("Keyword argument bits must be an int.")
 
     path: Path = Path(prog_path)
     if not path.suffix == ".csv":
         raise exceptions.FileNotCSV(path)
     helpers.setup_8bit()
     parser.parse_csv(path)
     if "bits" in kwargs:
         assert kwargs["bits"] > 1
         global_vars.NUM_BITS_IN_REGISTERS = kwargs["bits"]
         # Don't need to call setup_n_bit.
-        # All it does is change NUM_BITS_IN_REGISTERS and reset globals.
+        # All it does is change NUM_BITS_IN_REGISTERS and reset globals, which was already done
+        # by setup_8bit().
     if "change" in kwargs:
         changes = kwargs["change"].split(",")
         for change in changes:
             if change.count(":") != 1:
                 print(
                     "Invalid syntax for change parameter, correct format is <addr>:<base-10 value>, <addr>:<base-10 value>, ..."
                 )
@@ -160,20 +170,9 @@
     else:
         execute_full_speed()
         if not kwargs.get("no_print"):
             helpers.print_RAM()
             helpers.print_info()
             print("Program halted.")
 
-
-@is_documented_by(
-    run,
-    2,
-    "",
-    r"""
-    :return: ``dict`` containing program state (see ``helpers.get_state``)
-    :rtype: ``dict[str, Any]``
-    """,
-)
-def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
-    run(prog_path, **kwargs)
-    return helpers.get_state()
+    if kwargs.get("return_state"):
+        return helpers.get_state()
```

### Comparing `SAPsim-1.0.5/SAPsim/utils/global_vars.py` & `SAPsim-1.0.6/SAPsim/utils/global_vars.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/SAPsim/utils/helpers.py` & `SAPsim-1.0.6/SAPsim/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/SAPsim/utils/instructions.py` & `SAPsim-1.0.6/SAPsim/utils/instructions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-"""All function docstrings (and even most implementations) are ripped straight from the SAP Instruction Set, with only slight modifications.
+"""SAP instruction implementation.
 
-This DOES NOT exist in actual SAP but for the purposes of simulation and testing, ``add(arg)`` and ``sub(arg)`` have optional kwargs direct_add= and direct_sub= that will cause A = A + arg, A = A - arg instead of A = A + Mem(arg), A = A - Mem(arg).
+All function docstrings (and even most implementations) are ripped straight from the SAP Instruction Set,
+with only slight modifications.
 
-This DOES NOT exist in actual SAP but for implementation purposes, instructions that don't need an arg (i.e. NOP, OUT, HLT) get a default parameter so that they can still be called with an argument. In actual SAP, all instructions (byte) have a required Arg, not a default or optional arg.
+This DOES NOT exist in actual SAP but for the purposes of simulation and testing,
+``add(arg)`` and ``sub(arg)`` have optional kwargs ``direct_add=`` and ``direct_sub=``
+that will cause ``A = A + arg``, ``A = A - arg`` instead of ``A = A + Mem(arg)``, ``A = A - Mem(arg)``.
 
-INSTRUCTIONS dict for using an opcode to call a specific function is defined at the bottom."""
+This DOES NOT exist in actual SAP but for implementation purposes, instructions that don't need an
+arg (i.e. NOP, OUT, HLT) get a default parameter so that they can still be called with an argument.
+In actual SAP, all instructions (byte) have a required Arg, not a default or optional arg.
+
+``OPCODE_TO_INSTR_PROCEDURE`` dict that maps opcodes to procedures is defined at the bottom."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from tabulate import tabulate
 import SAPsim.utils.global_vars as global_vars
 import SAPsim.utils.exceptions as exceptions
 import SAPsim.utils.helpers as helpers
```

### Comparing `SAPsim-1.0.5/SAPsim/utils/parser.py` & `SAPsim-1.0.6/SAPsim/utils/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Parses a SAP program in the CSV format given in ``template.csv`` into ``globs.RAM``."""
+"""Parses a SAP program in the CSV format given in ``template.csv`` into ``global_vars.RAM``."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from csv import DictReader
 from pathlib import Path
 import SAPsim.utils.exceptions as exceptions
 import SAPsim.utils.global_vars as global_vars
```

### Comparing `SAPsim-1.0.5/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.6/SAPsim.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -14,21 +14,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SAPsim
+[![tests GitHub action](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml)
+[![documentation badge](https://readthedocs.org/projects/sapsim/badge/?version=latest)](https://SAPsim.readthedocs.io/en/latest/)
 
-![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
+# SAPsim
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/SAPsim_demo.gif" alt="SAPsim demo">
 </p>
 
 ## Install
 
@@ -41,31 +40,35 @@
 ## Usage
 
 Write a SAP program in the CSV file format shown below.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/ex1.jpg" alt="Screenshot of ex1.csv in Excel">
 </p>
-<p align="center"><a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a></p>
+<p align="center">
+    <a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a>
+</p>
 
-You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension.
+You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension. For a blank template, see [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
 
 Open a Python terminal. Import SAPsim's `run()` function, and pass the path to your SAP program as an argument.
 
 ```py
 >>> from SAPsim import run
->>> run("ex1.csv")                 # run ex1.csv at full speed (default)
+>>> run("ex1.csv")                 # Run ex1.csv at full speed (default)
 ...
->>> run("ex1.csv", debug=True)     # run ex1.csv in debug (step) mode
+>>> run("ex1.csv", debug=True)     # Run ex1.csv in debug (step) mode
 ...
 ```
 
 **Note**: There is a debug (step) mode, as shown above.
 
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
+## Settings
+
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed table format).
 
 ## Rules
 
 It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
```

#### html2text {}

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.5 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.6 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE # SAPsim ![Test badge](https://github.com/jesse-wei/SAPsim/actions/
-workflows/tests.yml/badge.svg) ![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg) ![Python](https://img.shields.io/badge/
-python-3670A0?style=plastic&logo=python&logoColor=ffdd54) > Simulation of [SAP
-(Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from
-COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+LICENSE [![tests GitHub action](https://github.com/jesse-wei/SAPsim/actions/
+workflows/tests.yml/badge.svg)](https://github.com/jesse-wei/SAPsim/actions/
+workflows/tests.yml) [![documentation badge](https://readthedocs.org/projects/
+sapsim/badge/?version=latest)](https://SAPsim.readthedocs.io/en/latest/) #
+SAPsim Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/
+img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://
+unc.edu).
                                  [SAPsim demo]
 ## Install `pip install SAPsim` Your Python version needs to be 3.9+. Check
 with `python --version`. If `python` doesn't work, try `python3`. If `pip`
 doesn't work, try `pip3`. ## Usage Write a SAP program in the CSV file format
 shown below.
                        [Screenshot of ex1.csv in Excel]
                                     ex1.csv
 You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets,
-etc.), as long as you preserve the `.csv` extension. Open a Python terminal.
-Import SAPsim's `run()` function, and pass the path to your SAP program as an
-argument. ```py >>> from SAPsim import run >>> run("ex1.csv") # run ex1.csv at
-full speed (default) ... >>> run("ex1.csv", debug=True) # run ex1.csv in debug
-(step) mode ... ``` **Note**: There is a debug (step) mode, as shown above.
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/
-#settings) (e.g., table format). ## Rules It's easy to just mimic the [example
-programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but
-if you need it, here's the list of [rules for SAPsim programs](https://
-SAPsim.readthedocs.io/en/latest/rules.html). ## SAP instruction set
+etc.), as long as you preserve the `.csv` extension. For a blank template, see
+[template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
+Open a Python terminal. Import SAPsim's `run()` function, and pass the path to
+your SAP program as an argument. ```py >>> from SAPsim import run >>> run
+("ex1.csv") # Run ex1.csv at full speed (default) ... >>> run("ex1.csv",
+debug=True) # Run ex1.csv in debug (step) mode ... ``` **Note**: There is a
+debug (step) mode, as shown above. ## Settings Here's a list of [additional
+settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed
+table format). ## Rules It's easy to just mimic the [example programs](https://
+github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it,
+here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/
+en/latest/rules.html). ## SAP instruction set
                              [SAP instruction set]
 ## Documentation [https://SAPsim.readthedocs.io](https://SAPsim.readthedocs.io/
 en/latest/)
```

### Comparing `SAPsim-1.0.5/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.6/SAPsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/pyproject.toml` & `SAPsim-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/setup.py` & `SAPsim-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Check https://pypi.org/project/SAPsim/ for latest version number
-    version="1.0.5",
+    version="1.0.6",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-1.0.5/tests/test_example_progs.py` & `SAPsim-1.0.6/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/tests/test_exceptions.py` & `SAPsim-1.0.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/tests/test_helpers.py` & `SAPsim-1.0.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/tests/test_instructions.py` & `SAPsim-1.0.6/tests/test_instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.5/tests/test_run.py` & `SAPsim-1.0.6/tests/test_run.py`

 * *Files identical despite different names*

