# Comparing `tmp/duckdbt-0.1.0.tar.gz` & `tmp/duckdbt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdbt-0.1.0.tar", last modified: Sat Jan 14 05:05:14 2023, max compression
+gzip compressed data, was "duckdbt-0.3.0.tar", last modified: Mon May  8 20:57:45 2023, max compression
```

## Comparing `duckdbt-0.1.0.tar` & `duckdbt-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-14 05:05:14.743397 duckdbt-0.1.0/
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.1.0/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-01-14 05:05:14.743277 duckdbt-0.1.0/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 05:05:08.000000 duckdbt-0.1.0/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-14 05:05:14.741822 duckdbt-0.1.0/duckdbt/
--rw-r--r--   0 jwills     (501) staff       (20)     1997 2023-01-14 04:58:00.000000 duckdbt-0.1.0/duckdbt/api.py
--rw-r--r--   0 jwills     (501) staff       (20)     4471 2023-01-14 05:01:51.000000 duckdbt-0.1.0/duckdbt/server.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-14 05:05:14.742875 duckdbt-0.1.0/duckdbt/static/
--rw-r--r--   0 jwills     (501) staff       (20)     1246 2023-01-14 04:58:00.000000 duckdbt-0.1.0/duckdbt/static/dashboard.css
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-14 05:05:14.743092 duckdbt-0.1.0/duckdbt/templates/
--rw-r--r--   0 jwills     (501) staff       (20)     4951 2023-01-14 04:58:00.000000 duckdbt-0.1.0/duckdbt/templates/index.html
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-14 05:05:14.742768 duckdbt-0.1.0/duckdbt.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-01-14 05:05:14.000000 duckdbt-0.1.0/duckdbt.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      275 2023-01-14 05:05:14.000000 duckdbt-0.1.0/duckdbt.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-01-14 05:05:14.000000 duckdbt-0.1.0/duckdbt.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       93 2023-01-14 05:05:14.000000 duckdbt-0.1.0/duckdbt.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        8 2023-01-14 05:05:14.000000 duckdbt-0.1.0/duckdbt.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-01-14 05:05:14.743429 duckdbt-0.1.0/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)      978 2023-01-14 04:59:32.000000 duckdbt-0.1.0/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.846511 duckdbt-0.3.0/
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.3.0/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-08 20:57:45.846402 duckdbt-0.3.0/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.3.0/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.845054 duckdbt-0.3.0/duckdbt/
+-rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/api.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/extensions.py
+-rw-r--r--   0 jwills     (501) staff       (20)      696 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/ipython.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1388 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/load_db_profile.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1884 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/server.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.846078 duckdbt-0.3.0/duckdbt/static/
+-rw-r--r--   0 jwills     (501) staff       (20)     1246 2023-01-14 04:58:00.000000 duckdbt-0.3.0/duckdbt/static/dashboard.css
+-rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/static/favicon.ico
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.846219 duckdbt-0.3.0/duckdbt/templates/
+-rw-r--r--   0 jwills     (501) staff       (20)     5332 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/templates/index.html
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.845726 duckdbt-0.3.0/duckdbt.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      370 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       79 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        8 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-08 20:57:45.846544 duckdbt-0.3.0/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)      954 2023-05-08 20:17:37.000000 duckdbt-0.3.0/setup.py
```

### Comparing `duckdbt-0.1.0/duckdbt/static/dashboard.css` & `duckdbt-0.3.0/duckdbt/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `duckdbt-0.1.0/duckdbt/templates/index.html` & `duckdbt-0.3.0/duckdbt/templates/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,37 @@
   <head>
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
     <link href="https://cdn.jsdelivr.net/npm/codemirror@5.57.0/lib/codemirror.css" rel="stylesheet">
     <link href="/static/dashboard.css">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
     <script src="https://cdn.jsdelivr.net/npm/codemirror@5.57.0/lib/codemirror.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/codemirror@5.57.0/mode/sql/sql.js"></script>
+
+    <!-- thank you GPT-4 -->
+    <style>
+      .relation-item {
+        white-space: nowrap;
+        overflow: hidden;
+        text-overflow: ellipsis;
+      }
+
+      .relation-link {
+        display: block;
+        max-width: 100%;
+      }
+
+      .relation-link:hover {
+        text-decoration: none;
+      }
+
+      .relation-column {
+        padding-left: 1.5rem;
+      }
+    </style>
+
   </head>
 
   <body>
     <header class="navbar navbar-dark sticky-top bg-dark flex-md-nowrap p-0 shadow">
       <a class="navbar-brand col-md-3 col-lg-2 me-0 px-3 fs-6" href="#">DuckDBT</a>
     </header>
     
@@ -87,39 +110,39 @@
 
       const form = document.getElementById('query-form');
       const resultTable = document.getElementById('result-table');
       const queryError = document.getElementById("query-error");
 
       form.addEventListener('submit', async (event) => {
         event.preventDefault();
-        const response = await fetch('/api/query', {
+        const response = await fetch('/v1/statement', {
             headers: {
                 'Accept': 'application/json',
                 'Content-Type': 'application/json'
             },
             method: 'POST',
-            body: JSON.stringify({"sql": queryEditor.getValue()})
+            body: queryEditor.getValue()
         });
         if (response.status != 200) {
           queryError.hidden = false;
           queryError.innerText = (await response.json())["detail"];
           resultTable.innerHTML = "";
         } else {
-          const data = await response.json();
+          const payload = await response.json();
 
           // update the table with the new data
           queryError.hidden = true;
           queryError.innerText = "";
 
           resultTable.innerHTML = `
           <thead>
-              ${data.columns.map((column) => `<th scope="col">${column}</th>`).join('')}
+              ${payload.columns.map((column) => `<th scope="col">${column.name}</th>`).join('')}
           </thead>
           <tbody>
-          ${data.rows.map((row) => `
+          ${payload.data.map((row) => `
             <tr>
               ${row.map((cell) => `<td>${cell}</td>`).join('')}
             </tr>
           `).join('')}
           </tbody>
           `;
         }
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
 
+
  DuckDBT
 * Tables *
     * {% for relation, columns in relations.items() %}
     * {{_relation_}}
           o_{%_for_column_in_columns_%}
           o_{{_column_}}
           o_{%_endfor_%}
```

### Comparing `duckdbt-0.1.0/setup.py` & `duckdbt-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python
 import os
-import re
 
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "duckdbt"
 
 
-package_version = "0.1.0"
+package_version = "0.3.0"
 description = """The Modern Data Stack in a Python Package"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+duckdbt@gmail.com",
     url="https://github.com/jwills/duckdbt",
     packages=find_namespace_packages(include=["duckdbt", "duckdbt.*"]),
     include_package_data=True,
     install_requires=[
-        "buenavista~=0.1.0",
-        "dbt-buenavista~=1.3.0",
-        "dbt-duckdb~=1.3.0",
-        "duckdb~=0.6.0",
+        "buenavista~=0.2.1",
+        "dbt-duckdb~=1.5.0",
+        "duckdb~=0.7.0",
         "fastapi[all]",
         "pyarrow",
+        "sqlglot",
     ],
 )
```

