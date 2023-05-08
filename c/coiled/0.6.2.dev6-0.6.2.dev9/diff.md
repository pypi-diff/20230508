# Comparing `tmp/coiled-0.6.2.dev6.tar.gz` & `tmp/coiled-0.6.2.dev9.tar.gz`

## Comparing `coiled-0.6.2.dev6.tar` & `coiled-0.6.2.dev9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_version.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/context.py
--rw-r--r--   0        0        0   112046 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/magic.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/software.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/types.py
--rw-r--r--   0        0        0    47640 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    84970 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    60439 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/README.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/pyproject.toml
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 coiled-0.6.2.dev6/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_version.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/context.py
+-rw-r--r--   0        0        0   112046 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/magic.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/software.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/types.py
+-rw-r--r--   0        0        0    47664 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/websockets.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    84970 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    60439 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/README.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/pyproject.toml
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 coiled-0.6.2.dev9/PKG-INFO
```

### Comparing `coiled-0.6.2.dev6/coiled/__init__.py` & `coiled-0.6.2.dev9/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/analytics.py` & `coiled-0.6.2.dev9/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cluster.py` & `coiled-0.6.2.dev9/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/coiled.yaml` & `coiled-0.6.2.dev9/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/context.py` & `coiled-0.6.2.dev9/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/core.py` & `coiled-0.6.2.dev9/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/exceptions.py` & `coiled-0.6.2.dev9/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/magic.py` & `coiled-0.6.2.dev9/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/scan.py` & `coiled-0.6.2.dev9/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/software.py` & `coiled-0.6.2.dev9/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/types.py` & `coiled-0.6.2.dev9/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/utils.py` & `coiled-0.6.2.dev9/coiled/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,16 +419,16 @@
                 "token": token,
                 "server": server,
                 "account": account,
             }
         }
         config, config_file = save_config(new_config=creds)
         rich.print(f"Credentials have been saved at [blue]{config_file}")
-        # Make sure saved configuration values are set for the current Python process
-        dask.config.set(config)
+        # Make sure saved configuration values are set for the current Python process.
+        dask.config.update(dask.config.config, config)
 
     return user, token, server
 
 
 def save_config(new_config: dict) -> tuple[dict, str]:
     """Save new config values to Coiled config file, return new config and path to file."""
     config_file = os.path.join(os.path.expanduser("~"), ".config", "dask", "coiled.yaml")
```

### Comparing `coiled-0.6.2.dev6/coiled/websockets.py` & `coiled-0.6.2.dev9/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/cluster.py` & `coiled-0.6.2.dev9/coiled/_beta/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/core.py` & `coiled-0.6.2.dev9/coiled/_beta/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/cwi_log_link.py` & `coiled-0.6.2.dev9/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/states.py` & `coiled-0.6.2.dev9/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/widgets/__init__.py` & `coiled-0.6.2.dev9/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/widgets/rich.py` & `coiled-0.6.2.dev9/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/_beta/widgets/util.py` & `coiled-0.6.2.dev9/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/config.py` & `coiled-0.6.2.dev9/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/core.py` & `coiled-0.6.2.dev9/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/curl.py` & `coiled-0.6.2.dev9/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/env.py` & `coiled-0.6.2.dev9/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/login.py` & `coiled-0.6.2.dev9/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/package_sync.py` & `coiled-0.6.2.dev9/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/utils.py` & `coiled-0.6.2.dev9/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/cluster/__init__.py` & `coiled-0.6.2.dev9/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/cluster/better_logs.py` & `coiled-0.6.2.dev9/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/cluster/logs.py` & `coiled-0.6.2.dev9/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/cluster/ssh.py` & `coiled-0.6.2.dev9/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/notebook/__init__.py` & `coiled-0.6.2.dev9/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/notebook/notebook.py` & `coiled-0.6.2.dev9/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/setup/__init__.py` & `coiled-0.6.2.dev9/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/setup/amp.py` & `coiled-0.6.2.dev9/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/setup/aws.py` & `coiled-0.6.2.dev9/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/setup/entry.py` & `coiled-0.6.2.dev9/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/setup/gcp.py` & `coiled-0.6.2.dev9/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/cli/setup/prometheus.py` & `coiled-0.6.2.dev9/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/coiled/v2/__init__.py` & `coiled-0.6.2.dev9/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/LICENSE` & `coiled-0.6.2.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/README.md` & `coiled-0.6.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/pyproject.toml` & `coiled-0.6.2.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.2.dev6/PKG-INFO` & `coiled-0.6.2.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.2.dev6
+Version: 0.6.2.dev9
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.2.dev6 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.2.dev9 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
```

