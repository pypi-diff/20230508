# Comparing `tmp/beatlesalbuns-0.0.1.tar.gz` & `tmp/beatlesalbuns-0.0.2.tar.gz`

## Comparing `beatlesalbuns-0.0.1.tar` & `beatlesalbuns-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.1/src/beatlesalbuns/__init__.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.1/src/beatlesalbuns/beatlesalbuns.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.1/README.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.2/src/beatlesalbuns/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.2/src/beatlesalbuns/beatlesalbuns.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.2/README.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 beatlesalbuns-0.0.2/PKG-INFO
```

### Comparing `beatlesalbuns-0.0.1/src/beatlesalbuns/beatlesalbuns.py` & `beatlesalbuns-0.0.2/src/beatlesalbuns/beatlesalbuns.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,8 +16,9 @@
                       '11-Yellow Submarine',
                       '12-Abbey Road',
                       '13-Let It Be'],
                     'Year': [1963, 1963, 1964, 1964, 1965, 1965, 1966, 1967, 1967, 1968, 1969, 1969, 1970]}
     def show_albuns(self):
         #Converter dicionário numa Dataframe em Pandas
          print(f"=== Welcome! This is the list of The Beatles's albums ===".center(50))
+         print(f"=== I love The Beatles!! ===".center(50))
          return pd.DataFrame(self.balbums)
```

### Comparing `beatlesalbuns-0.0.1/LICENSE.txt` & `beatlesalbuns-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

