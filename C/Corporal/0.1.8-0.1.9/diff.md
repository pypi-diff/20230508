# Comparing `tmp/Corporal-0.1.8.tar.gz` & `tmp/Corporal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/corporal/dist/.tmp-5k3188kt/Corporal-0.1.8.tar", last modified: Mon Jan  2 23:01:24 2023, max compression
+gzip compressed data, was "/home/lance/src/corporal/dist/.tmp-58_5qqtr/Corporal-0.1.9.tar", last modified: Thu Jan 19 01:33:48 2023, max compression
```

## Comparing `Corporal-0.1.8.tar` & `Corporal-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/
--rw-r--r--   0 lance     (1000) lance     (1000)     1464 2023-01-02 23:00:50.000000 Corporal-0.1.8/CHANGELOG.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)      748 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      770 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      276 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      157 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        9 2023-01-02 23:01:24.000000 Corporal-0.1.8/Corporal.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      187 2020-12-03 04:15:58.000000 Corporal-0.1.8/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)      748 2023-01-02 23:01:24.000000 Corporal-0.1.8/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      152 2020-12-03 04:18:01.000000 Corporal-0.1.8/README.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/
--rw-r--r--   0 lance     (1000) lance     (1000)       65 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-01-02 23:00:54.000000 Corporal-0.1.8/corporal/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-14 18:50:52.000000 Corporal-0.1.8/corporal/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9875 2022-03-10 00:30:05.000000 Corporal-0.1.8/corporal/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)      691 2020-12-03 21:01:57.000000 Corporal-0.1.8/corporal/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)      862 2022-08-08 00:04:03.000000 Corporal-0.1.8/corporal/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/db/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-14 18:04:09.000000 Corporal-0.1.8/corporal/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      234 2021-02-14 18:03:37.000000 Corporal-0.1.8/corporal/db/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)      427 2021-07-22 16:44:53.000000 Corporal-0.1.8/corporal/emails.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/fablib/
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/fablib/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7937 2023-01-02 22:48:02.000000 Corporal-0.1.8/corporal/fablib/corporal.py
--rw-r--r--   0 lance     (1000) lance     (1000)      688 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/fablib/python.py
--rw-r--r--   0 lance     (1000) lance     (1000)      547 2022-08-09 23:13:11.000000 Corporal-0.1.8/corporal/settings.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/web/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/web/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      984 2023-01-02 22:40:58.000000 Corporal-0.1.8/corporal/web/app.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3253 2022-03-09 18:47:09.000000 Corporal-0.1.8/corporal/web/menus.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/web/static/
--rw-r--r--   0 lance     (1000) lance     (1000)      192 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/web/static/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      337 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/web/subscribers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/web/templates/
--rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-06-15 20:53:54.000000 Corporal-0.1.8/corporal/web/templates/base_meta.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 23:01:24.000000 Corporal-0.1.8/corporal/web/views/
--rw-r--r--   0 lance     (1000) lance     (1000)      932 2022-03-10 00:09:01.000000 Corporal-0.1.8/corporal/web/views/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)      284 2020-12-03 04:15:58.000000 Corporal-0.1.8/corporal/web/views/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-01-02 23:01:24.000000 Corporal-0.1.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     3864 2022-08-08 00:04:28.000000 Corporal-0.1.8/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1717 2023-01-19 01:33:18.000000 Corporal-0.1.9/CHANGELOG.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)      748 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      802 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      275 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      152 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        9 2023-01-19 01:33:48.000000 Corporal-0.1.9/Corporal.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      233 2023-01-09 02:29:22.000000 Corporal-0.1.9/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      748 2023-01-19 01:33:48.000000 Corporal-0.1.9/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      152 2020-12-03 04:18:01.000000 Corporal-0.1.9/README.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/
+-rw-r--r--   0 lance     (1000) lance     (1000)       65 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-01-19 01:33:21.000000 Corporal-0.1.9/corporal/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-14 18:50:52.000000 Corporal-0.1.9/corporal/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9875 2022-03-10 00:30:05.000000 Corporal-0.1.9/corporal/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      855 2023-01-18 20:20:31.000000 Corporal-0.1.9/corporal/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      841 2023-01-18 20:21:20.000000 Corporal-0.1.9/corporal/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/data/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/data/config/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3411 2020-12-04 20:37:48.000000 Corporal-0.1.9/corporal/data/config/corporal-rattail.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)     1721 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/data/config/corporal-web.conf
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-14 18:04:09.000000 Corporal-0.1.9/corporal/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      234 2021-02-14 18:03:37.000000 Corporal-0.1.9/corporal/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      427 2021-07-22 16:44:53.000000 Corporal-0.1.9/corporal/emails.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/fablib/
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/fablib/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8503 2023-01-02 23:02:34.000000 Corporal-0.1.9/corporal/fablib/corporal.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      688 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/fablib/python.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/web/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/web/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      984 2023-01-02 22:40:58.000000 Corporal-0.1.9/corporal/web/app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1126 2023-01-18 03:15:27.000000 Corporal-0.1.9/corporal/web/menus.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/web/static/
+-rw-r--r--   0 lance     (1000) lance     (1000)      192 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/web/static/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      337 2020-12-03 04:15:58.000000 Corporal-0.1.9/corporal/web/subscribers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/web/templates/
+-rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-06-15 20:53:54.000000 Corporal-0.1.9/corporal/web/templates/base_meta.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-19 01:33:48.000000 Corporal-0.1.9/corporal/web/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)      400 2023-01-18 19:53:55.000000 Corporal-0.1.9/corporal/web/views/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-01-19 01:33:48.000000 Corporal-0.1.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     3863 2023-01-18 20:20:36.000000 Corporal-0.1.9/setup.py
```

### Comparing `Corporal-0.1.8/CHANGELOG.md` & `Corporal-0.1.9/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 
 # Changelog
 All notable changes to Corporal will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.9] - 2023-01-18
+### Changed
+- Use handler to build menus.
+- Include sample config files in manifest.
+- Tweak view config per upstream changes.
+- Remove reference to `rattail[auth]` extra.
+- Add support for new-style `corporal install` command.
+
 ## [0.1.8] - 2023-01-02
 ### Changed
 - Register entry points for emails.
 - Expose app setting for default grid pagesize.
 - Add ASGI app wrapper.
 
 ## [0.1.7] - 2022-03-10
```

### Comparing `Corporal-0.1.8/Corporal.egg-info/PKG-INFO` & `Corporal-0.1.9/Corporal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Corporal
-Version: 0.1.8
+Version: 0.1.9
 Summary: Companion Back-end for CORE-POS
 Home-page: https://rattailproject.org
 Author: Lance Edgar
 Author-email: lance@edbob.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `Corporal-0.1.8/Corporal.egg-info/SOURCES.txt` & `Corporal-0.1.9/Corporal.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 Corporal.egg-info/requires.txt
 Corporal.egg-info/top_level.txt
 corporal/__init__.py
 corporal/_version.py
 corporal/commands.py
 corporal/config.py
 corporal/emails.py
-corporal/settings.py
 corporal/batch/__init__.py
 corporal/batch/vendorcatalog.py
+corporal/data/config/corporal-rattail.conf
+corporal/data/config/corporal-web.conf
 corporal/db/__init__.py
 corporal/db/model.py
 corporal/fablib/__init__.py
 corporal/fablib/corporal.py
 corporal/fablib/python.py
 corporal/web/__init__.py
 corporal/web/app.py
 corporal/web/menus.py
 corporal/web/subscribers.py
 corporal/web/static/__init__.py
 corporal/web/templates/base_meta.mako
-corporal/web/views/__init__.py
-corporal/web/views/common.py
+corporal/web/views/__init__.py
```

### Comparing `Corporal-0.1.8/PKG-INFO` & `Corporal-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Corporal
-Version: 0.1.8
+Version: 0.1.9
 Summary: Companion Back-end for CORE-POS
 Home-page: https://rattailproject.org
 Author: Lance Edgar
 Author-email: lance@edbob.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `Corporal-0.1.8/corporal/batch/vendorcatalog.py` & `Corporal-0.1.9/corporal/batch/vendorcatalog.py`

 * *Files identical despite different names*

### Comparing `Corporal-0.1.8/corporal/commands.py` & `Corporal-0.1.9/corporal/commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,16 +24,20 @@
     """
     name = 'corporal'
     version = __version__
     description = "Corporal (custom Rattail system)"
     long_description = ''
 
 
-class HelloWorld(commands.Subcommand):
+class Install(commands.InstallSubcommand):
     """
-    The requisite 'hello world' example
+    Install the Corporal app
     """
-    name = 'hello'
+    name = 'install'
     description = __doc__.strip()
 
-    def run(self, args):
-        self.stdout.write("hello world!\n")
+    # nb. these must be explicitly set b/c config is not available
+    # when running normally, e.g. `corporal -n install`
+    app_title = "Corporal"
+    app_package = 'corporal'
+    app_eggname = 'Corporal'
+    app_pypiname = 'Corporal'
```

### Comparing `Corporal-0.1.8/corporal/config.py` & `Corporal-0.1.9/corporal/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8; -*-
 """
 Custom config
 """
 
 from rattail.config import ConfigExtension
 
 
@@ -14,13 +15,12 @@
     def configure(self, config):
 
         if config.getbool('rattail.config', 'corporal.set_defaults',
                           usedb=False, default=True):
 
             # set some default config values
             config.setdefault('rattail', 'model', 'corporal.db.model')
-            config.setdefault('rattail', 'settings', 'corporal.settings')
-            config.setdefault('tailbone', 'menus', 'corporal.web.menus')
+            config.setdefault('tailbone.menus', 'handler', 'corporal.web.menus:CorporalMenuHandler')
             config.setdefault('rattail.config', 'templates', 'corporal:data/config rattail:data/config')
 
             # batches
             config.setdefault('rattail.batch', 'vendor_catalog.handler', 'corporal.batch.vendorcatalog:VendorCatalogHandler')
```

### Comparing `Corporal-0.1.8/corporal/fablib/corporal.py` & `Corporal-0.1.9/corporal/fablib/corporal.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from rattail_fabric2 import apache, postgresql, python, exists, mkdir
 
 from corporal.fablib import deploy_common
 
 
 def bootstrap_corporal_app(c, env, envname='corporal', user='rattail',
-                           port=7900, sitename=None, stage=False,
+                           port=7900, asgi=False, sitename=None, stage=False,
                            coredir=None, lanes=None,
                            core_office_url=None):
     """
     Create a virtual environment for use with a Corporal app.
     """
     safename = envname.replace('-', '_')
     dbname = envname
@@ -31,14 +31,20 @@
 
     # virtualenv
     if not exists(c, envdir):
         python.mkvirtualenv(c, envname, python='/usr/bin/python3', runas_user=user)
     c.sudo('chmod 0600 {}/pip.conf'.format(envdir))
     mkdir(c, srcdir, owner=user, use_sudo=True)
 
+    # uvicorn
+    if asgi:
+        # (latest as of writing is 0.20.0)
+        c.sudo("bash -lc 'workon {} && pip install uvicorn[standard]'".format(envname),
+               user=user)
+
     if stage:
 
         # pycorepos
         if not exists(c, '{}/pycorepos'.format(srcdir)):
             c.sudo('git clone https://kallithea.rattailproject.org/rattail-project/pycorepos {}/pycorepos'.format(srcdir),
                    user=user)
             c.sudo("bash -lc 'workon {} && pip install -e {}/pycorepos'".format(envname, srcdir),
@@ -112,14 +118,18 @@
                user=user)
     deploy_common(c, 'corporal/cron.conf.mako', '{}/cron.conf'.format(appdir),
                   use_sudo=True, owner=user, context={'envdir': envdir})
     deploy_common(c, 'corporal/web.conf.mako', '{}/web.conf'.format(appdir),
                   use_sudo=True, owner=user, mode='0600', 
                   context={'env': env, 'envname': envname, 'envdir': envdir,
                            'port': port})
+    if asgi:
+        deploy_common(c, 'corporal/webasgi.conf.mako', '{}/webasgi.conf'.format(appdir),
+                      use_sudo=True, owner=user, mode='0600',
+                      context={'env': env, 'envname': envname, 'envdir': envdir})
     deploy_common(c, 'corporal/upgrade.sh.mako', '{}/upgrade.sh'.format(appdir),
                   use_sudo=True, owner=user, 
                   context={'envdir': envdir, 'production': production})
     # if host:
     deploy_common(c, 'corporal/tasks.py.mako', '{}/tasks.py'.format(appdir),
                   use_sudo=True, owner=user,
                   context={'envdir': envdir, 'stage': stage})
@@ -135,28 +145,30 @@
         postgresql.sql(c, "insert into setting values ('tailbone.theme', 'falafel')",
                        database=dbname)
         postgresql.sql(c, "insert into setting values ('tailbone.themes.expose_picker', 'false')",
                        database=dbname)
 
     # supervisor
     deploy_common(c, 'corporal/supervisor.conf.mako', '/etc/supervisor/conf.d/{}.conf'.format(safename),
-                  use_sudo=True, context={'envdir': envdir, 'safename': safename})
+                  use_sudo=True, context={'envdir': envdir, 'safename': safename,
+                                          'port': port, 'asgi': asgi})
     c.sudo('supervisorctl update')
     c.sudo('supervisorctl start {}:'.format(safename))
 
     # cron etc.
     deploy_common.sudoers(c, 'corporal/sudoers.mako', '/etc/sudoers.d/{}'.format(safename),
                           context={'envdir': envdir, 'safename': safename})
     deploy_common(c, 'corporal/logrotate.conf.mako', '/etc/logrotate.d/{}'.format(safename),
                   use_sudo=True, context={'envdir': envdir})
 
     # apache
     deploy_common.apache_site(c, 'apache/site-corporal.mako', sitename,
                               enable=True,
-                              context={'sitename': sitename, 'port': port})
+                              context={'sitename': sitename, 'port': port,
+                                       'asgi': asgi})
     apache.restart(c)
 
 
 def parse_fannie_lanes(c, script, coredir):
     """
     Parse and return the CORE lane definitions from Fannie config file.
     """
```

### Comparing `Corporal-0.1.8/corporal/fablib/python.py` & `Corporal-0.1.9/corporal/fablib/python.py`

 * *Files identical despite different names*

### Comparing `Corporal-0.1.8/corporal/web/app.py` & `Corporal-0.1.9/corporal/web/app.py`

 * *Files identical despite different names*

### Comparing `Corporal-0.1.8/setup.py` & `Corporal-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     # at first i didn't set this here, but for some reason an install
     # got SA 1.4.x so then i had to.
     'SQLAlchemy<1.4',                   # 0.7.6                 1.3.24
 
     'invoke',                           # 1.4.1
     'psycopg2',                         # 2.8.4
 
-    'rattail[auth,db,bouncer]',         # 0.9.141
+    'rattail[db,bouncer]',              # 0.9.141
     'rattail-fabric2',                  # 0.2.1
     'Tailbone',                         # 0.8.72
     'pyCOREPOS',                        # 0.1.1
     'rattail-corepos',                  # 0.1.3
     'tailbone-corepos',                 # 0.1.3
 ]
 
@@ -95,15 +95,15 @@
     entry_points = {
 
         'console_scripts': [
             'corporal = corporal.commands:main',
         ],
 
         'corporal.commands': [
-            'hello = corporal.commands:HelloWorld',
+            'install = corporal.commands:Install',
         ],
 
         'paste.app_factory': [
             'main = corporal.web.app:main',
         ],
 
         'rattail.config.extensions': [
```

