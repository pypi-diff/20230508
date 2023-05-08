# Comparing `tmp/geckordp-0.4.44.zip` & `tmp/geckordp-0.4.53.zip`

## zipinfo {}

```diff
@@ -1,107 +1,104 @@
-Zip file size: 98777 bytes, number of entries: 105
--rwxr-xr-x  3.0 unx     6154 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/utils.py
--rwxr-xr-x  3.0 unx     1956 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/logger.py
--rwxr-xr-x  3.0 unx     5137 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/settings.py
--rwxr-xr-x  3.0 unx      994 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/__init__.py
--rwxr-xr-x  3.0 unx     1550 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/buffers.py
--rw-rw-r--  3.0 unx    20460 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/profile.py
--rwxr-xr-x  3.0 unx     5481 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/firefox.py
--rw-rw-r--  3.0 unx    30688 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/rdp_client.py
--rwxr-xr-x  3.0 unx     1385 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/screenshot.py
--rwxr-xr-x  3.0 unx     3183 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/node.py
--rwxr-xr-x  3.0 unx     5396 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/source.py
--rw-rw-r--  3.0 unx    12633 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/walker.py
--rwxr-xr-x  3.0 unx      775 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/node_list.py
--rw-rw-r--  3.0 unx     4786 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/storage.py
--rwxr-xr-x  3.0 unx      493 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/heap_snapshot.py
--rwxr-xr-x  3.0 unx     1730 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/network_content.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/accessibility/__init__.py
--rwxr-xr-x  3.0 unx      898 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/accessibility/simulator.py
--rwxr-xr-x  3.0 unx      903 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/accessibility/accessibility.py
--rwxr-xr-x  3.0 unx     2429 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/accessibility/accessible_walker.py
--rwxr-xr-x  3.0 unx     1147 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/accessibility/accessible.py
--rwxr-xr-x  3.0 unx      699 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/accessibility/parent_accessibility.py
--rwxr-xr-x  3.0 unx      553 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/event_source.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/__init__.py
--rwxr-xr-x  3.0 unx     2067 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/preference.py
--rwxr-xr-x  3.0 unx     2736 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/network_event.py
--rwxr-xr-x  3.0 unx     4023 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/memory.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/addon/__init__.py
--rwxr-xr-x  3.0 unx      672 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/addon/addons.py
--rwxr-xr-x  3.0 unx     2526 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/addon/web_extension_inspected_window.py
--rwxr-xr-x  3.0 unx     3655 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/web_console.py
--rwxr-xr-x  3.0 unx     2077 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/root.py
--rwxr-xr-x  3.0 unx      481 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/string.py
--rwxr-xr-x  3.0 unx      531 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/descriptors/worker.py
--rwxr-xr-x  3.0 unx      805 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/descriptors/process.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/descriptors/__init__.py
--rwxr-xr-x  3.0 unx     1304 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/descriptors/tab.py
--rwxr-xr-x  3.0 unx      696 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/descriptors/web_extension.py
--rwxr-xr-x  3.0 unx      549 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/web_socket.py
--rwxr-xr-x  3.0 unx     4076 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/watcher.py
--rwxr-xr-x  3.0 unx      414 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/device.py
--rwxr-xr-x  3.0 unx     8326 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/thread.py
--rwxr-xr-x  3.0 unx     7130 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/events.py
--rwxr-xr-x  3.0 unx     2244 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/network_parent.py
--rwxr-xr-x  3.0 unx      439 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/actor.py
--rwxr-xr-x  3.0 unx     2193 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/target_configuration.py
--rw-rw-r--  3.0 unx     2330 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/targets/window_global.py
--rwxr-xr-x  3.0 unx      662 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/targets/content_process.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/targets/__init__.py
--rwxr-xr-x  3.0 unx     3159 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp/actors/inspector.py
--rw-rw-r--  3.0 unx       15 t- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp.egg-info/top_level.txt
--rw-rw-r--  3.0 unx       99 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp.egg-info/requires.txt
--rw-rw-r--  3.0 unx    12070 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp.egg-info/PKG-INFO
--rw-rw-r--  3.0 unx        1 t- stor 81-Jan-01 02:01 geckordp-0.4.44/geckordp.egg-info/dependency_links.txt
--rw-rw-r--  3.0 unx     3432 t- defN 81-Jan-01 02:01 geckordp-0.4.44/geckordp.egg-info/SOURCES.txt
--rwxr-xr-x  3.0 unx     2411 t- defN 81-Jan-01 02:01 geckordp-0.4.44/setup.py
--rwxr-xr-x  3.0 unx      158 t- defN 81-Jan-01 02:01 geckordp-0.4.44/setup.cfg
--rw-rw-r--  3.0 unx    12070 t- defN 81-Jan-01 02:01 geckordp-0.4.44/PKG-INFO
--rw-rw-r--  3.0 unx    11158 t- defN 81-Jan-01 02:01 geckordp-0.4.44/README.md
--rwxr-xr-x  3.0 unx     1180 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/helpers/utils.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/tests/helpers/__init__.py
--rwxr-xr-x  3.0 unx      129 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/helpers/constants.py
--rwxr-xr-x  3.0 unx     3079 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage_cookie.py
--rwxr-xr-x  3.0 unx     2772 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_source.py
--rwxr-xr-x  3.0 unx     4313 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_node.py
--rwxr-xr-x  3.0 unx     2970 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_inspector.py
--rwxr-xr-x  3.0 unx     2622 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_root.py
--rwxr-xr-x  3.0 unx     3756 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_memory.py
--rwxr-xr-x  3.0 unx     1713 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/accessibility/test_simulator.py
--rwxr-xr-x  3.0 unx     1326 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/accessibility/test_parent_accessibility.py
--rwxr-xr-x  3.0 unx     2363 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/accessibility/test_accessible.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/accessibility/__init__.py
--rwxr-xr-x  3.0 unx     3201 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/accessibility/test_accessible_walker.py
--rwxr-xr-x  3.0 unx     1711 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/accessibility/test_accessibility.py
--rwxr-xr-x  3.0 unx     1467 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_heap_snapshot.py
--rwxr-xr-x  3.0 unx      882 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/__init__.py
--rwxr-xr-x  3.0 unx     1021 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_event_source.py
--rw-rw-r--  3.0 unx     4134 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_network_event.py
--rw-rw-r--  3.0 unx     1604 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_network_content.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/addon/__init__.py
--rwxr-xr-x  3.0 unx      746 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/addon/test_addons.py
--rwxr-xr-x  3.0 unx     1601 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/addon/test_web_extension_inspected_window.py
--rwxr-xr-x  3.0 unx      735 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_device.py
--rwxr-xr-x  3.0 unx     2876 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_network_parent.py
--rwxr-xr-x  3.0 unx     2883 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage_local.py
--rwxr-xr-x  3.0 unx     3532 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_watcher.py
--rwxr-xr-x  3.0 unx     1119 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/descriptors/test_tab.py
--rwxr-xr-x  3.0 unx     1800 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/descriptors/test_web_extension.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/descriptors/__init__.py
--rwxr-xr-x  3.0 unx      859 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/descriptors/test_worker.py
--rwxr-xr-x  3.0 unx     1004 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/descriptors/test_process.py
--rwxr-xr-x  3.0 unx     2425 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage_cache.py
--rwxr-xr-x  3.0 unx     3785 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_web_console.py
--rwxr-xr-x  3.0 unx     1599 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_node_list.py
--rwxr-xr-x  3.0 unx      966 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_screenshot.py
--rwxr-xr-x  3.0 unx     3030 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_preference.py
--rwxr-xr-x  3.0 unx     2157 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage_indexed.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/targets/__init__.py
--rw-rw-r--  3.0 unx     3150 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/targets/test_window_global.py
--rwxr-xr-x  3.0 unx     1300 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/targets/test_content_process.py
--rwxr-xr-x  3.0 unx     2931 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage_session.py
--rw-rw-r--  3.0 unx     5472 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_thread.py
--rwxr-xr-x  3.0 unx      785 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_storage_extension.py
--rw-rw-r--  3.0 unx    14235 t- defN 81-Jan-01 02:01 geckordp-0.4.44/tests/actors/test_walker.py
-105 files, 303172 bytes uncompressed, 80741 bytes compressed:  73.4%
+Zip file size: 97088 bytes, number of entries: 102
+-rwxr-xr-x  3.0 unx     6154 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/utils.py
+-rwxr-xr-x  3.0 unx     1956 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/logger.py
+-rwxr-xr-x  3.0 unx     5137 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/settings.py
+-rwxr-xr-x  3.0 unx      994 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/__init__.py
+-rwxr-xr-x  3.0 unx     1550 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/buffers.py
+-rw-rw-r--  3.0 unx    20460 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/profile.py
+-rwxr-xr-x  3.0 unx     5481 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/firefox.py
+-rw-rw-r--  3.0 unx    30688 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/rdp_client.py
+-rwxr-xr-x  3.0 unx     1385 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/screenshot.py
+-rwxr-xr-x  3.0 unx     3183 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/node.py
+-rwxr-xr-x  3.0 unx     5396 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/source.py
+-rw-rw-r--  3.0 unx    12633 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/walker.py
+-rwxr-xr-x  3.0 unx      775 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/node_list.py
+-rw-rw-r--  3.0 unx     4427 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/storage.py
+-rwxr-xr-x  3.0 unx      493 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/heap_snapshot.py
+-rwxr-xr-x  3.0 unx     1730 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/network_content.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/__init__.py
+-rwxr-xr-x  3.0 unx      898 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/simulator.py
+-rwxr-xr-x  3.0 unx      903 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/accessibility.py
+-rwxr-xr-x  3.0 unx     2429 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/accessible_walker.py
+-rwxr-xr-x  3.0 unx     1147 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/accessible.py
+-rwxr-xr-x  3.0 unx      699 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/parent_accessibility.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/__init__.py
+-rwxr-xr-x  3.0 unx     2067 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/preference.py
+-rwxr-xr-x  3.0 unx     2736 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/network_event.py
+-rwxr-xr-x  3.0 unx     4023 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/memory.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/addon/__init__.py
+-rwxr-xr-x  3.0 unx      672 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/addon/addons.py
+-rwxr-xr-x  3.0 unx     2526 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/addon/web_extension_inspected_window.py
+-rwxr-xr-x  3.0 unx     3655 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/web_console.py
+-rwxr-xr-x  3.0 unx     1907 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/root.py
+-rwxr-xr-x  3.0 unx      481 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/string.py
+-rwxr-xr-x  3.0 unx      531 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/worker.py
+-rwxr-xr-x  3.0 unx      805 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/process.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/__init__.py
+-rwxr-xr-x  3.0 unx     1304 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/tab.py
+-rwxr-xr-x  3.0 unx      696 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/web_extension.py
+-rwxr-xr-x  3.0 unx      549 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/web_socket.py
+-rwxr-xr-x  3.0 unx     4076 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/watcher.py
+-rwxr-xr-x  3.0 unx      414 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/device.py
+-rwxr-xr-x  3.0 unx     8326 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/thread.py
+-rwxr-xr-x  3.0 unx     7130 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/events.py
+-rwxr-xr-x  3.0 unx     2244 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/network_parent.py
+-rwxr-xr-x  3.0 unx      439 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/actor.py
+-rwxr-xr-x  3.0 unx     2193 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/target_configuration.py
+-rw-rw-r--  3.0 unx     2139 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/targets/window_global.py
+-rwxr-xr-x  3.0 unx      662 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/targets/content_process.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/targets/__init__.py
+-rwxr-xr-x  3.0 unx     3159 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/inspector.py
+-rw-rw-r--  3.0 unx       15 t- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/top_level.txt
+-rw-rw-r--  3.0 unx       99 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/requires.txt
+-rw-rw-r--  3.0 unx    12070 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/PKG-INFO
+-rw-rw-r--  3.0 unx        1 t- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/dependency_links.txt
+-rw-rw-r--  3.0 unx     3337 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/SOURCES.txt
+-rwxr-xr-x  3.0 unx     2411 t- defN 81-Jan-01 02:01 geckordp-0.4.53/setup.py
+-rwxr-xr-x  3.0 unx      158 t- defN 81-Jan-01 02:01 geckordp-0.4.53/setup.cfg
+-rw-rw-r--  3.0 unx    12070 t- defN 81-Jan-01 02:01 geckordp-0.4.53/PKG-INFO
+-rw-rw-r--  3.0 unx    11158 t- defN 81-Jan-01 02:01 geckordp-0.4.53/README.md
+-rwxr-xr-x  3.0 unx     1180 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/helpers/utils.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/helpers/__init__.py
+-rwxr-xr-x  3.0 unx      129 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/helpers/constants.py
+-rwxr-xr-x  3.0 unx     3079 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_cookie.py
+-rwxr-xr-x  3.0 unx     2772 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_source.py
+-rwxr-xr-x  3.0 unx     4313 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_node.py
+-rwxr-xr-x  3.0 unx     2970 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_inspector.py
+-rwxr-xr-x  3.0 unx     2442 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_root.py
+-rwxr-xr-x  3.0 unx     3756 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_memory.py
+-rwxr-xr-x  3.0 unx     1713 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_simulator.py
+-rwxr-xr-x  3.0 unx     1326 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_parent_accessibility.py
+-rwxr-xr-x  3.0 unx     2363 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_accessible.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/__init__.py
+-rwxr-xr-x  3.0 unx     3201 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_accessible_walker.py
+-rwxr-xr-x  3.0 unx     1711 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_accessibility.py
+-rwxr-xr-x  3.0 unx     1467 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_heap_snapshot.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/__init__.py
+-rw-rw-r--  3.0 unx     4134 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_network_event.py
+-rw-rw-r--  3.0 unx     1604 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_network_content.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/addon/__init__.py
+-rwxr-xr-x  3.0 unx      746 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/addon/test_addons.py
+-rwxr-xr-x  3.0 unx     1601 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/addon/test_web_extension_inspected_window.py
+-rwxr-xr-x  3.0 unx      735 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_device.py
+-rwxr-xr-x  3.0 unx     2876 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_network_parent.py
+-rwxr-xr-x  3.0 unx     2883 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_local.py
+-rwxr-xr-x  3.0 unx     3532 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_watcher.py
+-rwxr-xr-x  3.0 unx     1119 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_tab.py
+-rwxr-xr-x  3.0 unx     1800 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_web_extension.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/__init__.py
+-rwxr-xr-x  3.0 unx      859 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_worker.py
+-rwxr-xr-x  3.0 unx     1004 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_process.py
+-rwxr-xr-x  3.0 unx     2425 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_cache.py
+-rwxr-xr-x  3.0 unx     3785 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_web_console.py
+-rwxr-xr-x  3.0 unx     1599 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_node_list.py
+-rwxr-xr-x  3.0 unx      966 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_screenshot.py
+-rwxr-xr-x  3.0 unx     3030 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_preference.py
+-rwxr-xr-x  3.0 unx     2157 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_indexed.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/targets/__init__.py
+-rw-rw-r--  3.0 unx     2886 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/targets/test_window_global.py
+-rwxr-xr-x  3.0 unx     1300 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/targets/test_content_process.py
+-rwxr-xr-x  3.0 unx     2931 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_session.py
+-rw-rw-r--  3.0 unx     5472 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_thread.py
+-rwxr-xr-x  3.0 unx      785 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_extension.py
+-rw-rw-r--  3.0 unx    14235 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_walker.py
+102 files, 299457 bytes uncompressed, 79560 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -1,316 +1,307 @@
-Filename: geckordp-0.4.44/geckordp/utils.py
+Filename: geckordp-0.4.53/geckordp/utils.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/logger.py
+Filename: geckordp-0.4.53/geckordp/logger.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/settings.py
+Filename: geckordp-0.4.53/geckordp/settings.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/__init__.py
+Filename: geckordp-0.4.53/geckordp/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/buffers.py
+Filename: geckordp-0.4.53/geckordp/buffers.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/profile.py
+Filename: geckordp-0.4.53/geckordp/profile.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/firefox.py
+Filename: geckordp-0.4.53/geckordp/firefox.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/rdp_client.py
+Filename: geckordp-0.4.53/geckordp/rdp_client.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/screenshot.py
+Filename: geckordp-0.4.53/geckordp/actors/screenshot.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/node.py
+Filename: geckordp-0.4.53/geckordp/actors/node.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/source.py
+Filename: geckordp-0.4.53/geckordp/actors/source.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/walker.py
+Filename: geckordp-0.4.53/geckordp/actors/walker.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/node_list.py
+Filename: geckordp-0.4.53/geckordp/actors/node_list.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/storage.py
+Filename: geckordp-0.4.53/geckordp/actors/storage.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/heap_snapshot.py
+Filename: geckordp-0.4.53/geckordp/actors/heap_snapshot.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/network_content.py
+Filename: geckordp-0.4.53/geckordp/actors/network_content.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/accessibility/__init__.py
+Filename: geckordp-0.4.53/geckordp/actors/accessibility/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/accessibility/simulator.py
+Filename: geckordp-0.4.53/geckordp/actors/accessibility/simulator.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/accessibility/accessibility.py
+Filename: geckordp-0.4.53/geckordp/actors/accessibility/accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/accessibility/accessible_walker.py
+Filename: geckordp-0.4.53/geckordp/actors/accessibility/accessible_walker.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/accessibility/accessible.py
+Filename: geckordp-0.4.53/geckordp/actors/accessibility/accessible.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/accessibility/parent_accessibility.py
+Filename: geckordp-0.4.53/geckordp/actors/accessibility/parent_accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/event_source.py
+Filename: geckordp-0.4.53/geckordp/actors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/__init__.py
+Filename: geckordp-0.4.53/geckordp/actors/preference.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/preference.py
+Filename: geckordp-0.4.53/geckordp/actors/network_event.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/network_event.py
+Filename: geckordp-0.4.53/geckordp/actors/memory.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/memory.py
+Filename: geckordp-0.4.53/geckordp/actors/addon/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/addon/__init__.py
+Filename: geckordp-0.4.53/geckordp/actors/addon/addons.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/addon/addons.py
+Filename: geckordp-0.4.53/geckordp/actors/addon/web_extension_inspected_window.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/addon/web_extension_inspected_window.py
+Filename: geckordp-0.4.53/geckordp/actors/web_console.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/web_console.py
+Filename: geckordp-0.4.53/geckordp/actors/root.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/root.py
+Filename: geckordp-0.4.53/geckordp/actors/string.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/string.py
+Filename: geckordp-0.4.53/geckordp/actors/descriptors/worker.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/descriptors/worker.py
+Filename: geckordp-0.4.53/geckordp/actors/descriptors/process.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/descriptors/process.py
+Filename: geckordp-0.4.53/geckordp/actors/descriptors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/descriptors/__init__.py
+Filename: geckordp-0.4.53/geckordp/actors/descriptors/tab.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/descriptors/tab.py
+Filename: geckordp-0.4.53/geckordp/actors/descriptors/web_extension.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/descriptors/web_extension.py
+Filename: geckordp-0.4.53/geckordp/actors/web_socket.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/web_socket.py
+Filename: geckordp-0.4.53/geckordp/actors/watcher.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/watcher.py
+Filename: geckordp-0.4.53/geckordp/actors/device.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/device.py
+Filename: geckordp-0.4.53/geckordp/actors/thread.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/thread.py
+Filename: geckordp-0.4.53/geckordp/actors/events.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/events.py
+Filename: geckordp-0.4.53/geckordp/actors/network_parent.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/network_parent.py
+Filename: geckordp-0.4.53/geckordp/actors/actor.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/actor.py
+Filename: geckordp-0.4.53/geckordp/actors/target_configuration.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/target_configuration.py
+Filename: geckordp-0.4.53/geckordp/actors/targets/window_global.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/targets/window_global.py
+Filename: geckordp-0.4.53/geckordp/actors/targets/content_process.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/targets/content_process.py
+Filename: geckordp-0.4.53/geckordp/actors/targets/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/targets/__init__.py
+Filename: geckordp-0.4.53/geckordp/actors/inspector.py
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp/actors/inspector.py
+Filename: geckordp-0.4.53/geckordp.egg-info/top_level.txt
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp.egg-info/top_level.txt
+Filename: geckordp-0.4.53/geckordp.egg-info/requires.txt
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp.egg-info/requires.txt
+Filename: geckordp-0.4.53/geckordp.egg-info/PKG-INFO
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp.egg-info/PKG-INFO
+Filename: geckordp-0.4.53/geckordp.egg-info/dependency_links.txt
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp.egg-info/dependency_links.txt
+Filename: geckordp-0.4.53/geckordp.egg-info/SOURCES.txt
 Comment: 
 
-Filename: geckordp-0.4.44/geckordp.egg-info/SOURCES.txt
+Filename: geckordp-0.4.53/setup.py
 Comment: 
 
-Filename: geckordp-0.4.44/setup.py
+Filename: geckordp-0.4.53/setup.cfg
 Comment: 
 
-Filename: geckordp-0.4.44/setup.cfg
+Filename: geckordp-0.4.53/PKG-INFO
 Comment: 
 
-Filename: geckordp-0.4.44/PKG-INFO
+Filename: geckordp-0.4.53/README.md
 Comment: 
 
-Filename: geckordp-0.4.44/README.md
+Filename: geckordp-0.4.53/tests/helpers/utils.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/helpers/utils.py
+Filename: geckordp-0.4.53/tests/helpers/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/helpers/__init__.py
+Filename: geckordp-0.4.53/tests/helpers/constants.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/helpers/constants.py
+Filename: geckordp-0.4.53/tests/actors/test_storage_cookie.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_storage_cookie.py
+Filename: geckordp-0.4.53/tests/actors/test_source.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_source.py
+Filename: geckordp-0.4.53/tests/actors/test_node.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_node.py
+Filename: geckordp-0.4.53/tests/actors/test_inspector.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_inspector.py
+Filename: geckordp-0.4.53/tests/actors/test_root.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_root.py
+Filename: geckordp-0.4.53/tests/actors/test_memory.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_memory.py
+Filename: geckordp-0.4.53/tests/actors/accessibility/test_simulator.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/accessibility/test_simulator.py
+Filename: geckordp-0.4.53/tests/actors/accessibility/test_parent_accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/accessibility/test_parent_accessibility.py
+Filename: geckordp-0.4.53/tests/actors/accessibility/test_accessible.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/accessibility/test_accessible.py
+Filename: geckordp-0.4.53/tests/actors/accessibility/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/accessibility/__init__.py
+Filename: geckordp-0.4.53/tests/actors/accessibility/test_accessible_walker.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/accessibility/test_accessible_walker.py
+Filename: geckordp-0.4.53/tests/actors/accessibility/test_accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/accessibility/test_accessibility.py
+Filename: geckordp-0.4.53/tests/actors/test_heap_snapshot.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_heap_snapshot.py
+Filename: geckordp-0.4.53/tests/actors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_storage.py
+Filename: geckordp-0.4.53/tests/actors/test_network_event.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/__init__.py
+Filename: geckordp-0.4.53/tests/actors/test_network_content.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_event_source.py
+Filename: geckordp-0.4.53/tests/actors/addon/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_network_event.py
+Filename: geckordp-0.4.53/tests/actors/addon/test_addons.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_network_content.py
+Filename: geckordp-0.4.53/tests/actors/addon/test_web_extension_inspected_window.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/addon/__init__.py
+Filename: geckordp-0.4.53/tests/actors/test_device.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/addon/test_addons.py
+Filename: geckordp-0.4.53/tests/actors/test_network_parent.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/addon/test_web_extension_inspected_window.py
+Filename: geckordp-0.4.53/tests/actors/test_storage_local.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_device.py
+Filename: geckordp-0.4.53/tests/actors/test_watcher.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_network_parent.py
+Filename: geckordp-0.4.53/tests/actors/descriptors/test_tab.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_storage_local.py
+Filename: geckordp-0.4.53/tests/actors/descriptors/test_web_extension.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_watcher.py
+Filename: geckordp-0.4.53/tests/actors/descriptors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/descriptors/test_tab.py
+Filename: geckordp-0.4.53/tests/actors/descriptors/test_worker.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/descriptors/test_web_extension.py
+Filename: geckordp-0.4.53/tests/actors/descriptors/test_process.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/descriptors/__init__.py
+Filename: geckordp-0.4.53/tests/actors/test_storage_cache.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/descriptors/test_worker.py
+Filename: geckordp-0.4.53/tests/actors/test_web_console.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/descriptors/test_process.py
+Filename: geckordp-0.4.53/tests/actors/test_node_list.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_storage_cache.py
+Filename: geckordp-0.4.53/tests/actors/test_screenshot.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_web_console.py
+Filename: geckordp-0.4.53/tests/actors/test_preference.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_node_list.py
+Filename: geckordp-0.4.53/tests/actors/test_storage_indexed.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_screenshot.py
+Filename: geckordp-0.4.53/tests/actors/targets/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_preference.py
+Filename: geckordp-0.4.53/tests/actors/targets/test_window_global.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_storage_indexed.py
+Filename: geckordp-0.4.53/tests/actors/targets/test_content_process.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/targets/__init__.py
+Filename: geckordp-0.4.53/tests/actors/test_storage_session.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/targets/test_window_global.py
+Filename: geckordp-0.4.53/tests/actors/test_thread.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/targets/test_content_process.py
+Filename: geckordp-0.4.53/tests/actors/test_storage_extension.py
 Comment: 
 
-Filename: geckordp-0.4.44/tests/actors/test_storage_session.py
-Comment: 
-
-Filename: geckordp-0.4.44/tests/actors/test_thread.py
-Comment: 
-
-Filename: geckordp-0.4.44/tests/actors/test_storage_extension.py
-Comment: 
-
-Filename: geckordp-0.4.44/tests/actors/test_walker.py
+Filename: geckordp-0.4.53/tests/actors/test_walker.py
 Comment: 
 
 Zip file comment:
```

## Comparing `geckordp-0.4.44/geckordp/utils.py` & `geckordp-0.4.53/geckordp/utils.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/logger.py` & `geckordp-0.4.53/geckordp/logger.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/settings.py` & `geckordp-0.4.53/geckordp/settings.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/__init__.py` & `geckordp-0.4.53/geckordp/__init__.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/buffers.py` & `geckordp-0.4.53/geckordp/buffers.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/profile.py` & `geckordp-0.4.53/geckordp/profile.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/firefox.py` & `geckordp-0.4.53/geckordp/firefox.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/rdp_client.py` & `geckordp-0.4.53/geckordp/rdp_client.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/screenshot.py` & `geckordp-0.4.53/geckordp/actors/screenshot.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/node.py` & `geckordp-0.4.53/geckordp/actors/node.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/source.py` & `geckordp-0.4.53/geckordp/actors/source.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/walker.py` & `geckordp-0.4.53/geckordp/actors/walker.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/node_list.py` & `geckordp-0.4.53/geckordp/actors/node_list.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/storage.py` & `geckordp-0.4.53/geckordp/actors/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,28 +78,14 @@
             "to": self.actor_id,
             "type": "removeAll",
             "host": host,
             "name": name,
         })
 
 
-class StorageActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def list_stores(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "listStores",
-        })
-
-
 class CookieStorageActor(_impl_storage, _impl_add_item, _impl_remove_item):
     """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
     """
 
     def edit_item(self, host: str, field: str, old_value, new_value, cookie_data: dict):
         return self.client.send_receive({
             "to": self.actor_id,
```

## Comparing `geckordp-0.4.44/geckordp/actors/network_content.py` & `geckordp-0.4.53/geckordp/actors/network_content.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/accessibility/simulator.py` & `geckordp-0.4.53/geckordp/actors/accessibility/simulator.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/accessibility/accessibility.py` & `geckordp-0.4.53/geckordp/actors/accessibility/accessibility.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/accessibility/accessible_walker.py` & `geckordp-0.4.53/geckordp/actors/accessibility/accessible_walker.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/accessibility/accessible.py` & `geckordp-0.4.53/geckordp/actors/accessibility/accessible.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/accessibility/parent_accessibility.py` & `geckordp-0.4.53/geckordp/actors/accessibility/parent_accessibility.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/event_source.py` & `geckordp-0.4.53/geckordp/actors/web_socket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from geckordp.actors.actor import Actor
 
 
-class EventSourceActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/eventsource.js
+class WebSocketActor(Actor):
+    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/websocket.js
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def start_listening(self):
         return self.client.send({
```

## Comparing `geckordp-0.4.44/geckordp/actors/preference.py` & `geckordp-0.4.53/geckordp/actors/preference.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/network_event.py` & `geckordp-0.4.53/geckordp/actors/network_event.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/memory.py` & `geckordp-0.4.53/geckordp/actors/memory.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/addon/addons.py` & `geckordp-0.4.53/geckordp/actors/addon/addons.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/addon/web_extension_inspected_window.py` & `geckordp-0.4.53/geckordp/actors/addon/web_extension_inspected_window.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/web_console.py` & `geckordp-0.4.53/geckordp/actors/web_console.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/root.py` & `geckordp-0.4.53/geckordp/actors/root.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,19 +61,12 @@
 
     def request_types(self):
         return self.client.send_receive({
             "to": "root",
             "type": "requestTypes"
         }, "requestTypes")
 
-    def echo(self, text: str):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "echo",
-            "text": f"{text}",
-        })
-
     def current_tab(self):
         return self.client.send_receive({
             "to": "root",
             "type": "listTabs"
         }, "tabs[?selected==`true`] | [0]")
```

## Comparing `geckordp-0.4.44/geckordp/actors/descriptors/worker.py` & `geckordp-0.4.53/geckordp/actors/descriptors/worker.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/descriptors/process.py` & `geckordp-0.4.53/geckordp/actors/descriptors/process.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/descriptors/tab.py` & `geckordp-0.4.53/geckordp/actors/descriptors/tab.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/descriptors/web_extension.py` & `geckordp-0.4.53/geckordp/actors/descriptors/web_extension.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/watcher.py` & `geckordp-0.4.53/geckordp/actors/watcher.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/thread.py` & `geckordp-0.4.53/geckordp/actors/thread.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/events.py` & `geckordp-0.4.53/geckordp/actors/events.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/network_parent.py` & `geckordp-0.4.53/geckordp/actors/network_parent.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/target_configuration.py` & `geckordp-0.4.53/geckordp/actors/target_configuration.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/targets/window_global.py` & `geckordp-0.4.53/geckordp/actors/targets/window_global.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 
     def detach(self):
         return self.client.send_receive({
             "to": self.actor_id,
             "type": "detach",
         })
 
-    def ensure_css_error_reporting_enabled(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "ensureCSSErrorReportingEnabled",
-        })
-
     def focus(self):
         return self.client.send_receive({
             "to": self.actor_id,
             "type": "focus",
         })
 
     def go_forward(self):
```

## Comparing `geckordp-0.4.44/geckordp/actors/targets/content_process.py` & `geckordp-0.4.53/geckordp/actors/targets/content_process.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp/actors/inspector.py` & `geckordp-0.4.53/geckordp/actors/inspector.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/geckordp.egg-info/PKG-INFO` & `geckordp-0.4.53/geckordp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geckordp
-Version: 0.4.44
+Version: 0.4.53
 Summary: A client implementation of Firefox DevTools over remote debug protocol
 Home-page: https://github.com/jpramosi/geckordp
 Author: jpramosi
 Author-email: jimmy.pramosi@protonmail.com
 License: MIT
 Project-URL: Documentation, https://jpramosi.github.io/geckordp
 Project-URL: Source, https://github.com/jpramosi/geckordp
@@ -128,17 +128,17 @@
 
 
 ## Tested Platforms
 <!-- SEPARATOR -->
 
 | Tested Platform                            | Working                 | Firefox-Version         | Geckordp-Version        |
 | -------------------------------------------| ------------------------| ------------------------| ------------------------|
-| Windows (x64)                              | yes                     |  110.0                   |  0.4.44                  |
-| Ubuntu 20.04                               | yes                     |  110.0                   |  0.4.44                  |
-| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  110.0                   |  0.4.44                  |
+| Windows (x64)                              | yes                     |  113.0                   |  0.4.53                  |
+| Ubuntu 20.04                               | yes                     |  113.0                   |  0.4.53                  |
+| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.4.53                  |
 
 Geckordp requires minimum Python 3.10 and the latest Firefox build. Older versions of Firefox may also work as long the API changes are not too drastically. In case of doubt, clone and run tests with:
 ```bash
 cd <your-repositories-path>
 git clone https://github.com/jpramosi/geckordp
 cd geckordp
 python -m pip uninstall geckordp
@@ -294,15 +294,15 @@
 
 
 ## License
 <!-- SEPARATOR -->
 ```
 MIT License
 
-Copyright (c) 2022 jpramosi
+Copyright (c) 2023 jpramosi
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `geckordp-0.4.44/geckordp.egg-info/SOURCES.txt` & `geckordp-0.4.53/geckordp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 geckordp.egg-info/SOURCES.txt
 geckordp.egg-info/dependency_links.txt
 geckordp.egg-info/requires.txt
 geckordp.egg-info/top_level.txt
 geckordp/actors/__init__.py
 geckordp/actors/actor.py
 geckordp/actors/device.py
-geckordp/actors/event_source.py
 geckordp/actors/events.py
 geckordp/actors/heap_snapshot.py
 geckordp/actors/inspector.py
 geckordp/actors/memory.py
 geckordp/actors/network_content.py
 geckordp/actors/network_event.py
 geckordp/actors/network_parent.py
@@ -54,28 +53,26 @@
 geckordp/actors/descriptors/web_extension.py
 geckordp/actors/descriptors/worker.py
 geckordp/actors/targets/__init__.py
 geckordp/actors/targets/content_process.py
 geckordp/actors/targets/window_global.py
 tests/actors/__init__.py
 tests/actors/test_device.py
-tests/actors/test_event_source.py
 tests/actors/test_heap_snapshot.py
 tests/actors/test_inspector.py
 tests/actors/test_memory.py
 tests/actors/test_network_content.py
 tests/actors/test_network_event.py
 tests/actors/test_network_parent.py
 tests/actors/test_node.py
 tests/actors/test_node_list.py
 tests/actors/test_preference.py
 tests/actors/test_root.py
 tests/actors/test_screenshot.py
 tests/actors/test_source.py
-tests/actors/test_storage.py
 tests/actors/test_storage_cache.py
 tests/actors/test_storage_cookie.py
 tests/actors/test_storage_extension.py
 tests/actors/test_storage_indexed.py
 tests/actors/test_storage_local.py
 tests/actors/test_storage_session.py
 tests/actors/test_thread.py
```

## Comparing `geckordp-0.4.44/setup.py` & `geckordp-0.4.53/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from setuptools import setup, find_packages
 
 NAME = "geckordp"
 EMAIL = "jimmy.pramosi@protonmail.com"
-__version__ = "0.4.44"
+__version__ = "0.4.53"
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 10)
 
 # check version
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
         """
```

## Comparing `geckordp-0.4.44/PKG-INFO` & `geckordp-0.4.53/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geckordp
-Version: 0.4.44
+Version: 0.4.53
 Summary: A client implementation of Firefox DevTools over remote debug protocol
 Home-page: https://github.com/jpramosi/geckordp
 Author: jpramosi
 Author-email: jimmy.pramosi@protonmail.com
 License: MIT
 Project-URL: Documentation, https://jpramosi.github.io/geckordp
 Project-URL: Source, https://github.com/jpramosi/geckordp
@@ -128,17 +128,17 @@
 
 
 ## Tested Platforms
 <!-- SEPARATOR -->
 
 | Tested Platform                            | Working                 | Firefox-Version         | Geckordp-Version        |
 | -------------------------------------------| ------------------------| ------------------------| ------------------------|
-| Windows (x64)                              | yes                     |  110.0                   |  0.4.44                  |
-| Ubuntu 20.04                               | yes                     |  110.0                   |  0.4.44                  |
-| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  110.0                   |  0.4.44                  |
+| Windows (x64)                              | yes                     |  113.0                   |  0.4.53                  |
+| Ubuntu 20.04                               | yes                     |  113.0                   |  0.4.53                  |
+| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.4.53                  |
 
 Geckordp requires minimum Python 3.10 and the latest Firefox build. Older versions of Firefox may also work as long the API changes are not too drastically. In case of doubt, clone and run tests with:
 ```bash
 cd <your-repositories-path>
 git clone https://github.com/jpramosi/geckordp
 cd geckordp
 python -m pip uninstall geckordp
@@ -294,15 +294,15 @@
 
 
 ## License
 <!-- SEPARATOR -->
 ```
 MIT License
 
-Copyright (c) 2022 jpramosi
+Copyright (c) 2023 jpramosi
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `geckordp-0.4.44/README.md` & `geckordp-0.4.53/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,17 @@
 
 
 ## Tested Platforms
 <!-- SEPARATOR -->
 
 | Tested Platform                            | Working                 | Firefox-Version         | Geckordp-Version        |
 | -------------------------------------------| ------------------------| ------------------------| ------------------------|
-| Windows (x64)                              | yes                     |  110.0                   |  0.4.44                  |
-| Ubuntu 20.04                               | yes                     |  110.0                   |  0.4.44                  |
-| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  110.0                   |  0.4.44                  |
+| Windows (x64)                              | yes                     |  113.0                   |  0.4.53                  |
+| Ubuntu 20.04                               | yes                     |  113.0                   |  0.4.53                  |
+| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.4.53                  |
 
 Geckordp requires minimum Python 3.10 and the latest Firefox build. Older versions of Firefox may also work as long the API changes are not too drastically. In case of doubt, clone and run tests with:
 ```bash
 cd <your-repositories-path>
 git clone https://github.com/jpramosi/geckordp
 cd geckordp
 python -m pip uninstall geckordp
@@ -272,15 +272,15 @@
 
 
 ## License
 <!-- SEPARATOR -->
 ```
 MIT License
 
-Copyright (c) 2022 jpramosi
+Copyright (c) 2023 jpramosi
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `geckordp-0.4.44/tests/helpers/utils.py` & `geckordp-0.4.53/tests/helpers/utils.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_storage_cookie.py` & `geckordp-0.4.53/tests/actors/test_storage_cookie.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_source.py` & `geckordp-0.4.53/tests/actors/test_source.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_node.py` & `geckordp-0.4.53/tests/actors/test_node.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_inspector.py` & `geckordp-0.4.53/tests/actors/test_inspector.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_root.py` & `geckordp-0.4.53/tests/actors/test_root.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,7 @@
     try:
         cl, root = init()
         types = root.request_types()
         assert len(types) >= 2
         assert "getRoot" in types and "listTabs" in types
     finally:
         cl.disconnect()
-
-
-def test_echo():
-    cl = None
-    try:
-        cl, root = init()
-        types = root.echo("hello")
-        assert types["text"] == "hello"
-    finally:
-        cl.disconnect()
```

## Comparing `geckordp-0.4.44/tests/actors/test_memory.py` & `geckordp-0.4.53/tests/actors/test_memory.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/accessibility/test_simulator.py` & `geckordp-0.4.53/tests/actors/accessibility/test_simulator.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/accessibility/test_parent_accessibility.py` & `geckordp-0.4.53/tests/actors/accessibility/test_parent_accessibility.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/accessibility/test_accessible.py` & `geckordp-0.4.53/tests/actors/accessibility/test_accessible.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/accessibility/test_accessible_walker.py` & `geckordp-0.4.53/tests/actors/accessibility/test_accessible_walker.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/accessibility/test_accessibility.py` & `geckordp-0.4.53/tests/actors/accessibility/test_accessibility.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_heap_snapshot.py` & `geckordp-0.4.53/tests/actors/test_heap_snapshot.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_storage.py` & `geckordp-0.4.53/tests/actors/descriptors/test_process.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 # pylint: disable=unused-import
 import pytest
 import tests.helpers.constants as constants
 from tests.helpers.utils import *
 from geckordp.rdp_client import RDPClient
 from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.storage import StorageActor
+from geckordp.actors.descriptors.process import ProcessActor
 from geckordp.logger import log, logdict
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
-    current_tab = root.current_tab()
-    tab = TabActor(cl, current_tab["actor"])
-    actor_ids = tab.get_target()
-    storage = StorageActor(cl, actor_ids["storageActor"])
-    return cl, storage
+    processes = root.list_processes()
+    process = ProcessActor(
+        cl, processes[0]["actor"])
+    return cl, process
 
 
-def test_list_stores():
+def test_get_target():
     cl = None
     try:
-        cl, storage = init()
-        val = storage.list_stores()
-        assert response_valid("storageActor", val), str(val)
+        cl, process = init()
+        val = process.get_target()["consoleActor"]
+        assert "consoleActor" in val
+    finally:
+        cl.disconnect()
+
+
+def test_get_watcher():
+    cl = None
+    try:
+        cl, process = init()
+        val = process.get_watcher()["actor"]
+        assert "watcher" in val
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.44/tests/actors/test_event_source.py` & `geckordp-0.4.53/tests/actors/descriptors/test_worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # pylint: disable=unused-import
 import pytest
 import tests.helpers.constants as constants
 from tests.helpers.utils import *
 from geckordp.rdp_client import RDPClient
 from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.event_source import EventSourceActor
+from geckordp.actors.descriptors.worker import WorkerActor
 from geckordp.logger import log, logdict
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
-    current_tab = root.current_tab()
-    tab = TabActor(cl, current_tab["actor"])
-    actor_ids = tab.get_target()
-    event_source = EventSourceActor(cl, actor_ids["eventSourceActor"])
-    return cl, event_source
+    workers = root.list_workers()
+    worker = WorkerActor(cl, workers[0]["actor"])
+    return cl, worker
 
 
-def test_start_listening():
+def test_detach():
     cl = None
     try:
-        cl, event_source = init()
-        event_source.start_listening()
+        cl, worker = init()
+        worker.detach()
     finally:
         cl.disconnect()
 
 
-def test_stop_listening():
+def test_get_target():
     cl = None
     try:
-        cl, event_source = init()
-        event_source.stop_listening()
+        cl, worker = init()
+        val = worker.get_target()["type"]
+        assert "connected" in val
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.44/tests/actors/test_network_event.py` & `geckordp-0.4.53/tests/actors/test_network_event.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_network_content.py` & `geckordp-0.4.53/tests/actors/test_network_content.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/addon/test_addons.py` & `geckordp-0.4.53/tests/actors/addon/test_addons.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/addon/test_web_extension_inspected_window.py` & `geckordp-0.4.53/tests/actors/addon/test_web_extension_inspected_window.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_device.py` & `geckordp-0.4.53/tests/actors/test_device.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_network_parent.py` & `geckordp-0.4.53/tests/actors/test_network_parent.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_storage_local.py` & `geckordp-0.4.53/tests/actors/test_storage_local.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_watcher.py` & `geckordp-0.4.53/tests/actors/test_watcher.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/descriptors/test_tab.py` & `geckordp-0.4.53/tests/actors/descriptors/test_tab.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/descriptors/test_web_extension.py` & `geckordp-0.4.53/tests/actors/descriptors/test_web_extension.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/descriptors/test_worker.py` & `geckordp-0.4.53/tests/actors/targets/test_content_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # pylint: disable=unused-import
 import pytest
 import tests.helpers.constants as constants
 from tests.helpers.utils import *
 from geckordp.rdp_client import RDPClient
 from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.worker import WorkerActor
+from geckordp.actors.descriptors.process import ProcessActor
+from geckordp.actors.targets.content_process import ContentProcessActor
 from geckordp.logger import log, logdict
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
-    workers = root.list_workers()
-    worker = WorkerActor(cl, workers[0]["actor"])
-    return cl, worker
+    processes = root.list_processes()
+    content_process = None
+    for p in processes:
+        if (not p["isParent"]):
+            process = ProcessActor(cl, p["actor"])
+            content_process = ContentProcessActor(
+                cl, process.get_target()["actor"])
+            break
+    return cl, content_process
 
 
-def test_detach():
+def test_list_workers():
     cl = None
     try:
-        cl, worker = init()
-        worker.detach()
+        cl, content_process = init()
+        val = content_process.list_workers()
+        assert len(val) >= 0
     finally:
         cl.disconnect()
 
 
-def test_get_target():
+def test_pause_matching_service_workers():
     cl = None
     try:
-        cl, worker = init()
-        val = worker.get_target()["type"]
-        assert "connected" in val
+        cl, content_process = init()
+        val = content_process.pause_matching_service_workers()
+        assert response_valid("contentProcessTarget", val), str(val)
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.44/tests/actors/test_storage_cache.py` & `geckordp-0.4.53/tests/actors/test_storage_cache.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_web_console.py` & `geckordp-0.4.53/tests/actors/test_web_console.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_node_list.py` & `geckordp-0.4.53/tests/actors/test_node_list.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_screenshot.py` & `geckordp-0.4.53/tests/actors/test_screenshot.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_preference.py` & `geckordp-0.4.53/tests/actors/test_preference.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_storage_indexed.py` & `geckordp-0.4.53/tests/actors/test_storage_indexed.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/targets/test_window_global.py` & `geckordp-0.4.53/tests/actors/targets/test_window_global.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,24 +27,14 @@
         cl, browser = init()
         val = browser.detach()
         assert response_valid("windowGlobalTarget", val), str(val)
     finally:
         cl.disconnect()
 
 
-def test_ensure_css_error_reporting_enabled():
-    cl = None
-    try:
-        cl, browser = init()
-        val = browser.ensure_css_error_reporting_enabled()
-        assert response_valid("windowGlobalTarget", val), str(val)
-    finally:
-        cl.disconnect()
-
-
 def test_focus():
     cl = None
     try:
         cl, browser = init()
         val = browser.focus()
         assert response_valid("windowGlobalTarget", val), str(val)
     finally:
```

## Comparing `geckordp-0.4.44/tests/actors/test_storage_session.py` & `geckordp-0.4.53/tests/actors/test_storage_session.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_thread.py` & `geckordp-0.4.53/tests/actors/test_thread.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_storage_extension.py` & `geckordp-0.4.53/tests/actors/test_storage_extension.py`

 * *Files identical despite different names*

## Comparing `geckordp-0.4.44/tests/actors/test_walker.py` & `geckordp-0.4.53/tests/actors/test_walker.py`

 * *Files identical despite different names*

