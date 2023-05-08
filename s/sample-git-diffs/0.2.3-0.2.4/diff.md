# Comparing `tmp/sample-git-diffs-0.2.3.tar.gz` & `tmp/sample-git-diffs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-git-diffs-0.2.3.tar", max compression
+gzip compressed data, was "sample-git-diffs-0.2.4.tar", max compression
```

## Comparing `sample-git-diffs-0.2.3.tar` & `sample-git-diffs-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      441 2023-01-16 14:40:19.027075 sample-git-diffs-0.2.3/README.md
--rw-r--r--   0        0        0      483 2023-01-16 15:12:33.605628 sample-git-diffs-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.2.3/sample_git_diffs/__init__.py
--rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.2.3/sample_git_diffs/sample_git_diffs.py
--rw-r--r--   0        0        0     1242 2023-01-16 15:12:41.909346 sample-git-diffs-0.2.3/setup.py
--rw-r--r--   0        0        0     1053 2023-01-16 15:12:41.909508 sample-git-diffs-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      441 2023-01-16 14:40:19.027075 sample-git-diffs-0.2.4/README.md
+-rw-r--r--   0        0        0      478 2023-05-08 10:00:22.968024 sample-git-diffs-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.2.4/sample_git_diffs/__init__.py
+-rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.2.4/sample_git_diffs/sample_git_diffs.py
+-rw-r--r--   0        0        0     1228 2023-05-08 10:00:27.534187 sample-git-diffs-0.2.4/setup.py
+-rw-r--r--   0        0        0     1036 2023-05-08 10:00:27.534374 sample-git-diffs-0.2.4/PKG-INFO
```

### Comparing `sample-git-diffs-0.2.3/sample_git_diffs/sample_git_diffs.py` & `sample-git-diffs-0.2.4/sample_git_diffs/sample_git_diffs.py`

 * *Files identical despite different names*

### Comparing `sample-git-diffs-0.2.3/setup.py` & `sample-git-diffs-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['sample_git_diffs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=1.4.0,<2.0.0']
+['pandas']
 
 entry_points = \
 {'console_scripts': ['sample-git-diffs = '
                      'sample_git_diffs.sample_git_diffs:cli']}
 
 setup_kwargs = {
     'name': 'sample-git-diffs',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': '',
     'long_description': '# sample-git-diffs\n\n```\nSample git diffs uniformly wrt. number of changes per file. The output is formatted as a .diff file.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --n N                 Total number of diffs to be sampled\n  --diffstat DIFFSTAT   Custom git diff command for the sampling probabilities\n  --diffcommand DIFFCOMMAND\n                        Custom git diff command for the actual diff\n```\n',
     'author': 'ninpnin',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ninpnin/sample-git-diffs',
```

### Comparing `sample-git-diffs-0.2.3/PKG-INFO` & `sample-git-diffs-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sample-git-diffs
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Home-page: https://github.com/ninpnin/sample-git-diffs
 License: MIT
 Author: ninpnin
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pandas (>=1.4.0,<2.0.0)
+Requires-Dist: pandas
 Project-URL: Repository, https://github.com/ninpnin/sample-git-diffs
 Description-Content-Type: text/markdown
 
 # sample-git-diffs
 
 ```
 Sample git diffs uniformly wrt. number of changes per file. The output is formatted as a .diff file.
```

