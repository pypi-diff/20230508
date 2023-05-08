# Comparing `tmp/mkdocs_exporter-0.0.1.tar.gz` & `tmp/mkdocs_exporter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-0.0.1.tar", max compression
+gzip compressed data, was "mkdocs_exporter-0.0.2.tar", max compression
```

## Comparing `mkdocs_exporter-0.0.1.tar` & `mkdocs_exporter-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-0.0.1/LICENSE
--rw-r--r--   0        0        0      135 2023-05-08 14:45:15.233544 mkdocs_exporter-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-05 18:56:04.368330 mkdocs_exporter-0.0.1/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-08 11:09:34.624775 mkdocs_exporter-0.0.1/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-06 09:39:49.274344 mkdocs_exporter-0.0.1/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      409 2023-05-08 14:24:05.183541 mkdocs_exporter-0.0.1/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      712 2023-05-08 12:52:22.504789 mkdocs_exporter-0.0.1/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      891 2023-05-08 07:07:05.787453 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      598 2023-05-08 12:36:36.054788 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4375 2023-05-08 14:23:36.843541 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2225 2023-05-08 14:22:11.153541 mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3541 2023-05-08 12:40:20.574787 mkdocs_exporter-0.0.1/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-0.0.1/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-0.0.1/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-0.0.1/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-0.0.1/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1140 2023-05-08 14:52:09.793543 mkdocs_exporter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 mkdocs_exporter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2661 2023-05-08 17:27:32.453564 mkdocs_exporter-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-0.0.2/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1771 2023-05-08 16:10:13.643556 mkdocs_exporter-0.0.2/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-06 09:39:49.274344 mkdocs_exporter-0.0.2/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-0.0.2/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      894 2023-05-08 15:35:52.373552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      629 2023-05-08 15:31:52.723552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4420 2023-05-08 15:32:35.993552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2257 2023-05-08 15:48:43.343554 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3714 2023-05-08 15:34:26.483550 mkdocs_exporter-0.0.2/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-0.0.2/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-0.0.2/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-0.0.2/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-0.0.2/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1214 2023-05-08 15:49:58.273555 mkdocs_exporter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 mkdocs_exporter-0.0.2/PKG-INFO
```

### Comparing `mkdocs_exporter-0.0.1/LICENSE` & `mkdocs_exporter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/browser.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import asyncio
 
-from typing import Self
 from tempfile import NamedTemporaryFile
 from mkdocs_exporter.logging import logger
 from playwright.async_api import async_playwright
 
 
 class Browser:
   """A web browser instance."""
@@ -25,15 +26,15 @@
   def __init__(self):
     """The constructor."""
 
     self._launched = False
     self.lock = asyncio.Lock()
 
 
-  async def launch(self) -> Self:
+  async def launch(self) -> Browser:
     """Launches the browser."""
 
     if self.launched:
       return self
 
     async with self.lock:
       if self.launched:
@@ -46,23 +47,23 @@
       self.context = await self.browser.new_context()
 
       self._launched = True
 
     return self
 
 
-  async def close(self) -> Self:
+  async def close(self) -> Browser:
     """Closes the browser."""
 
     if self.context:
       await self.context.close()
     if self.browser:
       await self.browser.close()
-    if self.playwright:
-      await self.playwright.stop()
+
+    self._launched = False
 
     return self
 
 
   async def print(self, html: str) -> bytes:
     """Prints some HTML to PDF."""
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugin.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Invoked after a page has been built."""
 
     page.html = None
     page.formats = {}
 
 
   @event_priority(-100)
-  def on_post_page(self, html: str, **kwargs) -> str | None:
+  def on_post_page(self, html: str, **kwargs) -> str:
     """Invoked after a page has been built (and after all other plugins)."""
 
     preprocessor = Preprocessor()
 
     preprocessor.preprocess(html)
     preprocessor.remove('*[data-decompose=true]')
     preprocessor.teleport()
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config as BaseConfig
 
 
 class ButtonConfig(BaseConfig):
   """The configuration of a button."""
 
-  title = c.Type(str | Callable)
+  title = c.Type((str, Callable))
   """The button's title."""
 
-  icon = c.Type(str | Callable)
+  icon = c.Type((str, Callable))
   """The button's icon (typically, an SVG element)."""
 
-  href = c.Type(str | Callable)
+  href = c.Type((str, Callable))
   """The button's 'href' attribute."""
 
-  download = c.Optional(c.Type(bool | str | Callable))
+  download = c.Optional(c.Type((bool, str, Callable)))
   """The button's 'download' attribute."""
 
   target = c.Optional(c.Choice(('_blank', '_self', '_parent', '_top')))
   """The button's 'target' attribute."""
 
 
 class Config(BaseConfig):
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from typing import Optional
 from mkdocs.plugins import BasePlugin
 from mkdocs_exporter.page import Page
 from mkdocs_exporter.preprocessor import Preprocessor
 from mkdocs_exporter.plugins.extras.config import Config
 
 
 class Plugin(BasePlugin[Config]):
   """The plugin."""
 
 
-  def on_post_page(self, html: str, page: Page, **kwargs) -> None | str:
+  def on_post_page(self, html: str, page: Page, **kwargs) -> Optional[str]:
     """Invoked after a page has been built."""
 
     preprocessor = Preprocessor()
 
     preprocessor.preprocess(html)
 
     for button in self.config.buttons:
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import types
 import asyncio
 
 from weasyprint import urls
+from typing import Optional
 from mkdocs.plugins import BasePlugin
 from mkdocs_exporter.page import Page
 from mkdocs.structure.pages import Page
 from mkdocs.plugins import event_priority
 from mkdocs_exporter.logging import logger
 from mkdocs.livereload import LiveReloadServer
 from mkdocs_exporter.plugins.pdf.config import Config
@@ -16,17 +17,17 @@
 class Plugin(BasePlugin[Config]):
   """The plugin."""
 
 
   def __init__(self):
     """The constructor."""
 
-    self.renderer: None | Renderer = None
+    self.renderer: Optional[Renderer] = None
     self.tasks: list[types.CoroutineType] = []
-    self.loop: None | asyncio.AbstractEventLoop = None
+    self.loop: Optional[asyncio.AbstractEventLoop] = None
 
 
   def on_config(self, config: dict) -> None:
     """Invoked when the configuration has been validated."""
 
     def resolve(path: str) -> str:
       if path is None:
@@ -97,15 +98,15 @@
     fullpath = os.path.join(directory, filename)
 
     if page.meta.get('pdf', True):
       page.formats['pdf'] = os.path.relpath(fullpath, config['site_dir'])
 
 
   @event_priority(-75)
-  def on_post_page(self, html: str, page: Page, config: dict) -> None | str:
+  def on_post_page(self, html: str, page: Page, config: dict) -> Optional[str]:
     """Invoked after a page has been built."""
 
     page.html = html
 
     if not self.config.enabled or 'pdf' not in page.formats:
       return html
 
@@ -121,15 +122,15 @@
       logger.info('[PDF] File written to %s!', fullpath)
 
     self.tasks.append(render(page))
 
     return page.html
 
 
-  def on_post_build(self, **kwargs):
+  def on_post_build(self, **kwargs) -> None:
     """Invoked after the build process."""
 
     if not self.config.enabled:
       return
 
     self.loop = asyncio.new_event_loop()
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
+
 import os
-import importlib.resources
+import importlib_resources
 
-from typing import Self
 from mkdocs_exporter.page import Page
 from mkdocs_exporter.resources import js
 from mkdocs_exporter.browser import Browser
 from mkdocs_exporter.preprocessor import Preprocessor
 from mkdocs_exporter.renderer import Renderer as BaseRenderer
 
 
@@ -18,31 +19,31 @@
     self.back_cover = None
     self.front_cover = None
     self.scripts: list[str] = []
     self.stylesheets: list[str] = []
     self.browser = browser or Browser()
 
 
-  def add_stylesheet(self, path: str) -> Self:
+  def add_stylesheet(self, path: str) -> Renderer:
     """Adds a stylesheet to the renderer."""
 
     self.stylesheets.append(path)
 
     return self
 
 
-  def add_script(self, path: str) -> Self:
+  def add_script(self, path: str) -> Renderer:
     """Adds a script to the renderer."""
 
     self.scripts.append(path)
 
     return self
 
 
-  def cover(self, template: str) -> Self:
+  def cover(self, template: str) -> Renderer:
     """Renders a cover."""
 
     content = template.strip('\n')
 
     return f'<div data-decompose="true">{content}</div>' + '\n'
 
 
@@ -66,19 +67,19 @@
       with open(stylesheet, 'r') as file:
         preprocessor.stylesheet(file.read())
     for script in self.scripts:
       with open(script, 'r') as file:
         preprocessor.script(file.read())
 
     if kwargs.get('polyfills', True):
-      preprocessor.script(importlib.resources.files(js).joinpath('pagedjs.min.js').read_text())
+      preprocessor.script(importlib_resources.files(js).joinpath('pagedjs.min.js').read_text())
 
     html = preprocessor.done()
 
     return await self.browser.print(html)
 
 
-  async def dispose(self):
+  async def dispose(self) -> None:
     """Dispose of the renderer."""
 
     if self.browser:
       await self.browser.close()
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-0.0.2/mkdocs_exporter/preprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,48 @@
+from __future__ import annotations
+
 import os
 import sass
 
 from weasyprint import urls
 from bs4 import BeautifulSoup, Tag
-from typing import Any, Callable, Self
+from typing import Any, Callable, Union
 from mkdocs_exporter.logging import logger
 
 
 class Preprocessor():
   """The HTML preprocessor."""
 
   def __init__(self, html: str = None):
     """The constructor."""
 
     self.preprocess(html)
 
 
-  def preprocess(self, html: str) -> Self:
+  def preprocess(self, html: str) -> Preprocessor:
     """Gives the preprocessor some HTML to work on."""
 
     self.html = BeautifulSoup(html, 'lxml') if isinstance(html, str) else None
 
     return self
 
 
-  def button(self, title: str, href: str, icon: str, **kwargs) -> Self:
+  def button(self, title: str, href: str, icon: str, **kwargs) -> Preprocessor:
     """Adds a button at the top of the page."""
 
     button = self.html.new_tag('a', title=title, href=href, **kwargs, attrs={'class': 'md-content__button md-icon'})
     svg = BeautifulSoup(icon, 'lxml')
 
     button.append(svg)
     self.html.find('article', { 'class': 'md-content__inner' }).insert(0, button)
 
     return self
 
 
-  def teleport(self) -> Self:
+  def teleport(self) -> Preprocessor:
     """Teleport elements to their destination."""
 
     for element in self.html.select('*[data-teleport]'):
       selector = element.attrs['data-teleport']
       destination = self.html.select_one(selector)
       tag = Tag(None, name=element.name, attrs=element.attrs)
 
@@ -55,57 +57,63 @@
       element.attrs['data-teleport'] = None
 
       destination.append(element)
 
     return self
 
 
-  def script(self, script: str = None, type: str = 'text/javascript', **kwargs):
+  def script(self, script: str = None, type: str = 'text/javascript', **kwargs) -> Preprocessor:
     """Appends a script to the document's body."""
 
     element = self.html.new_tag('script', type=type, **kwargs)
 
     element.string = script
 
     self.html.body.append(element)
 
+    return self
+
 
-  def stylesheet(self, stylesheet: str, **kwargs) -> Self:
+  def stylesheet(self, stylesheet: str, **kwargs) -> Preprocessor:
     """Appends a stylesheet to the document's head."""
 
     css = sass.compile(string=stylesheet, output_style='compressed')
     element = self.html.new_tag('style', type='text/css', rel='stylesheet', **kwargs)
 
     element.string = css
 
     self.html.head.append(element)
 
+    return self
 
-  def remove(self, selectors: str | list[str]) -> Self:
+
+  def remove(self, selectors: Union[str, list[str]]) -> Preprocessor:
     """Removes some elements."""
 
     if isinstance(selectors, str):
       selectors = [selectors]
 
     for selector in selectors:
       for element in self.html.select(selector):
         element.decompose()
 
+    return self
+
 
-  def remove_scripts(self, predicate: Callable[[Any], bool] = lambda _: True) -> Self:
+  def remove_scripts(self, predicate: Callable[[Any], bool] = lambda _: True) -> Preprocessor:
     """Remove all script tags."""
 
     for element in self.html.find_all('script'):
       if predicate(element):
         element.decompose()
 
     return self
 
 
-  def update_links(self, base: str, root: str = None) -> Self:
+  def update_links(self, base: str, root: str = None) -> Preprocessor:
     """Updates links to their new base location."""
 
     for element in self.html.find_all('link', href=True):
       element['href'] = self._resolve_link(element['href'], base, root)
     for element in self.html.find_all(src=True):
       element['src'] = self._resolve_link(element['src'], base, root)
 
@@ -118,15 +126,15 @@
     result = str(self.html)
 
     self.html = None
 
     return result
 
 
-  def _resolve_link(self, url: str, base: str, root: str = None):
+  def _resolve_link(self, url: str, base: str, root: str = None) -> str:
     """Resolves a link to its new base location."""
 
     if urls.url_is_absolute(url):
       return url
     if root is not None and os.path.isabs(url):
       return 'file://' + os.path.abspath(os.path.join(root, url.strip('/')))
```

### Comparing `mkdocs_exporter-0.0.1/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-0.0.2/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.1/pyproject.toml` & `mkdocs_exporter-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "0.0.1"
+version = "0.0.2"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
-description = "Lorem ipsum dolor sit amet..."
+description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: Documentation",
@@ -23,14 +23,15 @@
 python = ">=3.7"
 mkdocs = ">=1.4"
 playwright = ">=1.33"
 beautifulsoup4 = ">=4.12.2"
 weasyprint = ">=50.0"
 lxml = ">=4.9"
 libsass = ">=0.22.0"
+importlib-resources = "*"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 "mkdocs/exporter" = "mkdocs_exporter.plugin:Plugin"
 "mkdocs/exporter/pdf" = "mkdocs_exporter.plugins.pdf.plugin:Plugin"
 "mkdocs/exporter/extras" = "mkdocs_exporter.plugins.extras.plugin:Plugin"
 
 [tool.poetry.urls]
```

