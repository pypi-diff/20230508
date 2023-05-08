# Comparing `tmp/selenium-4.9.0.tar.gz` & `tmp/selenium-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-4.9.0.tar", last modified: Sat Jan  1 00:00:00 2000, max compression
+gzip compressed data, was "selenium-4.9.1.tar", last modified: Sat Jan  1 00:00:00 2000, max compression
```

## Comparing `selenium-4.9.0.tar` & `selenium-4.9.1.tar`

### file list

```diff
@@ -1,337 +1,340 @@
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/
--rw-r--r--   0        0        0    46800 2000-01-01 00:00:00.000000 selenium-4.9.0/CHANGES
--rw-r--r--   0        0        0      834 2000-01-01 00:00:00.000000 selenium-4.9.0/MANIFEST.in
--rw-r--r--   0        0        0     7160 2000-01-01 00:00:00.000000 selenium-4.9.0/PKG-INFO
--rw-r--r--   0        0        0     6241 2000-01-01 00:00:00.000000 selenium-4.9.0/README.rst
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/
--rw-r--r--   0        0        0      811 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/__init__.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/common/
--rw-r--r--   0        0        0     3546 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/common/__init__.py
--rw-r--r--   0        0        0     8865 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/common/exceptions.py
--rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/py.typed
--rw-r--r--   0        0        0     1010 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/types.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/
--rw-r--r--   0        0        0     2415 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/__init__.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chrome/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chrome/__init__.py
--rw-r--r--   0        0        0     1380 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chrome/options.py
--rw-r--r--   0        0        0     2169 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chrome/service.py
--rw-r--r--   0        0        0     3997 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chrome/webdriver.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chromium/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chromium/__init__.py
--rw-r--r--   0        0        0     7362 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chromium/options.py
--rw-r--r--   0        0        0     2604 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chromium/remote_connection.py
--rw-r--r--   0        0        0     2417 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chromium/service.py
--rw-r--r--   0        0        0     9392 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/chromium/webdriver.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/__init__.py
--rw-r--r--   0        0        0    12955 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/action_chains.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/__init__.py
--rw-r--r--   0        0        0     3500 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/action_builder.py
--rw-r--r--   0        0        0     1184 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/input_device.py
--rw-r--r--   0        0        0     1438 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/interaction.py
--rw-r--r--   0        0        0     1786 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/key_actions.py
--rw-r--r--   0        0        0     1804 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/key_input.py
--rw-r--r--   0        0        0      879 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/mouse_button.py
--rw-r--r--   0        0        0     5850 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/pointer_actions.py
--rw-r--r--   0        0        0     2982 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/pointer_input.py
--rw-r--r--   0        0        0     1331 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/wheel_actions.py
--rw-r--r--   0        0        0     2610 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/actions/wheel_input.py
--rw-r--r--   0        0        0     2512 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/alert.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/bidi/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/bidi/__init__.py
--rw-r--r--   0        0        0    17766 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/bidi/cdp.py
--rw-r--r--   0        0        0      885 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/bidi/console.py
--rw-r--r--   0        0        0     1091 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/by.py
--rw-r--r--   0        0        0     2925 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/desired_capabilities.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/
--rw-r--r--   0        0        0     1293 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/__init__.py
--rw-r--r--   0        0        0    22199 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/accessibility.py
--rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/animation.py
--rw-r--r--   0        0        0    48312 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/audits.py
--rw-r--r--   0        0        0     5919 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/background_service.py
--rw-r--r--   0        0        0    20794 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/browser.py
--rw-r--r--   0        0        0     8286 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/cache_storage.py
--rw-r--r--   0        0        0     4382 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/cast.py
--rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/console.py
--rw-r--r--   0        0        0    59547 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/css.py
--rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/database.py
--rw-r--r--   0        0        0    49095 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/debugger.py
--rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/device_orientation.py
--rw-r--r--   0        0        0    61726 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom.py
--rw-r--r--   0        0        0     9459 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom_debugger.py
--rw-r--r--   0        0        0    36732 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom_snapshot.py
--rw-r--r--   0        0        0     5765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom_storage.py
--rw-r--r--   0        0        0    25819 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/emulation.py
--rw-r--r--   0        0        0     1289 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/event_breakpoints.py
--rw-r--r--   0        0        0    19105 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/fetch.py
--rw-r--r--   0        0        0     4576 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/headless_experimental.py
--rw-r--r--   0        0        0    13806 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/heap_profiler.py
--rw-r--r--   0        0        0    15159 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/indexed_db.py
--rw-r--r--   0        0        0    27841 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/input_.py
--rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/inspector.py
--rw-r--r--   0        0        0     3036 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/io.py
--rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/layer_tree.py
--rw-r--r--   0        0        0     5264 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/log.py
--rw-r--r--   0        0        0     7627 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/media.py
--rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/memory.py
--rw-r--r--   0        0        0   126116 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/network.py
--rw-r--r--   0        0        0    50256 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/overlay.py
--rw-r--r--   0        0        0   107219 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/page.py
--rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/performance.py
--rw-r--r--   0        0        0     6623 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/performance_timeline.py
--rw-r--r--   0        0        0    12930 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/profiler.py
--rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/py.typed
--rw-r--r--   0        0        0    57994 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/runtime.py
--rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/schema.py
--rw-r--r--   0        0        0    16861 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/security.py
--rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/service_worker.py
--rw-r--r--   0        0        0    31381 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/storage.py
--rw-r--r--   0        0        0    11517 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/system_info.py
--rw-r--r--   0        0        0    23888 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/target.py
--rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/tethering.py
--rw-r--r--   0        0        0    12886 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/tracing.py
--rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/util.py
--rw-r--r--   0        0        0    16895 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/web_audio.py
--rw-r--r--   0        0        0    15154 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v110/web_authn.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/
--rw-r--r--   0        0        0     1293 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/__init__.py
--rw-r--r--   0        0        0    22199 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/accessibility.py
--rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/animation.py
--rw-r--r--   0        0        0    48898 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/audits.py
--rw-r--r--   0        0        0     5919 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/background_service.py
--rw-r--r--   0        0        0    20861 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/browser.py
--rw-r--r--   0        0        0     8286 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/cache_storage.py
--rw-r--r--   0        0        0     4382 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/cast.py
--rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/console.py
--rw-r--r--   0        0        0    59547 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/css.py
--rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/database.py
--rw-r--r--   0        0        0    49095 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/debugger.py
--rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/device_orientation.py
--rw-r--r--   0        0        0    61726 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom.py
--rw-r--r--   0        0        0     9459 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom_debugger.py
--rw-r--r--   0        0        0    36732 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom_snapshot.py
--rw-r--r--   0        0        0     5765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom_storage.py
--rw-r--r--   0        0        0    25913 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/emulation.py
--rw-r--r--   0        0        0     1289 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/event_breakpoints.py
--rw-r--r--   0        0        0    19105 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/fetch.py
--rw-r--r--   0        0        0     4576 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/headless_experimental.py
--rw-r--r--   0        0        0    13806 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/heap_profiler.py
--rw-r--r--   0        0        0    15159 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/indexed_db.py
--rw-r--r--   0        0        0    27841 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/input_.py
--rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/inspector.py
--rw-r--r--   0        0        0     3036 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/io.py
--rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/layer_tree.py
--rw-r--r--   0        0        0     5264 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/log.py
--rw-r--r--   0        0        0     7627 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/media.py
--rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/memory.py
--rw-r--r--   0        0        0   126787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/network.py
--rw-r--r--   0        0        0    50256 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/overlay.py
--rw-r--r--   0        0        0   107897 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/page.py
--rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/performance.py
--rw-r--r--   0        0        0     6623 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/performance_timeline.py
--rw-r--r--   0        0        0    12930 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/profiler.py
--rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/py.typed
--rw-r--r--   0        0        0    58743 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/runtime.py
--rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/schema.py
--rw-r--r--   0        0        0    16861 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/security.py
--rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/service_worker.py
--rw-r--r--   0        0        0    31857 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/storage.py
--rw-r--r--   0        0        0    11517 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/system_info.py
--rw-r--r--   0        0        0    24094 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/target.py
--rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/tethering.py
--rw-r--r--   0        0        0    12886 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/tracing.py
--rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/util.py
--rw-r--r--   0        0        0    16895 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/web_audio.py
--rw-r--r--   0        0        0    15500 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v111/web_authn.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/
--rw-r--r--   0        0        0     1343 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/__init__.py
--rw-r--r--   0        0        0    22200 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/accessibility.py
--rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/animation.py
--rw-r--r--   0        0        0    45147 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/audits.py
--rw-r--r--   0        0        0     5919 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/background_service.py
--rw-r--r--   0        0        0    20861 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/browser.py
--rw-r--r--   0        0        0     8286 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/cache_storage.py
--rw-r--r--   0        0        0     4382 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/cast.py
--rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/console.py
--rw-r--r--   0        0        0    59551 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/css.py
--rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/database.py
--rw-r--r--   0        0        0    49095 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/debugger.py
--rw-r--r--   0        0        0     3322 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/device_access.py
--rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/device_orientation.py
--rw-r--r--   0        0        0    61795 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom.py
--rw-r--r--   0        0        0     9459 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom_debugger.py
--rw-r--r--   0        0        0    36732 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom_snapshot.py
--rw-r--r--   0        0        0     5765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom_storage.py
--rw-r--r--   0        0        0    26059 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/emulation.py
--rw-r--r--   0        0        0     1289 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/event_breakpoints.py
--rw-r--r--   0        0        0    19105 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/fetch.py
--rw-r--r--   0        0        0     4576 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/headless_experimental.py
--rw-r--r--   0        0        0    13806 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/heap_profiler.py
--rw-r--r--   0        0        0    15160 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/indexed_db.py
--rw-r--r--   0        0        0    27841 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/input_.py
--rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/inspector.py
--rw-r--r--   0        0        0     3036 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/io.py
--rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/layer_tree.py
--rw-r--r--   0        0        0     5264 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/log.py
--rw-r--r--   0        0        0     7627 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/media.py
--rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/memory.py
--rw-r--r--   0        0        0   126787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/network.py
--rw-r--r--   0        0        0    50256 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/overlay.py
--rw-r--r--   0        0        0   110999 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/page.py
--rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/performance.py
--rw-r--r--   0        0        0     6623 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/performance_timeline.py
--rw-r--r--   0        0        0     2580 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/preload.py
--rw-r--r--   0        0        0    12930 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/profiler.py
--rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/py.typed
--rw-r--r--   0        0        0    58743 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/runtime.py
--rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/schema.py
--rw-r--r--   0        0        0    16861 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/security.py
--rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/service_worker.py
--rw-r--r--   0        0        0    31857 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/storage.py
--rw-r--r--   0        0        0    11517 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/system_info.py
--rw-r--r--   0        0        0    24094 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/target.py
--rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/tethering.py
--rw-r--r--   0        0        0    12886 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/tracing.py
--rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/util.py
--rw-r--r--   0        0        0    16895 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/web_audio.py
--rw-r--r--   0        0        0    15500 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v112/web_authn.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/
--rw-r--r--   0        0        0     1258 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/__init__.py
--rw-r--r--   0        0        0    15011 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/accessibility.py
--rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/animation.py
--rw-r--r--   0        0        0     5735 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/application_cache.py
--rw-r--r--   0        0        0    17067 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/audits.py
--rw-r--r--   0        0        0     5760 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/background_service.py
--rw-r--r--   0        0        0    17298 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/browser.py
--rw-r--r--   0        0        0     7810 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/cache_storage.py
--rw-r--r--   0        0        0     3982 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/cast.py
--rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/console.py
--rw-r--r--   0        0        0    42907 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/css.py
--rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/database.py
--rw-r--r--   0        0        0    43473 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/debugger.py
--rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/device_orientation.py
--rw-r--r--   0        0        0    54390 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom.py
--rw-r--r--   0        0        0     8592 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom_debugger.py
--rw-r--r--   0        0        0    34069 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom_snapshot.py
--rw-r--r--   0        0        0     5026 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom_storage.py
--rw-r--r--   0        0        0    20775 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/emulation.py
--rw-r--r--   0        0        0    16053 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/fetch.py
--rw-r--r--   0        0        0     4791 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/headless_experimental.py
--rw-r--r--   0        0        0    11207 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/heap_profiler.py
--rw-r--r--   0        0        0    12762 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/indexed_db.py
--rw-r--r--   0        0        0    19701 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/input_.py
--rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/inspector.py
--rw-r--r--   0        0        0     3034 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/io.py
--rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/layer_tree.py
--rw-r--r--   0        0        0     5062 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/log.py
--rw-r--r--   0        0        0     6605 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/media.py
--rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/memory.py
--rw-r--r--   0        0        0    86888 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/network.py
--rw-r--r--   0        0        0    24823 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/overlay.py
--rw-r--r--   0        0        0    70797 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/page.py
--rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/performance.py
--rw-r--r--   0        0        0    17177 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/profiler.py
--rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/py.typed
--rw-r--r--   0        0        0    51695 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/runtime.py
--rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/schema.py
--rw-r--r--   0        0        0    16913 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/security.py
--rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/service_worker.py
--rw-r--r--   0        0        0     8277 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/storage.py
--rw-r--r--   0        0        0    11049 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/system_info.py
--rw-r--r--   0        0        0    18516 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/target.py
--rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/tethering.py
--rw-r--r--   0        0        0    10556 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/tracing.py
--rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/util.py
--rw-r--r--   0        0        0    16894 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/web_audio.py
--rw-r--r--   0        0        0     9424 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/devtools/v85/web_authn.py
--rw-r--r--   0        0        0     1660 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/driver_finder.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/html5/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/html5/__init__.py
--rw-r--r--   0        0        0     1626 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/html5/application_cache.py
--rw-r--r--   0        0        0     2317 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/keys.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/linux/
--rw-r--r--   0        0        0  4335456 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/linux/selenium-manager
--rw-r--r--   0        0        0     5913 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/log.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/macos/
--rw-r--r--   0        0        0  3614624 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/macos/selenium-manager
--rw-r--r--   0        0        0     1944 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/mutation-listener.js
--rw-r--r--   0        0        0     9123 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/options.py
--rw-r--r--   0        0        0     8607 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/print_page_options.py
--rw-r--r--   0        0        0    10533 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/proxy.py
--rw-r--r--   0        0        0     4475 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/selenium_manager.py
--rw-r--r--   0        0        0     8476 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/service.py
--rw-r--r--   0        0        0     3804 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/timeouts.py
--rw-r--r--   0        0        0     4458 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/utils.py
--rw-r--r--   0        0        0     7827 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/virtual_authenticator.py
--rw-r--r--   0        0        0      927 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/window.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/windows/
--rw-r--r--   0        0        0  3627520 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/common/windows/selenium-manager.exe
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/edge/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/edge/__init__.py
--rw-r--r--   0        0        0     1711 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/edge/options.py
--rw-r--r--   0        0        0     2725 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/edge/service.py
--rw-r--r--   0        0        0     3619 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/edge/webdriver.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/__init__.py
--rw-r--r--   0        0        0     2801 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/extension_connection.py
--rw-r--r--   0        0        0     8991 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/firefox_binary.py
--rw-r--r--   0        0        0    14364 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/firefox_profile.py
--rw-r--r--   0        0        0     5684 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/options.py
--rw-r--r--   0        0        0     1683 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/remote_connection.py
--rw-r--r--   0        0        0     2709 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/service.py
--rw-r--r--   0        0        0    14528 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/webdriver.py
--rw-r--r--   0        0        0     2826 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/firefox/webdriver_prefs.json
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/ie/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/ie/__init__.py
--rw-r--r--   0        0        0    11497 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/ie/options.py
--rw-r--r--   0        0        0     2473 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/ie/service.py
--rw-r--r--   0        0        0     5653 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/ie/webdriver.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/__init__.py
--rw-r--r--   0        0        0      968 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/bidi_connection.py
--rw-r--r--   0        0        0     4997 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/command.py
--rw-r--r--   0        0        0    11677 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/errorhandler.py
--rw-r--r--   0        0        0     1803 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/file_detector.py
--rw-r--r--   0        0        0    53824 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/findElements.js
--rw-r--r--   0        0        0    43157 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/getAttribute.js
--rw-r--r--   0        0        0    43996 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/isDisplayed.js
--rw-r--r--   0        0        0     2625 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/mobile.py
--rw-r--r--   0        0        0    16829 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/remote_connection.py
--rw-r--r--   0        0        0     1084 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/script_key.py
--rw-r--r--   0        0        0     2949 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/shadowroot.py
--rw-r--r--   0        0        0     5015 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/switch_to.py
--rw-r--r--   0        0        0      996 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/utils.py
--rw-r--r--   0        0        0    43299 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/webdriver.py
--rw-r--r--   0        0        0    17016 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/remote/webelement.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/__init__.py
--rw-r--r--   0        0        0     4284 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/options.py
--rw-r--r--   0        0        0      922 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/permissions.py
--rw-r--r--   0        0        0     1531 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/remote_connection.py
--rw-r--r--   0        0        0     3155 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/service.py
--rw-r--r--   0        0        0     6326 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/safari/webdriver.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/__init__.py
--rw-r--r--   0        0        0     2178 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/abstract_event_listener.py
--rw-r--r--   0        0        0    12207 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/color.py
--rw-r--r--   0        0        0     9193 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/event_firing_webdriver.py
--rw-r--r--   0        0        0      920 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/events.py
--rw-r--r--   0        0        0    14812 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/expected_conditions.py
--rw-r--r--   0        0        0     5930 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/relative_locator.py
--rw-r--r--   0        0        0     9276 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/select.py
--rw-r--r--   0        0        0      863 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/ui.py
--rw-r--r--   0        0        0     4868 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/support/wait.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/webkitgtk/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/webkitgtk/__init__.py
--rw-r--r--   0        0        0     2679 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/webkitgtk/options.py
--rw-r--r--   0        0        0     2301 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/webkitgtk/service.py
--rw-r--r--   0        0        0     3136 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/webkitgtk/webdriver.py
-drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/wpewebkit/
--rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/wpewebkit/__init__.py
--rw-r--r--   0        0        0     2207 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/wpewebkit/options.py
--rw-r--r--   0        0        0     2292 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/wpewebkit/service.py
--rw-r--r--   0        0        0     2932 2000-01-01 00:00:00.000000 selenium-4.9.0/selenium/webdriver/wpewebkit/webdriver.py
--rw-r--r--   0        0        0     3429 2000-01-01 00:00:00.000000 selenium-4.9.0/setup.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/
+-rw-r--r--   0        0        0    47017 2000-01-01 00:00:00.000000 selenium-4.9.1/CHANGES
+-rw-r--r--   0        0        0      834 2000-01-01 00:00:00.000000 selenium-4.9.1/MANIFEST.in
+-rw-r--r--   0        0        0     7163 2000-01-01 00:00:00.000000 selenium-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0     6241 2000-01-01 00:00:00.000000 selenium-4.9.1/README.rst
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/
+-rw-r--r--   0        0        0      811 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/__init__.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/common/
+-rw-r--r--   0        0        0     3546 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/common/__init__.py
+-rw-r--r--   0        0        0     8865 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/common/exceptions.py
+-rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/py.typed
+-rw-r--r--   0        0        0     1010 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/types.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/
+-rw-r--r--   0        0        0     2415 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/__init__.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chrome/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chrome/__init__.py
+-rw-r--r--   0        0        0     1380 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chrome/options.py
+-rw-r--r--   0        0        0     2169 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chrome/service.py
+-rw-r--r--   0        0        0     3997 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chrome/webdriver.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chromium/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chromium/__init__.py
+-rw-r--r--   0        0        0     7362 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chromium/options.py
+-rw-r--r--   0        0        0     2604 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chromium/remote_connection.py
+-rw-r--r--   0        0        0     2417 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chromium/service.py
+-rw-r--r--   0        0        0     9392 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/chromium/webdriver.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/__init__.py
+-rw-r--r--   0        0        0    12955 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/action_chains.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/__init__.py
+-rw-r--r--   0        0        0     3500 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/action_builder.py
+-rw-r--r--   0        0        0     1184 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/input_device.py
+-rw-r--r--   0        0        0     1438 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/interaction.py
+-rw-r--r--   0        0        0     1786 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/key_actions.py
+-rw-r--r--   0        0        0     1804 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/key_input.py
+-rw-r--r--   0        0        0      879 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/mouse_button.py
+-rw-r--r--   0        0        0     5850 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/pointer_actions.py
+-rw-r--r--   0        0        0     2982 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/pointer_input.py
+-rw-r--r--   0        0        0     1331 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/wheel_actions.py
+-rw-r--r--   0        0        0     2610 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/actions/wheel_input.py
+-rw-r--r--   0        0        0     2512 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/alert.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/bidi/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/bidi/__init__.py
+-rw-r--r--   0        0        0    17766 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/bidi/cdp.py
+-rw-r--r--   0        0        0      885 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/bidi/console.py
+-rw-r--r--   0        0        0     1091 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/by.py
+-rw-r--r--   0        0        0     2925 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/desired_capabilities.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/
+-rw-r--r--   0        0        0     1293 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/__init__.py
+-rw-r--r--   0        0        0    22199 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/accessibility.py
+-rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/animation.py
+-rw-r--r--   0        0        0    48898 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/audits.py
+-rw-r--r--   0        0        0     5919 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/background_service.py
+-rw-r--r--   0        0        0    20861 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/browser.py
+-rw-r--r--   0        0        0     8286 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/cache_storage.py
+-rw-r--r--   0        0        0     4382 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/cast.py
+-rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/console.py
+-rw-r--r--   0        0        0    59547 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/css.py
+-rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/database.py
+-rw-r--r--   0        0        0    49095 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/debugger.py
+-rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/device_orientation.py
+-rw-r--r--   0        0        0    61726 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom.py
+-rw-r--r--   0        0        0     9459 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom_debugger.py
+-rw-r--r--   0        0        0    36732 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom_snapshot.py
+-rw-r--r--   0        0        0     5765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom_storage.py
+-rw-r--r--   0        0        0    25913 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/emulation.py
+-rw-r--r--   0        0        0     1289 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/event_breakpoints.py
+-rw-r--r--   0        0        0    19105 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/fetch.py
+-rw-r--r--   0        0        0     4576 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/headless_experimental.py
+-rw-r--r--   0        0        0    13806 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/heap_profiler.py
+-rw-r--r--   0        0        0    15159 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/indexed_db.py
+-rw-r--r--   0        0        0    27841 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/input_.py
+-rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/inspector.py
+-rw-r--r--   0        0        0     3036 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/io.py
+-rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/layer_tree.py
+-rw-r--r--   0        0        0     5264 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/log.py
+-rw-r--r--   0        0        0     7627 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/media.py
+-rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/memory.py
+-rw-r--r--   0        0        0   126787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/network.py
+-rw-r--r--   0        0        0    50256 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/overlay.py
+-rw-r--r--   0        0        0   107897 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/page.py
+-rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/performance.py
+-rw-r--r--   0        0        0     6623 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/performance_timeline.py
+-rw-r--r--   0        0        0    12930 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/profiler.py
+-rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/py.typed
+-rw-r--r--   0        0        0    58743 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/runtime.py
+-rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/schema.py
+-rw-r--r--   0        0        0    16861 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/security.py
+-rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/service_worker.py
+-rw-r--r--   0        0        0    31857 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/storage.py
+-rw-r--r--   0        0        0    11517 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/system_info.py
+-rw-r--r--   0        0        0    24094 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/target.py
+-rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/tethering.py
+-rw-r--r--   0        0        0    12886 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/tracing.py
+-rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/util.py
+-rw-r--r--   0        0        0    16895 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/web_audio.py
+-rw-r--r--   0        0        0    15500 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v111/web_authn.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/
+-rw-r--r--   0        0        0     1343 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/__init__.py
+-rw-r--r--   0        0        0    22200 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/accessibility.py
+-rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/animation.py
+-rw-r--r--   0        0        0    45147 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/audits.py
+-rw-r--r--   0        0        0     5919 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/background_service.py
+-rw-r--r--   0        0        0    20861 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/browser.py
+-rw-r--r--   0        0        0     8286 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/cache_storage.py
+-rw-r--r--   0        0        0     4382 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/cast.py
+-rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/console.py
+-rw-r--r--   0        0        0    59551 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/css.py
+-rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/database.py
+-rw-r--r--   0        0        0    49095 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/debugger.py
+-rw-r--r--   0        0        0     3322 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/device_access.py
+-rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/device_orientation.py
+-rw-r--r--   0        0        0    61795 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom.py
+-rw-r--r--   0        0        0     9459 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom_debugger.py
+-rw-r--r--   0        0        0    36732 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom_snapshot.py
+-rw-r--r--   0        0        0     5765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom_storage.py
+-rw-r--r--   0        0        0    26059 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/emulation.py
+-rw-r--r--   0        0        0     1289 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/event_breakpoints.py
+-rw-r--r--   0        0        0    19105 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/fetch.py
+-rw-r--r--   0        0        0     4576 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/headless_experimental.py
+-rw-r--r--   0        0        0    13806 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/heap_profiler.py
+-rw-r--r--   0        0        0    15160 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/indexed_db.py
+-rw-r--r--   0        0        0    27841 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/input_.py
+-rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/inspector.py
+-rw-r--r--   0        0        0     3036 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/io.py
+-rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/layer_tree.py
+-rw-r--r--   0        0        0     5264 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/log.py
+-rw-r--r--   0        0        0     7627 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/media.py
+-rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/memory.py
+-rw-r--r--   0        0        0   126787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/network.py
+-rw-r--r--   0        0        0    50256 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/overlay.py
+-rw-r--r--   0        0        0   110999 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/page.py
+-rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/performance.py
+-rw-r--r--   0        0        0     6623 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/performance_timeline.py
+-rw-r--r--   0        0        0     2580 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/preload.py
+-rw-r--r--   0        0        0    12930 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/profiler.py
+-rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/py.typed
+-rw-r--r--   0        0        0    58743 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/runtime.py
+-rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/schema.py
+-rw-r--r--   0        0        0    16861 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/security.py
+-rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/service_worker.py
+-rw-r--r--   0        0        0    31857 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/storage.py
+-rw-r--r--   0        0        0    11517 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/system_info.py
+-rw-r--r--   0        0        0    24094 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/target.py
+-rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/tethering.py
+-rw-r--r--   0        0        0    12886 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/tracing.py
+-rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/util.py
+-rw-r--r--   0        0        0    16895 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/web_audio.py
+-rw-r--r--   0        0        0    15500 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v112/web_authn.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/
+-rw-r--r--   0        0        0     1364 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/__init__.py
+-rw-r--r--   0        0        0    22200 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/accessibility.py
+-rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/animation.py
+-rw-r--r--   0        0        0    45373 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/audits.py
+-rw-r--r--   0        0        0     5919 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/background_service.py
+-rw-r--r--   0        0        0    20861 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/browser.py
+-rw-r--r--   0        0        0     8286 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/cache_storage.py
+-rw-r--r--   0        0        0     4382 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/cast.py
+-rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/console.py
+-rw-r--r--   0        0        0    59947 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/css.py
+-rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/database.py
+-rw-r--r--   0        0        0    49095 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/debugger.py
+-rw-r--r--   0        0        0     3322 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/device_access.py
+-rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/device_orientation.py
+-rw-r--r--   0        0        0    61795 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom.py
+-rw-r--r--   0        0        0     9459 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom_debugger.py
+-rw-r--r--   0        0        0    36732 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom_snapshot.py
+-rw-r--r--   0        0        0     5765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom_storage.py
+-rw-r--r--   0        0        0    26059 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/emulation.py
+-rw-r--r--   0        0        0     1289 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/event_breakpoints.py
+-rw-r--r--   0        0        0     5178 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/fed_cm.py
+-rw-r--r--   0        0        0    19105 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/fetch.py
+-rw-r--r--   0        0        0     4576 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/headless_experimental.py
+-rw-r--r--   0        0        0    13806 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/heap_profiler.py
+-rw-r--r--   0        0        0    15160 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/indexed_db.py
+-rw-r--r--   0        0        0    27841 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/input_.py
+-rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/inspector.py
+-rw-r--r--   0        0        0     3036 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/io.py
+-rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/layer_tree.py
+-rw-r--r--   0        0        0     5264 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/log.py
+-rw-r--r--   0        0        0     7627 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/media.py
+-rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/memory.py
+-rw-r--r--   0        0        0   126787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/network.py
+-rw-r--r--   0        0        0    50256 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/overlay.py
+-rw-r--r--   0        0        0   104698 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/page.py
+-rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/performance.py
+-rw-r--r--   0        0        0     6623 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/performance_timeline.py
+-rw-r--r--   0        0        0    14075 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/preload.py
+-rw-r--r--   0        0        0    12930 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/profiler.py
+-rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/py.typed
+-rw-r--r--   0        0        0    58743 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/runtime.py
+-rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/schema.py
+-rw-r--r--   0        0        0    16861 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/security.py
+-rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/service_worker.py
+-rw-r--r--   0        0        0    34968 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/storage.py
+-rw-r--r--   0        0        0    11517 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/system_info.py
+-rw-r--r--   0        0        0    24094 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/target.py
+-rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/tethering.py
+-rw-r--r--   0        0        0    12886 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/tracing.py
+-rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/util.py
+-rw-r--r--   0        0        0    16895 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/web_audio.py
+-rw-r--r--   0        0        0    15500 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v113/web_authn.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/
+-rw-r--r--   0        0        0     1258 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/__init__.py
+-rw-r--r--   0        0        0    15011 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/accessibility.py
+-rw-r--r--   0        0        0    11112 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/animation.py
+-rw-r--r--   0        0        0     5735 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/application_cache.py
+-rw-r--r--   0        0        0    17067 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/audits.py
+-rw-r--r--   0        0        0     5760 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/background_service.py
+-rw-r--r--   0        0        0    17298 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/browser.py
+-rw-r--r--   0        0        0     7810 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/cache_storage.py
+-rw-r--r--   0        0        0     3982 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/cast.py
+-rw-r--r--   0        0        0     2765 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/console.py
+-rw-r--r--   0        0        0    42907 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/css.py
+-rw-r--r--   0        0        0     3925 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/database.py
+-rw-r--r--   0        0        0    43473 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/debugger.py
+-rw-r--r--   0        0        0     1209 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/device_orientation.py
+-rw-r--r--   0        0        0    54390 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom.py
+-rw-r--r--   0        0        0     8592 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom_debugger.py
+-rw-r--r--   0        0        0    34069 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom_snapshot.py
+-rw-r--r--   0        0        0     5026 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom_storage.py
+-rw-r--r--   0        0        0    20775 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/emulation.py
+-rw-r--r--   0        0        0    16053 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/fetch.py
+-rw-r--r--   0        0        0     4791 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/headless_experimental.py
+-rw-r--r--   0        0        0    11207 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/heap_profiler.py
+-rw-r--r--   0        0        0    12762 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/indexed_db.py
+-rw-r--r--   0        0        0    19701 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/input_.py
+-rw-r--r--   0        0        0     1718 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/inspector.py
+-rw-r--r--   0        0        0     3034 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/io.py
+-rw-r--r--   0        0        0    15049 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/layer_tree.py
+-rw-r--r--   0        0        0     5062 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/log.py
+-rw-r--r--   0        0        0     6605 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/media.py
+-rw-r--r--   0        0        0     6808 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/memory.py
+-rw-r--r--   0        0        0    86888 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/network.py
+-rw-r--r--   0        0        0    24823 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/overlay.py
+-rw-r--r--   0        0        0    70797 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/page.py
+-rw-r--r--   0        0        0     2927 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/performance.py
+-rw-r--r--   0        0        0    17177 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/profiler.py
+-rw-r--r--   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/py.typed
+-rw-r--r--   0        0        0    51695 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/runtime.py
+-rw-r--r--   0        0        0     1111 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/schema.py
+-rw-r--r--   0        0        0    16913 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/security.py
+-rw-r--r--   0        0        0    11066 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/service_worker.py
+-rw-r--r--   0        0        0     8277 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/storage.py
+-rw-r--r--   0        0        0    11049 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/system_info.py
+-rw-r--r--   0        0        0    18516 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/target.py
+-rw-r--r--   0        0        0     1538 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/tethering.py
+-rw-r--r--   0        0        0    10556 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/tracing.py
+-rw-r--r--   0        0        0      455 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/util.py
+-rw-r--r--   0        0        0    16894 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/web_audio.py
+-rw-r--r--   0        0        0     9424 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/devtools/v85/web_authn.py
+-rw-r--r--   0        0        0     1660 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/driver_finder.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/html5/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/html5/__init__.py
+-rw-r--r--   0        0        0     1626 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/html5/application_cache.py
+-rw-r--r--   0        0        0     2317 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/keys.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/linux/
+-rw-r--r--   0        0        0  4335456 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/linux/selenium-manager
+-rw-r--r--   0        0        0     5913 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/log.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/macos/
+-rw-r--r--   0        0        0  3614624 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/macos/selenium-manager
+-rw-r--r--   0        0        0     1944 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/mutation-listener.js
+-rw-r--r--   0        0        0     9123 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/options.py
+-rw-r--r--   0        0        0     8607 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/print_page_options.py
+-rw-r--r--   0        0        0    10511 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/proxy.py
+-rw-r--r--   0        0        0     4317 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/selenium_manager.py
+-rw-r--r--   0        0        0     8476 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/service.py
+-rw-r--r--   0        0        0     3804 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/timeouts.py
+-rw-r--r--   0        0        0     4458 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/utils.py
+-rw-r--r--   0        0        0     7827 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/virtual_authenticator.py
+-rw-r--r--   0        0        0      927 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/window.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/windows/
+-rw-r--r--   0        0        0  3627520 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/common/windows/selenium-manager.exe
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/edge/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/edge/__init__.py
+-rw-r--r--   0        0        0     1711 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/edge/options.py
+-rw-r--r--   0        0        0     2725 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/edge/service.py
+-rw-r--r--   0        0        0     3619 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/edge/webdriver.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/__init__.py
+-rw-r--r--   0        0        0     2801 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/extension_connection.py
+-rw-r--r--   0        0        0     8991 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/firefox_binary.py
+-rw-r--r--   0        0        0    14364 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/firefox_profile.py
+-rw-r--r--   0        0        0     5684 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/options.py
+-rw-r--r--   0        0        0     1683 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/remote_connection.py
+-rw-r--r--   0        0        0     2709 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/service.py
+-rw-r--r--   0        0        0    14621 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/webdriver.py
+-rw-r--r--   0        0        0     2826 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/firefox/webdriver_prefs.json
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/ie/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/ie/__init__.py
+-rw-r--r--   0        0        0    11497 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/ie/options.py
+-rw-r--r--   0        0        0     2473 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/ie/service.py
+-rw-r--r--   0        0        0     5653 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/ie/webdriver.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/__init__.py
+-rw-r--r--   0        0        0      968 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/bidi_connection.py
+-rw-r--r--   0        0        0     4997 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/command.py
+-rw-r--r--   0        0        0    11677 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/errorhandler.py
+-rw-r--r--   0        0        0     1803 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/file_detector.py
+-rw-r--r--   0        0        0    53824 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/findElements.js
+-rw-r--r--   0        0        0    43157 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/getAttribute.js
+-rw-r--r--   0        0        0    43996 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/isDisplayed.js
+-rw-r--r--   0        0        0     2625 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/mobile.py
+-rw-r--r--   0        0        0    16829 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/remote_connection.py
+-rw-r--r--   0        0        0     1084 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/script_key.py
+-rw-r--r--   0        0        0     2949 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/shadowroot.py
+-rw-r--r--   0        0        0     5015 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/switch_to.py
+-rw-r--r--   0        0        0      996 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/utils.py
+-rw-r--r--   0        0        0    43299 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/webdriver.py
+-rw-r--r--   0        0        0    17016 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/remote/webelement.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/__init__.py
+-rw-r--r--   0        0        0     4284 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/options.py
+-rw-r--r--   0        0        0      922 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/permissions.py
+-rw-r--r--   0        0        0     1531 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/remote_connection.py
+-rw-r--r--   0        0        0     3155 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/service.py
+-rw-r--r--   0        0        0     6307 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/safari/webdriver.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/__init__.py
+-rw-r--r--   0        0        0     2178 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/abstract_event_listener.py
+-rw-r--r--   0        0        0    12207 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/color.py
+-rw-r--r--   0        0        0     9193 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/event_firing_webdriver.py
+-rw-r--r--   0        0        0      920 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/events.py
+-rw-r--r--   0        0        0    14812 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/expected_conditions.py
+-rw-r--r--   0        0        0     5930 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/relative_locator.py
+-rw-r--r--   0        0        0     9276 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/select.py
+-rw-r--r--   0        0        0      863 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/ui.py
+-rw-r--r--   0        0        0     4868 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/support/wait.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/webkitgtk/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/webkitgtk/__init__.py
+-rw-r--r--   0        0        0     2679 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/webkitgtk/options.py
+-rw-r--r--   0        0        0     2301 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/webkitgtk/service.py
+-rw-r--r--   0        0        0     3136 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/webkitgtk/webdriver.py
+drwxr-xr-x   0        0        0        0 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/wpewebkit/
+-rw-r--r--   0        0        0      787 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/wpewebkit/__init__.py
+-rw-r--r--   0        0        0     2207 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/wpewebkit/options.py
+-rw-r--r--   0        0        0     2292 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/wpewebkit/service.py
+-rw-r--r--   0        0        0     2932 2000-01-01 00:00:00.000000 selenium-4.9.1/selenium/webdriver/wpewebkit/webdriver.py
+-rw-r--r--   0        0        0     3432 2000-01-01 00:00:00.000000 selenium-4.9.1/setup.py
```

### Comparing `selenium-4.9.0/CHANGES` & `selenium-4.9.1/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Selenium 4.9.1
+* Add CDP files for v113 and remove v110
+* Minor fixes for docstring and dictionary declarations (#11975)
+* Update logging to match other bindings (#11990)
+* Support newer versions of urllib3 (#11993)
+
 Selenium 4.9.0
 * Remove "shadow_root" assertion in Python bindings for Firefox (#11821)
 * Simplify driver binary and driver location selecting (#11864)
 * Do not pass desired caps in Safari (#11854)
 * Selenium Manager get Browser Version from Options classes
 * Selenium Manager use binary from Browser Options
 * Adding v112 and removing v109
```

### Comparing `selenium-4.9.0/MANIFEST.in` & `selenium-4.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/PKG-INFO` & `selenium-4.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
-Requires-Dist: urllib3[socks]~=1.26
+Requires-Dist: urllib3[socks]>=1.26,<3
 Requires-Dist: trio~=0.17
 Requires-Dist: trio-websocket~=0.9
 Requires-Dist: certifi>=2021.10.8
-Version: 4.9.0
+Version: 4.9.1
 
 ======================
 Selenium Client Driver
 ======================
 
 Introduction
 ============
@@ -55,15 +55,15 @@
 Installing
 ==========
 
 If you have `pip <https://pip.pypa.io/>`_ on your system, you can simply install or upgrade the Python bindings::
 
     pip install -U selenium
 
-Alternately, you can download the source distribution from `PyPI <https://pypi.org/project/selenium/#files>`_ (e.g. selenium-4.9.0.tar.gz), unarchive it, and run::
+Alternately, you can download the source distribution from `PyPI <https://pypi.org/project/selenium/#files>`_ (e.g. selenium-4.9.1.tar.gz), unarchive it, and run::
 
     python setup.py install
 
 Note: You may want to consider using `virtualenv <http://www.virtualenv.org/>`_ to create isolated Python environments.
 
 Drivers
 =======
```

### Comparing `selenium-4.9.0/README.rst` & `selenium-4.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Installing
 ==========
 
 If you have `pip <https://pip.pypa.io/>`_ on your system, you can simply install or upgrade the Python bindings::
 
     pip install -U selenium
 
-Alternately, you can download the source distribution from `PyPI <https://pypi.org/project/selenium/#files>`_ (e.g. selenium-4.9.0.tar.gz), unarchive it, and run::
+Alternately, you can download the source distribution from `PyPI <https://pypi.org/project/selenium/#files>`_ (e.g. selenium-4.9.1.tar.gz), unarchive it, and run::
 
     python setup.py install
 
 Note: You may want to consider using `virtualenv <http://www.virtualenv.org/>`_ to create isolated Python environments.
 
 Drivers
 =======
```

### Comparing `selenium-4.9.0/selenium/__init__.py` & `selenium-4.9.1/selenium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "4.9.0"
+__version__ = "4.9.1"
```

### Comparing `selenium-4.9.0/selenium/common/__init__.py` & `selenium-4.9.1/selenium/common/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/common/exceptions.py` & `selenium-4.9.1/selenium/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/types.py` & `selenium-4.9.1/selenium/types.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/__init__.py` & `selenium-4.9.1/selenium/webdriver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .remote.webdriver import WebDriver as Remote  # noqa
 from .safari.webdriver import WebDriver as Safari  # noqa
 from .webkitgtk.options import Options as WebKitGTKOptions  # noqa
 from .webkitgtk.webdriver import WebDriver as WebKitGTK  # noqa
 from .wpewebkit.options import Options as WPEWebKitOptions  # noqa
 from .wpewebkit.webdriver import WebDriver as WPEWebKit  # noqa
 
-__version__ = "4.9.0"
+__version__ = "4.9.1"
 
 # We need an explicit __all__ because the above won't otherwise be exported.
 __all__ = [
     "Firefox",
     "FirefoxProfile",
     "FirefoxOptions",
     "Chrome",
```

### Comparing `selenium-4.9.0/selenium/webdriver/chrome/__init__.py` & `selenium-4.9.1/selenium/webdriver/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chrome/options.py` & `selenium-4.9.1/selenium/webdriver/chrome/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chrome/service.py` & `selenium-4.9.1/selenium/webdriver/chrome/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chrome/webdriver.py` & `selenium-4.9.1/selenium/webdriver/chrome/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chromium/__init__.py` & `selenium-4.9.1/selenium/webdriver/chromium/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chromium/options.py` & `selenium-4.9.1/selenium/webdriver/chromium/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chromium/remote_connection.py` & `selenium-4.9.1/selenium/webdriver/chromium/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chromium/service.py` & `selenium-4.9.1/selenium/webdriver/chromium/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/chromium/webdriver.py` & `selenium-4.9.1/selenium/webdriver/chromium/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/action_chains.py` & `selenium-4.9.1/selenium/webdriver/common/action_chains.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/action_builder.py` & `selenium-4.9.1/selenium/webdriver/common/actions/action_builder.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/input_device.py` & `selenium-4.9.1/selenium/webdriver/common/actions/input_device.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/interaction.py` & `selenium-4.9.1/selenium/webdriver/common/actions/interaction.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/key_actions.py` & `selenium-4.9.1/selenium/webdriver/common/actions/key_actions.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/key_input.py` & `selenium-4.9.1/selenium/webdriver/common/actions/key_input.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/mouse_button.py` & `selenium-4.9.1/selenium/webdriver/common/actions/mouse_button.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/pointer_actions.py` & `selenium-4.9.1/selenium/webdriver/common/actions/pointer_actions.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/pointer_input.py` & `selenium-4.9.1/selenium/webdriver/common/actions/pointer_input.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/wheel_actions.py` & `selenium-4.9.1/selenium/webdriver/common/actions/wheel_actions.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/actions/wheel_input.py` & `selenium-4.9.1/selenium/webdriver/common/actions/wheel_input.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/alert.py` & `selenium-4.9.1/selenium/webdriver/common/alert.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/bidi/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/bidi/cdp.py` & `selenium-4.9.1/selenium/webdriver/common/bidi/cdp.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/bidi/console.py` & `selenium-4.9.1/selenium/webdriver/common/bidi/console.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/by.py` & `selenium-4.9.1/selenium/webdriver/common/by.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/desired_capabilities.py` & `selenium-4.9.1/selenium/webdriver/common/desired_capabilities.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/accessibility.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/accessibility.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/animation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/animation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/audits.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/audits.py`

 * *Files 1% similar despite different names*

```diff
@@ -788,14 +788,18 @@
             location=SourceCodeLocation.from_json(json['location']) if 'location' in json else None,
         )
 
 
 class GenericIssueErrorType(enum.Enum):
     CROSS_ORIGIN_PORTAL_POST_MESSAGE_ERROR = "CrossOriginPortalPostMessageError"
     FORM_LABEL_FOR_NAME_ERROR = "FormLabelForNameError"
+    FORM_DUPLICATE_ID_FOR_INPUT_ERROR = "FormDuplicateIdForInputError"
+    FORM_INPUT_WITH_NO_LABEL_ERROR = "FormInputWithNoLabelError"
+    FORM_AUTOCOMPLETE_ATTRIBUTE_EMPTY_ERROR = "FormAutocompleteAttributeEmptyError"
+    FORM_EMPTY_ID_AND_NAME_ATTRIBUTES_FOR_INPUT_ERROR = "FormEmptyIdAndNameAttributesForInputError"
 
     def to_json(self):
         return self.value
 
     @classmethod
     def from_json(cls, json):
         return cls(json)
@@ -854,28 +858,30 @@
     INSECURE_PRIVATE_NETWORK_SUBRESOURCE_REQUEST = "InsecurePrivateNetworkSubresourceRequest"
     LOCAL_CSS_FILE_EXTENSION_REJECTED = "LocalCSSFileExtensionRejected"
     MEDIA_SOURCE_ABORT_REMOVE = "MediaSourceAbortRemove"
     MEDIA_SOURCE_DURATION_TRUNCATING_BUFFERED = "MediaSourceDurationTruncatingBuffered"
     NO_SYSEX_WEB_MIDI_WITHOUT_PERMISSION = "NoSysexWebMIDIWithoutPermission"
     NOTIFICATION_INSECURE_ORIGIN = "NotificationInsecureOrigin"
     NOTIFICATION_PERMISSION_REQUESTED_IFRAME = "NotificationPermissionRequestedIframe"
+    OBSOLETE_CREATE_IMAGE_BITMAP_IMAGE_ORIENTATION_NONE = "ObsoleteCreateImageBitmapImageOrientationNone"
     OBSOLETE_WEB_RTC_CIPHER_SUITE = "ObsoleteWebRtcCipherSuite"
     OPEN_WEB_DATABASE_INSECURE_CONTEXT = "OpenWebDatabaseInsecureContext"
     OVERFLOW_VISIBLE_ON_REPLACED_ELEMENT = "OverflowVisibleOnReplacedElement"
     PAYMENT_INSTRUMENTS = "PaymentInstruments"
     PAYMENT_REQUEST_CSP_VIOLATION = "PaymentRequestCSPViolation"
     PERSISTENT_QUOTA_TYPE = "PersistentQuotaType"
     PICTURE_SOURCE_SRC = "PictureSourceSrc"
     PREFIXED_CANCEL_ANIMATION_FRAME = "PrefixedCancelAnimationFrame"
     PREFIXED_REQUEST_ANIMATION_FRAME = "PrefixedRequestAnimationFrame"
     PREFIXED_STORAGE_INFO = "PrefixedStorageInfo"
     PREFIXED_VIDEO_DISPLAYING_FULLSCREEN = "PrefixedVideoDisplayingFullscreen"
-    PREFIXED_VIDEO_ENTER_FULL_SCREEN = "PrefixedVideoEnterFullScreen"
-    PREFIXED_VIDEO_EXIT_FULL_SCREEN = "PrefixedVideoExitFullScreen"
+    PREFIXED_VIDEO_ENTER_FULLSCREEN = "PrefixedVideoEnterFullscreen"
+    PREFIXED_VIDEO_EXIT_FULLSCREEN = "PrefixedVideoExitFullscreen"
     PREFIXED_VIDEO_SUPPORTS_FULLSCREEN = "PrefixedVideoSupportsFullscreen"
+    PRIVACY_SANDBOX_EXTENSIONS_API = "PrivacySandboxExtensionsAPI"
     RANGE_EXPAND = "RangeExpand"
     REQUESTED_SUBRESOURCE_WITH_EMBEDDED_CREDENTIALS = "RequestedSubresourceWithEmbeddedCredentials"
     RTC_CONSTRAINT_ENABLE_DTLS_SRTP_FALSE = "RTCConstraintEnableDtlsSrtpFalse"
     RTC_CONSTRAINT_ENABLE_DTLS_SRTP_TRUE = "RTCConstraintEnableDtlsSrtpTrue"
     RTC_PEER_CONNECTION_COMPLEX_PLAN_B_SDP_USING_DEFAULT_SDP_SEMANTICS = "RTCPeerConnectionComplexPlanBSdpUsingDefaultSdpSemantics"
     RTC_PEER_CONNECTION_SDP_SEMANTICS_PLAN_B = "RTCPeerConnectionSdpSemanticsPlanB"
     RTCP_MUX_POLICY_NEGOTIATE = "RtcpMuxPolicyNegotiate"
@@ -959,28 +965,30 @@
     all cases except for success.
     '''
     SHOULD_EMBARGO = "ShouldEmbargo"
     TOO_MANY_REQUESTS = "TooManyRequests"
     WELL_KNOWN_HTTP_NOT_FOUND = "WellKnownHttpNotFound"
     WELL_KNOWN_NO_RESPONSE = "WellKnownNoResponse"
     WELL_KNOWN_INVALID_RESPONSE = "WellKnownInvalidResponse"
+    WELL_KNOWN_LIST_EMPTY = "WellKnownListEmpty"
     CONFIG_NOT_IN_WELL_KNOWN = "ConfigNotInWellKnown"
     WELL_KNOWN_TOO_BIG = "WellKnownTooBig"
     CONFIG_HTTP_NOT_FOUND = "ConfigHttpNotFound"
     CONFIG_NO_RESPONSE = "ConfigNoResponse"
     CONFIG_INVALID_RESPONSE = "ConfigInvalidResponse"
     CLIENT_METADATA_HTTP_NOT_FOUND = "ClientMetadataHttpNotFound"
     CLIENT_METADATA_NO_RESPONSE = "ClientMetadataNoResponse"
     CLIENT_METADATA_INVALID_RESPONSE = "ClientMetadataInvalidResponse"
     DISABLED_IN_SETTINGS = "DisabledInSettings"
     ERROR_FETCHING_SIGNIN = "ErrorFetchingSignin"
     INVALID_SIGNIN_RESPONSE = "InvalidSigninResponse"
     ACCOUNTS_HTTP_NOT_FOUND = "AccountsHttpNotFound"
     ACCOUNTS_NO_RESPONSE = "AccountsNoResponse"
     ACCOUNTS_INVALID_RESPONSE = "AccountsInvalidResponse"
+    ACCOUNTS_LIST_EMPTY = "AccountsListEmpty"
     ID_TOKEN_HTTP_NOT_FOUND = "IdTokenHttpNotFound"
     ID_TOKEN_NO_RESPONSE = "IdTokenNoResponse"
     ID_TOKEN_INVALID_RESPONSE = "IdTokenInvalidResponse"
     ID_TOKEN_INVALID_REQUEST = "IdTokenInvalidRequest"
     ERROR_ID_TOKEN = "ErrorIdToken"
     CANCELED = "Canceled"
     RP_PAGE_NOT_VISIBLE = "RpPageNotVisible"
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/background_service.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/background_service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/browser.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     NFC = "nfc"
     NOTIFICATIONS = "notifications"
     PAYMENT_HANDLER = "paymentHandler"
     PERIODIC_BACKGROUND_SYNC = "periodicBackgroundSync"
     PROTECTED_MEDIA_IDENTIFIER = "protectedMediaIdentifier"
     SENSORS = "sensors"
     STORAGE_ACCESS = "storageAccess"
+    TOP_LEVEL_STORAGE_ACCESS = "topLevelStorageAccess"
     VIDEO_CAPTURE = "videoCapture"
     VIDEO_CAPTURE_PAN_TILT_ZOOM = "videoCapturePanTiltZoom"
     WAKE_LOCK_SCREEN = "wakeLockScreen"
     WAKE_LOCK_SYSTEM = "wakeLockSystem"
     WINDOW_MANAGEMENT = "windowManagement"
 
     def to_json(self):
@@ -487,15 +488,15 @@
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.List[Histogram]]:
     '''
     Get Chrome histograms.
 
     **EXPERIMENTAL**
 
     :param query: *(Optional)* Requested substring in name. Only histograms which have query as a substring in their name are extracted. An empty or absent query returns all histograms.
-    :param delta: *(Optional)* If true, retrieve delta since last call.
+    :param delta: *(Optional)* If true, retrieve delta since last delta call.
     :returns: Histograms.
     '''
     params: T_JSON_DICT = dict()
     if query is not None:
         params['query'] = query
     if delta is not None:
         params['delta'] = delta
@@ -513,15 +514,15 @@
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,Histogram]:
     '''
     Get a Chrome histogram by name.
 
     **EXPERIMENTAL**
 
     :param name: Requested histogram name.
-    :param delta: *(Optional)* If true, retrieve delta since last call.
+    :param delta: *(Optional)* If true, retrieve delta since last delta call.
     :returns: Histogram.
     '''
     params: T_JSON_DICT = dict()
     params['name'] = name
     if delta is not None:
         params['delta'] = delta
     cmd_dict: T_JSON_DICT = {
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/cache_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/cache_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/cast.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/cast.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/console.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/console.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/css.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/css.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/database.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/database.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/device_orientation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/device_orientation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom_debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom_snapshot.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/dom_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/dom_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/emulation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/emulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,18 @@
 
     architecture: str
 
     model: str
 
     mobile: bool
 
+    #: Brands appearing in Sec-CH-UA.
     brands: typing.Optional[typing.List[UserAgentBrandVersion]] = None
 
+    #: Brands appearing in Sec-CH-UA-Full-Version-List.
     full_version_list: typing.Optional[typing.List[UserAgentBrandVersion]] = None
 
     full_version: typing.Optional[str] = None
 
     bitness: typing.Optional[str] = None
 
     wow64: typing.Optional[bool] = None
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/event_breakpoints.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/fetch.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/fetch.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/headless_experimental.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/heap_profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/indexed_db.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/indexed_db.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/input_.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/input_.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/inspector.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/inspector.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/io.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/io.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/layer_tree.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/layer_tree.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/log.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/log.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/media.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/media.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/memory.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/memory.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/network.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -748,36 +748,36 @@
 @dataclass
 class TrustTokenParams:
     '''
     Determines what type of Trust Token operation is executed and
     depending on the type, some additional parameters. The values
     are specified in third_party/blink/renderer/core/fetch/trust_token.idl.
     '''
-    type_: TrustTokenOperationType
+    operation: TrustTokenOperationType
 
-    #: Only set for "token-redemption" type and determine whether
+    #: Only set for "token-redemption" operation and determine whether
     #: to request a fresh SRR or use a still valid cached SRR.
     refresh_policy: str
 
     #: Origins of issuers from whom to request tokens or redemption
     #: records.
     issuers: typing.Optional[typing.List[str]] = None
 
     def to_json(self):
         json = dict()
-        json['type'] = self.type_.to_json()
+        json['operation'] = self.operation.to_json()
         json['refreshPolicy'] = self.refresh_policy
         if self.issuers is not None:
             json['issuers'] = [i for i in self.issuers]
         return json
 
     @classmethod
     def from_json(cls, json):
         return cls(
-            type_=TrustTokenOperationType.from_json(json['type']),
+            operation=TrustTokenOperationType.from_json(json['operation']),
             refresh_policy=str(json['refreshPolicy']),
             issuers=[str(i) for i in json['issuers']] if 'issuers' in json else None,
         )
 
 
 class TrustTokenOperationType(enum.Enum):
     ISSUANCE = "Issuance"
@@ -2403,14 +2403,15 @@
     json = yield cmd_dict
 
 
 def get_all_cookies() -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.List[Cookie]]:
     '''
     Returns all browser cookies. Depending on the backend support, will return detailed cookie
     information in the ``cookies`` field.
+    Deprecated. Use Storage.getCookies instead.
 
     :returns: Array of cookie objects.
     '''
     cmd_dict: T_JSON_DICT = {
         'method': 'Network.getAllCookies',
     }
     json = yield cmd_dict
@@ -3502,24 +3503,31 @@
     #: The status code of the response. This is useful in cases the request failed and no responseReceived
     #: event is triggered, which is the case for, e.g., CORS errors. This is also the correct status code
     #: for cached requests, where the status in responseReceived is a 200 and this will be 304.
     status_code: int
     #: Raw response header text as it was received over the wire. The raw text may not always be
     #: available, such as in the case of HTTP/2 or QUIC.
     headers_text: typing.Optional[str]
+    #: The cookie partition key that will be used to store partitioned cookies set in this response.
+    #: Only sent when partitioned cookies are enabled.
+    cookie_partition_key: typing.Optional[str]
+    #: True if partitioned cookies are enabled, but the partition key is not serializeable to string.
+    cookie_partition_key_opaque: typing.Optional[bool]
 
     @classmethod
     def from_json(cls, json: T_JSON_DICT) -> ResponseReceivedExtraInfo:
         return cls(
             request_id=RequestId.from_json(json['requestId']),
             blocked_cookies=[BlockedSetCookieWithReason.from_json(i) for i in json['blockedCookies']],
             headers=Headers.from_json(json['headers']),
             resource_ip_address_space=IPAddressSpace.from_json(json['resourceIPAddressSpace']),
             status_code=int(json['statusCode']),
-            headers_text=str(json['headersText']) if 'headersText' in json else None
+            headers_text=str(json['headersText']) if 'headersText' in json else None,
+            cookie_partition_key=str(json['cookiePartitionKey']) if 'cookiePartitionKey' in json else None,
+            cookie_partition_key_opaque=bool(json['cookiePartitionKeyOpaque']) if 'cookiePartitionKeyOpaque' in json else None
         )
 
 
 @event_class('Network.trustTokenOperationDone')
 @dataclass
 class TrustTokenOperationDone:
     '''
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/overlay.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/overlay.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/page.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,28 +219,31 @@
     LOCAL_FONTS = "local-fonts"
     MAGNETOMETER = "magnetometer"
     MICROPHONE = "microphone"
     MIDI = "midi"
     OTP_CREDENTIALS = "otp-credentials"
     PAYMENT = "payment"
     PICTURE_IN_PICTURE = "picture-in-picture"
+    PRIVATE_AGGREGATION = "private-aggregation"
     PUBLICKEY_CREDENTIALS_GET = "publickey-credentials-get"
     RUN_AD_AUCTION = "run-ad-auction"
     SCREEN_WAKE_LOCK = "screen-wake-lock"
     SERIAL = "serial"
     SHARED_AUTOFILL = "shared-autofill"
     SHARED_STORAGE = "shared-storage"
+    SHARED_STORAGE_SELECT_URL = "shared-storage-select-url"
     SMART_CARD = "smart-card"
     STORAGE_ACCESS = "storage-access"
     SYNC_XHR = "sync-xhr"
     TRUST_TOKEN_REDEMPTION = "trust-token-redemption"
     UNLOAD = "unload"
     USB = "usb"
     VERTICAL_SCROLL = "vertical-scroll"
     WEB_SHARE = "web-share"
+    WINDOW_MANAGEMENT = "window-management"
     WINDOW_PLACEMENT = "window-placement"
     XR_SPATIAL_TRACKING = "xr-spatial-tracking"
 
     def to_json(self):
         return self.value
 
     @classmethod
@@ -1338,14 +1341,15 @@
     SPEECH_SYNTHESIS = "SpeechSynthesis"
     KEYBOARD_LOCK = "KeyboardLock"
     WEB_OTP_SERVICE = "WebOTPService"
     OUTSTANDING_NETWORK_REQUEST_DIRECT_SOCKET = "OutstandingNetworkRequestDirectSocket"
     INJECTED_JAVASCRIPT = "InjectedJavascript"
     INJECTED_STYLE_SHEET = "InjectedStyleSheet"
     KEEPALIVE_REQUEST = "KeepaliveRequest"
+    INDEXED_DB_EVENT = "IndexedDBEvent"
     DUMMY = "Dummy"
     AUTHORIZATION_HEADER = "AuthorizationHeader"
     CONTENT_SECURITY_HANDLER = "ContentSecurityHandler"
     CONTENT_WEB_AUTHENTICATION_API = "ContentWebAuthenticationAPI"
     CONTENT_FILE_CHOOSER = "ContentFileChooser"
     CONTENT_SERIAL = "ContentSerial"
     CONTENT_FILE_SYSTEM_ACCESS = "ContentFileSystemAccess"
@@ -1497,14 +1501,20 @@
     SAME_SITE_CROSS_ORIGIN_REDIRECT = "SameSiteCrossOriginRedirect"
     SAME_SITE_CROSS_ORIGIN_NAVIGATION = "SameSiteCrossOriginNavigation"
     SAME_SITE_CROSS_ORIGIN_REDIRECT_NOT_OPT_IN = "SameSiteCrossOriginRedirectNotOptIn"
     SAME_SITE_CROSS_ORIGIN_NAVIGATION_NOT_OPT_IN = "SameSiteCrossOriginNavigationNotOptIn"
     ACTIVATION_NAVIGATION_PARAMETER_MISMATCH = "ActivationNavigationParameterMismatch"
     ACTIVATED_IN_BACKGROUND = "ActivatedInBackground"
     EMBEDDER_HOST_DISALLOWED = "EmbedderHostDisallowed"
+    ACTIVATION_NAVIGATION_DESTROYED_BEFORE_SUCCESS = "ActivationNavigationDestroyedBeforeSuccess"
+    TAB_CLOSED_BY_USER_GESTURE = "TabClosedByUserGesture"
+    TAB_CLOSED_WITHOUT_USER_GESTURE = "TabClosedWithoutUserGesture"
+    PRIMARY_MAIN_FRAME_RENDERER_PROCESS_CRASHED = "PrimaryMainFrameRendererProcessCrashed"
+    PRIMARY_MAIN_FRAME_RENDERER_PROCESS_KILLED = "PrimaryMainFrameRendererProcessKilled"
+    ACTIVATION_FRAME_POLICY_NOT_COMPATIBLE = "ActivationFramePolicyNotCompatible"
 
     def to_json(self):
         return self.value
 
     @classmethod
     def from_json(cls, json):
         return cls(json)
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/performance.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/performance.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/performance_timeline.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/runtime.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -798,14 +798,15 @@
         return_by_value: typing.Optional[bool] = None,
         generate_preview: typing.Optional[bool] = None,
         user_gesture: typing.Optional[bool] = None,
         await_promise: typing.Optional[bool] = None,
         execution_context_id: typing.Optional[ExecutionContextId] = None,
         object_group: typing.Optional[str] = None,
         throw_on_side_effect: typing.Optional[bool] = None,
+        unique_context_id: typing.Optional[str] = None,
         generate_web_driver_value: typing.Optional[bool] = None
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.Tuple[RemoteObject, typing.Optional[ExceptionDetails]]]:
     '''
     Calls function with given declaration on the given object. Object group of the result is
     inherited from the target object.
 
     :param function_declaration: Declaration of the function to call.
@@ -815,14 +816,15 @@
     :param return_by_value: *(Optional)* Whether the result is expected to be a JSON object which should be sent by value.
     :param generate_preview: **(EXPERIMENTAL)** *(Optional)* Whether preview should be generated for the result.
     :param user_gesture: *(Optional)* Whether execution should be treated as initiated by user in the UI.
     :param await_promise: *(Optional)* Whether execution should ````await```` for resulting value and return once awaited promise is resolved.
     :param execution_context_id: *(Optional)* Specifies execution context which global object will be used to call function on. Either executionContextId or objectId should be specified.
     :param object_group: *(Optional)* Symbolic group name that can be used to release multiple objects. If objectGroup is not specified and objectId is, objectGroup will be inherited from object.
     :param throw_on_side_effect: **(EXPERIMENTAL)** *(Optional)* Whether to throw an exception if side effect cannot be ruled out during evaluation.
+    :param unique_context_id: **(EXPERIMENTAL)** *(Optional)* An alternative way to specify the execution context to call function on. Compared to contextId that may be reused across processes, this is guaranteed to be system-unique, so it can be used to prevent accidental function call in context different than intended (e.g. as a result of navigation across process boundaries). This is mutually exclusive with ````executionContextId````.
     :param generate_web_driver_value: **(EXPERIMENTAL)** *(Optional)* Whether the result should contain ````webDriverValue````, serialized according to https://w3c.github.io/webdriver-bidi. This is mutually exclusive with ````returnByValue````, but resulting ````objectId``` is still provided.
     :returns: A tuple with the following items:
 
         0. **result** - Call result.
         1. **exceptionDetails** - *(Optional)* Exception details.
     '''
     params: T_JSON_DICT = dict()
@@ -843,14 +845,16 @@
         params['awaitPromise'] = await_promise
     if execution_context_id is not None:
         params['executionContextId'] = execution_context_id.to_json()
     if object_group is not None:
         params['objectGroup'] = object_group
     if throw_on_side_effect is not None:
         params['throwOnSideEffect'] = throw_on_side_effect
+    if unique_context_id is not None:
+        params['uniqueContextId'] = unique_context_id
     if generate_web_driver_value is not None:
         params['generateWebDriverValue'] = generate_web_driver_value
     cmd_dict: T_JSON_DICT = {
         'method': 'Runtime.callFunctionOn',
         'params': params,
     }
     json = yield cmd_dict
@@ -1492,19 +1496,22 @@
 @dataclass
 class ExecutionContextDestroyed:
     '''
     Issued when execution context is destroyed.
     '''
     #: Id of the destroyed context
     execution_context_id: ExecutionContextId
+    #: Unique Id of the destroyed context
+    execution_context_unique_id: str
 
     @classmethod
     def from_json(cls, json: T_JSON_DICT) -> ExecutionContextDestroyed:
         return cls(
-            execution_context_id=ExecutionContextId.from_json(json['executionContextId'])
+            execution_context_id=ExecutionContextId.from_json(json['executionContextId']),
+            execution_context_unique_id=str(json['executionContextUniqueId'])
         )
 
 
 @event_class('Runtime.executionContextsCleared')
 @dataclass
 class ExecutionContextsCleared:
     '''
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/schema.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/schema.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/security.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/security.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/service_worker.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/service_worker.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -911,14 +911,33 @@
     cmd_dict: T_JSON_DICT = {
         'method': 'Storage.clearSharedStorageEntries',
         'params': params,
     }
     json = yield cmd_dict
 
 
+def reset_shared_storage_budget(
+        owner_origin: str
+    ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
+    '''
+    Resets the budget for ``ownerOrigin`` by clearing all budget withdrawals.
+
+    **EXPERIMENTAL**
+
+    :param owner_origin:
+    '''
+    params: T_JSON_DICT = dict()
+    params['ownerOrigin'] = owner_origin
+    cmd_dict: T_JSON_DICT = {
+        'method': 'Storage.resetSharedStorageBudget',
+        'params': params,
+    }
+    json = yield cmd_dict
+
+
 def set_shared_storage_tracking(
         enable: bool
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
     '''
     Enables/disables issuing of sharedStorageAccessed events.
 
     **EXPERIMENTAL**
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/system_info.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/system_info.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/target.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,26 +326,28 @@
 def create_target(
         url: str,
         width: typing.Optional[int] = None,
         height: typing.Optional[int] = None,
         browser_context_id: typing.Optional[browser.BrowserContextID] = None,
         enable_begin_frame_control: typing.Optional[bool] = None,
         new_window: typing.Optional[bool] = None,
-        background: typing.Optional[bool] = None
+        background: typing.Optional[bool] = None,
+        for_tab: typing.Optional[bool] = None
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,TargetID]:
     '''
     Creates a new page.
 
     :param url: The initial URL the page will be navigated to. An empty string indicates about:blank.
     :param width: *(Optional)* Frame width in DIP (headless chrome only).
     :param height: *(Optional)* Frame height in DIP (headless chrome only).
     :param browser_context_id: **(EXPERIMENTAL)** *(Optional)* The browser context to create the page in.
     :param enable_begin_frame_control: **(EXPERIMENTAL)** *(Optional)* Whether BeginFrames for this target will be controlled via DevTools (headless chrome only, not supported on MacOS yet, false by default).
     :param new_window: *(Optional)* Whether to create a new Window or Tab (chrome-only, false by default).
     :param background: *(Optional)* Whether to create the target in background or foreground (chrome-only, false by default).
+    :param for_tab: **(EXPERIMENTAL)** *(Optional)* Whether to create the target of type "tab".
     :returns: The id of the page opened.
     '''
     params: T_JSON_DICT = dict()
     params['url'] = url
     if width is not None:
         params['width'] = width
     if height is not None:
@@ -354,14 +356,16 @@
         params['browserContextId'] = browser_context_id.to_json()
     if enable_begin_frame_control is not None:
         params['enableBeginFrameControl'] = enable_begin_frame_control
     if new_window is not None:
         params['newWindow'] = new_window
     if background is not None:
         params['background'] = background
+    if for_tab is not None:
+        params['forTab'] = for_tab
     cmd_dict: T_JSON_DICT = {
         'method': 'Target.createTarget',
         'params': params,
     }
     json = yield cmd_dict
     return TargetID.from_json(json['targetId'])
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/tethering.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/tethering.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/tracing.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/tracing.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/web_audio.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/web_audio.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v110/web_authn.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v111/web_authn.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,19 @@
     has_cred_blob: typing.Optional[bool] = None
 
     #: If set to true, the authenticator will support the minPinLength extension.
     #: https://fidoalliance.org/specs/fido-v2.1-ps-20210615/fido-client-to-authenticator-protocol-v2.1-ps-20210615.html#sctn-minpinlength-extension
     #: Defaults to false.
     has_min_pin_length: typing.Optional[bool] = None
 
+    #: If set to true, the authenticator will support the prf extension.
+    #: https://w3c.github.io/webauthn/#prf-extension
+    #: Defaults to false.
+    has_prf: typing.Optional[bool] = None
+
     #: If set to true, tests of user presence will succeed immediately.
     #: Otherwise, they will not be resolved. Defaults to true.
     automatic_presence_simulation: typing.Optional[bool] = None
 
     #: Sets whether User Verification succeeds or fails for an authenticator.
     #: Defaults to false.
     is_user_verified: typing.Optional[bool] = None
@@ -111,14 +116,16 @@
             json['hasUserVerification'] = self.has_user_verification
         if self.has_large_blob is not None:
             json['hasLargeBlob'] = self.has_large_blob
         if self.has_cred_blob is not None:
             json['hasCredBlob'] = self.has_cred_blob
         if self.has_min_pin_length is not None:
             json['hasMinPinLength'] = self.has_min_pin_length
+        if self.has_prf is not None:
+            json['hasPrf'] = self.has_prf
         if self.automatic_presence_simulation is not None:
             json['automaticPresenceSimulation'] = self.automatic_presence_simulation
         if self.is_user_verified is not None:
             json['isUserVerified'] = self.is_user_verified
         return json
 
     @classmethod
@@ -128,14 +135,15 @@
             transport=AuthenticatorTransport.from_json(json['transport']),
             ctap2_version=Ctap2Version.from_json(json['ctap2Version']) if 'ctap2Version' in json else None,
             has_resident_key=bool(json['hasResidentKey']) if 'hasResidentKey' in json else None,
             has_user_verification=bool(json['hasUserVerification']) if 'hasUserVerification' in json else None,
             has_large_blob=bool(json['hasLargeBlob']) if 'hasLargeBlob' in json else None,
             has_cred_blob=bool(json['hasCredBlob']) if 'hasCredBlob' in json else None,
             has_min_pin_length=bool(json['hasMinPinLength']) if 'hasMinPinLength' in json else None,
+            has_prf=bool(json['hasPrf']) if 'hasPrf' in json else None,
             automatic_presence_simulation=bool(json['automaticPresenceSimulation']) if 'automaticPresenceSimulation' in json else None,
             is_user_verified=bool(json['isUserVerified']) if 'isUserVerified' in json else None,
         )
 
 
 @dataclass
 class Credential:
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # DO NOT EDIT THIS FILE!
 #
 # This file is generated from the CDP specification. If you need to make
 # changes, edit the generator and regenerate all of the modules.
 from . import accessibility
 from . import animation
+from . import application_cache
 from . import audits
 from . import background_service
 from . import browser
 from . import css
 from . import cache_storage
 from . import cast
 from . import console
@@ -15,15 +16,14 @@
 from . import dom_debugger
 from . import dom_snapshot
 from . import dom_storage
 from . import database
 from . import debugger
 from . import device_orientation
 from . import emulation
-from . import event_breakpoints
 from . import fetch
 from . import headless_experimental
 from . import heap_profiler
 from . import io
 from . import indexed_db
 from . import input_
 from . import inspector
@@ -31,15 +31,14 @@
 from . import log
 from . import media
 from . import memory
 from . import network
 from . import overlay
 from . import page
 from . import performance
-from . import performance_timeline
 from . import profiler
 from . import runtime
 from . import schema
 from . import security
 from . import service_worker
 from . import storage
 from . import system_info
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/accessibility.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/accessibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
     Fetches the accessibility node and partial accessibility tree for this DOM node, if it exists.
 
     **EXPERIMENTAL**
 
     :param node_id: *(Optional)* Identifier of the node to get the partial accessibility tree for.
     :param backend_node_id: *(Optional)* Identifier of the backend node to get the partial accessibility tree for.
     :param object_id: *(Optional)* JavaScript object id of the node wrapper to get the partial accessibility tree for.
-    :param fetch_relatives: *(Optional)* Whether to fetch this nodes ancestors, siblings and children. Defaults to true.
+    :param fetch_relatives: *(Optional)* Whether to fetch this node's ancestors, siblings and children. Defaults to true.
     :returns: The ``Accessibility.AXNode`` for this DOM node, if it exists, plus its ancestors, siblings and children, if requested.
     '''
     params: T_JSON_DICT = dict()
     if node_id is not None:
         params['nodeId'] = node_id.to_json()
     if backend_node_id is not None:
         params['backendNodeId'] = backend_node_id.to_json()
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/animation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/animation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/audits.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/audits.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,24 +672,28 @@
             resource_ip_address_space=network.IPAddressSpace.from_json(json['resourceIPAddressSpace']) if 'resourceIPAddressSpace' in json else None,
             client_security_state=network.ClientSecurityState.from_json(json['clientSecurityState']) if 'clientSecurityState' in json else None,
         )
 
 
 class AttributionReportingIssueType(enum.Enum):
     PERMISSION_POLICY_DISABLED = "PermissionPolicyDisabled"
-    PERMISSION_POLICY_NOT_DELEGATED = "PermissionPolicyNotDelegated"
     UNTRUSTWORTHY_REPORTING_ORIGIN = "UntrustworthyReportingOrigin"
     INSECURE_CONTEXT = "InsecureContext"
     INVALID_HEADER = "InvalidHeader"
     INVALID_REGISTER_TRIGGER_HEADER = "InvalidRegisterTriggerHeader"
     INVALID_ELIGIBLE_HEADER = "InvalidEligibleHeader"
     TOO_MANY_CONCURRENT_REQUESTS = "TooManyConcurrentRequests"
     SOURCE_AND_TRIGGER_HEADERS = "SourceAndTriggerHeaders"
     SOURCE_IGNORED = "SourceIgnored"
     TRIGGER_IGNORED = "TriggerIgnored"
+    OS_SOURCE_IGNORED = "OsSourceIgnored"
+    OS_TRIGGER_IGNORED = "OsTriggerIgnored"
+    INVALID_REGISTER_OS_SOURCE_HEADER = "InvalidRegisterOsSourceHeader"
+    INVALID_REGISTER_OS_TRIGGER_HEADER = "InvalidRegisterOsTriggerHeader"
+    WEB_AND_OS_HEADERS = "WebAndOsHeaders"
 
     def to_json(self):
         return self.value
 
     @classmethod
     def from_json(cls, json):
         return cls(json)
@@ -792,14 +796,19 @@
 class GenericIssueErrorType(enum.Enum):
     CROSS_ORIGIN_PORTAL_POST_MESSAGE_ERROR = "CrossOriginPortalPostMessageError"
     FORM_LABEL_FOR_NAME_ERROR = "FormLabelForNameError"
     FORM_DUPLICATE_ID_FOR_INPUT_ERROR = "FormDuplicateIdForInputError"
     FORM_INPUT_WITH_NO_LABEL_ERROR = "FormInputWithNoLabelError"
     FORM_AUTOCOMPLETE_ATTRIBUTE_EMPTY_ERROR = "FormAutocompleteAttributeEmptyError"
     FORM_EMPTY_ID_AND_NAME_ATTRIBUTES_FOR_INPUT_ERROR = "FormEmptyIdAndNameAttributesForInputError"
+    FORM_ARIA_LABELLED_BY_TO_NON_EXISTING_ID = "FormAriaLabelledByToNonExistingId"
+    FORM_INPUT_ASSIGNED_AUTOCOMPLETE_VALUE_TO_ID_OR_NAME_ATTRIBUTE_ERROR = "FormInputAssignedAutocompleteValueToIdOrNameAttributeError"
+    FORM_LABEL_HAS_NEITHER_FOR_NOR_NESTED_INPUT = "FormLabelHasNeitherForNorNestedInput"
+    FORM_LABEL_FOR_MATCHES_NON_EXISTING_ID_ERROR = "FormLabelForMatchesNonExistingIdError"
+    FORM_INPUT_HAS_WRONG_BUT_WELL_INTENDED_AUTOCOMPLETE_VALUE_ERROR = "FormInputHasWrongButWellIntendedAutocompleteValueError"
 
     def to_json(self):
         return self.value
 
     @classmethod
     def from_json(cls, json):
         return cls(json)
@@ -831,104 +840,40 @@
         return cls(
             error_type=GenericIssueErrorType.from_json(json['errorType']),
             frame_id=page.FrameId.from_json(json['frameId']) if 'frameId' in json else None,
             violating_node_id=dom.BackendNodeId.from_json(json['violatingNodeId']) if 'violatingNodeId' in json else None,
         )
 
 
-class DeprecationIssueType(enum.Enum):
-    AUTHORIZATION_COVERED_BY_WILDCARD = "AuthorizationCoveredByWildcard"
-    CAN_REQUEST_URLHTTP_CONTAINING_NEWLINE = "CanRequestURLHTTPContainingNewline"
-    CHROME_LOAD_TIMES_CONNECTION_INFO = "ChromeLoadTimesConnectionInfo"
-    CHROME_LOAD_TIMES_FIRST_PAINT_AFTER_LOAD_TIME = "ChromeLoadTimesFirstPaintAfterLoadTime"
-    CHROME_LOAD_TIMES_WAS_ALTERNATE_PROTOCOL_AVAILABLE = "ChromeLoadTimesWasAlternateProtocolAvailable"
-    COOKIE_WITH_TRUNCATING_CHAR = "CookieWithTruncatingChar"
-    CROSS_ORIGIN_ACCESS_BASED_ON_DOCUMENT_DOMAIN = "CrossOriginAccessBasedOnDocumentDomain"
-    CROSS_ORIGIN_WINDOW_ALERT = "CrossOriginWindowAlert"
-    CROSS_ORIGIN_WINDOW_CONFIRM = "CrossOriginWindowConfirm"
-    CSS_SELECTOR_INTERNAL_MEDIA_CONTROLS_OVERLAY_CAST_BUTTON = "CSSSelectorInternalMediaControlsOverlayCastButton"
-    DEPRECATION_EXAMPLE = "DeprecationExample"
-    DOCUMENT_DOMAIN_SETTING_WITHOUT_ORIGIN_AGENT_CLUSTER_HEADER = "DocumentDomainSettingWithoutOriginAgentClusterHeader"
-    EVENT_PATH = "EventPath"
-    EXPECT_CT_HEADER = "ExpectCTHeader"
-    GEOLOCATION_INSECURE_ORIGIN = "GeolocationInsecureOrigin"
-    GEOLOCATION_INSECURE_ORIGIN_DEPRECATED_NOT_REMOVED = "GeolocationInsecureOriginDeprecatedNotRemoved"
-    GET_USER_MEDIA_INSECURE_ORIGIN = "GetUserMediaInsecureOrigin"
-    HOST_CANDIDATE_ATTRIBUTE_GETTER = "HostCandidateAttributeGetter"
-    IDENTITY_IN_CAN_MAKE_PAYMENT_EVENT = "IdentityInCanMakePaymentEvent"
-    INSECURE_PRIVATE_NETWORK_SUBRESOURCE_REQUEST = "InsecurePrivateNetworkSubresourceRequest"
-    LOCAL_CSS_FILE_EXTENSION_REJECTED = "LocalCSSFileExtensionRejected"
-    MEDIA_SOURCE_ABORT_REMOVE = "MediaSourceAbortRemove"
-    MEDIA_SOURCE_DURATION_TRUNCATING_BUFFERED = "MediaSourceDurationTruncatingBuffered"
-    NO_SYSEX_WEB_MIDI_WITHOUT_PERMISSION = "NoSysexWebMIDIWithoutPermission"
-    NOTIFICATION_INSECURE_ORIGIN = "NotificationInsecureOrigin"
-    NOTIFICATION_PERMISSION_REQUESTED_IFRAME = "NotificationPermissionRequestedIframe"
-    OBSOLETE_CREATE_IMAGE_BITMAP_IMAGE_ORIENTATION_NONE = "ObsoleteCreateImageBitmapImageOrientationNone"
-    OBSOLETE_WEB_RTC_CIPHER_SUITE = "ObsoleteWebRtcCipherSuite"
-    OPEN_WEB_DATABASE_INSECURE_CONTEXT = "OpenWebDatabaseInsecureContext"
-    OVERFLOW_VISIBLE_ON_REPLACED_ELEMENT = "OverflowVisibleOnReplacedElement"
-    PAYMENT_INSTRUMENTS = "PaymentInstruments"
-    PAYMENT_REQUEST_CSP_VIOLATION = "PaymentRequestCSPViolation"
-    PERSISTENT_QUOTA_TYPE = "PersistentQuotaType"
-    PICTURE_SOURCE_SRC = "PictureSourceSrc"
-    PREFIXED_CANCEL_ANIMATION_FRAME = "PrefixedCancelAnimationFrame"
-    PREFIXED_REQUEST_ANIMATION_FRAME = "PrefixedRequestAnimationFrame"
-    PREFIXED_STORAGE_INFO = "PrefixedStorageInfo"
-    PREFIXED_VIDEO_DISPLAYING_FULLSCREEN = "PrefixedVideoDisplayingFullscreen"
-    PREFIXED_VIDEO_ENTER_FULLSCREEN = "PrefixedVideoEnterFullscreen"
-    PREFIXED_VIDEO_EXIT_FULLSCREEN = "PrefixedVideoExitFullscreen"
-    PREFIXED_VIDEO_SUPPORTS_FULLSCREEN = "PrefixedVideoSupportsFullscreen"
-    PRIVACY_SANDBOX_EXTENSIONS_API = "PrivacySandboxExtensionsAPI"
-    RANGE_EXPAND = "RangeExpand"
-    REQUESTED_SUBRESOURCE_WITH_EMBEDDED_CREDENTIALS = "RequestedSubresourceWithEmbeddedCredentials"
-    RTC_CONSTRAINT_ENABLE_DTLS_SRTP_FALSE = "RTCConstraintEnableDtlsSrtpFalse"
-    RTC_CONSTRAINT_ENABLE_DTLS_SRTP_TRUE = "RTCConstraintEnableDtlsSrtpTrue"
-    RTC_PEER_CONNECTION_COMPLEX_PLAN_B_SDP_USING_DEFAULT_SDP_SEMANTICS = "RTCPeerConnectionComplexPlanBSdpUsingDefaultSdpSemantics"
-    RTC_PEER_CONNECTION_SDP_SEMANTICS_PLAN_B = "RTCPeerConnectionSdpSemanticsPlanB"
-    RTCP_MUX_POLICY_NEGOTIATE = "RtcpMuxPolicyNegotiate"
-    SHARED_ARRAY_BUFFER_CONSTRUCTED_WITHOUT_ISOLATION = "SharedArrayBufferConstructedWithoutIsolation"
-    TEXT_TO_SPEECH_DISALLOWED_BY_AUTOPLAY = "TextToSpeech_DisallowedByAutoplay"
-    V8_SHARED_ARRAY_BUFFER_CONSTRUCTED_IN_EXTENSION_WITHOUT_ISOLATION = "V8SharedArrayBufferConstructedInExtensionWithoutIsolation"
-    XHRJSON_ENCODING_DETECTION = "XHRJSONEncodingDetection"
-    XML_HTTP_REQUEST_SYNCHRONOUS_IN_NON_WORKER_OUTSIDE_BEFORE_UNLOAD = "XMLHttpRequestSynchronousInNonWorkerOutsideBeforeUnload"
-    XR_SUPPORTS_SESSION = "XRSupportsSession"
-
-    def to_json(self):
-        return self.value
-
-    @classmethod
-    def from_json(cls, json):
-        return cls(json)
-
-
 @dataclass
 class DeprecationIssueDetails:
     '''
     This issue tracks information needed to print a deprecation message.
     https://source.chromium.org/chromium/chromium/src/+/main:third_party/blink/renderer/core/frame/third_party/blink/renderer/core/frame/deprecation/README.md
     '''
     source_code_location: SourceCodeLocation
 
-    type_: DeprecationIssueType
+    #: One of the deprecation names from third_party/blink/renderer/core/frame/deprecation/deprecation.json5
+    type_: str
 
     affected_frame: typing.Optional[AffectedFrame] = None
 
     def to_json(self):
         json = dict()
         json['sourceCodeLocation'] = self.source_code_location.to_json()
-        json['type'] = self.type_.to_json()
+        json['type'] = self.type_
         if self.affected_frame is not None:
             json['affectedFrame'] = self.affected_frame.to_json()
         return json
 
     @classmethod
     def from_json(cls, json):
         return cls(
             source_code_location=SourceCodeLocation.from_json(json['sourceCodeLocation']),
-            type_=DeprecationIssueType.from_json(json['type']),
+            type_=str(json['type']),
             affected_frame=AffectedFrame.from_json(json['affectedFrame']) if 'affectedFrame' in json else None,
         )
 
 
 class ClientHintIssueReason(enum.Enum):
     META_TAG_ALLOW_LIST_INVALID_ORIGIN = "MetaTagAllowListInvalidOrigin"
     META_TAG_MODIFIED_HTML = "MetaTagModifiedHTML"
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/background_service.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/background_service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/browser.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/browser.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/cache_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/cache_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/cast.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/cast.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/console.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/console.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/css.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/css.py`

 * *Files 0% similar despite different names*

```diff
@@ -1463,15 +1463,15 @@
 
 def take_computed_style_updates() -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.List[dom.NodeId]]:
     '''
     Polls the next batch of computed style updates.
 
     **EXPERIMENTAL**
 
-    :returns: The list of node Ids that have their tracked computed styles updated
+    :returns: The list of node Ids that have their tracked computed styles updated.
     '''
     cmd_dict: T_JSON_DICT = {
         'method': 'CSS.takeComputedStyleUpdates',
     }
     json = yield cmd_dict
     return [dom.NodeId.from_json(i) for i in json['nodeIds']]
 
@@ -1706,29 +1706,29 @@
     }
     json = yield cmd_dict
 
 
 def stop_rule_usage_tracking() -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.List[RuleUsage]]:
     '''
     Stop tracking rule usage and return the list of rules that were used since last call to
-    ``takeCoverageDelta`` (or since start of coverage instrumentation)
+    ``takeCoverageDelta`` (or since start of coverage instrumentation).
 
     :returns: 
     '''
     cmd_dict: T_JSON_DICT = {
         'method': 'CSS.stopRuleUsageTracking',
     }
     json = yield cmd_dict
     return [RuleUsage.from_json(i) for i in json['ruleUsage']]
 
 
 def take_coverage_delta() -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.Tuple[typing.List[RuleUsage], float]]:
     '''
     Obtain list of rules that became used since last call to this method (or since start of coverage
-    instrumentation)
+    instrumentation).
 
     :returns: A tuple with the following items:
 
         0. **coverage** - 
         1. **timestamp** - Monotonically increasing time, in seconds.
     '''
     cmd_dict: T_JSON_DICT = {
@@ -1761,15 +1761,15 @@
 
 
 @event_class('CSS.fontsUpdated')
 @dataclass
 class FontsUpdated:
     '''
     Fires whenever a web font is updated.  A non-empty font parameter indicates a successfully loaded
-    web font
+    web font.
     '''
     #: The web font that has loaded.
     font: typing.Optional[FontFace]
 
     @classmethod
     def from_json(cls, json: T_JSON_DICT) -> FontsUpdated:
         return cls(
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/database.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/database.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/device_orientation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/device_orientation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom.py`

 * *Files 0% similar despite different names*

```diff
@@ -838,14 +838,15 @@
 
 def get_document(
         depth: typing.Optional[int] = None,
         pierce: typing.Optional[bool] = None
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,Node]:
     '''
     Returns the root DOM node (and optionally the subtree) to the caller.
+    Implicitly enables the DOM domain events for the current target.
 
     :param depth: *(Optional)* The maximum depth at which children should be retrieved, defaults to 1. Use -1 for the entire subtree or provide an integer larger than 0.
     :param pierce: *(Optional)* Whether or not iframes and shadow roots should be traversed when returning the subtree (default is false).
     :returns: Resulting node.
     '''
     params: T_JSON_DICT = dict()
     if depth is not None:
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom_debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom_snapshot.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/dom_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/dom_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/emulation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/emulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,15 +482,15 @@
         type_: str
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
     '''
     Emulates the given vision deficiency.
 
     **EXPERIMENTAL**
 
-    :param type_: Vision deficiency to emulate.
+    :param type_: Vision deficiency to emulate. Order: best-effort emulations come first, followed by any physiologically accurate emulations for medically recognized color vision deficiencies.
     '''
     params: T_JSON_DICT = dict()
     params['type'] = type_
     cmd_dict: T_JSON_DICT = {
         'method': 'Emulation.setEmulatedVisionDeficiency',
         'params': params,
     }
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/event_breakpoints.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/fetch.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/fetch.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/headless_experimental.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/heap_profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/indexed_db.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/indexed_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
 def get_metadata(
         security_origin: typing.Optional[str] = None,
         storage_key: typing.Optional[str] = None,
         database_name: str = None,
         object_store_name: str = None
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.Tuple[float, float]]:
     '''
-    Gets metadata of an object store
+    Gets metadata of an object store.
 
     :param security_origin: *(Optional)* At least and at most one of securityOrigin, storageKey must be specified. Security origin.
     :param storage_key: *(Optional)* Storage key.
     :param database_name: Database name.
     :param object_store_name: Object store name.
     :returns: A tuple with the following items:
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/input_.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/input_.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/inspector.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/inspector.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/io.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/io.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/layer_tree.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/layer_tree.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/log.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/log.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/media.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/media.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/memory.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/memory.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/network.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/network.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/overlay.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/overlay.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/page.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1226,14 +1226,31 @@
     def from_json(cls, json):
         return cls(
             url=str(json['url']),
             eager=bool(json['eager']) if 'eager' in json else None,
         )
 
 
+class AutoResponseMode(enum.Enum):
+    '''
+    Enum of possible auto-reponse for permisison / prompt dialogs.
+    '''
+    NONE = "none"
+    AUTO_ACCEPT = "autoAccept"
+    AUTO_REJECT = "autoReject"
+    AUTO_OPT_OUT = "autoOptOut"
+
+    def to_json(self):
+        return self.value
+
+    @classmethod
+    def from_json(cls, json):
+        return cls(json)
+
+
 class NavigationType(enum.Enum):
     '''
     The type of a frameNavigated event.
     '''
     NAVIGATION = "Navigation"
     BACK_FORWARD_CACHE_RESTORE = "BackForwardCacheRestore"
 
@@ -1507,14 +1524,38 @@
     EMBEDDER_HOST_DISALLOWED = "EmbedderHostDisallowed"
     ACTIVATION_NAVIGATION_DESTROYED_BEFORE_SUCCESS = "ActivationNavigationDestroyedBeforeSuccess"
     TAB_CLOSED_BY_USER_GESTURE = "TabClosedByUserGesture"
     TAB_CLOSED_WITHOUT_USER_GESTURE = "TabClosedWithoutUserGesture"
     PRIMARY_MAIN_FRAME_RENDERER_PROCESS_CRASHED = "PrimaryMainFrameRendererProcessCrashed"
     PRIMARY_MAIN_FRAME_RENDERER_PROCESS_KILLED = "PrimaryMainFrameRendererProcessKilled"
     ACTIVATION_FRAME_POLICY_NOT_COMPATIBLE = "ActivationFramePolicyNotCompatible"
+    PRELOADING_DISABLED = "PreloadingDisabled"
+    BATTERY_SAVER_ENABLED = "BatterySaverEnabled"
+    ACTIVATED_DURING_MAIN_FRAME_NAVIGATION = "ActivatedDuringMainFrameNavigation"
+    PRELOADING_UNSUPPORTED_BY_WEB_CONTENTS = "PreloadingUnsupportedByWebContents"
+
+    def to_json(self):
+        return self.value
+
+    @classmethod
+    def from_json(cls, json):
+        return cls(json)
+
+
+class PreloadingStatus(enum.Enum):
+    '''
+    Preloading status values, see also PreloadingTriggeringOutcome. This
+    status is shared by prefetchStatusUpdated and prerenderStatusUpdated.
+    '''
+    PENDING = "Pending"
+    RUNNING = "Running"
+    READY = "Ready"
+    SUCCESS = "Success"
+    FAILURE = "Failure"
+    NOT_SUPPORTED = "NotSupported"
 
     def to_json(self):
         return self.value
 
     @classmethod
     def from_json(cls, json):
         return cls(json)
@@ -1780,15 +1821,15 @@
     }
     json = yield cmd_dict
     return [InstallabilityError.from_json(i) for i in json['installabilityErrors']]
 
 
 def get_manifest_icons() -> typing.Generator[T_JSON_DICT,T_JSON_DICT,typing.Optional[str]]:
     '''
-
+    Deprecated because it's not guaranteed that the returned icon is in fact the one used for PWA installation.
 
     **EXPERIMENTAL**
 
     :returns: 
     '''
     cmd_dict: T_JSON_DICT = {
         'method': 'Page.getManifestIcons',
@@ -2726,33 +2767,53 @@
     cmd_dict: T_JSON_DICT = {
         'method': 'Page.clearCompilationCache',
     }
     json = yield cmd_dict
 
 
 def set_spc_transaction_mode(
-        mode: str
+        mode: AutoResponseMode
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
     '''
     Sets the Secure Payment Confirmation transaction mode.
     https://w3c.github.io/secure-payment-confirmation/#sctn-automation-set-spc-transaction-mode
 
     **EXPERIMENTAL**
 
     :param mode:
     '''
     params: T_JSON_DICT = dict()
-    params['mode'] = mode
+    params['mode'] = mode.to_json()
     cmd_dict: T_JSON_DICT = {
         'method': 'Page.setSPCTransactionMode',
         'params': params,
     }
     json = yield cmd_dict
 
 
+def set_rph_registration_mode(
+        mode: AutoResponseMode
+    ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
+    '''
+    Extensions for Custom Handlers API:
+    https://html.spec.whatwg.org/multipage/system-state.html#rph-automation
+
+    **EXPERIMENTAL**
+
+    :param mode:
+    '''
+    params: T_JSON_DICT = dict()
+    params['mode'] = mode.to_json()
+    cmd_dict: T_JSON_DICT = {
+        'method': 'Page.setRPHRegistrationMode',
+        'params': params,
+    }
+    json = yield cmd_dict
+
+
 def generate_test_report(
         message: str,
         group: typing.Optional[str] = None
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
     '''
     Generates a report for testing.
 
@@ -3250,14 +3311,60 @@
             initiating_frame_id=FrameId.from_json(json['initiatingFrameId']),
             prerendering_url=str(json['prerenderingUrl']),
             final_status=PrerenderFinalStatus.from_json(json['finalStatus']),
             disallowed_api_method=str(json['disallowedApiMethod']) if 'disallowedApiMethod' in json else None
         )
 
 
+@event_class('Page.prefetchStatusUpdated')
+@dataclass
+class PrefetchStatusUpdated:
+    '''
+    **EXPERIMENTAL**
+
+    TODO(crbug/1384419): Create a dedicated domain for preloading.
+    Fired when a prefetch attempt is updated.
+    '''
+    #: The frame id of the frame initiating prefetch.
+    initiating_frame_id: FrameId
+    prefetch_url: str
+    status: PreloadingStatus
+
+    @classmethod
+    def from_json(cls, json: T_JSON_DICT) -> PrefetchStatusUpdated:
+        return cls(
+            initiating_frame_id=FrameId.from_json(json['initiatingFrameId']),
+            prefetch_url=str(json['prefetchUrl']),
+            status=PreloadingStatus.from_json(json['status'])
+        )
+
+
+@event_class('Page.prerenderStatusUpdated')
+@dataclass
+class PrerenderStatusUpdated:
+    '''
+    **EXPERIMENTAL**
+
+    TODO(crbug/1384419): Create a dedicated domain for preloading.
+    Fired when a prerender attempt is updated.
+    '''
+    #: The frame id of the frame initiating prerender.
+    initiating_frame_id: FrameId
+    prerendering_url: str
+    status: PreloadingStatus
+
+    @classmethod
+    def from_json(cls, json: T_JSON_DICT) -> PrerenderStatusUpdated:
+        return cls(
+            initiating_frame_id=FrameId.from_json(json['initiatingFrameId']),
+            prerendering_url=str(json['prerenderingUrl']),
+            status=PreloadingStatus.from_json(json['status'])
+        )
+
+
 @event_class('Page.loadEventFired')
 @dataclass
 class LoadEventFired:
     timestamp: network.MonotonicTime
 
     @classmethod
     def from_json(cls, json: T_JSON_DICT) -> LoadEventFired:
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/performance.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/performance.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/performance_timeline.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/runtime.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/runtime.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/schema.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/schema.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/security.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/security.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/service_worker.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/service_worker.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/system_info.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/system_info.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/target.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/target.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/tethering.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/tethering.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/tracing.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/tracing.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/web_audio.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/web_audio.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v111/web_authn.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/web_authn.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/accessibility.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/accessibility.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/animation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/animation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/audits.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/audits.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/background_service.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/background_service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/browser.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/browser.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/cache_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/cache_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/cast.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/cast.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/console.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/console.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/css.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/css.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,17 @@
     #: Associated style declaration.
     style: CSSStyle
 
     #: The css style sheet identifier (absent for user agent stylesheet and user-specified
     #: stylesheet rules) this rule came from.
     style_sheet_id: typing.Optional[StyleSheetId] = None
 
+    #: Array of selectors from ancestor style rules, sorted by distance from the current rule.
+    nesting_selectors: typing.Optional[typing.List[str]] = None
+
     #: Media list array (for rules involving media queries). The array enumerates media queries
     #: starting with the innermost one, going outwards.
     media: typing.Optional[typing.List[CSSMedia]] = None
 
     #: Container query list array (for rules involving container queries).
     #: The array enumerates container queries starting with the innermost one, going outwards.
     container_queries: typing.Optional[typing.List[CSSContainerQuery]] = None
@@ -348,14 +351,16 @@
     def to_json(self):
         json = dict()
         json['selectorList'] = self.selector_list.to_json()
         json['origin'] = self.origin.to_json()
         json['style'] = self.style.to_json()
         if self.style_sheet_id is not None:
             json['styleSheetId'] = self.style_sheet_id.to_json()
+        if self.nesting_selectors is not None:
+            json['nestingSelectors'] = [i for i in self.nesting_selectors]
         if self.media is not None:
             json['media'] = [i.to_json() for i in self.media]
         if self.container_queries is not None:
             json['containerQueries'] = [i.to_json() for i in self.container_queries]
         if self.supports is not None:
             json['supports'] = [i.to_json() for i in self.supports]
         if self.layers is not None:
@@ -367,14 +372,15 @@
     @classmethod
     def from_json(cls, json):
         return cls(
             selector_list=SelectorList.from_json(json['selectorList']),
             origin=StyleSheetOrigin.from_json(json['origin']),
             style=CSSStyle.from_json(json['style']),
             style_sheet_id=StyleSheetId.from_json(json['styleSheetId']) if 'styleSheetId' in json else None,
+            nesting_selectors=[str(i) for i in json['nestingSelectors']] if 'nestingSelectors' in json else None,
             media=[CSSMedia.from_json(i) for i in json['media']] if 'media' in json else None,
             container_queries=[CSSContainerQuery.from_json(i) for i in json['containerQueries']] if 'containerQueries' in json else None,
             supports=[CSSSupports.from_json(i) for i in json['supports']] if 'supports' in json else None,
             layers=[CSSLayer.from_json(i) for i in json['layers']] if 'layers' in json else None,
             scopes=[CSSScope.from_json(i) for i in json['scopes']] if 'scopes' in json else None,
         )
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/database.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/database.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/device_access.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/device_access.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/device_orientation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/device_orientation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom_debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom_snapshot.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/dom_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/dom_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/emulation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/emulation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/event_breakpoints.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/fetch.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/fetch.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/headless_experimental.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/heap_profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/indexed_db.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/indexed_db.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/input_.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/input_.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/inspector.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/inspector.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/io.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/io.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/layer_tree.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/layer_tree.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/log.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/log.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/media.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/media.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/memory.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/memory.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/network.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/network.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/overlay.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/overlay.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/page.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1468,103 +1468,14 @@
         return cls(
             url=str(json['url']),
             explanations=[BackForwardCacheNotRestoredExplanation.from_json(i) for i in json['explanations']],
             children=[BackForwardCacheNotRestoredExplanationTree.from_json(i) for i in json['children']],
         )
 
 
-class PrerenderFinalStatus(enum.Enum):
-    '''
-    List of FinalStatus reasons for Prerender2.
-    '''
-    ACTIVATED = "Activated"
-    DESTROYED = "Destroyed"
-    LOW_END_DEVICE = "LowEndDevice"
-    INVALID_SCHEME_REDIRECT = "InvalidSchemeRedirect"
-    INVALID_SCHEME_NAVIGATION = "InvalidSchemeNavigation"
-    IN_PROGRESS_NAVIGATION = "InProgressNavigation"
-    NAVIGATION_REQUEST_BLOCKED_BY_CSP = "NavigationRequestBlockedByCsp"
-    MAIN_FRAME_NAVIGATION = "MainFrameNavigation"
-    MOJO_BINDER_POLICY = "MojoBinderPolicy"
-    RENDERER_PROCESS_CRASHED = "RendererProcessCrashed"
-    RENDERER_PROCESS_KILLED = "RendererProcessKilled"
-    DOWNLOAD = "Download"
-    TRIGGER_DESTROYED = "TriggerDestroyed"
-    NAVIGATION_NOT_COMMITTED = "NavigationNotCommitted"
-    NAVIGATION_BAD_HTTP_STATUS = "NavigationBadHttpStatus"
-    CLIENT_CERT_REQUESTED = "ClientCertRequested"
-    NAVIGATION_REQUEST_NETWORK_ERROR = "NavigationRequestNetworkError"
-    MAX_NUM_OF_RUNNING_PRERENDERS_EXCEEDED = "MaxNumOfRunningPrerendersExceeded"
-    CANCEL_ALL_HOSTS_FOR_TESTING = "CancelAllHostsForTesting"
-    DID_FAIL_LOAD = "DidFailLoad"
-    STOP = "Stop"
-    SSL_CERTIFICATE_ERROR = "SslCertificateError"
-    LOGIN_AUTH_REQUESTED = "LoginAuthRequested"
-    UA_CHANGE_REQUIRES_RELOAD = "UaChangeRequiresReload"
-    BLOCKED_BY_CLIENT = "BlockedByClient"
-    AUDIO_OUTPUT_DEVICE_REQUESTED = "AudioOutputDeviceRequested"
-    MIXED_CONTENT = "MixedContent"
-    TRIGGER_BACKGROUNDED = "TriggerBackgrounded"
-    EMBEDDER_TRIGGERED_AND_CROSS_ORIGIN_REDIRECTED = "EmbedderTriggeredAndCrossOriginRedirected"
-    MEMORY_LIMIT_EXCEEDED = "MemoryLimitExceeded"
-    FAIL_TO_GET_MEMORY_USAGE = "FailToGetMemoryUsage"
-    DATA_SAVER_ENABLED = "DataSaverEnabled"
-    HAS_EFFECTIVE_URL = "HasEffectiveUrl"
-    ACTIVATED_BEFORE_STARTED = "ActivatedBeforeStarted"
-    INACTIVE_PAGE_RESTRICTION = "InactivePageRestriction"
-    START_FAILED = "StartFailed"
-    TIMEOUT_BACKGROUNDED = "TimeoutBackgrounded"
-    CROSS_SITE_REDIRECT = "CrossSiteRedirect"
-    CROSS_SITE_NAVIGATION = "CrossSiteNavigation"
-    SAME_SITE_CROSS_ORIGIN_REDIRECT = "SameSiteCrossOriginRedirect"
-    SAME_SITE_CROSS_ORIGIN_NAVIGATION = "SameSiteCrossOriginNavigation"
-    SAME_SITE_CROSS_ORIGIN_REDIRECT_NOT_OPT_IN = "SameSiteCrossOriginRedirectNotOptIn"
-    SAME_SITE_CROSS_ORIGIN_NAVIGATION_NOT_OPT_IN = "SameSiteCrossOriginNavigationNotOptIn"
-    ACTIVATION_NAVIGATION_PARAMETER_MISMATCH = "ActivationNavigationParameterMismatch"
-    ACTIVATED_IN_BACKGROUND = "ActivatedInBackground"
-    EMBEDDER_HOST_DISALLOWED = "EmbedderHostDisallowed"
-    ACTIVATION_NAVIGATION_DESTROYED_BEFORE_SUCCESS = "ActivationNavigationDestroyedBeforeSuccess"
-    TAB_CLOSED_BY_USER_GESTURE = "TabClosedByUserGesture"
-    TAB_CLOSED_WITHOUT_USER_GESTURE = "TabClosedWithoutUserGesture"
-    PRIMARY_MAIN_FRAME_RENDERER_PROCESS_CRASHED = "PrimaryMainFrameRendererProcessCrashed"
-    PRIMARY_MAIN_FRAME_RENDERER_PROCESS_KILLED = "PrimaryMainFrameRendererProcessKilled"
-    ACTIVATION_FRAME_POLICY_NOT_COMPATIBLE = "ActivationFramePolicyNotCompatible"
-    PRELOADING_DISABLED = "PreloadingDisabled"
-    BATTERY_SAVER_ENABLED = "BatterySaverEnabled"
-    ACTIVATED_DURING_MAIN_FRAME_NAVIGATION = "ActivatedDuringMainFrameNavigation"
-    PRELOADING_UNSUPPORTED_BY_WEB_CONTENTS = "PreloadingUnsupportedByWebContents"
-
-    def to_json(self):
-        return self.value
-
-    @classmethod
-    def from_json(cls, json):
-        return cls(json)
-
-
-class PreloadingStatus(enum.Enum):
-    '''
-    Preloading status values, see also PreloadingTriggeringOutcome. This
-    status is shared by prefetchStatusUpdated and prerenderStatusUpdated.
-    '''
-    PENDING = "Pending"
-    RUNNING = "Running"
-    READY = "Ready"
-    SUCCESS = "Success"
-    FAILURE = "Failure"
-    NOT_SUPPORTED = "NotSupported"
-
-    def to_json(self):
-        return self.value
-
-    @classmethod
-    def from_json(cls, json):
-        return cls(json)
-
-
 def add_script_to_evaluate_on_load(
         script_source: str
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,ScriptIdentifier]:
     '''
     Deprecated, please use addScriptToEvaluateOnNewDocument instead.
 
     **EXPERIMENTAL**
@@ -3285,86 +3196,14 @@
             loader_id=network.LoaderId.from_json(json['loaderId']),
             frame_id=FrameId.from_json(json['frameId']),
             not_restored_explanations=[BackForwardCacheNotRestoredExplanation.from_json(i) for i in json['notRestoredExplanations']],
             not_restored_explanations_tree=BackForwardCacheNotRestoredExplanationTree.from_json(json['notRestoredExplanationsTree']) if 'notRestoredExplanationsTree' in json else None
         )
 
 
-@event_class('Page.prerenderAttemptCompleted')
-@dataclass
-class PrerenderAttemptCompleted:
-    '''
-    **EXPERIMENTAL**
-
-    Fired when a prerender attempt is completed.
-    '''
-    #: The frame id of the frame initiating prerendering.
-    initiating_frame_id: FrameId
-    prerendering_url: str
-    final_status: PrerenderFinalStatus
-    #: This is used to give users more information about the name of the API call
-    #: that is incompatible with prerender and has caused the cancellation of the attempt
-    disallowed_api_method: typing.Optional[str]
-
-    @classmethod
-    def from_json(cls, json: T_JSON_DICT) -> PrerenderAttemptCompleted:
-        return cls(
-            initiating_frame_id=FrameId.from_json(json['initiatingFrameId']),
-            prerendering_url=str(json['prerenderingUrl']),
-            final_status=PrerenderFinalStatus.from_json(json['finalStatus']),
-            disallowed_api_method=str(json['disallowedApiMethod']) if 'disallowedApiMethod' in json else None
-        )
-
-
-@event_class('Page.prefetchStatusUpdated')
-@dataclass
-class PrefetchStatusUpdated:
-    '''
-    **EXPERIMENTAL**
-
-    TODO(crbug/1384419): Create a dedicated domain for preloading.
-    Fired when a prefetch attempt is updated.
-    '''
-    #: The frame id of the frame initiating prefetch.
-    initiating_frame_id: FrameId
-    prefetch_url: str
-    status: PreloadingStatus
-
-    @classmethod
-    def from_json(cls, json: T_JSON_DICT) -> PrefetchStatusUpdated:
-        return cls(
-            initiating_frame_id=FrameId.from_json(json['initiatingFrameId']),
-            prefetch_url=str(json['prefetchUrl']),
-            status=PreloadingStatus.from_json(json['status'])
-        )
-
-
-@event_class('Page.prerenderStatusUpdated')
-@dataclass
-class PrerenderStatusUpdated:
-    '''
-    **EXPERIMENTAL**
-
-    TODO(crbug/1384419): Create a dedicated domain for preloading.
-    Fired when a prerender attempt is updated.
-    '''
-    #: The frame id of the frame initiating prerender.
-    initiating_frame_id: FrameId
-    prerendering_url: str
-    status: PreloadingStatus
-
-    @classmethod
-    def from_json(cls, json: T_JSON_DICT) -> PrerenderStatusUpdated:
-        return cls(
-            initiating_frame_id=FrameId.from_json(json['initiatingFrameId']),
-            prerendering_url=str(json['prerenderingUrl']),
-            status=PreloadingStatus.from_json(json['status'])
-        )
-
-
 @event_class('Page.loadEventFired')
 @dataclass
 class LoadEventFired:
     timestamp: network.MonotonicTime
 
     @classmethod
     def from_json(cls, json: T_JSON_DICT) -> LoadEventFired:
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/performance.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/performance.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/performance_timeline.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/preload.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v112/preload.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/runtime.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/runtime.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/schema.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/schema.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/security.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/security.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/service_worker.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/service_worker.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     LOCAL_STORAGE = "local_storage"
     SHADER_CACHE = "shader_cache"
     WEBSQL = "websql"
     SERVICE_WORKERS = "service_workers"
     CACHE_STORAGE = "cache_storage"
     INTEREST_GROUPS = "interest_groups"
     SHARED_STORAGE = "shared_storage"
+    STORAGE_BUCKETS = "storage_buckets"
     ALL_ = "all"
     OTHER = "other"
 
     def to_json(self):
         return self.value
 
     @classmethod
@@ -412,14 +413,71 @@
             urls_with_metadata=[SharedStorageUrlWithMetadata.from_json(i) for i in json['urlsWithMetadata']] if 'urlsWithMetadata' in json else None,
             key=str(json['key']) if 'key' in json else None,
             value=str(json['value']) if 'value' in json else None,
             ignore_if_present=bool(json['ignoreIfPresent']) if 'ignoreIfPresent' in json else None,
         )
 
 
+class StorageBucketsDurability(enum.Enum):
+    RELAXED = "relaxed"
+    STRICT = "strict"
+
+    def to_json(self):
+        return self.value
+
+    @classmethod
+    def from_json(cls, json):
+        return cls(json)
+
+
+@dataclass
+class StorageBucketInfo:
+    storage_key: SerializedStorageKey
+
+    id_: str
+
+    name: str
+
+    is_default: bool
+
+    expiration: network.TimeSinceEpoch
+
+    #: Storage quota (bytes).
+    quota: float
+
+    persistent: bool
+
+    durability: StorageBucketsDurability
+
+    def to_json(self):
+        json = dict()
+        json['storageKey'] = self.storage_key.to_json()
+        json['id'] = self.id_
+        json['name'] = self.name
+        json['isDefault'] = self.is_default
+        json['expiration'] = self.expiration.to_json()
+        json['quota'] = self.quota
+        json['persistent'] = self.persistent
+        json['durability'] = self.durability.to_json()
+        return json
+
+    @classmethod
+    def from_json(cls, json):
+        return cls(
+            storage_key=SerializedStorageKey.from_json(json['storageKey']),
+            id_=str(json['id']),
+            name=str(json['name']),
+            is_default=bool(json['isDefault']),
+            expiration=network.TimeSinceEpoch.from_json(json['expiration']),
+            quota=float(json['quota']),
+            persistent=bool(json['persistent']),
+            durability=StorageBucketsDurability.from_json(json['durability']),
+        )
+
+
 def get_storage_key_for_frame(
         frame_id: page.FrameId
     ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,SerializedStorageKey]:
     '''
     Returns a storage key given a frame id.
 
     :param frame_id:
@@ -949,14 +1007,58 @@
     cmd_dict: T_JSON_DICT = {
         'method': 'Storage.setSharedStorageTracking',
         'params': params,
     }
     json = yield cmd_dict
 
 
+def set_storage_bucket_tracking(
+        storage_key: str,
+        enable: bool
+    ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
+    '''
+    Set tracking for a storage key's buckets.
+
+    **EXPERIMENTAL**
+
+    :param storage_key:
+    :param enable:
+    '''
+    params: T_JSON_DICT = dict()
+    params['storageKey'] = storage_key
+    params['enable'] = enable
+    cmd_dict: T_JSON_DICT = {
+        'method': 'Storage.setStorageBucketTracking',
+        'params': params,
+    }
+    json = yield cmd_dict
+
+
+def delete_storage_bucket(
+        storage_key: str,
+        bucket_name: str
+    ) -> typing.Generator[T_JSON_DICT,T_JSON_DICT,None]:
+    '''
+    Deletes the Storage Bucket with the given storage key and bucket name.
+
+    **EXPERIMENTAL**
+
+    :param storage_key:
+    :param bucket_name:
+    '''
+    params: T_JSON_DICT = dict()
+    params['storageKey'] = storage_key
+    params['bucketName'] = bucket_name
+    cmd_dict: T_JSON_DICT = {
+        'method': 'Storage.deleteStorageBucket',
+        'params': params,
+    }
+    json = yield cmd_dict
+
+
 @event_class('Storage.cacheStorageContentUpdated')
 @dataclass
 class CacheStorageContentUpdated:
     '''
     A cache's contents have been modified.
     '''
     #: Origin to update.
@@ -1083,7 +1185,31 @@
         return cls(
             access_time=network.TimeSinceEpoch.from_json(json['accessTime']),
             type_=SharedStorageAccessType.from_json(json['type']),
             main_frame_id=page.FrameId.from_json(json['mainFrameId']),
             owner_origin=str(json['ownerOrigin']),
             params=SharedStorageAccessParams.from_json(json['params'])
         )
+
+
+@event_class('Storage.storageBucketCreatedOrUpdated')
+@dataclass
+class StorageBucketCreatedOrUpdated:
+    bucket: StorageBucketInfo
+
+    @classmethod
+    def from_json(cls, json: T_JSON_DICT) -> StorageBucketCreatedOrUpdated:
+        return cls(
+            bucket=StorageBucketInfo.from_json(json['bucket'])
+        )
+
+
+@event_class('Storage.storageBucketDeleted')
+@dataclass
+class StorageBucketDeleted:
+    bucket_id: str
+
+    @classmethod
+    def from_json(cls, json: T_JSON_DICT) -> StorageBucketDeleted:
+        return cls(
+            bucket_id=str(json['bucketId'])
+        )
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/system_info.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/system_info.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/target.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/target.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/tethering.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/tethering.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/tracing.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/tracing.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/web_audio.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/web_audio.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v112/web_authn.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/web_authn.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v113/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # DO NOT EDIT THIS FILE!
 #
 # This file is generated from the CDP specification. If you need to make
 # changes, edit the generator and regenerate all of the modules.
 from . import accessibility
 from . import animation
-from . import application_cache
 from . import audits
 from . import background_service
 from . import browser
 from . import css
 from . import cache_storage
 from . import cast
 from . import console
 from . import dom
 from . import dom_debugger
 from . import dom_snapshot
 from . import dom_storage
 from . import database
 from . import debugger
+from . import device_access
 from . import device_orientation
 from . import emulation
+from . import event_breakpoints
+from . import fed_cm
 from . import fetch
 from . import headless_experimental
 from . import heap_profiler
 from . import io
 from . import indexed_db
 from . import input_
 from . import inspector
@@ -31,14 +33,16 @@
 from . import log
 from . import media
 from . import memory
 from . import network
 from . import overlay
 from . import page
 from . import performance
+from . import performance_timeline
+from . import preload
 from . import profiler
 from . import runtime
 from . import schema
 from . import security
 from . import service_worker
 from . import storage
 from . import system_info
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/accessibility.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/accessibility.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/animation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/animation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/application_cache.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/application_cache.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/audits.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/audits.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/background_service.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/background_service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/browser.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/browser.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/cache_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/cache_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/cast.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/cast.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/console.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/console.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/css.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/css.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/database.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/database.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/device_orientation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/device_orientation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom_debugger.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom_snapshot.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/dom_storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/dom_storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/emulation.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/emulation.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/fetch.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/fetch.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/headless_experimental.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/heap_profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/indexed_db.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/indexed_db.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/input_.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/input_.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/inspector.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/inspector.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/io.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/io.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/layer_tree.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/layer_tree.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/log.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/log.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/media.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/media.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/memory.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/memory.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/network.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/network.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/overlay.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/overlay.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/page.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/page.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/performance.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/performance.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/profiler.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/profiler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/runtime.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/runtime.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/schema.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/schema.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/security.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/security.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/service_worker.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/service_worker.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/storage.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/storage.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/system_info.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/system_info.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/target.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/target.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/tethering.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/tethering.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/tracing.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/tracing.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/web_audio.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/web_audio.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/devtools/v85/web_authn.py` & `selenium-4.9.1/selenium/webdriver/common/devtools/v85/web_authn.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/driver_finder.py` & `selenium-4.9.1/selenium/webdriver/common/driver_finder.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/html5/__init__.py` & `selenium-4.9.1/selenium/webdriver/common/html5/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/html5/application_cache.py` & `selenium-4.9.1/selenium/webdriver/common/html5/application_cache.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/keys.py` & `selenium-4.9.1/selenium/webdriver/common/keys.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/linux/selenium-manager` & `selenium-4.9.1/selenium/webdriver/common/linux/selenium-manager`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/log.py` & `selenium-4.9.1/selenium/webdriver/common/log.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/macos/selenium-manager` & `selenium-4.9.1/selenium/webdriver/common/macos/selenium-manager`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/mutation-listener.js` & `selenium-4.9.1/selenium/webdriver/common/mutation-listener.js`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/options.py` & `selenium-4.9.1/selenium/webdriver/common/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/print_page_options.py` & `selenium-4.9.1/selenium/webdriver/common/print_page_options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/proxy.py` & `selenium-4.9.1/selenium/webdriver/common/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,16 +286,15 @@
 
     def add_to_capabilities(self, capabilities):
         """Adds proxy information as capability in specified capabilities.
 
         :Args:
          - capabilities: The capabilities to which proxy will be added.
         """
-        proxy_caps = {}
-        proxy_caps["proxyType"] = self.proxyType["string"]
+        proxy_caps = {"proxyType": self.proxyType["string"]}
         if self.autodetect:
             proxy_caps["autodetect"] = self.autodetect
         if self.ftpProxy:
             proxy_caps["ftpProxy"] = self.ftpProxy
         if self.httpProxy:
             proxy_caps["httpProxy"] = self.httpProxy
         if self.proxyAutoconfigUrl:
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/selenium_manager.py` & `selenium-4.9.1/selenium/webdriver/common/selenium_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,63 +66,55 @@
         """
         Determines the path of the correct driver.
         :Args:
          - browser: which browser to get the driver path for.
         :Returns: The driver path to use
         """
 
-        browser = options.capabilities["browserName"]
-
-        allowed_browsers = {
-            "chrome": "chrome",
-            "firefox": "firefox",
-            "edge": "edge",
-            "MicrosoftEdge": "edge",
-            "ie": "iexplorer",
-        }
-
-        if browser not in allowed_browsers.keys():
-            raise SeleniumManagerException(
-                f"{browser} is not a valid browser.  Choose one of: {list(allowed_browsers.keys())}"
-            )
+        logger.info("Applicable driver not found; attempting to install with Selenium Manager (Beta)")
 
-        browser = allowed_browsers[browser]
+        browser = options.capabilities["browserName"]
 
         args = [str(self.get_binary()), "--browser", browser, "--output", "json"]
 
         if options.browser_version:
             args.append("--browser-version")
             args.append(str(options.browser_version))
 
         binary_location = getattr(options, "binary_location", None)
         if binary_location:
             args.append("--browser-path")
             args.append(str(binary_location))
 
+        if logger.getEffectiveLevel() == logging.DEBUG:
+            args.append("--debug")
+
         result = self.run(args)
         executable = result.split("\t")[-1].strip()
         logger.debug(f"Using driver at: {executable}")
         return executable
 
     @staticmethod
     def run(args: List[str]) -> str:
         """
         Executes the Selenium Manager Binary.
         :Args:
          - args: the components of the command being executed.
         :Returns: The log string containing the driver location.
         """
         command = " ".join(args)
-        logger.info(f"Executing: {command}")
+        logger.debug(f"Executing process: {command}")
         completed_proc = subprocess.run(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         stdout = completed_proc.stdout.decode("utf-8").rstrip("\n")
         stderr = completed_proc.stderr.decode("utf-8").rstrip("\n")
         output = json.loads(stdout)
         result = output["result"]["message"]
         if completed_proc.returncode:
             raise SeleniumManagerException(f"Selenium Manager failed for: {command}.\n{result}{stderr}")
         else:
             # Selenium Manager exited successfully, return executable path and print warnings
             for item in output["logs"]:
                 if item["level"] == "WARN":
                     logger.warning(item["message"])
+                if item["level"] == "DEBUG":
+                    logger.debug(item["message"])
             return result
```

### Comparing `selenium-4.9.0/selenium/webdriver/common/service.py` & `selenium-4.9.1/selenium/webdriver/common/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/timeouts.py` & `selenium-4.9.1/selenium/webdriver/common/timeouts.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/utils.py` & `selenium-4.9.1/selenium/webdriver/common/utils.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/virtual_authenticator.py` & `selenium-4.9.1/selenium/webdriver/common/virtual_authenticator.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/window.py` & `selenium-4.9.1/selenium/webdriver/common/window.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/common/windows/selenium-manager.exe` & `selenium-4.9.1/selenium/webdriver/common/windows/selenium-manager.exe`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/edge/__init__.py` & `selenium-4.9.1/selenium/webdriver/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/edge/options.py` & `selenium-4.9.1/selenium/webdriver/edge/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/edge/service.py` & `selenium-4.9.1/selenium/webdriver/edge/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/edge/webdriver.py` & `selenium-4.9.1/selenium/webdriver/edge/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/__init__.py` & `selenium-4.9.1/selenium/webdriver/firefox/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/extension_connection.py` & `selenium-4.9.1/selenium/webdriver/firefox/extension_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/firefox_binary.py` & `selenium-4.9.1/selenium/webdriver/firefox/firefox_binary.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/firefox_profile.py` & `selenium-4.9.1/selenium/webdriver/firefox/firefox_profile.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/options.py` & `selenium-4.9.1/selenium/webdriver/firefox/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/remote_connection.py` & `selenium-4.9.1/selenium/webdriver/firefox/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/service.py` & `selenium-4.9.1/selenium/webdriver/firefox/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/webdriver.py` & `selenium-4.9.1/selenium/webdriver/firefox/webdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
 
     def install_addon(self, path, temporary=False) -> str:
         """Installs Firefox addon.
 
         Returns identifier of installed addon. This identifier can later
         be used to uninstall addon.
 
+        :param temporary: allows you to load browser extensions temporarily during a session
         :param path: Absolute path to the addon that will be installed.
 
         :Usage:
             ::
 
                 driver.install_addon('/path/to/firebug.xpi')
         """
```

### Comparing `selenium-4.9.0/selenium/webdriver/firefox/webdriver_prefs.json` & `selenium-4.9.1/selenium/webdriver/firefox/webdriver_prefs.json`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/ie/__init__.py` & `selenium-4.9.1/selenium/webdriver/ie/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/ie/options.py` & `selenium-4.9.1/selenium/webdriver/ie/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/ie/service.py` & `selenium-4.9.1/selenium/webdriver/ie/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/ie/webdriver.py` & `selenium-4.9.1/selenium/webdriver/ie/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/__init__.py` & `selenium-4.9.1/selenium/webdriver/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/bidi_connection.py` & `selenium-4.9.1/selenium/webdriver/remote/bidi_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/command.py` & `selenium-4.9.1/selenium/webdriver/remote/command.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/errorhandler.py` & `selenium-4.9.1/selenium/webdriver/remote/errorhandler.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/file_detector.py` & `selenium-4.9.1/selenium/webdriver/remote/file_detector.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/findElements.js` & `selenium-4.9.1/selenium/webdriver/remote/findElements.js`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/getAttribute.js` & `selenium-4.9.1/selenium/webdriver/remote/getAttribute.js`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/isDisplayed.js` & `selenium-4.9.1/selenium/webdriver/remote/isDisplayed.js`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/mobile.py` & `selenium-4.9.1/selenium/webdriver/remote/mobile.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/remote_connection.py` & `selenium-4.9.1/selenium/webdriver/remote/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/script_key.py` & `selenium-4.9.1/selenium/webdriver/remote/script_key.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/shadowroot.py` & `selenium-4.9.1/selenium/webdriver/remote/shadowroot.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/switch_to.py` & `selenium-4.9.1/selenium/webdriver/remote/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/utils.py` & `selenium-4.9.1/selenium/webdriver/remote/utils.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/webdriver.py` & `selenium-4.9.1/selenium/webdriver/remote/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/remote/webelement.py` & `selenium-4.9.1/selenium/webdriver/remote/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/safari/__init__.py` & `selenium-4.9.1/selenium/webdriver/safari/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/safari/options.py` & `selenium-4.9.1/selenium/webdriver/safari/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/safari/permissions.py` & `selenium-4.9.1/selenium/webdriver/safari/permissions.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/safari/remote_connection.py` & `selenium-4.9.1/selenium/webdriver/safari/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/safari/service.py` & `selenium-4.9.1/selenium/webdriver/safari/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/safari/webdriver.py` & `selenium-4.9.1/selenium/webdriver/safari/webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,15 @@
     # https://developer.apple.com/library/content/documentation/NetworkingInternetWeb/Conceptual/WebDriverEndpointDoc/Commands/Commands.html
 
     # First available in Safari 11.1 and Safari Technology Preview 41.
     def set_permission(self, permission, value):
         if not isinstance(value, bool):
             raise WebDriverException("Value of a session permission must be set to True or False.")
 
-        payload = {}
-        payload[permission] = value
+        payload = {permission: value}
         self.execute("SET_PERMISSIONS", {"permissions": payload})
 
     # First available in Safari 11.1 and Safari Technology Preview 41.
     def get_permission(self, permission):
         payload = self.execute("GET_PERMISSIONS")["value"]
         permissions = payload["permissions"]
         if not permissions:
```

### Comparing `selenium-4.9.0/selenium/webdriver/support/__init__.py` & `selenium-4.9.1/selenium/webdriver/support/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/abstract_event_listener.py` & `selenium-4.9.1/selenium/webdriver/support/abstract_event_listener.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/color.py` & `selenium-4.9.1/selenium/webdriver/support/color.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/event_firing_webdriver.py` & `selenium-4.9.1/selenium/webdriver/support/event_firing_webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/events.py` & `selenium-4.9.1/selenium/webdriver/support/events.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/expected_conditions.py` & `selenium-4.9.1/selenium/webdriver/support/expected_conditions.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/relative_locator.py` & `selenium-4.9.1/selenium/webdriver/support/relative_locator.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/select.py` & `selenium-4.9.1/selenium/webdriver/support/select.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/ui.py` & `selenium-4.9.1/selenium/webdriver/support/ui.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/support/wait.py` & `selenium-4.9.1/selenium/webdriver/support/wait.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/webkitgtk/__init__.py` & `selenium-4.9.1/selenium/webdriver/webkitgtk/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/webkitgtk/options.py` & `selenium-4.9.1/selenium/webdriver/webkitgtk/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/webkitgtk/service.py` & `selenium-4.9.1/selenium/webdriver/webkitgtk/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/webkitgtk/webdriver.py` & `selenium-4.9.1/selenium/webdriver/webkitgtk/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/wpewebkit/__init__.py` & `selenium-4.9.1/selenium/webdriver/wpewebkit/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/wpewebkit/options.py` & `selenium-4.9.1/selenium/webdriver/wpewebkit/options.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/wpewebkit/service.py` & `selenium-4.9.1/selenium/webdriver/wpewebkit/service.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/selenium/webdriver/wpewebkit/webdriver.py` & `selenium-4.9.1/selenium/webdriver/wpewebkit/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-4.9.0/setup.py` & `selenium-4.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 for scheme in INSTALL_SCHEMES.values():
     scheme['data'] = scheme['purelib']
 
 setup_args = {
     'cmdclass': {'install': install},
     'name': 'selenium',
-    'version': "4.9.0",
+    'version': "4.9.1",
     'license': 'Apache 2.0',
     'description': 'Python bindings for Selenium',
     'long_description': open(join(abspath(dirname(__file__)), "README.rst")).read(),
     'url': 'https://github.com/SeleniumHQ/selenium/',
     'project_urls': {
         'Bug Tracker': 'https://github.com/SeleniumHQ/selenium/issues',
         'Changes': 'https://github.com/SeleniumHQ/selenium/blob/trunk/py/CHANGES',
@@ -67,15 +67,15 @@
                  'selenium.webdriver.firefox',
                  'selenium.webdriver.ie',
                  'selenium.webdriver.edge',
                  'selenium.webdriver.remote',
                  'selenium.webdriver.support', ],
     'include_package_data': True,
     'install_requires': [
-        "urllib3[socks]~=1.26",
+        "urllib3[socks]>=1.26,<3",
         "trio~=0.17",
         "trio-websocket~=0.9",
         "certifi>=2021.10.8",
     ],
     'zip_safe': False
 }
```

