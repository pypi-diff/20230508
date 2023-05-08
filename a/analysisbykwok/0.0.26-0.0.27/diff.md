# Comparing `tmp/analysisbykwok-0.0.26.tar.gz` & `tmp/analysisbykwok-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.26.tar", last modified: Mon May  8 14:14:36 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.27.tar", last modified: Mon May  8 15:39:12 2023, max compression
```

## Comparing `analysisbykwok-0.0.26.tar` & `analysisbykwok-0.0.27.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:14:36.050233 analysisbykwok-0.0.26/
--rw-rw-rw-   0        0        0       62 2023-05-08 14:14:36.050233 analysisbykwok-0.0.26/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 14:14:36.045251 analysisbykwok-0.0.26/analysisbykwok/
--rw-rw-rw-   0        0        0    18404 2023-05-08 14:14:13.000000 analysisbykwok-0.0.26/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-08 14:13:20.000000 analysisbykwok-0.0.26/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:14:36.049236 analysisbykwok-0.0.26/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-05-08 14:14:36.000000 analysisbykwok-0.0.26/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-08 14:14:36.000000 analysisbykwok-0.0.26/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:14:36.000000 analysisbykwok-0.0.26/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:14:36.000000 analysisbykwok-0.0.26/analysisbykwok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 14:14:36.000000 analysisbykwok-0.0.26/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-05-08 14:13:14.000000 analysisbykwok-0.0.26/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 14:14:36.051231 analysisbykwok-0.0.26/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 15:39:12.351728 analysisbykwok-0.0.27/
+-rw-rw-rw-   0        0        0       62 2023-05-08 15:39:12.351728 analysisbykwok-0.0.27/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 15:39:12.351728 analysisbykwok-0.0.27/analysisbykwok/
+-rw-rw-rw-   0        0        0    18382 2023-05-08 15:38:50.000000 analysisbykwok-0.0.27/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-08 15:37:28.000000 analysisbykwok-0.0.27/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:39:12.351728 analysisbykwok-0.0.27/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-05-08 15:39:12.000000 analysisbykwok-0.0.27/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-08 15:39:12.000000 analysisbykwok-0.0.27/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:39:12.000000 analysisbykwok-0.0.27/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:39:12.000000 analysisbykwok-0.0.27/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 15:39:12.000000 analysisbykwok-0.0.27/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-05-08 15:37:28.000000 analysisbykwok-0.0.27/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:39:12.351728 analysisbykwok-0.0.27/setup.cfg
```

### Comparing `analysisbykwok-0.0.26/analysisbykwok/__init__.py` & `analysisbykwok-0.0.27/analysisbykwok/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         else:
             for i in range(0,len(list(date))):
                 if list(date)[i] in name:
                     pass
                 else:
                     del(date1[list(date)[i]])
         return date1
-
+class Model():
     def GetProbMatrix(df):
         name = []
         for son in df:
             if son not in name:
                 name.append(son)
         result = []
         name = np.sort(name)
@@ -379,22 +379,19 @@
                         result[i][ii] = result[i][ii] + 1
             sum = np.sum(result[i])
             for iiii in range(len(result[i])):
                 result[i][iiii] = result[i][iiii] / sum
             # print('sum is ',np.sum(result[i]),'序列',result[i],'\n')
         result = np.array(result)
         return result
-
     def ToMat(df):
-        df = df[-2:]
         wide = df.shape[1]
         high = df.shape[0]
         df = df.values
         result = []
         size = []
         for i in range(0, high):
             for ii in range(0, wide):
-                result.append([df[i][ii]])
+                result.append([[df[i][ii]]])
             size.append(wide)
-        result = np.mat(result)
-        back = [result, size]
+        back = [np.concatenate(result), size]
         return back
```

