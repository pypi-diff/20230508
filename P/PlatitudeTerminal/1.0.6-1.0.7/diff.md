# Comparing `tmp/PlatitudeTerminal-1.0.6.tar.gz` & `tmp/PlatitudeTerminal-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PlatitudeTerminal-1.0.6.tar", last modified: Sun May  7 22:40:44 2023, max compression
+gzip compressed data, was "dist/PlatitudeTerminal-1.0.7.tar", last modified: Mon May  8 21:17:30 2023, max compression
```

## Comparing `PlatitudeTerminal-1.0.6.tar` & `PlatitudeTerminal-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/
--rw-r--r--   0 louis      (501) staff       (20)      224 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PKG-INFO
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PlatitudeTerminal.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)      224 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PlatitudeTerminal.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      417 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PlatitudeTerminal.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)       44 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PlatitudeTerminal.egg-info/entry_points.txt
--rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PlatitudeTerminal.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/PlatitudeTerminal.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.6/pyproject.toml
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/peregrine/
--rw-r--r--   0 louis      (501) staff       (20)     2738 2023-05-07 20:21:08.000000 PlatitudeTerminal-1.0.6/peregrine/client.py
--rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.6/peregrine/colorutils.py
--rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.6/peregrine/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     2990 2023-05-03 05:17:22.000000 PlatitudeTerminal-1.0.6/peregrine/stateutils.py
--rw-r--r--   0 louis      (501) staff       (20)    30330 2023-05-07 21:02:37.000000 PlatitudeTerminal-1.0.6/peregrine/cli.py
--rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-07 18:08:06.000000 PlatitudeTerminal-1.0.6/peregrine/install.py
--rw-r--r--   0 louis      (501) staff       (20)      275 2023-05-07 20:27:54.000000 PlatitudeTerminal-1.0.6/peregrine/errors.py
--rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.6/peregrine/main.py
--rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.6/README.md
--rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.6/setup.py
--rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-07 22:40:44.000000 PlatitudeTerminal-1.0.6/setup.cfg
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/
+-rw-r--r--   0 louis      (501) staff       (20)      224 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PKG-INFO
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)      224 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      417 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)       44 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/entry_points.txt
+-rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.7/pyproject.toml
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/peregrine/
+-rw-r--r--   0 louis      (501) staff       (20)     2738 2023-05-07 20:21:08.000000 PlatitudeTerminal-1.0.7/peregrine/client.py
+-rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.7/peregrine/colorutils.py
+-rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.7/peregrine/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     2990 2023-05-03 05:17:22.000000 PlatitudeTerminal-1.0.7/peregrine/stateutils.py
+-rw-r--r--   0 louis      (501) staff       (20)    30407 2023-05-08 21:12:51.000000 PlatitudeTerminal-1.0.7/peregrine/cli.py
+-rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-08 21:17:02.000000 PlatitudeTerminal-1.0.7/peregrine/install.py
+-rw-r--r--   0 louis      (501) staff       (20)      275 2023-05-07 20:27:54.000000 PlatitudeTerminal-1.0.7/peregrine/errors.py
+-rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.7/peregrine/main.py
+-rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.7/README.md
+-rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.7/setup.py
+-rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/setup.cfg
```

### Comparing `PlatitudeTerminal-1.0.6/pyproject.toml` & `PlatitudeTerminal-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.6/peregrine/client.py` & `PlatitudeTerminal-1.0.7/peregrine/client.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.6/peregrine/colorutils.py` & `PlatitudeTerminal-1.0.7/peregrine/colorutils.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.6/peregrine/stateutils.py` & `PlatitudeTerminal-1.0.7/peregrine/stateutils.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.6/peregrine/cli.py` & `PlatitudeTerminal-1.0.7/peregrine/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,15 @@
             p = fetchPricing(uid=uid, idT=idToken)
             
 
             typer.echo(
                 f'''
                                     {colorutils.colors.BOLD}      Select your plan  {colorutils.colors.ENDC}
                 ===================================================================
+                        All Platitude.ai Plans come with a 7 day free trial!
 
           {colorutils.colors.BOLD}             Starter               Enthusiast              Professional {colorutils.colors.ENDC}
                 ====================    ====================    ====================   
                 |                  |    |                  |    |                  |                                        
                 |    ${p['1']['price']} / month    |    |    ${p['2']['price']} / month    |    |    ${p['3']['price']} / month    |
                 |    ~{int(p['1']['tokens']/100)} queries   |    |   ~{int(p['2']['tokens']/100)} queries   |    |   ~{int(p['3']['tokens']/100)} queries   |
                 |                  |    |                  |    |                  |
```

### Comparing `PlatitudeTerminal-1.0.6/README.md` & `PlatitudeTerminal-1.0.7/README.md`

 * *Files identical despite different names*

