# Comparing `tmp/canopy-platform-0.0.7.tar.gz` & `tmp/canopy-platform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canopy-platform-0.0.7.tar", last modified: Tue Dec 21 04:16:22 2021, max compression
+gzip compressed data, was "canopy-platform-0.0.9.tar", last modified: Mon Jan 24 20:13:24 2022, max compression
```

## Comparing `canopy-platform-0.0.7.tar` & `canopy-platform-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    34523 2021-10-07 18:31:00.200626 canopy-platform-0.0.7/LICENSE
--rw-r--r--   0        0        0     1648 2021-12-04 06:47:57.290287 canopy-platform-0.0.7/canopy/__init__.py
--rw-r--r--   0        0        0     6544 2021-12-16 22:36:07.313335 canopy-platform-0.0.7/canopy/bootstrap/__init__.py
--rw-r--r--   0        0        0     4123 2021-12-16 21:34:45.160776 canopy-platform-0.0.7/canopy/bootstrap/templates/index.html
--rw-r--r--   0        0        0     2714 2021-12-19 18:45:52.135310 canopy-platform-0.0.7/canopy/static/screen.css
--rw-r--r--   0        0        0       48 2021-10-02 20:39:06.865377 canopy-platform-0.0.7/canopy/templates/__init__.py
--rw-r--r--   0        0        0      507 2021-10-17 18:39:52.242553 canopy-platform-0.0.7/canopy/templates/sign_in.html
--rw-r--r--   0        0        0     4379 2021-11-12 03:49:35.281078 canopy-platform-0.0.7/canopy/templates/template.html
--rw-r--r--   0        0        0     1827 2021-12-21 04:16:20.152539 canopy-platform-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1149 2021-12-21 04:16:22.830920 canopy-platform-0.0.7/setup.py
--rw-r--r--   0        0        0     1009 2021-12-21 04:16:22.831176 canopy-platform-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2021-10-07 18:31:00.200626 canopy-platform-0.0.9/LICENSE
+-rw-r--r--   0        0        0      308 2022-01-24 19:16:46.067935 canopy-platform-0.0.9/README.md
+-rw-r--r--   0        0        0     1643 2022-01-23 21:31:18.250866 canopy-platform-0.0.9/canopy/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-22 23:32:30.870600 canopy-platform-0.0.9/canopy/static/__init__.py
+-rw-r--r--   0        0        0     2714 2021-12-19 18:45:52.135310 canopy-platform-0.0.9/canopy/static/screen.css
+-rw-r--r--   0        0        0       48 2021-10-02 20:39:06.865377 canopy-platform-0.0.9/canopy/templates/__init__.py
+-rw-r--r--   0        0        0      507 2022-01-16 00:11:39.936462 canopy-platform-0.0.9/canopy/templates/sign_in.html
+-rw-r--r--   0        0        0     4335 2022-01-17 04:35:25.692126 canopy-platform-0.0.9/canopy/templates/template.html
+-rw-r--r--   0        0        0     2027 2022-01-24 20:13:20.730149 canopy-platform-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1486 2022-01-24 20:13:24.919906 canopy-platform-0.0.9/setup.py
+-rw-r--r--   0        0        0     1452 2022-01-24 20:13:24.920211 canopy-platform-0.0.9/PKG-INFO
```

### Comparing `canopy-platform-0.0.7/LICENSE` & `canopy-platform-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `canopy-platform-0.0.7/canopy/__init__.py` & `canopy-platform-0.0.9/canopy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""A decentralized social platform."""
+"""Social web platform."""
 
 from understory import web
 from understory.apps import (cache, data, indieauth_client, indieauth_server,
                              jobs, micropub_server, microsub_server, owner,
                              search, sites, system, text_editor, text_reader,
                              tracker, webmention_endpoint, websub_endpoint)
 from understory.web import tx
 
-__all__ = ["app"]
-
 app = web.application(
     __name__,
     db=True,
     mounts=(
         owner.app,
         jobs.app,
         sites.app,
@@ -51,12 +49,12 @@
     yield
     if tx.response.headers.content_type == "text/html" and tx.response.claimed:
         tx.response.body = "<!doctype html>" + str(tx.response.body)
 
 
 @app.control("sign-in")
 class SignIn:
-    """"""
+    """Sign in as owner or guest."""
 
     def get(self):
         return_url = web.form(return_url="").return_url
         return app.view.sign_in(return_url)
```

### Comparing `canopy-platform-0.0.7/canopy/static/screen.css` & `canopy-platform-0.0.9/canopy/static/screen.css`

 * *Files identical despite different names*

### Comparing `canopy-platform-0.0.7/canopy/templates/template.html` & `canopy-platform-0.0.9/canopy/templates/template.html`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 </div>
 $if "suffix" in resource:
     $:resource.suffix
 </article>
 <nav id=site>
 <div class=h-card>
 <strong><big class=p-name><a class="u-url u-uid"
-href=$owner["uid"][0]>$owner["name"][0]</a></big></strong><br>
-<small>$tx.origin.partition("//")[2]</small>
+href=$owner["uid"][0]>$owner["name"][0]</a></big></strong>
 $ note = owner.get("note")
 $if note:
     <p>$note[0]</p>
 <ul class=elsewhere>
 $for url in owner.get("url", []):
     $if tx.request.uri.host in url:
         $continue
@@ -87,15 +86,15 @@
             src=/static/logos/$(service.lower()).svg alt=$service
             style="height:1em"><span>$match.groupdict()["user"]</span></a>
             $break
     $else:
         <a rel=me href=$url>$url</a>
     </li>
 </ul>
-<p style=text-align:right><small><a href=/about>more about me</a></small></p>
+<!--p style=text-align:right><small><a href=/about>more about me</a></small></p-->
 </div>
 $if not getattr(tx.user, "is_authenticating", False) and path != "sign-in":
     $if "uid" in tx.user.session:
         $if tx.user.is_owner:
             $ action = "/owner/sign-out"
         $else:
             $ action = "/guests/sign-out"
```

#### html2text {}

```diff
@@ -18,22 +18,20 @@
 $:sep$:post_sep\ $ n -= 1
  $if "title" in resource and getattr(resource, "show_title", True):
 ****** $:resource.title ******
 $if "header" in resource: $:resource.header()
 $:resource
  $if "aside" in resource: $:resource.aside()
 $if "suffix" in resource: $:resource.suffix
-$owner["name"][0]
-$tx.origin.partition("//")[2] $ note = owner.get("note") $if note:
+$owner["name"][0] $ note = owner.get("note") $if note:
 $note[0]
     * $for url in owner.get("url", []): $if tx.request.uri.host in url:
       $continue
     * $for service, pattern in SILOS.items(): $ match = re.match(pattern, url)
       $if match: [$service]$match.groupdict()["user"] $break $else: $url
-more_about_me
 $if not getattr(tx.user, "is_authenticating", False) and path != "sign-in": $if
 "uid" in tx.user.session: $if tx.user.is_owner: $ action = "/owner/sign-out"
 $else: $ action = "/guests/sign-out"
  $if not tx.user.is_owner:
 $tx.user.session["name"]
 $tx.user.session["uid"].partition("//")[2]
 Sign Out
```

### Comparing `canopy-platform-0.0.7/setup.py` & `canopy-platform-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['canopy', 'canopy.bootstrap', 'canopy.templates']
+['canopy', 'canopy.static', 'canopy.templates']
 
 package_data = \
-{'': ['*'], 'canopy': ['static/*'], 'canopy.bootstrap': ['templates/*']}
+{'': ['*']}
 
 install_requires = \
-['micropub>=0.0.5,<0.0.6',
+['datrie>=0.8.2,<0.9.0',
  'understory-indieauth-client>=0.0.4,<0.0.5',
  'understory-indieauth-server>=0.0.4,<0.0.5',
  'understory-micropub-server>=0.0.5,<0.0.6',
  'understory-microsub-server>=0.0.2,<0.0.3',
  'understory-text-editor>=0.0.5,<0.0.6',
  'understory-text-reader>=0.0.2,<0.0.3',
  'understory-tracker>=0.0.2,<0.0.3',
  'understory-webmention-endpoint>=0.0.3,<0.0.4',
  'understory-websub-endpoint>=0.0.3,<0.0.4',
  'understory>=0,<1']
 
+entry_points = \
+{'console_scripts': ['build_gaea = gaea:build']}
+
 setup_kwargs = {
     'name': 'canopy-platform',
-    'version': '0.0.7',
-    'description': 'A decentralized social platform.',
-    'long_description': None,
+    'version': '0.0.9',
+    'description': 'Social web platform.',
+    'long_description': '# Canopy\n\nSocial web platform.\n\n![Demo](https://media.githubusercontent.com/media/canopy/canopy/main/demo.gif)\n\n## Use\n\n[Linux](https://github.com/canopy/canopy/releases/download/v0.0.1-alpha/gaea) |\nWindows |\nMac\n\n## Develop\n\n    poetry install\n    poetry run web serve canopy:app\n    poetry run build_gaea\n',
     'author': 'Angelo Gladding',
-    'author_email': 'self@angelogladding.com',
+    'author_email': 'angelo@ragt.ag',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.9,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

