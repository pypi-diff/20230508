# Comparing `tmp/opensesame_extension_osweb-2.0.0.0a7.tar.gz` & `tmp/opensesame_extension_osweb-2.0.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_extension_osweb-2.0.0.0a7.tar", max compression
+gzip compressed data, was "opensesame_extension_osweb-2.0.0.0a8.tar", max compression
```

## Comparing `opensesame_extension_osweb-2.0.0.0a7.tar` & `opensesame_extension_osweb-2.0.0.0a8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      184 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/__init__.py
--rw-r--r--   0        0        0      309 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/__init__.py
--rw-r--r--   0        0        0      664 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/__init__.py
--rw-r--r--   0        0        0     4140 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/data.py
--rw-r--r--   0        0        0    12853 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/export.py
--rw-r--r--   0        0        0     5407 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/linter.py
--rw-r--r--   0        0        0     1588 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/jatos.css
--rw-r--r--   0        0        0     3183 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css
--rw-r--r--   0        0        0     4183 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css.map
--rw-r--r--   0        0        0   198929 2023-03-30 13:16:57.820797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css
--rw-r--r--   0        0        0   261109 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css.map
--rw-r--r--   0        0        0    28441 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css
--rw-r--r--   0        0        0    34871 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css.map
--rw-r--r--   0        0        0     1049 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/html/jatos.html
--rw-r--r--   0        0        0     1054 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/html/standalone.html
--rw-r--r--   0        0        0    12472 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/img/opensesame.png
--rw-r--r--   0        0        0      803 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/img/osdoc.png
--rw-r--r--   0        0        0      603 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/img/warning.png
--rw-r--r--   0        0        0     2791 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/_shared.js
--rw-r--r--   0        0        0     8447 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js
--rw-r--r--   0        0        0     6864 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js.map
--rw-r--r--   0        0        0     7940 2023-03-30 13:16:57.824797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/jatos.js
--rw-r--r--   0        0        0   979131 2023-03-30 13:16:57.828797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js
--rw-r--r--   0        0        0   461402 2023-03-30 13:16:57.832797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js.map
--rw-r--r--   0        0        0     4220 2023-03-30 13:16:57.832797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/standalone.js
--rw-r--r--   0        0        0   514218 2023-03-30 13:16:57.832797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js
--rw-r--r--   0        0        0   647657 2023-03-30 13:16:57.836797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js.map
--rw-r--r--   0        0        0  2886144 2023-03-30 13:16:57.852797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js
--rw-r--r--   0        0        0  3091007 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js.map
--rw-r--r--   0        0        0     1896 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb_runner.py
--rw-r--r--   0        0        0     3803 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebext.py
--rw-r--r--   0        0        0     6007 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebext.ui
--rw-r--r--   0        0        0     8215 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebext_widget.py
--rw-r--r--   0        0        0     4622 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebwriter.py
--rw-r--r--   0        0        0       76 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/__init__.py
--rw-r--r--   0        0        0      307 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_html/__init__.py
--rw-r--r--   0        0        0      709 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_html/inline_html.png
--rw-r--r--   0        0        0      436 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_html/inline_html.py
--rw-r--r--   0        0        0     1490 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_html/inline_html_large.png
--rw-r--r--   0        0        0      115 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/__init__.py
--rw-r--r--   0        0        0      795 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/inline_javascript.png
--rw-r--r--   0        0        0     5118 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/inline_javascript.py
--rw-r--r--   0        0        0     1709 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/inline_javascript_large.png
--rw-r--r--   0        0        0     1389 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/javascript_code_edit.py
--rw-r--r--   0        0        0     5166 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/javascript_workspace_api.py
--rw-r--r--   0        0        0      649 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/pyproject.toml
--rw-r--r--   0        0        0      727 2023-03-30 13:16:57.868797 opensesame_extension_osweb-2.0.0.0a7/readme.md
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 opensesame_extension_osweb-2.0.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/__init__.py
+-rw-r--r--   0        0        0      664 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/__init__.py
+-rw-r--r--   0        0        0     4140 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/data.py
+-rw-r--r--   0        0        0    12853 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/export.py
+-rw-r--r--   0        0        0     5410 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/linter.py
+-rw-r--r--   0        0        0     1588 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/jatos.css
+-rw-r--r--   0        0        0     3183 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css
+-rw-r--r--   0        0        0     4183 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css.map
+-rw-r--r--   0        0        0   198929 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css
+-rw-r--r--   0        0        0   261109 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css.map
+-rw-r--r--   0        0        0    28441 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css
+-rw-r--r--   0        0        0    34871 2023-04-09 10:34:41.553289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css.map
+-rw-r--r--   0        0        0     1049 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/html/jatos.html
+-rw-r--r--   0        0        0     1054 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/html/standalone.html
+-rw-r--r--   0        0        0    12472 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/img/opensesame.png
+-rw-r--r--   0        0        0      803 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/img/osdoc.png
+-rw-r--r--   0        0        0      603 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/img/warning.png
+-rw-r--r--   0        0        0     2791 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/_shared.js
+-rw-r--r--   0        0        0     8447 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js
+-rw-r--r--   0        0        0     6864 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js.map
+-rw-r--r--   0        0        0     7940 2023-04-09 10:34:41.557289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/jatos.js
+-rw-r--r--   0        0        0   979131 2023-04-09 10:34:41.561289 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js
+-rw-r--r--   0        0        0   461402 2023-04-09 10:34:41.565290 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js.map
+-rw-r--r--   0        0        0     4220 2023-04-09 10:34:41.565290 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/standalone.js
+-rw-r--r--   0        0        0   514218 2023-04-09 10:34:41.569290 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js
+-rw-r--r--   0        0        0   647657 2023-04-09 10:34:41.569290 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js.map
+-rw-r--r--   0        0        0  2886144 2023-04-09 10:34:41.589291 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js
+-rw-r--r--   0        0        0  3091007 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js.map
+-rw-r--r--   0        0        0     1896 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb_runner.py
+-rw-r--r--   0        0        0     3803 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebext.py
+-rw-r--r--   0        0        0     6007 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebext.ui
+-rw-r--r--   0        0        0     8215 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebext_widget.py
+-rw-r--r--   0        0        0     4622 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebwriter.py
+-rw-r--r--   0        0        0       76 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_html/__init__.py
+-rw-r--r--   0        0        0      709 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_html/inline_html.png
+-rw-r--r--   0        0        0      436 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_html/inline_html.py
+-rw-r--r--   0        0        0     1490 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_html/inline_html_large.png
+-rw-r--r--   0        0        0      130 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/__init__.py
+-rw-r--r--   0        0        0      795 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/inline_javascript.png
+-rw-r--r--   0        0        0     5118 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/inline_javascript.py
+-rw-r--r--   0        0        0     1709 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/inline_javascript_large.png
+-rw-r--r--   0        0        0     1389 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/javascript_code_edit.py
+-rw-r--r--   0        0        0     5166 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/javascript_workspace_api.py
+-rw-r--r--   0        0        0      649 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/pyproject.toml
+-rw-r--r--   0        0        0      727 2023-04-09 10:34:41.605293 opensesame_extension_osweb-2.0.0.0a8/readme.md
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 opensesame_extension_osweb-2.0.0.0a8/PKG-INFO
```

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/__init__.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/__init__.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/data.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/data.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/export.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/export.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/linter.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/linter.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 'The {} phase for item {} is called multiple times in a row'.format(
                     state,
                     item_name
                 )
             )
         states[item_name] = state
         if item.item_type == 'sequence':
-            for sub_item_name, _ in item.items:
+            for sub_item_name, _, _ in item.items:
                 set_state(sub_item_name, state)
         elif item.item_type == 'loop':
             set_state(item._item, 'prepare')
             set_state(item._item, 'run')
 
     errors = []
     states = {}
```

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/jatos.css` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/jatos.css`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/osweb.a806febd2fee54727c2c.bundle.css.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~extra.994f94ff3982825d9914.bundle.css.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/css/vendors~osweb.52753ac50071328beeda.bundle.css.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/html/jatos.html` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/html/jatos.html`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/html/standalone.html` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/html/standalone.html`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/img/opensesame.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/img/opensesame.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/img/osdoc.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/img/osdoc.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/img/warning.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/img/warning.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/_shared.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/_shared.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/extra.4d7f06d400013993e892.bundle.js.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/jatos.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/jatos.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/osweb.a806febd2fee54727c2c.bundle.js.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/standalone.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/standalone.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~extra.994f94ff3982825d9914.bundle.js.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js.map` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb/src/js/vendors~osweb.52753ac50071328beeda.bundle.js.map`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/osweb_runner.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/osweb_runner.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebext.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebext.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebext.ui` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebext.ui`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebext_widget.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebext_widget.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_extensions/osweb/oswebext/oswebwriter.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_extensions/osweb/oswebext/oswebwriter.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_html/inline_html.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_html/inline_html.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_html/inline_html_large.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_html/inline_html_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/inline_javascript.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/inline_javascript.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/inline_javascript.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/inline_javascript.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/inline_javascript_large.png` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/inline_javascript_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/javascript_code_edit.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/javascript_code_edit.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/opensesame_plugins/osweb/inline_javascript/javascript_workspace_api.py` & `opensesame_extension_osweb-2.0.0.0a8/opensesame_plugins/osweb/inline_javascript/javascript_workspace_api.py`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/pyproject.toml` & `opensesame_extension_osweb-2.0.0.0a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensesame-extension-osweb"
-version = "2.0.0.0a7"
+version = "2.0.0.0a8"
 description = "Extensions and plugins for OpenSesame to run experiments in a browser using OSWeb"
 authors = ["Sebastiaan Mathôt <s.mathot@cogsci.nl>"]
 readme = "readme.md"
 license = "COPYING"
 packages = [
     {include = "opensesame_extensions"},
     {include = "opensesame_plugins"}
```

### Comparing `opensesame_extension_osweb-2.0.0.0a7/readme.md` & `opensesame_extension_osweb-2.0.0.0a8/readme.md`

 * *Files identical despite different names*

### Comparing `opensesame_extension_osweb-2.0.0.0a7/PKG-INFO` & `opensesame_extension_osweb-2.0.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-extension-osweb
-Version: 2.0.0.0a7
+Version: 2.0.0.0a8
 Summary: Extensions and plugins for OpenSesame to run experiments in a browser using OSWeb
 Home-page: https://osdoc.cogsci.nl
 License: COPYING
 Author: Sebastiaan Mathôt
 Author-email: s.mathot@cogsci.nl
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
```

