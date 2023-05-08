# Comparing `tmp/xdantic-0.0.2.tar.gz` & `tmp/xdantic-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdantic-0.0.2.tar", last modified: Mon May  8 16:19:40 2023, max compression
+gzip compressed data, was "xdantic-0.0.2.dev0.tar", last modified: Tue Apr 25 09:56:54 2023, max compression
```

## Comparing `xdantic-0.0.2.tar` & `xdantic-0.0.2.dev0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0   104406 2023-04-26 09:42:31.670918 xdantic-0.0.2/.github/img/logo.png
--rw-r--r--   0        0        0      908 2023-04-25 13:23:20.142269 xdantic-0.0.2/.github/pull_reqeust_template.md
--rw-r--r--   0        0        0     2019 2023-04-25 13:27:34.678166 xdantic-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     3088 2023-04-25 13:23:20.144546 xdantic-0.0.2/.gitignore
--rw-r--r--   0        0        0     1047 2023-04-25 13:23:20.145675 xdantic-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       50 2023-04-25 13:23:20.146628 xdantic-0.0.2/LICENSE
--rw-r--r--   0        0        0     4367 2023-05-08 16:17:16.489382 xdantic-0.0.2/README.md
--rw-r--r--   0        0        0     1405 2023-04-25 13:23:20.147879 xdantic-0.0.2/README_DEV.md
--rw-r--r--   0        0        0     3236 2023-05-08 16:15:06.702574 xdantic-0.0.2/README_PYPI.md
--rw-r--r--   0        0        0     1438 2023-05-08 16:15:06.674211 xdantic-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 13:23:20.153786 xdantic-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      113 2023-05-08 16:15:06.657666 xdantic-0.0.2/src/xdantic/__init__.py
--rw-r--r--   0        0        0     7116 2023-04-25 13:45:32.906671 xdantic-0.0.2/src/xdantic/xdantic.py
--rw-r--r--   0        0        0      324 2023-04-25 13:23:20.156911 xdantic-0.0.2/test/conftest.py
--rw-r--r--   0        0        0     1104 2023-04-25 13:23:20.157872 xdantic-0.0.2/test/notebook_test/test_demo_notebook.py
--rw-r--r--   0        0        0      149 2023-04-25 13:23:20.159374 xdantic-0.0.2/test/resources/test_config_files/yaml_test.yaml
--rw-r--r--   0        0        0      157 2023-04-25 13:23:20.160377 xdantic-0.0.2/test/resources/test_config_files/yaml_test_override.yaml
--rw-r--r--   0        0        0       72 2023-04-25 13:23:20.161314 xdantic-0.0.2/test/resources/test_config_files/yaml_test_singelton_getter.yaml
--rw-r--r--   0        0        0      115 2023-04-25 13:23:20.162150 xdantic-0.0.2/test/resources/test_config_files/yaml_test_wrong_schema.yaml
--rw-r--r--   0        0        0     4184 2023-04-25 13:23:20.162978 xdantic-0.0.2/test/unit_test/test_xdantic.py
--rw-r--r--   0        0        0      933 2023-04-25 13:23:20.163668 xdantic-0.0.2/tox.ini
--rw-r--r--   0        0        0     4359 1970-01-01 00:00:00.000000 xdantic-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      908 2023-04-24 10:28:30.290694 xdantic-0.0.2.dev0/.github/pull_reqeust_template.md
+-rw-r--r--   0        0        0     2636 2023-04-24 17:39:37.044970 xdantic-0.0.2.dev0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     3088 2023-04-25 09:55:49.789990 xdantic-0.0.2.dev0/.gitignore
+-rw-r--r--   0        0        0     1047 2023-04-25 09:32:38.861333 xdantic-0.0.2.dev0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       50 2023-04-24 10:22:37.106802 xdantic-0.0.2.dev0/LICENSE
+-rw-r--r--   0        0        0     1549 2023-04-24 17:14:15.614796 xdantic-0.0.2.dev0/README.md
+-rw-r--r--   0        0        0      505 2023-04-24 16:46:33.433824 xdantic-0.0.2.dev0/mkdocs.yml
+-rw-r--r--   0        0        0     1438 2023-04-25 09:56:12.267883 xdantic-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 09:53:56.769884 xdantic-0.0.2.dev0/src/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-25 09:56:12.268968 xdantic-0.0.2.dev0/src/xdantic/__init__.py
+-rw-r--r--   0        0        0     7115 2023-04-25 09:27:57.664031 xdantic-0.0.2.dev0/src/xdantic/xdantic.py
+-rw-r--r--   0        0        0      324 2023-04-25 09:24:22.133415 xdantic-0.0.2.dev0/test/conftest.py
+-rw-r--r--   0        0        0     1104 2023-04-25 09:24:22.116776 xdantic-0.0.2.dev0/test/notebook_test/test_demo_notebook.py
+-rw-r--r--   0        0        0      149 2023-04-24 10:41:27.886722 xdantic-0.0.2.dev0/test/resources/test_config_files/yaml_test.yaml
+-rw-r--r--   0        0        0      157 2023-04-24 10:41:51.253021 xdantic-0.0.2.dev0/test/resources/test_config_files/yaml_test_override.yaml
+-rw-r--r--   0        0        0       72 2023-04-24 10:42:14.479835 xdantic-0.0.2.dev0/test/resources/test_config_files/yaml_test_singelton_getter.yaml
+-rw-r--r--   0        0        0      115 2023-04-24 10:42:34.949294 xdantic-0.0.2.dev0/test/resources/test_config_files/yaml_test_wrong_schema.yaml
+-rw-r--r--   0        0        0     4184 2023-04-25 09:24:22.121055 xdantic-0.0.2.dev0/test/unit_test/test_xdantic.py
+-rw-r--r--   0        0        0      933 2023-04-25 09:54:36.850831 xdantic-0.0.2.dev0/tox.ini
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 xdantic-0.0.2.dev0/PKG-INFO
```

### Comparing `xdantic-0.0.2/.github/pull_reqeust_template.md` & `xdantic-0.0.2.dev0/.github/pull_reqeust_template.md`

 * *Files identical despite different names*

### Comparing `xdantic-0.0.2/.github/workflows/ci.yaml` & `xdantic-0.0.2.dev0/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,34 @@
                 pytest -s test/
             - name: Save code coverage report
               uses: actions/upload-artifact@v3
               with:
                 name: code-coverage-report
                 path: tmp
 
+    build-docs:
+      runs-on: ubuntu-latest
+      steps:
+        - id: checkout
+          uses: actions/checkout@v3
+        - id: setup-python
+          uses: actions/setup-python@v4
+          with:
+            python-version: ${{ env.PYTHON_VERSION }}
+
+        - id: install-deps
+          name: Install dependencies and test
+          run: |
+            pip install --upgrade setuptools flit wheel
+            FLIT_ROOT_INSTALL=1 PIP_FIND_LINKS=deps flit install -s --deps production --extras docs
+        - id: build
+          name: Build documentation
+          run: |
+            mkdocs build --site-dir build
+
     build-package:
       runs-on: ubuntu-latest
       steps:
         - id: checkout
           uses: actions/checkout@v3
         - id: setup-python
           uses: actions/setup-python@v4
```

### Comparing `xdantic-0.0.2/.gitignore` & `xdantic-0.0.2.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `xdantic-0.0.2/.pre-commit-config.yaml` & `xdantic-0.0.2.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xdantic-0.0.2/README_DEV.md` & `xdantic-0.0.2.dev0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 - Check if you have installed the right Python version via Python --version / Python3 --version
 - Create virtual environment via `Python3.9 -m venv <env_folder>` and activate your virtual environment via `source <env_folder>/bin/activate`
   - Usually we create your <env_folder> right under project root folder
 - Install required build tools: `pip install --upgrade pip setuptools wheel flit`
   - If you don't have pip preinstalled, run `python get-pip.py`. More info from https://pip.pypa.io/en/stable/installation/
 - Install dependencies: `PIP_FIND_LINKS=deps flit install -s --deps production --extras testing`
   -If new dependency needs to be added, you should define it in file `pyproject.toml`
+- Install manually dependencies for xconfig : `pip install deps/xconfig-0.0.1.dev1.tar.gz`
+- jarvis must have a `__init__.py` file in which there must be a version number in there
+- Create empty folder data in root folder and create models and cache folders inside data folders
 
 ## How to build docs
-To build the documentation locally, install the `docs` dependency group and run:
+To build the documentation locally, install the `doc` dependency group and run:
 
 ```
 mkdocs build --site-dir build
 ```
 
 ## Tutorial
 
@@ -25,16 +28,8 @@
 
 ## Tests
 
 To run the test locally, install the `testing` dependency group and run:
 
 ```
 pytest -s test
-```
-
-## Release a new version
-
-Use bumpversion to update the project file with a new version
-
-```
-bumpversion {patch, minor, major}
-```
+```
```

### Comparing `xdantic-0.0.2/pyproject.toml` & `xdantic-0.0.2.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 ]
 
 [project]
 name = "xdantic"
 authors = [
     {name = "Sebastian Lettner", email = "sebastian.a.lettner@gmail.com"},
 ]
-readme = "README_PYPI.md"
+readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
-version = "0.0.2"
+version = "0.0.2.dev0"
 description = "A lightweight Python config library on top of Pydantic."
 
 dependencies = [
     "pydantic[dotenv]>=1.10.2",
     "pyyaml>=6.0"
 ]
```

### Comparing `xdantic-0.0.2/src/xdantic/xdantic.py` & `xdantic-0.0.2.dev0/src/xdantic/xdantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             return merged
         else:
             return self.__class__(**merged)
 
 
 class XConfigSingleton(XConfig, ABC):
     """
-    Singleton version of the XConfig class. Will save the initialization arguments in
+    Singleton version of the XConfig class. Will save the initialization argumets in
     a class scoped property, and return copies if the `xconfig_update` parameter is set to False
     """
 
     class _Single(NamedTuple):
         init_kwargs: Dict[str, Any]
         env_file: Optional[DotenvType] = None
         env_file_encoding: Optional[str] = None
```

### Comparing `xdantic-0.0.2/test/notebook_test/test_demo_notebook.py` & `xdantic-0.0.2.dev0/test/notebook_test/test_demo_notebook.py`

 * *Files identical despite different names*

### Comparing `xdantic-0.0.2/test/unit_test/test_xdantic.py` & `xdantic-0.0.2.dev0/test/unit_test/test_xdantic.py`

 * *Files identical despite different names*

### Comparing `xdantic-0.0.2/tox.ini` & `xdantic-0.0.2.dev0/tox.ini`

 * *Files identical despite different names*

