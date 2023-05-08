# Comparing `tmp/odoo_manager-0.0.8.tar.gz` & `tmp/odoo_manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo_manager-0.0.8.tar", last modified: Tue May 28 17:02:54 2019, max compression
+gzip compressed data, was "dist/odoo_manager-0.0.9.tar", last modified: Tue Jun 18 14:38:58 2019, max compression
```

## Comparing `odoo_manager-0.0.8.tar` & `odoo_manager-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/
--rw-r--r--   0 travis     (501) staff       (20)      430 2019-05-14 15:18:23.000000 odoo_manager-0.0.8/MANIFEST.in
--rw-r--r--   0 travis     (501) staff       (20)     1261 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/PKG-INFO
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/odoo_manager/
--rw-r--r--   0 travis     (501) staff       (20)       81 2019-05-28 17:01:34.000000 odoo_manager-0.0.8/odoo_manager/__init__.py
--rw-r--r--   0 travis     (501) staff       (20)       33 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/__main__.py
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/odoo_manager/cli/
--rw-r--r--   0 travis     (501) staff       (20)       41 2019-05-14 15:18:23.000000 odoo_manager-0.0.8/odoo_manager/cli/__init__.py
--rw-r--r--   0 travis     (501) staff       (20)     4418 2019-05-28 17:01:34.000000 odoo_manager-0.0.8/odoo_manager/cli/cli.py
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/
--rw-r--r--   0 travis     (501) staff       (20)      120 2019-05-21 12:55:31.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/__init__.py
--rw-r--r--   0 travis     (501) staff       (20)     1632 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/base.py
--rw-r--r--   0 travis     (501) staff       (20)    12546 2019-05-28 17:01:34.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/convert.py
--rw-r--r--   0 travis     (501) staff       (20)     5546 2019-05-28 17:01:34.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/format.py
--rw-r--r--   0 travis     (501) staff       (20)      240 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/hello.py
--rw-r--r--   0 travis     (501) staff       (20)     7216 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/new.py
--rw-r--r--   0 travis     (501) staff       (20)     3189 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/cli/commands/setup.py
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/odoo_manager/cli/exceptions/
--rw-r--r--   0 travis     (501) staff       (20)       81 2019-05-14 15:18:23.000000 odoo_manager-0.0.8/odoo_manager/cli/exceptions/__init__.py
--rw-r--r--   0 travis     (501) staff       (20)       44 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/cli/exceptions/command_exception.py
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/odoo_manager/core/
--rw-r--r--   0 travis     (501) staff       (20)       99 2019-05-14 15:18:23.000000 odoo_manager-0.0.8/odoo_manager/core/__init__.py
--rw-r--r--   0 travis     (501) staff       (20)     3770 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/core/configs.py
--rw-r--r--   0 travis     (501) staff       (20)     6354 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/core/git.py
--rw-r--r--   0 travis     (501) staff       (20)      219 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/core/misc.py
--rw-r--r--   0 travis     (501) staff       (20)     1756 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/odoo_manager/core/paths.py
--rw-r--r--   0 travis     (501) staff       (20)     2561 2019-05-21 12:55:31.000000 odoo_manager-0.0.8/odoo_manager/core/shell.py
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/odoo_manager.egg-info/
--rw-r--r--   0 travis     (501) staff       (20)      679 2019-05-28 17:02:53.000000 odoo_manager-0.0.8/odoo_manager.egg-info/SOURCES.txt
--rw-r--r--   0 travis     (501) staff       (20)      535 2019-05-28 17:01:34.000000 odoo_manager-0.0.8/readme.md
--rw-r--r--   0 travis     (501) staff       (20)       67 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/setup.cfg
--rw-r--r--   0 travis     (501) staff       (20)     1316 2019-05-14 19:13:55.000000 odoo_manager-0.0.8/setup.py
-drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-05-28 17:02:54.000000 odoo_manager-0.0.8/tests/
--rw-r--r--   0 travis     (501) staff       (20)        0 2019-05-14 15:18:23.000000 odoo_manager-0.0.8/tests/.gitignore
--rw-r--r--   0 travis     (501) staff       (20)      641 2019-05-14 15:34:18.000000 odoo_manager-0.0.8/tests/test_cli.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/
+-rw-r--r--   0 travis     (501) staff       (20)      430 2019-05-14 15:18:23.000000 odoo_manager-0.0.9/MANIFEST.in
+-rw-r--r--   0 travis     (501) staff       (20)     1261 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/PKG-INFO
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager/
+-rw-r--r--   0 travis     (501) staff       (20)       81 2019-06-18 14:37:11.000000 odoo_manager-0.0.9/odoo_manager/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)       33 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/__main__.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager/cli/
+-rw-r--r--   0 travis     (501) staff       (20)       41 2019-05-14 15:18:23.000000 odoo_manager-0.0.9/odoo_manager/cli/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)     4418 2019-05-31 12:23:14.000000 odoo_manager-0.0.9/odoo_manager/cli/cli.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/
+-rw-r--r--   0 travis     (501) staff       (20)      120 2019-05-21 12:55:31.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)     1632 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/base.py
+-rw-r--r--   0 travis     (501) staff       (20)    12546 2019-05-31 12:23:14.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/convert.py
+-rw-r--r--   0 travis     (501) staff       (20)     5546 2019-05-31 12:23:14.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/format.py
+-rw-r--r--   0 travis     (501) staff       (20)      240 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/hello.py
+-rw-r--r--   0 travis     (501) staff       (20)     7152 2019-06-18 14:38:13.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/new.py
+-rw-r--r--   0 travis     (501) staff       (20)     3189 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/cli/commands/setup.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager/cli/exceptions/
+-rw-r--r--   0 travis     (501) staff       (20)       81 2019-05-14 15:18:23.000000 odoo_manager-0.0.9/odoo_manager/cli/exceptions/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)       44 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/cli/exceptions/command_exception.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager/core/
+-rw-r--r--   0 travis     (501) staff       (20)       99 2019-05-14 15:18:23.000000 odoo_manager-0.0.9/odoo_manager/core/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)     3770 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/core/configs.py
+-rw-r--r--   0 travis     (501) staff       (20)     6344 2019-06-18 14:37:11.000000 odoo_manager-0.0.9/odoo_manager/core/git.py
+-rw-r--r--   0 travis     (501) staff       (20)      219 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/core/misc.py
+-rw-r--r--   0 travis     (501) staff       (20)     1756 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/odoo_manager/core/paths.py
+-rw-r--r--   0 travis     (501) staff       (20)     2561 2019-05-21 12:55:31.000000 odoo_manager-0.0.9/odoo_manager/core/shell.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager.egg-info/
+-rw-r--r--   0 travis     (501) staff       (20)      679 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/odoo_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 travis     (501) staff       (20)      535 2019-05-31 12:23:14.000000 odoo_manager-0.0.9/readme.md
+-rw-r--r--   0 travis     (501) staff       (20)       67 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/setup.cfg
+-rw-r--r--   0 travis     (501) staff       (20)     1316 2019-05-14 19:13:55.000000 odoo_manager-0.0.9/setup.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2019-06-18 14:38:58.000000 odoo_manager-0.0.9/tests/
+-rw-r--r--   0 travis     (501) staff       (20)        0 2019-05-14 15:18:23.000000 odoo_manager-0.0.9/tests/.gitignore
+-rw-r--r--   0 travis     (501) staff       (20)      641 2019-05-14 15:34:18.000000 odoo_manager-0.0.9/tests/test_cli.py
```

### Comparing `odoo_manager-0.0.8/PKG-INFO` & `odoo_manager-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Odoo manager utility
 Home-page: UNKNOWN
 Author: Blue Stingray
 Author-email: odoo@bluestingray.com
 License: UNKNOWN
 Description: # odoo-manager
```

### Comparing `odoo_manager-0.0.8/odoo_manager/cli/cli.py` & `odoo_manager-0.0.9/odoo_manager/cli/cli.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/cli/commands/base.py` & `odoo_manager-0.0.9/odoo_manager/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/cli/commands/convert.py` & `odoo_manager-0.0.9/odoo_manager/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/cli/commands/format.py` & `odoo_manager-0.0.9/odoo_manager/cli/commands/format.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/cli/commands/new.py` & `odoo_manager-0.0.9/odoo_manager/cli/commands/new.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 
         if not name:
             shell.out('Missing project name. Try "odoo-manager new project --name=my_project"')
             return
 
         try:
             shell.run(
-                'git clone git@bitbucket.org:bluestingray/collections_scaffold {} --branch="{}" "{}"'.format(
+                'git clone git@github.com:gobluestingray/odoo_project_scaffold.git {} --branch="{}" "{}"'.format(
                     "--quiet" if not verbose else "", branch, name
                 )
             )
         except:
-            username = quote(input("bitbucket username? "))
-            password = quote(getpass.getpass("bitbucket password? "))
+            username = quote(input("Username? "))
+            password = quote(getpass.getpass("Password? "))
 
             try:
                 shell.run(
-                    'git clone https://{}:{}@bitbucket.org/bluestingray/collections_scaffold --quiet --branch="{}" "{}"'.format(
+                    'git clone https://{}:{}@github.com/gobluestingray/odoo_project_scaffold.git --quiet --branch="{}" "{}"'.format(
                         username, password, branch, name
                     )
                 )
             except:
                 shell.out("Invalid credentials.", color=shell.COLOR_RED)
 
         shell.run('rm -rf "./{}/.git"'.format(name))
@@ -77,25 +77,25 @@
         )
 
         shell.out("\n")
         shell.out("Generating the module...")
 
         try:
             shell.run(
-                'git clone git@bitbucket.org:bluestingray/module_scaffold {} --branch="{}" "{}"'.format(
+                'git clone git@github.com:gobluestingray/odoo_module_scaffold.git {} --branch="{}" "{}"'.format(
                     "--quiet" if not verbose else "", branch, name
                 )
             )
         except:
-            username = quote(input("bitbucket username? "))
-            password = quote(getpass.getpass("bitbucket password? "))
+            username = quote(input("Username? "))
+            password = quote(getpass.getpass("Password? "))
 
             try:
                 shell.run(
-                    'git clone https://{}:{}@bitbucket.org/bluestingray/module_scaffold --quiet --branch="{}" "{}"'.format(
+                    'git clone https://{}:{}@github.com/gobluestingray/odoo_module_scaffold.git --quiet --branch="{}" "{}"'.format(
                         username, password, branch, name
                     )
                 )
             except:
                 shell.out("Invalid credentials.", color=shell.COLOR_RED)
 
         shell.run('rm -rf "./{}/.git"'.format(name))
@@ -115,17 +115,15 @@
 <section class="oe_container">
     <div class="oe_row oe_spaced">
         <div class="oe_span12">
             <h2 class="oe_slogan">{}</h2>
             <h3 class="oe_slogan">{}</h3>
         </div>
     </div>
-</section>""".strip(
-                    "\n"
-                ).format(
+</section>\n""".format(
                     module_display_name, module_tagline
                 )
             )
         with open("./{}/doc/index.rst".format(name), "w") as index_rst_file:
             content = "{} documentation.".format(name)
             index_rst_file.write("{}\n{}".format(content, "=" * len(content)))
```

### Comparing `odoo_manager-0.0.8/odoo_manager/cli/commands/setup.py` & `odoo_manager-0.0.9/odoo_manager/cli/commands/setup.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/core/configs.py` & `odoo_manager-0.0.9/odoo_manager/core/configs.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/core/git.py` & `odoo_manager-0.0.9/odoo_manager/core/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
             url=url, branch=branch, output=output, depth=depth, pipe=redirect()
         )
     )
 
 
 def _get_git_config():
     git_config = {}
-    # right now, just assuming bitbucket.org repo's
+    # Right now, just assuming github.com repos
     if not configs.config.has_option("options", "USERNAME") or not configs.config.has_option("options", "PASSWORD"):
-        git_config["username"] = quote(input("bitbucket username? "))
-        git_config["password"] = quote(getpass.getpass("bitbucket password? "))
+        git_config["username"] = quote(input("Github username? "))
+        git_config["password"] = quote(getpass.getpass("Github password? "))
     else:
         git_config["username"] = configs.config.get("options", "USERNAME")
         git_config["password"] = configs.config.get("options", "PASSWORD")
     return git_config
 
 
 def _get_git_urls(repo_url):
```

### Comparing `odoo_manager-0.0.8/odoo_manager/core/paths.py` & `odoo_manager-0.0.9/odoo_manager/core/paths.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager/core/shell.py` & `odoo_manager-0.0.9/odoo_manager/core/shell.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/odoo_manager.egg-info/SOURCES.txt` & `odoo_manager-0.0.9/odoo_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/readme.md` & `odoo_manager-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/setup.py` & `odoo_manager-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `odoo_manager-0.0.8/tests/test_cli.py` & `odoo_manager-0.0.9/tests/test_cli.py`

 * *Files identical despite different names*

