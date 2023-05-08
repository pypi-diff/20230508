# Comparing `tmp/cagen-0.2.0rc3.tar.gz` & `tmp/cagen-0.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0rc3.tar", last modified: Mon May  8 16:22:59 2023, max compression
+gzip compressed data, was "cagen-0.2.0rc4.tar", last modified: Mon May  8 16:34:56 2023, max compression
```

## Comparing `cagen-0.2.0rc3.tar` & `cagen-0.2.0rc4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:22:59.099770 cagen-0.2.0rc3/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0rc3/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-05-08 16:22:59.099770 cagen-0.2.0rc3/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0rc3/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1148 2023-05-08 16:22:51.000000 cagen-0.2.0rc3/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-08 16:22:59.099770 cagen-0.2.0rc3/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:22:59.096436 cagen-0.2.0rc3/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:22:59.096436 cagen-0.2.0rc3/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0rc3/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4659 2023-05-07 17:29:41.000000 cagen-0.2.0rc3/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0rc3/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:22:59.099770 cagen-0.2.0rc3/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      714 2023-05-08 16:21:27.000000 cagen-0.2.0rc3/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0rc3/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     3998 2023-05-07 17:21:41.000000 cagen-0.2.0rc3/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0rc3/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:22:59.096436 cagen-0.2.0rc3/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-05-08 16:22:59.000000 cagen-0.2.0rc3/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-08 16:22:59.000000 cagen-0.2.0rc3/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-08 16:22:59.000000 cagen-0.2.0rc3/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       80 2023-05-08 16:22:59.000000 cagen-0.2.0rc3/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-08 16:22:59.000000 cagen-0.2.0rc3/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-08 16:22:59.000000 cagen-0.2.0rc3/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:34:56.686405 cagen-0.2.0rc4/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0rc4/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-05-08 16:34:56.686405 cagen-0.2.0rc4/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0rc4/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1148 2023-05-08 16:34:06.000000 cagen-0.2.0rc4/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-08 16:34:56.686405 cagen-0.2.0rc4/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:34:56.683071 cagen-0.2.0rc4/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:34:56.683071 cagen-0.2.0rc4/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0rc4/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4659 2023-05-07 17:29:41.000000 cagen-0.2.0rc4/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0rc4/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:34:56.686405 cagen-0.2.0rc4/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      786 2023-05-08 16:32:54.000000 cagen-0.2.0rc4/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0rc4/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     3998 2023-05-07 17:21:41.000000 cagen-0.2.0rc4/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0rc4/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-08 16:34:56.683071 cagen-0.2.0rc4/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-05-08 16:34:56.000000 cagen-0.2.0rc4/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-08 16:34:56.000000 cagen-0.2.0rc4/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-08 16:34:56.000000 cagen-0.2.0rc4/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       80 2023-05-08 16:34:56.000000 cagen-0.2.0rc4/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-08 16:34:56.000000 cagen-0.2.0rc4/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-08 16:34:56.000000 cagen-0.2.0rc4/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0rc3/PKG-INFO` & `cagen-0.2.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0rc3
+Version: 0.2.0rc4
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0rc3/README.md` & `cagen-0.2.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc3/pyproject.toml` & `cagen-0.2.0rc4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.rc3"
+version = "0.2.0.rc4"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0rc3/src/cagen/cmd.py` & `cagen-0.2.0rc4/src/cagen/cmd.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc3/src/cagen/libcagen.py` & `cagen-0.2.0rc4/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc3/src/cagen/templates/list.md.tmpl` & `cagen-0.2.0rc4/src/cagen/templates/list.md.tmpl`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   import types
 
 %>
 
 <%def name="make_index(col)">
 % for e in sorted(col.entries):
 - [${e}](${e.path})
-% enfor
+% endfor
 </%def>
 
 <%def name="sorted_index(col, crit)">
 
 <%
 grouped = cols.group_by(cri)
 %>
@@ -26,25 +26,27 @@
 
 % for entry in sorted(grouped[key]):
 - [${entry}](${entry.path})
 % endfor
 
 % endfor
 
-<%/def>
-
+</%def>
 
-% if groupby:
 
-% if isinstance(groupby, types.FunctionType):
-${sorted_index(collection, groupby)}
-% elif:
-<% criterium = lambda x: x.to_dict[groupby] if groupby in x.to_dict else None %>
-${sorted_index(collection, criterium)}
-% else:
-${make_index(col=collection)}
+% if groupby is not UNDEFINED:
+  % if isinstance(groupby, types.FunctionType):
+  ${sorted_index(collection, groupby)}
+  % elif isinstance(groupby, str):
+  <%
+    criterium = lambda x: x.to_dict[groupby] if groupby in x.to_dict else None
+  %>
+  ${sorted_index(collection, criterium)}
+  % else:
+  ${make_index(col=collection)}
+  % endif
 
 % else:
 
 ${make_index(col=collection)}
 
 % endif
```

### Comparing `cagen-0.2.0rc3/src/cagen/templates/schema.tmpl` & `cagen-0.2.0rc4/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc3/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0rc4/src/cagen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0rc3
+Version: 0.2.0rc4
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

