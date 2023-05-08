# Comparing `tmp/sppersist-0.1.8.tar.gz` & `tmp/sppersist-0.1.9.tar.gz`

## Comparing `sppersist-0.1.8.tar` & `sppersist-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.8/src/spPersist/__init__.py
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 sppersist-0.1.8/src/spPersist/dp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.8/LICENSE
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sppersist-0.1.8/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sppersist-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.9/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 sppersist-0.1.9/src/spPersist/dp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.9/LICENSE
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sppersist-0.1.9/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sppersist-0.1.9/PKG-INFO
```

### Comparing `sppersist-0.1.8/src/spPersist/dp.py` & `sppersist-0.1.9/src/spPersist/dp.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,16 @@
   if 'GSE' in id_num:
     path = 'https://ftp.ncbi.nlm.nih.gov/geo/series/GSE'+id_num[3:6]+'nnn/'+id_num+'/suppl/'
   elif 'zenodo' in id_num:
     record_id = id_num.split('.')[-1]
     r = requests.get(f"https://zenodo.org/api/records/{record_id}") 
     urls = [f['links']['self'] for f in r.json()['files']]
     path = os.path.commonprefix(urls)
+    if not os.path.isdir(path):
+      path = os.path.dirname(path)
   else:
     raise ValueError(id_num + ' is neither GEO accession or Zenodo doi.')
 
   return path
 
 
 def zenodo_to_h5(doi: str, filename: str, ttype: str):
```

### Comparing `sppersist-0.1.8/LICENSE` & `sppersist-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.8/pyproject.toml` & `sppersist-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.1.8/PKG-INFO` & `sppersist-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.1.8
+Version: 0.1.9
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

