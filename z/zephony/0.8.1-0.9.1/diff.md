# Comparing `tmp/zephony-0.8.1.tar.gz` & `tmp/zephony-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephony-0.8.1.tar", last modified: Thu Jun  9 16:35:41 2022, max compression
+gzip compressed data, was "zephony-0.9.1.tar", last modified: Sat Aug  6 19:32:26 2022, max compression
```

## Comparing `zephony-0.8.1.tar` & `zephony-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-09 16:35:40.995834 zephony-0.8.1/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      228 2022-06-09 16:35:40.995834 zephony-0.8.1/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)      233 2022-06-08 11:00:54.000000 zephony-0.8.1/README.md
--rw-r--r--   0 kevin     (1000) kevin     (1000)       79 2022-06-09 16:35:40.995834 zephony-0.8.1/setup.cfg
--rw-r--r--   0 kevin     (1000) kevin     (1000)      408 2022-06-09 16:35:19.000000 zephony-0.8.1/setup.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-09 16:35:40.995834 zephony-0.8.1/zephony/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2022-06-04 16:11:00.000000 zephony-0.8.1/zephony/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1544 2022-06-09 15:06:40.000000 zephony-0.8.1/zephony/decorators.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3689 2022-06-04 17:35:04.000000 zephony-0.8.1/zephony/exceptions.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    17947 2022-06-04 17:16:22.000000 zephony-0.8.1/zephony/helpers.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-09 16:35:40.995834 zephony-0.8.1/zephony/models/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    29406 2022-06-04 17:46:46.000000 zephony-0.8.1/zephony/models/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5188 2022-06-09 16:34:58.000000 zephony-0.8.1/zephony/validators.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-09 16:35:40.995834 zephony-0.8.1/zephony.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      228 2022-06-09 16:35:40.000000 zephony-0.8.1/zephony.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)      314 2022-06-09 16:35:40.000000 zephony-0.8.1/zephony.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2022-06-09 16:35:40.000000 zephony-0.8.1/zephony.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)       18 2022-06-09 16:35:40.000000 zephony-0.8.1/zephony.egg-info/requires.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        8 2022-06-09 16:35:40.000000 zephony-0.8.1/zephony.egg-info/top_level.txt
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-08-06 19:32:26.737912 zephony-0.9.1/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      228 2022-08-06 19:32:26.737912 zephony-0.9.1/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      233 2022-06-08 11:00:54.000000 zephony-0.9.1/README.md
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       79 2022-08-06 19:32:26.737912 zephony-0.9.1/setup.cfg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      408 2022-08-06 19:31:17.000000 zephony-0.9.1/setup.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-08-06 19:32:26.737912 zephony-0.9.1/zephony/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2022-06-04 16:11:00.000000 zephony-0.9.1/zephony/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1544 2022-06-09 15:06:40.000000 zephony-0.9.1/zephony/decorators.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3689 2022-06-04 17:35:04.000000 zephony-0.9.1/zephony/exceptions.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    17947 2022-06-04 17:16:22.000000 zephony-0.9.1/zephony/helpers.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-08-06 19:32:26.737912 zephony-0.9.1/zephony/models/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    29489 2022-08-06 19:30:50.000000 zephony-0.9.1/zephony/models/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5188 2022-06-09 16:34:58.000000 zephony-0.9.1/zephony/validators.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2022-08-06 19:32:26.737912 zephony-0.9.1/zephony.egg-info/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      228 2022-08-06 19:32:26.000000 zephony-0.9.1/zephony.egg-info/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      314 2022-08-06 19:32:26.000000 zephony-0.9.1/zephony.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2022-08-06 19:32:26.000000 zephony-0.9.1/zephony.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       18 2022-08-06 19:32:26.000000 zephony-0.9.1/zephony.egg-info/requires.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        8 2022-08-06 19:32:26.000000 zephony-0.9.1/zephony.egg-info/top_level.txt
```

### Comparing `zephony-0.8.1/zephony/decorators.py` & `zephony-0.9.1/zephony/decorators.py`

 * *Files identical despite different names*

### Comparing `zephony-0.8.1/zephony/exceptions.py` & `zephony-0.9.1/zephony/exceptions.py`

 * *Files identical despite different names*

### Comparing `zephony-0.8.1/zephony/helpers.py` & `zephony-0.9.1/zephony/helpers.py`

 * *Files identical despite different names*

### Comparing `zephony-0.8.1/zephony/models/__init__.py` & `zephony-0.9.1/zephony/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,16 @@
                     try:
                         date_str_format = '%d/%m/%Y' if '/' in row[v[0]] else '%Y-%m-%d'
                         data[k] = datetime.datetime.strptime(row[v[0]], date_str_format).isoformat()
                     except ValueError:
                         #TODO: Doing this only to make import work quickly
                         data[k] = None
                         # raise ValueError('`{}`: Cannot parse datetime'.format(row[v[0]]))
+                elif callable(v[1]):
+                    data[k] = v[1](row[v[0]])
                 else:
                     raise ValueError('`{}`: Unsupported type to type case to'.format(v[1]))
             elif len(v) == 3:
                 if v[2] == 'power_of_2':  # Used for permissions to calculate & store permission bit
                     # Permission bit cannot be empty
                     if not row[v[0]].strip():
                         raise ValueError('Permission bit value cannot be empty')
```

### Comparing `zephony-0.8.1/zephony/validators.py` & `zephony-0.9.1/zephony/validators.py`

 * *Files identical despite different names*

