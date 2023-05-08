# Comparing `tmp/auptitcafe-0.1.1.tar.gz` & `tmp/auptitcafe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.1.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.2.tar", max compression
```

## Comparing `auptitcafe-0.1.1.tar` & `auptitcafe-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.1/auptitcafe/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-08 01:33:58.893072 auptitcafe-0.1.1/auptitcafe/menus.py
--rw-r--r--   0        0        0      280 2023-05-08 01:32:24.031863 auptitcafe-0.1.1/auptitcafe/plat.py
--rw-r--r--   0        0        0      441 2023-05-08 01:34:50.885782 auptitcafe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.2/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     1928 2023-05-08 01:45:43.605501 auptitcafe-0.1.2/auptitcafe/menus.py
+-rw-r--r--   0        0        0      501 2023-05-08 01:45:31.385359 auptitcafe-0.1.2/auptitcafe/plat.py
+-rw-r--r--   0        0        0      441 2023-05-08 01:45:22.073255 auptitcafe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.2/PKG-INFO
```

### Comparing `auptitcafe-0.1.1/auptitcafe/menus.py` & `auptitcafe-0.1.2/auptitcafe/menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,11 +47,10 @@
                         img_url = image)
             print("================================================================")
             out.append(plat)
         return out
 
     def get_all_as_df(self):
         df = pd.DataFrame.from_records([plat.to_dict() for plat in Menus.get_all(self)])
-        df
         return df
```

### Comparing `auptitcafe-0.1.1/PKG-INFO` & `auptitcafe-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auptitcafe
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

