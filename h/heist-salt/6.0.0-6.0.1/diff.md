# Comparing `tmp/heist-salt-6.0.0.tar.gz` & `tmp/heist-salt-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heist-salt-6.0.0.tar", last modified: Wed May  3 19:49:26 2023, max compression
+gzip compressed data, was "heist-salt-6.0.1.tar", last modified: Mon May  8 17:04:31 2023, max compression
```

## Comparing `heist-salt-6.0.0.tar` & `heist-salt-6.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)    11342 2023-05-02 20:35:58.000000 heist-salt-6.0.0/LICENSE
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2417 2023-05-03 19:49:26.553431 heist-salt-6.0.0/PKG-INFO
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1856 2023-05-03 18:58:51.000000 heist-salt-6.0.0/README.rst
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/artifact/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)    20587 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/artifact/salt.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1848 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/conf.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.546764 heist-salt-6.0.0/heist_salt/heist/
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/heist/salt/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)    17322 2023-05-03 15:04:25.000000 heist-salt-6.0.0/heist_salt/heist/salt/init.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     4684 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/heist/salt/master.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     5991 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/heist/salt/minion.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     5729 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/heist/salt/proxy.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/salt/
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/salt/call/
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/salt/call/contracts/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      280 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/call/contracts/init.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1851 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/call/init.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/init.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/salt/key/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      108 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/api.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/salt/key/contracts/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      134 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/contracts/init.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     6344 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/init.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2125 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/local_master.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      108 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/raas.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/salt/pillar/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1598 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/pillar/init.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/service/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      186 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/service/init.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/service/salt/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     5702 2023-05-03 17:04:40.000000 heist-salt-6.0.0/heist_salt/service/salt/init.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/tool/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      974 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/artifacts.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1607 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/config.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/init.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1081 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/service.py
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       18 2023-05-03 17:06:32.000000 heist-salt-6.0.0/heist_salt/version.py
-drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt.egg-info/
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2417 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/PKG-INFO
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      850 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/SOURCES.txt
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)        1 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/dependency_links.txt
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       50 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/requires.txt
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       11 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/top_level.txt
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      921 2023-05-02 20:35:58.000000 heist-salt-6.0.0/pyproject.toml
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       38 2023-05-03 19:49:26.553431 heist-salt-6.0.0/setup.cfg
--rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2095 2023-05-02 20:35:58.000000 heist-salt-6.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.529930 heist-salt-6.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-05-08 17:04:01.000000 heist-salt-6.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-08 17:04:31.529930 heist-salt-6.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-05-08 17:04:01.000000 heist-salt-6.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.518929 heist-salt-6.0.1/heist_salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.521929 heist-salt-6.0.1/heist_salt/artifact/
+-rw-rw-rw-   0 root         (0) root         (0)    20587 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/artifact/salt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.513928 heist-salt-6.0.1/heist_salt/heist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.522929 heist-salt-6.0.1/heist_salt/heist/salt/
+-rw-rw-rw-   0 root         (0) root         (0)    17322 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     4684 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/master.py
+-rw-rw-rw-   0 root         (0) root         (0)     5991 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/minion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5729 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.523929 heist-salt-6.0.1/heist_salt/salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.523929 heist-salt-6.0.1/heist_salt/salt/call/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.524929 heist-salt-6.0.1/heist_salt/salt/call/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/call/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/call/init.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.525929 heist-salt-6.0.1/heist_salt/salt/key/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.526929 heist-salt-6.0.1/heist_salt/salt/key/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/local_master.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/raas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.526929 heist-salt-6.0.1/heist_salt/salt/pillar/
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/pillar/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.526929 heist-salt-6.0.1/heist_salt/service/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/service/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.527929 heist-salt-6.0.1/heist_salt/service/salt/
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/service/salt/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.528930 heist-salt-6.0.1/heist_salt/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/service.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.520929 heist-salt-6.0.1/heist_salt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-08 17:04:01.000000 heist-salt-6.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 17:04:31.529930 heist-salt-6.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-08 17:04:01.000000 heist-salt-6.0.1/setup.py
```

### Comparing `heist-salt-6.0.0/LICENSE` & `heist-salt-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/PKG-INFO` & `heist-salt-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist-salt
-Version: 6.0.0
+Version: 6.0.1
 Summary: Vertical app-merge components for salt into heist
 Home-page: 
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `heist-salt-6.0.0/README.rst` & `heist-salt-6.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/artifact/salt.py` & `heist-salt-6.0.1/heist_salt/artifact/salt.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/conf.py` & `heist-salt-6.0.1/heist_salt/conf.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/heist/salt/init.py` & `heist-salt-6.0.1/heist_salt/heist/salt/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/heist/salt/master.py` & `heist-salt-6.0.1/heist_salt/heist/salt/master.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/heist/salt/minion.py` & `heist-salt-6.0.1/heist_salt/heist/salt/minion.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/heist/salt/proxy.py` & `heist-salt-6.0.1/heist_salt/heist/salt/proxy.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/salt/call/init.py` & `heist-salt-6.0.1/heist_salt/salt/call/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/salt/key/init.py` & `heist-salt-6.0.1/heist_salt/salt/key/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,24 @@
         key_dir = run_dir / "root_dir" / "conf" / "pki" / minion_type
     else:
         key_dir = run_dir / "root_dir" / "etc" / "salt" / "pki" / minion_type
 
     hub.log.debug(f"Create and secure pki dir and parent directores: {key_dir}")
     if target_os == "windows":
         # Owner (OW), System (SY), and Administrators (BA) have Full Control
-        sddl = "D:PAI(A;OICI;FA;;;OW)(A;OICI;FA;;;SY)(A;OICI;FA;;;BA)"
-        owner = r'[System.Security.Principal.NTAccount]"BUILTIN\Administrators"'
-        cmd = (
-            "powershell -command "
-            + "'"
-            + "; ".join(
-                [
-                    f'New-Item -Path "{key_dir}" -Type Directory',
-                    f'$acl = Get-Acl "{key_dir.parent}"',
-                    f'$acl.SetSecurityDescriptorSddlForm("{sddl}")',
-                    f"$acl.SetOwner({owner})",
-                    f'Set-Acl -Path "{key_dir.parent}" -AclObject $acl',
-                ]
-            )
-            + "'"
+        sddl = "'D:PAI(A;OICI;FA;;;OW)(A;OICI;FA;;;SY)(A;OICI;FA;;;BA)'"
+        owner = r"[System.Security.Principal.NTAccount]'BUILTIN\Administrators'"
+        cmd = "; ".join(
+            [
+                f'powershell -command "New-Item -Path "{key_dir}" -Type Directory',
+                f'$acl = Get-Acl "{key_dir.parent}"',
+                f'$acl.SetSecurityDescriptorSddlForm("{sddl}")',
+                f"$acl.SetOwner({owner})",
+                f'Set-Acl -Path "{key_dir.parent}" -AclObject $acl"',
+            ]
         )
     else:
         # mkdir will not add the correct permissions to the parent directories
         # unless each directory is specified
         perms = 0o710 if hub.tunnel.asyncssh.CONS[target_name].get("sudo") else 0o700
         cmd = f"mkdir -m{perms:o} -p {key_dir.parent.parent.parent} {key_dir.parent.parent} {key_dir.parent} {key_dir}"
```

### Comparing `heist-salt-6.0.0/heist_salt/salt/key/local_master.py` & `heist-salt-6.0.1/heist_salt/salt/key/local_master.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/salt/pillar/init.py` & `heist-salt-6.0.1/heist_salt/salt/pillar/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/service/salt/init.py` & `heist-salt-6.0.1/heist_salt/service/salt/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/tool/artifacts.py` & `heist-salt-6.0.1/heist_salt/tool/artifacts.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/tool/config.py` & `heist-salt-6.0.1/heist_salt/tool/config.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt/tool/service.py` & `heist-salt-6.0.1/heist_salt/tool/service.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/heist_salt.egg-info/PKG-INFO` & `heist-salt-6.0.1/heist_salt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist-salt
-Version: 6.0.0
+Version: 6.0.1
 Summary: Vertical app-merge components for salt into heist
 Home-page: 
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `heist-salt-6.0.0/heist_salt.egg-info/SOURCES.txt` & `heist-salt-6.0.1/heist_salt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/pyproject.toml` & `heist-salt-6.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.0/setup.py` & `heist-salt-6.0.1/setup.py`

 * *Files identical despite different names*

