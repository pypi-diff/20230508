# Comparing `tmp/webconsole-0.0.3.tar.gz` & `tmp/webconsole-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webconsole-0.0.3.tar", last modified: Fri May  5 07:17:34 2023, max compression
+gzip compressed data, was "dist/webconsole-0.0.5.tar", last modified: Mon May  8 01:40:44 2023, max compression
```

## Comparing `webconsole-0.0.3.tar` & `webconsole-0.0.5.tar`

### file list

```diff
@@ -1,233 +1,234 @@
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 05:18:55.000000 webconsole-0.0.3/MANIFEST.in
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      277 2023-05-05 07:17:34.000000 webconsole-0.0.3/PKG-INFO
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       38 2023-05-05 07:17:34.000000 webconsole-0.0.3/setup.cfg
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      744 2023-05-05 07:17:30.000000 webconsole-0.0.3/setup.py
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-26 08:47:41.000000 webconsole-0.0.3/webconsole/__init__.py
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/docker/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-26 08:52:12.000000 webconsole-0.0.3/webconsole/docker/__init__.py
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3257 2023-05-05 07:12:25.000000 webconsole-0.0.3/webconsole/docker/docker_console.py
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/linux/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-05-04 01:38:26.000000 webconsole-0.0.3/webconsole/linux/__init__.py
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     6690 2023-05-05 07:15:48.000000 webconsole-0.0.3/webconsole/linux/linux_console.py
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/__init__.py
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/js/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:54:18.000000 webconsole-0.0.3/webconsole/static/js/__init__.py
--rw-rw-r--   0 raypick   (1000) raypick   (1000)   293430 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/js/jquery-1.12.4.js
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1177 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/LICENSE
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     8511 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/README.md
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:54:23.000000 webconsole-0.0.3/webconsole/static/xterm/__init__.py
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/bower.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/attach/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3823 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/attach/attach.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       71 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/attach/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fit/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2942 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fit/fit.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       65 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fit/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fullscreen/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fullscreen/fullscreen.css
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1245 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fullscreen/fullscreen.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       79 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/fullscreen/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/linkify/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     7180 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/linkify/linkify.js
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/search/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)   197383 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/search/search.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)   286713 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/search/search.js.map
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/terminado/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       77 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/terminado/package.json
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4182 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/addons/terminado/terminado.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    35217 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/xterm.css
--rw-rw-r--   0 raypick   (1000) raypick   (1000)   193743 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/xterm.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)   280191 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/dist/xterm.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5886 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/gulpfile.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      446 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/jsdoc.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3190 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3528 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     6109 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5651 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2308 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1275 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1571 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1248 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2802 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Charsets.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3341 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Charsets.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5140 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4707 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     9499 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     6806 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      891 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/EscapeSequences.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1074 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/EscapeSequences.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1800 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1940 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3298 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3179 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    37312 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    43920 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     7597 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     9352 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      117 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Interfaces.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       91 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Interfaces.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    10087 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     9399 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     8951 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     6981 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    24426 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Parser.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    21493 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Parser.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    12074 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Renderer.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    11173 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Renderer.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    16912 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    15726 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    11175 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    10246 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2713 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2622 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     6473 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5425 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      112 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Types.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       86 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Types.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3818 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3869 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3481 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2988 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.test.js.map
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/attach/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3823 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/attach/attach.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       71 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/attach/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fit/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2942 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fit/fit.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       65 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fit/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fullscreen/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fullscreen/fullscreen.css
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1245 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fullscreen/fullscreen.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       79 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/fullscreen/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2925 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/SearchHelper.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3166 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/SearchHelper.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1038 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/search.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1141 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/search.js.map
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/terminado/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       77 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/terminado/package.json
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4182 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/addons/terminado/terminado.js
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/handlers/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2223 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2413 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      665 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      511 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.test.js.map
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/addons/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      337 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/addons/test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      431 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/addons/test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3584 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/escape-sequences-test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4525 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/escape-sequences-test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    39843 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    48497 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/test/test.js.map
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      778 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/Browser.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      879 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/Browser.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1303 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/BufferLine.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1289 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/BufferLine.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2557 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1615 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2597 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2224 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5940 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5427 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    10189 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    12167 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1724 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1518 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1820 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1709 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      209 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/Generic.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      235 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/Generic.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1523 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/Mouse.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1903 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/Mouse.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1438 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/TestUtils.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1173 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/utils/TestUtils.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    35217 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/xterm.css
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    52391 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/xterm.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    64536 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/lib/xterm.js.map
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     9705 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5500 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Buffer.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4715 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Buffer.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1287 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/BufferSet.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2389 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/BufferSet.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4442 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Charsets.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     8883 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/CompositionHelper.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     8951 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/CompositionHelper.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2461 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/EscapeSequences.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2535 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/EventEmitter.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1570 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/EventEmitter.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     8156 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/InputHandler.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    56684 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/InputHandler.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5620 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Interfaces.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     7199 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Linkifier.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    13483 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Linkifier.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    22646 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Parser.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    13690 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Renderer.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     9508 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/SelectionManager.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    21348 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/SelectionManager.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4978 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/SelectionModel.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3645 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/SelectionModel.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      427 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Types.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2815 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Viewport.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     5093 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/Viewport.ts
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/attach/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3823 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/attach/attach.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       71 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/attach/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fit/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2942 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fit/fit.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       65 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fit/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fullscreen/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fullscreen/fullscreen.css
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1245 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fullscreen/fullscreen.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       79 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/fullscreen/package.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/search/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3985 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/search/SearchHelper.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1576 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/search/search.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      193 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/search/tsconfig.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/terminado/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       77 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/terminado/package.json
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4182 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/addons/terminado/terminado.js
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/handlers/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      579 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/handlers/Clipboard.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3475 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/handlers/Clipboard.ts
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/test/
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/test/addons/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      338 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/test/addons/test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     4334 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/test/escape-sequences-test.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    36207 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/test/test.js
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      972 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/Browser.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1806 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/BufferLine.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2433 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/CharMeasure.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1837 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/CharMeasure.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     7888 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/CircularList.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     6211 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/CircularList.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1431 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/DomElementObjectPool.test.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     2117 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/DomElementObjectPool.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      428 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/Generic.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     3119 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/Mouse.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     1602 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/utils/TestUtils.ts
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    35217 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/xterm.css
--rw-rw-r--   0 raypick   (1000) raypick   (1000)    65338 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/src/xterm.js
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      269 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/tsconfig.json
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      966 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/tslint.json
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      106 2023-04-27 02:48:36.000000 webconsole-0.0.3/webconsole/static/xterm/typings.json
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole/templates/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:45:05.000000 webconsole-0.0.3/webconsole/templates/__init__.py
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      869 2023-04-27 02:45:05.000000 webconsole-0.0.3/webconsole/templates/index.html
-drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-05 07:17:34.000000 webconsole-0.0.3/webconsole.egg-info/
--rw-rw-r--   0 raypick   (1000) raypick   (1000)      277 2023-05-05 07:17:33.000000 webconsole-0.0.3/webconsole.egg-info/PKG-INFO
--rw-rw-r--   0 raypick   (1000) raypick   (1000)     9044 2023-05-05 07:17:33.000000 webconsole-0.0.3/webconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 raypick   (1000) raypick   (1000)        1 2023-05-05 07:17:33.000000 webconsole-0.0.3/webconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       66 2023-05-05 07:17:33.000000 webconsole-0.0.3/webconsole.egg-info/requires.txt
--rw-rw-r--   0 raypick   (1000) raypick   (1000)       11 2023-05-05 07:17:33.000000 webconsole-0.0.3/webconsole.egg-info/top_level.txt
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 05:18:55.000000 webconsole-0.0.5/MANIFEST.in
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2071 2023-05-08 01:40:44.000000 webconsole-0.0.5/PKG-INFO
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1752 2023-05-08 01:35:00.000000 webconsole-0.0.5/README.md
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       38 2023-05-08 01:40:44.000000 webconsole-0.0.5/setup.cfg
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      847 2023-05-08 01:40:20.000000 webconsole-0.0.5/setup.py
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-26 08:47:41.000000 webconsole-0.0.5/webconsole/__init__.py
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/docker/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-26 08:52:12.000000 webconsole-0.0.5/webconsole/docker/__init__.py
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3257 2023-05-05 07:12:25.000000 webconsole-0.0.5/webconsole/docker/docker_console.py
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/linux/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-05-04 01:38:26.000000 webconsole-0.0.5/webconsole/linux/__init__.py
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     6644 2023-05-08 01:39:58.000000 webconsole-0.0.5/webconsole/linux/linux_console.py
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/__init__.py
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/js/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:54:18.000000 webconsole-0.0.5/webconsole/static/js/__init__.py
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)   293430 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/js/jquery-1.12.4.js
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1177 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/LICENSE
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     8511 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/README.md
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:54:23.000000 webconsole-0.0.5/webconsole/static/xterm/__init__.py
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/bower.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/attach/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3823 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/attach/attach.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       71 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/attach/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fit/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2942 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fit/fit.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       65 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fit/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fullscreen/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fullscreen/fullscreen.css
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1245 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fullscreen/fullscreen.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       79 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/fullscreen/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/linkify/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     7180 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/linkify/linkify.js
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/search/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)   197383 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/search/search.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)   286713 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/search/search.js.map
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/terminado/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       77 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/terminado/package.json
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4182 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/addons/terminado/terminado.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    35217 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/xterm.css
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)   193743 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/xterm.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)   280191 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/dist/xterm.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5886 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/gulpfile.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      446 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/jsdoc.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3190 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3528 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     6109 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5651 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2308 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1275 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1571 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1248 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2802 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Charsets.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3341 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Charsets.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5140 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4707 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     9499 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     6806 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      891 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/EscapeSequences.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1074 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/EscapeSequences.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1800 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1940 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3298 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3179 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    37312 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    43920 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     7597 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     9352 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      117 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Interfaces.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       91 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Interfaces.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    10087 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     9399 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     8951 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     6981 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    24426 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Parser.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    21493 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Parser.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    12074 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Renderer.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    11173 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Renderer.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    16912 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    15726 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    11175 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    10246 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2713 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2622 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     6473 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5425 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      112 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Types.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       86 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Types.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3818 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3869 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3481 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2988 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.test.js.map
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/attach/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3823 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/attach/attach.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       71 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/attach/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fit/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2942 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fit/fit.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       65 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fit/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fullscreen/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fullscreen/fullscreen.css
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1245 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fullscreen/fullscreen.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       79 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/fullscreen/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2925 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/SearchHelper.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3166 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/SearchHelper.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1038 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/search.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1141 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/search.js.map
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/terminado/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       77 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/terminado/package.json
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4182 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/addons/terminado/terminado.js
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/handlers/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2223 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2413 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      665 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      511 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.test.js.map
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/addons/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      337 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/addons/test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      431 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/addons/test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3584 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/escape-sequences-test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4525 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/escape-sequences-test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    39843 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    48497 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/test/test.js.map
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      778 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/Browser.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      879 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/Browser.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1303 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/BufferLine.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1289 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/BufferLine.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2557 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1615 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2597 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2224 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5940 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5427 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    10189 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    12167 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1724 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1518 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1820 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1709 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      209 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/Generic.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      235 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/Generic.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1523 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/Mouse.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1903 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/Mouse.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1438 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/TestUtils.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1173 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/utils/TestUtils.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    35217 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/xterm.css
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    52391 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/xterm.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    64536 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/lib/xterm.js.map
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     9705 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5500 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Buffer.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4715 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Buffer.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1287 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/BufferSet.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2389 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/BufferSet.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4442 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Charsets.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     8883 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/CompositionHelper.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     8951 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/CompositionHelper.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2461 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/EscapeSequences.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2535 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/EventEmitter.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1570 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/EventEmitter.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     8156 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/InputHandler.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    56684 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/InputHandler.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5620 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Interfaces.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     7199 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Linkifier.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    13483 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Linkifier.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    22646 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Parser.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    13690 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Renderer.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     9508 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/SelectionManager.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    21348 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/SelectionManager.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4978 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/SelectionModel.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3645 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/SelectionModel.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      427 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Types.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2815 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Viewport.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     5093 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/Viewport.ts
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/attach/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3823 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/attach/attach.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       71 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/attach/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fit/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2942 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fit/fit.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       65 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fit/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fullscreen/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      150 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fullscreen/fullscreen.css
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1245 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fullscreen/fullscreen.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       79 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/fullscreen/package.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/search/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3985 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/search/SearchHelper.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1576 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/search/search.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      193 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/search/tsconfig.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/terminado/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       77 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/terminado/package.json
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4182 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/addons/terminado/terminado.js
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/handlers/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      579 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/handlers/Clipboard.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3475 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/handlers/Clipboard.ts
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/test/
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/test/addons/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      338 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/test/addons/test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     4334 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/test/escape-sequences-test.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    36207 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/test/test.js
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      972 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/Browser.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1806 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/BufferLine.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2433 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/CharMeasure.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1837 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/CharMeasure.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     7888 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/CircularList.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     6211 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/CircularList.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1431 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/DomElementObjectPool.test.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2117 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/DomElementObjectPool.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      428 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/Generic.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     3119 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/Mouse.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     1602 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/utils/TestUtils.ts
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    35217 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/xterm.css
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)    65338 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/src/xterm.js
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      269 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/tsconfig.json
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      966 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/tslint.json
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      106 2023-04-27 02:48:36.000000 webconsole-0.0.5/webconsole/static/xterm/typings.json
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:44.000000 webconsole-0.0.5/webconsole/templates/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        0 2023-04-27 02:45:05.000000 webconsole-0.0.5/webconsole/templates/__init__.py
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)      869 2023-04-27 02:45:05.000000 webconsole-0.0.5/webconsole/templates/index.html
+drwxrwxr-x   0 raypick   (1000) raypick   (1000)        0 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole.egg-info/
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     2071 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)     9054 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)        1 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       66 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole.egg-info/requires.txt
+-rw-rw-r--   0 raypick   (1000) raypick   (1000)       11 2023-05-08 01:40:43.000000 webconsole-0.0.5/webconsole.egg-info/top_level.txt
```

### Comparing `webconsole-0.0.3/webconsole/docker/docker_console.py` & `webconsole-0.0.5/webconsole/docker/docker_console.py`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/linux/linux_console.py` & `webconsole-0.0.5/webconsole/linux/linux_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,14 @@
                     print("websocket has disconnected.")
                     lbc.chan.close()
                     break
             if message is not None:
                 lbc.chan.send(message)
                 handled_flag = False
             if message == '\r':
-                # import pdb; pdb.set_trace()
                 # \x0c : ctrl+l    \x7f : backspace   \x03 :  ETX
                 if tmp_message.strip() == 'exit':  # noqa
                     tmp_message = ''
                     loop_flag = False
                     handled_flag = False
                 else:
                     loop_flag = True
```

### Comparing `webconsole-0.0.3/webconsole/static/js/jquery-1.12.4.js` & `webconsole-0.0.5/webconsole/static/js/jquery-1.12.4.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/LICENSE` & `webconsole-0.0.5/webconsole/static/xterm/LICENSE`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/README.md` & `webconsole-0.0.5/webconsole/static/xterm/README.md`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/attach/attach.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/attach/attach.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/fit/fit.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/fit/fit.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/fullscreen/fullscreen.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/fullscreen/fullscreen.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/linkify/linkify.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/linkify/linkify.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/search/search.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/search/search.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/search/search.js.map` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/search/search.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/addons/terminado/terminado.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/addons/terminado/terminado.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/xterm.css` & `webconsole-0.0.5/webconsole/static/xterm/dist/xterm.css`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/xterm.js` & `webconsole-0.0.5/webconsole/static/xterm/dist/xterm.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/dist/xterm.js.map` & `webconsole-0.0.5/webconsole/static/xterm/dist/xterm.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/gulpfile.js` & `webconsole-0.0.5/webconsole/static/xterm/gulpfile.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Buffer.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Buffer.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/BufferSet.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/BufferSet.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Charsets.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Charsets.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Charsets.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Charsets.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/CompositionHelper.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/CompositionHelper.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/EscapeSequences.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/EscapeSequences.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/EscapeSequences.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/EscapeSequences.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/EventEmitter.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/EventEmitter.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/InputHandler.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/InputHandler.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Linkifier.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Linkifier.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Parser.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Parser.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Parser.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Parser.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Renderer.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Renderer.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Renderer.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Renderer.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionManager.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionManager.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/SelectionModel.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/SelectionModel.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/Viewport.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/Viewport.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/attach/attach.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/attach/attach.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/fit/fit.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/fit/fit.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/fullscreen/fullscreen.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/fullscreen/fullscreen.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/SearchHelper.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/SearchHelper.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/SearchHelper.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/SearchHelper.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/search.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/search.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/search/search.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/search/search.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/addons/terminado/terminado.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/addons/terminado/terminado.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/handlers/Clipboard.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/handlers/Clipboard.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/test/escape-sequences-test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/test/escape-sequences-test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/test/escape-sequences-test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/test/escape-sequences-test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/test/test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/test/test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/test/test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/test/test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/Browser.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/Browser.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/Browser.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/Browser.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/BufferLine.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/BufferLine.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/BufferLine.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/BufferLine.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CharMeasure.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CharMeasure.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/CircularList.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/CircularList.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/DomElementObjectPool.test.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/Mouse.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/Mouse.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/Mouse.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/Mouse.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/TestUtils.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/TestUtils.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/utils/TestUtils.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/utils/TestUtils.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/xterm.css` & `webconsole-0.0.5/webconsole/static/xterm/lib/xterm.css`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/xterm.js` & `webconsole-0.0.5/webconsole/static/xterm/lib/xterm.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/lib/xterm.js.map` & `webconsole-0.0.5/webconsole/static/xterm/lib/xterm.js.map`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/package.json` & `webconsole-0.0.5/webconsole/static/xterm/package.json`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Buffer.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Buffer.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Buffer.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Buffer.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/BufferSet.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/BufferSet.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/BufferSet.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/BufferSet.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Charsets.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Charsets.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/CompositionHelper.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/CompositionHelper.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/CompositionHelper.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/CompositionHelper.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/EscapeSequences.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/EscapeSequences.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/EventEmitter.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/EventEmitter.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/EventEmitter.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/EventEmitter.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/InputHandler.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/InputHandler.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/InputHandler.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/InputHandler.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Interfaces.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Interfaces.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Linkifier.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Linkifier.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Linkifier.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Linkifier.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Parser.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Parser.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Renderer.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Renderer.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/SelectionManager.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/SelectionManager.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/SelectionManager.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/SelectionManager.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/SelectionModel.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/SelectionModel.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/SelectionModel.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/SelectionModel.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Viewport.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Viewport.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/Viewport.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/Viewport.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/addons/attach/attach.js` & `webconsole-0.0.5/webconsole/static/xterm/src/addons/attach/attach.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/addons/fit/fit.js` & `webconsole-0.0.5/webconsole/static/xterm/src/addons/fit/fit.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/addons/fullscreen/fullscreen.js` & `webconsole-0.0.5/webconsole/static/xterm/src/addons/fullscreen/fullscreen.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/addons/search/SearchHelper.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/addons/search/SearchHelper.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/addons/search/search.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/addons/search/search.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/addons/terminado/terminado.js` & `webconsole-0.0.5/webconsole/static/xterm/src/addons/terminado/terminado.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/handlers/Clipboard.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/handlers/Clipboard.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/handlers/Clipboard.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/handlers/Clipboard.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/test/escape-sequences-test.js` & `webconsole-0.0.5/webconsole/static/xterm/src/test/escape-sequences-test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/test/test.js` & `webconsole-0.0.5/webconsole/static/xterm/src/test/test.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/Browser.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/Browser.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/BufferLine.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/BufferLine.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/CharMeasure.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/CharMeasure.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/CharMeasure.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/CharMeasure.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/CircularList.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/CircularList.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/CircularList.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/CircularList.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/DomElementObjectPool.test.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/DomElementObjectPool.test.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/DomElementObjectPool.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/DomElementObjectPool.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/Mouse.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/Mouse.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/utils/TestUtils.ts` & `webconsole-0.0.5/webconsole/static/xterm/src/utils/TestUtils.ts`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/xterm.css` & `webconsole-0.0.5/webconsole/static/xterm/src/xterm.css`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/src/xterm.js` & `webconsole-0.0.5/webconsole/static/xterm/src/xterm.js`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/static/xterm/tslint.json` & `webconsole-0.0.5/webconsole/static/xterm/tslint.json`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole/templates/index.html` & `webconsole-0.0.5/webconsole/templates/index.html`

 * *Files identical despite different names*

### Comparing `webconsole-0.0.3/webconsole.egg-info/SOURCES.txt` & `webconsole-0.0.5/webconsole.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+README.md
 setup.py
 webconsole/__init__.py
 webconsole.egg-info/PKG-INFO
 webconsole.egg-info/SOURCES.txt
 webconsole.egg-info/dependency_links.txt
 webconsole.egg-info/requires.txt
 webconsole.egg-info/top_level.txt
```

