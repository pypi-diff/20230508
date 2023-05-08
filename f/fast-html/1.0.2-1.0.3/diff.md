# Comparing `tmp/fast_html-1.0.2.tar.gz` & `tmp/fast_html-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_html-1.0.2.tar", max compression
+gzip compressed data, was "fast_html-1.0.3.tar", max compression
```

## Comparing `fast_html-1.0.2.tar` & `fast_html-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7636 2022-09-30 09:37:45.787169 fast_html-1.0.2/LICENSE
--rw-r--r--   0        0        0     3476 2022-10-01 08:51:42.117514 fast_html-1.0.2/README.rst
--rw-r--r--   0        0        0    10838 2022-09-30 09:20:55.555921 fast_html-1.0.2/fast_html/__init__.py
--rw-r--r--   0        0        0      609 2022-10-01 08:50:46.826396 fast_html-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4161 2022-10-01 08:55:23.100976 fast_html-1.0.2/setup.py
--rw-r--r--   0        0        0     4353 2022-10-01 08:55:23.101256 fast_html-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7636 2023-05-08 16:52:22.164958 fast_html-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3519 2023-05-08 17:36:28.591856 fast_html-1.0.3/README.rst
+-rw-r--r--   0        0        0    10906 2023-05-08 17:36:04.512192 fast_html-1.0.3/fast_html/__init__.py
+-rw-r--r--   0        0        0      609 2023-05-08 17:38:34.218098 fast_html-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4207 2023-05-08 17:52:27.192949 fast_html-1.0.3/setup.py
+-rw-r--r--   0        0        0     4396 2023-05-08 17:52:27.193223 fast_html-1.0.3/PKG-INFO
```

### Comparing `fast_html-1.0.2/LICENSE` & `fast_html-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_html-1.0.2/README.rst` & `fast_html-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 <div>text<span>item 1</span><span>item 2</span></div>
 
 The innerHTML can also be a list of lists:
 
 >>> print(render(div(["text", [span(f"item {i}") for i in [1,2]]])))
 <div>text<span>item 1</span><span>item 2</span></div>
 
+>>> print(render([br(), br()]))
+<br><br>
 
 The innerHTML can also be specified using the ``i`` parameter,
 after the other attributes, to match the order of rendering:
 
 >>> print(render(ul(class_="s12", i=[
 ...                 li("item 1"),
 ...                 li("item 2")]
@@ -100,15 +102,15 @@
 >>> print(render(my_tag("text")))
 <my_tag>text</my_tag>
 
 
 When debugging your code, you can set global variable ``indent`` to ``True``
 (or call ``indent_it(True)``) to obtain HTML with tag indentation, e.g.,
 
->>> indent_it(True); print(render(div(class_="s12", i=["text", span("item 1"), span("item 2")])))
+>>> indent_it(True); print(render(div(class_="s12", i=["text\n", span("item 1"), span("item 2")])))
 <div class="s12">
   text
   <span>
     item 1
   </span>
   <span>
     item 2
```

### Comparing `fast_html-1.0.2/fast_html/__init__.py` & `fast_html-1.0.3/fast_html/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.1'
+__version__ = '1.0.3'
 
 indent = False
 
 
 from typing import Iterator, List, Optional, Union
 import re
 
@@ -13,14 +13,16 @@
 _cr = "\n"
 
 def indent_it(value):
     global indent
     indent = value
 
 def render(gen: Tag) -> str:
+    if type(gen) == list:
+        return ''.join(render(t) for t in gen)
     return ''.join(gen)
 
 
 def solo_tag(tag_name: str, ** kwargs) -> Tag:
     """returns a tag without innerHTML, e.g. `<br id="1">`
 
     Args:
@@ -78,15 +80,15 @@
 
     if inner is not None:
         if type(inner) == str:  # inner is a str
             yield (f"{_tab}{inner}{_cr}" if indent else inner)
         else:
             for i in inner:
                 if type(i) == str:  # inner is a Tag
-                    yield (f"{_tab}{i}{_cr}" if indent else i)
+                    yield (f"{_tab}{i}" if indent else i)
                 else:
                     for i1 in i:
                         yield from _inner(i1)
 
     yield f"</{tag_name}>{_cr if indent else ''}"
```

### Comparing `fast_html-1.0.2/pyproject.toml` & `fast_html-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast_html"
-version = "1.0.2"
+version = "1.0.3"
 description = "A fast, minimalist HTML generator"
 authors = ["Pierre <pierre.carbonnelle@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/pcarbonn/fast_html"
 license = "LGPL-3.0-or-later"
 keywords = ["HTML", "HTMX"]
 classifiers = [
```

### Comparing `fast_html-1.0.2/setup.py` & `fast_html-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['fast_html']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'fast-html',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'A fast, minimalist HTML generator',
-    'long_description': 'fast_html is a fast, minimalist HTML generator.\n\nIt is an alternative to templating engines, like Jinja,\nfor use with, e.g., `htmx <https://htmx.org/>`__.\n\nPros:\n\n- use familiar python syntax\n\n- use efficient concatenation techniques\n\n- optional automatic indentation\n\nUnlike other HTML generators (e.g. `Dominate <https://pypi.org/project/dominate/>`__) that use python objects to represent HTML snippets,\nfast_html represents HTML snippets using string `generators <https://docs.python.org/3/glossary.html#term-generator>`__\nthat can be rendered extremely fast using ``join``.\n(see `here <https://python.plainenglish.io/concatenating-strings-efficiently-in-python-9bfc8e8d6f6e>`__)\n\nLike other HTML generators, one needs to remember:\n\n- the name of some tags and attributes is changed (e.g., ``class_`` instead of ``class``, due to Python parser)\n\n- there may be conflicts of function names with your code base\n\n\nInstallation\n------------\n``pip install fast_html`` or copy the (single) source file in your project.\n\nDon\'t forget to `add a star on GitHub <https://github.com/pcarbonn/fast_html>`_ ! Thanks.\n\n\nTutorial:\n---------\n\n>>> from fast_html import *\n\nA tag is created by calling a function of the corresponding name,\nand rendered using ``render``:\n\n>>> print(render(p("text")))\n<p>text</p>\n\n\nTag attributes are specified using named arguments:\n\n>>> print(render(br(id="1")))\n<br id="1">\n\n>>> print(render(br(id=None)))\n<br>\n\n>>> print(render(ul(li("text", selected=True))))\n<ul><li selected>text</li></ul>\n\n>>> print(render(ul(li("text", selected=False))))\n<ul><li>text</li></ul>\n\nThe python parser introduces some constraints:\n\n- The following tags require a trailing underscore: ``del_``, ``input_``, ``map_``, ``object_``.\n\n- The following tag attributes require a trailing underscore: ``class_``, ``for_`` (and possibly others).\n\nIn fact, the trailing underscore in attribute names is always removed by fast_html,\nand other underscores are replaced by ``-``.\nFor example, the htmx attribute ``hx-get`` is set using ``hx_get="url"``.\n\n>>> print(render(object_("text", class_="s12", hx_get="url")))\n<object class="s12" hx-get="url">text</object>\n\n>>> print(render(button("Click me", hx_post="/clicked", hx_swap="outerHTML")))\n<button hx-post="/clicked" hx-swap="outerHTML">Click me</button>\n\n\nThe innerHTML can be a list:\n\n>>> print(render(div(["text", span("item 1"), span("item 2")])))\n<div>text<span>item 1</span><span>item 2</span></div>\n\nThe innerHTML can also be a list of lists:\n\n>>> print(render(div(["text", [span(f"item {i}") for i in [1,2]]])))\n<div>text<span>item 1</span><span>item 2</span></div>\n\n\nThe innerHTML can also be specified using the ``i`` parameter,\nafter the other attributes, to match the order of rendering:\n\n>>> print(render(ul(class_="s12", i=[\n...                 li("item 1"),\n...                 li("item 2")]\n...      )))\n<ul class="s12"><li>item 1</li><li>item 2</li></ul>\n\nYou can create your own tag using the ``tag`` function:\n\n>>> def my_tag(inner=None, **kwargs):\n...     yield from tag("my_tag", inner, **kwargs)\n>>> print(render(my_tag("text")))\n<my_tag>text</my_tag>\n\n\nWhen debugging your code, you can set global variable ``indent`` to ``True``\n(or call ``indent_it(True)``) to obtain HTML with tag indentation, e.g.,\n\n>>> indent_it(True); print(render(div(class_="s12", i=["text", span("item 1"), span("item 2")])))\n<div class="s12">\n  text\n  <span>\n    item 1\n  </span>\n  <span>\n    item 2\n  </span>\n</div>\n<BLANKLINE>\n',
+    'long_description': 'fast_html is a fast, minimalist HTML generator.\n\nIt is an alternative to templating engines, like Jinja,\nfor use with, e.g., `htmx <https://htmx.org/>`__.\n\nPros:\n\n- use familiar python syntax\n\n- use efficient concatenation techniques\n\n- optional automatic indentation\n\nUnlike other HTML generators (e.g. `Dominate <https://pypi.org/project/dominate/>`__) that use python objects to represent HTML snippets,\nfast_html represents HTML snippets using string `generators <https://docs.python.org/3/glossary.html#term-generator>`__\nthat can be rendered extremely fast using ``join``.\n(see `here <https://python.plainenglish.io/concatenating-strings-efficiently-in-python-9bfc8e8d6f6e>`__)\n\nLike other HTML generators, one needs to remember:\n\n- the name of some tags and attributes is changed (e.g., ``class_`` instead of ``class``, due to Python parser)\n\n- there may be conflicts of function names with your code base\n\n\nInstallation\n------------\n``pip install fast_html`` or copy the (single) source file in your project.\n\nDon\'t forget to `add a star on GitHub <https://github.com/pcarbonn/fast_html>`_ ! Thanks.\n\n\nTutorial:\n---------\n\n>>> from fast_html import *\n\nA tag is created by calling a function of the corresponding name,\nand rendered using ``render``:\n\n>>> print(render(p("text")))\n<p>text</p>\n\n\nTag attributes are specified using named arguments:\n\n>>> print(render(br(id="1")))\n<br id="1">\n\n>>> print(render(br(id=None)))\n<br>\n\n>>> print(render(ul(li("text", selected=True))))\n<ul><li selected>text</li></ul>\n\n>>> print(render(ul(li("text", selected=False))))\n<ul><li>text</li></ul>\n\nThe python parser introduces some constraints:\n\n- The following tags require a trailing underscore: ``del_``, ``input_``, ``map_``, ``object_``.\n\n- The following tag attributes require a trailing underscore: ``class_``, ``for_`` (and possibly others).\n\nIn fact, the trailing underscore in attribute names is always removed by fast_html,\nand other underscores are replaced by ``-``.\nFor example, the htmx attribute ``hx-get`` is set using ``hx_get="url"``.\n\n>>> print(render(object_("text", class_="s12", hx_get="url")))\n<object class="s12" hx-get="url">text</object>\n\n>>> print(render(button("Click me", hx_post="/clicked", hx_swap="outerHTML")))\n<button hx-post="/clicked" hx-swap="outerHTML">Click me</button>\n\n\nThe innerHTML can be a list:\n\n>>> print(render(div(["text", span("item 1"), span("item 2")])))\n<div>text<span>item 1</span><span>item 2</span></div>\n\nThe innerHTML can also be a list of lists:\n\n>>> print(render(div(["text", [span(f"item {i}") for i in [1,2]]])))\n<div>text<span>item 1</span><span>item 2</span></div>\n\n>>> print(render([br(), br()]))\n<br><br>\n\nThe innerHTML can also be specified using the ``i`` parameter,\nafter the other attributes, to match the order of rendering:\n\n>>> print(render(ul(class_="s12", i=[\n...                 li("item 1"),\n...                 li("item 2")]\n...      )))\n<ul class="s12"><li>item 1</li><li>item 2</li></ul>\n\nYou can create your own tag using the ``tag`` function:\n\n>>> def my_tag(inner=None, **kwargs):\n...     yield from tag("my_tag", inner, **kwargs)\n>>> print(render(my_tag("text")))\n<my_tag>text</my_tag>\n\n\nWhen debugging your code, you can set global variable ``indent`` to ``True``\n(or call ``indent_it(True)``) to obtain HTML with tag indentation, e.g.,\n\n>>> indent_it(True); print(render(div(class_="s12", i=["text\\n", span("item 1"), span("item 2")])))\n<div class="s12">\n  text\n  <span>\n    item 1\n  </span>\n  <span>\n    item 2\n  </span>\n</div>\n<BLANKLINE>\n',
     'author': 'Pierre',
     'author_email': 'pierre.carbonnelle@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pcarbonn/fast_html',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fast_html-1.0.2/PKG-INFO` & `fast_html-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-html
-Version: 1.0.2
+Version: 1.0.3
 Summary: A fast, minimalist HTML generator
 Home-page: https://github.com/pcarbonn/fast_html
 License: LGPL-3.0-or-later
 Keywords: HTML,HTMX
 Author: Pierre
 Author-email: pierre.carbonnelle@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -101,14 +101,16 @@
 <div>text<span>item 1</span><span>item 2</span></div>
 
 The innerHTML can also be a list of lists:
 
 >>> print(render(div(["text", [span(f"item {i}") for i in [1,2]]])))
 <div>text<span>item 1</span><span>item 2</span></div>
 
+>>> print(render([br(), br()]))
+<br><br>
 
 The innerHTML can also be specified using the ``i`` parameter,
 after the other attributes, to match the order of rendering:
 
 >>> print(render(ul(class_="s12", i=[
 ...                 li("item 1"),
 ...                 li("item 2")]
@@ -122,15 +124,15 @@
 >>> print(render(my_tag("text")))
 <my_tag>text</my_tag>
 
 
 When debugging your code, you can set global variable ``indent`` to ``True``
 (or call ``indent_it(True)``) to obtain HTML with tag indentation, e.g.,
 
->>> indent_it(True); print(render(div(class_="s12", i=["text", span("item 1"), span("item 2")])))
+>>> indent_it(True); print(render(div(class_="s12", i=["text\n", span("item 1"), span("item 2")])))
 <div class="s12">
   text
   <span>
     item 1
   </span>
   <span>
     item 2
```

