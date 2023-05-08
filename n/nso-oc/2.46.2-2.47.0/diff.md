# Comparing `tmp/nso-oc-2.46.2.tar.gz` & `tmp/nso-oc-2.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.46.2.tar", last modified: Thu Apr 27 21:07:17 2023, max compression
+gzip compressed data, was "nso-oc-2.47.0.tar", last modified: Mon May  8 13:26:45 2023, max compression
```

## Comparing `nso-oc-2.46.2.tar` & `nso-oc-2.47.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:07:17.579881 nso-oc-2.46.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-27 21:06:44.000000 nso-oc-2.46.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 21:06:44.000000 nso-oc-2.46.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-27 21:07:17.579881 nso-oc-2.46.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-27 21:06:44.000000 nso-oc-2.46.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:07:17.579881 nso-oc-2.46.2/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-27 21:07:17.000000 nso-oc-2.46.2/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-27 21:07:17.000000 nso-oc-2.46.2/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:07:17.000000 nso-oc-2.46.2/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 21:07:17.000000 nso-oc-2.46.2/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 21:07:17.000000 nso-oc-2.46.2/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 21:07:17.000000 nso-oc-2.46.2/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:07:17.579881 nso-oc-2.46.2/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:07:17.579881 nso-oc-2.46.2/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29451 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:07:17.579881 nso-oc-2.46.2/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-27 21:06:44.000000 nso-oc-2.46.2/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-27 21:06:44.000000 nso-oc-2.46.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 21:07:17.583881 nso-oc-2.46.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 21:06:44.000000 nso-oc-2.46.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:26:45.647633 nso-oc-2.47.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-08 13:26:12.000000 nso-oc-2.47.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 13:26:12.000000 nso-oc-2.47.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-08 13:26:45.647633 nso-oc-2.47.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-08 13:26:12.000000 nso-oc-2.47.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:26:45.647633 nso-oc-2.47.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-08 13:26:45.000000 nso-oc-2.47.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-08 13:26:45.000000 nso-oc-2.47.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:26:45.000000 nso-oc-2.47.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 13:26:45.000000 nso-oc-2.47.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 13:26:45.000000 nso-oc-2.47.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 13:26:45.000000 nso-oc-2.47.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:26:45.647633 nso-oc-2.47.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:26:45.647633 nso-oc-2.47.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:26:45.647633 nso-oc-2.47.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-08 13:26:12.000000 nso-oc-2.47.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 13:26:12.000000 nso-oc-2.47.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 13:26:45.647633 nso-oc-2.47.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-08 13:26:12.000000 nso-oc-2.47.0/setup.py
```

### Comparing `nso-oc-2.46.2/LICENSE` & `nso-oc-2.47.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/PKG-INFO` & `nso-oc-2.47.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.46.2
+Version: 2.47.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.46.2/README.md` & `nso-oc-2.47.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.47.0/nso_oc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.46.2
+Version: 2.47.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.46.2/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.47.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/README.md` & `nso-oc-2.47.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/common.py` & `nso-oc-2.47.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/main.py` & `nso-oc-2.47.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,42 +179,44 @@
 
     openconfig_routing_policies["openconfig-routing-policy:routing-policy"]["openconfig-routing-policy:defined-sets"]["openconfig-bgp-policy:bgp-defined-sets"].update(as_path_sets)
 
 def process_community_sets(config_before, config_after):
     community_sets = {"openconfig-bgp-policy:community-sets": {"openconfig-bgp-policy:community-set": []}}
     community_list = config_before.get("tailf-ned-cisco-ios:ip", {}).get("community-list", {})
     community_list_after = config_after.get("tailf-ned-cisco-ios:ip", {}).get("community-list", {})
+    process_community_members(community_sets, "number", community_list, community_list_after)
     process_community_members(community_sets, "standard", community_list, community_list_after)
     process_community_members(community_sets, "expanded", community_list, community_list_after)
     openconfig_routing_policies["openconfig-routing-policy:routing-policy"]["openconfig-routing-policy:defined-sets"]["openconfig-bgp-policy:bgp-defined-sets"].update(community_sets)
 
 def process_community_members(community_sets, type, community_list, community_list_after):
     all_processed = True
     updated_community_list = []
+    name_or_num_key = "no" if type == "number" else "name"
 
     for community_index, community in enumerate(community_list.get(type, [])):
         new_community_set = {
-            "openconfig-bgp-policy:community-set-name": community.get("name"),
+            "openconfig-bgp-policy:community-set-name": community.get(name_or_num_key),
             "openconfig-bgp-policy:config": {
-                "openconfig-bgp-policy:community-set-name": community.get("name"),
+                "openconfig-bgp-policy:community-set-name": community.get(name_or_num_key),
                 "openconfig-bgp-policy:match-set-options": "ANY", # IOS only supports ANY
                 "openconfig-bgp-policy:community-member": []
             }
         }
         members = new_community_set["openconfig-bgp-policy:config"]["openconfig-bgp-policy:community-member"]
         entry_after = common.get_index_or_default(community_list_after.get(type, []), community_index, {}).get("entry", [])
 
         for entry_index, entry in enumerate(community.get("entry", [])):
             if not "expr" in entry:
                 continue
             if entry["expr"].startswith("deny"):
                 all_processed = False
                 routing_policy_notes.append(
 f"""
-Community Name: {community.get("name")}
+Community Name: {community.get(name_or_num_key)}
 Community Type: {type}
 Entry: {entry["expr"]}
 This entry contains a deny operation, which is not supported in OpenConfig. Translation, of the entire list, to OC will be skipped.
 """)
                 continue
 
             member = entry["expr"][entry["expr"].find(' ') + 1:]
@@ -222,56 +224,58 @@
 
             # Ensure the value we're nullifying does exist
             if common.get_index_or_default(entry_after, entry_index, None):
                 entry_after[entry_index] = None
 
         if all_processed:
             community_sets["openconfig-bgp-policy:community-sets"]["openconfig-bgp-policy:community-set"].append(new_community_set)
-            common.get_index_or_default(community_list_after.get(type, []), community_index, {})["name"] = None
+            common.get_index_or_default(community_list_after.get(type, []), community_index, {})[name_or_num_key] = None
     
     for community_list_item in community_list_after.get(type, []):
-        if "name" in community_list_item and community_list_item["name"]:
+        if name_or_num_key in community_list_item and community_list_item[name_or_num_key]:
             updated_community_list.append(community_list_item)
     
     if len(updated_community_list) > 0:
         community_list_after[type] = updated_community_list
     elif type in community_list_after:
         del community_list_after[type]
 
 def process_ext_community_sets(config_before, config_after):
     ext_community_sets = {"openconfig-bgp-policy:ext-community-sets": {"openconfig-bgp-policy:ext-community-set": []}}
     ext_community_list = config_before.get("tailf-ned-cisco-ios:ip", {}).get("extcommunity-list", {})
     ext_community_list_after = config_after.get("tailf-ned-cisco-ios:ip", {}).get("extcommunity-list", {})
+    process_ext_community_members(ext_community_sets, "number", ext_community_list, ext_community_list_after)
     process_ext_community_members(ext_community_sets, "standard", ext_community_list, ext_community_list_after)
     process_ext_community_members(ext_community_sets, "expanded", ext_community_list, ext_community_list_after)
     openconfig_routing_policies["openconfig-routing-policy:routing-policy"]["openconfig-routing-policy:defined-sets"]["openconfig-bgp-policy:bgp-defined-sets"].update(ext_community_sets)
 
 def process_ext_community_members(ext_community_sets, type, ext_community_list, ext_community_list_after):
     all_processed = True
     updated_ext_community_list = []
+    name_or_num_key = "no" if type == "number" else "name"
 
     for ext_community_index, ext_community in enumerate(ext_community_list.get(type, {"no-mode-list": []}).get("no-mode-list", [])):
         ext_new_community_set = {
-            "openconfig-bgp-policy:ext-community-set-name": ext_community.get("name"),
+            "openconfig-bgp-policy:ext-community-set-name": ext_community.get(name_or_num_key),
             "openconfig-bgp-policy:config": {
-                "openconfig-bgp-policy:ext-community-set-name": ext_community.get("name"),
+                "openconfig-bgp-policy:ext-community-set-name": ext_community.get(name_or_num_key),
                 "openconfig-bgp-policy:ext-community-member": []
             }
         }
         ext_members = ext_new_community_set["openconfig-bgp-policy:config"]["openconfig-bgp-policy:ext-community-member"]
         entry_after = common.get_index_or_default(ext_community_list_after.get(type, {"no-mode-list": []}).get("no-mode-list", []), ext_community_index, {}).get("entry", [])
 
         for entry_index, entry in enumerate(ext_community.get("entry", [])):
             if not "expr" in entry:
                 continue
             if entry["expr"].startswith("deny"):
                 all_processed = False
                 routing_policy_notes.append(
 f"""
-Ext Community Name: {ext_community.get("name")}
+Ext Community Name: {ext_community.get(name_or_num_key)}
 Ext Community Type: {type}
 Ext Entry: {entry["expr"]}
 This ext entry contains a deny operation, which is not supported in OpenConfig. Translation, of the entire list, to OC will be skipped.
 """)
                 continue
 
             member = entry["expr"][entry["expr"].find(' rt ') + 4:]
@@ -279,18 +283,18 @@
 
             # Ensure the value we're nullifying does exist
             if common.get_index_or_default(entry_after, entry_index, None):
                 entry_after[entry_index] = None
 
         if all_processed:
             ext_community_sets["openconfig-bgp-policy:ext-community-sets"]["openconfig-bgp-policy:ext-community-set"].append(ext_new_community_set)
-            common.get_index_or_default(ext_community_list_after.get(type, {"no-mode-list": []}).get("no-mode-list", []), ext_community_index, {})["name"] = None
+            common.get_index_or_default(ext_community_list_after.get(type, {"no-mode-list": []}).get("no-mode-list", []), ext_community_index, {})[name_or_num_key] = None
     
     for community_list_item in ext_community_list_after.get(type, {"no-mode-list": []}).get("no-mode-list", []):
-        if "name" in community_list_item and community_list_item["name"]:
+        if name_or_num_key in community_list_item and community_list_item[name_or_num_key]:
             updated_ext_community_list.append(community_list_item)
     
     if len(updated_ext_community_list) > 0:
         ext_community_list_after[type]["no-mode-list"] = updated_ext_community_list
     elif type in ext_community_list_after and "no-mode-list" in ext_community_list_after[type]:
         del ext_community_list_after[type]["no-mode-list"]
```

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.47.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.47.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.47.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.47.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.47.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.47.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.46.2/setup.py` & `nso-oc-2.47.0/setup.py`

 * *Files identical despite different names*

