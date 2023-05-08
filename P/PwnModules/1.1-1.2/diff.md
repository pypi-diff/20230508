# Comparing `tmp/PwnModules-1.1.tar.gz` & `tmp/PwnModules-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PwnModules-1.1.tar", last modified: Tue Apr 25 14:58:36 2023, max compression
+gzip compressed data, was "PwnModules-1.2.tar", last modified: Mon May  8 12:25:49 2023, max compression
```

## Comparing `PwnModules-1.1.tar` & `PwnModules-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 14:58:36.196752 PwnModules-1.1/
--rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.1/License.txt
--rw-rw-rw-   0        0        0      747 2023-04-25 14:58:36.195754 PwnModules-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 14:58:36.193759 PwnModules-1.1/PwnModules.egg-info/
--rw-rw-rw-   0        0        0      747 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-04-25 14:58:36.000000 PwnModules-1.1/PwnModules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1823 2023-04-25 14:47:46.000000 PwnModules-1.1/PwnModules.py
--rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 14:58:36.196752 PwnModules-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:25:49.473729 PwnModules-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.2/License.txt
+-rw-rw-rw-   0        0        0      747 2023-05-08 12:25:49.473729 PwnModules-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 12:25:49.472731 PwnModules-1.2/PwnModules.egg-info/
+-rw-rw-rw-   0        0        0      747 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 12:25:49.000000 PwnModules-1.2/PwnModules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1829 2023-05-04 12:32:41.000000 PwnModules-1.2/PwnModules.py
+-rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:25:49.473729 PwnModules-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.2/setup.py
```

### Comparing `PwnModules-1.1/License.txt` & `PwnModules-1.2/License.txt`

 * *Files identical despite different names*

### Comparing `PwnModules-1.1/PKG-INFO` & `PwnModules-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.1
+Version: 1.2
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.1/PwnModules.egg-info/PKG-INFO` & `PwnModules-1.2/PwnModules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.1
+Version: 1.2
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.1/PwnModules.py` & `PwnModules-1.2/PwnModules.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Pwntools-Extern Functions
 开源包，任何人都可以使用并修改！
 """
 
 from LibcSearcher import *
 from pwn import *
 
-__version__ = '1.1'
+__version__ = '1.2'
 
 def leak_addr(i, io_i):
     if i == 0:
         address_internal = u32(io_i.recv(4))
         return address_internal
     if i == 1:
         address_internal = u64(io_i.recvuntil(b'\x7f')[:6].ljust(8, b'\x00'))
@@ -59,9 +59,9 @@
 
 
 def debug(io):
     gdb.attach(io)
     pause()
 
 
-def get_int_addr(io):
-    return int(io.recv(12), 16)
+def get_int_addr(io, num):
+    return int(io.recv(num), 16)
```

### Comparing `PwnModules-1.1/setup.py` & `PwnModules-1.2/setup.py`

 * *Files identical despite different names*

