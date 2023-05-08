# Comparing `tmp/pyproject_pre_commit-0.0.8.tar.gz` & `tmp/pyproject_pre_commit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_pre_commit-0.0.8.tar", max compression
+gzip compressed data, was "pyproject_pre_commit-0.0.9.tar", max compression
```

## Comparing `pyproject_pre_commit-0.0.8.tar` & `pyproject_pre_commit-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11337 2023-04-24 01:02:50.116757 pyproject_pre_commit-0.0.8/LICENSE
--rw-r--r--   0        0        0     5374 2023-04-24 01:02:50.116757 pyproject_pre_commit-0.0.8/README.md
--rw-r--r--   0        0        0     2944 2023-04-24 01:02:51.068768 pyproject_pre_commit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      118 2023-04-24 01:02:51.068768 pyproject_pre_commit-0.0.8/src/pyproject_pre_commit/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-24 01:02:50.116757 pyproject_pre_commit-0.0.8/src/pyproject_pre_commit/pyproject_pre_commit.py
--rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-05-08 01:00:00.632696 pyproject_pre_commit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5374 2023-05-08 01:00:00.632696 pyproject_pre_commit-0.0.9/README.md
+-rw-r--r--   0        0        0     2944 2023-05-08 01:00:01.148700 pyproject_pre_commit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-08 01:00:01.152700 pyproject_pre_commit-0.0.9/src/pyproject_pre_commit/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-08 01:00:00.632696 pyproject_pre_commit-0.0.9/src/pyproject_pre_commit/pyproject_pre_commit.py
+-rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.0.9/PKG-INFO
```

### Comparing `pyproject_pre_commit-0.0.8/LICENSE` & `pyproject_pre_commit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.8/README.md` & `pyproject_pre_commit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.8/pyproject.toml` & `pyproject_pre_commit-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyproject-pre-commit"
-version = "0.0.8"
+version = "0.0.9"
 description = "pre-commit hooks for python projects using pyproject.toml."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/pyproject-pre-commit"
 homepage = "https://github.com/rcmdnk/pyproject-pre-commit"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["pre-commit", "pyproject.toml", "poetry"]
@@ -16,15 +16,15 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-pre-commit = "3.2.2"
+pre-commit = "3.3.1"
 black = "23.3.0"
 blacken-docs = "1.13.0"
 flake8-pyproject = "1.2.3"
 flake8-annotations-complexity = "0.0.7"
 flake8-bugbear = "23.3.23"
 flake8-builtins = "2.1.0"
 flake8-comprehensions = "3.12.0"
```

### Comparing `pyproject_pre_commit-0.0.8/src/pyproject_pre_commit/pyproject_pre_commit.py` & `pyproject_pre_commit-0.0.9/src/pyproject_pre_commit/pyproject_pre_commit.py`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.8/PKG-INFO` & `pyproject_pre_commit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-pre-commit
-Version: 0.0.8
+Version: 0.0.9
 Summary: pre-commit hooks for python projects using pyproject.toml.
 Home-page: https://github.com/rcmdnk/pyproject-pre-commit
 License: Apache-2.0
 Keywords: pre-commit,pyproject.toml,poetry
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -40,15 +40,15 @@
 Requires-Dist: isort (==5.12.0)
 Requires-Dist: mdformat (==0.7.16)
 Requires-Dist: mdformat-footnote (==0.1.1)
 Requires-Dist: mdformat-frontmatter (==2.0.1)
 Requires-Dist: mdformat-gfm (==0.3.5)
 Requires-Dist: mypy (==1.2.0)
 Requires-Dist: pep8-naming (==0.13.3)
-Requires-Dist: pre-commit (==3.2.2)
+Requires-Dist: pre-commit (==3.3.1)
 Requires-Dist: pycodestyle (==2.10.0)
 Requires-Dist: shellcheck-py (==0.9.0.2)
 Project-URL: Repository, https://github.com/rcmdnk/pyproject-pre-commit
 Description-Content-Type: text/markdown
 
 # pyproject-pre-commit
```

