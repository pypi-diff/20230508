# Comparing `tmp/pyfoundt-0.6.8.tar.gz` & `tmp/pyfoundt-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfoundt-0.6.8.tar", last modified: Sat Apr 29 02:45:54 2023, max compression
+gzip compressed data, was "pyfoundt-0.7.9.tar", last modified: Mon May  8 12:03:34 2023, max compression
```

## Comparing `pyfoundt-0.6.8.tar` & `pyfoundt-0.7.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:45:54.951129 pyfoundt-0.6.8/
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:33:21.000000 pyfoundt-0.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0      378 2023-04-29 02:45:54.950130 pyfoundt-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-20 10:07:47.000000 pyfoundt-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 02:45:54.929143 pyfoundt-0.6.8/pyfoundt/
--rw-rw-rw-   0        0        0       31 2023-04-29 02:09:19.000000 pyfoundt-0.6.8/pyfoundt/__init__.py
--rw-rw-rw-   0        0        0     6366 2023-04-10 11:36:17.000000 pyfoundt-0.6.8/pyfoundt/setplt.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:45:54.945133 pyfoundt-0.6.8/pyfoundt.egg-info/
--rw-rw-rw-   0        0        0      378 2023-04-29 02:45:54.000000 pyfoundt-0.6.8/pyfoundt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-29 02:45:54.000000 pyfoundt-0.6.8/pyfoundt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:45:54.000000 pyfoundt-0.6.8/pyfoundt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 02:45:54.000000 pyfoundt-0.6.8/pyfoundt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 02:45:54.000000 pyfoundt-0.6.8/pyfoundt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 02:45:54.951129 pyfoundt-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-04-29 02:45:12.000000 pyfoundt-0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:45:54.947144 pyfoundt-0.6.8/tests/
--rw-rw-rw-   0        0        0     3270 2023-04-29 02:11:11.000000 pyfoundt-0.6.8/tests/test_setplt.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:34.020469 pyfoundt-0.7.9/
+-rw-rw-rw-   0        0        0     1073 2023-05-07 11:02:30.000000 pyfoundt-0.7.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      378 2023-05-08 12:03:34.019472 pyfoundt-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-08 11:59:15.000000 pyfoundt-0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:33.996533 pyfoundt-0.7.9/pyfoundt/
+-rw-rw-rw-   0        0        0       31 2023-05-08 11:34:05.000000 pyfoundt-0.7.9/pyfoundt/__init__.py
+-rw-rw-rw-   0        0        0     3461 2023-05-08 11:52:21.000000 pyfoundt-0.7.9/pyfoundt/setplt.py
+-rw-rw-rw-   0        0        0     4409 2023-05-08 11:18:46.000000 pyfoundt-0.7.9/pyfoundt/useragents.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:34.011492 pyfoundt-0.7.9/pyfoundt.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-08 12:03:33.000000 pyfoundt-0.7.9/pyfoundt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-08 12:03:33.000000 pyfoundt-0.7.9/pyfoundt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:03:33.000000 pyfoundt-0.7.9/pyfoundt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 12:03:33.000000 pyfoundt-0.7.9/pyfoundt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 12:03:33.000000 pyfoundt-0.7.9/pyfoundt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:03:34.021466 pyfoundt-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-05-08 12:02:09.000000 pyfoundt-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:34.017476 pyfoundt-0.7.9/tests/
+-rw-rw-rw-   0        0        0     3235 2023-05-08 11:54:20.000000 pyfoundt-0.7.9/tests/test_setplt.py
+-rw-rw-rw-   0        0        0     5397 2023-05-08 11:42:03.000000 pyfoundt-0.7.9/tests/test_useragents.py
```

### Comparing `pyfoundt-0.6.8/LICENSE.txt` & `pyfoundt-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfoundt-0.6.8/setup.py` & `pyfoundt-0.7.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyfoundt',
     packages=find_packages(),
-    version='0.6.8',
+    version='0.7.9',
     install_requires=[
         "requests"
     ],
     author="ZuoYihan(左易晗)[china(中国)]",
     description="一个普通的模块",
     long_description="一个简洁且易于上手的一种包含了Python语言一些常用操作的模块.",
     platforms=["Windows", "Linux"],
```

### Comparing `pyfoundt-0.6.8/tests/test_setplt.py` & `pyfoundt-0.7.9/tests/test_setplt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 import unittest
-from pyfoundt.pyfoundt import setplt
+from pyfoundt import setplt
 
 te = 1
-set_plt.xin_jian_file("c:/ll.txt")
-set_plt.xin_jian_file("c:/l.txt")
-pip = set_plt.PipOperation()
+setplt.newfile("c:/ll.txt")
+setplt.new_ile("c:/l.txt")
+pip = setplt.PipOperation()
 pip.uninstall("numpy", "c:/")
 pip.install("numpy", "c:/")
-pip.upgrade_pip("c:/")
-pip.pip_list("c:/")
+pip.upgrademodular("c:/pip")
+pip.piplist("c:/")
 
 
 class TestSetPltFoundent(unittest.TestCase):
-    def test_xin_jian_file(self):
+    def test_newfile(self):
         try:
             with open("c:/ll.txt", "r") as f:
                 f.close()
         except Exception:
             self.assertEqual(te, 2)
         else:
             self.assertEqual(te, 1)
             f.close()
 
-    def test_return_file_info(self):
-        l = set_plt.return_file_info("c:/ll.txt")
+    def test_returnfileinfo(self):
+        l = setplt.return_file_info("c:/ll.txt")
         with open("c:/ll.txt", "r") as f:
             lv = f.read()
             self.assertEqual(l, lv)
             f.close()
 
     def test_delete(self):
-        set_plt.delete("c:/l.txt")
+        setplt.delete("c:/l.txt")
         try:
             with open("c:/l.txt") as f:
                 f.close()
         except Exception:
             self.assertEqual(te, 1)
         else:
             self.assertEqual(te, 2)
             f.close()
 
-    def test_return_url_info(self):
+    def test_returnrlnfo(self):
         import requests
-        l = set_plt.return_url_info("https://baidu.com")
+        l = setplt.return_url_info("https://baidu.com")
         lv = requests.get("https://baidu.com").text
         self.assertEqual(l, lv)
 
-    def test_get_url_Infile(self):
+    def test_geturlInfile(self):
         import requests
-        set_plt.get_url_Infile("https://baidu.com")
+        setplt.get_url_Infile("https://baidu.com")
         r = requests.get("https://baidu.com")
         r.encoding = "utf-8"
         with open("c:/n.html", "wb") as f:
             f.write(r.content)
         try:
             with open("c:/.html", "r", encoding="utf-8") as f:
                 rv = f.read()
@@ -81,15 +81,15 @@
             with open("c:/uninstall -numpy.bat", "r"):
                 print()
         except FileNotFoundError:
             self.assertEqual(te, 2)
         else:
             self.assertEqual(te, 1)
 
-    def test_upgrade_pip(self):
+    def test_upgrademodular(self):
         try:
             with open("c:/upgrade pip.bat", "r"):
                 print()
         except FileNotFoundError:
             self.assertEqual(te, 2)
         else:
             self.assertEqual(te, 1)
@@ -103,15 +103,15 @@
         else:
             self.assertEqual(te, 1)
 
 
 class TestClassTime(unittest.TestCase):
     def test_now(self):
         from datetime import datetime
-        time = set_plt.Time
+        time = setplt.Time
         n = time.now(detailed=True)
         nv = datetime.now()
         self.assertEqual(n, nv)
 
 
 if __name__ == "__main__":
     unittest.main()
```

