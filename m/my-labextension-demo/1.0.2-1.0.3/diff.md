# Comparing `tmp/my_labextension_demo-1.0.2.tar.gz` & `tmp/my_labextension_demo-1.0.3.tar.gz`

## Comparing `my_labextension_demo-1.0.2.tar` & `my_labextension_demo-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/babel.config.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/jest.config.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/tsconfig.json
--rw-r--r--   0        0        0   382637 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/yarn.lock
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/_version.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/plugin.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/package.json
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/schemas/my-labextension-demo/package.json.orig
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/schemas/my-labextension-demo/plugin.json
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/568.b6a88c5b3cd181be9505.js
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/747.1b8fd0ee47d900ebc630.js
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/remoteEntry.b9f6bdf6f8cc6d6bccc5.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/schema/plugin.json
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/src/index.ts
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/src/__tests__/my_labextension_demo.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/ui-tests/tests/my_labextension_demo.spec.ts
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/LICENSE
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/README.md
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/babel.config.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/jest.config.js
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/tsconfig.json
+-rw-r--r--   0        0        0   382637 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/yarn.lock
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/_version.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/package.json
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/schemas/my-labextension-demo/package.json.orig
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/schemas/my-labextension-demo/plugin.json
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/568.b6a88c5b3cd181be9505.js
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/747.1b8fd0ee47d900ebc630.js
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/remoteEntry.ff39d0d51412ea6b92f9.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/schema/plugin.json
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/src/index.ts
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/src/__tests__/my_labextension_demo.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   125817 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/ui-tests/tests/my_labextension_demo.spec.ts
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/README.md
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 my_labextension_demo-1.0.3/PKG-INFO
```

### Comparing `my_labextension_demo-1.0.2/RELEASE.md` & `my_labextension_demo-1.0.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/jest.config.js` & `my_labextension_demo-1.0.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/package.json` & `my_labextension_demo-1.0.3/my_labextension_demo/labextension/schemas/my-labextension-demo/package.json.orig`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/tsconfig.json` & `my_labextension_demo-1.0.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/yarn.lock` & `my_labextension_demo-1.0.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/my_labextension_demo/labextension/package.json` & `my_labextension_demo-1.0.3/my_labextension_demo/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9746527777777777%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ff39d0d51412ea6b92f9.js'}, 'discovery': "*

 * *                 "OrderedDict([('server', OrderedDict([('base', OrderedDict([('name', "*

 * *                 "'my_labextension_demo')])), ('managers', ['pip', 'conda'])]))])}",*

 * * "'version'": "'1.0.2'"}*

```diff
@@ -102,17 +102,28 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/my-labextension-demo",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b9f6bdf6f8cc6d6bccc5.js",
+            "load": "static/remoteEntry.ff39d0d51412ea6b92f9.js",
             "style": "./style"
         },
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "my_labextension_demo"
+                },
+                "managers": [
+                    "pip",
+                    "conda"
+                ]
+            }
+        },
         "extension": true,
         "outputDir": "my_labextension_demo/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -176,9 +187,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "1.0.2"
 }
```

### Comparing `my_labextension_demo-1.0.2/my_labextension_demo/labextension/schemas/my-labextension-demo/package.json.orig` & `my_labextension_demo-1.0.3/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9739583333333334%*

 * *Differences: {"'jupyterlab'": "{'discovery': OrderedDict([('server', OrderedDict([('base', "*

 * *                 "OrderedDict([('name', 'my_labextension_demo')])), ('managers', ['pip'])]))])}",*

 * * "'version'": "'1.0.3'"}*

```diff
@@ -100,14 +100,24 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/my-labextension-demo",
     "jupyterlab": {
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "my_labextension_demo"
+                },
+                "managers": [
+                    "pip"
+                ]
+            }
+        },
         "extension": true,
         "outputDir": "my_labextension_demo/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -171,9 +181,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "1.0.3"
 }
```

### Comparing `my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/568.b6a88c5b3cd181be9505.js` & `my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/568.b6a88c5b3cd181be9505.js`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/747.1b8fd0ee47d900ebc630.js` & `my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/747.1b8fd0ee47d900ebc630.js`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/remoteEntry.b9f6bdf6f8cc6d6bccc5.js` & `my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/remoteEntry.ff39d0d51412ea6b92f9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => g.e(568).then((() => () => g(568))),
                         from: i,
                         eager: !1
                     })
-                })("my-labextension-demo", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("my-labextension-demo", "1.0.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `my_labextension_demo-1.0.2/my_labextension_demo/labextension/static/third-party-licenses.json` & `my_labextension_demo-1.0.3/my_labextension_demo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/src/index.ts` & `my_labextension_demo-1.0.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/ui-tests/README.md` & `my_labextension_demo-1.0.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/ui-tests/jupyter_server_test_config.py` & `my_labextension_demo-1.0.3/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/ui-tests/tests/my_labextension_demo.spec.ts` & `my_labextension_demo-1.0.3/ui-tests/tests/my_labextension_demo.spec.ts`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/.gitignore` & `my_labextension_demo-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/LICENSE` & `my_labextension_demo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/README.md` & `my_labextension_demo-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/pyproject.toml` & `my_labextension_demo-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `my_labextension_demo-1.0.2/PKG-INFO` & `my_labextension_demo-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_labextension_demo
-Version: 1.0.2
+Version: 1.0.3
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/my-labextension-demo
 Project-URL: Bug Tracker, https://github.com/github_username/my-labextension-demo/issues
 Project-URL: Repository, https://github.com/github_username/my-labextension-demo.git
 Author-email: Tai Lai <ctlai95@gmail.com>
 License: BSD 3-Clause License
```

