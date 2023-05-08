# Comparing `tmp/betweens-0.2.3.tar.gz` & `tmp/betweens-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-0.2.3.tar", last modified: Fri May  5 10:33:49 2023, max compression
+gzip compressed data, was "betweens-0.3.0.tar", last modified: Mon May  8 10:57:31 2023, max compression
```

## Comparing `betweens-0.2.3.tar` & `betweens-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:33:49.170697 betweens-0.2.3/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1180 2023-05-05 10:33:49.169696 betweens-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 10:33:49.158696 betweens-0.2.3/betweens/
--rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-0.2.3/betweens/__init__.py
--rw-rw-rw-   0        0        0     2565 2023-05-05 10:31:57.000000 betweens-0.2.3/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-0.2.3/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:33:49.167695 betweens-0.2.3/betweens.egg-info/
--rw-rw-rw-   0        0        0     1180 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 10:33:49.000000 betweens-0.2.3/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      355 2023-05-05 10:32:39.000000 betweens-0.2.3/new.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 10:33:49.170697 betweens-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-05-05 10:32:45.000000 betweens-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:57:31.081975 betweens-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-05-08 10:57:31.081975 betweens-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-08 10:56:31.000000 betweens-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 10:57:31.066354 betweens-0.3.0/betweens/
+-rw-rw-rw-   0        0        0      311 2023-05-05 10:33:20.000000 betweens-0.3.0/betweens/__init__.py
+-rw-rw-rw-   0        0        0     3905 2023-05-08 10:52:21.000000 betweens-0.3.0/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-05 10:18:08.000000 betweens-0.3.0/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:57:31.081975 betweens-0.3.0/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 10:57:31.000000 betweens-0.3.0/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      455 2023-05-08 10:53:43.000000 betweens-0.3.0/new.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:57:31.081975 betweens-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-05-08 10:52:35.000000 betweens-0.3.0/setup.py
```

### Comparing `betweens-0.2.3/LICENSE` & `betweens-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-0.2.3/PKG-INFO` & `betweens-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.2.3
+Version: 0.3.0
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
@@ -22,19 +22,19 @@
 License-File: LICENSE
 
 # Betweens
 
 This is a package named betweens.
 There are 3 between mode.
 
-### Between 1
+## Between 1
 
 two intergers.
 
-### Between 2
+## Between 2
 
 two lists, tuples or dicts.
 And two indexes.
 
-### Between 3
+## Between 3
 
-two length or area units.
+two length, area, volume or mass units
```

### Comparing `betweens-0.2.3/betweens/betweens.py` & `betweens-0.3.0/betweens/betweens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# -*- coding:utf-8 -*-
+
+
 def between1(a,b):
     '''Print numbers between a and b'''
     if type(a) != type(int()) and type(b) != type(int()):
         raise TypeError('Must be integer.')
     result = []
     if a>b:
         for i in range(a-1,b):
@@ -9,14 +12,15 @@
     elif a<b:
         for i in range(a-1,b,-1):
             result.append(i)
     else:
         print('a and b must be different!')
     return result
 
+
 def between2(l1,l2,a,b):
     '''Print numbers between l1[a] and l2[b]'''
     if type(l1) != type(list()) and type(l1) != type(tuple()) and type(l1) != type(dict()) and type(l2) != type(list()) and type(l2) != type(tuple()) and type(l1) != type(dict()):
         raise TypeError('l1, l2 must be list, dict or tuple.')
     if type(a) != type(int()) and type(b) != type(int()):
         raise TypeError('a, b must be integer.')
     result = []
@@ -26,42 +30,70 @@
     elif l1[a]<l2[b]:
         for i in range(l1[a-1],l2[b],-1):
             result.append(i)
     else:
         print('l1[a] and l2[b] must be different!')
     return result
 
+
 def between3(s1,s2):
     l1 = ['nm','um','mm','cm','dm','m','km']
     l2 = ['nm2','um2','mm2','cm2','dm2','m2','hm2','km2']
+    l3 = ['nm3','um3','mm3','cm3','dm3','m3','km3']
+    l4 = ['mg','g','kg','t']
     if type(s1) != type(str()) and type(s2) != type(str()):
         raise TypeError('Must be string.')
     result = []
-    if len(s1) != len(s2):
-        raise TypeError('s1 and s2 must be same type.')
-    if len(s1)==2:
+    if s1 in l1 and s2 in l2:
         try:
             if l1.index(s1)>l1.index(s2):
                 for i in l1[l1.index(s1)-1:l1.index(s2)]:
                     result.append(i)
             elif l1.index(s1)<l1.index(s2):
                 for i in l1[l1.index(s1)-1:l1.index(s2):-1]:
                     result.append(i)
             else:
                 print('s1 and s2 must be different!')
         except ValueError:
-            raise ValueError('s1 and s2 must be units of length or area.')
-    elif len(s1)==3:
+            raise ValueError('s1 and s2 must be one of the units of length, area, volume and mass.')
+    elif s1 in l2 and s2 in l2:
         try:
             if l2.index(s1)>l2.index(s2):
-                for i in l1[l2.index(s1)-1:l2.index(s2)]:
+                for i in l2[l2.index(s1)-1:l2.index(s2)]:
                     result.append(i)
-            elif l1.index(s1)<l1.index(s2):
+            elif l2.index(s1)<l2.index(s2):
                 for i in l2[l2.index(s1)-1:l2.index(s2):-1]:
                     result.append(i)
             else:
                 print('s1 and s2 must be different!')
         except ValueError:
-            raise ValueError('s1 and s2 must be units of length or area.')
+            raise ValueError('s1 and s2 must be one of the units of length, area, volume and mass.')
+    elif s1 in l3 and s2 in l3:
+        try:
+            if l3.index(s1)>l3.index(s2):
+                for i in l3[l3.index(s1)-1:l3.index(s2)]:
+                    result.append(i)
+            elif l3.index(s1)<l3.index(s2):
+                for i in l3[l3.index(s1)-1:l3.index(s2):-1]:
+                    result.append(i)
+            else:
+                print('s1 and s2 must be different!')
+        except ValueError:
+            raise ValueError('s1 and s2 must be one of the units of length, area, volume and mass.')
+    elif s1 in l4 and s2 in l4:
+        try:
+            if l4.index(s1)>l4.index(s2):
+                for i in l4[l4.index(s1)-1:l4.index(s2)]:
+                    result.append(i)
+            elif l4.index(s1)<l4.index(s2):
+                for i in l4[l4.index(s1)-1:l4.index(s2):-1]:
+                    result.append(i)
+            else:
+                print('s1 and s2 must be different!')
+        except ValueError:
+            raise ValueError('s1 and s2 must be one of the units of length, area, volume and mass.')
     else:
-        raise ValueError('s1 and s2 must be units of length or area.')
+        for i in range(4):
+            if s1 in eval('l' + str(i+1)):
+                raise ValueError('s1 and s2 must be same type.')
+        raise ValueError('s1 and s2 must be one of the units of length, area, volume and mass.')
     return result
```

### Comparing `betweens-0.2.3/betweens.egg-info/PKG-INFO` & `betweens-0.3.0/betweens.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.2.3
+Version: 0.3.0
 Author: yuanbaoge
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
@@ -22,19 +22,19 @@
 License-File: LICENSE
 
 # Betweens
 
 This is a package named betweens.
 There are 3 between mode.
 
-### Between 1
+## Between 1
 
 two intergers.
 
-### Between 2
+## Between 2
 
 two lists, tuples or dicts.
 And two indexes.
 
-### Between 3
+## Between 3
 
-two length or area units.
+two length, area, volume or mass units
```

### Comparing `betweens-0.2.3/setup.py` & `betweens-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 long_description = None
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='betweens', # 包名称
       packages=find_packages(), # 需要处理的包目录
-      version='0.2.3', # 版本
+      version='0.3.0', # 版本
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python', 'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Operating System :: MacOS :: MacOS X',
           'Operating System :: Microsoft :: Windows :: Windows 10',
```

