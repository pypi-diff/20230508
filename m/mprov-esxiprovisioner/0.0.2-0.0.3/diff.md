# Comparing `tmp/mprov_esxiprovisioner-0.0.2.tar.gz` & `tmp/mprov_esxiprovisioner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mprov_esxiprovisioner-0.0.2.tar", last modified: Thu Dec 22 20:47:24 2022, max compression
+gzip compressed data, was "mprov_esxiprovisioner-0.0.3.tar", last modified: Mon May  8 13:15:47 2023, max compression
```

## Comparing `mprov_esxiprovisioner-0.0.2.tar` & `mprov_esxiprovisioner-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:47:24.638078 mprov_esxiprovisioner-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      672 2022-12-22 20:47:24.638078 mprov_esxiprovisioner-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-22 20:47:18.000000 mprov_esxiprovisioner-0.0.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-22 20:47:24.638078 mprov_esxiprovisioner-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:47:24.634078 mprov_esxiprovisioner-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:47:24.638078 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:47:24.634078 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:47:24.638078 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/templates/systems/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/templates/systems/ipxe
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2022-12-22 20:47:07.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:47:24.638078 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2022-12-22 20:47:24.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2022-12-22 20:47:24.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:47:24.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2022-12-22 20:47:24.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-22 20:47:24.000000 mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:47.608427 mprov_esxiprovisioner-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-08 13:15:47.608427 mprov_esxiprovisioner-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 13:15:40.000000 mprov_esxiprovisioner-0.0.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 13:15:47.608427 mprov_esxiprovisioner-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:47.604427 mprov_esxiprovisioner-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:47.604427 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:47.604427 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:47.608427 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/templates/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/templates/systems/ipxe
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-08 13:15:20.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:47.608427 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-08 13:15:47.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 13:15:47.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:15:47.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 13:15:47.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:15:47.000000 mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/top_level.txt
```

### Comparing `mprov_esxiprovisioner-0.0.2/setup.cfg` & `mprov_esxiprovisioner-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/admin.py` & `mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/admin.py`

 * *Files identical despite different names*

### Comparing `mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/models.py` & `mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/models.py`

 * *Files identical despite different names*

### Comparing `mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner/views.py` & `mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,19 @@
 
         # and then see if we can grab any related associations to vcenter hosts.
         if system.vchassociation_set.all().count() > 0:
             # we found something
             context = {
                 'vchassc':  system.vchassociation_set.all()[0] ,
                 'bootserver': platform.node()
-            }            
+            }
+            if request.get_full_path().startswith("/tramp"):
+                print(f"Serving VMWare Tramp to {ip}")
+                return(HttpResponse(f"#!ipxe\nchain http://{ context['bootserver'] }/media/{ context['vchassc'].vcenterHost.name }/tramp", content_type="text/plain"))
+                        
             print(f"Serving ESXi PXE to {ip}")
             return(TemplateResponse(request, "systems/ipxe", context=context, content_type="text/plain" ))
             
         # if we get here, then there doesn't seem to be any VCH Associations, let the normal ipxe code take over. 
         return(None)
         
         # return(render(template_name="ipxe", request=request, context=context, content_type="text/plain" ))
```

### Comparing `mprov_esxiprovisioner-0.0.2/src/mprov_esxiprovisioner.egg-info/SOURCES.txt` & `mprov_esxiprovisioner-0.0.3/src/mprov_esxiprovisioner.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
```

