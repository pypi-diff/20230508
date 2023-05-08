# Comparing `tmp/nextbox_ui_plugin-0.9.1.tar.gz` & `tmp/nextbox_ui_plugin-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nextbox_ui_plugin-0.9.1.tar", last modified: Fri Oct  1 13:23:36 2021, max compression
+gzip compressed data, was "dist/nextbox_ui_plugin-0.9.2.tar", last modified: Fri Oct  1 14:03:03 2021, max compression
```

## Comparing `nextbox_ui_plugin-0.9.1.tar` & `nextbox_ui_plugin-0.9.2.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1074 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/LICENSE
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      126 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/MANIFEST.in
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16622 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/PKG-INFO
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    13485 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/README.md
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      481 2021-10-01 13:20:07.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/__init__.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      212 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/admin.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/api/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)       37 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/api/__init__.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      904 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/api/serializers.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      274 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/api/urls.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      472 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/api/views.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1080 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/filters.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2281 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/forms.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/migrations/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      814 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/migrations/0001_initial.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/migrations/__init__.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      556 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/models.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      195 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/navigation.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    81084 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.bundle.min.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   155758 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.min.css
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1504 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/button_utils.js
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/img/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     8991 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/img/dead_node.png
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    89476 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery/jquery-3.5.1.min.js
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery-ui-1.12.1/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   253669 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery-ui-1.12.1/jquery-ui.min.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    14227 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_app.js
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    13120 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/LICENSE.txt
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/css/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   109158 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/css/next.css
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4507 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/api.js
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      491 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/external-small.png
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     7143 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/logo.png
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18199 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/main.css
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     5430 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/favicon.ico
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/img/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2685 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/img/spinner.gif
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/index.html
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1445 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-filter.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6568 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-list.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2924 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-search.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    10297 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/apidocs.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      482 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/yui-prettify.js
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6084 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    11358 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/COPYING
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     7912 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/README.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      675 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    17803 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/index.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25234 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Iterable.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    48619 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Object.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    35302 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Observable.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45639 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Collection.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37901 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18661 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Convex.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    43043 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Counter.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    33264 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Dictionary.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53932 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Edge.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    59726 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSet.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   119401 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18999 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Force.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    63973 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    36330 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16431 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16439 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    20336 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    55235 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    35562 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableObject.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45256 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Query.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    49392 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.SortedMap.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    62409 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Vertex.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    71085 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.VertexSet.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19005 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    32582 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Line.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16363 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Math.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16367 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Matrix.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    35270 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Vector.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82638 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78093 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Circle.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    75391 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Component.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    39045 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.DragManager.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78090 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Group.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    79964 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icon.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25185 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icons.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78997 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Image.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78087 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Line.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47423 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47417 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47451 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78087 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Path.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    79031 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Polygon.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78087 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Rect.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    64159 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Stage.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78993 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Text.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    96941 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   104702 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    17814 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82659 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    21210 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37494 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    65840 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37371 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    81928 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    95877 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    86763 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    23428 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   123134 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45654 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   131521 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    93323 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   129258 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    38474 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   135707 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    96743 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    85369 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    91173 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82662 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82658 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37180 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    23767 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    38916 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37480 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    43075 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    66091 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    58522 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18810 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16446 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19201 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37528 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   217923 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78089 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Triangle.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    42047 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45721 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    48292 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Application.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47377 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Component.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    29569 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssClass.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    29569 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssStyle.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53483 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    64459 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popover.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    62226 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popup.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16384 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    33822 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Env.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    30512 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Util.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53166 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    66752 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16830 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16733 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16811 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16396 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   488048 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/data.json
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/files/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/files/index.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16629 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/index.html
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/index.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    20154 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.data.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16998 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.geometry.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    24856 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.Topology.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19379 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16910 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19782 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.ui.html
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53944 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansExtraLight.otf
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    52108 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansRegular.otf
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    44036 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.eot
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    50305 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.svg
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    43832 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    23556 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.woff
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    44332 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.eot
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    48996 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.svg
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    44140 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.ttf
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    24084 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.woff
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    26072 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.eot
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   101322 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.svg
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25900 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.ttf
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25976 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.woff
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/js/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)   554834 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/js/next.js
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      757 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/template_content.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      967 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1007 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4607 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     3754 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6062 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     7737 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      222 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/urls.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19778 2021-10-01 13:18:12.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/views.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16622 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/PKG-INFO
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    14933 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)        1 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)       18 2021-10-01 13:23:35.000000 nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/top_level.txt
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)       38 2021-10-01 13:23:36.000000 nextbox_ui_plugin-0.9.1/setup.cfg
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1118 2021-10-01 13:19:57.000000 nextbox_ui_plugin-0.9.1/setup.py
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1074 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/LICENSE
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      126 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/MANIFEST.in
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16622 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/PKG-INFO
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    13485 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/README.md
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      481 2021-10-01 14:02:13.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/__init__.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      212 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/admin.py
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/api/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)       37 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/api/__init__.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      904 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/api/serializers.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      274 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/api/urls.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      472 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/api/views.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1080 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/filters.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2281 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/forms.py
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/migrations/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      814 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/migrations/0001_initial.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/migrations/__init__.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      556 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/models.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      195 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/navigation.py
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    81084 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.bundle.min.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   155758 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.min.css
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1504 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/button_utils.js
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/img/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     8991 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/img/dead_node.png
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    89476 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery/jquery-3.5.1.min.js
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery-ui-1.12.1/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   253669 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery-ui-1.12.1/jquery-ui.min.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    14227 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_app.js
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    13120 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/LICENSE.txt
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/css/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   109158 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/css/next.css
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4507 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/api.js
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      491 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/external-small.png
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     7143 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/logo.png
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18199 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/main.css
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     5430 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/favicon.ico
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/img/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2685 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/img/spinner.gif
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/index.html
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1445 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-filter.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6568 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-list.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2924 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-search.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    10297 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/apidocs.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      482 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/yui-prettify.js
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6084 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    11358 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/COPYING
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     7912 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/README.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      675 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    17803 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/index.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25234 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Iterable.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    48619 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Object.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    35302 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Observable.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45639 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Collection.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37901 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18661 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Convex.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    43043 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Counter.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    33264 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Dictionary.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53932 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Edge.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    59726 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSet.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   119401 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18999 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Force.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    63973 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    36330 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16431 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16439 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    20336 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    55235 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    35562 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableObject.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45256 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Query.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    49392 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.SortedMap.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    62409 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Vertex.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    71085 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.VertexSet.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19005 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    32582 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Line.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16363 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Math.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16367 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Matrix.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    35270 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Vector.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82638 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78093 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Circle.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    75391 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Component.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    39045 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.DragManager.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78090 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Group.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    79964 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icon.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25185 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icons.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78997 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Image.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78087 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Line.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47423 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47417 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47451 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78087 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Path.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    79031 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Polygon.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78087 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Rect.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    64159 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Stage.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78993 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Text.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    96941 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   104702 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    17814 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82659 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    21210 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37494 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    65840 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37371 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    81928 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    95877 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    86763 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    23428 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   123134 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45654 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   131521 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    93323 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   129258 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    38474 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   135707 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    96743 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    85369 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    91173 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82662 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    82658 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37180 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    23767 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    38916 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37480 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    43075 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    66091 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    58522 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    18810 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16446 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19201 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    37528 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   217923 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    78089 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Triangle.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    42047 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    45721 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    48292 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Application.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    47377 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Component.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    29569 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssClass.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    29569 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssStyle.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53483 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    64459 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popover.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    62226 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popup.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16384 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    33822 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Env.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    30512 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Util.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53166 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    66752 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16830 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16733 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16811 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16396 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   488048 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/data.json
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/files/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/files/index.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16629 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/index.html
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      216 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/index.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    20154 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.data.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16998 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.geometry.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    24856 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.Topology.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19379 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16910 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19782 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.ui.html
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    53944 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansExtraLight.otf
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    52108 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansRegular.otf
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    44036 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.eot
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    50305 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.svg
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    43832 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    23556 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.woff
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    44332 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.eot
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    48996 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.svg
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    44140 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.ttf
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    24084 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.woff
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    26072 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.eot
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   101322 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.svg
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25900 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.ttf
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    25976 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.woff
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/js/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)   554834 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/js/next.js
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      757 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/template_content.py
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      967 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1007 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button_3.x.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4607 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     3754 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology_3.x.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6062 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     7737 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology_3.x.html
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)      222 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/urls.py
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    19775 2021-10-01 14:00:45.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/views.py
+drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    16622 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)    14933 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)        1 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)       18 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/top_level.txt
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)       38 2021-10-01 14:03:03.000000 nextbox_ui_plugin-0.9.2/setup.cfg
+-rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1118 2021-10-01 14:02:15.000000 nextbox_ui_plugin-0.9.2/setup.py
```

### Comparing `nextbox_ui_plugin-0.9.1/LICENSE` & `nextbox_ui_plugin-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/PKG-INFO` & `nextbox_ui_plugin-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nextbox_ui_plugin
-Version: 0.9.1
+Version: 0.9.2
 Summary: A topology visualization plugin for Netbox powered by NextUI Toolkit.
 Home-page: https://github.com/iDebugAll/nextbox-ui-plugin
 Author: Igor Korotchenkov
 Author-email: iDebugAll@gmail.com
 License: MIT
-Download-URL: https://github.com/iDebugAll/nextbox-ui-plugin/archive/v0.9.1.tar.gz
+Download-URL: https://github.com/iDebugAll/nextbox-ui-plugin/archive/v0.9.2.tar.gz
 Description: # NextBox UI Plugin
         
         A topology visualization plugin for [NetBox](https://github.com/netbox-community/netbox) powered by [NextUI](https://developer.cisco.com/site/neXt/) Toolkit. Netbox v2.8.0+ is required.
         
         # Installation
         
         General installation steps and considerations follow the [official guidelines](https://netbox.readthedocs.io/en/stable/plugins/).
```

### Comparing `nextbox_ui_plugin-0.9.1/README.md` & `nextbox_ui_plugin-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/api/serializers.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/filters.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/filters.py`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/forms.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/migrations/0001_initial.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/models.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/models.py`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.bundle.min.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.min.css` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/button_utils.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/button_utils.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/img/dead_node.png` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/img/dead_node.png`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery/jquery-3.5.1.min.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery-ui-1.12.1/jquery-ui.min.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/jquery-ui-1.12.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_app.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_app.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/LICENSE.txt` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/css/next.css` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/css/next.css`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/api.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/api.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/logo.png` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/logo.png`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/main.css` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/favicon.ico` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/img/spinner.gif` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/img/spinner.gif`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-filter.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-filter.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-list.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-list.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-search.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/api-search.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/apidocs.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/js/apidocs.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/COPYING` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/COPYING`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/README.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/README.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Iterable.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Iterable.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Object.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Object.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Observable.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.Observable.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Collection.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Collection.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Convex.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Convex.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Counter.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Counter.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Dictionary.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Dictionary.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Edge.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Edge.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSet.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSet.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Force.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Force.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableObject.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.ObservableObject.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Query.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Query.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.SortedMap.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.SortedMap.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Vertex.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.Vertex.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.VertexSet.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.data.VertexSet.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Line.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Line.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Math.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Math.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Matrix.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Matrix.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Vector.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.geometry.Vector.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Circle.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Circle.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Component.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Component.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.DragManager.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.DragManager.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Group.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Group.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icon.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icon.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icons.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Icons.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Image.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Image.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Line.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Line.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Path.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Path.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Polygon.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Polygon.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Rect.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Rect.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Stage.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Stage.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Text.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Text.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Topology.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Triangle.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.graphic.Triangle.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Application.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Application.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Component.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Component.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssClass.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssClass.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssStyle.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.CssStyle.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popover.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popover.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popup.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.Popup.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Env.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Env.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Util.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.Util.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/data.json` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/data.json`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/index.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/index.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.data.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.data.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.geometry.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.geometry.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.Topology.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.Topology.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.graphic.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.ui.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/doc/modules/nx.ui.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansExtraLight.otf` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansExtraLight.otf`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansRegular.otf` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/CiscoSansRegular.otf`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.eot` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.svg` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.woff` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansextralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.eot` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.eot`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.svg` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.svg`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.ttf` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.woff` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/ciscosansregular-webfont.woff`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.eot` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.eot`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.svg` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.svg`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.ttf` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.ttf`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.woff` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/fonts/next-font.woff`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/js/next.js` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/static/nextbox_ui_plugin/next_sources/js/next.js`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/template_content.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button_3.x.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topo_button_3.x.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology_3.x.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/site_topology_3.x.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology_3.x.html` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/templates/nextbox_ui_plugin/topology_3.x.html`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin/views.py` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
 def get_vlan_topology(nb_devices_qs, vlans):
 
     topology_dict = {'nodes': [], 'links': []}
     device_roles = set()
     all_device_tags = set()
     multi_cable_connections = []
-    vlan = VLAN.objects.get(id=vlans[0])
+    vlan = VLAN.objects.get(id=vlans)
     interfaces = vlan.get_interfaces()
     filtred_devices = [d.id for d in nb_devices_qs]
     filtred_interfaces = []
     for interface in interfaces:
         if interface.is_connectable:
             direct_device_id = interface.device.id
             interface_trace = interface.trace()
```

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/PKG-INFO` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nextbox-ui-plugin
-Version: 0.9.1
+Version: 0.9.2
 Summary: A topology visualization plugin for Netbox powered by NextUI Toolkit.
 Home-page: https://github.com/iDebugAll/nextbox-ui-plugin
 Author: Igor Korotchenkov
 Author-email: iDebugAll@gmail.com
 License: MIT
-Download-URL: https://github.com/iDebugAll/nextbox-ui-plugin/archive/v0.9.1.tar.gz
+Download-URL: https://github.com/iDebugAll/nextbox-ui-plugin/archive/v0.9.2.tar.gz
 Description: # NextBox UI Plugin
         
         A topology visualization plugin for [NetBox](https://github.com/netbox-community/netbox) powered by [NextUI](https://developer.cisco.com/site/neXt/) Toolkit. Netbox v2.8.0+ is required.
         
         # Installation
         
         General installation steps and considerations follow the [official guidelines](https://netbox.readthedocs.io/en/stable/plugins/).
```

### Comparing `nextbox_ui_plugin-0.9.1/nextbox_ui_plugin.egg-info/SOURCES.txt` & `nextbox_ui_plugin-0.9.2/nextbox_ui_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextbox_ui_plugin-0.9.1/setup.py` & `nextbox_ui_plugin-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from os import path
 top_level_directory = path.abspath(path.dirname(__file__))
 with open(path.join(top_level_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='nextbox_ui_plugin',
-    version='0.9.1',
+    version='0.9.2',
     url='https://github.com/iDebugAll/nextbox-ui-plugin',
-    download_url='https://github.com/iDebugAll/nextbox-ui-plugin/archive/v0.9.1.tar.gz',
+    download_url='https://github.com/iDebugAll/nextbox-ui-plugin/archive/v0.9.2.tar.gz',
     description='A topology visualization plugin for Netbox powered by NextUI Toolkit.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Igor Korotchenkov',
     author_email='iDebugAll@gmail.com',
     install_requires=[],
     packages=find_packages(),
```

