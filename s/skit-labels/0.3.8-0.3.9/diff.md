# Comparing `tmp/skit-labels-0.3.8.tar.gz` & `tmp/skit-labels-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skit-labels-0.3.8.tar", max compression
+gzip compressed data, was "skit-labels-0.3.9.tar", max compression
```

## Comparing `skit-labels-0.3.8.tar` & `skit-labels-0.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      664 2022-01-26 11:16:38.048264 skit-labels-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       22 2022-01-26 11:16:35.408264 skit-labels-0.3.8/skit_labels/__init__.py
--rw-r--r--   0        0        0     9880 2022-01-24 15:21:23.179240 skit-labels-0.3.8/skit_labels/cli.py
--rw-r--r--   0        0        0     8973 2022-01-26 10:55:38.348257 skit-labels-0.3.8/skit_labels/commands.py
--rw-r--r--   0        0        0     2760 2022-01-24 14:45:51.939228 skit-labels-0.3.8/skit_labels/constants.py
--rw-r--r--   0        0        0    14822 2022-01-24 15:21:23.259240 skit-labels-0.3.8/skit_labels/db.py
--rw-r--r--   0        0        0     6545 2022-01-24 14:45:51.939228 skit-labels-0.3.8/skit_labels/types.py
--rw-r--r--   0        0        0     1857 2022-01-24 14:45:51.939228 skit-labels-0.3.8/skit_labels/utils.py
--rw-r--r--   0        0        0     1043 2022-01-26 11:17:24.244145 skit-labels-0.3.8/setup.py
--rw-r--r--   0        0        0      866 2022-01-26 11:17:24.244397 skit-labels-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      664 2022-01-26 12:54:42.648297 skit-labels-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-01-26 12:55:21.668297 skit-labels-0.3.9/skit_labels/__init__.py
+-rw-r--r--   0        0        0    10075 2022-01-26 12:54:12.558297 skit-labels-0.3.9/skit_labels/cli.py
+-rw-r--r--   0        0        0     8973 2022-01-26 10:55:38.348257 skit-labels-0.3.9/skit_labels/commands.py
+-rw-r--r--   0        0        0     2760 2022-01-24 14:45:51.939228 skit-labels-0.3.9/skit_labels/constants.py
+-rw-r--r--   0        0        0    14822 2022-01-24 15:21:23.259240 skit-labels-0.3.9/skit_labels/db.py
+-rw-r--r--   0        0        0     6545 2022-01-24 14:45:51.939228 skit-labels-0.3.9/skit_labels/types.py
+-rw-r--r--   0        0        0     1857 2022-01-24 14:45:51.939228 skit-labels-0.3.9/skit_labels/utils.py
+-rw-r--r--   0        0        0     1043 2022-01-26 12:56:07.153644 skit-labels-0.3.9/setup.py
+-rw-r--r--   0        0        0      866 2022-01-26 12:56:07.153949 skit-labels-0.3.9/PKG-INFO
```

### Comparing `skit-labels-0.3.8/pyproject.toml` & `skit-labels-0.3.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skit-labels"
-version = "0.3.8"
+version = "0.3.9"
 description = "Command line tool for interacting with labelled datasets at skit.ai."
 authors = []
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 attrs = "^19.3.0"
```

### Comparing `skit-labels-0.3.8/skit_labels/cli.py` & `skit-labels-0.3.9/skit_labels/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,21 @@
     )
     parser.add_argument(
         "-i",
         "--input",
         type=str,
         help="The raw data to be uploaded.",
     )
+    parser.add_argument(
+        "-j",
+        "--job-id",
+        type=is_numeric,
+        required=True,
+        help="Id of the tog dataset that we want to download.",
+    )
     return parser
 
 
 def build_upload_command(parser: argparse.ArgumentParser) -> None:
     data_source_parsers = parser.add_subparsers(dest="data_source")
     upload_dataset_to_tog_command(
         data_source_parsers.add_parser(
@@ -283,15 +290,15 @@
             if is_pipe:
                 args.input = sys.stdin.readline().strip()
             else:
                 raise argparse.ArgumentTypeError(
                     "Expected to receive --input=<file> or its valued piped in."
                 )
 
-        upload_dataset(args.input, args.url, args.token, args.job_id)
+        errors, df_size = upload_dataset(args.input, args.url, args.token, args.job_id)
 
         if errors:
             error_summary = "\n".join(set(errors))
             return (
                 f"Encountered {len(errors)} over {df_size}.\nSummary:\n{error_summary}."
             )
     elif args.command == const.DESCRIBE:
```

### Comparing `skit-labels-0.3.8/skit_labels/commands.py` & `skit-labels-0.3.9/skit_labels/commands.py`

 * *Files identical despite different names*

### Comparing `skit-labels-0.3.8/skit_labels/constants.py` & `skit-labels-0.3.9/skit_labels/constants.py`

 * *Files identical despite different names*

### Comparing `skit-labels-0.3.8/skit_labels/db.py` & `skit-labels-0.3.9/skit_labels/db.py`

 * *Files identical despite different names*

### Comparing `skit-labels-0.3.8/skit_labels/types.py` & `skit-labels-0.3.9/skit_labels/types.py`

 * *Files identical despite different names*

### Comparing `skit-labels-0.3.8/skit_labels/utils.py` & `skit-labels-0.3.9/skit_labels/utils.py`

 * *Files identical despite different names*

### Comparing `skit-labels-0.3.8/setup.py` & `skit-labels-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'tqdm>=4.46.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['skit-labels = skit_labels.cli:main']}
 
 setup_kwargs = {
     'name': 'skit-labels',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Command line tool for interacting with labelled datasets at skit.ai.',
     'long_description': None,
     'author': None,
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `skit-labels-0.3.8/PKG-INFO` & `skit-labels-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skit-labels
-Version: 0.3.8
+Version: 0.3.9
 Summary: Command line tool for interacting with labelled datasets at skit.ai.
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

