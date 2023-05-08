# Comparing `tmp/ansible-butler-1.0.8.tar.gz` & `tmp/ansible-butler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-butler-1.0.8.tar", last modified: Fri May  5 16:29:00 2023, max compression
+gzip compressed data, was "ansible-butler-1.0.9.tar", last modified: Mon May  8 02:35:41 2023, max compression
```

## Comparing `ansible-butler-1.0.8.tar` & `ansible-butler-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.947415 ansible-butler-1.0.8/
--rw-r--r--   0 zach       (501) staff       (20)      387 2023-02-16 18:57:23.000000 ansible-butler-1.0.8/.ansible-butler.yml
--rw-r--r--   0 zach       (501) staff       (20)     1908 2023-02-16 18:58:06.000000 ansible-butler-1.0.8/.gitignore
--rw-r--r--   0 zach       (501) staff       (20)    35149 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/LICENSE
--rw-r--r--   0 zach       (501) staff       (20)       43 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/MANIFEST.in
--rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:29:00.947551 ansible-butler-1.0.8/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     2525 2023-02-16 18:54:36.000000 ansible-butler-1.0.8/README.md
--rw-r--r--   0 zach       (501) staff       (20)      392 2023-02-16 18:58:41.000000 ansible-butler-1.0.8/ansible-butler.yml
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.942934 ansible-butler-1.0.8/ansible_butler.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)      837 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)       54 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/entry_points.txt
--rw-r--r--   0 zach       (501) staff       (20)       42 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/requires.txt
--rw-r--r--   0 zach       (501) staff       (20)       14 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/top_level.txt
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.943529 ansible-butler-1.0.8/ansiblebutler/
--rw-r--r--   0 zach       (501) staff       (20)     1062 2023-02-16 18:46:37.000000 ansible-butler-1.0.8/ansiblebutler/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)       68 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/__main__.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.944022 ansible-butler-1.0.8/ansiblebutler/common/
--rw-r--r--   0 zach       (501) staff       (20)      403 2023-02-16 18:19:30.000000 ansible-butler-1.0.8/ansiblebutler/common/.ansible-butler.yml
--rw-r--r--   0 zach       (501) staff       (20)     2177 2023-05-05 02:05:35.000000 ansible-butler-1.0.8/ansiblebutler/common/__init__.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.945037 ansible-butler-1.0.8/ansiblebutler/directory/
--rw-r--r--   0 zach       (501) staff       (20)      355 2023-02-16 18:19:44.000000 ansible-butler-1.0.8/ansiblebutler/directory/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      857 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/directory/_clean.py
--rw-r--r--   0 zach       (501) staff       (20)      975 2023-02-16 18:19:42.000000 ansible-butler-1.0.8/ansiblebutler/directory/_initialize.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.945370 ansible-butler-1.0.8/ansiblebutler/directory/templates/
--rw-r--r--   0 zach       (501) staff       (20)      213 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/directory/templates/playbook.yml.j2
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.946712 ansible-butler-1.0.8/ansiblebutler/roles/
--rw-r--r--   0 zach       (501) staff       (20)      525 2023-02-12 15:35:55.000000 ansible-butler-1.0.8/ansiblebutler/roles/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      279 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/roles/_clean.py
--rw-r--r--   0 zach       (501) staff       (20)       71 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/roles/_list.py
--rw-r--r--   0 zach       (501) staff       (20)     1242 2023-05-05 16:27:29.000000 ansible-butler-1.0.8/ansiblebutler/roles/_mkreadme.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.946898 ansible-butler-1.0.8/ansiblebutler/roles/templates/
--rw-r--r--   0 zach       (501) staff       (20)     2980 2023-05-05 16:20:23.000000 ansible-butler-1.0.8/ansiblebutler/roles/templates/README.md.j2
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.938758 ansible-butler-1.0.8/docs/
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.947075 ansible-butler-1.0.8/docs/config/
--rw-r--r--   0 zach       (501) staff       (20)      486 2023-02-16 18:28:54.000000 ansible-butler-1.0.8/docs/config/.ansible-butler.example.yml
--rwxr-xr-x   0 zach       (501) staff       (20)      161 2023-02-02 23:36:43.000000 ansible-butler-1.0.8/package.sh
--rw-r--r--   0 zach       (501) staff       (20)      147 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/pyproject.toml
--rw-r--r--   0 zach       (501) staff       (20)      828 2023-05-05 16:29:00.947909 ansible-butler-1.0.8/setup.cfg
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.885632 ansible-butler-1.0.9/
+-rw-r--r--   0 zach       (501) staff       (20)      445 2023-05-08 02:34:16.000000 ansible-butler-1.0.9/.ansible-butler.yml
+-rw-r--r--   0 zach       (501) staff       (20)     1908 2023-02-16 18:58:06.000000 ansible-butler-1.0.9/.gitignore
+-rw-r--r--   0 zach       (501) staff       (20)    35149 2023-02-02 23:05:59.000000 ansible-butler-1.0.9/LICENSE
+-rw-r--r--   0 zach       (501) staff       (20)       59 2023-05-07 17:53:17.000000 ansible-butler-1.0.9/MANIFEST.in
+-rw-r--r--   0 zach       (501) staff       (20)     3662 2023-05-08 02:35:41.885799 ansible-butler-1.0.9/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     3096 2023-05-07 17:50:04.000000 ansible-butler-1.0.9/README.md
+-rw-r--r--   0 zach       (501) staff       (20)      392 2023-05-07 17:37:15.000000 ansible-butler-1.0.9/ansible-butler.yml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.881053 ansible-butler-1.0.9/ansible_butler.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     3662 2023-05-08 02:35:41.000000 ansible-butler-1.0.9/ansible_butler.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     1208 2023-05-08 02:35:41.000000 ansible-butler-1.0.9/ansible_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-08 02:35:41.000000 ansible-butler-1.0.9/ansible_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)       54 2023-05-08 02:35:41.000000 ansible-butler-1.0.9/ansible_butler.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (501) staff       (20)       59 2023-05-08 02:35:41.000000 ansible-butler-1.0.9/ansible_butler.egg-info/requires.txt
+-rw-r--r--   0 zach       (501) staff       (20)       14 2023-05-08 02:35:41.000000 ansible-butler-1.0.9/ansible_butler.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.881394 ansible-butler-1.0.9/ansiblebutler/
+-rw-r--r--   0 zach       (501) staff       (20)     1264 2023-05-07 17:32:39.000000 ansible-butler-1.0.9/ansiblebutler/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)       68 2023-02-02 23:05:59.000000 ansible-butler-1.0.9/ansiblebutler/__main__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.881678 ansible-butler-1.0.9/ansiblebutler/common/
+-rw-r--r--   0 zach       (501) staff       (20)      753 2023-05-07 17:26:15.000000 ansible-butler-1.0.9/ansiblebutler/common/.ansible-butler.yml
+-rw-r--r--   0 zach       (501) staff       (20)     2287 2023-05-08 02:32:46.000000 ansible-butler-1.0.9/ansiblebutler/common/__init__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.882403 ansible-butler-1.0.9/ansiblebutler/directory/
+-rw-r--r--   0 zach       (501) staff       (20)      355 2023-02-16 18:19:44.000000 ansible-butler-1.0.9/ansiblebutler/directory/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      857 2023-02-02 23:05:59.000000 ansible-butler-1.0.9/ansiblebutler/directory/_clean.py
+-rw-r--r--   0 zach       (501) staff       (20)      975 2023-02-16 18:19:42.000000 ansible-butler-1.0.9/ansiblebutler/directory/_initialize.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.882634 ansible-butler-1.0.9/ansiblebutler/directory/templates/
+-rw-r--r--   0 zach       (501) staff       (20)      247 2023-05-07 17:07:02.000000 ansible-butler-1.0.9/ansiblebutler/directory/templates/playbook.yml.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.883296 ansible-butler-1.0.9/ansiblebutler/execution_environment/
+-rw-r--r--   0 zach       (501) staff       (20)      262 2023-05-07 17:26:48.000000 ansible-butler-1.0.9/ansiblebutler/execution_environment/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      820 2023-05-07 17:13:35.000000 ansible-butler-1.0.9/ansiblebutler/execution_environment/_initialize.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.883973 ansible-butler-1.0.9/ansiblebutler/execution_environment/templates/
+-rw-r--r--   0 zach       (501) staff       (20)       69 2023-05-07 17:43:53.000000 ansible-butler-1.0.9/ansiblebutler/execution_environment/templates/bindep.txt.j2
+-rw-r--r--   0 zach       (501) staff       (20)      748 2023-05-07 17:44:43.000000 ansible-butler-1.0.9/ansiblebutler/execution_environment/templates/execution-environment.yml.j2
+-rw-r--r--   0 zach       (501) staff       (20)       69 2023-05-07 17:44:46.000000 ansible-butler-1.0.9/ansiblebutler/execution_environment/templates/requirements.txt.j2
+-rw-r--r--   0 zach       (501) staff       (20)       89 2023-05-07 17:44:48.000000 ansible-butler-1.0.9/ansiblebutler/execution_environment/templates/requirements.yml.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.884604 ansible-butler-1.0.9/ansiblebutler/roles/
+-rw-r--r--   0 zach       (501) staff       (20)      525 2023-02-12 15:35:55.000000 ansible-butler-1.0.9/ansiblebutler/roles/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      279 2023-02-02 23:05:59.000000 ansible-butler-1.0.9/ansiblebutler/roles/_clean.py
+-rw-r--r--   0 zach       (501) staff       (20)       71 2023-02-02 23:05:59.000000 ansible-butler-1.0.9/ansiblebutler/roles/_list.py
+-rw-r--r--   0 zach       (501) staff       (20)     1242 2023-05-05 16:27:29.000000 ansible-butler-1.0.9/ansiblebutler/roles/_mkreadme.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.884871 ansible-butler-1.0.9/ansiblebutler/roles/templates/
+-rw-r--r--   0 zach       (501) staff       (20)     2980 2023-05-05 16:20:23.000000 ansible-butler-1.0.9/ansiblebutler/roles/templates/README.md.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.877769 ansible-butler-1.0.9/docs/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-08 02:35:41.885318 ansible-butler-1.0.9/docs/config/
+-rw-r--r--   0 zach       (501) staff       (20)      486 2023-02-16 18:28:54.000000 ansible-butler-1.0.9/docs/config/.ansible-butler.test-plugins.yml
+-rwxr-xr-x   0 zach       (501) staff       (20)      161 2023-02-02 23:36:43.000000 ansible-butler-1.0.9/package.sh
+-rw-r--r--   0 zach       (501) staff       (20)      147 2023-02-02 23:05:59.000000 ansible-butler-1.0.9/pyproject.toml
+-rw-r--r--   0 zach       (501) staff       (20)      846 2023-05-08 02:35:41.886213 ansible-butler-1.0.9/setup.cfg
```

### Comparing `ansible-butler-1.0.8/.gitignore` & `ansible-butler-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/LICENSE` & `ansible-butler-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/PKG-INFO` & `ansible-butler-1.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-butler
-Version: 1.0.8
+Version: 1.0.9
 Summary: A butler CLI for assistance in managing Ansible projects
 Home-page: https://github.com/zjleblanc/ansible-butler
 Author: Zach LeBlanc
 Author-email: zjleblanc3@gmail.com
 Project-URL: Bug Tracker, https://github.com/zjleblanc/ansible-butler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -21,25 +21,27 @@
 Functions
 ------------
 
 | Object | Action | Description |
 | ------ | ------ | ----------- |
 | directory | init | initialize an ansible directory |
 | directory | init | cleanup an ansible directory |
+| ee | init | initialize an execution environment directory for ansible-builder |
 | role | list | list roles |
 | role | clean | clean role directory structure (remove empty yml files & dirs) |
 | role | mk-readme | auto generate readme based on role meta and basic yml info |
 
 Usage
 --------------
 
 ```
 Usage:
   ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
+  ansible-butler ee init [<dir>] [--config=PATH]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
@@ -56,14 +58,17 @@
 
 - Initialize Ansible Directory
   - `ansible-butler directory init ./sandbox`
   - `ansible-butler directory init ./sandbox --config=~/configs/ansible-butler.yml`
 - Clean an Ansible Directory
   - `ansible-butler directory clean ./sandbox`
   - `ansible-butler directory clean ./sandbox --skip-roles`
+- Initialize Execution Environment Directory
+  - `ansible-butler ee init ./ee-windows`
+  - `ansible-butler ee init ./ee-windows --config=~/configs/ansible-butler.yml`
 - Clean Roles 
   - `ansible-butler role clean my-role-1`
   - `ansible-butler role clean my-role-*`
 - Generate README
   - `ansible-butler role mk-readme my-role-1`
   - `ansible-butler role mk-readme my-role-*`
 
@@ -77,31 +82,40 @@
 ./                      ## highest precedence
 ```
 
 You can also specify a specific path at runtime via the `--config` option.
 
 ```yaml
 # Configuration Schema
-
-role: {}
+execution_environment:
+  init:
+    version: 2
+    ansible_config: ansible.cfg
+    ee_base_image: quay.io/ansible/ansible-runner:latest
+    ee_builder_image: quay.io/ansible/ansible-builder:latest
+    prepend_build_steps:
+      - ...
+    append_build_steps:
+      - ...
 directory:
   init:
     folders:
       - name: plugins
         folders:
           ...
         files:
           - README.md
     files:
       - playbook.yml
+role: {}
 ```
 
-[🔗](./ansiblebutler/common/.ansible-butler.yml) Default configuration file
+[🔗 Default configuration file](./ansiblebutler/common/.ansible-butler.yml)
 <br>
-[🔗](./docs/config/.ansible-butler.example.yml) Example adding test plugins directory
+[🔗 Example adding test plugins directory](./docs/config/.ansible-butler.test-plugins.yml)
 
 Troubleshooting
 ----------------
 
 - `ansible-butler: command not found`
   - check the $PATH environment variable and ensure that `~/.local/bin` is included
```

### Comparing `ansible-butler-1.0.8/README.md` & `ansible-butler-1.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 Functions
 ------------
 
 | Object | Action | Description |
 | ------ | ------ | ----------- |
 | directory | init | initialize an ansible directory |
 | directory | init | cleanup an ansible directory |
+| ee | init | initialize an execution environment directory for ansible-builder |
 | role | list | list roles |
 | role | clean | clean role directory structure (remove empty yml files & dirs) |
 | role | mk-readme | auto generate readme based on role meta and basic yml info |
 
 Usage
 --------------
 
 ```
 Usage:
   ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
+  ansible-butler ee init [<dir>] [--config=PATH]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
@@ -41,14 +43,17 @@
 
 - Initialize Ansible Directory
   - `ansible-butler directory init ./sandbox`
   - `ansible-butler directory init ./sandbox --config=~/configs/ansible-butler.yml`
 - Clean an Ansible Directory
   - `ansible-butler directory clean ./sandbox`
   - `ansible-butler directory clean ./sandbox --skip-roles`
+- Initialize Execution Environment Directory
+  - `ansible-butler ee init ./ee-windows`
+  - `ansible-butler ee init ./ee-windows --config=~/configs/ansible-butler.yml`
 - Clean Roles 
   - `ansible-butler role clean my-role-1`
   - `ansible-butler role clean my-role-*`
 - Generate README
   - `ansible-butler role mk-readme my-role-1`
   - `ansible-butler role mk-readme my-role-*`
 
@@ -62,31 +67,40 @@
 ./                      ## highest precedence
 ```
 
 You can also specify a specific path at runtime via the `--config` option.
 
 ```yaml
 # Configuration Schema
-
-role: {}
+execution_environment:
+  init:
+    version: 2
+    ansible_config: ansible.cfg
+    ee_base_image: quay.io/ansible/ansible-runner:latest
+    ee_builder_image: quay.io/ansible/ansible-builder:latest
+    prepend_build_steps:
+      - ...
+    append_build_steps:
+      - ...
 directory:
   init:
     folders:
       - name: plugins
         folders:
           ...
         files:
           - README.md
     files:
       - playbook.yml
+role: {}
 ```
 
-[🔗](./ansiblebutler/common/.ansible-butler.yml) Default configuration file
+[🔗 Default configuration file](./ansiblebutler/common/.ansible-butler.yml)
 <br>
-[🔗](./docs/config/.ansible-butler.example.yml) Example adding test plugins directory
+[🔗 Example adding test plugins directory](./docs/config/.ansible-butler.test-plugins.yml)
 
 Troubleshooting
 ----------------
 
 - `ansible-butler: command not found`
   - check the $PATH environment variable and ensure that `~/.local/bin` is included
```

### Comparing `ansible-butler-1.0.8/ansible_butler.egg-info/PKG-INFO` & `ansible-butler-1.0.9/ansible_butler.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-butler
-Version: 1.0.8
+Version: 1.0.9
 Summary: A butler CLI for assistance in managing Ansible projects
 Home-page: https://github.com/zjleblanc/ansible-butler
 Author: Zach LeBlanc
 Author-email: zjleblanc3@gmail.com
 Project-URL: Bug Tracker, https://github.com/zjleblanc/ansible-butler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -21,25 +21,27 @@
 Functions
 ------------
 
 | Object | Action | Description |
 | ------ | ------ | ----------- |
 | directory | init | initialize an ansible directory |
 | directory | init | cleanup an ansible directory |
+| ee | init | initialize an execution environment directory for ansible-builder |
 | role | list | list roles |
 | role | clean | clean role directory structure (remove empty yml files & dirs) |
 | role | mk-readme | auto generate readme based on role meta and basic yml info |
 
 Usage
 --------------
 
 ```
 Usage:
   ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
+  ansible-butler ee init [<dir>] [--config=PATH]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
@@ -56,14 +58,17 @@
 
 - Initialize Ansible Directory
   - `ansible-butler directory init ./sandbox`
   - `ansible-butler directory init ./sandbox --config=~/configs/ansible-butler.yml`
 - Clean an Ansible Directory
   - `ansible-butler directory clean ./sandbox`
   - `ansible-butler directory clean ./sandbox --skip-roles`
+- Initialize Execution Environment Directory
+  - `ansible-butler ee init ./ee-windows`
+  - `ansible-butler ee init ./ee-windows --config=~/configs/ansible-butler.yml`
 - Clean Roles 
   - `ansible-butler role clean my-role-1`
   - `ansible-butler role clean my-role-*`
 - Generate README
   - `ansible-butler role mk-readme my-role-1`
   - `ansible-butler role mk-readme my-role-*`
 
@@ -77,31 +82,40 @@
 ./                      ## highest precedence
 ```
 
 You can also specify a specific path at runtime via the `--config` option.
 
 ```yaml
 # Configuration Schema
-
-role: {}
+execution_environment:
+  init:
+    version: 2
+    ansible_config: ansible.cfg
+    ee_base_image: quay.io/ansible/ansible-runner:latest
+    ee_builder_image: quay.io/ansible/ansible-builder:latest
+    prepend_build_steps:
+      - ...
+    append_build_steps:
+      - ...
 directory:
   init:
     folders:
       - name: plugins
         folders:
           ...
         files:
           - README.md
     files:
       - playbook.yml
+role: {}
 ```
 
-[🔗](./ansiblebutler/common/.ansible-butler.yml) Default configuration file
+[🔗 Default configuration file](./ansiblebutler/common/.ansible-butler.yml)
 <br>
-[🔗](./docs/config/.ansible-butler.example.yml) Example adding test plugins directory
+[🔗 Example adding test plugins directory](./docs/config/.ansible-butler.test-plugins.yml)
 
 Troubleshooting
 ----------------
 
 - `ansible-butler: command not found`
   - check the $PATH environment variable and ensure that `~/.local/bin` is included
```

### Comparing `ansible-butler-1.0.8/ansible_butler.egg-info/SOURCES.txt` & `ansible-butler-1.0.9/ansible_butler.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,13 +17,19 @@
 ansiblebutler/__main__.py
 ansiblebutler/common/.ansible-butler.yml
 ansiblebutler/common/__init__.py
 ansiblebutler/directory/__init__.py
 ansiblebutler/directory/_clean.py
 ansiblebutler/directory/_initialize.py
 ansiblebutler/directory/templates/playbook.yml.j2
+ansiblebutler/execution_environment/__init__.py
+ansiblebutler/execution_environment/_initialize.py
+ansiblebutler/execution_environment/templates/bindep.txt.j2
+ansiblebutler/execution_environment/templates/execution-environment.yml.j2
+ansiblebutler/execution_environment/templates/requirements.txt.j2
+ansiblebutler/execution_environment/templates/requirements.yml.j2
 ansiblebutler/roles/__init__.py
 ansiblebutler/roles/_clean.py
 ansiblebutler/roles/_list.py
 ansiblebutler/roles/_mkreadme.py
 ansiblebutler/roles/templates/README.md.j2
-docs/config/.ansible-butler.example.yml
+docs/config/.ansible-butler.test-plugins.yml
```

### Comparing `ansible-butler-1.0.8/ansiblebutler/__init__.py` & `ansible-butler-1.0.9/ansiblebutler/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Usage:
   ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
+  ansible-butler ee init [<dir>] [--config=PATH]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
@@ -15,22 +16,25 @@
   --config=PATH       Path to config file
   --roles-path=PATH   Path to roles directory [default: ./roles]
   --skip-roles        Flag to skip cleaning roles
 """
 from docopt import docopt
 from ansiblebutler import roles
 from ansiblebutler import directory
+from ansiblebutler import execution_environment
 from ansiblebutler.common import process_config
 
 def main():
   args = docopt(__doc__)
   config = process_config(args.get('--config'))
 
   if args.get('role'):
     roles.do_roles_action(args, config.get('role'))
   elif args.get('directory'):
     directory.do_dir_action(args, config.get('directory'))
+  elif args.get('ee'):
+    execution_environment.do_ee_action(args, config.get('execution_environment'))
   else:
     print(args)
 
 if __name__ == '__main__':
   main()
```

### Comparing `ansible-butler-1.0.8/ansiblebutler/common/__init__.py` & `ansible-butler-1.0.9/ansiblebutler/common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import yaml
 from pathlib import Path
 from jinja2 import Environment, FileSystemLoader, Template
+from mergedeep import merge, Strategy
 
 TEMPLATE_DIR = os.path.dirname(os.path.abspath(__file__)) + '/templates'
 
 CONFIG_FILE_NAME = '.ansible-butler.yml'
 CONFIG_LOCATIONS = [
   ## order matters
   '/etc/ansible-butler', ## least precedence
@@ -22,18 +23,18 @@
 
 def process_config(custom):
   defaults = os.path.join(os.path.dirname(__file__), CONFIG_FILE_NAME)
   config = load_yml(defaults)
 
   for loc in CONFIG_LOCATIONS:
     path = loc + '/' + CONFIG_FILE_NAME
-    config.update(load_yml(path))
+    merge(config, load_yml(path), strategy=Strategy.TYPESAFE_REPLACE)
 
   if custom:
-    config.update(load_yml(custom))
+    merge(config, load_yml(custom), strategy=Strategy.TYPESAFE_REPLACE)
 
   return config
 
 def parse_yml(yml: str):
   yml_dict = None
   with open(yml, 'r') as stream:
     try:
```

### Comparing `ansible-butler-1.0.8/ansiblebutler/directory/_clean.py` & `ansible-butler-1.0.9/ansiblebutler/directory/_clean.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/ansiblebutler/directory/_initialize.py` & `ansible-butler-1.0.9/ansiblebutler/directory/_initialize.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/ansiblebutler/roles/__init__.py` & `ansible-butler-1.0.9/ansiblebutler/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/ansiblebutler/roles/_mkreadme.py` & `ansible-butler-1.0.9/ansiblebutler/roles/_mkreadme.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/ansiblebutler/roles/templates/README.md.j2` & `ansible-butler-1.0.9/ansiblebutler/roles/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.8/setup.cfg` & `ansible-butler-1.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-butler
-version = 1.0.8
+version = 1.0.9
 author = Zach LeBlanc
 author_email = zjleblanc3@gmail.com
 description = A butler CLI for assistance in managing Ansible projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zjleblanc/ansible-butler
 project_urls = 
@@ -19,14 +19,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
 	docopt>=0.6.2
 	PyYAML>=5.4.1
 	Jinja2>=3.0.0
+	mergedeep>=1.3.4
 
 [options.entry_points]
 console_scripts = 
 	ansible-butler = ansiblebutler:main
 
 [egg_info]
 tag_build =
```

