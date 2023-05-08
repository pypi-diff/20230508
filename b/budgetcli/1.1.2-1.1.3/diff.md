# Comparing `tmp/budgetcli-1.1.2.tar.gz` & `tmp/budgetcli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.1.2.tar", last modified: Sun May  7 20:29:18 2023, max compression
+gzip compressed data, was "budgetcli-1.1.3.tar", last modified: Mon May  8 20:30:58 2023, max compression
```

## Comparing `budgetcli-1.1.2.tar` & `budgetcli-1.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-07 20:28:54.000000 budgetcli-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-07 20:29:18.454256 budgetcli-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-07 20:28:54.000000 budgetcli-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-07 20:28:54.000000 budgetcli-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-07 20:29:18.454256 budgetcli-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.450256 budgetcli-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.114588 budgetcli-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 20:30:29.000000 budgetcli-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-08 20:30:58.114588 budgetcli-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 20:30:29.000000 budgetcli-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-08 20:30:29.000000 budgetcli-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 20:30:58.114588 budgetcli-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.106587 budgetcli-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.106587 budgetcli-1.1.3/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.110587 budgetcli-1.1.3/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.110587 budgetcli-1.1.3/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.110587 budgetcli-1.1.3/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.1.2/LICENSE` & `budgetcli-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/PKG-INFO` & `budgetcli-1.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: budgetcli
-Version: 1.1.2
-Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
-Author: Code Rustle
-Author-email: coderustle@gmail.com
-License: MIT
-Classifier: Topic :: Utilities
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Budget CLI
 
 [![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml) [![Test](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml/badge.svg)](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml) [![License](https://img.shields.io/pypi/l/budgetcli)](https://img.shields.io/pypi/l/budgetcli)
 
 A simple terminal app written in Python to manage budgets and expenses in Google Sheet.
 
 ## Features
@@ -69,44 +54,65 @@
 budgetcli <VERB> <OBJECT> <OPTIONS>
 ```
 ### Incomes
 To add an income you need to provide only an amount and a category. By default, all the income transactions are added
 with default today date and without no description.
 
 **Add an income**
+```bash
+budgetcli add income 5000 salary
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income.gif)
 
 **Add an income with description**
+```bash
+budgetcli add income 5000 projects --description "Project A"
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-description.gif)
 
 **Add an income with date and description**
+```bash
+budgetcli add income 500 projects --description "Project A" --date 2023-04-01
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-date.gif)
 
 ### Outcomes
 Same for outcome transactions, you need to provide only an amount and a category. By default, all the outcome transactions are added
 with default today date and without no description.
 
 **Add an outcome**
+```bash
+budgetcli add outcome 400 rent
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome.gif)
 
 **Add an outcome with description**
+```bash
+budgetcli add 400 rent --date 2023-05-01 --description "Rent for May"
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome-date.gif)
 
 ### List transactions
 
 **List first 100 transactions**
+```bash
+budgetcli list transactions
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions.gif)
 
 **List only first 10 transactions**
+```bash
+budgetcli list transaction --rows 10
+```
 
 ![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions-rows.gif)
 
 **List transactions for a specific month**
 ```bash
 budgetcli list transactions --month April 
 ```
```

### Comparing `budgetcli-1.1.2/pyproject.toml` & `budgetcli-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/setup.cfg` & `budgetcli-1.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.1.2
+version = 1.1.3
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.1.2/src/budgetcli/auth.py` & `budgetcli-1.1.3/src/budgetcli/auth.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/cli/add.py` & `budgetcli-1.1.3/src/budgetcli/cli/add.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/cli/config.py` & `budgetcli-1.1.3/src/budgetcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/cli/display.py` & `budgetcli-1.1.3/src/budgetcli/cli/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/commands.py` & `budgetcli-1.1.3/src/budgetcli/commands.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/data_manager.py` & `budgetcli-1.1.3/src/budgetcli/data_manager.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/main.py` & `budgetcli-1.1.3/src/budgetcli/main.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/models.py` & `budgetcli-1.1.3/src/budgetcli/models.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/settings.py` & `budgetcli-1.1.3/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/utils/config.py` & `budgetcli-1.1.3/src/budgetcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/utils/dates.py` & `budgetcli-1.1.3/src/budgetcli/utils/dates.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli/utils/display.py` & `budgetcli-1.1.3/src/budgetcli/utils/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.2/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-1.1.3/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

