# Comparing `tmp/ajenti.plugin.plugins-0.8.tar.gz` & `tmp/ajenti.plugin.plugins-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ajenti.plugin.plugins-0.8.tar", last modified: Fri Feb 13 09:21:21 2015, max compression
+gzip compressed data, was "dist/ajenti.plugin.plugins-0.9.tar", last modified: Fri Feb 13 10:12:17 2015, max compression
```

## Comparing `ajenti.plugin.plugins-0.8.tar` & `ajenti.plugin.plugins-0.9.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-02-13 09:21:20.000000 ajenti.plugin.plugins-0.8/setup.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      241 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/PKG-INFO
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       22 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       30 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      241 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     6722 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       29 2015-02-13 09:21:20.000000 ajenti.plugin.plugins-0.8/requirements.txt
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      415 2015-02-13 09:18:01.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/plugin.yml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       25 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      448 2015-02-12 16:34:47.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/main.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/partial/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5762 2015-02-13 09:04:48.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/partial/index.html
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2039 2015-02-13 08:20:00.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/partial/repo-plugin.html
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/js/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      197 2015-02-13 08:41:02.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/js/routing.coffee
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2015-02-12 16:35:44.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/js/module.coffee
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/js/controllers/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2705 2015-02-13 09:14:52.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/js/controllers/index.controller.coffee
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/build/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3866 2015-02-13 09:14:10.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/build/all.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:14:10.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/build/all.css
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3214 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/serialize.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4414 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/deferred.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      574 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/jquery.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1867 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/defaultDisplay.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1452 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/curCSS.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3198 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      509 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/addGetHookIf.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      380 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/hiddenVisibleSelectors.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      410 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/getStyles.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       45 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/rmargin.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      113 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/rnumnonpx.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      355 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/isHidden.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       70 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/cssExpand.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      555 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/swap.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    18626 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    59443 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    29161 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      240 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/_evalUrl.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      975 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/support.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/var/rcheckableType.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      200 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1393 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/intro.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      322 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event/ajax.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1094 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event/alias.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      123 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      294 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/selector-sizzle.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    12346 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/parseXML.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1669 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/load.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2516 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/jsonp.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1271 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/script.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      222 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/parseJSON.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3488 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/xhr.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       40 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/var/rquery.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       73 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/var/nonce.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    21168 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    11580 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       33 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/selector.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4434 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/selector-native.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4535 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    16914 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/effects.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5588 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/offset.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1496 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/wrap.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    24475 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4942 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        5 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/outro.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3063 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/queue.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2464 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/findFilter.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      110 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/var/rneedsContext.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/queue/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      561 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/queue/delay.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4155 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/classes.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1854 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/prop.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      893 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3839 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/val.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3320 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/attr.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       80 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/pnum.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       92 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/hasOwn.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       61 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/push.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       86 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/toString.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/indexOf.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       99 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       62 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/slice.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/strundefined.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/class2type.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       42 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/rnotwhite.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       36 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/arr.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       63 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/var/concat.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2381 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/ready.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      938 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/parseHTML.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3401 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/init.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1210 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/access.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       91 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/var/rsingleTag.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    15039 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      225 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/animatedSelector.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3028 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/Tween.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4882 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/Data.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/var/data_user.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/var/data_priv.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      383 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/accepts.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      641 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/global.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1006 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/amd.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      223 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/deprecated.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1776 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/dimensions.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5506 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/callbacks.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      731 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/.bower.json
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:21:21.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)   127542 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.map
--rw-rw-r--   0 eugene    (1000) eugene    (1000)   247387 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    84355 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      435 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/bower.json
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1099 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/MIT-LICENSE.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2272 2015-02-13 08:19:44.000000 ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/views.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      219 2015-02-13 09:21:20.000000 ajenti.plugin.plugins-0.8/MANIFEST.in
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/setup.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      241 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/PKG-INFO
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       22 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       30 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      241 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     6722 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       29 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/requirements.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      415 2015-02-13 10:11:42.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/plugin.yml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       25 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      448 2015-02-12 16:34:47.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/main.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/partial/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5747 2015-02-13 10:11:30.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/partial/index.html
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2039 2015-02-13 08:20:00.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/partial/repo-plugin.html
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/js/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      197 2015-02-13 08:41:02.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/js/routing.coffee
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2015-02-12 16:35:44.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/js/module.coffee
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/js/controllers/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2705 2015-02-13 09:14:52.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/js/controllers/index.controller.coffee
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/build/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3866 2015-02-13 09:14:10.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/build/all.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:14:10.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/build/all.css
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3214 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/serialize.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4414 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/deferred.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      574 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/jquery.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1867 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/defaultDisplay.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1452 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/curCSS.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3198 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      509 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/addGetHookIf.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      380 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/hiddenVisibleSelectors.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      410 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/getStyles.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       45 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/rmargin.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      113 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/rnumnonpx.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      355 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/isHidden.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       70 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/var/cssExpand.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      555 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/swap.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    18626 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    59443 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    29161 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      240 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/_evalUrl.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      975 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/support.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/var/rcheckableType.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      200 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1393 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/intro.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      322 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event/ajax.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1094 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event/alias.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      123 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      294 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/selector-sizzle.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    12346 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/parseXML.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1669 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/load.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2516 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/jsonp.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1271 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/script.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      222 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/parseJSON.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3488 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/xhr.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       40 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/var/rquery.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       73 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/var/nonce.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    21168 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    11580 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       33 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/selector.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4434 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/selector-native.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4535 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    16914 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/effects.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5588 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/offset.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1496 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/wrap.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    24475 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4942 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        5 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/outro.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3063 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/queue.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2464 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/findFilter.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      110 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/var/rneedsContext.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/queue/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      561 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/queue/delay.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4155 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/classes.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1854 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/prop.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      893 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3839 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/val.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3320 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/attr.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       80 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/pnum.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       92 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/hasOwn.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       61 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/push.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       86 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/toString.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/indexOf.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       99 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       62 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/slice.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/strundefined.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/class2type.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       42 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/rnotwhite.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       36 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/arr.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       63 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/var/concat.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2381 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/ready.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      938 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/parseHTML.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3401 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/init.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1210 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/access.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       91 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/var/rsingleTag.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    15039 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      225 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/animatedSelector.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3028 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/Tween.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4882 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/Data.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/var/data_user.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/var/data_priv.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      383 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/accepts.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      641 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/global.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1006 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/amd.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      223 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/deprecated.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1776 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/dimensions.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5506 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/callbacks.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      731 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/.bower.json
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)   127542 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.map
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)   247387 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    84355 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      435 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/bower.json
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1099 2015-02-12 16:34:04.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/MIT-LICENSE.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2272 2015-02-13 08:19:44.000000 ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/views.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      219 2015-02-13 10:12:17.000000 ajenti.plugin.plugins-0.9/MANIFEST.in
```

### Comparing `ajenti.plugin.plugins-0.8/ajenti.plugin.plugins.egg-info/SOURCES.txt` & `ajenti.plugin.plugins-0.9/ajenti.plugin.plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/partial/index.html` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/partial/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 <h3>Available plugins</h3>
 
 <progress-spinner ng:show="repoList == null"></progress-spinner>
 
 <div class="list-group">
-    <div class="list-group-item list-group-item-small" ng:repeat="plugin in repoList|orderBy:'title'" ng:hideeee="isInstalled(plugin)"> <!--TODO-->
+    <div class="list-group-item list-group-item-small" ng:repeat="plugin in repoList|orderBy:'title'" ng:hide="isInstalled(plugin)">
         <a ng:click="installPlugin(plugin)" class="list-group-btn" title="Install">
             <i class="fa fa-download"></i>
         </a>
         <a ng:click="$parent.selectedRepoPlugin = plugin" class="list-group-main">
             <i class="fa fa-fw fa-{{plugin.icon}}"></i> {{plugin.title}}
             &nbsp;
             <span class="subtle">{{plugin.name}} {{plugin.version}}</span>
```

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/partial/repo-plugin.html` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/partial/repo-plugin.html`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/js/controllers/index.controller.coffee` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/js/controllers/index.controller.coffee`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/build/all.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/build/all.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/serialize.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/deferred.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/jquery.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/defaultDisplay.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/curCSS.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/support.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css/swap.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/support.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/intro.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event/alias.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/css.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/load.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/jsonp.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/script.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/xhr.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/selector-native.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/effects.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/offset.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/wrap.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/event.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/queue.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/findFilter.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/queue/delay.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/classes.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/prop.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/support.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/val.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/attr.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/ready.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/parseHTML.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/init.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/core/access.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/Tween.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/data/Data.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/global.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/amd.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/dimensions.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/src/callbacks.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/.bower.json` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.map` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.js` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/resources/vendor/jquery/MIT-LICENSE.txt` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/resources/vendor/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.plugins-0.8/ajenti_plugin_plugins/views.py` & `ajenti.plugin.plugins-0.9/ajenti_plugin_plugins/views.py`

 * *Files identical despite different names*

