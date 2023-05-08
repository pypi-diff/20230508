# Comparing `tmp/takao-0.1.0.tar.gz` & `tmp/takao-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "takao-0.1.0.tar", max compression
+gzip compressed data, was "takao-0.1.1.tar", max compression
```

## Comparing `takao-0.1.0.tar` & `takao-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      679 2023-03-12 18:56:20.497597 takao-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1573 2023-03-12 18:56:08.718501 takao-0.1.0/README.md
--rw-r--r--   0        0        0     1271 2023-02-12 21:33:59.770761 takao-0.1.0/takao/__init__.py
--rw-r--r--   0        0        0     1062 2023-03-11 20:44:22.084027 takao-0.1.0/takao/layout.html
--rw-r--r--   0        0        0      264 2023-03-11 21:08:54.122579 takao-0.1.0/takao/partials/global-toc.jinja2
--rw-r--r--   0        0        0      215 2023-03-11 21:08:54.117570 takao-0.1.0/takao/partials/mobile-menubar.jinja2
--rw-r--r--   0        0        0      729 2023-03-11 21:08:54.147498 takao-0.1.0/takao/partials/page-nav.jinja2
--rw-r--r--   0        0        0      460 2023-03-11 21:08:54.162543 takao-0.1.0/takao/partials/prev-next.jinja2
--rw-r--r--   0        0        0       43 2023-03-11 21:08:54.097782 takao-0.1.0/takao/partials/readthedocs-menu.jinja2
--rw-r--r--   0        0        0   138764 2023-03-12 19:10:26.262893 takao-0.1.0/takao/static/Inter (web)/Inter-Black.woff
--rw-r--r--   0        0        0   102868 2023-03-12 19:10:26.263893 takao-0.1.0/takao/static/Inter (web)/Inter-Black.woff2
--rw-r--r--   0        0        0   146824 2023-03-12 19:10:26.264894 takao-0.1.0/takao/static/Inter (web)/Inter-BlackItalic.woff
--rw-r--r--   0        0        0   108752 2023-03-12 19:10:26.266893 takao-0.1.0/takao/static/Inter (web)/Inter-BlackItalic.woff2
--rw-r--r--   0        0        0   143208 2023-03-12 19:10:26.267894 takao-0.1.0/takao/static/Inter (web)/Inter-Bold.woff
--rw-r--r--   0        0        0   106140 2023-03-12 19:10:26.269893 takao-0.1.0/takao/static/Inter (web)/Inter-Bold.woff2
--rw-r--r--   0        0        0   151052 2023-03-12 19:10:26.270894 takao-0.1.0/takao/static/Inter (web)/Inter-BoldItalic.woff
--rw-r--r--   0        0        0   111808 2023-03-12 19:10:26.271894 takao-0.1.0/takao/static/Inter (web)/Inter-BoldItalic.woff2
--rw-r--r--   0        0        0   142920 2023-03-12 19:10:26.273894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBold.woff
--rw-r--r--   0        0        0   106108 2023-03-12 19:10:26.274894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBold.woff2
--rw-r--r--   0        0        0   150628 2023-03-12 19:10:26.276894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff
--rw-r--r--   0        0        0   111708 2023-03-12 19:10:26.277894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff2
--rw-r--r--   0        0        0   140724 2023-03-12 19:10:26.278894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLight.woff
--rw-r--r--   0        0        0   104232 2023-03-12 19:10:26.280894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLight.woff2
--rw-r--r--   0        0        0   149996 2023-03-12 19:10:26.281894 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLightItalic.woff
--rw-r--r--   0        0        0   111392 2023-03-12 19:10:26.283907 takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLightItalic.woff2
--rw-r--r--   0        0        0   245036 2023-03-12 19:10:26.284893 takao-0.1.0/takao/static/Inter (web)/Inter-italic.var.woff2
--rw-r--r--   0        0        0   144372 2023-03-12 19:10:26.285894 takao-0.1.0/takao/static/Inter (web)/Inter-Italic.woff
--rw-r--r--   0        0        0   106876 2023-03-12 19:10:26.287893 takao-0.1.0/takao/static/Inter (web)/Inter-Italic.woff2
--rw-r--r--   0        0        0   140632 2023-03-12 19:10:26.288895 takao-0.1.0/takao/static/Inter (web)/Inter-Light.woff
--rw-r--r--   0        0        0   104332 2023-03-12 19:10:26.289896 takao-0.1.0/takao/static/Inter (web)/Inter-Light.woff2
--rw-r--r--   0        0        0   150092 2023-03-12 19:10:26.291912 takao-0.1.0/takao/static/Inter (web)/Inter-LightItalic.woff
--rw-r--r--   0        0        0   111332 2023-03-12 19:10:26.292902 takao-0.1.0/takao/static/Inter (web)/Inter-LightItalic.woff2
--rw-r--r--   0        0        0   142552 2023-03-12 19:10:26.294909 takao-0.1.0/takao/static/Inter (web)/Inter-Medium.woff
--rw-r--r--   0        0        0   105924 2023-03-12 19:10:26.295895 takao-0.1.0/takao/static/Inter (web)/Inter-Medium.woff2
--rw-r--r--   0        0        0   150988 2023-03-12 19:10:26.296895 takao-0.1.0/takao/static/Inter (web)/Inter-MediumItalic.woff
--rw-r--r--   0        0        0   112184 2023-03-12 19:10:26.297895 takao-0.1.0/takao/static/Inter (web)/Inter-MediumItalic.woff2
--rw-r--r--   0        0        0   133844 2023-03-12 19:10:26.298895 takao-0.1.0/takao/static/Inter (web)/Inter-Regular.woff
--rw-r--r--   0        0        0    98868 2023-03-12 19:10:26.300907 takao-0.1.0/takao/static/Inter (web)/Inter-Regular.woff2
--rw-r--r--   0        0        0   227180 2023-03-12 19:10:26.301894 takao-0.1.0/takao/static/Inter (web)/Inter-roman.var.woff2
--rw-r--r--   0        0        0   142932 2023-03-12 19:10:26.303894 takao-0.1.0/takao/static/Inter (web)/Inter-SemiBold.woff
--rw-r--r--   0        0        0   105804 2023-03-12 19:10:26.304894 takao-0.1.0/takao/static/Inter (web)/Inter-SemiBold.woff2
--rw-r--r--   0        0        0   151180 2023-03-12 19:10:26.305895 takao-0.1.0/takao/static/Inter (web)/Inter-SemiBoldItalic.woff
--rw-r--r--   0        0        0   112048 2023-03-12 19:10:26.307893 takao-0.1.0/takao/static/Inter (web)/Inter-SemiBoldItalic.woff2
--rw-r--r--   0        0        0   135920 2023-03-12 19:10:26.308894 takao-0.1.0/takao/static/Inter (web)/Inter-Thin.woff
--rw-r--r--   0        0        0    99632 2023-03-12 19:10:26.309896 takao-0.1.0/takao/static/Inter (web)/Inter-Thin.woff2
--rw-r--r--   0        0        0   145480 2023-03-12 19:10:26.311910 takao-0.1.0/takao/static/Inter (web)/Inter-ThinItalic.woff
--rw-r--r--   0        0        0   106496 2023-03-12 19:10:26.312895 takao-0.1.0/takao/static/Inter (web)/Inter-ThinItalic.woff2
--rw-r--r--   0        0        0   324864 2023-03-12 19:10:26.313894 takao-0.1.0/takao/static/Inter (web)/Inter.var.woff2
--rw-r--r--   0        0        0     4366 2023-03-12 19:10:26.462415 takao-0.1.0/takao/static/Inter (web)/LICENSE.txt
--rw-r--r--   0        0        0    16700 2023-03-11 20:24:09.159245 takao-0.1.0/takao/static/takao.css
--rw-r--r--   0        0        0     1827 2023-03-12 19:10:27.992927 takao-0.1.0/takao/static/takao.js
--rw-r--r--   0        0        0      231 2023-02-13 21:21:35.804660 takao-0.1.0/takao/theme.conf
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 takao-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      679 2023-05-08 18:25:49.004760 takao-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1573 2023-03-12 18:56:08.718501 takao-0.1.1/README.md
+-rw-r--r--   0        0        0     1271 2023-02-12 21:33:59.770761 takao-0.1.1/takao/__init__.py
+-rw-r--r--   0        0        0     1062 2023-03-11 20:44:22.084027 takao-0.1.1/takao/layout.html
+-rw-r--r--   0        0        0      254 2023-05-08 18:15:27.278687 takao-0.1.1/takao/partials/global-toc.jinja2
+-rw-r--r--   0        0        0      215 2023-03-11 21:08:54.117570 takao-0.1.1/takao/partials/mobile-menubar.jinja2
+-rw-r--r--   0        0        0      683 2023-05-08 18:15:27.279687 takao-0.1.1/takao/partials/page-nav.jinja2
+-rw-r--r--   0        0        0      460 2023-03-11 21:08:54.162543 takao-0.1.1/takao/partials/prev-next.jinja2
+-rw-r--r--   0        0        0       43 2023-03-11 21:08:54.097782 takao-0.1.1/takao/partials/readthedocs-menu.jinja2
+-rw-r--r--   0        0        0   138764 2023-05-08 18:26:05.733503 takao-0.1.1/takao/static/Inter (web)/Inter-Black.woff
+-rw-r--r--   0        0        0   102868 2023-05-08 18:26:05.737504 takao-0.1.1/takao/static/Inter (web)/Inter-Black.woff2
+-rw-r--r--   0        0        0   146824 2023-05-08 18:26:05.740503 takao-0.1.1/takao/static/Inter (web)/Inter-BlackItalic.woff
+-rw-r--r--   0        0        0   108752 2023-05-08 18:26:05.743504 takao-0.1.1/takao/static/Inter (web)/Inter-BlackItalic.woff2
+-rw-r--r--   0        0        0   143208 2023-05-08 18:26:05.746504 takao-0.1.1/takao/static/Inter (web)/Inter-Bold.woff
+-rw-r--r--   0        0        0   106140 2023-05-08 18:26:05.749504 takao-0.1.1/takao/static/Inter (web)/Inter-Bold.woff2
+-rw-r--r--   0        0        0   151052 2023-05-08 18:26:05.753503 takao-0.1.1/takao/static/Inter (web)/Inter-BoldItalic.woff
+-rw-r--r--   0        0        0   111808 2023-05-08 18:26:05.756504 takao-0.1.1/takao/static/Inter (web)/Inter-BoldItalic.woff2
+-rw-r--r--   0        0        0   142920 2023-05-08 18:26:05.759504 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBold.woff
+-rw-r--r--   0        0        0   106108 2023-05-08 18:26:05.762503 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBold.woff2
+-rw-r--r--   0        0        0   150628 2023-05-08 18:26:05.765504 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff
+-rw-r--r--   0        0        0   111708 2023-05-08 18:26:05.768503 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff2
+-rw-r--r--   0        0        0   140724 2023-05-08 18:26:05.771504 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLight.woff
+-rw-r--r--   0        0        0   104232 2023-05-08 18:26:05.774505 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLight.woff2
+-rw-r--r--   0        0        0   149996 2023-05-08 18:26:05.777504 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLightItalic.woff
+-rw-r--r--   0        0        0   111392 2023-05-08 18:26:05.781503 takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLightItalic.woff2
+-rw-r--r--   0        0        0   245036 2023-05-08 18:26:05.784505 takao-0.1.1/takao/static/Inter (web)/Inter-italic.var.woff2
+-rw-r--r--   0        0        0   144372 2023-05-08 18:26:05.787504 takao-0.1.1/takao/static/Inter (web)/Inter-Italic.woff
+-rw-r--r--   0        0        0   106876 2023-05-08 18:26:05.790503 takao-0.1.1/takao/static/Inter (web)/Inter-Italic.woff2
+-rw-r--r--   0        0        0   140632 2023-05-08 18:26:05.809503 takao-0.1.1/takao/static/Inter (web)/Inter-Light.woff
+-rw-r--r--   0        0        0   104332 2023-05-08 18:26:05.812504 takao-0.1.1/takao/static/Inter (web)/Inter-Light.woff2
+-rw-r--r--   0        0        0   150092 2023-05-08 18:26:05.815503 takao-0.1.1/takao/static/Inter (web)/Inter-LightItalic.woff
+-rw-r--r--   0        0        0   111332 2023-05-08 18:26:05.819503 takao-0.1.1/takao/static/Inter (web)/Inter-LightItalic.woff2
+-rw-r--r--   0        0        0   142552 2023-05-08 18:26:05.822504 takao-0.1.1/takao/static/Inter (web)/Inter-Medium.woff
+-rw-r--r--   0        0        0   105924 2023-05-08 18:26:05.826503 takao-0.1.1/takao/static/Inter (web)/Inter-Medium.woff2
+-rw-r--r--   0        0        0   150988 2023-05-08 18:26:05.829504 takao-0.1.1/takao/static/Inter (web)/Inter-MediumItalic.woff
+-rw-r--r--   0        0        0   112184 2023-05-08 18:26:05.832503 takao-0.1.1/takao/static/Inter (web)/Inter-MediumItalic.woff2
+-rw-r--r--   0        0        0   133844 2023-05-08 18:26:05.836504 takao-0.1.1/takao/static/Inter (web)/Inter-Regular.woff
+-rw-r--r--   0        0        0    98868 2023-05-08 18:26:05.839503 takao-0.1.1/takao/static/Inter (web)/Inter-Regular.woff2
+-rw-r--r--   0        0        0   227180 2023-05-08 18:26:05.842503 takao-0.1.1/takao/static/Inter (web)/Inter-roman.var.woff2
+-rw-r--r--   0        0        0   142932 2023-05-08 18:26:05.845503 takao-0.1.1/takao/static/Inter (web)/Inter-SemiBold.woff
+-rw-r--r--   0        0        0   105804 2023-05-08 18:26:05.848503 takao-0.1.1/takao/static/Inter (web)/Inter-SemiBold.woff2
+-rw-r--r--   0        0        0   151180 2023-05-08 18:26:05.851503 takao-0.1.1/takao/static/Inter (web)/Inter-SemiBoldItalic.woff
+-rw-r--r--   0        0        0   112048 2023-05-08 18:26:05.854504 takao-0.1.1/takao/static/Inter (web)/Inter-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0   135920 2023-05-08 18:26:05.857503 takao-0.1.1/takao/static/Inter (web)/Inter-Thin.woff
+-rw-r--r--   0        0        0    99632 2023-05-08 18:26:05.860504 takao-0.1.1/takao/static/Inter (web)/Inter-Thin.woff2
+-rw-r--r--   0        0        0   145480 2023-05-08 18:26:05.863503 takao-0.1.1/takao/static/Inter (web)/Inter-ThinItalic.woff
+-rw-r--r--   0        0        0   106496 2023-05-08 18:26:05.866504 takao-0.1.1/takao/static/Inter (web)/Inter-ThinItalic.woff2
+-rw-r--r--   0        0        0   324864 2023-05-08 18:26:05.869504 takao-0.1.1/takao/static/Inter (web)/Inter.var.woff2
+-rw-r--r--   0        0        0     4366 2023-05-08 18:26:05.952504 takao-0.1.1/takao/static/Inter (web)/LICENSE.txt
+-rw-r--r--   0        0        0    16810 2023-05-08 18:26:05.306503 takao-0.1.1/takao/static/takao.css
+-rw-r--r--   0        0        0     1827 2023-05-08 18:26:09.707505 takao-0.1.1/takao/static/takao.js
+-rw-r--r--   0        0        0      231 2023-02-13 21:21:35.804660 takao-0.1.1/takao/theme.conf
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 takao-0.1.1/PKG-INFO
```

### Comparing `takao-0.1.0/pyproject.toml` & `takao-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "takao"
-version = "0.1.0"
+version = "0.1.1"
 description = "A dark theme for Sphinx."
 authors = ["Reupen Shah"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/reupen/takao"
 packages = [{include = "takao"}]
 include = ["takao/static/**/*"]
```

### Comparing `takao-0.1.0/README.md` & `takao-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/__init__.py` & `takao-0.1.1/takao/__init__.py`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/layout.html` & `takao-0.1.1/takao/layout.html`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/partials/page-nav.jinja2` & `takao-0.1.1/takao/partials/page-nav.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
       {%- for item in page_nav_items -%}
         <li>
           <a href="{{ item.href }}" class="page-nav-link">{{ item.title }}</a>
           {%- if item.children -%}
             <ul>
               {%- for subitem in item.children -%}
                 <li>
-                  <a href="{{ subitem.href }}" class="page-nav-link">{{ subitem.title }}</a
-                    >
-                  </li>
-                {%- endfor -%}
-              </ul>
-            {%- endif -%}
-          </li>
-        {%- endfor -%}
-      </ul>
-    {%- endif -%}
-    <p>
-      <a href="#top">Back to top</a>
-    </p>
-  </div>
+                  <a href="{{ subitem.href }}" class="page-nav-link">{{ subitem.title }}</a>
+                </li>
+              {%- endfor -%}
+            </ul>
+          {%- endif -%}
+        </li>
+      {%- endfor -%}
+    </ul>
+  {%- endif -%}
+  <p>
+    <a href="#top">Back to top</a>
+  </p>
+</div>
```

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Black.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Black.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Black.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Black.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-BlackItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-BlackItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Bold.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Bold.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Bold.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Bold.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-BoldItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-BoldItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBold.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBold.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLight.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLight.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLight.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLight.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLightItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLightItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ExtraLightItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-ExtraLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-italic.var.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Italic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Italic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Italic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Italic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Light.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Light.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Light.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Light.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-LightItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-LightItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Medium.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Medium.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Medium.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Medium.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-MediumItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-MediumItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Regular.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Regular.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Regular.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-roman.var.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-SemiBold.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-SemiBold.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-SemiBoldItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-SemiBoldItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Thin.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-Thin.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-Thin.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-Thin.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ThinItalic.woff` & `takao-0.1.1/takao/static/Inter (web)/Inter-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter-ThinItalic.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/Inter.var.woff2` & `takao-0.1.1/takao/static/Inter (web)/Inter.var.woff2`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/Inter (web)/LICENSE.txt` & `takao-0.1.1/takao/static/Inter (web)/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/takao/static/takao.css` & `takao-0.1.1/takao/static/takao.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-:root{--text-accent-colour:#fb660a;--admonition-default-accent:#0e4f68;--admonition-default-background:rgba(14,79,104,.18);--admonition-attention-accent:var(--admonition-important-accent);--admonition-attention-background:var(--admonition-important-background);--admonition-caution-accent:#663900;--admonition-caution-background:rgba(102,57,0,.18);--admonition-danger-accent:#5f0000;--admonition-danger-background:rgba(95,0,0,.18);--admonition-error-accent:var(--admonition-danger-accent);--admonition-error-background:var(--admonition-danger-background);--admonition-hint-accent:#094819;--admonition-hint-background:rgba(9,72,25,.18);--admonition-important-accent:#4c1b6e;--admonition-important-background:rgba(76,27,110,.18);--admonition-note-accent:#155d5a;--admonition-note-background:rgba(21,93,90,.18);--admonition-seealso-accent:#344c23;--admonition-seealso-background:rgba(52,76,35,.18);--admonition-tip-accent:var(--admonition-hint-accent);--admonition-tip-background:var(--admonition-hint-background);--admonition-warning-accent:var(--admonition-caution-accent);--admonition-warning-background:var(--admonition-caution-background);font-family:Inter,sans-serif}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100;src:url("Inter (web)/Inter-Thin.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Thin.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100;src:url("Inter (web)/Inter-ThinItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ThinItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:200;src:url("Inter (web)/Inter-ExtraLight.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraLight.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:200;src:url("Inter (web)/Inter-ExtraLightItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraLightItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:300;src:url("Inter (web)/Inter-Light.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Light.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:300;src:url("Inter (web)/Inter-LightItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-LightItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:400;src:url("Inter (web)/Inter-Regular.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Regular.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:400;src:url("Inter (web)/Inter-Italic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Italic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:500;src:url("Inter (web)/Inter-Medium.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Medium.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:500;src:url("Inter (web)/Inter-MediumItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-MediumItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:600;src:url("Inter (web)/Inter-SemiBold.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-SemiBold.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:600;src:url("Inter (web)/Inter-SemiBoldItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-SemiBoldItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:700;src:url("Inter (web)/Inter-Bold.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Bold.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:700;src:url("Inter (web)/Inter-BoldItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-BoldItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:800;src:url("Inter (web)/Inter-ExtraBold.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraBold.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:800;src:url("Inter (web)/Inter-ExtraBoldItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraBoldItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:900;src:url("Inter (web)/Inter-Black.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Black.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:900;src:url("Inter (web)/Inter-BlackItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-BlackItalic.woff?v=3.19") format("woff")}@font-face{font-named-instance:"Regular";font-display:swap;font-family:Inter var;font-style:normal;font-weight:100 900;src:url("Inter (web)/Inter-roman.var.woff2?v=3.19") format("woff2 supports variations(gvar)"),url("Inter (web)/Inter-roman.var.woff2?v=3.19") format("woff2-variations"),url("Inter (web)/Inter-roman.var.woff2?v=3.19") format("woff2")}@font-face{font-named-instance:"Italic";font-display:swap;font-family:Inter var;font-style:italic;font-weight:100 900;src:url("Inter (web)/Inter-italic.var.woff2?v=3.19") format("woff2 supports variations(gvar)"),url("Inter (web)/Inter-italic.var.woff2?v=3.19") format("woff2-variations"),url("Inter (web)/Inter-italic.var.woff2?v=3.19") format("woff2")}@font-face{font-display:swap;font-family:Inter var experimental;font-style:oblique 0deg 10deg;font-weight:100 900;src:url("Inter (web)/Inter.var.woff2?v=3.19") format("woff2-variations"),url("Inter (web)/Inter.var.woff2?v=3.19") format("woff2")}@supports (font-variation-settings:normal){:root{font-family:Inter var,sans-serif}}*,:after,:before{box-sizing:border-box}html{font-size:16px}body{background:#1e1e1e;color:#fff;display:flex;margin:0}code{font-size:15px}h1,h2,h3,h4,h5,h6{margin:0}h1{font-size:36px;margin-bottom:25px}h2{font-size:30px}h2,h3{margin-bottom:20px}h3{font-size:24px}h4{font-size:20px;margin-bottom:15px}h5{font-size:18px}h5,h6{margin-bottom:10px}h6{font-size:16px}p{line-height:1.75;margin:0 0 1rem}li p{margin:0}a{-webkit-text-decoration:none;text-decoration:none}a,a :visited{color:#ebebeb}a:hover{-webkit-text-decoration:underline;text-decoration:underline}pre{border:1px solid #333;border-radius:2px;font-size:15px;overflow:auto;padding:.625rem}code{background:#333;border:1px solid #444;border-radius:2px;padding:0 3px;word-break:break-word}button,input{background:#000;border:1px solid #777;border-radius:5px;color:#fff;font-size:16px;padding:.325rem}button:focus,input:focus{outline:1px solid #fb660a;outline:1px solid var(--text-accent-colour)}html.overlay-active{overflow-y:hidden}.visually-hidden{clip:rect(0 0 0 0);-webkit-clip-path:inset(50%);clip-path:inset(50%);height:1px;overflow:hidden;position:absolute;white-space:nowrap;width:1px}.spacer{flex:1}.root-left{background:#000}.root-left,.root-right{flex:1 1 auto}.root{margin:0 auto;max-width:1300px;width:100%}.content{height:100%}@media (min-width:800px){.content{display:flex}.content-main{flex:1;overflow-x:hidden}}.blur-overlay{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);background:hsla(0,0%,8%,.67);height:100%;left:0;position:fixed;top:0;width:100%;z-index:1000}.sidebar-container{background:#000;height:100vh;height:100dvh;left:0;max-width:100vw;opacity:.5;overflow-y:auto;padding:1rem 1rem 2rem;position:fixed;top:0;transform:translateX(-100%);transition:opacity .1s,transform .25s cubic-bezier(.165,.84,.44,1);width:-moz-fit-content;width:fit-content}.sidebar-container.open{opacity:1;transform:translateX(0);z-index:2000}@media (min-width:800px){.sidebar-container{flex:0 0 275px;opacity:1;padding:1.5rem 2rem;position:sticky;transform:translateX(0)}}@media print{.sidebar-container{display:none}}.sphinxsidebarwrapper a.current{color:#fb660a}.sphinxsidebarwrapper .caption{font-weight:600;margin:2.5rem 0 0}.sphinxsidebarwrapper>ul{margin-top:.425rem}.sphinxsidebarwrapper>ul>li:first-child{margin-top:.3rem}.sphinxsidebarwrapper ul{list-style:none;margin:0;padding:0}.sphinxsidebarwrapper ul ul{margin-left:.75rem}.sphinxsidebarwrapper li{margin:.6rem 0}.sphinxsidebarwrapper #searchbox{margin-top:3rem}.sphinxsidebarwrapper .search{display:flex}.sphinxsidebarwrapper .search :first-child{flex:1;margin-right:.4rem;min-width:0}.mobile-menubar{align-items:center;-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);background:rgba(0,0,0,.51);display:flex;padding:.5rem 1rem;position:sticky;top:0}@media (min-width:800px){.mobile-menubar{display:none}}@media print{.mobile-menubar{display:none}}.mobile-menubar button{margin:0}.document{overflow-x:hidden;padding:1.5rem 1rem}@media (min-width:800px){.document{overflow-x:auto;padding:1.5rem 2rem}}.document button,.document input{margin-bottom:2rem}.document li,.document p{line-height:1.75}.document .toctree-wrapper .caption{font-size:24px;font-weight:700}.document .toctree-wrapper ul{list-style-type:none;padding-left:0}.document .toctree-wrapper ul ul,.document ol,.document ul{padding-left:1.625rem}.document li{padding-left:.125rem}.document ol .loweralpha{list-style:lower-alpha}.document ol .lowerroman{list-style:lower-roman}.document ol .upperalpha{list-style:upper-alpha}.document ol .upperroman{list-style:upper-roman}.document a{color:#fb660a}.document section{margin-bottom:3rem}.document section section{margin:3rem 0}.document section section section{margin:2.5rem 0}.document section section section:first-of-type{margin-top:1.5rem}.document dt{background:#333;border:1px solid #444;border-radius:2px;line-height:1.75;padding:0 6px}.document dd,.document dt{margin-bottom:.75rem;word-break:break-word}.document dd{margin-left:1.625rem;margin-top:.75rem}.document dd p{margin-bottom:.75rem}.document dd p+.admonition{margin-top:.75rem}.document dl{margin-top:1rem}.document dl ol,.document dl ul{margin-left:0;padding-left:1.25rem}.document dl ol p,.document dl ul p{margin:0;padding:2px 0}.document table{border-collapse:collapse;margin:1.5rem 0}.document table th{font-weight:600;text-align:left}.document table tr{border-bottom:1px solid #9e9a9a}.document table td,.document table th{padding:.25rem .5rem}.document table td:first-child,.document table th:first-child{padding-left:0}.document table td:last-child,.document table th:last-child{padding-right:0}.document table td>:last-child,.document table th>:last-child{margin-bottom:0}.document table thead th{padding-top:0}.document table tbody tr:last-child{border-bottom:none}.document table tbody tr:last-child td{padding-bottom:0}.document .caption-text,.document .rubric{font-weight:600}.document .code-block-caption+* pre{margin-top:.5rem}.headerlink{margin-left:.25rem}*>.headerlink{visibility:hidden}:hover>.headerlink{visibility:visible}.sig-name{color:#ff0086;font-family:ui-monospace,monospace}.prev-next-links{grid-column-gap:1rem;grid-row-gap:1rem;-moz-column-gap:1rem;column-gap:1rem;display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));row-gap:1rem}@media print{.prev-next-links{display:none}}.prev-next-links>span{display:block;visibility:hidden}.prev-next-links>a{border:1px solid #555;border-radius:5px;display:block;line-height:1.65;padding:.5rem 1rem}.prev-next-links>a:hover{border-color:#fb660a;border-color:var(--text-accent-colour);-webkit-text-decoration:none;text-decoration:none}.prev-next-links .next-page{text-align:right}.prev-next-caption{color:#ebebeb;display:block}.document .admonition{background:rgba(14,79,104,.18);background:var(--admonition-default-background);border:1px solid #0e4f68;border:1px solid var(--admonition-default-accent);border-radius:2px;margin:1rem 0}.document .admonition>p{margin:0}.document .admonition>p:not(:empty):not(.admonition-title){padding:2px 7px}.document .admonition>p:last-child{margin-bottom:.25rem}.document .admonition ol,.document .admonition ul{padding-left:1.75rem}.document .admonition .admonition-title{background:#0e4f68;background:var(--admonition-default-accent);border-radius:2px 2px 0 0;margin-bottom:.25rem;padding:1px 7px}.document .admonition.attention{background:rgba(76,27,110,.18);background:var(--admonition-attention-background);border-color:#4c1b6e;border-color:var(--admonition-attention-accent)}.document .admonition.attention .admonition-title{background:#4c1b6e;background:var(--admonition-attention-accent)}.document .admonition.caution{background:rgba(102,57,0,.18);background:var(--admonition-caution-background);border-color:#663900;border-color:var(--admonition-caution-accent)}.document .admonition.caution .admonition-title{background:#663900;background:var(--admonition-caution-accent)}.document .admonition.danger{background:rgba(95,0,0,.18);background:var(--admonition-danger-background);border-color:#5f0000;border-color:var(--admonition-danger-accent)}.document .admonition.danger .admonition-title{background:#5f0000;background:var(--admonition-danger-accent)}.document .admonition.error{background:rgba(95,0,0,.18);background:var(--admonition-error-background);border-color:#5f0000;border-color:var(--admonition-error-accent)}.document .admonition.error .admonition-title{background:#5f0000;background:var(--admonition-error-accent)}.document .admonition.hint{background:rgba(9,72,25,.18);background:var(--admonition-hint-background);border-color:#094819;border-color:var(--admonition-hint-accent)}.document .admonition.hint .admonition-title{background:#094819;background:var(--admonition-hint-accent)}.document .admonition.important{background:rgba(76,27,110,.18);background:var(--admonition-important-background);border-color:#4c1b6e;border-color:var(--admonition-important-accent)}.document .admonition.important .admonition-title{background:#4c1b6e;background:var(--admonition-important-accent)}.document .admonition.note{background:rgba(21,93,90,.18);background:var(--admonition-note-background);border-color:#155d5a;border-color:var(--admonition-note-accent)}.document .admonition.note .admonition-title{background:#155d5a;background:var(--admonition-note-accent)}.document .admonition.seealso{background:rgba(52,76,35,.18);background:var(--admonition-seealso-background);border-color:#344c23;border-color:var(--admonition-seealso-accent)}.document .admonition.seealso .admonition-title{background:#344c23;background:var(--admonition-seealso-accent)}.document .admonition.tip{background:rgba(9,72,25,.18);background:var(--admonition-tip-background);border-color:#094819;border-color:var(--admonition-tip-accent)}.document .admonition.tip .admonition-title{background:#094819;background:var(--admonition-tip-accent)}.document .admonition.warning{background:rgba(102,57,0,.18);background:var(--admonition-warning-background);border-color:#663900;border-color:var(--admonition-warning-accent)}.document .admonition.warning .admonition-title{background:#663900;background:var(--admonition-warning-accent)}.localtoc{display:none}@media screen and (min-width:1150px){.localtoc{display:block;flex:0 0 225px;font-size:14px;height:100vh;overflow-y:auto;padding:1.5rem 2rem 1.5rem 0;position:sticky;top:0}}.localtoc ul{list-style:none;margin:.125rem 0 0;padding:0}.localtoc li a{display:inline-block;padding:.3rem 0}.localtoc li li a{padding-left:.75rem}.localtoc li a{color:#b8b8b8;font-weight:500;position:relative}.localtoc p{margin:0}.localtoc .caption,.localtoc>ul{margin-bottom:.5rem}.localtoc>ul{margin-left:13px;position:relative}.localtoc>ul:after{background:#444;bottom:.15rem;content:"";left:-11px;position:absolute;top:.15rem;width:1px;z-index:1000}.localtoc li a.current{color:#fff}.localtoc li a.current:after{background:#fb660a;background:var(--text-accent-colour);bottom:.3rem;content:"";left:-11.5px;position:absolute;top:.3rem;width:2px;z-index:2000}#readthedocs-embed-flyout .rst-versions{border:1px solid #555;border-radius:5px;margin-top:3rem;position:static;width:calc(300px - 4rem)}#readthedocs-embed-flyout .rst-versions .rst-current-version{border-radius:5px;padding:0 .75rem}#readthedocs-embed-flyout .rst-versions .rst-other-versions dl+dl{margin-top:.9rem}#readthedocs-embed-flyout .rst-versions .rst-other-versions>dl:last-of-type>dd{width:100%}#readthedocs-embed-flyout .rst-versions .rst-other-versions dd a{padding:.375rem .375rem 0 0}#readthedocs-embed-flyout .rst-versions .rst-other-versions dd>div{padding:.375rem .375rem 0 0!important}#readthedocs-embed-flyout .rst-versions .rst-other-versions input{width:100%}
+:root{--fixed-sidebar-width:275px;--text-accent-colour:#fb660a;--admonition-default-accent:#0e4f68;--admonition-default-background:rgba(14,79,104,.18);--admonition-attention-accent:var(--admonition-important-accent);--admonition-attention-background:var(--admonition-important-background);--admonition-caution-accent:#663900;--admonition-caution-background:rgba(102,57,0,.18);--admonition-danger-accent:#5f0000;--admonition-danger-background:rgba(95,0,0,.18);--admonition-error-accent:var(--admonition-danger-accent);--admonition-error-background:var(--admonition-danger-background);--admonition-hint-accent:#094819;--admonition-hint-background:rgba(9,72,25,.18);--admonition-important-accent:#4c1b6e;--admonition-important-background:rgba(76,27,110,.18);--admonition-note-accent:#155d5a;--admonition-note-background:rgba(21,93,90,.18);--admonition-seealso-accent:#344c23;--admonition-seealso-background:rgba(52,76,35,.18);--admonition-tip-accent:var(--admonition-hint-accent);--admonition-tip-background:var(--admonition-hint-background);--admonition-warning-accent:var(--admonition-caution-accent);--admonition-warning-background:var(--admonition-caution-background);font-family:Inter,sans-serif}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:100;src:url("Inter (web)/Inter-Thin.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Thin.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:100;src:url("Inter (web)/Inter-ThinItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ThinItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:200;src:url("Inter (web)/Inter-ExtraLight.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraLight.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:200;src:url("Inter (web)/Inter-ExtraLightItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraLightItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:300;src:url("Inter (web)/Inter-Light.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Light.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:300;src:url("Inter (web)/Inter-LightItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-LightItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:400;src:url("Inter (web)/Inter-Regular.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Regular.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:400;src:url("Inter (web)/Inter-Italic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Italic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:500;src:url("Inter (web)/Inter-Medium.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Medium.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:500;src:url("Inter (web)/Inter-MediumItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-MediumItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:600;src:url("Inter (web)/Inter-SemiBold.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-SemiBold.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:600;src:url("Inter (web)/Inter-SemiBoldItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-SemiBoldItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:700;src:url("Inter (web)/Inter-Bold.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Bold.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:700;src:url("Inter (web)/Inter-BoldItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-BoldItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:800;src:url("Inter (web)/Inter-ExtraBold.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraBold.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:800;src:url("Inter (web)/Inter-ExtraBoldItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-ExtraBoldItalic.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:normal;font-weight:900;src:url("Inter (web)/Inter-Black.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-Black.woff?v=3.19") format("woff")}@font-face{font-display:swap;font-family:Inter;font-style:italic;font-weight:900;src:url("Inter (web)/Inter-BlackItalic.woff2?v=3.19") format("woff2"),url("Inter (web)/Inter-BlackItalic.woff?v=3.19") format("woff")}@font-face{font-named-instance:"Regular";font-display:swap;font-family:Inter var;font-style:normal;font-weight:100 900;src:url("Inter (web)/Inter-roman.var.woff2?v=3.19") format("woff2 supports variations(gvar)"),url("Inter (web)/Inter-roman.var.woff2?v=3.19") format("woff2-variations"),url("Inter (web)/Inter-roman.var.woff2?v=3.19") format("woff2")}@font-face{font-named-instance:"Italic";font-display:swap;font-family:Inter var;font-style:italic;font-weight:100 900;src:url("Inter (web)/Inter-italic.var.woff2?v=3.19") format("woff2 supports variations(gvar)"),url("Inter (web)/Inter-italic.var.woff2?v=3.19") format("woff2-variations"),url("Inter (web)/Inter-italic.var.woff2?v=3.19") format("woff2")}@font-face{font-display:swap;font-family:Inter var experimental;font-style:oblique 0deg 10deg;font-weight:100 900;src:url("Inter (web)/Inter.var.woff2?v=3.19") format("woff2-variations"),url("Inter (web)/Inter.var.woff2?v=3.19") format("woff2")}@supports (font-variation-settings:normal){:root{font-family:Inter var,sans-serif}}*,:after,:before{box-sizing:border-box}html{font-size:16px}body{background:#1e1e1e;color:#fff;display:flex;margin:0}code{font-size:15px}h1,h2,h3,h4,h5,h6{margin:0}h1{font-size:36px;margin-bottom:25px}h2{font-size:30px}h2,h3{margin-bottom:20px}h3{font-size:24px}h4{font-size:20px;margin-bottom:15px}h5{font-size:18px}h5,h6{margin-bottom:10px}h6{font-size:16px}p{line-height:1.75;margin:0 0 1rem}li p{margin:0}a{-webkit-text-decoration:none;text-decoration:none}a,a :visited{color:#ebebeb}a:hover{-webkit-text-decoration:underline;text-decoration:underline}pre{border:1px solid #333;border-radius:2px;font-size:15px;overflow:auto;padding:.625rem}code{background:#333;border:1px solid #444;border-radius:2px;padding:0 3px;word-break:break-word}button,input{background:#000;border:1px solid #777;border-radius:5px;color:#fff;font-size:16px;padding:.325rem}button:focus,input:focus{outline:1px solid #fb660a;outline:1px solid var(--text-accent-colour)}html.overlay-active{overflow-y:hidden}.visually-hidden{clip:rect(0 0 0 0);-webkit-clip-path:inset(50%);clip-path:inset(50%);height:1px;overflow:hidden;position:absolute;white-space:nowrap;width:1px}.spacer{flex:1}.root-left{background:#000}.root-left,.root-right{flex:1 1 auto}.root{margin:0 auto;max-width:1300px;width:100%}.content{height:100%}@media (min-width:800px){.content{display:flex}.content-main{flex:1;overflow-x:hidden}}.blur-overlay{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);background:hsla(0,0%,8%,.67);height:100%;left:0;position:fixed;top:0;width:100%;z-index:1000}.sidebar-container{background:#000;height:100vh;height:100dvh;left:0;max-width:100vw;opacity:.5;overflow-y:auto;padding:1rem 1rem 2rem;position:fixed;top:0;transform:translateX(-100%);transition:opacity .1s,transform .25s cubic-bezier(.165,.84,.44,1);width:-moz-fit-content;width:fit-content}.sidebar-container.open{opacity:1;transform:translateX(0);z-index:2000}@media (min-width:800px){.sidebar-container{flex:0 0 275px;flex:0 0 var(--fixed-sidebar-width);opacity:1;padding:1.5rem 2rem;position:sticky;transform:translateX(0)}}@media print{.sidebar-container{display:none}}.sphinxsidebarwrapper a.current{color:#fb660a}.sphinxsidebarwrapper .caption{font-weight:600;margin:2.5rem 0 0}.sphinxsidebarwrapper>ul{margin-top:.425rem}.sphinxsidebarwrapper>ul>li:first-child{margin-top:.3rem}.sphinxsidebarwrapper ul{list-style:none;margin:0;padding:0}.sphinxsidebarwrapper ul ul{margin-left:.75rem}.sphinxsidebarwrapper li{margin:.6rem 0}.sphinxsidebarwrapper #searchbox{margin-top:3rem}.sphinxsidebarwrapper .search{display:flex}.sphinxsidebarwrapper .search :first-child{flex:1;margin-right:.4rem;min-width:0}.mobile-menubar{align-items:center;-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);background:rgba(0,0,0,.51);display:flex;padding:.5rem 1rem;position:sticky;top:0}@media (min-width:800px){.mobile-menubar{display:none}}@media print{.mobile-menubar{display:none}}.mobile-menubar button{margin:0}.document{overflow-x:hidden;padding:1.5rem 1rem}@media (min-width:800px){.document{overflow-x:auto;padding:1.5rem 2rem}}.document button,.document input{margin-bottom:2rem}.document li,.document p{line-height:1.75}.document .toctree-wrapper .caption{font-size:24px;font-weight:700}.document .toctree-wrapper ul{list-style-type:none;padding-left:0}.document .toctree-wrapper ul ul,.document ol,.document ul{padding-left:1.625rem}.document li{padding-left:.125rem}.document ol .loweralpha{list-style:lower-alpha}.document ol .lowerroman{list-style:lower-roman}.document ol .upperalpha{list-style:upper-alpha}.document ol .upperroman{list-style:upper-roman}.document a{color:#fb660a}.document section{margin-bottom:3rem}.document section section{margin:3rem 0}.document section section section{margin:2.5rem 0}.document section section section:first-of-type{margin-top:1.5rem}.document dt{background:#333;border:1px solid #444;border-radius:2px;line-height:1.75;padding:0 6px}.document dd,.document dt{margin-bottom:.75rem;word-break:break-word}.document dd{margin-left:1.625rem;margin-top:.75rem}.document dd p{margin-bottom:.75rem}.document dd p+.admonition{margin-top:.75rem}.document dl{margin-top:1rem}.document dl ol,.document dl ul{margin-left:0;padding-left:1.25rem}.document dl ol p,.document dl ul p{margin:0;padding:2px 0}.document table{border-collapse:collapse;margin:1.5rem 0}.document table th{font-weight:600;text-align:left}.document table tr{border-bottom:1px solid #9e9a9a}.document table td,.document table th{padding:.25rem .5rem}.document table td:first-child,.document table th:first-child{padding-left:0}.document table td:last-child,.document table th:last-child{padding-right:0}.document table td>:last-child,.document table th>:last-child{margin-bottom:0}.document table thead th{padding-top:0}.document table tbody tr:last-child{border-bottom:none}.document table tbody tr:last-child td{padding-bottom:0}.document .caption-text,.document .rubric{font-weight:600}.document .code-block-caption+* pre{margin-top:.5rem}.headerlink{margin-left:.25rem}*>.headerlink{visibility:hidden}:hover>.headerlink{visibility:visible}.sig-name{color:#ff0086;font-family:ui-monospace,monospace}.prev-next-links{grid-column-gap:1rem;grid-row-gap:1rem;-moz-column-gap:1rem;column-gap:1rem;display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));row-gap:1rem}@media print{.prev-next-links{display:none}}.prev-next-links>span{display:block;visibility:hidden}.prev-next-links>a{border:1px solid #555;border-radius:5px;display:block;line-height:1.65;padding:.5rem 1rem}.prev-next-links>a:hover{border-color:#fb660a;border-color:var(--text-accent-colour);-webkit-text-decoration:none;text-decoration:none}.prev-next-links .next-page{text-align:right}.prev-next-caption{color:#ebebeb;display:block}.document .admonition{background:rgba(14,79,104,.18);background:var(--admonition-default-background);border:1px solid #0e4f68;border:1px solid var(--admonition-default-accent);border-radius:2px;margin:1rem 0}.document .admonition>p{margin:0}.document .admonition>p:not(:empty):not(.admonition-title){padding:2px 7px}.document .admonition>p:last-child{margin-bottom:.25rem}.document .admonition ol,.document .admonition ul{padding-left:1.75rem}.document .admonition .admonition-title{background:#0e4f68;background:var(--admonition-default-accent);border-radius:2px 2px 0 0;margin-bottom:.25rem;padding:1px 7px}.document .admonition.attention{background:rgba(76,27,110,.18);background:var(--admonition-attention-background);border-color:#4c1b6e;border-color:var(--admonition-attention-accent)}.document .admonition.attention .admonition-title{background:#4c1b6e;background:var(--admonition-attention-accent)}.document .admonition.caution{background:rgba(102,57,0,.18);background:var(--admonition-caution-background);border-color:#663900;border-color:var(--admonition-caution-accent)}.document .admonition.caution .admonition-title{background:#663900;background:var(--admonition-caution-accent)}.document .admonition.danger{background:rgba(95,0,0,.18);background:var(--admonition-danger-background);border-color:#5f0000;border-color:var(--admonition-danger-accent)}.document .admonition.danger .admonition-title{background:#5f0000;background:var(--admonition-danger-accent)}.document .admonition.error{background:rgba(95,0,0,.18);background:var(--admonition-error-background);border-color:#5f0000;border-color:var(--admonition-error-accent)}.document .admonition.error .admonition-title{background:#5f0000;background:var(--admonition-error-accent)}.document .admonition.hint{background:rgba(9,72,25,.18);background:var(--admonition-hint-background);border-color:#094819;border-color:var(--admonition-hint-accent)}.document .admonition.hint .admonition-title{background:#094819;background:var(--admonition-hint-accent)}.document .admonition.important{background:rgba(76,27,110,.18);background:var(--admonition-important-background);border-color:#4c1b6e;border-color:var(--admonition-important-accent)}.document .admonition.important .admonition-title{background:#4c1b6e;background:var(--admonition-important-accent)}.document .admonition.note{background:rgba(21,93,90,.18);background:var(--admonition-note-background);border-color:#155d5a;border-color:var(--admonition-note-accent)}.document .admonition.note .admonition-title{background:#155d5a;background:var(--admonition-note-accent)}.document .admonition.seealso{background:rgba(52,76,35,.18);background:var(--admonition-seealso-background);border-color:#344c23;border-color:var(--admonition-seealso-accent)}.document .admonition.seealso .admonition-title{background:#344c23;background:var(--admonition-seealso-accent)}.document .admonition.tip{background:rgba(9,72,25,.18);background:var(--admonition-tip-background);border-color:#094819;border-color:var(--admonition-tip-accent)}.document .admonition.tip .admonition-title{background:#094819;background:var(--admonition-tip-accent)}.document .admonition.warning{background:rgba(102,57,0,.18);background:var(--admonition-warning-background);border-color:#663900;border-color:var(--admonition-warning-accent)}.document .admonition.warning .admonition-title{background:#663900;background:var(--admonition-warning-accent)}.localtoc{display:none}@media screen and (min-width:1150px){.localtoc{display:block;flex:0 0 225px;font-size:14px;height:100vh;overflow-y:auto;padding:1.5rem 2rem 1.5rem 0;position:sticky;top:0}}.localtoc ul{list-style:none;margin:.125rem 0 0;padding:0}.localtoc li a{display:inline-block;padding:.3rem 0}.localtoc li li a{padding-left:.75rem}.localtoc li a{color:#b8b8b8;font-weight:500;position:relative}.localtoc p{margin:0}.localtoc .caption,.localtoc>ul{margin-bottom:.5rem}.localtoc>ul{margin-left:13px;position:relative}.localtoc>ul:after{background:#444;bottom:.15rem;content:"";left:-11px;position:absolute;top:.15rem;width:1px;z-index:1000}.localtoc li a.current{color:#fff}.localtoc li a.current:after{background:#fb660a;background:var(--text-accent-colour);bottom:.3rem;content:"";left:-11.5px;position:absolute;top:.3rem;width:2px;z-index:2000}#readthedocs-embed-flyout .rst-versions{border:1px solid #555;border-radius:5px;margin-top:3rem;position:static;width:calc(275px - 4rem);width:calc(var(--fixed-sidebar-width) - 4rem)}#readthedocs-embed-flyout .rst-versions .rst-current-version{border-radius:5px;padding:0 .75rem}#readthedocs-embed-flyout .rst-versions .rst-other-versions dl+dl{margin-top:.9rem}#readthedocs-embed-flyout .rst-versions .rst-other-versions>dl:last-of-type>dd{width:100%}#readthedocs-embed-flyout .rst-versions .rst-other-versions dd a{padding:.375rem .375rem 0 0}#readthedocs-embed-flyout .rst-versions .rst-other-versions dd>div{padding:.375rem .375rem 0 0!important}#readthedocs-embed-flyout .rst-versions .rst-other-versions input{width:100%}
```

### Comparing `takao-0.1.0/takao/static/takao.js` & `takao-0.1.1/takao/static/takao.js`

 * *Files identical despite different names*

### Comparing `takao-0.1.0/PKG-INFO` & `takao-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: takao
-Version: 0.1.0
+Version: 0.1.1
 Summary: A dark theme for Sphinx.
 Home-page: https://github.com/reupen/takao
 License: MIT
 Author: Reupen Shah
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

