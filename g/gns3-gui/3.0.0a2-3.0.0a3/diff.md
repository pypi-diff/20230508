# Comparing `tmp/gns3-gui-3.0.0a2.tar.gz` & `tmp/gns3-gui-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gns3-gui-3.0.0a2.tar", last modified: Tue Sep  6 23:14:08 2022, max compression
+gzip compressed data, was "gns3-gui-3.0.0a3.tar", last modified: Tue Dec 27 07:36:33 2022, max compression
```

## Comparing `gns3-gui-3.0.0a2.tar` & `gns3-gui-3.0.0a3.tar`

### file list

```diff
@@ -1,883 +1,883 @@
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.095902 gns3-gui-3.0.0a2/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       35 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/AUTHORS
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22882 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/COPYING
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35147 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/LICENSE
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      238 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/MANIFEST.in
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2867 2022-09-06 23:14:08.095902 gns3-gui-3.0.0a2/PKG-INFO
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1670 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/README.md
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.771907 gns3-gui-3.0.0a2/gns3/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       33 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      736 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/__main__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3180 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/appliance_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2742 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/application.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8604 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/base_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5711 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/compute.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9953 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/compute_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7934 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/compute_summary_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9461 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/console_cmd.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9947 2022-08-30 09:42:14.000000 gns3-gui-3.0.0a2/gns3/console_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16418 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/controller.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6678 2022-09-06 23:02:02.000000 gns3-gui-3.0.0a2/gns3/crash_report.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.779907 gns3-gui-3.0.0a2/gns3/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1197 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/about_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30809 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/appliance_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/capture_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2339 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/configuration_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/console_command_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8429 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/custom_adapters_configuration_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7834 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/doctor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3310 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/edit_compute_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6900 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/edit_project_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1993 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/exec_command_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4830 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/export_debug_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/file_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/filter_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3579 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/idlepc_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6480 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/image_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/login_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11851 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/new_template_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/node_info_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11399 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/node_properties_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/notif_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9036 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/preferences_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3788 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/profile_select.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14147 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/project_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9689 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/project_export_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3411 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/project_welcome_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11056 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/setup_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2457 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/show_readme_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5704 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/snapshots_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6355 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/style_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4600 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/style_editor_dialog_link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7859 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/symbol_selection_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4714 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/text_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7249 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/dialogs/vm_with_images_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6493 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/dialogs/vm_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    70254 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/graphics_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31751 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/http_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1690 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/http_client_error.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8433 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/image_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2397 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/image_upload_manager.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.783907 gns3-gui-3.0.0a2/gns3/items/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9857 2022-08-29 21:29:31.000000 gns3-gui-3.0.0a2/gns3/items/drawing_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/ellipse_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10344 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/ethernet_link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2428 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/image_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8318 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/label_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/line_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21441 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/items/link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4404 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/logo_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/node_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1989 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/rectangle_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7942 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/serial_link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7452 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/shape_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6164 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/text_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1058 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/items/utils.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18698 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19682 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/local_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21068 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/local_server.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/logger.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12007 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/main.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    55926 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/main_window.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.783907 gns3-gui-3.0.0a2/gns3/modules/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1095 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.787907 gns3-gui-3.0.0a2/gns3/modules/builtin/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4854 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5616 2022-07-25 10:38:28.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/atm_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5123 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/cloud.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.787907 gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/cloud_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1930 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2893 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ethernet_hub.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4559 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ethernet_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4087 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/frame_relay_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2437 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/nat.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.791907 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7683 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/atm_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2595 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/builtin_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22227 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/cloud_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9690 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/cloud_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5598 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9526 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10234 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10250 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6627 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1750 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.799907 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9107 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/atm_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13163 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2666 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/builtin_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3269 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/builtin_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19129 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24391 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4401 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5315 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3433 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5232 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3876 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5670 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4431 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5536 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4186 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6247 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9148 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13299 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4397 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5674 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4222 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6343 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7303 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11148 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.799907 gns3-gui-3.0.0a2/gns3/modules/builtin/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1212 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/builtin/utils/tree_widget_item.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.803907 gns3-gui-3.0.0a2/gns3/modules/docker/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4407 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.803907 gns3-gui-3.0.0a2/gns3/modules/docker/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5356 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/dialogs/docker_vm_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5190 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/docker_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.803907 gns3-gui-3.0.0a2/gns3/modules/docker/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1968 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/pages/docker_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9347 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/pages/docker_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12245 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/pages/docker_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1385 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.807906 gns3-gui-3.0.0a2/gns3/modules/docker/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2400 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2852 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12930 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17480 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4709 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11020 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16543 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.811906 gns3-gui-3.0.0a2/gns3/modules/dynamips/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7828 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2360 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/adapters.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.811906 gns3-gui-3.0.0a2/gns3/modules/dynamips/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17596 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/dialogs/ios_router_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.819906 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1759 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c1700.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2320 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c2600.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c2691.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c3600.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c3725.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c3745.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c7200.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2218 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/etherswitch_router.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12172 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/router.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.819906 gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/dynamips_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27874 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/ios_router_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22457 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/ios_router_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7767 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.823906 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     6439 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/dynamips_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8491 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    35772 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    45950 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4850 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5957 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15247 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.827906 gns3-gui-3.0.0a2/gns3/modules/dynamips/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/utils/decompress_ios.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2179 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/utils/decompress_ios_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/dynamips/wics.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.827906 gns3-gui-3.0.0a2/gns3/modules/iou/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3974 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.831906 gns3-gui-3.0.0a2/gns3/modules/iou/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/iou/dialogs/iou_device_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4932 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/iou/iou_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.831906 gns3-gui-3.0.0a2/gns3/modules/iou/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13513 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/iou/pages/iou_device_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15081 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/iou/pages/iou_device_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5027 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/pages/iou_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1305 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/iou/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.835906 gns3-gui-3.0.0a2/gns3/modules/iou/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    13890 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17361 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4638 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5659 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6717 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2927 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3557 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/module.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1066 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/module_error.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.835906 gns3-gui-3.0.0a2/gns3/modules/qemu/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5394 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.835906 gns3-gui-3.0.0a2/gns3/modules/qemu/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8042 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/dialogs/qemu_image_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4726 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/dialogs/qemu_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.839906 gns3-gui-3.0.0a2/gns3/modules/qemu/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2896 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/pages/qemu_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30339 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/pages/qemu_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15055 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/pages/qemu_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7486 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/qemu_vm.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2017 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.843906 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23636 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_image_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29391 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_image_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2888 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3655 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    32090 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    42819 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4602 2021-10-08 05:49:21.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5444 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12608 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18585 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.843906 gns3-gui-3.0.0a2/gns3/modules/virtualbox/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5807 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.843906 gns3-gui-3.0.0a2/gns3/modules/virtualbox/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3607 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.847906 gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4001 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11547 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10014 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1438 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.847906 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3684 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4480 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    10804 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4373 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3801 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5833 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4955 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/modules/virtualbox/virtualbox_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.847906 gns3-gui-3.0.0a2/gns3/modules/vmware/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10348 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.847906 gns3-gui-3.0.0a2/gns3/modules/vmware/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3531 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/dialogs/vmware_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.851906 gns3-gui-3.0.0a2/gns3/modules/vmware/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/pages/vmware_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11191 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/pages/vmware_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10365 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/pages/vmware_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1731 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.851906 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7503 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8865 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9806 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13005 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4329 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5270 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3802 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5702 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6183 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vmware/vmware_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.855906 gns3-gui-3.0.0a2/gns3/modules/vpcs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4669 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.855906 gns3-gui-3.0.0a2/gns3/modules/vpcs/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.855906 gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7092 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9184 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/vpcs_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1064 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.859906 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4135 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6719 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4278 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4868 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3424 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5202 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3653 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4263 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a2/gns3/modules/vpcs/vpcs_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1630 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/network_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29180 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/nodes_dock_widget.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9340 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/nodes_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10620 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/packet_capture.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.859906 gns3-gui-3.0.0a2/gns3/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14166 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/pages/controller_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21133 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/pages/general_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/pages/gns3_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/pages/packet_capture_preferences_page.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.863906 gns3-gui-3.0.0a2/gns3/ports/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ports/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ports/ethernet_port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8108 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ports/port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2335 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ports/port_name_factory.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      887 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ports/serial_port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10489 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/progress.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25052 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/project.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/pycutext.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.863906 gns3-gui-3.0.0a2/gns3/qt/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7943 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/qt/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/qt/qimage_svg_renderer.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.863906 gns3-gui-3.0.0a2/gns3/registry/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/registry/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7028 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/registry/appliance.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9250 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/registry/appliance_to_template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2646 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/registry/config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4251 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/registry/image.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4698 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/registry/registry.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.863906 gns3-gui-3.0.0a2/gns3/schemas/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15212 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/schemas/appliance.json
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18517 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/settings.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2148 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/spice_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.863906 gns3-gui-3.0.0a2/gns3/static/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/static/.keep
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2732 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/status_bar.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/style.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/symbol.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3815 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/telnet_console.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8435 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/template_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20587 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/topology.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14489 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/topology_summary_view.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.907905 gns3-gui-3.0.0a2/gns3/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    96556 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/about_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   112145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/about_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9192 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/appliance_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11305 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/appliance_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3516 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/capture_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4471 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/capture_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3197 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/configuration_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/configuration_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/console_command_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/console_command_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    18928 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/controller_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23470 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/controller_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2012 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/custom_adapters_configuration_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2258 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/custom_adapters_configuration_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3252 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/doctor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3521 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/doctor_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5487 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/edit_compute_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6478 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/edit_compute_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9096 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/edit_project_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11089 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/edit_project_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     1694 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/exec_command_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/exec_command_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3559 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/export_debug_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3716 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/export_debug_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5607 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/export_project_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8170 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/export_project_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3422 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/file_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/file_editor_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3881 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/filter_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3708 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/filter_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    42307 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/general_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53669 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/general_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7845 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/gns3_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10781 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/gns3_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1824 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/idlepc_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1919 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/idlepc_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3693 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/image_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3823 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/image_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2758 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/login_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2734 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/login_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    41586 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/main_window.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    50821 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/main_window_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3059 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/new_template_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4766 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/new_template_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2636 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/node_info_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/node_info_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/node_properties_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5071 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/node_properties_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4366 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/packet_capture_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/packet_capture_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4704 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/preferences_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/preferences_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4950 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/profile_select_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/profile_select_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/project_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11436 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/project_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2754 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/project_welcome_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/project_welcome_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)  9439247 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/resources_rc.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7770 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/setup_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11373 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/setup_wizard_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     2778 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/show_readme_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2882 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/ui/show_readme_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2357 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/snapshots_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2588 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/snapshots_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4807 2021-06-12 04:52:20.000000 gns3-gui-3.0.0a2/gns3/ui/style_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6125 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/style_editor_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/symbol_selection_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5838 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/symbol_selection_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4884 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a2/gns3/ui/text_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/ui/text_editor_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10594 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/update_manager.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.911905 gns3-gui-3.0.0a2/gns3/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3691 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5724 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/analytics.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2799 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/bring_to_front.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/file_copy_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1326 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/get_icon.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2239 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/get_resource.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/gns3/utils/import_project_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/interfaces.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1256 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/normalize_filename.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5435 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/process_files_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/progress_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/run_in_terminal.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2524 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/server_select.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4424 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/sudo.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2420 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/wait_for_command_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2713 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/wait_for_connection_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2288 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/wait_for_lambda_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2850 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/utils/wait_for_runas_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1490 2022-09-06 23:05:29.000000 gns3-gui-3.0.0a2/gns3/version.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2072 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/gns3/vnc_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.911905 gns3-gui-3.0.0a2/gns3_gui.egg-info/
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2867 2022-09-06 23:14:07.000000 gns3-gui-3.0.0a2/gns3_gui.egg-info/PKG-INFO
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    29963 2022-09-06 23:14:07.000000 gns3-gui-3.0.0a2/gns3_gui.egg-info/SOURCES.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        1 2022-09-06 23:14:07.000000 gns3-gui-3.0.0a2/gns3_gui.egg-info/dependency_links.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       37 2022-09-06 23:14:07.000000 gns3-gui-3.0.0a2/gns3_gui.egg-info/entry_points.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       83 2022-09-06 23:14:07.000000 gns3-gui-3.0.0a2/gns3_gui.egg-info/requires.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        5 2022-09-06 23:14:07.000000 gns3-gui-3.0.0a2/gns3_gui.egg-info/top_level.txt
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      158 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/requirements.txt
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.911905 gns3-gui-3.0.0a2/resources/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.947904 gns3-gui-3.0.0a2/resources/charcoal_icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6231 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/add-link-1-cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/add-link-1-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/add-link-1.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/add-note-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/aux-console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/browse-all-icons-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/browse-all-icons.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13891 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/calculate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2220 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2127 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/capture-start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/capture-stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3362 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/command_line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/configuration-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8406 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/console_edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4172 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/delete-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4156 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2881 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/duplicate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3852 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3846 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/export-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2822 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/filter-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/filter-reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25640 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24989 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/firewall-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/front-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12619 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/help-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12581 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/image-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/import-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/import_export_configs-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2409 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/inspect-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4013 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/link-pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3593 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/link-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3738 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/lock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3730 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3546 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/lower_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/minus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/new-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4223 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/node_conception-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/open-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/pc-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/pc.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2680 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/plus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2673 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6090 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/preferences-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6084 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/preferences.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5543 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/quit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5870 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/raise_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3542 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/reload-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2181 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2175 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/router-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5279 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/save-as-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5281 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/save-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/save-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/show-hostname-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/show-interface-names-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/snapshot-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2684 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/switch-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/unlock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-in-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-in.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2808 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-out-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1746 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-out.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.995903 gns3-gui-3.0.0a2/resources/classic_icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5935 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/add-link-cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2971 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/add-link-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3086 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/add-link.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4148 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/add-note-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2593 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/aux-console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2589 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/browse-all-icons-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5646 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/browse-all-icons.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13890 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/calculate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2992 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2914 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/capture-start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3368 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/capture-stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3363 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/command_line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6254 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/configuration-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2046 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2070 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/console_edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4162 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/delete-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/duplicate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3856 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4312 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4321 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/export-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24995 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/filter-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/filter-reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25639 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24990 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2047 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/firewall-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2056 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/front-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9629 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/help-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9625 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2011 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/image-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2020 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/import-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2351 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/import_export_configs-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2373 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/inspect-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2382 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4003 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/classic_icons/link-pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3593 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/classic_icons/link-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/lock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3731 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3545 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/lower_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/minus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4249 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/new-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4245 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/node_conception-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2243 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/open-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2166 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/pc-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3493 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/pc.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2679 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/plus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2674 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5725 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/preferences-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5719 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/preferences.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5032 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/quit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5026 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/raise_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3541 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2530 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2539 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2266 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/reload-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2275 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2180 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2174 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2313 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/router-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2322 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4710 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/save-as-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4748 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3383 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/save-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3417 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/save-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/show-hostname-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3636 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/show-interface-names-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3686 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2876 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/snapshot-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2901 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1742 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2495 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/switch-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/unlock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2761 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/zoom-in-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2785 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/zoom-in.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2719 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/zoom-out-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2727 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/classic_icons/zoom-out.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.039903 gns3-gui-3.0.0a2/resources/icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    63187 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/PC-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    60045 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/PC.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    28134 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16099 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/applications.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21937 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   291074 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/browse-all-icons-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   297712 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/browse-all-icons.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32570 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39042 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    37642 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25560 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/cancel-connection.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31090 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26448 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19139 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23701 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/connection-new-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23702 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/connection-new.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21216 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13772 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/dialog-warning.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26729 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/drawing.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23490 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16831 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24733 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21372 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10572 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21681 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/filter-capture.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23917 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    57273 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/firewall-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53702 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/firewall.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13259 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7175 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/horizontally.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19675 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10549 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39319 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15756 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/led_gray.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/led_green.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6952 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/led_red.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9965 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/led_yellow.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32132 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6518 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4612 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24126 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16626 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/new.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27187 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30745 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23462 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21534 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19130 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7903 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35282 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31055 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16810 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8571 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    58719 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/router-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54133 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/router.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/rtv.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    40599 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31854 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/save-as.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29835 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/save.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15166 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26306 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18013 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17454 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    67991 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/switch-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    64865 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/switch.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    34969 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5816 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/vertically.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/virtualbox.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/warning.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1906 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/wireshark.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5939 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/zoom-in-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/zoom-in.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/zoom-out-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6157 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/icons/zoom-out.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.043902 gns3-gui-3.0.0a2/resources/images/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   370070 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/images/gns3.ico
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7892 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/images/gns3_icon_128x128.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16745 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/images/gns3_icon_256x256.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7921 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/images/gns3_logo.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.043902 gns3-gui-3.0.0a2/resources/linux/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.043902 gns3-gui-3.0.0a2/resources/linux/applications/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      282 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/applications/gns3.desktop
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/gns3-gui.xml
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.751907 gns3-gui-3.0.0a2/resources/linux/icons/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.751907 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.751907 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/16x16/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.043902 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/16x16/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      832 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/16x16/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.751907 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/32x32/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.043902 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/32x32/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/32x32/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.751907 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.047902 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.047902 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6075 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4500 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.751907 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.051902 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/apps/gns3.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.055902 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11492 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16025 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/resources.qrc
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.055902 gns3-gui-3.0.0a2/resources/styles/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1231 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/resources/styles/charcoal.css
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.067902 gns3-gui-3.0.0a2/resources/symbols/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16298 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/atm_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    78565 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/cloud.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/computer.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19782 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/docker_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18650 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/ethernet_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18401 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18343 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/frame_relay_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18128 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/hub.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19150 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/multilayer_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18421 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/qemu_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18494 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16401 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/vbox_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16843 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/vmware_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/resources/symbols/vpcs_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       38 2022-09-06 23:14:08.095902 gns3-gui-3.0.0a2/setup.cfg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4467 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/setup.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.079902 gns3-gui-3.0.0a2/tests/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6558 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/conftest.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.083902 gns3-gui-3.0.0a2/tests/items/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1997 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/items/test_ellipse_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1509 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/items/test_image_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/items/test_label_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/items/test_line_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3046 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/items/test_rectangle_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/items/test_text_item.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:07.755907 gns3-gui-3.0.0a2/tests/modules/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.083902 gns3-gui-3.0.0a2/tests/modules/docker/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1478 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/modules/docker/test_docker_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.083902 gns3-gui-3.0.0a2/tests/modules/dynamips/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1486 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/modules/dynamips/test_dynamips_init.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.083902 gns3-gui-3.0.0a2/tests/modules/iou/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1841 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/modules/iou/test_iou_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.087902 gns3-gui-3.0.0a2/tests/modules/qemu/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1526 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/modules/qemu/test_qemu_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.087902 gns3-gui-3.0.0a2/tests/modules/virtualbox/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/modules/virtualbox/test_virtualbox_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.087902 gns3-gui-3.0.0a2/tests/modules/vpcs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/modules/vpcs/test_vpcs_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.087902 gns3-gui-3.0.0a2/tests/qt/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/qt/test_qimage_svg_renderer.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.091902 gns3-gui-3.0.0a2/tests/registry/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.095902 gns3-gui-3.0.0a2/tests/registry/appliances/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2395 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/arista-veos.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1356 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/broken-microcore-linux.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1298 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/cisco-3745.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      961 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/cisco-iou-l3.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1620 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/juniper-vsrx.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2025 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/microcore-linux.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/appliances/openvswitch.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/test_appliance.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10579 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/registry/test_appliance_to_template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2895 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/registry/test_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2304 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/test_image.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2185 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/registry/test_registry.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1376 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_compute.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5771 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_compute_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1717 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_controller.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_graphics_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8702 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_http_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3093 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_image_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1596 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_image_upload_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4739 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13656 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_local_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2756 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_local_server.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1420 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_main_window.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_network_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5698 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_progress.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5498 2022-08-29 17:14:02.000000 gns3-gui-3.0.0a2/tests/test_project.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_spice_console.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_topology.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3593 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_update_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_utils.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1814 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/test_vnc_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-09-06 23:14:08.095902 gns3-gui-3.0.0a2/tests/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1394 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/utils/test_file_copy_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3705 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a2/tests/utils/test_server_select.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.830072 gns3-gui-3.0.0a3/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       35 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/AUTHORS
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22882 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/COPYING
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35147 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/LICENSE
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      238 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/MANIFEST.in
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2916 2022-12-27 07:36:33.830072 gns3-gui-3.0.0a3/PKG-INFO
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1670 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/README.md
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.278066 gns3-gui-3.0.0a3/gns3/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       33 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      736 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/__main__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3456 2022-12-27 05:53:55.000000 gns3-gui-3.0.0a3/gns3/appliance_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2893 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/application.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8604 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/base_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5711 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/compute.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9953 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/compute_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7934 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/compute_summary_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9461 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/console_cmd.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9947 2022-08-30 09:42:14.000000 gns3-gui-3.0.0a3/gns3/console_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16385 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/controller.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6665 2022-12-27 07:16:29.000000 gns3-gui-3.0.0a3/gns3/crash_report.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.290067 gns3-gui-3.0.0a3/gns3/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1197 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/about_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30809 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/appliance_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/capture_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2339 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/configuration_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/console_command_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8429 2022-11-02 16:17:56.000000 gns3-gui-3.0.0a3/gns3/dialogs/custom_adapters_configuration_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7834 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/doctor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3310 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/edit_compute_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6711 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/edit_project_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1993 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/exec_command_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4830 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/export_debug_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/file_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/filter_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3579 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/idlepc_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6480 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/image_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/login_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11851 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/new_template_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/node_info_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11399 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/node_properties_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/notif_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9036 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/preferences_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3788 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/profile_select.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14147 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/project_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9689 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/project_export_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3411 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/project_welcome_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11056 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/setup_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2457 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/show_readme_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5704 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/snapshots_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6355 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/style_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4600 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/style_editor_dialog_link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7859 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/symbol_selection_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4714 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/text_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7249 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/dialogs/vm_with_images_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6493 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/dialogs/vm_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    70254 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/graphics_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32119 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/http_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1690 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/http_client_error.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8433 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/image_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2347 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/image_upload_manager.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.302067 gns3-gui-3.0.0a3/gns3/items/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9857 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/items/drawing_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/ellipse_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10344 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/ethernet_link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2428 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/image_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8318 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/label_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/line_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21441 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/items/link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4404 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/logo_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/node_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1989 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/rectangle_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7942 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/serial_link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7452 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/shape_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6164 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/text_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1058 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/items/utils.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18698 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19682 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/local_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21068 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/local_server.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/logger.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12007 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/main.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    55926 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/main_window.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.302067 gns3-gui-3.0.0a3/gns3/modules/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1095 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.306067 gns3-gui-3.0.0a3/gns3/modules/builtin/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4854 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5616 2022-07-25 10:38:28.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/atm_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5123 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/cloud.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.306067 gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/cloud_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1930 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2893 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ethernet_hub.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4559 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ethernet_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4087 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/frame_relay_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2437 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/nat.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.310067 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7683 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/atm_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2595 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/builtin_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22227 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/cloud_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9690 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/cloud_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5598 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9526 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10381 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10250 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6627 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1750 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.322067 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9107 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/atm_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13163 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2666 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/builtin_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3269 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/builtin_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19129 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24391 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4401 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5315 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3433 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5232 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3876 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5670 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4431 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5536 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4186 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6247 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9148 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13299 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4397 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5674 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4222 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6343 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7303 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11148 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.322067 gns3-gui-3.0.0a3/gns3/modules/builtin/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1212 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/builtin/utils/tree_widget_item.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.322067 gns3-gui-3.0.0a3/gns3/modules/docker/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4407 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.322067 gns3-gui-3.0.0a3/gns3/modules/docker/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5356 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/dialogs/docker_vm_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5190 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/docker_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.322067 gns3-gui-3.0.0a3/gns3/modules/docker/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1968 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/pages/docker_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9347 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/pages/docker_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12245 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/pages/docker_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1385 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.330067 gns3-gui-3.0.0a3/gns3/modules/docker/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2400 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2852 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12930 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17480 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4709 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11020 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16543 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.330067 gns3-gui-3.0.0a3/gns3/modules/dynamips/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7828 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2360 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/adapters.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.330067 gns3-gui-3.0.0a3/gns3/modules/dynamips/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17596 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/dialogs/ios_router_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.334067 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1759 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c1700.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2320 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c2600.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c2691.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-12-24 09:42:12.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c3600.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c3725.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c3745.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c7200.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2218 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/etherswitch_router.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12172 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/router.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.334067 gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/dynamips_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27874 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/ios_router_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22457 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/ios_router_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7767 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.338067 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     6439 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/dynamips_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8491 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    35772 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    45950 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4850 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5957 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15247 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.342067 gns3-gui-3.0.0a3/gns3/modules/dynamips/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/utils/decompress_ios.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2179 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/utils/decompress_ios_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/dynamips/wics.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.342067 gns3-gui-3.0.0a3/gns3/modules/iou/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3974 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.342067 gns3-gui-3.0.0a3/gns3/modules/iou/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/iou/dialogs/iou_device_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4932 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/iou/iou_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.342067 gns3-gui-3.0.0a3/gns3/modules/iou/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13513 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/iou/pages/iou_device_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15081 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/iou/pages/iou_device_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5027 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/pages/iou_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1305 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/iou/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.346067 gns3-gui-3.0.0a3/gns3/modules/iou/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    13890 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17361 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4638 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5659 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6717 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2927 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3557 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/module.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1066 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/module_error.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.346067 gns3-gui-3.0.0a3/gns3/modules/qemu/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5394 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.346067 gns3-gui-3.0.0a3/gns3/modules/qemu/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8042 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/dialogs/qemu_image_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4726 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/dialogs/qemu_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.346067 gns3-gui-3.0.0a3/gns3/modules/qemu/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2896 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/pages/qemu_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30339 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/pages/qemu_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15055 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/pages/qemu_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7486 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/qemu_vm.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2017 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.358067 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23636 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_image_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29391 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_image_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2888 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3655 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    32090 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    42819 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4602 2021-10-08 05:49:21.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5444 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12608 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18585 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.358067 gns3-gui-3.0.0a3/gns3/modules/virtualbox/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5807 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.362067 gns3-gui-3.0.0a3/gns3/modules/virtualbox/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3607 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.362067 gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4001 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11547 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10014 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1438 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.366067 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3684 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4480 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    10804 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4373 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3801 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5833 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4955 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/modules/virtualbox/virtualbox_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.366067 gns3-gui-3.0.0a3/gns3/modules/vmware/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10348 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.366067 gns3-gui-3.0.0a3/gns3/modules/vmware/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3531 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/dialogs/vmware_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.366067 gns3-gui-3.0.0a3/gns3/modules/vmware/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/pages/vmware_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11191 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/pages/vmware_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10365 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/pages/vmware_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1731 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.370067 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7503 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8865 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9806 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13005 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4329 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5270 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3802 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5702 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6183 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vmware/vmware_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.370067 gns3-gui-3.0.0a3/gns3/modules/vpcs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4669 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.370067 gns3-gui-3.0.0a3/gns3/modules/vpcs/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.370067 gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7092 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9184 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/vpcs_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1064 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.374067 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4135 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6719 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4278 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4868 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3424 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5202 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3653 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4263 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2022-07-11 22:23:49.000000 gns3-gui-3.0.0a3/gns3/modules/vpcs/vpcs_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1630 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/network_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29180 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/nodes_dock_widget.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9340 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/nodes_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10620 2022-10-19 11:38:43.000000 gns3-gui-3.0.0a3/gns3/packet_capture.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.374067 gns3-gui-3.0.0a3/gns3/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14166 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/pages/controller_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21133 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/pages/general_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/pages/gns3_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/pages/packet_capture_preferences_page.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.378067 gns3-gui-3.0.0a3/gns3/ports/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ports/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ports/ethernet_port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8108 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ports/port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2335 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ports/port_name_factory.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      887 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ports/serial_port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10489 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/progress.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25052 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/project.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/pycutext.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.378067 gns3-gui-3.0.0a3/gns3/qt/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7943 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/qt/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/qt/qimage_svg_renderer.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.378067 gns3-gui-3.0.0a3/gns3/registry/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/registry/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7028 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/registry/appliance.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9250 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/registry/appliance_to_template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2646 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/registry/config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4251 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/registry/image.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4698 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/registry/registry.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.378067 gns3-gui-3.0.0a3/gns3/schemas/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15212 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/schemas/appliance.json
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18383 2022-12-27 05:26:03.000000 gns3-gui-3.0.0a3/gns3/settings.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2148 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/spice_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.378067 gns3-gui-3.0.0a3/gns3/static/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/static/.keep
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2732 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/status_bar.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/style.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/symbol.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3815 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/telnet_console.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8435 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/template_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20587 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/topology.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14489 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/topology_summary_view.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.418068 gns3-gui-3.0.0a3/gns3/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    96556 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/about_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   112145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/about_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9192 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/appliance_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11305 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/appliance_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3516 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/capture_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4471 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/capture_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3197 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/configuration_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/configuration_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/console_command_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/console_command_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    18928 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/controller_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23470 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/controller_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2012 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/custom_adapters_configuration_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2258 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/custom_adapters_configuration_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3252 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/doctor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3521 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/doctor_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5487 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/edit_compute_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6478 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/edit_compute_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9096 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/edit_project_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11089 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/edit_project_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     1694 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/exec_command_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/exec_command_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3559 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/export_debug_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3716 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/export_debug_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5607 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/export_project_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8170 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/export_project_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3422 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/file_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/file_editor_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3881 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/filter_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3708 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/filter_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    42307 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/general_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53669 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/general_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7845 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/gns3_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10781 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/gns3_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1824 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/idlepc_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1919 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/idlepc_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3693 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/image_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3823 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/image_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2758 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/login_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2734 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/login_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    41586 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/main_window.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    50821 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/main_window_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3059 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/new_template_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4766 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/new_template_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2636 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/node_info_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/node_info_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/node_properties_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5071 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/node_properties_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4366 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/packet_capture_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/packet_capture_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4704 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/preferences_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/preferences_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4950 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/profile_select_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/profile_select_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/project_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11436 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/project_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2754 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/project_welcome_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/project_welcome_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)  9439247 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/resources_rc.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7770 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/setup_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11373 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/setup_wizard_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     2778 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/show_readme_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2882 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/ui/show_readme_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2357 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/snapshots_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2588 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/snapshots_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4807 2021-06-12 04:52:20.000000 gns3-gui-3.0.0a3/gns3/ui/style_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6125 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/style_editor_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/symbol_selection_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5838 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/symbol_selection_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4884 2020-11-07 04:27:16.000000 gns3-gui-3.0.0a3/gns3/ui/text_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/ui/text_editor_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11357 2022-11-09 12:07:45.000000 gns3-gui-3.0.0a3/gns3/update_manager.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.426068 gns3-gui-3.0.0a3/gns3/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3691 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5724 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/analytics.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2799 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/bring_to_front.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/file_copy_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1326 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/get_icon.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2239 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/get_resource.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/gns3/utils/import_project_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/interfaces.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1256 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/normalize_filename.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5435 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/process_files_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/progress_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/run_in_terminal.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2524 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/server_select.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4424 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/sudo.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2420 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/wait_for_command_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2713 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/wait_for_connection_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2288 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/wait_for_lambda_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2850 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/utils/wait_for_runas_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1490 2022-12-27 07:22:10.000000 gns3-gui-3.0.0a3/gns3/version.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2072 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/gns3/vnc_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.430068 gns3-gui-3.0.0a3/gns3_gui.egg-info/
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2916 2022-12-27 07:36:33.000000 gns3-gui-3.0.0a3/gns3_gui.egg-info/PKG-INFO
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    29963 2022-12-27 07:36:33.000000 gns3-gui-3.0.0a3/gns3_gui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        1 2022-12-27 07:36:33.000000 gns3-gui-3.0.0a3/gns3_gui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       36 2022-12-27 07:36:33.000000 gns3-gui-3.0.0a3/gns3_gui.egg-info/entry_points.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       97 2022-12-27 07:36:33.000000 gns3-gui-3.0.0a3/gns3_gui.egg-info/requires.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        5 2022-12-27 07:36:33.000000 gns3-gui-3.0.0a3/gns3_gui.egg-info/top_level.txt
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       97 2022-12-27 05:26:26.000000 gns3-gui-3.0.0a3/requirements.txt
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.430068 gns3-gui-3.0.0a3/resources/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.510069 gns3-gui-3.0.0a3/resources/charcoal_icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6231 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/add-link-1-cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/add-link-1-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/add-link-1.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/add-note-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/aux-console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/browse-all-icons-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/browse-all-icons.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13891 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/calculate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2220 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2127 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/capture-start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/capture-stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3362 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/command_line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/configuration-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8406 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/console_edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4172 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/delete-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4156 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2881 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/duplicate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3852 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3846 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/export-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2822 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/filter-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/filter-reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25640 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24989 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/firewall-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/front-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12619 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/help-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12581 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/image-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/import-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/import_export_configs-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2409 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/inspect-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4013 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/link-pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3593 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/link-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3738 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/lock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3730 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3546 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/lower_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/minus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/new-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4223 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/node_conception-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/open-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/pc-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/pc.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2680 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/plus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2673 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6090 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/preferences-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6084 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/preferences.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5543 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/quit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5870 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/raise_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3542 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/reload-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2181 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2175 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/router-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5279 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/save-as-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5281 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/save-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/save-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/show-hostname-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/show-interface-names-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/snapshot-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2684 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/switch-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/unlock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-in-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-in.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2808 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-out-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1746 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-out.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.562069 gns3-gui-3.0.0a3/resources/classic_icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5935 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/add-link-cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2971 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/add-link-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3086 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/add-link.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4148 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/add-note-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2593 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/aux-console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2589 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/browse-all-icons-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5646 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/browse-all-icons.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13890 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/calculate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2992 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2914 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/capture-start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3368 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/capture-stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3363 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/command_line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6254 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/configuration-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2046 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2070 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/console_edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4162 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/delete-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/duplicate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3856 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4312 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4321 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/export-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24995 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/filter-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/filter-reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25639 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24990 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2047 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/firewall-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2056 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/front-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9629 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/help-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9625 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2011 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/image-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2020 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/import-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2351 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/import_export_configs-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2373 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/inspect-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2382 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4003 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/classic_icons/link-pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3593 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/classic_icons/link-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/lock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3731 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3545 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/lower_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/minus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4249 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/new-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4245 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/node_conception-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2243 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/open-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2166 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/pc-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3493 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/pc.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2679 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/plus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2674 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5725 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/preferences-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5719 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/preferences.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5032 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/quit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5026 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/raise_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3541 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2530 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2539 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2266 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/reload-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2275 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2180 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2174 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2313 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/router-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2322 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4710 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/save-as-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4748 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3383 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/save-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3417 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/save-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/show-hostname-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3636 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/show-interface-names-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3686 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2876 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/snapshot-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2901 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1742 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2495 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/switch-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/unlock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2761 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/zoom-in-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2785 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/zoom-in.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2719 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/zoom-out-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2727 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/classic_icons/zoom-out.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.718071 gns3-gui-3.0.0a3/resources/icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    63187 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/PC-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    60045 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/PC.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    28134 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16099 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/applications.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21937 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   291074 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/browse-all-icons-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   297712 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/browse-all-icons.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32570 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39042 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    37642 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25560 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/cancel-connection.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18737 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31090 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26448 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19139 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23701 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/connection-new-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23702 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/connection-new.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21216 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13772 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/dialog-warning.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26729 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/drawing.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23490 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16831 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24733 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21372 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10572 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21681 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/filter-capture.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23917 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    57273 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/firewall-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53702 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/firewall.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13259 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7175 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/horizontally.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19675 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10549 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39319 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15756 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/led_gray.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10135 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/led_green.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6952 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/led_red.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9965 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/led_yellow.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32132 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6518 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4612 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24126 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16626 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/new.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27187 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30745 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23462 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21534 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19130 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7903 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35282 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31055 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16810 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8571 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    58719 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/router-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54133 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/router.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/rtv.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    40599 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31854 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/save-as.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29835 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/save.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15166 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26306 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18013 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17454 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    67991 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/switch-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    64865 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/switch.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    34969 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5816 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/vertically.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/virtualbox.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/warning.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1906 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/wireshark.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5939 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/zoom-in-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/zoom-in.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/zoom-out-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6157 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/icons/zoom-out.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.730071 gns3-gui-3.0.0a3/resources/images/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   370070 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/images/gns3.ico
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7892 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/images/gns3_icon_128x128.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16745 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/images/gns3_icon_256x256.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7921 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/images/gns3_logo.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.730071 gns3-gui-3.0.0a3/resources/linux/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.734071 gns3-gui-3.0.0a3/resources/linux/applications/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      282 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/applications/gns3.desktop
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/gns3-gui.xml
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/resources/linux/icons/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/16x16/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.742071 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/16x16/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      832 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/16x16/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/32x32/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.742071 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/32x32/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/32x32/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.766071 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.770072 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6075 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4500 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.770072 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/apps/gns3.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.798072 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11492 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16025 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/resources.qrc
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.798072 gns3-gui-3.0.0a3/resources/styles/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1231 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/resources/styles/charcoal.css
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.802072 gns3-gui-3.0.0a3/resources/symbols/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16298 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/atm_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    78565 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/cloud.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/computer.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19782 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/docker_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18650 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/ethernet_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18401 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18343 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/frame_relay_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18128 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/hub.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19150 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/multilayer_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18421 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/qemu_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18494 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16401 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/vbox_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16843 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/vmware_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/resources/symbols/vpcs_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       38 2022-12-27 07:36:33.830072 gns3-gui-3.0.0a3/setup.cfg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4517 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/setup.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.818072 gns3-gui-3.0.0a3/tests/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6260 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/conftest.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.818072 gns3-gui-3.0.0a3/tests/items/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1997 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/items/test_ellipse_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1509 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/items/test_image_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/items/test_label_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/items/test_line_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3046 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/items/test_rectangle_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/items/test_text_item.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.250066 gns3-gui-3.0.0a3/tests/modules/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/modules/docker/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1478 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/modules/docker/test_docker_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/modules/dynamips/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1486 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/modules/dynamips/test_dynamips_init.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/modules/iou/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1841 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/modules/iou/test_iou_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/modules/qemu/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1526 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/modules/qemu/test_qemu_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/modules/virtualbox/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/modules/virtualbox/test_virtualbox_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/modules/vpcs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/modules/vpcs/test_vpcs_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/qt/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/qt/test_qimage_svg_renderer.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.822072 gns3-gui-3.0.0a3/tests/registry/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.830072 gns3-gui-3.0.0a3/tests/registry/appliances/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2395 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/arista-veos.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1356 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/broken-microcore-linux.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1298 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/cisco-3745.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      961 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/cisco-iou-l3.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1620 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/juniper-vsrx.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2025 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/microcore-linux.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/appliances/openvswitch.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/test_appliance.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10538 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/registry/test_appliance_to_template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2895 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/registry/test_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2304 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/test_image.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2185 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/registry/test_registry.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1376 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_compute.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5810 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_compute_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1717 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_controller.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_graphics_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8696 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_http_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3087 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_image_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1596 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_image_upload_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4739 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13656 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_local_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2957 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_local_server.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1760 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_main_window.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_network_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5698 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_progress.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5498 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_project.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_spice_console.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_topology.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3575 2022-12-27 05:25:52.000000 gns3-gui-3.0.0a3/tests/test_update_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_utils.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1814 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/test_vnc_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2022-12-27 07:36:33.830072 gns3-gui-3.0.0a3/tests/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1394 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/utils/test_file_copy_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3705 2022-07-11 22:23:48.000000 gns3-gui-3.0.0a3/tests/utils/test_server_select.py
```

### Comparing `gns3-gui-3.0.0a2/COPYING` & `gns3-gui-3.0.0a3/COPYING`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/LICENSE` & `gns3-gui-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/PKG-INFO` & `gns3-gui-3.0.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3-gui
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: GNS3 graphical interface for the GNS3 server.
 Home-page: http://github.com/GNS3/gns3-gui
 Author: Jeremy Grossmann
 Author-email: package-maintainer@gns3.net
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.4
 License-File: LICENSE
 License-File: COPYING
 License-File: AUTHORS
 
 # GNS3-gui
@@ -70,9 +71,7 @@
 https://github.com/Kozea/wdb
 
 ## Security issues
 
 Please contact us at security@gns3.net
 
 
-
-
```

### Comparing `gns3-gui-3.0.0a2/README.md` & `gns3-gui-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/__main__.py` & `gns3-gui-3.0.0a3/gns3/__main__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/appliance_manager.py` & `gns3-gui-3.0.0a3/gns3/appliance_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from .qt import QtCore
 from .controller import Controller
 from .local_config import LocalConfig
 from .settings import GENERAL_SETTINGS
+from .http_client_error import HttpClientError
 
 
 import logging
 log = logging.getLogger(__name__)
 
 
 class ApplianceManager(QtCore.QObject):
@@ -45,20 +46,25 @@
         Gets the appliances from the controller.
         """
 
         if self._controller.connected():
             settings = LocalConfig.instance().loadSectionSettings("MainWindow", GENERAL_SETTINGS)
             symbol_theme = settings["symbol_theme"]
             if update is True:
-                self._controller.get(
-                    "/appliances?update=yes&symbol_theme={}".format(symbol_theme),
-                    self._listAppliancesCallback,
-                    progress_text="Downloading appliances from online registry...",
-                    wait=True
-                )
+                try:
+                    self._controller.get(
+                        "/appliances?update=yes&symbol_theme={}".format(symbol_theme),
+                        self._listAppliancesCallback,
+                        progress_text="Downloading appliances from online registry...",
+                        wait=True,
+                        timeout=300
+                    )
+                except HttpClientError as e:
+                    log.error(f"Error while getting appliances list: {e}")
+                    return
             else:
                 self._controller.get("/appliances?symbol_theme={}".format(symbol_theme), self._listAppliancesCallback)
 
     def _controllerDisconnectedSlot(self):
         """
         Called when the controller has been disconnected.
         """
```

### Comparing `gns3-gui-3.0.0a2/gns3/application.py` & `gns3-gui-3.0.0a3/gns3/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import sys
 
 from .qt import QtWidgets, QtGui, QtCore
 from gns3.utils import parse_version
+from gns3.local_config import LocalConfig
 from .version import __version__
 
 import logging
 log = logging.getLogger(__name__)
 
 
 class Application(QtWidgets.QApplication):
@@ -33,15 +34,17 @@
 
         self.setStyle(QtWidgets.QStyleFactory.create("Fusion"))
         # both Qt and PyQt must be version >= 5.6 in order to enable high DPI scaling
         if parse_version(QtCore.QT_VERSION_STR) >= parse_version("5.6") and parse_version(QtCore.PYQT_VERSION_STR) >= parse_version("5.6"):
             # only available starting Qt version 5.6
             if hdpi:
                 if sys.platform.startswith("linux"):
-                    log.warning("HDPI mode is enabled. HDPI support on Linux is not fully stable and GNS3 may crash depending of your version of Linux. To disabled HDPI mode please edit ~/.config/GNS3/gns3_gui.conf and set 'hdpi' to 'false'")
+                    local_config_path = LocalConfig.instance().configFilePath()
+                    log.warning("HDPI mode is enabled. HDPI support on Linux is not fully stable and GNS3 may crash depending of your version of Linux. "
+                                f"To disabled HDPI mode please edit '{local_config_path}' and set 'hdpi' to 'false'")
                 self.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling)
                 self.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps)
             else:
                 log.info("HDPI mode is disabled")
                 self.setAttribute(QtCore.Qt.AA_DisableHighDpiScaling)
 
         super().__init__(argv)
```

### Comparing `gns3-gui-3.0.0a2/gns3/base_node.py` & `gns3-gui-3.0.0a3/gns3/base_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/compute.py` & `gns3-gui-3.0.0a3/gns3/compute.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/compute_manager.py` & `gns3-gui-3.0.0a3/gns3/compute_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/compute_summary_view.py` & `gns3-gui-3.0.0a3/gns3/compute_summary_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/console_cmd.py` & `gns3-gui-3.0.0a3/gns3/console_cmd.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/console_view.py` & `gns3-gui-3.0.0a3/gns3/console_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/controller.py` & `gns3-gui-3.0.0a3/gns3/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     def __init__(self):
 
         super().__init__()
         self._connected = False
         self._connecting = False
         self._notification_stream = None
         self._version = None
-        self._http_client = None
         self._cache_directory = tempfile.TemporaryDirectory(suffix="-gns3")
         self._http_client = None
         self._first_error = True
         self._error_dialog = None
         self._display_error = True
         self._projects = []
         self._images = []
```

### Comparing `gns3-gui-3.0.0a2/gns3/crash_report.py` & `gns3-gui-3.0.0a3/gns3/crash_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 class CrashReport:
 
     """
     Report crash to a third party service
     """
 
-    DSN = "https://d551ae4af1324d79bdbb21c7362a4833@o19455.ingest.sentry.io/38506"
+    DSN = "https://e53718a5b9234e56a2fd3634e6fa07c9@o19455.ingest.sentry.io/38506"
     _instance = None
 
     def __init__(self):
         # We don't want sentry making noise if an error is caught when we don't have internet
         sentry_errors = logging.getLogger('sentry.errors')
         sentry_errors.disabled = True
 
@@ -82,15 +82,15 @@
                             integrations=[sentry_logging])
 
             tags = {
                 "os:name": platform.system(),
                 "os:release": platform.release(),
                 "os:win_32": " ".join(platform.win32_ver()),
                 "os:mac": "{} {}".format(platform.mac_ver()[0], platform.mac_ver()[2]),
-                "os:linux": " ".join(distro.linux_distribution()),
+                "os:linux": distro.name(pretty=True),
 
             }
 
             self._add_qt_information(tags)
 
             with sentry_sdk.configure_scope() as scope:
                 for key, value in tags.items():
```

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/about_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/about_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/appliance_wizard.py` & `gns3-gui-3.0.0a3/gns3/dialogs/appliance_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/capture_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/capture_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/configuration_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/configuration_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/console_command_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/console_command_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/custom_adapters_configuration_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/custom_adapters_configuration_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/doctor_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/doctor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/edit_compute_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/edit_compute_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/edit_project_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/edit_project_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         self.uiNewVarButton.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         self.uiNewVarButton.clicked.connect(self.onAddNewVariable)
         self.uiGlobalVariablesGrid.addWidget(self.uiNewVarButton, 0, 3, QtCore.Qt.AlignRight)
 
         self._readme_filename = "README.txt"
         self.uiTabWidget.currentChanged.connect(self._previewMarkdownSlot)
         self._loadReadme()
-
-        self._variables = self.setUpVariables()
+        self._variables = self._project.variables()
+        if not self._variables:
+            self._variables = [{"name": "", "value": ""}]
         self.updateGlobalVariables()
 
     def _loadReadme(self):
 
         self._project.get("/files/{}".format(self._readme_filename), self._loadedReadme, raw=True)
 
     def _loadedReadme(self, result, error=False, context={}, **kwargs):
@@ -76,24 +77,14 @@
                 return
 
             # show Markdown preview
             document = QtGui.QTextDocument()
             self.uiReadmePreview.setDocument(document)
             document.setMarkdown(self.uiReadmeTextEdit.toPlainText())
 
-    def setUpVariables(self):
-        new_variable = {"name": "", "value": ""}
-        variables = self._project.variables()
-
-        if variables is not None:
-            variables.append(new_variable)
-        else:
-            variables = [new_variable]
-        return variables
-
     def updateGlobalVariables(self):
         while True:
             item = self.uiGlobalVariablesGrid.takeAt(1)
             if item is None:
                 break
             elif item.widget():
                 item.widget().deleteLater()
```

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/exec_command_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/exec_command_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/export_debug_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/export_debug_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/file_editor_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/file_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/filter_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/filter_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/idlepc_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/idlepc_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/image_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/image_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/login_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/login_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/new_template_wizard.py` & `gns3-gui-3.0.0a3/gns3/dialogs/new_template_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/node_info_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/node_info_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/node_properties_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/node_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/notif_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/notif_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/preferences_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/profile_select.py` & `gns3-gui-3.0.0a3/gns3/dialogs/profile_select.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/project_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/project_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/project_export_wizard.py` & `gns3-gui-3.0.0a3/gns3/dialogs/project_export_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/project_welcome_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/project_welcome_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/setup_wizard.py` & `gns3-gui-3.0.0a3/gns3/dialogs/setup_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/show_readme_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/show_readme_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/snapshots_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/snapshots_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/style_editor_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/style_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/style_editor_dialog_link.py` & `gns3-gui-3.0.0a3/gns3/dialogs/style_editor_dialog_link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/symbol_selection_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/symbol_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/text_editor_dialog.py` & `gns3-gui-3.0.0a3/gns3/dialogs/text_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/vm_with_images_wizard.py` & `gns3-gui-3.0.0a3/gns3/dialogs/vm_with_images_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/dialogs/vm_wizard.py` & `gns3-gui-3.0.0a3/gns3/dialogs/vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/graphics_view.py` & `gns3-gui-3.0.0a3/gns3/graphics_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/http_client.py` & `gns3-gui-3.0.0a3/gns3/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         super().__init__()
         from gns3.main_window import MainWindow
         self._main_window = MainWindow.instance()
 
         self._protocol = settings.get("protocol", "http")
         self._host = settings["host"]
         self._prefix = prefix
+        self._auth_attempted = False
         self._jwt_token = None
         try:
             if self._host is None or self._host == "0.0.0.0":
                 self._host = "127.0.0.1"
             elif ":" in self._host and ipaddress.IPv6Address(self._host) and str(ipaddress.IPv6Address(self._host)) == "::":
                 self._host = "::1"
         except ipaddress.AddressValueError:
@@ -497,43 +498,55 @@
         Disconnect from the server
         """
 
         if self.connected():
             self.disconnected_signal.emit()
             self.close()
 
+    def _requestCredentialsFromUser(self):
+        """
+        Request credentials from user
+
+        :return: username, password
+        """
+
+        username = password = None
+        login_dialog = LoginDialog(self._main_window)
+        if self._username:
+            login_dialog.setUsername(self._username)
+        login_dialog.show()
+        login_dialog.raise_()
+        if login_dialog.exec_():
+            username = login_dialog.getUsername()
+            password = login_dialog.getPassword()
+        return username, password
+
     def _handleUnauthorizedRequest(self, reply: QtNetwork.QNetworkReply) -> None:
         """
         Request the username / password to authenticate with the server
         """
 
-        if not self._username or not self._password:
-            username = password = None
-            login_dialog = LoginDialog(self._main_window)
-            if self._username:
-                login_dialog.setUsername(self._username)
-            login_dialog.show()
-            login_dialog.raise_()
-            if login_dialog.exec_():
-                username = login_dialog.getUsername()
-                password = login_dialog.getPassword()
+        if not self._username or not self._password or self._auth_attempted is True:
+            username, password = self._requestCredentialsFromUser()
         else:
             username = self._username
             password = self._password
 
         if username and password:
             body = {
                 "username": username,
                 "password": password
             }
+            self._auth_attempted = True
             content = self._executeHTTPQuery("POST", "/users/authenticate", body=body, wait=True)
             if content:
                 log.info(f"Authenticated with controller {self._host} on port {self._port}")
                 token = content.get("access_token")
                 if token:
+                    self._auth_attempted = False
                     self._jwt_token = token
                     return
         else:
             raise HttpClientUnauthorizedError(f"{reply.errorString()}")
 
     def _validateServerVersion(self, content: dict) -> None:
         """
@@ -542,15 +555,15 @@
 
         version = content.get("version")
         local = content.get("local")
 
         if version is None or local is None:
             raise HttpClientBadRequestError(f"The server is not a GNS3 server: {content}")
 
-        if version.split("-")[0] != __version__.split("-")[0]:
+        if version.split("+")[0] != __version__.split("+")[0]:
             msg = f"Client version {__version__} is not the same as server version {version}"
             # We don't allow different major version to interact even with dev build
             if __version_info__[3] == 0 or parse_version(__version__)[:2] != parse_version(version)[:2]:
                 raise HttpClientError(msg)
             log.warning(f"{msg}\nUsing different versions may result in unexpected problems.\n"
                         "Please upgrade or use at your own risk.")
```

### Comparing `gns3-gui-3.0.0a2/gns3/http_client_error.py` & `gns3-gui-3.0.0a3/gns3/http_client_error.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/image_manager.py` & `gns3-gui-3.0.0a3/gns3/image_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/image_upload_manager.py` & `gns3-gui-3.0.0a3/gns3/image_upload_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     def _fileUploadToController(self) -> bool:
 
         log.debug("Uploading image '{}' to controller".format(self._image.path))
         try:
             self._controller.post(
                 f"/images/upload/{self._image.filename}",
                 callback=None,
-                params={"allow_raw_image": True},
                 body=pathlib.Path(self._image.path),
                 context={"image_path": self._image.path},
                 progress_text="Uploading {}".format(self._image.filename),
                 timeout=None,
                 wait=True
             )
         except HttpClientCancelledRequestError:
```

### Comparing `gns3-gui-3.0.0a2/gns3/items/drawing_item.py` & `gns3-gui-3.0.0a3/gns3/items/drawing_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/ellipse_item.py` & `gns3-gui-3.0.0a3/gns3/items/ellipse_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/ethernet_link_item.py` & `gns3-gui-3.0.0a3/gns3/items/ethernet_link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/image_item.py` & `gns3-gui-3.0.0a3/gns3/items/image_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/label_item.py` & `gns3-gui-3.0.0a3/gns3/items/label_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/line_item.py` & `gns3-gui-3.0.0a3/gns3/items/line_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/link_item.py` & `gns3-gui-3.0.0a3/gns3/items/link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/logo_item.py` & `gns3-gui-3.0.0a3/gns3/items/logo_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/node_item.py` & `gns3-gui-3.0.0a3/gns3/items/node_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/rectangle_item.py` & `gns3-gui-3.0.0a3/gns3/items/rectangle_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/serial_link_item.py` & `gns3-gui-3.0.0a3/gns3/items/serial_link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/shape_item.py` & `gns3-gui-3.0.0a3/gns3/items/shape_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/text_item.py` & `gns3-gui-3.0.0a3/gns3/items/text_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/items/utils.py` & `gns3-gui-3.0.0a3/gns3/items/utils.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/link.py` & `gns3-gui-3.0.0a3/gns3/link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/local_config.py` & `gns3-gui-3.0.0a3/gns3/local_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/local_server.py` & `gns3-gui-3.0.0a3/gns3/local_server.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/logger.py` & `gns3-gui-3.0.0a3/gns3/logger.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/main.py` & `gns3-gui-3.0.0a3/gns3/main.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/main_window.py` & `gns3-gui-3.0.0a3/gns3/main_window.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/atm_switch.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/atm_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/cloud.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/cloud.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/cloud_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/cloud_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ethernet_hub.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ethernet_hub.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ethernet_switch.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ethernet_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/frame_relay_switch.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/frame_relay_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/nat.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/nat.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/atm_switch_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/atm_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/builtin_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/builtin_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/cloud_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/cloud_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/cloud_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/cloud_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,30 +123,32 @@
 
         port = self.uiPortSpinBox.value()
         vlan = self.uiVlanSpinBox.value()
         port_type = self.uiPortTypeComboBox.currentText()
         if port_type == "qinq":
             port_ethertype = self.uiPortEtherTypeComboBox.currentText()
         else:
-            port_ethertype = ""
+            port_ethertype = None
 
         if port in self._ports:
             # update a given entry in the tree widget
             item = self.uiPortsTreeWidget.findItems(str(port), QtCore.Qt.MatchFixedString)[0]
             item.setText(1, str(vlan))
             item.setText(2, port_type)
-            item.setText(3, port_ethertype)
+            if port_ethertype:
+                item.setText(3, port_ethertype)
 
         else:
             # add a new entry in the tree widget
             item = TreeWidgetItem(self.uiPortsTreeWidget)
             item.setText(0, str(port))
             item.setText(1, str(vlan))
             item.setText(2, port_type)
-            item.setText(3, port_ethertype)
+            if port_ethertype:
+                item.setText(3, port_ethertype)
             self.uiPortsTreeWidget.addTopLevelItem(item)
 
         self._ports[port] = {"name": "Ethernet{}".format(port),
                              "port_number": port,
                              "type": port_type,
                              "vlan": vlan,
                              "ethertype": port_ethertype}
@@ -220,15 +222,17 @@
             self.uiCategoryComboBox.hide()
 
         for port_info in settings["ports_mapping"]:
             item = TreeWidgetItem(self.uiPortsTreeWidget)
             item.setText(0, str(port_info["port_number"]))
             item.setText(1, str(port_info.get("vlan", 1)))
             item.setText(2, port_info.get("type", "access"))
-            item.setText(3, port_info.get("ethertype", ""))
+            port_ethertype = port_info.get("ethertype")
+            if port_ethertype:
+                item.setText(3, port_ethertype)
             self.uiPortsTreeWidget.addTopLevelItem(item)
             self._ports[port_info["port_number"]] = port_info
 
         # load the console type
         index = self.uiConsoleTypeComboBox.findText(settings["console_type"])
         if index != -1:
             self.uiConsoleTypeComboBox.setCurrentIndex(index)
```

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/atm_switch_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/atm_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/builtin_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/builtin_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/builtin_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/builtin_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/cloud_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/cloud_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/builtin/utils/tree_widget_item.py` & `gns3-gui-3.0.0a3/gns3/modules/builtin/utils/tree_widget_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/dialogs/docker_vm_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/dialogs/docker_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/docker_vm.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/docker_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/pages/docker_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/pages/docker_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/pages/docker_vm_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/pages/docker_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/pages/docker_vm_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/pages/docker_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/docker/ui/docker_vm_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/docker/ui/docker_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/adapters.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/adapters.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/dialogs/ios_router_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/dialogs/ios_router_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c1700.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c1700.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c2600.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c2600.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c2691.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c2691.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c3600.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c3600.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c3725.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c3725.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c3745.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c3745.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/c7200.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/c7200.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/etherswitch_router.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/etherswitch_router.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/nodes/router.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/nodes/router.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/dynamips_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/dynamips_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/ios_router_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/ios_router_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/pages/ios_router_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/pages/ios_router_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/dynamips_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/dynamips_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/ui/ios_router_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/ui/ios_router_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/utils/decompress_ios.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/utils/decompress_ios.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/utils/decompress_ios_worker.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/utils/decompress_ios_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/dynamips/wics.py` & `gns3-gui-3.0.0a3/gns3/modules/dynamips/wics.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/dialogs/iou_device_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/dialogs/iou_device_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/iou_device.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/iou_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/pages/iou_device_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/pages/iou_device_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/pages/iou_device_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/pages/iou_device_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/pages/iou_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/pages/iou_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_device_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_device_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/iou/ui/iou_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/iou/ui/iou_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/module.py` & `gns3-gui-3.0.0a3/gns3/modules/module.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/module_error.py` & `gns3-gui-3.0.0a3/gns3/modules/module_error.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/dialogs/qemu_image_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/dialogs/qemu_image_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/dialogs/qemu_vm_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/dialogs/qemu_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/pages/qemu_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/pages/qemu_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/pages/qemu_vm_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/pages/qemu_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/pages/qemu_vm_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/pages/qemu_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/qemu_vm.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/qemu_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_image_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_image_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_image_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_image_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/virtualbox/virtualbox_vm.py` & `gns3-gui-3.0.0a3/gns3/modules/virtualbox/virtualbox_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/dialogs/vmware_vm_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/dialogs/vmware_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/pages/vmware_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/pages/vmware_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/pages/vmware_vm_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/pages/vmware_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/pages/vmware_vm_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/pages/vmware_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vmware/vmware_vm.py` & `gns3-gui-3.0.0a3/gns3/modules/vmware/vmware_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/__init__.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/pages/vpcs_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/pages/vpcs_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/settings.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_wizard.ui` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/modules/vpcs/vpcs_node.py` & `gns3-gui-3.0.0a3/gns3/modules/vpcs/vpcs_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/network_client.py` & `gns3-gui-3.0.0a3/gns3/network_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/node.py` & `gns3-gui-3.0.0a3/gns3/node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/nodes_dock_widget.py` & `gns3-gui-3.0.0a3/gns3/nodes_dock_widget.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/nodes_view.py` & `gns3-gui-3.0.0a3/gns3/nodes_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/packet_capture.py` & `gns3-gui-3.0.0a3/gns3/packet_capture.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/pages/controller_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/pages/controller_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/pages/general_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/pages/general_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/pages/gns3_vm_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/pages/gns3_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/pages/packet_capture_preferences_page.py` & `gns3-gui-3.0.0a3/gns3/pages/packet_capture_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ports/ethernet_port.py` & `gns3-gui-3.0.0a3/gns3/ports/ethernet_port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ports/port.py` & `gns3-gui-3.0.0a3/gns3/ports/port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ports/port_name_factory.py` & `gns3-gui-3.0.0a3/gns3/ports/port_name_factory.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ports/serial_port.py` & `gns3-gui-3.0.0a3/gns3/ports/serial_port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/progress.py` & `gns3-gui-3.0.0a3/gns3/progress.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/project.py` & `gns3-gui-3.0.0a3/gns3/project.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/pycutext.py` & `gns3-gui-3.0.0a3/gns3/pycutext.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/qt/__init__.py` & `gns3-gui-3.0.0a3/gns3/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/qt/qimage_svg_renderer.py` & `gns3-gui-3.0.0a3/gns3/qt/qimage_svg_renderer.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/registry/appliance.py` & `gns3-gui-3.0.0a3/gns3/registry/appliance.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/registry/appliance_to_template.py` & `gns3-gui-3.0.0a3/gns3/registry/appliance_to_template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/registry/config.py` & `gns3-gui-3.0.0a3/gns3/registry/config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/registry/image.py` & `gns3-gui-3.0.0a3/gns3/registry/image.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/registry/registry.py` & `gns3-gui-3.0.0a3/gns3/registry/registry.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/schemas/appliance.json` & `gns3-gui-3.0.0a3/gns3/schemas/appliance.json`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/settings.py` & `gns3-gui-3.0.0a3/gns3/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         program_files = os.environ["PROGRAMFILES"]
         program_files_x86 = os.environ["PROGRAMFILES(X86)"]
     else:
         # windows 32-bit
         program_files_x86 = program_files = os.environ["PROGRAMFILES"]
 
     PRECONFIGURED_TELNET_CONSOLE_COMMANDS = {'Putty (normal standalone version)': 'putty_standalone.exe -telnet %h %p -loghost "%d"',
-                                             'Putty (custom deprecated version)': 'putty.exe -telnet %h %p -wt "%d" -gns3 5 -skin 4',
                                              'MobaXterm': r'"{}\Mobatek\MobaXterm Personal Edition\MobaXterm.exe" -newtab "telnet %h %p"'.format(program_files_x86),
                                              'Royal TS V3': r'{}\code4ward.net\Royal TS V3\RTS3App.exe /connectadhoc:%h /adhoctype:terminal /p:IsTelnetConnection="true" /p:ConnectionType="telnet;Telnet Connection" /p:Port="%p" /p:Name="%d"'.format(program_files),
                                              'Royal TS V5': r'"{}\Royal TS V5\RoyalTS.exe" /protocol:terminal /using:adhoc /uri:"%h" /property:Port="%p" /property:IsTelnetConnection="true" /property:Name="%d"'.format(program_files_x86),
                                              'SuperPutty': r'SuperPutty.exe -telnet "%h -P %p -wt \"%d\""',
                                              'SecureCRT': r'"{}\VanDyke Software\SecureCRT\SecureCRT.exe" /N "%d" /T /TELNET %h %p'.format(program_files),
                                              'SecureCRT (personal profile)': r'"{}\AppData\Local\VanDyke Software\SecureCRT\SecureCRT.exe" /T /N "%d" /TELNET %h %p'.format(userprofile),
                                              'TeraTerm Pro': r'"{}\teraterm\ttermpro.exe" /W="%d" /M="ttstart.macro" /T=1 %h %p'.format(program_files_x86),
```

### Comparing `gns3-gui-3.0.0a2/gns3/spice_console.py` & `gns3-gui-3.0.0a3/gns3/spice_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/status_bar.py` & `gns3-gui-3.0.0a3/gns3/status_bar.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/style.py` & `gns3-gui-3.0.0a3/gns3/style.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/symbol.py` & `gns3-gui-3.0.0a3/gns3/symbol.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/telnet_console.py` & `gns3-gui-3.0.0a3/gns3/telnet_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/template.py` & `gns3-gui-3.0.0a3/gns3/template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/template_manager.py` & `gns3-gui-3.0.0a3/gns3/template_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/topology.py` & `gns3-gui-3.0.0a3/gns3/topology.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/topology_summary_view.py` & `gns3-gui-3.0.0a3/gns3/topology_summary_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/about_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/about_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/about_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/appliance_wizard.ui` & `gns3-gui-3.0.0a3/gns3/ui/appliance_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/appliance_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/appliance_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/capture_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/capture_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/capture_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/capture_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/configuration_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/configuration_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/configuration_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/console_command_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/console_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/console_command_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/console_command_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/controller_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/ui/controller_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/controller_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/controller_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/custom_adapters_configuration_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/custom_adapters_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/custom_adapters_configuration_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/custom_adapters_configuration_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/doctor_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/doctor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/doctor_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/doctor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/edit_compute_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/edit_compute_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/edit_compute_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/edit_compute_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/edit_project_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/edit_project_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/edit_project_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/edit_project_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/exec_command_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/exec_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/exec_command_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/exec_command_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/export_debug_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/export_debug_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/export_debug_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/export_debug_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/export_project_wizard.ui` & `gns3-gui-3.0.0a3/gns3/ui/export_project_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/export_project_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/export_project_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/file_editor_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/file_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/file_editor_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/file_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/filter_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/filter_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/filter_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/filter_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/general_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/ui/general_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/general_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/general_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/gns3_vm_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/ui/gns3_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/gns3_vm_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/gns3_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/idlepc_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/idlepc_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/idlepc_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/idlepc_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/image_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/image_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/image_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/image_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/login_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/login_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/login_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/login_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/main_window.ui` & `gns3-gui-3.0.0a3/gns3/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/main_window_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/new_template_wizard.ui` & `gns3-gui-3.0.0a3/gns3/ui/new_template_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/new_template_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/new_template_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/node_info_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/node_info_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/node_info_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/node_info_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/node_properties_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/node_properties_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/node_properties_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/node_properties_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/packet_capture_preferences_page.ui` & `gns3-gui-3.0.0a3/gns3/ui/packet_capture_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/packet_capture_preferences_page_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/packet_capture_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/preferences_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/preferences_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/preferences_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/preferences_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/profile_select_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/profile_select_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/profile_select_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/profile_select_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/project_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/project_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/project_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/project_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/project_welcome_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/project_welcome_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/project_welcome_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/project_welcome_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/resources_rc.py` & `gns3-gui-3.0.0a3/gns3/ui/resources_rc.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/setup_wizard.ui` & `gns3-gui-3.0.0a3/gns3/ui/setup_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/setup_wizard_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/setup_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/show_readme_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/show_readme_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/show_readme_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/show_readme_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/snapshots_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/snapshots_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/snapshots_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/snapshots_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/style_editor_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/style_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/style_editor_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/style_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/symbol_selection_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/symbol_selection_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/symbol_selection_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/symbol_selection_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/text_editor_dialog.ui` & `gns3-gui-3.0.0a3/gns3/ui/text_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/ui/text_editor_dialog_ui.py` & `gns3-gui-3.0.0a3/gns3/ui/text_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/update_manager.py` & `gns3-gui-3.0.0a3/gns3/update_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,8 +235,26 @@
             with tarfile.open(tgz, 'r:gz') as tar:
                 # Tar add a folder with the name of archive in first position
                 # we need to drop it
                 members = tar.getmembers()[1:]
                 for member in members:
                     # Path separator is always / even on windows
                     member.name = member.name.split("/", 1)[1]
-                tar.extractall(path=self._package_directory, members=members)
+                def is_within_directory(directory, target):
+
+                    abs_directory = os.path.abspath(directory)
+                    abs_target = os.path.abspath(target)
+
+                    prefix = os.path.commonprefix([abs_directory, abs_target])
+
+                    return prefix == abs_directory
+
+                def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+
+                    for member in tar.getmembers():
+                        member_path = os.path.join(path, member.name)
+                        if not is_within_directory(path, member_path):
+                            raise Exception("Attempted Path Traversal in Tar File")
+
+                    tar.extractall(path, members, numeric_owner=numeric_owner)
+
+                safe_extract(tar, path=self._package_directory, members=members)
```

### Comparing `gns3-gui-3.0.0a2/gns3/utils/__init__.py` & `gns3-gui-3.0.0a3/gns3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/analytics.py` & `gns3-gui-3.0.0a3/gns3/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/bring_to_front.py` & `gns3-gui-3.0.0a3/gns3/utils/bring_to_front.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/file_copy_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/file_copy_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/get_icon.py` & `gns3-gui-3.0.0a3/gns3/utils/get_icon.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/get_resource.py` & `gns3-gui-3.0.0a3/gns3/utils/get_resource.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/import_project_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/import_project_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/interfaces.py` & `gns3-gui-3.0.0a3/gns3/utils/interfaces.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/normalize_filename.py` & `gns3-gui-3.0.0a3/gns3/utils/normalize_filename.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/process_files_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/process_files_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/progress_dialog.py` & `gns3-gui-3.0.0a3/gns3/utils/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/run_in_terminal.py` & `gns3-gui-3.0.0a3/gns3/utils/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/server_select.py` & `gns3-gui-3.0.0a3/gns3/utils/server_select.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/sudo.py` & `gns3-gui-3.0.0a3/gns3/utils/sudo.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/wait_for_command_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/wait_for_command_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/wait_for_connection_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/wait_for_connection_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/wait_for_lambda_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/wait_for_lambda_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/utils/wait_for_runas_worker.py` & `gns3-gui-3.0.0a3/gns3/utils/wait_for_runas_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3/version.py` & `gns3-gui-3.0.0a3/gns3/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 # __version_info__ is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 
-__version__ = "3.0.0a2"
+__version__ = "3.0.0a3"
 __version_info__ = (3, 0, 0, -99)
 
 if "dev" in __version__:
     try:
         import os
         import subprocess
         if os.path.exists(os.path.join(os.path.dirname(os.path.abspath(__file__)), "..", ".git")):
             r = subprocess.check_output(["git", "rev-parse", "--short", "HEAD"]).decode().strip("\n")
-            __version__ += "-" + r
+            __version__ += "+" + r
     except Exception as e:
         print(e)
```

### Comparing `gns3-gui-3.0.0a2/gns3/vnc_console.py` & `gns3-gui-3.0.0a3/gns3/vnc_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/gns3_gui.egg-info/PKG-INFO` & `gns3-gui-3.0.0a3/gns3_gui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3-gui
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: GNS3 graphical interface for the GNS3 server.
 Home-page: http://github.com/GNS3/gns3-gui
 Author: Jeremy Grossmann
 Author-email: package-maintainer@gns3.net
 License: GNU General Public License v3 (GPLv3)
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.4
 License-File: LICENSE
 License-File: COPYING
 License-File: AUTHORS
 
 # GNS3-gui
@@ -70,9 +71,7 @@
 https://github.com/Kozea/wdb
 
 ## Security issues
 
 Please contact us at security@gns3.net
 
 
-
-
```

### Comparing `gns3-gui-3.0.0a2/gns3_gui.egg-info/SOURCES.txt` & `gns3-gui-3.0.0a3/gns3_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/add-link-1-cancel.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/add-link-1-cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/add-link-1-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/add-link-1-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/add-link-1.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/add-link-1.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/add-note-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/add-note-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/add-note.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/aux-console-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/aux-console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/aux-console.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/browse-all-icons-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/browse-all-icons-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/browse-all-icons.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/browse-all-icons.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/calculate-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/calculate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/calculate.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/camera-photo-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/camera-photo.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/capture-start-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/capture-start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/capture-start.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/capture-stop-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/capture-stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/capture-stop.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/command_line-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/command_line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/command_line.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/configuration-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/configuration-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/configuration.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/console-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/console.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/console_edit-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/console_edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/console_edit.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/delete-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/delete-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/delete.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/duplicate-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/duplicate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/duplicate.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/edit-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/edit.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/ellipse-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/ellipse.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/export-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/export-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/export.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/filter-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/filter-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/filter-reset-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/filter-reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/filter-reset.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/filter.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/firewall-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/firewall-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/firewall.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/front-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/front-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/front.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/help-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/help.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/image-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/image-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/image.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/import-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/import-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/import.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/import_export_configs-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/import_export_configs-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/import_export_configs.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/inspect-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/inspect-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/inspect.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/line-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/line.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/link-pause.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/link-pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/link-start.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/link-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/lock-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/lock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/lock.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/lower_z_value-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/lower_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/lower_z_value.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/minus-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/minus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/minus.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/new-project-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/new-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/new-project.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/node_conception-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/node_conception-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/node_conception.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/open-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/open-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/open.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/pause-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/pause.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/pc-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/pc-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/pc.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/pc.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/plus-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/plus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/plus.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/preferences-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/preferences-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/preferences.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/quit-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/quit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/quit.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/raise_z_value-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/raise_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/raise_z_value.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/rectangle-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/rectangle.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/reload-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/reload-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/reload.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/reset-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/reset.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/router-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/router-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/router.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/save-as-project-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/save-as-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/save-as-project.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/save-project-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/save-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/save-project.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/save-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/show-hostname-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/show-hostname-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/show-hostname.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/show-interface-names-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/show-interface-names-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/show-interface-names.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/snapshot-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/snapshot-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/snapshot.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/start-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/start.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/stop-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/stop.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/switch-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/switch-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/switch.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/unlock-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/unlock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/unlock.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-in-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-in-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-in.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-out-hover.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-out-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/charcoal_icons/zoom-out.svg` & `gns3-gui-3.0.0a3/resources/charcoal_icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/add-link-cancel.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/add-link-cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/add-link-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/add-link-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/add-link.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/add-link.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/add-note-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/add-note-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/add-note.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/aux-console-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/aux-console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/aux-console.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/browse-all-icons-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/browse-all-icons-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/browse-all-icons.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/browse-all-icons.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/calculate-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/calculate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/calculate.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/camera-photo-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/camera-photo.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/capture-start-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/capture-start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/capture-start.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/capture-stop-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/capture-stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/capture-stop.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/command_line-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/command_line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/command_line.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/configuration-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/configuration-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/configuration.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/console-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/console.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/console_edit-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/console_edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/console_edit.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/delete-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/delete-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/delete.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/duplicate-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/duplicate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/duplicate.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/edit-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/edit.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/ellipse-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/ellipse.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/export-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/export-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/export.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/filter-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/filter-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/filter-reset-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/filter-reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/filter-reset.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/filter.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/firewall-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/firewall-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/firewall.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/front-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/front-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/front.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/help-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/help.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/image-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/image-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/image.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/import-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/import-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/import.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/import_export_configs-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/import_export_configs-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/import_export_configs.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/inspect-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/inspect-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/inspect.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/line-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/line.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/link-pause.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/link-pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/link-start.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/link-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/lock-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/lock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/lock.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/lower_z_value-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/lower_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/lower_z_value.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/minus-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/minus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/minus.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/new-project-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/new-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/new-project.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/node_conception-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/node_conception-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/node_conception.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/open-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/open-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/open.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/pause-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/pause.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/pc-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/pc-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/pc.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/pc.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/plus-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/plus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/plus.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/preferences-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/preferences-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/preferences.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/quit-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/quit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/quit.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/raise_z_value-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/raise_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/raise_z_value.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/rectangle-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/rectangle.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/reload-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/reload-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/reload.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/reset-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/reset.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/router-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/router-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/router.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/save-as-project-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/save-as-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/save-as-project.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/save-project-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/save-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/save-project.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/save-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/show-hostname-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/show-hostname-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/show-hostname.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/show-interface-names-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/show-interface-names-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/show-interface-names.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/snapshot-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/snapshot-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/snapshot.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/start-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/start.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/stop-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/stop.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/switch-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/switch-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/switch.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/unlock-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/unlock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/unlock.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/zoom-in-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/zoom-in-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/zoom-in.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/zoom-out-hover.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/zoom-out-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/classic_icons/zoom-out.svg` & `gns3-gui-3.0.0a3/resources/classic_icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/PC-hover.png` & `gns3-gui-3.0.0a3/resources/icons/PC-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/PC.png` & `gns3-gui-3.0.0a3/resources/icons/PC.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/add-note.svg` & `gns3-gui-3.0.0a3/resources/icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/applications.svg` & `gns3-gui-3.0.0a3/resources/icons/applications.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/aux-console.svg` & `gns3-gui-3.0.0a3/resources/icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/browse-all-icons-hover.png` & `gns3-gui-3.0.0a3/resources/icons/browse-all-icons-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/browse-all-icons.png` & `gns3-gui-3.0.0a3/resources/icons/browse-all-icons.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/calculate.svg` & `gns3-gui-3.0.0a3/resources/icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/camera-photo-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/camera-photo.svg` & `gns3-gui-3.0.0a3/resources/icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/cancel-connection.svg` & `gns3-gui-3.0.0a3/resources/icons/cancel-connection.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/cancel.svg` & `gns3-gui-3.0.0a3/resources/icons/cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/capture-start.svg` & `gns3-gui-3.0.0a3/resources/icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/capture-stop.svg` & `gns3-gui-3.0.0a3/resources/icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/command_line.svg` & `gns3-gui-3.0.0a3/resources/icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/configuration.svg` & `gns3-gui-3.0.0a3/resources/icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/connection-new-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/connection-new-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/connection-new.svg` & `gns3-gui-3.0.0a3/resources/icons/connection-new.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/console.svg` & `gns3-gui-3.0.0a3/resources/icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/console_edit.svg` & `gns3-gui-3.0.0a3/resources/icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/delete.svg` & `gns3-gui-3.0.0a3/resources/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/dialog-warning.svg` & `gns3-gui-3.0.0a3/resources/icons/dialog-warning.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/drawing.svg` & `gns3-gui-3.0.0a3/resources/icons/drawing.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/duplicate.svg` & `gns3-gui-3.0.0a3/resources/icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/edit.svg` & `gns3-gui-3.0.0a3/resources/icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/ellipse-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/ellipse.svg` & `gns3-gui-3.0.0a3/resources/icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/export.svg` & `gns3-gui-3.0.0a3/resources/icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/filter-capture.svg` & `gns3-gui-3.0.0a3/resources/icons/filter-capture.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/filter-reset.svg` & `gns3-gui-3.0.0a3/resources/icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/filter.svg` & `gns3-gui-3.0.0a3/resources/icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/firewall-hover.png` & `gns3-gui-3.0.0a3/resources/icons/firewall-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/firewall.png` & `gns3-gui-3.0.0a3/resources/icons/firewall.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/front.svg` & `gns3-gui-3.0.0a3/resources/icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/help.svg` & `gns3-gui-3.0.0a3/resources/icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/horizontally.svg` & `gns3-gui-3.0.0a3/resources/icons/horizontally.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/image.svg` & `gns3-gui-3.0.0a3/resources/icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/import.svg` & `gns3-gui-3.0.0a3/resources/icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/import_export_configs.svg` & `gns3-gui-3.0.0a3/resources/icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/inspect.svg` & `gns3-gui-3.0.0a3/resources/icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/led_gray.svg` & `gns3-gui-3.0.0a3/resources/icons/led_gray.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/led_green.svg` & `gns3-gui-3.0.0a3/resources/icons/led_green.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/led_red.svg` & `gns3-gui-3.0.0a3/resources/icons/led_red.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/led_yellow.svg` & `gns3-gui-3.0.0a3/resources/icons/led_yellow.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/lock.svg` & `gns3-gui-3.0.0a3/resources/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/lower_z_value.svg` & `gns3-gui-3.0.0a3/resources/icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/minus.svg` & `gns3-gui-3.0.0a3/resources/icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/new-project.svg` & `gns3-gui-3.0.0a3/resources/icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/new.svg` & `gns3-gui-3.0.0a3/resources/icons/new.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/node_conception.svg` & `gns3-gui-3.0.0a3/resources/icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/open.svg` & `gns3-gui-3.0.0a3/resources/icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/pause-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/pause.svg` & `gns3-gui-3.0.0a3/resources/icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/plus.svg` & `gns3-gui-3.0.0a3/resources/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/quit.svg` & `gns3-gui-3.0.0a3/resources/icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/raise_z_value.svg` & `gns3-gui-3.0.0a3/resources/icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/rectangle-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/rectangle.svg` & `gns3-gui-3.0.0a3/resources/icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/reload.svg` & `gns3-gui-3.0.0a3/resources/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/reset.svg` & `gns3-gui-3.0.0a3/resources/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/router-hover.png` & `gns3-gui-3.0.0a3/resources/icons/router-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/router.png` & `gns3-gui-3.0.0a3/resources/icons/router.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/rtv.png` & `gns3-gui-3.0.0a3/resources/icons/rtv.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/save-as-project.svg` & `gns3-gui-3.0.0a3/resources/icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/save-as.svg` & `gns3-gui-3.0.0a3/resources/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/save.svg` & `gns3-gui-3.0.0a3/resources/icons/save.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/show-hostname.svg` & `gns3-gui-3.0.0a3/resources/icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/show-interface-names.svg` & `gns3-gui-3.0.0a3/resources/icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/snapshot.svg` & `gns3-gui-3.0.0a3/resources/icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/start-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/start.svg` & `gns3-gui-3.0.0a3/resources/icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/stop-hover.svg` & `gns3-gui-3.0.0a3/resources/icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/stop.svg` & `gns3-gui-3.0.0a3/resources/icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/switch-hover.png` & `gns3-gui-3.0.0a3/resources/icons/switch-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/switch.png` & `gns3-gui-3.0.0a3/resources/icons/switch.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/unlock.svg` & `gns3-gui-3.0.0a3/resources/icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/vertically.svg` & `gns3-gui-3.0.0a3/resources/icons/vertically.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/virtualbox.png` & `gns3-gui-3.0.0a3/resources/icons/virtualbox.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/warning.svg` & `gns3-gui-3.0.0a3/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/wireshark.png` & `gns3-gui-3.0.0a3/resources/icons/wireshark.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/zoom-in-hover.png` & `gns3-gui-3.0.0a3/resources/icons/zoom-in-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/zoom-in.png` & `gns3-gui-3.0.0a3/resources/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/zoom-out-hover.png` & `gns3-gui-3.0.0a3/resources/icons/zoom-out-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/icons/zoom-out.png` & `gns3-gui-3.0.0a3/resources/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/images/gns3.ico` & `gns3-gui-3.0.0a3/resources/images/gns3.ico`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/images/gns3_icon_128x128.png` & `gns3-gui-3.0.0a3/resources/images/gns3_icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/images/gns3_icon_256x256.png` & `gns3-gui-3.0.0a3/resources/images/gns3_icon_256x256.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/images/gns3_logo.png` & `gns3-gui-3.0.0a3/resources/images/gns3_logo.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/gns3-gui.xml` & `gns3-gui-3.0.0a3/resources/linux/gns3-gui.xml`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/16x16/apps/gns3.png` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/16x16/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/32x32/apps/gns3.png` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/32x32/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/apps/gns3.png` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/apps/gns3.svg` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/apps/gns3.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg` & `gns3-gui-3.0.0a3/resources/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/resources.qrc` & `gns3-gui-3.0.0a3/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/styles/charcoal.css` & `gns3-gui-3.0.0a3/resources/styles/charcoal.css`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/atm_switch.svg` & `gns3-gui-3.0.0a3/resources/symbols/atm_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/cloud.svg` & `gns3-gui-3.0.0a3/resources/symbols/cloud.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/computer.svg` & `gns3-gui-3.0.0a3/resources/symbols/computer.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/docker_guest.svg` & `gns3-gui-3.0.0a3/resources/symbols/docker_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/ethernet_switch.svg` & `gns3-gui-3.0.0a3/resources/symbols/ethernet_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/firewall.svg` & `gns3-gui-3.0.0a3/resources/symbols/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/frame_relay_switch.svg` & `gns3-gui-3.0.0a3/resources/symbols/frame_relay_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/hub.svg` & `gns3-gui-3.0.0a3/resources/symbols/hub.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/multilayer_switch.svg` & `gns3-gui-3.0.0a3/resources/symbols/multilayer_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/qemu_guest.svg` & `gns3-gui-3.0.0a3/resources/symbols/qemu_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/router.svg` & `gns3-gui-3.0.0a3/resources/symbols/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/vbox_guest.svg` & `gns3-gui-3.0.0a3/resources/symbols/vbox_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/vmware_guest.svg` & `gns3-gui-3.0.0a3/resources/symbols/vmware_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/resources/symbols/vpcs_guest.svg` & `gns3-gui-3.0.0a3/resources/symbols/vpcs_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/setup.py` & `gns3-gui-3.0.0a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,10 +92,11 @@
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
 )
```

### Comparing `gns3-gui-3.0.0a2/tests/conftest.py` & `gns3-gui-3.0.0a3/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 import pytest
 import os
 import uuid
 from unittest.mock import MagicMock
 import tempfile
-import urllib.request
 import sys
 sys._called_from_test = True
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-# If the QT application is not initialized we can got segfault
+#  We can get segfault if the QT application is not initialized
 from gns3.qt.QtWidgets import QApplication
 app = QApplication([])
 
 
 @pytest.fixture(autouse=True)
 def reset_qt_signal():
     """
@@ -75,25 +74,14 @@
     Controller._instance = None
     c = Controller.instance()
     c._http_client = MagicMock()
     return c
 
 
 @pytest.fixture
-def gns3vm_server():
-
-    from gns3.servers import Servers
-
-    Servers.instance()._settings["vm"]["auto_start"] = True
-    Servers.instance().initVMServer()
-    assert Servers.instance().vmServer() is not None
-    return Servers.instance().vmServer()
-
-
-@pytest.fixture
 def vpcs_device(local_server, project):
 
     from gns3.modules.vpcs.vpcs_node import VPCSNode
     from gns3.modules.vpcs import VPCS
 
     device = VPCSNode(VPCS(), local_server, project)
     device._node_id = str(uuid.uuid4())
@@ -157,18 +145,18 @@
     (fd, config_path) = tempfile.mkstemp()
     os.close(fd)
 
     LocalConfig._instance = LocalConfig(config_file=config_path)
     return LocalConfig.instance()
 
 
-@pytest.yield_fixture(autouse=True)
+@pytest.fixture(autouse=True)
 def run_around_tests(local_config, main_window):
     """
-    This setup a temporay environnement around tests
+    This setup a temporary environment around tests
     """
 
     from gns3.main_window import MainWindow
     MainWindow._instance = main_window
     yield
```

### Comparing `gns3-gui-3.0.0a2/tests/items/test_ellipse_item.py` & `gns3-gui-3.0.0a3/tests/items/test_ellipse_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/items/test_image_item.py` & `gns3-gui-3.0.0a3/tests/items/test_image_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/items/test_label_item.py` & `gns3-gui-3.0.0a3/tests/items/test_label_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/items/test_line_item.py` & `gns3-gui-3.0.0a3/tests/items/test_line_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/items/test_rectangle_item.py` & `gns3-gui-3.0.0a3/tests/items/test_rectangle_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/items/test_text_item.py` & `gns3-gui-3.0.0a3/tests/items/test_text_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/modules/docker/test_docker_vm.py` & `gns3-gui-3.0.0a3/tests/modules/docker/test_docker_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/modules/dynamips/test_dynamips_init.py` & `gns3-gui-3.0.0a3/tests/modules/dynamips/test_dynamips_init.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/modules/iou/test_iou_device.py` & `gns3-gui-3.0.0a3/tests/modules/iou/test_iou_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/modules/qemu/test_qemu_vm.py` & `gns3-gui-3.0.0a3/tests/modules/qemu/test_qemu_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/modules/virtualbox/test_virtualbox_vm.py` & `gns3-gui-3.0.0a3/tests/modules/virtualbox/test_virtualbox_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/modules/vpcs/test_vpcs_device.py` & `gns3-gui-3.0.0a3/tests/modules/vpcs/test_vpcs_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/qt/test_qimage_svg_renderer.py` & `gns3-gui-3.0.0a3/tests/qt/test_qimage_svg_renderer.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/arista-veos.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/arista-veos.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/broken-microcore-linux.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/broken-microcore-linux.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/cisco-3745.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/cisco-3745.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/cisco-iou-l3.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/cisco-iou-l3.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/juniper-vsrx.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/juniper-vsrx.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/microcore-linux.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/microcore-linux.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/appliances/openvswitch.gns3a` & `gns3-gui-3.0.0a3/tests/registry/appliances/openvswitch.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/test_appliance.py` & `gns3-gui-3.0.0a3/tests/registry/test_appliance.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/test_appliance_to_template.py` & `gns3-gui-3.0.0a3/tests/registry/test_appliance_to_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "path": iou_l3
         }
     ]
     new_template = ApplianceToTemplate().new_template(config, "local")
     assert new_template == {
         "category": "router",
         "template_type": "iou",
-        "symbol": ":/symbols/router.svg",
+        "symbol": "router",
         "compute_id": "local",
         "name": "Cisco IOU L3",
         "nvram": 128,
         "ram": 256,
         "serial_adapters": 2,
         "ethernet_adapters": 2,
         "startup_config": "iou_l3_base_startup-config.txt",
@@ -97,15 +97,15 @@
 
     new_template = ApplianceToTemplate().new_template(config, "local")
     assert new_template == {
         "name": "Open vSwitch",
         "template_type": "docker",
         "image": "gns3/openvswitch:latest",
         "category": "switch",
-        "symbol": ":/symbols/multilayer_switch.svg",
+        "symbol": "multilayer_switch",
         "compute_id": "local",
         "adapters": 16,
         "usage": "By default all interfaces are connected to the br0"
     }
 
 
 def test_add_appliance_dynamips(cisco_3745):
@@ -134,15 +134,15 @@
         "compute_id": "local",
         "slot0": "GT96100-FE",
         "slot1": "NM-1FE-TX",
         "slot2": "NM-4T",
         "slot3": "",
         "slot4": "",
         "startup_config": "ios_base_startup-config.txt",
-        "symbol": ":/symbols/router.svg",
+        "symbol": "router",
         "wic0": "WIC-1T",
         "wic1": "WIC-1T",
         "wic2": "WIC-1T"
     }
 
 
 def test_add_appliance_guest(linux_microcore_img):
@@ -159,19 +159,19 @@
     new_template = ApplianceToTemplate().new_template(config, "local")
     assert new_template == {
         "template_type": "qemu",
         "adapter_type": "e1000",
         "adapters": 1,
         "category": "guest",
         "console_type": "telnet",
-        "symbol": ":/symbols/qemu_guest.svg",
+        "symbol": "qemu_guest",
         "hda_disk_image": "linux-microcore-3.4.1.img",
         "name": "Micro Core Linux",
         "options": "",
-        "qemu_path": "qemu-system-i386",
+        "platform": "i386",
         "usage": "Just start the appliance",
         "ram": 32,
         "compute_id": "local"
     }
 
 
 def test_add_appliance_with_symbol(linux_microcore_img):
@@ -185,26 +185,28 @@
         }
     ]
     config["symbol"] = ":/symbols/asa.svg"
     new_template = ApplianceToTemplate().new_template(config, "local")
     assert new_template["symbol"] == ":/symbols/asa.svg"
 
 
-def test_add_appliance_with_symbol_from_symbols_dir(empty_config, linux_microcore_img, symbols_dir):
+def test_add_appliance_with_symbol_from_symbols_dir(linux_microcore_img, symbols_dir, controller):
+
     with open("tests/registry/appliances/microcore-linux.gns3a", encoding="utf-8") as f:
         config = json.load(f)
     config["images"] = [
         {
             "type": "hda_disk_image",
             "filename": "linux-microcore-3.4.1.img",
             "path": linux_microcore_img
         }
     ]
     config["symbol"] = "linux_guest.svg"
 
+    controller.settings()["symbols_path"] = symbols_dir
     symbol_path = os.path.join(symbols_dir, "linux_guest.svg")
     open(symbol_path, 'w+').close()
 
     new_template = ApplianceToTemplate().new_template(config, "local")
     assert new_template["symbol"] == "linux_guest.svg"
 
 
@@ -257,20 +259,20 @@
 
     new_template = ApplianceToTemplate().new_template(config, "local")
     assert new_template == {
         "template_type": "qemu",
         "adapter_type": "e1000",
         "adapters": 8,
         "category": "router",
-        "symbol": ":/symbols/router.svg",
+        "symbol": "router",
         "hda_disk_image": "a",
         "hdb_disk_image": "b",
         "name": "Arista vEOS",
         "options": "",
-        "qemu_path": "qemu-system-x86_64",
+        "platform": "x86_64",
         "ram": 2048,
         "console_type": "telnet",
         "compute_id": "local"
     }
 
 
 def test_add_appliance_path_relative_to_images_dir(tmpdir, linux_microcore_img):
```

### Comparing `gns3-gui-3.0.0a2/tests/registry/test_config.py` & `gns3-gui-3.0.0a3/tests/registry/test_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/test_image.py` & `gns3-gui-3.0.0a3/tests/registry/test_image.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/registry/test_registry.py` & `gns3-gui-3.0.0a3/tests/registry/test_registry.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_compute.py` & `gns3-gui-3.0.0a3/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_compute_manager.py` & `gns3-gui-3.0.0a3/tests/test_compute_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import copy
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, ANY
 
 from gns3.compute_manager import ComputeManager
 from gns3.compute import Compute
 
 
 def test_getCompute():
     cm = ComputeManager()
@@ -163,15 +163,15 @@
     cm = ComputeManager()
     computes = []
     compute = Compute()
     computes.append(compute)
     controller._http_client = MagicMock()
     cm.updateList(computes)
     assert compute.id() in cm._computes
-    controller._http_client.sendRequest.assert_called_with("POST", "/computes", None, body=compute.__json__())
+    controller._http_client.sendRequest.assert_called_with("POST", "/computes", callback=ANY, body=compute.__json__(), params={'connect': True})
 
 
 def test_updateList_no_change(controller):
     cm = ComputeManager()
     computes = []
     compute = copy.copy(cm.getCompute("test1"))
     computes.append(compute)
```

### Comparing `gns3-gui-3.0.0a2/tests/test_controller.py` & `gns3-gui-3.0.0a3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_graphics_view.py` & `gns3-gui-3.0.0a3/tests/test_graphics_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_http_client.py` & `gns3-gui-3.0.0a3/tests/test_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 def http_client(http_request, network_manager):
 
     http_client = HTTPClient({"protocol": "http", "host": "127.0.0.1", "port": "3080"})
     http_client._network_manager = network_manager
     return http_client
 
 
-@pytest.yield_fixture(autouse=True)
+@pytest.fixture(autouse=True)
 def http_request():
 
     mock = unittest.mock.Mock()
 
     def call_request(url):
         mock(url)
         return mock
```

### Comparing `gns3-gui-3.0.0a2/tests/test_image_manager.py` & `gns3-gui-3.0.0a3/tests/test_image_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @pytest.fixture
 def images_dir(tmpdir):
     path = tmpdir / "images"
     path.mkdir()
     return path
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def image_manager(tmpdir, images_dir):
     ImageManager._instance = None
     settings = CONTROLLER_SETTINGS
     settings['images_path'] = str(images_dir)
     with patch('gns3.local_config.LocalConfig.loadSectionSettings', return_value=CONTROLLER_SETTINGS):
         yield ImageManager.instance()
     ImageManager._instance = None
```

### Comparing `gns3-gui-3.0.0a2/tests/test_image_upload_manager.py` & `gns3-gui-3.0.0a3/tests/test_image_upload_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_link.py` & `gns3-gui-3.0.0a3/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_local_config.py` & `gns3-gui-3.0.0a3/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_local_server.py` & `gns3-gui-3.0.0a3/tests/test_local_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,45 +12,45 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import sys
-import json
 import pytest
 import logging
 import subprocess
 import unittest
 from unittest.mock import MagicMock, patch
 
 from gns3.local_server import LocalServer
 
 
 @pytest.fixture
 def local_server_path(tmpdir):
     return str(tmpdir / "gns3server")
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def local_server(local_server_path, tmpdir):
     with open(str(tmpdir / "test.cfg"), "w+") as f:
         f.write("""
 [Server]
 path={}""".format(local_server_path))
 
     LocalServer._instance = None
     with patch("gns3.local_server.LocalServer.localServerAutoStartIfRequired"):
         local_server = LocalServer.instance()
         local_server._config_directory = str(tmpdir)
         yield local_server
 
 
+# Windows GUI doesn't support a local server starting with v3.0
 @pytest.mark.skipif(sys.platform.startswith('win') is True, reason='Not for windows')
-def test_startLocalServer(tmpdir, local_server, local_server_path):
+def test_start_local_server(tmpdir, local_server, local_server_path):
     logging.getLogger().setLevel(logging.DEBUG)  # Make sure we are using debug level in order to get the --debug
 
     process_mock = MagicMock()
     with patch("subprocess.Popen", return_value=process_mock) as mock:
 
         # If everything work fine the command is still running and a timeout is raised
         process_mock.communicate.side_effect = subprocess.TimeoutExpired("test", 1)
@@ -61,15 +61,17 @@
                                  '--allow',
                                  '--debug',
                                  '--logfile=' + str(tmpdir / "gns3_server.log"),
                                  '--pid=' + str(tmpdir / "gns3_server.pid")
                                  ], stderr=unittest.mock.ANY)
 
 
-def test_killAlreadyRunningServer(local_server):
+# Windows GUI doesn't support a local server starting with v3.0
+@pytest.mark.skipif(sys.platform.startswith('win') is True, reason='Not for windows')
+def test_kill_already_running_server(local_server):
     with open(local_server._pid_path(), "w+") as f:
         f.write("42")
 
     mock_process = MagicMock()
     with patch("psutil.Process", return_value=mock_process) as mock:
         LocalServer.instance()._killAlreadyRunningServer()
         mock.assert_called_with(pid=42)
```

### Comparing `gns3-gui-3.0.0a2/tests/test_network_client.py` & `gns3-gui-3.0.0a3/tests/test_network_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_node.py` & `gns3-gui-3.0.0a3/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_progress.py` & `gns3-gui-3.0.0a3/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_project.py` & `gns3-gui-3.0.0a3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_spice_console.py` & `gns3-gui-3.0.0a3/tests/test_spice_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_topology.py` & `gns3-gui-3.0.0a3/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_update_manager.py` & `gns3-gui-3.0.0a3/tests/test_update_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,33 @@
 import os
 
 
 from gns3.update_manager import UpdateManager
 from gns3 import version
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def frozen():
     sys.frozen = True
     yield
     delattr(sys, 'frozen')
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def devVersion():
     old_version_info = version.__version_info__
     old_version = version.__version__
     version.__version_info__ = (1, 4, 0, -99)
     version.__version__ = '1.4.0'
     yield
     version.__version_info__ = old_version
     version.__version__ = old_version
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def stableVersion():
     old_version_info = version.__version_info__
     old_version = version.__version__
     version.__version_info__ = (1, 4, 0, 0)
     version.__version__ = '1.4.0'
     yield
     version.__version_info__ = old_version_info
```

### Comparing `gns3-gui-3.0.0a2/tests/test_utils.py` & `gns3-gui-3.0.0a3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/test_vnc_console.py` & `gns3-gui-3.0.0a3/tests/test_vnc_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/utils/test_file_copy_worker.py` & `gns3-gui-3.0.0a3/tests/utils/test_file_copy_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0a2/tests/utils/test_server_select.py` & `gns3-gui-3.0.0a3/tests/utils/test_server_select.py`

 * *Files identical despite different names*

