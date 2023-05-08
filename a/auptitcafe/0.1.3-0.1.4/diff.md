# Comparing `tmp/auptitcafe-0.1.3.tar.gz` & `tmp/auptitcafe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.3.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.4.tar", max compression
```

## Comparing `auptitcafe-0.1.3.tar` & `auptitcafe-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.3/auptitcafe/__init__.py
--rw-r--r--   0        0        0     1928 2023-05-08 01:45:43.605501 auptitcafe-0.1.3/auptitcafe/menus.py
--rw-r--r--   0        0        0      501 2023-05-08 01:45:31.385359 auptitcafe-0.1.3/auptitcafe/plat.py
--rw-r--r--   0        0        0      441 2023-05-08 01:49:51.028751 auptitcafe-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.4/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     1932 2023-05-08 01:59:35.083951 auptitcafe-0.1.4/auptitcafe/menus.py
+-rw-r--r--   0        0        0      502 2023-05-08 01:58:46.975392 auptitcafe-0.1.4/auptitcafe/plat.py
+-rw-r--r--   0        0        0      441 2023-05-08 01:59:41.472027 auptitcafe-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.4/PKG-INFO
```

### Comparing `auptitcafe-0.1.3/auptitcafe/menus.py` & `auptitcafe-0.1.4/auptitcafe/menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,11 +46,11 @@
                         details = recette,
                         img_url = image)
             print("================================================================")
             out.append(plat)
         return out
 
     def get_all_as_df(self):
-        df = pd.DataFrame.from_records([plat.to_dict() for plat in Menus.get_all(self)])
+        df = pd.DataFrame.from_records([plat.to_dict(self) for plat in Menus.get_all(self)])
         return df
```

### Comparing `auptitcafe-0.1.3/PKG-INFO` & `auptitcafe-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auptitcafe
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

