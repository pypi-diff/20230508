# Comparing `tmp/raga-cli-0.1.8.tar.gz` & `tmp/raga-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.1.8.tar", last modified: Thu May  4 07:16:41 2023, max compression
+gzip compressed data, was "raga-cli-0.1.9.tar", last modified: Mon May  8 08:54:47 2023, max compression
```

## Comparing `raga-cli-0.1.8.tar` & `raga-cli-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.401707 raga-cli-0.1.8/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.8/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.8/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-04 07:16:41.401297 raga-cli-0.1.8/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.8/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-05-04 07:15:56.000000 raga-cli-0.1.8/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.393064 raga-cli-0.1.8/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      631 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.394040 raga-cli-0.1.8/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.395657 raga-cli-0.1.8/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.8/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.8/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2073 2023-05-04 07:16:17.000000 raga-cli-0.1.8/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)    13691 2023-05-04 06:38:24.000000 raga-cli-0.1.8/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.397134 raga-cli-0.1.8/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3406 2023-05-04 07:06:44.000000 raga-cli-0.1.8/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.8/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1915 2023-05-04 06:33:09.000000 raga-cli-0.1.8/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)    10482 2023-05-04 07:09:20.000000 raga-cli-0.1.8/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.398218 raga-cli-0.1.8/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5589 2023-05-04 06:38:29.000000 raga-cli-0.1.8/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.8/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.398644 raga-cli-0.1.8/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.400709 raga-cli-0.1.8/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1906 2023-05-04 06:47:33.000000 raga-cli-0.1.8/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1996 2023-05-01 08:38:56.000000 raga-cli-0.1.8/rc/utils/config.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6905 2023-05-04 06:55:58.000000 raga-cli-0.1.8/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-05-01 07:24:17.000000 raga-cli-0.1.8/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-05-04 07:16:41.401796 raga-cli-0.1.8/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.8/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.134624 raga-cli-0.1.9/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.9/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.9/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-08 08:54:47.134328 raga-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.9/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-05-08 08:54:27.000000 raga-cli-0.1.9/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.128021 raga-cli-0.1.9/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-08 08:54:47.000000 raga-cli-0.1.9/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      631 2023-05-08 08:54:47.000000 raga-cli-0.1.9/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-05-08 08:54:47.000000 raga-cli-0.1.9/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-05-08 08:54:47.000000 raga-cli-0.1.9/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-05-08 08:54:47.000000 raga-cli-0.1.9/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-05-08 08:54:47.000000 raga-cli-0.1.9/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.128798 raga-cli-0.1.9/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.129879 raga-cli-0.1.9/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-05-04 13:40:59.000000 raga-cli-0.1.9/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-05-05 04:22:34.000000 raga-cli-0.1.9/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2073 2023-05-08 08:54:33.000000 raga-cli-0.1.9/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    15667 2023-05-08 08:49:53.000000 raga-cli-0.1.9/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.131045 raga-cli-0.1.9/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3406 2023-05-04 07:06:44.000000 raga-cli-0.1.9/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.9/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1915 2023-05-05 06:27:21.000000 raga-cli-0.1.9/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    10482 2023-05-04 07:09:20.000000 raga-cli-0.1.9/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-05-05 04:22:34.000000 raga-cli-0.1.9/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.9/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.131837 raga-cli-0.1.9/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.9/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5668 2023-05-08 08:41:20.000000 raga-cli-0.1.9/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.9/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.132113 raga-cli-0.1.9/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.9/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-08 08:54:47.133844 raga-cli-0.1.9/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1906 2023-05-04 06:47:33.000000 raga-cli-0.1.9/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.9/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1996 2023-05-01 08:38:56.000000 raga-cli-0.1.9/rc/utils/config.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.9/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     8149 2023-05-08 08:13:47.000000 raga-cli-0.1.9/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-05-01 07:24:17.000000 raga-cli-0.1.9/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.9/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-05-08 08:54:47.134685 raga-cli-0.1.9/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.9/setup.py
```

### Comparing `raga-cli-0.1.8/.gitignore` & `raga-cli-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/LICENSE` & `raga-cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/PKG-INFO` & `raga-cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.8/pyproject.toml` & `raga-cli-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.1.8/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.9/raga_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.8/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.9/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.9/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/cli/__init__.py` & `raga-cli-0.1.9/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/cli/parser.py` & `raga-cli-0.1.9/rc/cli/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         add_help=False,
     )
 
     parser.add_argument(
         "-V",
         "--version",
         action="version",
-        version='0.1.8',
+        version='0.1.9',
         help="Show program's version.",
     )
 
     # Sub commands
     subparsers = parser.add_subparsers(
         title="Available Commands",
         metavar="COMMAND",
```

### Comparing `raga-cli-0.1.8/rc/cli/utils.py` & `raga-cli-0.1.9/rc/cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 import sys
 from rc.utils import DEBUG
 from multiprocessing import cpu_count
 from pathlib import Path
 import pathlib
 import re
 from datetime import datetime
+from rc.utils.config import get_config_value
+import glob
 
-from rc.utils.request import get_commit_repo, get_config_value_by_key, get_repo_version
+from rc.utils.request import dataset_upload_web, get_commit_repo, get_config_value_by_key, get_repo_version, model_upload_web
 
 logger = logging.getLogger(__name__)
 
 class RctlValidSubprocessError(Exception):
     def __init__(self, msg, *args):
         assert msg
         self.msg = msg
@@ -182,15 +184,15 @@
         str = str.rsplit("/", 1)[0] 
     return str
 
 def valid_cwd_rc():
     cwd = os.getcwd()   # get the current working directory
     rc_dir = os.path.join(cwd, ".rc")   # create a path to the .rc directory
     if not os.path.isdir(rc_dir):   # check if the path is a directory
-        print("Your current location is not a root directory location.")
+        print("Your current location is not a rc repo directory location.")
         sys.exit()
     return True
 
 def find_dvc_files():
     files = []
     cwd = os.getcwd()   # get the current working directory
     for file in os.listdir(cwd):   # iterate through the files in the current directory
@@ -298,14 +300,55 @@
         children = [path_to_dict(os.path.join(path, x)) for x in os.listdir(path)]
         d['children'] = [c for c in children if c is not None]
     else:
         d['type'] = "file"
         d['last_updated'] = datetime.fromtimestamp(os.path.getmtime(path)).strftime('%Y-%m-%d %H:%M:%S')
     return d
 
+def get_infra_file():
+    json_files = glob.glob("executions" + '/*.json')
+    if json_files:
+        if len(json_files) > 1:
+            print("Execution file can not be grater than 1")
+            sys.exit()
+        logger.debug(f"Infra file: {json_files[0]}")
+        return json_files[0]
+    print("Executions dir or execution json file does not exists.")
+    sys.exit()
+
+
+def upload_infra_json(version, cwd = None):
+    if cwd:
+        owd = os.getcwd()
+        os.chdir(f"{owd}/{cwd}") 
+    model_version = int(version)-1 if version else 1
+    logger.debug("INFRA FILE UPLOADING")
+    import botocore.session   
+    infra_file = get_infra_file()
+    CLOUD_STORAGE_BUCKET = get_config_value_by_key('bucket_name')
+    CLOUD_STORAGE_DIR = get_config_value_by_key('cloud_storage_dir')
+    AWS_SECRET = get_config_value_by_key('remote_storage_secret_key')
+    AWS_ACCESS = get_config_value_by_key('remote_storage_access_key')
+    repo = get_repo()
+    dest = f"{CLOUD_STORAGE_DIR}/{repo}/versions/{model_version}/result.json"
+    # Create a botocore session with the AWS access key and secret key
+    session = botocore.session.Session()
+    session.set_credentials(AWS_ACCESS, AWS_SECRET)
+
+    # Create an S3 client using the botocore session
+    s3 = session.create_client('s3')
+
+    # Upload the file to S3
+    with open(infra_file, 'rb') as file:
+        s3.put_object(Bucket=CLOUD_STORAGE_BUCKET, Key=dest, Body=file)          
+
+    if cwd:
+        os.chdir(owd)
+
+
 def upload_model_file_list_json(version, cwd = None):
     if cwd:
         owd = os.getcwd()
         os.chdir(f"{owd}/{cwd}") 
     logger.debug("MODEL FILE UPLOADING")
     import botocore.session   
     model_file_list = json.loads(json.dumps(path_to_dict('.')))
@@ -366,8 +409,18 @@
         return f_retry
     return deco_retry
 
 
 def folder_exists(folder_name):
     current_dir = os.getcwd()
     folder_path = os.path.join(current_dir, folder_name)
-    return os.path.exists(folder_path) and os.path.isdir(folder_path)
+    return os.path.exists(folder_path) and os.path.isdir(folder_path)
+
+def upload_model(model, version):
+    model_version = int(version)-1 if version else 1
+    model_name = f"{model}:version{model_version}"
+    model_upload_web(model_name, 2)
+
+def upload_dataset(dataset, version):
+    dataset_name = f"{dataset}:version{version}"
+    media_path = f"{get_config_value('remote_bucket_location')}/{get_config_value('repo')}"
+    dataset_upload_web(dataset_name, 2, media_path)
```

### Comparing `raga-cli-0.1.8/rc/commands/get.py` & `raga-cli-0.1.9/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/commands/list.py` & `raga-cli-0.1.9/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/commands/put.py` & `raga-cli-0.1.9/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/commands/repo.py` & `raga-cli-0.1.9/rc/commands/repo.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/exceptions.py` & `raga-cli-0.1.9/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/prompt.py` & `raga-cli-0.1.9/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/repo/get.py` & `raga-cli-0.1.9/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/repo/put.py` & `raga-cli-0.1.9/rc/repo/put.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,52 +33,51 @@
     if not is_current_version_stable():
         return False   
     print("Files uploading...")   
     paths = back_slash_trim(paths)
 
     for path in paths:
         dir_add(path)
-    dir_upload(paths)
     for path in paths:     
         md5_dir = get_dir_file(path)          
         request_payload = {
             "folder": path,
             "commit_message" : message,
             "repo" : repo,
             "dir_file":md5_dir,
             "version":current_version,
             "commit_id":"",
         }   
         commit_id = insert_repo_commit(json.dumps(request_payload))
         repo_commit_ids.append(commit_id['id'])
         logger.debug("Data upload for {}".format(path))
-    
+    dir_upload(paths)
     stop_checking_elastic_process = False
     while not stop_checking_elastic_process:
         stop_checking_elastic_process = server_repo_commit_status(repo_commit_ids)
         if not stop_checking_elastic_process:
             time.sleep(pool_time)
     return True
 
 def model_upload(message, repo, model_version):
-    update_repo_lock(repo, json.dumps({"locked":True}))
     print("Model files uploading...")
     commit_hash = current_commit_hash()
     if get_commit_version(commit_hash):
-        print("The latest commit is unchanged.")
+        print("There are no changes since last update.")
         sys.exit(50)
     branchName = current_branch()
     request_payload = {
                 "commit_message" : message,
                 "repo" : repo,
                 "commit_id":commit_hash,
                 "version":model_version,
                 "branch":branchName
             }  
     upload_model_file_list_json(commit_hash)
+    upload_infra_json(model_version)
     insert_repo_commit(json.dumps(request_payload))
     logger.debug("Data upload for branch {0} and {1} ".format(branchName,commit_hash ))
     print("Model files uploaded successfully")
 
 def make_repo_lock(stop_event):
     logger.debug("START HTTP THREAD")
     repo = get_repo() 
@@ -123,14 +122,16 @@
         http_thread = threading.Thread(target=make_repo_lock, args=(stop_event,))
         http_thread.start() 
         try:
             if dataset_upload(paths,message,repo, current_version):
                 # Set the stop event
                 stop_event.set()
                 update_repo_lock(repo, json.dumps({"locked":False}))
+                upload_dataset(repo, current_version)
+                make_repo_commit(message)
             else:
                 # Set the stop event
                 stop_event.set()
                 update_repo_lock(repo, json.dumps({"locked":False}))
         except Exception as e:
             # Set the stop event
             stop_event.set()
@@ -138,19 +139,18 @@
             print("Something went wrong.")
             logger.exception(e)
             sys.exit()
         # Start both threads
         
         # Wait for both threads to finish
         http_thread.join()
-        make_repo_commit(message)
-        
     elif tag == "model":
         check_extensions()
         if check_push_left():
             print('Please use "git push" to publish your local commits')
             sys.exit()
         model_version = model_current_version(repo)
         model_upload(message, repo, model_version)
+        upload_model(repo, model_version)
     
     update_repo_lock(repo, json.dumps({"locked":False}))
     logger.debug('TOTAL UPLOAD TIME {0}'.format(timedelta(seconds=timer()-start)))
```

### Comparing `raga-cli-0.1.8/rc/utils/__init__.py` & `raga-cli-0.1.9/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/utils/config.py` & `raga-cli-0.1.9/rc/utils/config.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.8/rc/utils/request.py` & `raga-cli-0.1.9/rc/utils/request.py`

 * *Files 15% similar despite different names*

```diff
@@ -184,12 +184,34 @@
 def get_commit_repo(id):
     url = f"{BASE_URL}/repocommit?key={id}"
     response = valid_response(make_request(url, "GET"))
     data = response["data"]
     logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
     return data
 
-# def model_upload_web():
+def model_upload_web(model, project=None):
+    from rc.utils.config import get_config_value
+    url = f"{WEB_BACKEND_URL}/model-upload?modelName={model}&projectId={project}"
+    response = valid_response(make_request(url, "POST", None, get_config_value('auth_token')))
+    data = response
+    logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
+    return data
+
+def dataset_upload_web(dataset, project=None, media_path=None):
+    from rc.utils.config import get_config_value
+    url = f"{WEB_BACKEND_URL}/dataSet/upload?dataSetName={dataset}&projectId={project}&mediaPath={media_path}"
+    response = valid_response(make_request(url, "POST", None, get_config_value('auth_token')))
+    data = response
+    logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
+    return data
+
+def update_model_execution_status(dataset, project=None, model=None):
+    from rc.utils.config import get_config_value
+    url = f"{WEB_BACKEND_URL}/modelExecutionStatus/update?project={project}&dataset={dataset}&model={model}"
+    response = valid_response(make_request(url, "POST", None, get_config_value('auth_token')))
+    data = response
+    logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
+    return data
```

### Comparing `raga-cli-0.1.8/rc/utils/sshKeyGen.py` & `raga-cli-0.1.9/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

