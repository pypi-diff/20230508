# Comparing `tmp/django-simple-stats-0.5.1.tar.gz` & `tmp/django-simple-stats-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-stats-0.5.1.tar", last modified: Wed Apr 26 10:53:45 2023, max compression
+gzip compressed data, was "django-simple-stats-0.6.0.tar", last modified: Mon May  8 09:29:11 2023, max compression
```

## Comparing `django-simple-stats-0.5.1.tar` & `django-simple-stats-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:53:45.823779 django-simple-stats-0.5.1/
--rw-rw-rw-   0        0        0     1078 2022-03-11 07:15:01.000000 django-simple-stats-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    13946 2023-04-26 10:53:45.823224 django-simple-stats-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    12839 2023-04-26 10:46:12.000000 django-simple-stats-0.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-26 10:53:45.816313 django-simple-stats-0.5.1/django_simple_stats.egg-info/
--rw-rw-rw-   0        0        0    13946 2023-04-26 10:53:45.000000 django-simple-stats-0.5.1/django_simple_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-26 10:53:45.000000 django-simple-stats-0.5.1/django_simple_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:53:45.000000 django-simple-stats-0.5.1/django_simple_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-11 07:16:38.000000 django-simple-stats-0.5.1/django_simple_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-26 10:53:45.000000 django-simple-stats-0.5.1/django_simple_stats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-26 10:53:45.000000 django-simple-stats-0.5.1/django_simple_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:53:45.824331 django-simple-stats-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-26 10:46:17.000000 django-simple-stats-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:53:45.819872 django-simple-stats-0.5.1/simple_stats/
--rw-rw-rw-   0        0        0      205 2023-04-13 07:28:54.000000 django-simple-stats-0.5.1/simple_stats/__init__.py
--rw-rw-rw-   0        0        0     6729 2023-04-26 10:41:47.000000 django-simple-stats-0.5.1/simple_stats/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.092419 django-simple-stats-0.6.0/
+-rw-rw-rw-   0        0        0     1078 2022-03-11 07:15:01.000000 django-simple-stats-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    14026 2023-05-08 09:29:11.091421 django-simple-stats-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12913 2023-05-08 08:14:06.000000 django-simple-stats-0.6.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.083421 django-simple-stats-0.6.0/django_simple_stats.egg-info/
+-rw-rw-rw-   0        0        0    14026 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-08 09:29:11.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-03-11 07:16:38.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 09:29:11.092419 django-simple-stats-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-05-08 08:14:12.000000 django-simple-stats-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.086419 django-simple-stats-0.6.0/simple_stats/
+-rw-rw-rw-   0        0        0      235 2023-05-08 08:13:47.000000 django-simple-stats-0.6.0/simple_stats/__init__.py
+-rw-rw-rw-   0        0        0     6643 2023-05-08 09:15:43.000000 django-simple-stats-0.6.0/simple_stats/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.089422 django-simple-stats-0.6.0/tests/
+-rw-rw-rw-   0        0        0      314 2023-05-08 08:11:10.000000 django-simple-stats-0.6.0/tests/test_decl.py
+-rw-rw-rw-   0        0        0     1016 2023-05-08 08:44:00.000000 django-simple-stats-0.6.0/tests/test_stats.py
```

### Comparing `django-simple-stats-0.5.1/LICENSE` & `django-simple-stats-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-stats-0.5.1/PKG-INFO` & `django-simple-stats-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-stats
-Version: 0.5.1
+Version: 0.6.0
 Summary: A django package for creating simple stats from a query
 Home-page: https://github.com/spapas/django-simple-stats
 Author: Serafeim Papastefanos
 Author-email: spapas@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
@@ -25,14 +25,19 @@
 django-simple-stats
 -------------------
 
 A django package for creating stats from a query. 
 This package should be compatible with all 
 Django versions > 3.x
 
+
+
+.. image:: ./showme.png
+  :alt: How does it look
+
 Installation
 ============
 
 Install it from pip:
 
 ``pip install django-simple-stats``
 
@@ -301,14 +306,15 @@
         create_xls_resp(response)
         return response
             
 
 Changelog
 =========
 
+* v.0.6.0: Add tests!
 * v.0.5.1: Allow adding a formatter for the values
 * v.0.5.0: Add declarative API
 * v.0.4.0: Allow the aggregate function to run on a different field using ``aggr_field``
 * v.0.3.1: Fix small bug with ``choice_aggregate_with_null``
 * v.0.3.0: Add ``choice_aggregate_with_null`` and throw if stat kind is not found
 * v.0.2.1: Fix small bug with column aliases
 * v.0.2.0: Changed API; use ``query_aggregate_datetime`` for a datetime field and ``query_aggregate_date`` for a date field
```

### Comparing `django-simple-stats-0.5.1/README.rst` & `django-simple-stats-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 django-simple-stats
 -------------------
 
 A django package for creating stats from a query. 
 This package should be compatible with all 
 Django versions > 3.x
 
+
+
+.. image:: ./showme.png
+  :alt: How does it look
+
 Installation
 ============
 
 Install it from pip:
 
 ``pip install django-simple-stats``
 
@@ -280,14 +285,15 @@
         create_xls_resp(response)
         return response
             
 
 Changelog
 =========
 
+* v.0.6.0: Add tests!
 * v.0.5.1: Allow adding a formatter for the values
 * v.0.5.0: Add declarative API
 * v.0.4.0: Allow the aggregate function to run on a different field using ``aggr_field``
 * v.0.3.1: Fix small bug with ``choice_aggregate_with_null``
 * v.0.3.0: Add ``choice_aggregate_with_null`` and throw if stat kind is not found
 * v.0.2.1: Fix small bug with column aliases
 * v.0.2.0: Changed API; use ``query_aggregate_datetime`` for a datetime field and ``query_aggregate_date`` for a date field
```

### Comparing `django-simple-stats-0.5.1/django_simple_stats.egg-info/PKG-INFO` & `django-simple-stats-0.6.0/django_simple_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-stats
-Version: 0.5.1
+Version: 0.6.0
 Summary: A django package for creating simple stats from a query
 Home-page: https://github.com/spapas/django-simple-stats
 Author: Serafeim Papastefanos
 Author-email: spapas@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
@@ -25,14 +25,19 @@
 django-simple-stats
 -------------------
 
 A django package for creating stats from a query. 
 This package should be compatible with all 
 Django versions > 3.x
 
+
+
+.. image:: ./showme.png
+  :alt: How does it look
+
 Installation
 ============
 
 Install it from pip:
 
 ``pip install django-simple-stats``
 
@@ -301,14 +306,15 @@
         create_xls_resp(response)
         return response
             
 
 Changelog
 =========
 
+* v.0.6.0: Add tests!
 * v.0.5.1: Allow adding a formatter for the values
 * v.0.5.0: Add declarative API
 * v.0.4.0: Allow the aggregate function to run on a different field using ``aggr_field``
 * v.0.3.1: Fix small bug with ``choice_aggregate_with_null``
 * v.0.3.0: Add ``choice_aggregate_with_null`` and throw if stat kind is not found
 * v.0.2.1: Fix small bug with column aliases
 * v.0.2.0: Changed API; use ``query_aggregate_datetime`` for a datetime field and ``query_aggregate_date`` for a date field
```

### Comparing `django-simple-stats-0.5.1/setup.py` & `django-simple-stats-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='django-simple-stats',
-    version='0.5.1',
+    version='0.6.0',
     description="A django package for creating simple stats from a query",
     long_description=readme(),
     author='Serafeim Papastefanos',
     author_email='spapas@gmail.com',
     license='MIT',
     url='https://github.com/spapas/django-simple-stats',
     zip_safe=False,
```

### Comparing `django-simple-stats-0.5.1/simple_stats/stats.py` & `django-simple-stats-0.6.0/simple_stats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if c[0] == value:
             return c[1]
 
 
 def get_stats(qs, cfg):
     r = []
     for c in cfg:
-        method = c['method'] if 'method' in c and c['method'] else 'count'
+        method = c["method"] if "method" in c and c["method"] else "count"
         aggr_function = get_aggregate_function(method)
         field = c["field"]
         aggr_field = c.get("aggr_field") or field
         limit = c.get("limit")
         values = []
         value = None
         if c["kind"] == "query_aggregate":
@@ -70,28 +70,25 @@
                 .order_by("aggr")
             ]
 
         elif c["kind"] in ["choice_aggregate", "choice_aggregate_with_null"]:
             values = [
                 (get_choice_label(c["choices"], x[field]), x["aggr"])
                 for x in qs.values(field)
-                .annotate(
-                    aggr=aggr_function(
-                        aggr_field if c["kind"] == "choice_aggregate" else "pk"
-                    )
-                )
+                .annotate(aggr=aggr_function(aggr_field))
                 .distinct()
                 .order_by(("-aggr"))
-                if c["kind"] == "choice_aggregate_with_null" or x.get(field) != None
+                if c["kind"] == "choice_aggregate_with_null"
+                or (x.get(field) is not None and x.get(field) != "")
             ]
 
         elif c["kind"] == "query_aggregate_buckets":
             buckets = c["buckets"]
             params = {
-                ">" + str(b): aggr_function("pk", filter=Q(**{field + "__gte": b}))
+                ">=" + str(b): aggr_function("pk", filter=Q(**{field + "__gte": b}))
                 for b in buckets
             }
 
             values = [(z[0], z[1]) for z in qs.aggregate(**params).items()]
 
         elif c["kind"] == "query_aggregate_single":
             value = qs.aggregate(aggr=aggr_function(field))["aggr"]
@@ -102,15 +99,15 @@
         formatter = c.get("formatter")
         if formatter:
             values = [(x[0], formatter(x[1])) for x in values]
             if value:
                 value = formatter(value)
 
         stat = {
-            "label": c["label"] if 'label' in c and c['label'] else c['field'],
+            "label": c["label"] if "label" in c and c["label"] else c["field"],
             "values": values[:limit] if limit else values,
             "value": value,
         }
         r.append(stat)
     return r
```

