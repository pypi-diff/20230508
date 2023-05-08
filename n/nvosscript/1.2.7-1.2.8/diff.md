# Comparing `tmp/nvosscript-1.2.7.tar.gz` & `tmp/nvosscript-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.2.7.tar", last modified: Mon May  8 02:37:15 2023, max compression
+gzip compressed data, was "nvosscript-1.2.8.tar", last modified: Mon May  8 02:53:25 2023, max compression
```

## Comparing `nvosscript-1.2.7.tar` & `nvosscript-1.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:37:15.995419 nvosscript-1.2.7/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.7/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-08 02:37:15.995268 nvosscript-1.2.7/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.7/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:37:15.991675 nvosscript-1.2.7/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.7/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    13019 2023-04-25 03:18:40.000000 nvosscript-1.2.7/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-24 10:46:35.000000 nvosscript-1.2.7/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8571 2023-04-25 06:40:19.000000 nvosscript-1.2.7/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4796 2023-04-24 10:50:50.000000 nvosscript-1.2.7/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      985 2023-04-25 03:15:56.000000 nvosscript-1.2.7/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:37:15.992816 nvosscript-1.2.7/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-08 02:37:15.000000 nvosscript-1.2.7/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      474 2023-05-08 02:37:15.000000 nvosscript-1.2.7/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-05-08 02:37:15.000000 nvosscript-1.2.7/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-05-08 02:37:15.000000 nvosscript-1.2.7/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-05-08 02:37:15.000000 nvosscript-1.2.7/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-05-08 02:37:15.000000 nvosscript-1.2.7/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-05-08 02:37:15.995463 nvosscript-1.2.7/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-05-08 02:34:48.000000 nvosscript-1.2.7/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:37:15.993614 nvosscript-1.2.7/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.2.7/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      712 2023-04-25 06:34:28.000000 nvosscript-1.2.7/skyeye/datahandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1797 2023-04-25 03:19:08.000000 nvosscript-1.2.7/skyeye/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      240 2023-04-24 10:14:48.000000 nvosscript-1.2.7/skyeye/skyeyecommand.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:37:15.994734 nvosscript-1.2.7/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.7/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      185 2023-04-25 03:16:06.000000 nvosscript-1.2.7/start/commonUtil.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4529 2023-05-08 02:34:59.000000 nvosscript-1.2.7/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:37:15.994963 nvosscript-1.2.7/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1273 2023-04-24 10:15:28.000000 nvosscript-1.2.7/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.127411 nvosscript-1.2.8/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.8/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-08 02:53:25.127238 nvosscript-1.2.8/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.8/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.123672 nvosscript-1.2.8/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.8/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    13019 2023-05-08 02:51:58.000000 nvosscript-1.2.8/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-24 10:46:35.000000 nvosscript-1.2.8/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8571 2023-04-25 06:40:19.000000 nvosscript-1.2.8/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4796 2023-04-24 10:50:50.000000 nvosscript-1.2.8/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      985 2023-04-25 03:15:56.000000 nvosscript-1.2.8/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.124739 nvosscript-1.2.8/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      474 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-05-08 02:53:25.127460 nvosscript-1.2.8/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-05-08 02:52:29.000000 nvosscript-1.2.8/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.125506 nvosscript-1.2.8/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.2.8/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      712 2023-04-25 06:34:28.000000 nvosscript-1.2.8/skyeye/datahandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1797 2023-04-25 03:19:08.000000 nvosscript-1.2.8/skyeye/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      240 2023-04-24 10:14:48.000000 nvosscript-1.2.8/skyeye/skyeyecommand.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.126607 nvosscript-1.2.8/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.8/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      185 2023-04-25 03:16:06.000000 nvosscript-1.2.8/start/commonUtil.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4529 2023-05-08 02:52:35.000000 nvosscript-1.2.8/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.126895 nvosscript-1.2.8/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1273 2023-04-24 10:15:28.000000 nvosscript-1.2.8/win/win_auto_script.py
```

### Comparing `nvosscript-1.2.7/LICENSE` & `nvosscript-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/nvos/file.py` & `nvosscript-1.2.8/nvos/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     for temp in file_list:
         if "%s_%s" % (temp["file_path"], temp["git_branch"]) not in origin_file_map:
             add_file_list.append(temp)
     logger.info(f"push add_file_list: {add_file_list}")
     if len(add_file_list) > 0:
         remote.upload_file(add_file_list, project_space_list)
         logger.info(f"start save all file config ")
-        origin_file_list.append(add_file_list)
+        origin_file_list.extend(add_file_list)
         with open(os.path.join(nvos_path, "config"), 'w') as f:
             for item in origin_file_list:
                 f.write(json.dumps(item) + "\n")
 
 
 # 同步项目数据到远程
 def sync_project_data(workspace_path):
```

### Comparing `nvosscript-1.2.7/nvos/login.py` & `nvosscript-1.2.8/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/nvos/remote.py` & `nvosscript-1.2.8/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/nvos/run.py` & `nvosscript-1.2.8/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/nvos/utils.py` & `nvosscript-1.2.8/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/setup.py` & `nvosscript-1.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.2.7',
+    version='1.2.8',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.2.7/skyeye/datahandler.py` & `nvosscript-1.2.8/skyeye/datahandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/skyeye/remote.py` & `nvosscript-1.2.8/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.7/start/main.py` & `nvosscript-1.2.8/start/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.type)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.2.7")
+        print("1.2.8")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.2.7/win/win_auto_script.py` & `nvosscript-1.2.8/win/win_auto_script.py`

 * *Files identical despite different names*

