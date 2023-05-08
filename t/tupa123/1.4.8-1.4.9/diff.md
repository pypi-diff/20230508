# Comparing `tmp/tupa123-1.4.8.tar.gz` & `tmp/tupa123-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.8.tar", last modified: Thu May  4 14:49:46 2023, max compression
+gzip compressed data, was "tupa123-1.4.9.tar", last modified: Thu May  4 19:58:02 2023, max compression
```

## Comparing `tupa123-1.4.8.tar` & `tupa123-1.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 14:49:46.687133 tupa123-1.4.8/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-05-04 14:49:46.687133 tupa123-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 14:49:46.687133 tupa123-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-05-04 14:49:10.000000 tupa123-1.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:49:46.655887 tupa123-1.4.8/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.8/tupa123/__init__.py
--rw-rw-rw-   0        0        0    75594 2023-05-04 14:46:14.000000 tupa123-1.4.8/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:49:46.671647 tupa123-1.4.8/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 14:49:46.000000 tupa123-1.4.8/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 19:58:02.403366 tupa123-1.4.9/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-05-04 19:58:02.403366 tupa123-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 19:58:02.403366 tupa123-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-04 19:54:48.000000 tupa123-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:58:02.387746 tupa123-1.4.9/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.9/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    76640 2023-05-04 19:50:42.000000 tupa123-1.4.9/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:58:02.403366 tupa123-1.4.9/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-05-04 19:58:02.000000 tupa123-1.4.9/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-04 19:58:02.000000 tupa123-1.4.9/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 19:58:02.000000 tupa123-1.4.9/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 19:58:02.000000 tupa123-1.4.9/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 19:58:02.000000 tupa123-1.4.9/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.8/LICENSE.txt` & `tupa123-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.8/PKG-INFO` & `tupa123-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.8
+Version: 1.4.9
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.8/README.md` & `tupa123-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.8/setup.py` & `tupa123-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.8',
+    version='1.4.9',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.8/tupa123/tupa123.py` & `tupa123-1.4.9/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,43 @@
         plt.legend(loc = "upper left")
         plt.show()
 
 
 
 
 
+#Plot 3 variables ifferences in a sequential series, min, max, target
+def PlotComparativeB3(CalculatedMin, CalculatedMax, Targeted):
+
+    numdata,numevar = Targeted.shape
+    eixoX = np.arange(0, numdata, dtype=int)
+
+    for j in range(0,numevar):    
+        eixoY1= Targeted[:,j]
+        eixoY2= CalculatedMin[:,j]
+        eixoY3= CalculatedMax[:,j]
+    
+        plt.figure(figsize=(12, 5))
+        plt.title('Comparison calculated variable range vs target')
+        plt.xlabel('Sequence of events')
+        plt.ylabel('Target and predicted variable ' + str(j+1))
+        plt.plot(eixoX, eixoY1, marker = '', label='Target', c='red', alpha=0.9)
+        
+        plt.plot(eixoX, eixoY2, marker = '', label='Calculated min', c='black', alpha=0.5)
+        plt.plot(eixoX, eixoY3, marker = '', label='Calculated max', c='black', alpha=0.5)
+        
+        plt.fill_between(np.arange(len(eixoY1)), eixoY2, eixoY3, color='gray', alpha=0.1)
+        
+        plt.legend(loc = "upper left")
+        plt.show()
+        
+
+
+
+
 
 
 #Plot the differences of two variables in a sequential series
 def PlotComparative2(Calculated, Targeted, window_size=10):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
```

### Comparing `tupa123-1.4.8/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.9/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.8
+Version: 1.4.9
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

