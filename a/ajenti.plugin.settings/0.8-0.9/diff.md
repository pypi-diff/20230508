# Comparing `tmp/ajenti.plugin.settings-0.8.tar.gz` & `tmp/ajenti.plugin.settings-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ajenti.plugin.settings-0.8.tar", last modified: Fri Feb 13 09:19:12 2015, max compression
+gzip compressed data, was "dist/ajenti.plugin.settings-0.9.tar", last modified: Thu Mar 19 16:29:59 2015, max compression
```

## Comparing `ajenti.plugin.settings-0.8.tar` & `ajenti.plugin.settings-0.9.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      544 2015-02-13 09:17:48.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/plugin.yml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       25 2015-01-22 13:45:46.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      445 2015-01-22 13:02:30.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/main.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/partial/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     8700 2015-01-23 14:42:51.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/partial/index.html
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/services/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      973 2015-02-06 17:12:15.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/services/settings.service.coffee
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      200 2015-01-22 13:03:02.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/routing.coffee
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-01-22 12:28:56.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/module.coffee
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/controllers/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3101 2015-02-06 17:13:04.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/controllers/index.controller.coffee
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/build/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5038 2015-02-13 09:14:10.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/build/all.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:14:10.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/build/all.css
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3214 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/serialize.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4414 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/deferred.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      574 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/jquery.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1867 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/defaultDisplay.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1452 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/curCSS.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3198 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      509 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/addGetHookIf.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      380 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/hiddenVisibleSelectors.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      410 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/getStyles.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       45 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/rmargin.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      113 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/rnumnonpx.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      355 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/isHidden.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       70 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/cssExpand.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      555 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/swap.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    18626 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    59443 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    29161 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      240 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/_evalUrl.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      975 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/support.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/var/rcheckableType.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      200 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1393 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/intro.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      322 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event/ajax.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1094 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event/alias.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      123 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      294 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/selector-sizzle.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    12346 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/parseXML.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1669 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/load.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2516 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/jsonp.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1271 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/script.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      222 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/parseJSON.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3488 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/xhr.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       40 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/var/rquery.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       73 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/var/nonce.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    21168 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    11580 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       33 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/selector.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4434 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/selector-native.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4535 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    16914 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/effects.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5588 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/offset.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1496 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/wrap.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    24475 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4942 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        5 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/outro.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3063 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/queue.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2464 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/findFilter.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      110 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/var/rneedsContext.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/queue/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      561 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/queue/delay.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4155 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/classes.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1854 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/prop.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      893 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3839 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/val.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3320 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/attr.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       80 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/pnum.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       92 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/hasOwn.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       61 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/push.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       86 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/toString.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/indexOf.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       99 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/support.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       62 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/slice.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/strundefined.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/class2type.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       42 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/rnotwhite.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       36 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/arr.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       63 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/var/concat.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2381 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/ready.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      938 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/parseHTML.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3401 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/init.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1210 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/access.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       91 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/var/rsingleTag.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    15039 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/effects/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      225 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/effects/animatedSelector.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3028 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/effects/Tween.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4882 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/Data.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/var/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/var/data_user.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/var/data_priv.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      383 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/accepts.js
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/exports/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      641 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/exports/global.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1006 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/exports/amd.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      223 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/deprecated.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1776 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/dimensions.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5506 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/callbacks.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      731 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/.bower.json
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)   127542 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.map
--rw-rw-r--   0 eugene    (1000) eugene    (1000)   247387 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    84355 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      435 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/bower.json
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1099 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/MIT-LICENSE.txt
--rw-rw-rw-   0 eugene    (1000) eugene    (1000)     3526 2015-02-06 16:40:38.000000 ajenti.plugin.settings-0.8/ajenti_plugin_settings/views.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/PKG-INFO
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       23 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       43 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     6839 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       43 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/requirements.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      222 2015-02-13 09:19:12.000000 ajenti.plugin.settings-0.8/MANIFEST.in
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      622 2015-03-19 16:28:00.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/plugin.yml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       25 2015-01-22 13:45:46.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      444 2015-03-17 12:28:16.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/main.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/partial/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     8700 2015-01-23 14:42:51.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/partial/index.html
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/services/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      973 2015-02-06 17:12:15.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/services/settings.service.coffee
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      200 2015-01-22 13:03:02.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/routing.coffee
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       96 2015-03-19 15:01:41.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/module.coffee
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/controllers/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3101 2015-02-06 17:13:04.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/controllers/index.controller.coffee
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/build/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5076 2015-03-19 16:29:26.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/build/all.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:26.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/build/all.css
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3214 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/serialize.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4414 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/deferred.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      574 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/jquery.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1867 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/defaultDisplay.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1452 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/curCSS.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3198 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      509 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/addGetHookIf.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      380 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/hiddenVisibleSelectors.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      410 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/getStyles.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       45 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/rmargin.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      113 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/rnumnonpx.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      355 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/isHidden.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       70 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/var/cssExpand.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      555 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/swap.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    18626 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    59443 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    29161 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      240 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/_evalUrl.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      975 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/support.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/var/rcheckableType.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      200 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1393 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/intro.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      322 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event/ajax.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1094 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event/alias.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      123 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      294 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/selector-sizzle.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    12346 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/parseXML.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1669 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/load.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2516 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/jsonp.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1271 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/script.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      222 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/parseJSON.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3488 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/xhr.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       40 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/var/rquery.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       73 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/var/nonce.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    21168 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    11580 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       33 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/selector.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4434 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/selector-native.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4535 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    16914 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/effects.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5588 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/offset.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1496 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/wrap.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    24475 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4942 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        5 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/outro.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3063 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/queue.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2464 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/findFilter.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      110 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/var/rneedsContext.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/queue/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      561 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/queue/delay.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4155 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/classes.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1854 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/prop.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      893 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3839 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/val.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3320 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/attr.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       80 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/pnum.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       92 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/hasOwn.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       61 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/push.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       86 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/toString.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/indexOf.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       99 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/support.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       62 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/slice.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/strundefined.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       64 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/class2type.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       42 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/rnotwhite.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       36 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/arr.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       63 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/var/concat.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2381 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/ready.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      938 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/parseHTML.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3401 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/init.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1210 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/access.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       91 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/var/rsingleTag.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    15039 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/effects/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      225 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/effects/animatedSelector.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3028 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/effects/Tween.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4882 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/Data.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/var/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/var/data_user.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       66 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/var/data_priv.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      383 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/accepts.js
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/exports/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      641 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/exports/global.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1006 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/exports/amd.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      223 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/deprecated.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1776 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/dimensions.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5506 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/callbacks.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      731 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/.bower.json
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)   127542 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.map
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)   247387 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    84355 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      435 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/bower.json
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1099 2015-01-22 12:25:11.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/MIT-LICENSE.txt
+-rw-rw-rw-   0 eugene    (1000) eugene    (1000)     3525 2015-03-17 12:28:20.000000 ajenti.plugin.settings-0.9/ajenti_plugin_settings/views.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/PKG-INFO
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       23 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       68 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     6839 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       68 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/requirements.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      222 2015-03-19 16:29:59.000000 ajenti.plugin.settings-0.9/MANIFEST.in
```

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/plugin.yml` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/plugin.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 name: settings
 author: Ajenti project
 email: e@ajenti.org
 url: http://ajenti.org
-version: '0.8'
+version: '0.9'
 title: 'Settings'
 icon: wrench
 dependencies:
     - !!python/object:aj.plugins.PluginDependency { plugin_name: core }
+    - !!python/object:aj.plugins.PluginDependency { plugin_name: filesystem }
     - !!python/object:aj.plugins.PluginDependency { plugin_name: passwd }
 resources:
     - 'resources/js/module.coffee'
     - 'resources/js/routing.coffee'
     - 'resources/js/controllers/index.controller.coffee'
     - 'resources/js/services/settings.service.coffee'
     - 'resources/partial/index.html'
```

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/partial/index.html` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/partial/index.html`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/services/settings.service.coffee` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/services/settings.service.coffee`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/js/controllers/index.controller.coffee` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/js/controllers/index.controller.coffee`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/build/all.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/build/all.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // Generated by CoffeeScript 1.8.0
 (function() {
-    angular.module('ajenti.settings', ['core']);
+    angular.module('ajenti.settings', ['core', 'ajenti.filesystem', 'ajenti.passwd']);
 
 }).call(this);
 
 // Generated by CoffeeScript 1.8.0
 (function() {
     angular.module('core').config(function($routeProvider) {
         return $routeProvider.when('/view/settings', {
```

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/serialize.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/deferred.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/jquery.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/defaultDisplay.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/curCSS.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/support.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css/swap.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/support.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/intro.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event/alias.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/css.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/load.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/jsonp.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/script.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/xhr.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/ajax.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/selector-native.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/effects.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/offset.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/wrap.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/event.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/queue.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/findFilter.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/queue/delay.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/classes.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/prop.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/support.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/val.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/attr.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/ready.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/parseHTML.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/init.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/core/access.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/effects/Tween.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/data/Data.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/exports/global.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/exports/amd.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/dimensions.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/src/callbacks.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/.bower.json` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.map` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.js` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/resources/vendor/jquery/MIT-LICENSE.txt` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/resources/vendor/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.settings-0.8/ajenti_plugin_settings/views.py` & `ajenti.plugin.settings-0.9/ajenti_plugin_settings/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from aj.api.http import url, HttpPlugin
 from aj.config import UserConfig
 
 from aj.plugins.core.api.endpoint import endpoint
 
 
 @component(HttpPlugin)
-class Handler (HttpPlugin):
+class Handler(HttpPlugin):
     def __init__(self, context):
         self.context = context
 
     @url(r'/api/settings/config')
     @endpoint(api=True)
     def handle_api_config(self, http_context):
         if self.context.identity != 'root':
```

### Comparing `ajenti.plugin.settings-0.8/ajenti.plugin.settings.egg-info/SOURCES.txt` & `ajenti.plugin.settings-0.9/ajenti.plugin.settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

