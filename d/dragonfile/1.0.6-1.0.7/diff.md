# Comparing `tmp/dragonfile-1.0.6.tar.gz` & `tmp/dragonfile-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonfile-1.0.6.tar", last modified: Wed May  3 13:02:29 2023, max compression
+gzip compressed data, was "dragonfile-1.0.7.tar", last modified: Mon May  8 17:42:28 2023, max compression
```

## Comparing `dragonfile-1.0.6.tar` & `dragonfile-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:02:29.293263 dragonfile-1.0.6/
--rw-rw-rw-   0        0        0     1086 2023-04-20 14:31:16.000000 dragonfile-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-03 13:02:29.292264 dragonfile-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2023-04-24 14:05:19.000000 dragonfile-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 13:02:29.280275 dragonfile-1.0.6/dragonfile/
--rw-rw-rw-   0        0        0     1260 2023-05-03 12:55:30.000000 dragonfile-1.0.6/dragonfile/__init__.py
--rw-rw-rw-   0        0        0      253 2023-05-02 18:27:29.000000 dragonfile-1.0.6/dragonfile/fileToCsv.py
--rw-rw-rw-   0        0        0      231 2023-05-02 18:27:29.000000 dragonfile-1.0.6/dragonfile/lenColumns.py
--rw-rw-rw-   0        0        0      601 2023-05-02 18:27:29.000000 dragonfile-1.0.6/dragonfile/readFile.py
--rw-rw-rw-   0        0        0     1186 2023-05-02 18:27:29.000000 dragonfile-1.0.6/dragonfile/readFileRename.py
--rw-rw-rw-   0        0        0     1879 2023-05-02 18:27:29.000000 dragonfile-1.0.6/dragonfile/readFileSetPeriod.py
--rw-rw-rw-   0        0        0      778 2023-05-02 18:27:29.000000 dragonfile-1.0.6/dragonfile/readValues.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:02:29.288264 dragonfile-1.0.6/dragonfile.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-03 13:02:29.000000 dragonfile-1.0.6/dragonfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-05-03 13:02:29.000000 dragonfile-1.0.6/dragonfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:02:29.000000 dragonfile-1.0.6/dragonfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 13:02:29.000000 dragonfile-1.0.6/dragonfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 13:02:29.293263 dragonfile-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-05-03 12:57:46.000000 dragonfile-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:02:29.291268 dragonfile-1.0.6/tests/
--rw-rw-rw-   0        0        0        8 2023-04-24 14:05:19.000000 dragonfile-1.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:42:28.370249 dragonfile-1.0.7/
+-rw-rw-rw-   0        0        0     1086 2023-04-20 14:31:16.000000 dragonfile-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-08 17:42:28.369239 dragonfile-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-04-24 14:05:19.000000 dragonfile-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:42:28.357239 dragonfile-1.0.7/dragonfile/
+-rw-rw-rw-   0        0        0     1245 2023-05-08 17:31:14.000000 dragonfile-1.0.7/dragonfile/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-05-02 18:27:29.000000 dragonfile-1.0.7/dragonfile/fileToCsv.py
+-rw-rw-rw-   0        0        0      231 2023-05-02 18:27:29.000000 dragonfile-1.0.7/dragonfile/lenColumns.py
+-rw-rw-rw-   0        0        0      608 2023-05-08 17:30:16.000000 dragonfile-1.0.7/dragonfile/readFile.py
+-rw-rw-rw-   0        0        0     1189 2023-05-08 17:30:45.000000 dragonfile-1.0.7/dragonfile/readFileRename.py
+-rw-rw-rw-   0        0        0     1881 2023-05-08 17:30:41.000000 dragonfile-1.0.7/dragonfile/readFileSetPeriod.py
+-rw-rw-rw-   0        0        0      785 2023-05-08 17:30:58.000000 dragonfile-1.0.7/dragonfile/readValues.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:42:28.367238 dragonfile-1.0.7/dragonfile.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-08 17:42:28.000000 dragonfile-1.0.7/dragonfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-05-08 17:42:28.000000 dragonfile-1.0.7/dragonfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:42:28.000000 dragonfile-1.0.7/dragonfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 17:42:28.000000 dragonfile-1.0.7/dragonfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:42:28.370249 dragonfile-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-05-08 17:41:37.000000 dragonfile-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:42:28.368237 dragonfile-1.0.7/tests/
+-rw-rw-rw-   0        0        0        8 2023-04-24 14:05:19.000000 dragonfile-1.0.7/tests/__init__.py
```

### Comparing `dragonfile-1.0.6/LICENSE` & `dragonfile-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfile-1.0.6/PKG-INFO` & `dragonfile-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.6
+Version: 1.0.7
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dragonfile-1.0.6/README.md` & `dragonfile-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dragonfile-1.0.6/dragonfile/__init__.py` & `dragonfile-1.0.7/dragonfile/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from .readFile import readFile
 from .readFileSetPeriod import readFileSetPeriod
 from .readFileRename import readFileRename
 from .readValues import readValues
 from .fileToCsv import fileToCsv
 from .lenColumns import lenColumns
 
-class DragonFile:
-    def __init__ (self, dFile, nColumn, dSep=",", coding="utf-8", dictD={}, validate=False):
+class SetFile:
+    def __init__ (self, dFile, dSep=",", coding="utf-8", dictD={}, validate=False):
         self.dFile = dFile
-        self.nColumn = nColumn
         self.dSep = dSep
         self.coding = coding
         self.dictD = dictD
         self.validate = validate
     
     def readFile(self):
         return readFile(self)
 
     def readFileSetPeriod(self, varOp0="", varOp1="Manhã", varOp2="Tarde", varOp3="Noite", varLog0="6", varLog1="12", varLog2="18", twoColumn=False):
-        return readFileSetPeriod(self, varOp0="", varOp1="Manhã", varOp2="Tarde", varOp3="Noite", varLog0="6", varLog1="12", varLog2="18", twoColumn=False)
+        return readFileSetPeriod(self, varOp0=varOp0, varOp1=varOp1, varOp2=varOp2, varOp3=varOp3, varLog0=varLog0, varLog1=varLog1, varLog2=varLog2, twoColumn=twoColumn)
 
     def readFileRename(self, nameRow=[], renameRow=[], mode=False, varOp0=""):
-        return readFileRename(self, nameRow=[], renameRow=[], mode=False, varOp0="")
+        return readFileRename(self, nameRow=nameRow, renameRow=renameRow, mode=mode, varOp0=varOp0)
         
     def readValues(self):   
         return readValues(self)
 
     def fileToCsv(self):
         return fileToCsv(self)
```

### Comparing `dragonfile-1.0.6/dragonfile/readFile.py` & `dragonfile-1.0.7/dragonfile/readFile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import csv
 
-def readFile(self):
+def readFile(self, indexColumn):
         columns = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
-            nameColumn = header[self.nColumn]
+            nameColumn = header[indexColumn]
 
             for i, row in enumerate(reader):
-                columns.append(row[self.nColumn])
+                columns.append(row[indexColumn])
 
         dictDaux = {nameColumn: columns}
         self.dictD.update(dictDaux)
 
         if self.validate == True:
-            print("Termino",self.nColumn)
+            print("Finish",indexColumn)
         
-        self.nColumn += 1
+        indexColumn += 1
 
-        return self.dictD, self.nColumn
+        return self.dictD, indexColumn
```

### Comparing `dragonfile-1.0.6/dragonfile/readFileRename.py` & `dragonfile-1.0.7/dragonfile/readFileRename.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import csv
 
-def readFileRename(self, nameRow=[], renameRow=[], mode=False, varOp0=""):
+def readFileRename(self, indexColumn, nameRow=[], renameRow=[], mode=False, varOp0=""):
         columns = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
-            nameColumn = header[self.nColumn]
+            nameColumn = header[indexColumn]
 
             for row in reader:
                 if mode == False:
-                    if row[self.nColumn] in nameRow:
-                        index = nameRow.index(row[self.nColumn])
+                    if row[indexColumn] in nameRow:
+                        index = nameRow.index(row[indexColumn])
                         columns.append(renameRow[index])
                     else:
-                        columns.append(row[self.nColumn])
+                        columns.append(row[indexColumn])
                 else:
-                    if row[self.nColumn] in nameRow:
-                        index = nameRow.index(row[self.nColumn])
+                    if row[indexColumn] in nameRow:
+                        index = nameRow.index(row[indexColumn])
                         columns.append(renameRow[index])
                     else:
                         columns.append(varOp0)
 
             dictDaux = {nameColumn: columns}
             self.dictD.update(dictDaux)
 
             if self.validate == True:
-                    print("Termino",self.nColumn)
+                    print("Finish",indexColumn)
 
-            self.nColumn += 1
+            indexColumn += 1
 
-            return self.dictD, self.nColumn
+            return self.dictD, indexColumn
```

### Comparing `dragonfile-1.0.6/dragonfile/readFileSetPeriod.py` & `dragonfile-1.0.7/dragonfile/readFileSetPeriod.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import csv
 
-def readFileSetPeriod(self, varOp0="", varOp1="Manhã", varOp2="Tarde", varOp3="Noite", varLog0="6", varLog1="12", varLog2="18", twoColumn=False):
+def readFileSetPeriod(self, indexColumn, varOp0="", varOp1="Manhã", varOp2="Tarde", varOp3="Noite", varLog0="6", varLog1="12", varLog2="18", twoColumn=False):
         columns = []
         columnsTwo = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
-            nameColumn = header[self.nColumn]
-            extraColum = "New"+header[self.nColumn]
+            nameColumn = header[indexColumn]
+            extraColum = "New"+header[indexColumn]
             
             for i, row in enumerate(reader):
-                word = row[self.nColumn]
+                word = row[indexColumn]
 
                 if word != "":
                     word = int(word[0]+word[1])
                 else:
                     word = varOp0
 
                 if word != varOp0 :
@@ -29,30 +29,30 @@
                     else:
                         word = varOp3
                         
                 else:
                     pass
                 
                 columns.append(word)
-                columnsTwo.append(row[self.nColumn])
+                columnsTwo.append(row[indexColumn])
 
             if twoColumn == False:
                 dictDaux = {extraColum: columns}
                 self.dictD.update(dictDaux)
 
                 if self.validate == True:
-                    print("Termino",self.nColumn)
+                    print("Finish",indexColumn)
 
-                self.nColumn += 1
+                indexColumn += 1
             else:
                 dictDaux1 = {nameColumn: columnsTwo}
                 dictDaux2 = {extraColum: columns}
 
                 dictDaux1.update(dictDaux2)
                 self.dictD.update(dictDaux1)
 
                 if self.validate == True:
-                    print("Termino",self.nColumn)
+                    print("Finish",indexColumn)
 
-                self.nColumn += 1
+                indexColumn += 1
             
-            return self.dictD, self.nColumn
+            return self.dictD, indexColumn
```

### Comparing `dragonfile-1.0.6/dragonfile/readValues.py` & `dragonfile-1.0.7/dragonfile/readValues.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import csv
 
-def readValues(self):   
+def readValues(self, indexColumn):   
         columns = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
-            nameColumn = header[self.nColumn]
+            nameColumn = header[indexColumn]
 
             for i, row in enumerate(reader):
-                valor = row[self.nColumn]
+                valor = row[indexColumn]
                 
                 valor = valor.replace(".", "")
                 valor = valor.replace(",", ".")
                 columns.append(valor)
                         
 
         dictDaux = {nameColumn: columns}
         self.dictD.update(dictDaux)
 
         if self.validate == True:
-            print("Termino",self.nColumn)
+            print("Finish",indexColumn)
         
-        self.nColumn += 1
+        indexColumn += 1
 
-        return self.dictD, self.nColumn
+        return self.dictD, indexColumn
```

### Comparing `dragonfile-1.0.6/dragonfile.egg-info/PKG-INFO` & `dragonfile-1.0.7/dragonfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.6
+Version: 1.0.7
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dragonfile-1.0.6/setup.py` & `dragonfile-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dragonfile',
-    version='1.0.6',
+    version='1.0.7',
     description='Read CSV - Version Test',
     author='Gabriel Arantd Felipe',
     author_email='grantd.ctt@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

