# Comparing `tmp/sphinxcontrib-bitfield-0.4.2.tar.gz` & `tmp/sphinxcontrib-bitfield-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-bitfield-0.4.2.tar", last modified: Wed Jan  4 20:41:05 2023, max compression
+gzip compressed data, was "sphinxcontrib-bitfield-1.0.0.tar", last modified: Mon May  8 20:00:41 2023, max compression
```

## Comparing `sphinxcontrib-bitfield-0.4.2.tar` & `sphinxcontrib-bitfield-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:41:05.198327 sphinxcontrib-bitfield-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-04 20:41:05.198327 sphinxcontrib-bitfield-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-01-04 20:40:52.000000 sphinxcontrib-bitfield-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-04 20:40:52.000000 sphinxcontrib-bitfield-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-04 20:41:05.198327 sphinxcontrib-bitfield-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:41:05.198327 sphinxcontrib-bitfield-0.4.2/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-04 20:40:52.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-01-04 20:40:52.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib/bitfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:41:05.198327 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-04 20:41:05.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-04 20:41:05.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 20:41:05.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-04 20:41:05.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-04 20:41:05.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-04 20:41:05.000000 sphinxcontrib-bitfield-0.4.2/sphinxcontrib_bitfield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:00:41.331107 sphinxcontrib-bitfield-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-08 20:00:41.331107 sphinxcontrib-bitfield-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-08 20:00:28.000000 sphinxcontrib-bitfield-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 20:00:28.000000 sphinxcontrib-bitfield-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 20:00:41.331107 sphinxcontrib-bitfield-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:00:41.327107 sphinxcontrib-bitfield-1.0.0/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 20:00:28.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-08 20:00:28.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib/bitfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:00:41.331107 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-08 20:00:41.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 20:00:41.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:00:41.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 20:00:41.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 20:00:41.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 20:00:41.000000 sphinxcontrib-bitfield-1.0.0/sphinxcontrib_bitfield.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-bitfield-0.4.2/README.rst` & `sphinxcontrib-bitfield-1.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -57,15 +57,23 @@
         overall bitwidth - default 32
     fontfamily:
         default sans-serif
     fontweight:
         default normal
     fontsize:
         default 14
+    strokewidth:
+        default 1
     compact:
         compact rendering mode
     hflip:
         horizontal flip
     vflip:
         vertical flip
+    uneven:
+        uneven lanes
+    trim:
+        trim long bitfield names, must provide the horizontal space available for a single character
+    legend:
+        space separated list of name and type optionally enclosed in quotes
 
 For more details, see the `bit_field <https://github.com/Arth-ur/bitfield>`_ package.
```

### Comparing `sphinxcontrib-bitfield-0.4.2/setup.cfg` & `sphinxcontrib-bitfield-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = sphinxcontrib-bitfield
-version = 0.4.2
+version = 1.0.0
 author = Arthur Gay
 description = Sphinx "bitfield" extension
-long_description = file: README.md
-long_description_content_type = text/markdown
+long_description = file: README.rst
+long_description_content_type = text/x-rst
 url = https://github.com/Arth-ur/sphinxcontrib-bitfield
 keywords = sphinx, extension, documentation, bitfield, bytefield, diagram, renderer, svg
 license = BSD
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Environment :: Web Environment
@@ -18,15 +18,15 @@
 	Programming Language :: Python
 	Framework :: Sphinx :: Extension
 	Topic :: Documentation
 	Topic :: Utilities
 
 [options]
 install_requires = 
-	bit-field>=0.4.0
+	bit-field>=1.0.0
 	Sphinx>=0.6
 packages = find:
 namespace_packages = 
 	sphinxcontrib
 
 [options.extras_require]
 LaTeX = CairoSVG>=2.5.2
```

### Comparing `sphinxcontrib-bitfield-0.4.2/sphinxcontrib/bitfield.py` & `sphinxcontrib-bitfield-1.0.0/sphinxcontrib/bitfield.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from docutils.parsers.rst import Directive
 from docutils.parsers.rst.directives import flag
 from bit_field import render, jsonml_stringify
 from json import loads
 from hashlib import sha1
 from os.path import join
 from sphinx.errors import ExtensionError
+from shlex import split
 
 
 class bitfield(nodes.General, nodes.Element):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.options = dict(kwargs['options'])
         self.options['compact'] = 'compact' in self.options
         self.options['hflip'] = 'hflip' in self.options
         self.options['vflip'] = 'vflip' in self.options
+        self.options['uneven'] = 'uneven' in self.options
 
 
 def visit_bitfield_html(self, node):
     self.body.append(
         jsonml_stringify(
             render(
                 loads(' '.join(node.rawsource)),
@@ -50,27 +52,36 @@
     self.body.append(r'\sphinxincludegraphics[]{{{}}}'.format(fname))
 
 
 def depart_bitfield(self, node):
     pass
 
 
+def legend(s):
+    x = split(s)
+    return {k: v for k, v in zip(x[0::2], x[1::2])}
+
+
 class BitfieldDirective(Directive):
     has_content = True
     option_spec = {
-        'vspace': int,
-        'hspace': int,
+        'vspace': float,
+        'hspace': float,
         'lanes': int,
         'bits': int,
-        'fontsize': int,
+        'fontsize': float,
         'fontfamily': str,
         'fontweight': str,
+        'strokewidth': float,
         'compact': flag,
         'hflip': flag,
         'vflip': flag,
+        'uneven': flag,
+        'trim': float,
+        'legend': legend,
     }
 
     def run(self):
         return [bitfield(self.content, options=self.options)]
 
 
 def setup(app):
```

