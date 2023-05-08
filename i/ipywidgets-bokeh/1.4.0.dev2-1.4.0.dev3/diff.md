# Comparing `tmp/ipywidgets_bokeh-1.4.0.dev2.tar.gz` & `tmp/ipywidgets_bokeh-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_bokeh-1.4.0.dev2.tar", last modified: Thu Apr 27 16:58:09 2023, max compression
+gzip compressed data, was "ipywidgets_bokeh-1.4.0.dev3.tar", last modified: Sun Apr 30 09:50:22 2023, max compression
```

## Comparing `ipywidgets_bokeh-1.4.0.dev2.tar` & `ipywidgets_bokeh-1.4.0.dev3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1494 2020-01-09 14:03:17.000000 ipywidgets_bokeh-1.4.0.dev2/LICENSE.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      184 2021-10-05 19:15:23.000000 ipywidgets_bokeh-1.4.0.dev2/MANIFEST.in
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      511 2020-07-10 18:26:09.000000 ipywidgets_bokeh-1.4.0.dev2/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.757953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       58 2023-04-27 14:59:03.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        3 2019-12-19 13:15:23.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/bokeh.ext.json
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.757953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)   432832 2023-04-27 16:58:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3529 2023-04-27 16:58:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)  3042125 2023-04-27 16:58:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/ipywidgets_bokeh.js
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       55 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/index.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      591 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/index.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      103 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/loader.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1668 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/loader.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1290 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     7924 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       48 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/webpack.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      292 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/webpack.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1192 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3971 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4480 2023-04-27 14:59:06.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/kernel.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1222 2023-04-27 14:59:16.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/package.json
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1243 2023-03-29 21:38:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/widget.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.757953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      900 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       51 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      106 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1880 2023-04-27 16:56:09.000000 ipywidgets_bokeh-1.4.0.dev2/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.175346 ipywidgets_bokeh-1.4.0.dev3/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1494 2020-01-09 14:03:17.000000 ipywidgets_bokeh-1.4.0.dev3/LICENSE.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      184 2021-10-05 19:15:23.000000 ipywidgets_bokeh-1.4.0.dev3/MANIFEST.in
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-30 09:50:22.175346 ipywidgets_bokeh-1.4.0.dev3/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      511 2020-07-10 18:26:09.000000 ipywidgets_bokeh-1.4.0.dev3/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.155346 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       58 2023-04-30 09:47:45.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        3 2019-12-19 13:15:23.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/bokeh.ext.json
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.159345 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)   432832 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3529 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)  3042068 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/ipywidgets_bokeh.js
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.175346 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       55 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/index.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      591 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/index.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      103 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/loader.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1668 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/loader.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1290 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     7924 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       48 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/webpack.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      292 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/webpack.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1221 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4034 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4480 2023-04-30 09:47:48.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/kernel.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1222 2023-04-30 09:47:55.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/package.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1243 2023-03-29 21:38:08.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/widget.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.159345 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      900 2023-04-30 09:50:22.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       51 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      106 2023-04-30 09:50:22.179345 ipywidgets_bokeh-1.4.0.dev3/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1880 2023-04-30 09:47:57.000000 ipywidgets_bokeh-1.4.0.dev3/setup.py
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/LICENSE.txt` & `ipywidgets_bokeh-1.4.0.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/PKG-INFO` & `ipywidgets_bokeh-1.4.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets_bokeh
-Version: 1.4.0.dev2
+Version: 1.4.0.dev3
 Summary: Allows embedding of Jupyter widgets in Bokeh layouts.
 Home-page: https://github.com/bokeh/ipywidgets_bokeh
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/ipywidgets_bokeh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -61702,42 +61702,35 @@
                     }
                 }
             },
             63840: (e, t, n) => {
                 "use strict";
                 e.exports = n(60053)
             },
-            20019: (e, t, n) => {
+            54993: (e, t, n) => {
                 "use strict";
                 n.r(t), n.d(t, {
-                    default: () => g
+                    default: () => v
                 });
                 var r = n(93379),
                     i = n.n(r),
                     o = n(7795),
                     a = n.n(o),
-                    s = n(3565),
+                    s = n(90569),
                     l = n.n(s),
-                    c = n(19216),
+                    c = n(3565),
                     u = n.n(c),
-                    d = n(98262),
-                    h = {};
-                d.Z && d.Z.locals && (h.locals = d.Z.locals);
-                var f, p = 0,
-                    m = {
-                        styleTagTransform: (e, t, n) => {
-                            n.handler(e)
-                        }
-                    };
-                m.setAttributes = l(), m.insert = (e, t) => {}, m.domAPI = a(), m.insertStyleElement = u(), h.use = function(e) {
-                    return m.options = e || {}, p++ || (f = i()(d.Z, m)), h
-                }, h.unuse = function() {
-                    p > 0 && !--p && (f(), f = null)
-                };
-                const g = h
+                    d = n(19216),
+                    h = n.n(d),
+                    f = n(44589),
+                    p = n.n(f),
+                    m = n(98262),
+                    g = {};
+                g.styleTagTransform = p(), g.setAttributes = u(), g.insert = l().bind(null, "head"), g.domAPI = a(), g.insertStyleElement = h(), i()(m.Z, g);
+                const v = m.Z && m.Z.locals ? m.Z.locals : void 0
             },
             93379: e => {
                 "use strict";
                 var t = [];
 
                 function n(e) {
                     for (var n = -1, r = 0; r < t.length; r++)
@@ -61798,14 +61791,34 @@
                             var u = n(o[c]);
                             0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                         }
                         o = l
                     }
                 }
             },
+            90569: e => {
+                "use strict";
+                var t = {};
+                e.exports = function(e, n) {
+                    var r = function(e) {
+                        if (void 0 === t[e]) {
+                            var n = document.querySelector(e);
+                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                                n = n.contentDocument.head
+                            } catch (e) {
+                                n = null
+                            }
+                            t[e] = n
+                        }
+                        return t[e]
+                    }(e);
+                    if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    r.appendChild(n)
+                }
+            },
             19216: e => {
                 "use strict";
                 e.exports = function(e) {
                     var t = document.createElement("style");
                     return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
                 }
             },
@@ -61840,14 +61853,24 @@
                                 if (null === e.parentNode) return !1;
                                 e.parentNode.removeChild(e)
                             }(t)
                         }
                     }
                 }
             },
+            44589: e => {
+                "use strict";
+                e.exports = function(e, t) {
+                    if (t.styleSheet) t.styleSheet.cssText = e;
+                    else {
+                        for (; t.firstChild;) t.removeChild(t.firstChild);
+                        t.appendChild(document.createTextNode(e))
+                    }
+                }
+            },
             70655: (e, t, n) => {
                 "use strict";
                 n.r(t), n.d(t, {
                     __assign: () => o,
                     __asyncDelegator: () => M,
                     __asyncGenerator: () => b,
                     __asyncValues: () => w,
@@ -64936,17 +64959,17 @@
             time_serializers: () => Cn,
             typeset: () => Dt,
             uuid: () => h,
             version: () => Ao
         });
         var r = {};
         __webpack_require__.r(r), __webpack_require__.d(r, {
-            OUTPUT_WIDGET_VERSION: () => Vo,
-            OutputModel: () => Bo,
-            OutputView: () => Uo
+            OUTPUT_WIDGET_VERSION: () => Yo,
+            OutputModel: () => Vo,
+            OutputView: () => Bo
         });
         var i = {};
         __webpack_require__.r(i), __webpack_require__.d(i, {
             OutputModel: () => qa,
             OutputView: () => $a
         });
         const o = document.currentScript;
@@ -76955,67 +76978,66 @@
         };
         const Ao = __webpack_require__(56070).i8,
             Io = self.Bokeh.loader["@bokehjs/core/dom"],
             No = self.Bokeh.loader["@bokehjs/models/layouts/layout_dom"],
             zo = self.Bokeh.loader["@bokehjs/document/events"],
             jo = self.Bokeh.loader["@bokehjs/core/util/types"],
             Oo = self.Bokeh.loader["@bokehjs/core/util/assert"],
-            Po = self.Bokeh.loader["@bokehjs/core/util/object"],
-            Ro = requirejs,
-            Ho = new Set;
+            Po = requirejs,
+            Ro = new Set;
 
-        function Yo(e) {
+        function Ho(e) {
             return function(t, n) {
-                if (!Ho.has(t)) {
-                    Ho.add(t);
+                if (!Ro.has(t)) {
+                    Ro.add(t);
                     const r = {
                         paths: {}
                     };
                     r.paths[t] = function(e, t, n) {
                         let r = e,
                             i = "index",
                             o = e.indexOf("/");
                         return -1 != o && "@" == e[0] && (o = e.indexOf("/", o + 1)), -1 != o && (i = e.substr(o + 1), r = e.substr(0, o)), `${n}/${r}@${t}/dist/${i}`
-                    }(t, n, e), Ro.config(r)
+                    }(t, n, e), Po.config(r)
                 }
                 return console.debug(`Loading ${t}@${n} from ${e}`), r = [t], new Promise(((e, t) => requirejs(r, e, t)));
                 var r
             }
         }
-        const Vo = "1.0.0";
-        class Bo extends ft {
+        const Yo = "1.0.0";
+        class Vo extends ft {
             defaults() {
                 return Object.assign(Object.assign({}, super.defaults()), {
                     _model_name: "OutputModel",
                     _view_name: "OutputView",
                     _model_module: "@jupyter-widgets/output",
                     _view_module: "@jupyter-widgets/output",
-                    _model_module_version: Vo,
-                    _view_module_version: Vo
+                    _model_module_version: Yo,
+                    _view_module_version: Yo
                 })
             }
         }
-        class Uo extends _t {}
+        class Bo extends _t {}
 
-        function Fo(e) {
+        function Uo(e) {
             return "execute_result" === e.output_type
         }
 
-        function Wo(e) {
+        function Fo(e) {
             return "display_data" === e.output_type
         }
 
-        function qo(e) {
+        function Wo(e) {
             return "stream" === e.output_type
         }
-        class $o {
+        class qo {
             constructor(e = {}) {
                 this._array = [], this._isDisposed = !1, this._changed = new U.Signal(this), void 0 !== e.values && (0, S.each)(e.values, (e => {
                     this._array.push(e)
-                })), this._itemCmp = e.itemCmp || Go.itemCmp
+                })), this._itemCmp = e.itemCmp || $o.itemCmp
             }
             get type() {
                 return "List"
             }
             get changed() {
                 return this._changed
             }
@@ -77132,23 +77154,23 @@
                     oldIndex: e,
                     newIndex: -1,
                     oldValues: n,
                     newValues: []
                 }), this.length
             }
         }
-        var Go, Ko, Qo, Zo;
+        var $o, Go, Ko, Qo;
         ! function(e) {
             e.itemCmp = function(e, t) {
                 return e === t
             }
-        }(Go || (Go = {}));
-        class Jo {
+        }($o || ($o = {}));
+        class Zo {
             constructor(e = {}) {
-                if (this._map = new Map, this._changed = new U.Signal(this), this._isDisposed = !1, this._itemCmp = e.itemCmp || Ko.itemCmp, e.values)
+                if (this._map = new Map, this._changed = new U.Signal(this), this._isDisposed = !1, this._itemCmp = e.itemCmp || Go.itemCmp, e.values)
                     for (const t in e.values) this._map.set(t, e.values[t])
             }
             get type() {
                 return "Map"
             }
             get changed() {
                 return this._changed
@@ -77204,16 +77226,16 @@
             dispose() {
                 this.isDisposed || (this._isDisposed = !0, U.Signal.clearData(this), this._map.clear())
             }
         }! function(e) {
             e.itemCmp = function(e, t) {
                 return e === t
             }
-        }(Ko || (Ko = {}));
-        class Xo extends Jo {
+        }(Go || (Go = {}));
+        class Jo extends Zo {
             constructor(e = {}) {
                 super({
                     itemCmp: a.JSONExt.deepEqual,
                     values: e.values
                 })
             }
             toJSON() {
@@ -77227,37 +77249,37 @@
             }
         }! function(e) {
             e.ChangeMessage = class extends H {
                 constructor(e, t) {
                     super(e), this.args = t
                 }
             }
-        }(Xo || (Xo = {}));
-        class ea {
+        }(Jo || (Jo = {}));
+        class Xo {
             constructor(e) {
                 this._changed = new U.Signal(this), this._raw = {};
                 const {
                     data: t,
                     metadata: n,
                     trusted: r
-                } = Qo.getBundleOptions(e);
-                this._data = new Xo({
+                } = Ko.getBundleOptions(e);
+                this._data = new Jo({
                     values: t
-                }), this._rawData = t, this._metadata = new Xo({
+                }), this._rawData = t, this._metadata = new Jo({
                     values: n
                 }), this._rawMetadata = n, this.trusted = r;
                 const i = e.value;
                 for (const e in i) switch (e) {
                     case "data":
                     case "metadata":
                         break;
                     default:
-                        this._raw[e] = Qo.extract(i, e)
+                        this._raw[e] = Ko.extract(i, e)
                 }
-                this.type = i.output_type, Fo(i) ? this.executionCount = i.execution_count : this.executionCount = null
+                this.type = i.output_type, Uo(i) ? this.executionCount = i.execution_count : this.executionCount = null
             }
             get changed() {
                 return this._changed
             }
             dispose() {
                 this._data.dispose(), this._metadata.dispose(), U.Signal.clearData(this)
             }
@@ -77268,15 +77290,15 @@
                 return this._rawMetadata
             }
             setData(e) {
                 e.data && (this._updateObservable(this._data, e.data), this._rawData = e.data), e.metadata && (this._updateObservable(this._metadata, e.metadata), this._rawMetadata = e.metadata), this._changed.emit(void 0)
             }
             toJSON() {
                 const e = {};
-                for (const t in this._raw) e[t] = Qo.extract(this._raw, t);
+                for (const t in this._raw) e[t] = Ko.extract(this._raw, t);
                 switch (this.type) {
                     case "display_data":
                     case "execute_result":
                     case "update_display_data":
                         e.data = this.data, e.metadata = this.metadata
                 }
                 return delete e.transient, e
@@ -77289,26 +77311,26 @@
                     const r = e.get(n),
                         i = t[n];
                     r !== i && e.set(n, i)
                 }
             }
         }! function(e) {
             e.getData = function(e) {
-                return Qo.getData(e)
+                return Ko.getData(e)
             }, e.getMetadata = function(e) {
-                return Qo.getMetadata(e)
+                return Ko.getMetadata(e)
             }
-        }(ea || (ea = {})),
+        }(Xo || (Xo = {})),
         function(e) {
             function t(e) {
                 let t = {};
-                if (Fo(e) || Wo(e) || function(e) {
+                if (Uo(e) || Fo(e) || function(e) {
                         return "update_display_data" === e.output_type
                     }(e)) t = e.data;
-                else if (qo(e)) "stderr" === e.name ? t["application/vnd.jupyter.stderr"] = e.text : t["application/vnd.jupyter.stdout"] = e.text;
+                else if (Wo(e)) "stderr" === e.name ? t["application/vnd.jupyter.stderr"] = e.text : t["application/vnd.jupyter.stdout"] = e.text;
                 else if (function(e) {
                         return "error" === e.output_type
                     }(e)) {
                     t["application/vnd.jupyter.error"] = e;
                     const n = e.traceback.join("\n");
                     t["application/vnd.jupyter.stderr"] = n || `${e.ename}: ${e.evalue}`
                 }
@@ -77317,15 +77339,15 @@
                     for (const n in e) t[n] = r(e, n);
                     return t
                 }(t)
             }
 
             function n(e) {
                 const t = Object.create(null);
-                if (Fo(e) || Wo(e))
+                if (Uo(e) || Fo(e))
                     for (const n in e.metadata) t[n] = r(e.metadata, n);
                 return t
             }
 
             function r(e, t) {
                 const n = e[t];
                 return void 0 === n || a.JSONExt.isPrimitive(n) ? n : JSON.parse(JSON.stringify(n))
@@ -77333,18 +77355,18 @@
             e.getData = t, e.getMetadata = n, e.getBundleOptions = function(e) {
                 return {
                     data: t(e.value),
                     metadata: n(e.value),
                     trusted: !!e.trusted
                 }
             }, e.extract = r
-        }(Qo || (Qo = {}));
-        class ta {
+        }(Ko || (Ko = {}));
+        class ea {
             constructor(e = {}) {
-                this.clearNext = !1, this._trusted = !1, this._isDisposed = !1, this._stateChanged = new U.Signal(this), this._changed = new U.Signal(this), this._trusted = !!e.trusted, this.contentFactory = e.contentFactory || ta.defaultContentFactory, this.list = new $o, e.values && (0, S.each)(e.values, (e => {
+                this.clearNext = !1, this._trusted = !1, this._isDisposed = !1, this._stateChanged = new U.Signal(this), this._changed = new U.Signal(this), this._trusted = !!e.trusted, this.contentFactory = e.contentFactory || ea.defaultContentFactory, this.list = new qo, e.values && (0, S.each)(e.values, (e => {
                     this._add(e)
                 })), this.list.changed.connect(this._onListChanged, this)
             }
             get stateChanged() {
                 return this._stateChanged
             }
             get changed() {
@@ -77374,15 +77396,15 @@
             dispose() {
                 this.isDisposed || (this._isDisposed = !0, this.list.dispose(), U.Signal.clearData(this))
             }
             get(e) {
                 return this.list.get(e)
             }
             set(e, t) {
-                t = a.JSONExt.deepCopy(t), Zo.normalize(t);
+                t = a.JSONExt.deepCopy(t), Qo.normalize(t);
                 const n = this._createItem({
                     value: t,
                     trusted: this._trusted
                 });
                 this.list.set(e, n)
             }
             add(e) {
@@ -77399,32 +77421,32 @@
                 }))
             }
             toJSON() {
                 return (0, S.toArray)((0, S.map)(this.list, (e => e.toJSON())))
             }
             _add(e) {
                 const t = this._trusted;
-                if (e = a.JSONExt.deepCopy(e), Zo.normalize(e), qo(e) && this._lastStream && e.name === this._lastName && this.shouldCombine({
+                if (e = a.JSONExt.deepCopy(e), Qo.normalize(e), Wo(e) && this._lastStream && e.name === this._lastName && this.shouldCombine({
                         value: e,
                         lastModel: this.list.get(this.length - 1)
                     })) {
-                    this._lastStream += e.text, this._lastStream = Zo.removeOverwrittenChars(this._lastStream), e.text = this._lastStream;
+                    this._lastStream += e.text, this._lastStream = Qo.removeOverwrittenChars(this._lastStream), e.text = this._lastStream;
                     const n = this._createItem({
                             value: e,
                             trusted: t
                         }),
                         r = this.length - 1;
                     return this.list.get(r).dispose(), this.list.set(r, n), r
                 }
-                qo(e) && (e.text = Zo.removeOverwrittenChars(e.text));
+                Wo(e) && (e.text = Qo.removeOverwrittenChars(e.text));
                 const n = this._createItem({
                     value: e,
                     trusted: t
                 });
-                return qo(e) ? (this._lastStream = e.text, this._lastName = e.name) : this._lastStream = "", this.list.push(n)
+                return Wo(e) ? (this._lastStream = e.text, this._lastName = e.name) : this._lastStream = "", this.list.push(n)
             }
             shouldCombine(e) {
                 return !0
             }
             _createItem(e) {
                 const t = this.contentFactory.createOutputModel(e);
                 return t.changed.connect(this._onGenericChange, this), t
@@ -77434,22 +77456,22 @@
             }
             _onGenericChange() {
                 this._stateChanged.emit(void 0)
             }
         }! function(e) {
             class t {
                 createOutputModel(e) {
-                    return new ea(e)
+                    return new Xo(e)
                 }
             }
             e.ContentFactory = t, e.defaultContentFactory = new t
-        }(ta || (ta = {})),
+        }(ea || (ea = {})),
         function(e) {
             e.normalize = function(e) {
-                qo(e) && Array.isArray(e.text) && (e.text = e.text.join("\n"))
+                Wo(e) && Array.isArray(e.text) && (e.text = e.text.join("\n"))
             }, e.removeOverwrittenChars = function(e) {
                 return function(e) {
                     for (e = e.replace(/\r+\n/gm, "\n"); e.search(/\r[^$]/g) > -1;) {
                         const t = e.match(/^(.*)\r+/m)[1];
                         let n = e.match(/\r+(.*)$/m)[1];
                         n += t.slice(n.length, t.length), e = e.replace(/\r+.*$/m, "\r").replace(/^.*\r/m, n)
                     }
@@ -77458,21 +77480,21 @@
                     let t = e;
                     do {
                         t = (e = t).replace(/[^\n]\x08/gm, "")
                     } while (t.length < e.length);
                     return e
                 }(e))
             }
-        }(Zo || (Zo = {}));
-        var na = __webpack_require__(17266);
-        class ra {
+        }(Qo || (Qo = {}));
+        var ta = __webpack_require__(17266);
+        class na {
             constructor(e) {
                 this._currentChanged = new U.Signal(this), this._deferred = null, this._isDisposed = !1, this._widgetAdded = new U.Signal(this), this._widgetUpdated = new U.Signal(this);
                 const t = this._focusTracker = new $e,
-                    n = this._pool = new na.RestorablePool(e);
+                    n = this._pool = new ta.RestorablePool(e);
                 this.namespace = e.namespace, t.currentChanged.connect(((e, t) => {
                     t.newValue !== this.currentWidget && (n.current = t.newValue)
                 }), this), n.added.connect(((e, t) => {
                     this._widgetAdded.emit(t)
                 }), this), n.currentChanged.connect(((e, r) => {
                     null === r && t.currentWidget ? n.current = t.currentWidget : (this.onCurrentChanged(r), this._currentChanged.emit(r))
                 }), this), n.updated.connect(((e, t) => {
@@ -77529,16 +77551,16 @@
                 this._deferred = e
             }
             async save(e) {
                 return this._pool.save(e)
             }
             onCurrentChanged(e) {}
         }
-        var ia = __webpack_require__(76240),
-            oa = function() {
+        var ra = __webpack_require__(76240),
+            ia = function() {
                 if ("undefined" != typeof Map) return Map;
 
                 function e(e, t) {
                     var n = -1;
                     return e.some((function(e, r) {
                         return e[0] === t && (n = r, !0)
                     })), n
@@ -77573,36 +77595,36 @@
                         for (var n = 0, r = this.__entries__; n < r.length; n++) {
                             var i = r[n];
                             e.call(t, i[1], i[0])
                         }
                     }, t
                 }()
             }(),
-            aa = "undefined" != typeof window && "undefined" != typeof document && window.document === document,
-            sa = void 0 !== __webpack_require__.g && __webpack_require__.g.Math === Math ? __webpack_require__.g : "undefined" != typeof self && self.Math === Math ? self : "undefined" != typeof window && window.Math === Math ? window : Function("return this")(),
-            la = "function" == typeof requestAnimationFrame ? requestAnimationFrame.bind(sa) : function(e) {
+            oa = "undefined" != typeof window && "undefined" != typeof document && window.document === document,
+            aa = void 0 !== __webpack_require__.g && __webpack_require__.g.Math === Math ? __webpack_require__.g : "undefined" != typeof self && self.Math === Math ? self : "undefined" != typeof window && window.Math === Math ? window : Function("return this")(),
+            sa = "function" == typeof requestAnimationFrame ? requestAnimationFrame.bind(aa) : function(e) {
                 return setTimeout((function() {
                     return e(Date.now())
                 }), 1e3 / 60)
             },
-            ca = ["top", "right", "bottom", "left", "width", "height", "size", "weight"],
-            ua = "undefined" != typeof MutationObserver,
-            da = function() {
+            la = ["top", "right", "bottom", "left", "width", "height", "size", "weight"],
+            ca = "undefined" != typeof MutationObserver,
+            ua = function() {
                 function e() {
                     this.connected_ = !1, this.mutationEventsAdded_ = !1, this.mutationsObserver_ = null, this.observers_ = [], this.onTransitionEnd_ = this.onTransitionEnd_.bind(this), this.refresh = function(e, t) {
                         var n = !1,
                             r = !1,
                             i = 0;
 
                         function o() {
                             n && (n = !1, e()), r && s()
                         }
 
                         function a() {
-                            la(o)
+                            sa(o)
                         }
 
                         function s() {
                             var e = Date.now();
                             if (n) {
                                 if (e - i < 2) return;
                                 r = !0
@@ -77624,200 +77646,200 @@
                     var e = this.observers_.filter((function(e) {
                         return e.gatherActive(), e.hasActive()
                     }));
                     return e.forEach((function(e) {
                         return e.broadcastActive()
                     })), e.length > 0
                 }, e.prototype.connect_ = function() {
-                    aa && !this.connected_ && (document.addEventListener("transitionend", this.onTransitionEnd_), window.addEventListener("resize", this.refresh), ua ? (this.mutationsObserver_ = new MutationObserver(this.refresh), this.mutationsObserver_.observe(document, {
+                    oa && !this.connected_ && (document.addEventListener("transitionend", this.onTransitionEnd_), window.addEventListener("resize", this.refresh), ca ? (this.mutationsObserver_ = new MutationObserver(this.refresh), this.mutationsObserver_.observe(document, {
                         attributes: !0,
                         childList: !0,
                         characterData: !0,
                         subtree: !0
                     })) : (document.addEventListener("DOMSubtreeModified", this.refresh), this.mutationEventsAdded_ = !0), this.connected_ = !0)
                 }, e.prototype.disconnect_ = function() {
-                    aa && this.connected_ && (document.removeEventListener("transitionend", this.onTransitionEnd_), window.removeEventListener("resize", this.refresh), this.mutationsObserver_ && this.mutationsObserver_.disconnect(), this.mutationEventsAdded_ && document.removeEventListener("DOMSubtreeModified", this.refresh), this.mutationsObserver_ = null, this.mutationEventsAdded_ = !1, this.connected_ = !1)
+                    oa && this.connected_ && (document.removeEventListener("transitionend", this.onTransitionEnd_), window.removeEventListener("resize", this.refresh), this.mutationsObserver_ && this.mutationsObserver_.disconnect(), this.mutationEventsAdded_ && document.removeEventListener("DOMSubtreeModified", this.refresh), this.mutationsObserver_ = null, this.mutationEventsAdded_ = !1, this.connected_ = !1)
                 }, e.prototype.onTransitionEnd_ = function(e) {
                     var t = e.propertyName,
                         n = void 0 === t ? "" : t;
-                    ca.some((function(e) {
+                    la.some((function(e) {
                         return !!~n.indexOf(e)
                     })) && this.refresh()
                 }, e.getInstance = function() {
                     return this.instance_ || (this.instance_ = new e), this.instance_
                 }, e.instance_ = null, e
             }(),
-            ha = function(e, t) {
+            da = function(e, t) {
                 for (var n = 0, r = Object.keys(t); n < r.length; n++) {
                     var i = r[n];
                     Object.defineProperty(e, i, {
                         value: t[i],
                         enumerable: !1,
                         writable: !1,
                         configurable: !0
                     })
                 }
                 return e
             },
-            fa = function(e) {
-                return e && e.ownerDocument && e.ownerDocument.defaultView || sa
+            ha = function(e) {
+                return e && e.ownerDocument && e.ownerDocument.defaultView || aa
             },
-            pa = ya(0, 0, 0, 0);
+            fa = _a(0, 0, 0, 0);
 
-        function ma(e) {
+        function pa(e) {
             return parseFloat(e) || 0
         }
 
-        function ga(e) {
+        function ma(e) {
             for (var t = [], n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
             return t.reduce((function(t, n) {
-                return t + ma(e["border-" + n + "-width"])
+                return t + pa(e["border-" + n + "-width"])
             }), 0)
         }
-        var va = "undefined" != typeof SVGGraphicsElement ? function(e) {
-            return e instanceof fa(e).SVGGraphicsElement
+        var ga = "undefined" != typeof SVGGraphicsElement ? function(e) {
+            return e instanceof ha(e).SVGGraphicsElement
         } : function(e) {
-            return e instanceof fa(e).SVGElement && "function" == typeof e.getBBox
+            return e instanceof ha(e).SVGElement && "function" == typeof e.getBBox
         };
 
-        function _a(e) {
-            return aa ? va(e) ? function(e) {
+        function va(e) {
+            return oa ? ga(e) ? function(e) {
                 var t = e.getBBox();
-                return ya(0, 0, t.width, t.height)
+                return _a(0, 0, t.width, t.height)
             }(e) : function(e) {
                 var t = e.clientWidth,
                     n = e.clientHeight;
-                if (!t && !n) return pa;
-                var r = fa(e).getComputedStyle(e),
+                if (!t && !n) return fa;
+                var r = ha(e).getComputedStyle(e),
                     i = function(e) {
                         for (var t = {}, n = 0, r = ["top", "right", "bottom", "left"]; n < r.length; n++) {
                             var i = r[n],
                                 o = e["padding-" + i];
-                            t[i] = ma(o)
+                            t[i] = pa(o)
                         }
                         return t
                     }(r),
                     o = i.left + i.right,
                     a = i.top + i.bottom,
-                    s = ma(r.width),
-                    l = ma(r.height);
-                if ("border-box" === r.boxSizing && (Math.round(s + o) !== t && (s -= ga(r, "left", "right") + o), Math.round(l + a) !== n && (l -= ga(r, "top", "bottom") + a)), ! function(e) {
-                        return e === fa(e).document.documentElement
+                    s = pa(r.width),
+                    l = pa(r.height);
+                if ("border-box" === r.boxSizing && (Math.round(s + o) !== t && (s -= ma(r, "left", "right") + o), Math.round(l + a) !== n && (l -= ma(r, "top", "bottom") + a)), ! function(e) {
+                        return e === ha(e).document.documentElement
                     }(e)) {
                     var c = Math.round(s + o) - t,
                         u = Math.round(l + a) - n;
                     1 !== Math.abs(c) && (s -= c), 1 !== Math.abs(u) && (l -= u)
                 }
-                return ya(i.left, i.top, s, l)
-            }(e) : pa
+                return _a(i.left, i.top, s, l)
+            }(e) : fa
         }
 
-        function ya(e, t, n, r) {
+        function _a(e, t, n, r) {
             return {
                 x: e,
                 y: t,
                 width: n,
                 height: r
             }
         }
-        var ba = function() {
+        var ya = function() {
                 function e(e) {
-                    this.broadcastWidth = 0, this.broadcastHeight = 0, this.contentRect_ = ya(0, 0, 0, 0), this.target = e
+                    this.broadcastWidth = 0, this.broadcastHeight = 0, this.contentRect_ = _a(0, 0, 0, 0), this.target = e
                 }
                 return e.prototype.isActive = function() {
-                    var e = _a(this.target);
+                    var e = va(this.target);
                     return this.contentRect_ = e, e.width !== this.broadcastWidth || e.height !== this.broadcastHeight
                 }, e.prototype.broadcastRect = function() {
                     var e = this.contentRect_;
                     return this.broadcastWidth = e.width, this.broadcastHeight = e.height, e
                 }, e
             }(),
-            Ma = function(e, t) {
+            ba = function(e, t) {
                 var n = function(e) {
                     var t = e.x,
                         n = e.y,
                         r = e.width,
                         i = e.height,
                         o = "undefined" != typeof DOMRectReadOnly ? DOMRectReadOnly : Object,
                         a = Object.create(o.prototype);
-                    return ha(a, {
+                    return da(a, {
                         x: t,
                         y: n,
                         width: r,
                         height: i,
                         top: n,
                         right: t + r,
                         bottom: i + n,
                         left: t
                     }), a
                 }(t);
-                ha(this, {
+                da(this, {
                     target: e,
                     contentRect: n
                 })
             },
-            wa = function() {
+            Ma = function() {
                 function e(e, t, n) {
-                    if (this.activeObservations_ = [], this.observations_ = new oa, "function" != typeof e) throw new TypeError("The callback provided as parameter 1 is not a function.");
+                    if (this.activeObservations_ = [], this.observations_ = new ia, "function" != typeof e) throw new TypeError("The callback provided as parameter 1 is not a function.");
                     this.callback_ = e, this.controller_ = t, this.callbackCtx_ = n
                 }
                 return e.prototype.observe = function(e) {
                     if (!arguments.length) throw new TypeError("1 argument required, but only 0 present.");
                     if ("undefined" != typeof Element && Element instanceof Object) {
-                        if (!(e instanceof fa(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
+                        if (!(e instanceof ha(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
                         var t = this.observations_;
-                        t.has(e) || (t.set(e, new ba(e)), this.controller_.addObserver(this), this.controller_.refresh())
+                        t.has(e) || (t.set(e, new ya(e)), this.controller_.addObserver(this), this.controller_.refresh())
                     }
                 }, e.prototype.unobserve = function(e) {
                     if (!arguments.length) throw new TypeError("1 argument required, but only 0 present.");
                     if ("undefined" != typeof Element && Element instanceof Object) {
-                        if (!(e instanceof fa(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
+                        if (!(e instanceof ha(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
                         var t = this.observations_;
                         t.has(e) && (t.delete(e), t.size || this.controller_.removeObserver(this))
                     }
                 }, e.prototype.disconnect = function() {
                     this.clearActive(), this.observations_.clear(), this.controller_.removeObserver(this)
                 }, e.prototype.gatherActive = function() {
                     var e = this;
                     this.clearActive(), this.observations_.forEach((function(t) {
                         t.isActive() && e.activeObservations_.push(t)
                     }))
                 }, e.prototype.broadcastActive = function() {
                     if (this.hasActive()) {
                         var e = this.callbackCtx_,
                             t = this.activeObservations_.map((function(e) {
-                                return new Ma(e.target, e.broadcastRect())
+                                return new ba(e.target, e.broadcastRect())
                             }));
                         this.callback_.call(e, t, e), this.clearActive()
                     }
                 }, e.prototype.clearActive = function() {
                     this.activeObservations_.splice(0)
                 }, e.prototype.hasActive = function() {
                     return this.activeObservations_.length > 0
                 }, e
             }(),
-            La = "undefined" != typeof WeakMap ? new WeakMap : new oa,
-            xa = function e(t) {
+            wa = "undefined" != typeof WeakMap ? new WeakMap : new ia,
+            La = function e(t) {
                 if (!(this instanceof e)) throw new TypeError("Cannot call a class as a function.");
                 if (!arguments.length) throw new TypeError("1 argument required, but only 0 present.");
-                var n = da.getInstance(),
-                    r = new wa(t, n, this);
-                La.set(this, r)
+                var n = ua.getInstance(),
+                    r = new Ma(t, n, this);
+                wa.set(this, r)
             };
         ["observe", "unobserve", "disconnect"].forEach((function(e) {
-            xa.prototype[e] = function() {
+            La.prototype[e] = function() {
                 var t;
-                return (t = La.get(this))[e].apply(t, arguments)
+                return (t = wa.get(this))[e].apply(t, arguments)
             }
         }));
-        const Ta = void 0 !== sa.ResizeObserver ? sa.ResizeObserver : xa,
-            Ea = "jp-OutputArea-child",
-            Ca = "jp-OutputArea-output",
-            Sa = "jp-OutputArea-prompt";
-        class ka extends fe {
+        const xa = void 0 !== aa.ResizeObserver ? aa.ResizeObserver : La,
+            Ta = "jp-OutputArea-child",
+            Ea = "jp-OutputArea-output",
+            Ca = "jp-OutputArea-prompt";
+        class Sa extends fe {
             constructor(e) {
                 var t;
                 super(), this.outputLengthChanged = new U.Signal(this), this._onIOPub = e => {
                     const t = this.model,
                         n = e.header.msg_type;
                     let r;
                     const i = (e.content.transient || {}).display_id;
@@ -77853,17 +77875,17 @@
                     if (!i.length) return;
                     const o = {
                         output_type: "display_data",
                         data: JSON.parse(JSON.stringify(i[0])).data,
                         metadata: {}
                     };
                     t.add(o)
-                }, this._minHeightTimeout = null, this._displayIdMap = new Map, this._outputTracker = new ra({
+                }, this._minHeightTimeout = null, this._displayIdMap = new Map, this._outputTracker = new na({
                     namespace: a.UUID.uuid4()
-                }), this.addClass("jp-OutputArea"), this.contentFactory = e.contentFactory || ka.defaultContentFactory, this.layout = new _e, this.rendermime = e.rendermime, this._maxNumberOutputs = null !== (t = e.maxNumberOutputs) && void 0 !== t ? t : 1 / 0;
+                }), this.addClass("jp-OutputArea"), this.contentFactory = e.contentFactory || Sa.defaultContentFactory, this.layout = new _e, this.rendermime = e.rendermime, this._maxNumberOutputs = null !== (t = e.maxNumberOutputs) && void 0 !== t ? t : 1 / 0;
                 const n = this.model = e.model;
                 for (let e = 0; e < Math.min(n.length, this._maxNumberOutputs + 1); e++) {
                     const t = n.get(e);
                     this._insertOutput(e, t)
                 }
                 n.changed.connect(this.onModelChanged, this), n.stateChanged.connect(this.onStateChanged, this)
             }
@@ -77872,15 +77894,15 @@
             }
             get future() {
                 return this._future
             }
             set future(e) {
                 if (this.model.isDisposed) throw Error("Model is disposed");
                 this._future !== e && (this._future && this._future.dispose(), this._future = e, this.model.clear(), this.widgets.length && (this._clear(), this.outputLengthChanged.emit(this.model.length)), e.onIOPub = this._onIOPub, e.onReply = this._onExecuteReply, e.onStdin = t => {
-                    ia.KernelMessage.isInputRequestMsg(t) && this.onInputRequest(t, e)
+                    ra.KernelMessage.isInputRequestMsg(t) && this.onInputRequest(t, e)
                 })
             }
             get maxNumberOutputs() {
                 return this._maxNumberOutputs
             }
             set maxNumberOutputs(e) {
                 if (e <= 0) return void console.warn("OutputArea.maxNumberOutputs must be strictly positive.");
@@ -77941,43 +77963,43 @@
                 }), 50)
             }
             onInputRequest(e, t) {
                 const n = this.contentFactory,
                     r = e.content.prompt,
                     i = e.content.password,
                     o = new Te;
-                o.addClass(Ea), o.addClass("jp-OutputArea-stdin-item");
+                o.addClass(Ta), o.addClass("jp-OutputArea-stdin-item");
                 const a = n.createOutputPrompt();
-                a.addClass(Sa), o.addWidget(a);
+                a.addClass(Ca), o.addWidget(a);
                 const s = n.createStdin({
                     parent_header: e.header,
                     prompt: r,
                     password: i,
                     future: t
                 });
-                s.addClass(Ca), o.addWidget(s), this.model.length >= this.maxNumberOutputs && (this.maxNumberOutputs = this.model.length), this.layout.addWidget(o), s.value.then((e => {
+                s.addClass(Ea), o.addWidget(s), this.model.length >= this.maxNumberOutputs && (this.maxNumberOutputs = this.model.length), this.layout.addWidget(o), s.value.then((e => {
                     this.model.length >= this.maxNumberOutputs && (this.maxNumberOutputs = this.model.length + 1), this.model.add({
                         output_type: "stream",
                         name: "stdin",
                         text: e + "\n"
                     }), o.dispose()
                 }))
             }
             _setOutput(e, t) {
                 if (e >= this._maxNumberOutputs) return;
                 const n = this.layout.widgets[e],
                     r = n.widgets ? n.widgets[1] : n,
                     i = this.rendermime.preferredMimeType(t.data, t.trusted ? "any" : "ensure");
-                r.renderModel && Ia.currentPreferredMimetype.get(r) === i && ka.isIsolated(i, t.metadata) === r instanceof Ia.IsolatedRenderer ? r.renderModel(t) : (this.layout.widgets[e].dispose(), this._insertOutput(e, t))
+                r.renderModel && Aa.currentPreferredMimetype.get(r) === i && Sa.isIsolated(i, t.metadata) === r instanceof Aa.IsolatedRenderer ? r.renderModel(t) : (this.layout.widgets[e].dispose(), this._insertOutput(e, t))
             }
             _insertOutput(e, t) {
                 if (e > this._maxNumberOutputs) return;
                 const n = this.layout;
                 if (e === this._maxNumberOutputs) {
-                    const t = new Ia.TrimmedOutputs(this._maxNumberOutputs, (() => {
+                    const t = new Aa.TrimmedOutputs(this._maxNumberOutputs, (() => {
                         const e = this._maxNumberOutputs;
                         this._maxNumberOutputs = 1 / 0, this._showTrimmedOutputs(e)
                     }));
                     n.insertWidget(e, this._wrappedOutput(t))
                 } else {
                     let r = this.createOutputItem(t);
                     r ? r.toggleClass("jp-OutputArea-executeResult", null !== t.executionCount) : r = new fe, this._outputTracker.has(r) || this._outputTracker.add(r), n.insertWidget(e, r)
@@ -77995,24 +78017,24 @@
                 const t = this.createRenderedMimetype(e);
                 return t ? this._wrappedOutput(t, e.executionCount) : null
             }
             createRenderedMimetype(e) {
                 const t = this.rendermime.preferredMimeType(e.data, e.trusted ? "any" : "ensure");
                 if (!t) return null;
                 let n = this.rendermime.createRenderer(t);
-                return !0 === ka.isIsolated(t, e.metadata) && (n = new Ia.IsolatedRenderer(n)), Ia.currentPreferredMimetype.set(n, t), n.renderModel(e).catch((e => {
+                return !0 === Sa.isIsolated(t, e.metadata) && (n = new Aa.IsolatedRenderer(n)), Aa.currentPreferredMimetype.set(n, t), n.renderModel(e).catch((e => {
                     const t = document.createElement("pre");
                     t.textContent = `Javascript Error: ${e.message}`, n.node.appendChild(t), n.node.className = "lm-Widget jp-RenderedText", n.node.setAttribute("data-mime-type", "application/vnd.jupyter.stderr")
                 })), n
             }
             _wrappedOutput(e, t = null) {
-                const n = new Ia.OutputPanel;
-                n.addClass(Ea);
+                const n = new Aa.OutputPanel;
+                n.addClass(Ta);
                 const r = this.contentFactory.createOutputPrompt();
-                return r.executionCount = t, r.addClass(Sa), n.addWidget(r), e.addClass(Ca), n.addWidget(e), n
+                return r.executionCount = t, r.addClass(Ca), n.addWidget(r), e.addClass(Ea), n.addWidget(e), n
             }
         }! function(e) {
             e.execute = async function(e, t, n, r) {
                 var i;
                 let o = !0;
                 r && Array.isArray(r.tags) && -1 !== r.tags.indexOf("raises-exception") && (o = !1);
                 const a = {
@@ -78025,78 +78047,78 @@
                 return t.future = l, l.done
             }, e.isIsolated = function(e, t) {
                 const n = t[e];
                 return n && void 0 !== n.isolated ? !!n.isolated : !!t.isolated
             };
             class t {
                 createOutputPrompt() {
-                    return new Da
+                    return new ka
                 }
                 createStdin(e) {
-                    return new Aa(e)
+                    return new Da(e)
                 }
             }
             e.ContentFactory = t, e.defaultContentFactory = new t
-        }(ka || (ka = {}));
-        class Da extends fe {
+        }(Sa || (Sa = {}));
+        class ka extends fe {
             constructor() {
                 super(), this._executionCount = null, this.addClass("jp-OutputPrompt")
             }
             get executionCount() {
                 return this._executionCount
             }
             set executionCount(e) {
                 this._executionCount = e, this.node.textContent = null === e ? "" : `[${e}]:`
             }
         }
-        class Aa extends fe {
+        class Da extends fe {
             constructor(e) {
                 super({
-                    node: Ia.createInputWidgetNode(e.prompt, e.password)
+                    node: Aa.createInputWidgetNode(e.prompt, e.password)
                 }), this._promise = new a.PromiseDelegate, this.addClass("jp-Stdin"), this._history_ix = 0, this._input = this.node.getElementsByTagName("input")[0], this._input.focus(), this._input.placeholder = "↑↓ for history", this._future = e.future, this._parentHeader = e.parent_header, this._value = e.prompt + " ", this._password = e.password
             }
             static _historyAt(e) {
-                const t = Aa._history.length;
-                if ((e = e < 0 ? t + e : e) < t) return Aa._history[e]
+                const t = Da._history.length;
+                if ((e = e < 0 ? t + e : e) < t) return Da._history[e]
             }
             static _historyPush(e) {
-                Aa._history.push(e), Aa._history.length > 1e3 && Aa._history.shift()
+                Da._history.push(e), Da._history.length > 1e3 && Da._history.shift()
             }
             get value() {
                 return this._promise.promise.then((() => this._value))
             }
             handleEvent(e) {
                 const t = this._input;
                 if ("keydown" === e.type)
                     if ("ArrowUp" === e.key) {
-                        const e = Aa._historyAt(this._history_ix - 1);
+                        const e = Da._historyAt(this._history_ix - 1);
                         e && (0 === this._history_ix && (this._value_cache = t.value), t.value = e, --this._history_ix)
                     } else if ("ArrowDown" === e.key)
                     if (0 === this._history_ix);
                     else if (-1 === this._history_ix) t.value = this._value_cache, ++this._history_ix;
                 else {
-                    const e = Aa._historyAt(this._history_ix + 1);
+                    const e = Da._historyAt(this._history_ix + 1);
                     e && (t.value = e, ++this._history_ix)
                 } else "Enter" === e.key && (this._future.sendInputReply({
                     status: "ok",
                     value: t.value
-                }, this._parentHeader), this._password ? this._value += "········" : (this._value += t.value, Aa._historyPush(t.value)), this._promise.resolve(void 0))
+                }, this._parentHeader), this._password ? this._value += "········" : (this._value += t.value, Da._historyPush(t.value)), this._promise.resolve(void 0))
             }
             onAfterAttach(e) {
                 this._input.addEventListener("keydown", this), this.update()
             }
             onUpdateRequest(e) {
                 this._input.focus()
             }
             onBeforeDetach(e) {
                 this._input.removeEventListener("keydown", this)
             }
         }
-        var Ia;
-        Aa._history = [],
+        var Aa;
+        Da._history = [],
             function(e) {
                 e.createInputWidgetNode = function(e, t) {
                     const n = document.createElement("div"),
                         r = document.createElement("pre");
                     r.className = "jp-Stdin-prompt", r.textContent = e;
                     const i = document.createElement("input");
                     return i.className = "jp-Stdin-input", t && (i.type = "password"), n.appendChild(r), r.appendChild(i), n
@@ -78105,15 +78127,15 @@
                         super({
                             node: document.createElement("iframe")
                         }), this.addClass("jp-mod-isolated"), this._wrapped = e;
                         const t = this.node;
                         t.frameBorder = "0", t.scrolling = "auto", t.addEventListener("load", (() => {
                             t.contentDocument.open(), t.contentDocument.write(this._wrapped.node.innerHTML), t.contentDocument.close();
                             const e = t.contentDocument.body;
-                            t.style.height = `${e.scrollHeight}px`, t.heightChangeObserver = new Ta((() => {
+                            t.style.height = `${e.scrollHeight}px`, t.heightChangeObserver = new xa((() => {
                                 t.style.height = `${e.scrollHeight}px`
                             })), t.heightChangeObserver.observe(e)
                         }))
                     }
                     renderModel(e) {
                         return this._wrapped.renderModel(e)
                     }
@@ -78146,71 +78168,64 @@
                     onAfterAttach(e) {
                         super.onAfterAttach(e), this.node.addEventListener("click", this)
                     }
                     onBeforeDetach(e) {
                         super.onBeforeDetach(e), this.node.removeEventListener("click", this)
                     }
                 }
-            }(Ia || (Ia = {}));
-        var Na = __webpack_require__(93379),
-            za = __webpack_require__.n(Na),
-            ja = __webpack_require__(7795),
-            Oa = __webpack_require__.n(ja),
-            Pa = __webpack_require__(3565),
-            Ra = __webpack_require__.n(Pa),
-            Ha = __webpack_require__(19216),
-            Ya = __webpack_require__.n(Ha),
-            Va = __webpack_require__(72024),
-            Ba = {};
-        Va.Z && Va.Z.locals && (Ba.locals = Va.Z.locals);
-        var Ua, Fa = 0,
-            Wa = {
-                styleTagTransform: (e, t, n) => {
-                    n.handler(e)
-                }
-            };
-        Wa.setAttributes = Ra(), Wa.insert = (e, t) => {}, Wa.domAPI = Oa(), Wa.insertStyleElement = Ya(), Ba.use = function(e) {
-            return Wa.options = e || {}, Fa++ || (Ua = za()(Va.Z, Wa)), Ba
-        }, Ba.unuse = function() {
-            Fa > 0 && !--Fa && (Ua(), Ua = null)
-        };
-        class qa extends Bo {
+            }(Aa || (Aa = {}));
+        var Ia = __webpack_require__(93379),
+            Na = __webpack_require__.n(Ia),
+            za = __webpack_require__(7795),
+            ja = __webpack_require__.n(za),
+            Oa = __webpack_require__(90569),
+            Pa = __webpack_require__.n(Oa),
+            Ra = __webpack_require__(3565),
+            Ha = __webpack_require__.n(Ra),
+            Ya = __webpack_require__(19216),
+            Va = __webpack_require__.n(Ya),
+            Ba = __webpack_require__(44589),
+            Ua = __webpack_require__.n(Ba),
+            Fa = __webpack_require__(72024),
+            Wa = {};
+        Wa.styleTagTransform = Ua(), Wa.setAttributes = Ha(), Wa.insert = Pa().bind(null, "head"), Wa.domAPI = ja(), Wa.insertStyleElement = Va(), Na()(Fa.Z, Wa), Fa.Z && Fa.Z.locals && Fa.Z.locals;
+        class qa extends Vo {
             defaults() {
                 return Object.assign(Object.assign({}, super.defaults()), {
                     msg_id: "",
                     outputs: []
                 })
             }
             initialize(e, t) {
-                super.initialize(e, t), this._outputs = new ta({
+                super.initialize(e, t), this._outputs = new ea({
                     trusted: !0
                 }), this.listenTo(this, "change:outputs", this.setOutputs), this.setOutputs()
             }
             get outputs() {
                 return this._outputs
             }
             clear_output(e = !1) {
                 this._outputs.clear(e)
             }
             setOutputs(e, t, n) {
                 n && n.newMessage || (this.clear_output(), this._outputs.fromJSON(JSON.parse(JSON.stringify(this.get("outputs")))))
             }
         }
-        class $a extends Uo {
+        class $a extends Bo {
             _createElement(e) {
                 return this.luminoWidget = new vt({
                     view: this
                 }), this.luminoWidget.node
             }
             _setElement(e) {
                 if (this.el || e !== this.luminoWidget.node) throw new Error("Cannot reset the DOM element.");
                 this.el = this.luminoWidget.node, this.$el = L()(this.luminoWidget.node)
             }
             render() {
-                super.render(), this._outputView = new ka({
+                super.render(), this._outputView = new Sa({
                     rendermime: this.model.widget_manager.renderMime,
                     model: this.model.outputs
                 }), this.luminoWidget.insertWidget(0, this._outputView), this.luminoWidget.addClass("jupyter-widgets"), this.luminoWidget.addClass("widget-output"), this.update()
             }
             remove() {
                 return this._outputView.dispose(), super.remove()
             }
@@ -80604,15 +80619,15 @@
                     return n ? `${t} ${n}` : t
                 }
                 renderLabel(e) {
                     const t = document.createElement("div");
                     return t.className = "jp-Dialog-buttonLabel", t.title = e.caption, t.appendChild(document.createTextNode(e.label)), t
                 }
             }
-            e.Renderer = n, e.defaultRenderer = new n, e.tracker = new ra({
+            e.Renderer = n, e.defaultRenderer = new n, e.tracker = new na({
                 namespace: "@jupyterlab/apputils:Dialog"
             })
         }(Vs || (Vs = {})),
         function(e) {
             e.launchQueue = [], e.errorMessagePromiseCache = new Map, e.handleOptions = function(e = {}) {
                 var t, n, r, i, o, a, s, l, c;
                 const u = null !== (t = e.buttons) && void 0 !== t ? t : [Vs.cancelButton(), Vs.okButton()];
@@ -80676,15 +80691,15 @@
             get isDisposed() {
                 return this._isDisposed
             }
             dispose() {
                 this._isDisposed || (this._isDisposed = !0, U.Signal.clearData(this), this.clear())
             }
         }
-        class Us extends $o {
+        class Us extends qo {
             constructor(e) {
                 super(), this._inCompound = !1, this._isUndoable = !0, this._madeCompoundChange = !1, this._index = -1, this._stack = [], this._serializer = e, this.changed.connect(this._onListChanged, this)
             }
             get canRedo() {
                 return this._index < this._stack.length - 1
             }
             get canUndo() {
@@ -80825,15 +80840,15 @@
                 this._isDisposed || (this._isDisposed = !0, U.Signal.clearData(this), this._value = null)
             }
         }! function(e) {
             e.IChangedArgs = class {}
         }(Fs || (Fs = {}));
         class Ws {
             constructor(e = {}) {
-                this.isPrepopulated = !1, this.isCollaborative = !1, this.connected = Promise.resolve(void 0), this._toDispose = !1, this._isDisposed = !1, this._disposables = new F.DisposableSet, this._basePath = e.basePath || "", e.baseDB ? this._db = e.baseDB : (this._db = new Jo, this._toDispose = !0)
+                this.isPrepopulated = !1, this.isCollaborative = !1, this.connected = Promise.resolve(void 0), this._toDispose = !1, this._isDisposed = !1, this._disposables = new F.DisposableSet, this._basePath = e.basePath || "", e.baseDB ? this._db = e.baseDB : (this._db = new Zo, this._toDispose = !0)
             }
             get basePath() {
                 return this._basePath
             }
             get isDisposed() {
                 return this._isDisposed
             }
@@ -80848,15 +80863,15 @@
                 return this._disposables.add(t), this.set(e, t), t
             }
             createList(e) {
                 const t = new Us(new Us.IdentitySerializer);
                 return this._disposables.add(t), this.set(e, t), t
             }
             createMap(e) {
-                const t = new Xo;
+                const t = new Jo;
                 return this._disposables.add(t), this.set(e, t), t
             }
             createValue(e) {
                 const t = new Fs;
                 return this._disposables.add(t), this.set(e, t), t
             }
             getValue(e) {
@@ -88050,82 +88065,39 @@
                 return new Promise(((e, a) => {
                     "@jupyter-widgets/base" === r ? e(t) : "@jupyter-widgets/controls" === r ? e(n) : "@jupyter-widgets/output" === r ? e(i) : void 0 !== this.loader ? e(this.loader(r, o)) : a(`Could not load module ${r}@${o}`)
                 })).then((t => t[e] ? t[e] : Promise.reject(`Class ${e} not found in module ${r}@${o}`)))
             }
         }
         var pp = __webpack_require__(27594),
             mp = {};
-        pp.Z && pp.Z.locals && (mp.locals = pp.Z.locals);
-        var gp, vp = 0,
-            _p = {
-                styleTagTransform: (e, t, n) => {
-                    n.handler(e)
-                }
-            };
-        _p.setAttributes = Ra(), _p.insert = (e, t) => {}, _p.domAPI = Oa(), _p.insertStyleElement = Ya(), mp.use = function(e) {
-            return _p.options = e || {}, vp++ || (gp = za()(pp.Z, _p)), mp
-        }, mp.unuse = function() {
-            vp > 0 && !--vp && (gp(), gp = null)
-        };
-        var yp = __webpack_require__(6846),
-            bp = {};
-        yp.Z && yp.Z.locals && (bp.locals = yp.Z.locals);
-        var Mp, wp = 0,
-            Lp = {
-                styleTagTransform: (e, t, n) => {
-                    n.handler(e)
-                }
-            };
-        Lp.setAttributes = Ra(), Lp.insert = (e, t) => {}, Lp.domAPI = Oa(), Lp.insertStyleElement = Ya(), bp.use = function(e) {
-            return Lp.options = e || {}, wp++ || (Mp = za()(yp.Z, Lp)), bp
-        }, bp.unuse = function() {
-            wp > 0 && !--wp && (Mp(), Mp = null)
-        };
-        var xp = __webpack_require__(15955),
-            Tp = {};
-        xp.Z && xp.Z.locals && (Tp.locals = xp.Z.locals);
-        var Ep, Cp = 0,
-            Sp = {
-                styleTagTransform: (e, t, n) => {
-                    n.handler(e)
-                }
-            };
-        Sp.setAttributes = Ra(), Sp.insert = (e, t) => {}, Sp.domAPI = Oa(), Sp.insertStyleElement = Ya(), Tp.use = function(e) {
-            return Sp.options = e || {}, Cp++ || (Ep = za()(xp.Z, Sp)), Tp
-        }, Tp.unuse = function() {
-            Cp > 0 && !--Cp && (Ep(), Ep = null)
-        };
-        var kp = __webpack_require__(97961),
-            Dp = {};
-        kp.Z && kp.Z.locals && (Dp.locals = kp.Z.locals);
-        var Ap, Ip = 0,
-            Np = {
-                styleTagTransform: (e, t, n) => {
-                    n.handler(e)
-                }
-            };
-        Np.setAttributes = Ra(), Np.insert = (e, t) => {}, Np.domAPI = Oa(), Np.insertStyleElement = Ya(), Dp.use = function(e) {
-            return Np.options = e || {}, Ip++ || (Ap = za()(kp.Z, Np)), Dp
-        }, Dp.unuse = function() {
-            Ip > 0 && !--Ip && (Ap(), Ap = null)
-        };
-        var zp = __webpack_require__(1581),
-            jp = __webpack_require__.n(zp);
-        __webpack_require__.p = window.__jupyter_widgets_assets_path__ || __webpack_require__.p, "" === getComputedStyle(document.documentElement).getPropertyValue("--jp-layout-color0") && __webpack_require__(20019);
-        const Op = __webpack_require__(48965).v2.state,
-            Pp = __webpack_require__(48965).v2.view,
-            Rp = new(jp());
-        Rp.compile(Op), Rp.compile(Pp);
-        let Hp = "https://cdn.jsdelivr.net/npm/",
-            Yp = !1;
-        const Vp = document.getElementsByTagName("script");
-        Array.prototype.forEach.call(Vp, (e => {
-            Hp = e.getAttribute("data-jupyter-widgets-cdn") || Hp, Yp = Yp || e.hasAttribute("data-jupyter-widgets-cdn-only")
+        mp.styleTagTransform = Ua(), mp.setAttributes = Ha(), mp.insert = Pa().bind(null, "head"), mp.domAPI = ja(), mp.insertStyleElement = Va(), Na()(pp.Z, mp), pp.Z && pp.Z.locals && pp.Z.locals;
+        var gp = __webpack_require__(6846),
+            vp = {};
+        vp.styleTagTransform = Ua(), vp.setAttributes = Ha(), vp.insert = Pa().bind(null, "head"), vp.domAPI = ja(), vp.insertStyleElement = Va(), Na()(gp.Z, vp), gp.Z && gp.Z.locals && gp.Z.locals;
+        var _p = __webpack_require__(15955),
+            yp = {};
+        yp.styleTagTransform = Ua(), yp.setAttributes = Ha(), yp.insert = Pa().bind(null, "head"), yp.domAPI = ja(), yp.insertStyleElement = Va(), Na()(_p.Z, yp), _p.Z && _p.Z.locals && _p.Z.locals;
+        var bp = __webpack_require__(97961),
+            Mp = {};
+        Mp.styleTagTransform = Ua(), Mp.setAttributes = Ha(), Mp.insert = Pa().bind(null, "head"), Mp.domAPI = ja(), Mp.insertStyleElement = Va(), Na()(bp.Z, Mp), bp.Z && bp.Z.locals && bp.Z.locals;
+        var wp = __webpack_require__(1581),
+            Lp = __webpack_require__.n(wp);
+        __webpack_require__.p = window.__jupyter_widgets_assets_path__ || __webpack_require__.p, "" === getComputedStyle(document.documentElement).getPropertyValue("--jp-layout-color0") && __webpack_require__(54993);
+        const xp = __webpack_require__(48965).v2.state,
+            Tp = __webpack_require__(48965).v2.view,
+            Ep = new(Lp());
+        Ep.compile(xp), Ep.compile(Tp);
+        let Cp = "https://cdn.jsdelivr.net/npm/",
+            Sp = !1;
+        const kp = document.getElementsByTagName("script");
+        Array.prototype.forEach.call(kp, (e => {
+            Cp = e.getAttribute("data-jupyter-widgets-cdn") || Cp, Sp = Sp || e.hasAttribute("data-jupyter-widgets-cdn-only")
         })), __webpack_require__(86801).i8;
-        class Bp {
+        const Dp = self.Bokeh.loader["@bokehjs/core/util/object"];
+        class Ap {
             constructor(e, t) {
                 this.CONNECTING = 0, this.OPEN = 1, this.CLOSING = 2, this.CLOSED = 3, this.onclose = null, this.onerror = null, this.onmessage = null, this.onopen = null, this.url = e instanceof URL ? e.toString() : e
             }
             close(e, t) {
                 var n;
                 const r = new CloseEvent("close", {
                     code: e,
@@ -88139,17 +88111,17 @@
             removeEventListener(e, t, n) {
                 throw new Error("not implemented")
             }
             dispatchEvent(e) {
                 throw new Error("not implemented")
             }
         }
-        Bp.CONNECTING = 0, Bp.OPEN = 1, Bp.CLOSING = 2, Bp.CLOSED = 3;
-        let Up = 0;
-        class Fp extends fp {
+        Ap.CONNECTING = 0, Ap.OPEN = 1, Ap.CLOSING = 2, Ap.CLOSED = 3;
+        let Ip = 0;
+        class Np extends fp {
             bk_open(e) {
                 var t, n;
                 null != this.ws && (this.bk_send = e, null === (n = (t = this.ws).onopen) || void 0 === n || n.call(t, new Event("open")))
             }
             bk_recv(e) {
                 var t, n;
                 null != this.ws && (null === (n = (t = this.ws).onmessage) || void 0 === n || n.call(t, new MessageEvent("message", {
@@ -88170,30 +88142,30 @@
                             credentials: "same-origin"
                         },
                         fetch: async (e, t) => new Response("[]", {
                             status: 200
                         }),
                         Headers,
                         Request,
-                        WebSocket: class extends Bp {
+                        WebSocket: class extends Ap {
                             constructor(e, n) {
                                 super(e, n), t.ws = this
                             }
                             send(e) {
                                 var n;
                                 (0, jo.isString)(e) || e instanceof ArrayBuffer ? null === (n = t.bk_send) || void 0 === n || n.call(t, e) : console.error("only string and ArrayBuffer types are supported, got " + typeof e)
                             }
                         }
                     };
-                this.kernel_manager = new ia.KernelManager({
+                this.kernel_manager = new ra.KernelManager({
                     serverSettings: n
                 });
                 const r = {
                     name: "bokeh_kernel",
-                    id: "" + Up++
+                    id: "" + Ip++
                 };
                 this.kernel = this.kernel_manager.connectTo({
                     model: r,
                     handleComms: !0
                 }), this.kernel.registerCommTarget(this.comm_target_name, ((e, t) => {
                     const n = this._model_objs.get(t.content.comm_id);
                     if (null != n && !n.comm_live) {
@@ -88207,15 +88179,15 @@
                 t.comm = e, e.on_close(t._handle_comm_closed.bind(t)), e.on_msg(t._handle_comm_msg.bind(t)), t.comm_live = !0
             }
             async render(e, t) {
                 const {
                     spec: n,
                     state: r
                 } = e, i = r.state;
-                for (const [e, t] of(0, Po.entries)(i)) this._known_models.set(e, t);
+                for (const [e, t] of(0, Dp.entries)(i)) this._known_models.set(e, t);
                 try {
                     const e = await this.set_state(r);
                     for (const t of e) {
                         if (this._model_objs.has(t.model_id)) continue;
                         const e = await this._create_comm(this.comm_target_name, t.model_id);
                         this._attach_comm(e, t), this._model_objs.set(t.model_id, t), t.once("comm:close", (() => {
                             this._model_objs.delete(t.model_id)
@@ -88224,30 +88196,30 @@
                     const i = e.find((e => e.model_id == n.model_id));
                     if (null == i) return null;
                     const o = await this.create_view(i, {
                         el: t
                     });
                     return await this.display_view(o, t), o
                 } finally {
-                    for (const e of (0, Po.keys)(i)) this._known_models.delete(e)
+                    for (const e of (0, Dp.keys)(i)) this._known_models.delete(e)
                 }
             }
             async _create_comm(e, t, n, r, i) {
                 const o = (() => {
                     const n = e + t,
                         r = this._comms.get(n);
                     if (null != r) return r; {
                         const r = this.kernel.createComm(e, t);
                         return this._comms.set(n, r), r
                     }
                 })();
                 return o.open(n, r, i), new xt.services.Comm(o)
             }
             _get_comm_info() {
-                return Promise.resolve((0, Po.to_object)(this._known_models))
+                return Promise.resolve((0, Dp.to_object)(this._known_models))
             }
             async new_model(e, t) {
                 if (void 0 === t) {
                     const n = this._known_models,
                         {
                             model_id: r
                         } = e;
@@ -88258,50 +88230,45 @@
             }
             loadClass(e, i, o) {
                 return new Promise(((e, a) => {
                     "@jupyter-widgets/base" === i ? e(t) : "@jupyter-widgets/controls" === i ? e(n) : "@jupyter-widgets/output" === i ? e(r) : void 0 !== this.loader ? e(this.loader(i, o)) : a(`Could not load module ${i}@${o}`)
                 })).then((t => t[e] ? t[e] : Promise.reject(`Class ${e} not found in module ${i}@${o}`)))
             }
         }
-        var Wp;
-        const qp = new WeakMap;
-        class $p extends No.LayoutDOMView {
+        var zp;
+        const jp = new WeakMap;
+        class Op extends No.LayoutDOMView {
             constructor() {
                 super(...arguments), this.rendered = !1, this.ipy_view = null
             }
             get child_models() {
                 return []
             }
+            connect_signals() {
+                super.connect_signals(), new MutationObserver((e => {
+                    for (const t of e)
+                        for (const e of [...t.addedNodes, ...t.removedNodes])
+                            if (e instanceof HTMLStyleElement) {
+                                this._update_stylesheets();
+                                break
+                            }
+                })).observe(document.head, {
+                    childList: !0
+                })
+            }
             _ipy_stylesheets() {
                 const e = [];
-
-                function t(t) {
-                    const n = t.replace(/:root/g, ":host");
-                    e.push(new Io.InlineStyleSheet(n))
-                }
-                const n = (0, Po.values)(__webpack_module_cache__).filter((({
-                    id: e,
-                    exports: t
-                }) => e.endsWith(".css") && "default" in t)).filter((function(e) {
-                    const {
-                        exports: t
-                    } = e;
-                    return (0, jo.isObject)(t.default) && "use" in t.default
-                }));
-                for (const e of n) {
-                    const n = e.exports.default;
-                    try {
-                        n.use({
-                            handler: t
-                        })
-                    } catch (e) {
-                        console.error("failed to apply a stylesheet")
-                    }
-                }
-                return e
+                for (const t of document.head.children)
+                    if (t instanceof HTMLStyleElement) {
+                        const n = t.textContent;
+                        if (null != n) {
+                            const t = n.replace(/:root/g, ":host");
+                            e.push(new Io.InlineStyleSheet(t))
+                        }
+                    } return e
             }
             stylesheets() {
                 return [...super.stylesheets(), ...this._ipy_stylesheets()]
             }
             render() {
                 super.render(), this.container = (0, Io.div)({
                     style: "display: contents;"
@@ -88314,46 +88281,46 @@
             }
             async _render() {
                 if (null == this.ipy_view) {
                     const {
                         document: e
                     } = this.model;
                     (0, Oo.assert)(null != e, "document is null");
-                    const t = qp.get(e);
+                    const t = jp.get(e);
                     (0, Oo.assert)(null != t, "manager is null"), this.ipy_view = await t.render(this.model.bundle, this.container)
                 } else this.container.append(this.ipy_view.el);
                 null != this.ipy_view && this.ipy_view.trigger("displayed", this.ipy_view)
             }
         }
-        class Gp extends No.LayoutDOM {
+        class Pp extends No.LayoutDOM {
             constructor(e) {
                 super(e)
             }
             _doc_attached() {
                 const e = this.document;
-                if (!qp.has(e)) {
-                    const t = new Fp({
-                        loader: Yo(this.cdn)
+                if (!jp.has(e)) {
+                    const t = new Np({
+                        loader: Ho(this.cdn)
                     });
-                    qp.set(e, t), t.bk_open((t => {
+                    jp.set(e, t), t.bk_open((t => {
                         const n = new zo.MessageSentEvent(e, "ipywidgets_bokeh", t);
                         e._trigger_on_change(n)
                     })), e.on_message("ipywidgets_bokeh", (e => {
                         (0, jo.isString)(e) || e instanceof ArrayBuffer ? t.bk_recv(e) : console.error("expected a string or ArrayBuffer, got " + typeof e)
                     }))
                 }
             }
         }
-        Wp = Gp, Gp.__name__ = "IPyWidget", Gp.__module__ = "ipywidgets_bokeh.widget", Wp.prototype.default_view = $p, Wp.define((({
+        zp = Pp, Pp.__name__ = "IPyWidget", Pp.__module__ = "ipywidgets_bokeh.widget", zp.prototype.default_view = Op, zp.define((({
             Any: e,
             String: t
         }) => ({
             bundle: [e],
             cdn: [t, "https://unpkg.com"]
         })));
-        const Kp = self.Bokeh.loader["@bokehjs/base"],
-            Qp = window.define;
-        Qp("@jupyter-widgets/base", [], t), Qp("@lumino/widgets", [], e), Qp("@jupyter-widgets/controls", [], n), (0, Kp.register_models)({
-            IPyWidget: Gp
+        const Rp = self.Bokeh.loader["@bokehjs/base"],
+            Hp = window.define;
+        Hp("@jupyter-widgets/base", [], t), Hp("@lumino/widgets", [], e), Hp("@jupyter-widgets/controls", [], n), (0, Rp.register_models)({
+            IPyWidget: Pp
         })
     })(), self["@bokeh/ipywidgets_bokeh"] = __webpack_exports__
 })();
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/index.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/index.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/loader.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/loader.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.d.ts` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.d.ts`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.d.ts` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.d.ts`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import { ModelBundle } from "./manager";
 export declare class IPyWidgetView extends LayoutDOMView {
     container: HTMLDivElement;
     model: IPyWidget;
     private rendered;
     private ipy_view;
     get child_models(): UIElement[];
+    connect_signals(): void;
     protected _ipy_stylesheets(): StyleSheetLike[];
     stylesheets(): StyleSheetLike[];
     render(): void;
     has_finished(): boolean;
     _render(): Promise<void>;
 }
 export declare namespace IPyWidget {
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.js` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -7,24 +7,20 @@
     LayoutDOM,
     LayoutDOMView
 } from "@bokehjs/models/layouts/layout_dom";
 import {
     MessageSentEvent
 } from "@bokehjs/document/events";
 import {
-    isString,
-    isObject
+    isString
 } from "@bokehjs/core/util/types";
 import {
     assert
 } from "@bokehjs/core/util/assert";
 import {
-    values
-} from "@bokehjs/core/util/object";
-import {
     generate_require_loader
 } from "./loader";
 import {
     WidgetManager
 } from "./manager";
 const widget_managers = new WeakMap();
 export class IPyWidgetView extends LayoutDOMView {
@@ -32,54 +28,51 @@
         super(...arguments);
         this.rendered = false;
         this.ipy_view = null;
     }
     get child_models() {
         return [];
     }
+    connect_signals() {
+        super.connect_signals();
+        const observer = new MutationObserver((mutations) => {
+            for (const mutation of mutations) {
+                for (const node of [...mutation.addedNodes, ...mutation.removedNodes]) {
+                    if (node instanceof HTMLStyleElement) {
+                        this._update_stylesheets();
+                        break;
+                    }
+                }
+            }
+        });
+        observer.observe(document.head, {
+            childList: true
+        });
+    }
     _ipy_stylesheets() {
         const stylesheets = [];
-
-        function handler(raw_css) {
-            const css = raw_css.replace(/:root/g, ":host");
-            stylesheets.push(new InlineStyleSheet(css));
-        }
-
-        function is_StyleModule(module) {
-            const {
-                exports
-            } = module;
-            return isObject(exports.default) && "use" in exports.default;
-        }
-        const modules = values(__webpack_module_cache__);
-        const css_modules = modules.filter(({
-            id,
-            exports
-        }) => id.endsWith(".css") && "default" in exports);
-        const style_modules = css_modules.filter(is_StyleModule);
-        for (const module of style_modules) {
-            const style = module.exports.default;
-            try {
-                style.use({
-                    handler
-                });
-            } catch (_b) {
-                console.error("failed to apply a stylesheet");
+        for (const child of document.head.children) {
+            if (child instanceof HTMLStyleElement) {
+                const raw_css = child.textContent;
+                if (raw_css != null) {
+                    const css = raw_css.replace(/:root/g, ":host");
+                    stylesheets.push(new InlineStyleSheet(css));
+                }
             }
         }
         return stylesheets;
     }
     stylesheets() {
         return [...super.stylesheets(), ...this._ipy_stylesheets()];
     }
     render() {
         super.render();
         this.container = div({
             style: "display: contents;"
-        });
+        }); // ipywidgets' APIs require HTMLElement, not DocumentFragment
         this.shadow_el.append(this.container);
         this._render().then(() => {
             this.invalidate_layout(); // TODO: this may be overzealous; probably should be removed
             this.rendered = true;
             this.notify_finished();
         });
     }
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/kernel.py` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     def flush(self, *args):
         pass
 
 
 class BokehKernel(ipykernel.kernelbase.Kernel):
     implementation = 'ipython'
-    implementation_version = '1.4.0.dev2'
+    implementation_version = '1.4.0.dev3'
     banner = 'banner'
 
     shell_stream = Any(ShellStream(), allow_none=True)
 
     def __init__(self):
         super(BokehKernel, self).__init__()
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/package.json` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.4.0-dev.3'"}*

```diff
@@ -37,9 +37,9 @@
         "build": "tsc && webpack --mode=production",
         "clean": "rimraf dist",
         "dev": "tsc; webpack --mode=development",
         "lint": "eslint -c eslint.json src/**/*.ts",
         "prepack": "npm run clean && npm run build",
         "test": "echo 'TODO'"
     },
-    "version": "1.4.0-dev.2"
+    "version": "1.4.0-dev.3"
 }
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/widget.py` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/widget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/PKG-INFO` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets-bokeh
-Version: 1.4.0.dev2
+Version: 1.4.0.dev3
 Summary: Allows embedding of Jupyter widgets in Bokeh layouts.
 Home-page: https://github.com/bokeh/ipywidgets_bokeh
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/SOURCES.txt` & `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev2/setup.py` & `ipywidgets_bokeh-1.4.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "bokeh ==3.*", # TODO 3.2.dev1
     "ipywidgets ==8.*",
     "ipykernel ==6.*,!=6.18.0", # until ipywidgets 8.0.6
 ]
 
 setup_args = dict(
     name="ipywidgets_bokeh",
-    version="1.4.0.dev2",
+    version="1.4.0.dev3",
     install_requires=install_requires,
     python_requires=">=3.9",
     description="Allows embedding of Jupyter widgets in Bokeh layouts.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bokeh Team",
     author_email="info@bokeh.org",
```

