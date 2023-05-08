# Comparing `tmp/knic_jupyter-0.1.1.tar.gz` & `tmp/knic_jupyter-0.1.2.tar.gz`

## Comparing `knic_jupyter-0.1.1.tar` & `knic_jupyter-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/.eslintrc.js
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/Dockerfile
--rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/GEO-R-6a.ipynb
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/babel.config.js
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/docker-compose.yaml
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/environment.yaml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/install.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/jest.config.js
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/package.json
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/requirements.txt
--rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/run-jupyter-lab.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/setup.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   388358 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/yarn.lock
--rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/build_log.json
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/package.json
--rw-r--r--   0        0        0    20043 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js.map
--rw-r--r--   0        0        0    29216 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js
--rw-r--r--   0        0        0    27936 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js.map
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/style.js
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map
--rw-r--r--   0        0        0   135674 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js
--rw-r--r--   0        0        0   117914 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map
--rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map
--rw-r--r--   0        0        0   195842 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js
--rw-r--r--   0        0        0   230605 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/src/index.ts
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/src/__tests__/KNICS_Jupyter_frontend.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/ui-tests/tests/KNICS_Jupyter_frontend.spec.ts
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/LICENSE
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/README.md
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 knic_jupyter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/.eslintrc.js
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/Dockerfile
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/GEO-R-6a.ipynb
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/babel.config.js
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/docker-compose.yaml
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/environment.yaml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/install.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/jest.config.js
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/package.json
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/requirements.txt
+-rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/run-jupyter-lab.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/setup.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   388358 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/yarn.lock
+-rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/build_log.json
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/package.json
+-rw-r--r--   0        0        0    20043 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js.map
+-rw-r--r--   0        0        0    29216 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js
+-rw-r--r--   0        0        0    27936 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js.map
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/style.js
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map
+-rw-r--r--   0        0        0   135674 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js
+-rw-r--r--   0        0        0   117914 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map
+-rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map
+-rw-r--r--   0        0        0   195842 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js
+-rw-r--r--   0        0        0   230605 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/src/index.ts
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/src/__tests__/KNICS_Jupyter_frontend.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/ui-tests/tests/KNICS_Jupyter_frontend.spec.ts
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/LICENSE
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/README.md
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 knic_jupyter-0.1.2/PKG-INFO
```

### Comparing `knic_jupyter-0.1.1/.eslintrc.js` & `knic_jupyter-0.1.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/GEO-R-6a.ipynb` & `knic_jupyter-0.1.2/GEO-R-6a.ipynb`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/RELEASE.md` & `knic_jupyter-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/environment.yaml` & `knic_jupyter-0.1.2/environment.yaml`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/jest.config.js` & `knic_jupyter-0.1.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/package.json` & `knic_jupyter-0.1.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -97,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `knic_jupyter-0.1.1/requirements.txt` & `knic_jupyter-0.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/tsconfig.json` & `knic_jupyter-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/yarn.lock` & `knic_jupyter-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/build_log.json` & `knic_jupyter-0.1.2/knic-jupyter/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/package.json` & `knic_jupyter-0.1.2/knic-jupyter/labextension/package.json`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js.map` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/lib_index_js.c863638f90a4e592ca27.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js.map` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/remoteEntry.a98285ffa48595c28920.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map` & `knic_jupyter-0.1.2/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/src/index.ts` & `knic_jupyter-0.1.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/ui-tests/README.md` & `knic_jupyter-0.1.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/ui-tests/jupyter_server_test_config.py` & `knic_jupyter-0.1.2/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/.gitignore` & `knic_jupyter-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.1/pyproject.toml` & `knic_jupyter-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,32 +2,41 @@
 requires = ["hatchling>=1.3.1", "jupyterlab>=3.4.7,<4.0.0", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "knic-jupyter"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8.15"
 classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.8",
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 3",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
-    "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
 ]
+
+dynamic = ["version", "description", "authors", "urls", "keywords"]
+
 dependencies = [
+  "jupyter_client == 7.4.9",
+  "jupyter_core == 5.1.5",
+  "jupyter-events == 0.6.3",
+  "jupyter_server == 2.1.0",
+  "jupyter_server_terminals == 0.4.4",
+  "jupyterlab == 3.5.3",
+  "jupyterlab-pygments == 0.2.2",
+  "jupyterlab_server == 2.19.0",
 ]
-dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
```

### Comparing `knic_jupyter-0.1.1/PKG-INFO` & `knic_jupyter-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: knic-jupyter
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/usc-isi-i2/knic-jupyter
 Project-URL: Bug Tracker, https://github.com/usc-isi-i2/knic-jupyter/issues
 Project-URL: Repository, https://github.com/usc-isi-i2/knic-jupyter.git
-License: BSD 3-Clause License
+License: MIT License
         
-        Copyright (c) 2022, Daniel Auerbach
-        All rights reserved.
+        Copyright (c) 2017 University of Southern California
         
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.15
+Requires-Dist: jupyter-client==7.4.9
+Requires-Dist: jupyter-core==5.1.5
+Requires-Dist: jupyter-events==0.6.3
+Requires-Dist: jupyter-server-terminals==0.4.4
+Requires-Dist: jupyter-server==2.1.0
+Requires-Dist: jupyterlab-pygments==0.2.2
+Requires-Dist: jupyterlab-server==2.19.0
+Requires-Dist: jupyterlab==3.5.3
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-tornasync; extra == 'test'
 Description-Content-Type: text/markdown
```

