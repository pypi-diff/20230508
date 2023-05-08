# Comparing `tmp/NodeGraphQt-0.5.8.tar.gz` & `tmp/NodeGraphQt-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.5.8.tar", last modified: Thu May  4 10:20:26 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.5.9.tar", last modified: Fri May  5 10:43:50 2023, max compression
```

## Comparing `NodeGraphQt-0.5.8.tar` & `NodeGraphQt-0.5.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.471355 NodeGraphQt-0.5.8/
--rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.8/LICENSE.md
--rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.5.8/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.214610 NodeGraphQt-0.5.8/NodeGraphQt/
--rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.264239 NodeGraphQt-0.5.8/NodeGraphQt/base/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/factory.py
--rw-rw-rw-   0        0        0    97821 2023-05-04 10:16:17.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    14329 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/model.py
--rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/node.py
--rw-rw-rw-   0        0        0    12137 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7417 2023-05-03 04:38:45.000000 NodeGraphQt-0.5.8/NodeGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.276242 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.326253 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.346258 NodeGraphQt-0.5.8/NodeGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    23281 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5817 2023-05-04 10:15:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      239 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.410273 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    10763 2023-05-03 01:54:07.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    36771 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    21504 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.447351 NodeGraphQt-0.5.8/NodeGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.448351 NodeGraphQt-0.5.8/NodeGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    14045 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    51080 2023-05-03 09:00:22.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6914 2023-05-04 05:49:13.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.232613 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/
--rw-rw-rw-   0        0        0     2738 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2738 2023-05-04 10:20:26.471355 NodeGraphQt-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     2034 2023-05-03 10:36:51.000000 NodeGraphQt-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.192605 NodeGraphQt-0.5.8/examples/
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.450350 NodeGraphQt-0.5.8/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6199 2023-05-04 10:16:17.000000 NodeGraphQt-0.5.8/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.470355 NodeGraphQt-0.5.8/examples/nodes/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.5.8/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1070 2023-05-04 10:20:26.476357 NodeGraphQt-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.868894 NodeGraphQt-0.5.9/
+-rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.9/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.5.9/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.573658 NodeGraphQt-0.5.9/NodeGraphQt/
+-rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.631841 NodeGraphQt-0.5.9/NodeGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0    97819 2023-05-05 10:40:41.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    14329 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    12137 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     7417 2023-05-03 04:38:45.000000 NodeGraphQt-0.5.9/NodeGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.644844 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.699856 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.729863 NodeGraphQt-0.5.9/NodeGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    23281 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5817 2023-05-04 10:15:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      239 2023-05-05 10:41:15.000000 NodeGraphQt-0.5.9/NodeGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.796878 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    10763 2023-05-03 01:54:07.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    36771 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    21504 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.838887 NodeGraphQt-0.5.9/NodeGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.839889 NodeGraphQt-0.5.9/NodeGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    14045 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    51135 2023-05-05 10:40:41.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6914 2023-05-04 05:49:13.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.593663 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/
+-rw-rw-rw-   0        0        0     2738 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2738 2023-05-05 10:43:50.868894 NodeGraphQt-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2034 2023-05-03 10:36:51.000000 NodeGraphQt-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.546651 NodeGraphQt-0.5.9/examples/
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.845890 NodeGraphQt-0.5.9/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6199 2023-05-04 10:16:17.000000 NodeGraphQt-0.5.9/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.867894 NodeGraphQt-0.5.9/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.5.9/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1070 2023-05-05 10:43:50.873911 NodeGraphQt-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.5.9/setup.py
```

### Comparing `NodeGraphQt-0.5.8/LICENSE.md` & `NodeGraphQt-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/__init__.py` & `NodeGraphQt-0.5.9/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -923,15 +923,15 @@
         See Also:
             To enable/disable pipe slicer
             :meth:`NodeGraph.set_pipe_slicing`
 
         Returns:
             bool: True if pipe slicing is enabled.
         """
-        return self._model.pipe_collision
+        return self._model.pipe_slicing
 
     def set_pipe_slicing(self, mode=True):
         """
         Enable/Disable pipe slicer.
 
         When set to true holding down ``Alt + Shift + LMB Drag`` will allow node
         pipe connections to be sliced.
```

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/model.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/node.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/base/port.py` & `NodeGraphQt-0.5.9/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/constants.py` & `NodeGraphQt-0.5.9/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.5.9/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.5.9/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.5.9/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,29 +670,28 @@
 
         # Todo: find a better solution to catch modifier keys.
         if event.modifiers() == (QtCore.Qt.AltModifier | QtCore.Qt.ShiftModifier):
             self.ALT_state = True
             self.SHIFT_state = True
 
         # show cursor text
+        overlay_text = None
         self._cusor_text.setVisible(False)
         if not self.ALT_state:
             if self.SHIFT_state:
-                self._cusor_text.setPlainText(
-                    '\n    SHIFT:'
-                    '\n    Toggle/Extend Selection'
-                )
+                overlay_text = '\n    SHIFT:\n    Toggle/Extend Selection'
             elif self.CTRL_state:
-                self._cusor_text.setPlainText(
-                    '\n    CTRL:'
-                    '\n    Deselect Nodes'
-                )
-            if self.SHIFT_state or self.CTRL_state:
-                self._cusor_text.setPos(self.mapToScene(self._previous_pos))
-                self._cusor_text.setVisible(True)
+                overlay_text = '\n    CTRL:\n    Deselect Nodes'
+        elif self.ALT_state and self.SHIFT_state:
+            if self.pipe_slicing:
+                overlay_text = '\n    ALT + SHIFT:\n    Pipe Slicer Enabled'
+        if overlay_text:
+            self._cusor_text.setPlainText(overlay_text)
+            self._cusor_text.setPos(self.mapToScene(self._previous_pos))
+            self._cusor_text.setVisible(True)
 
         super(NodeViewer, self).keyPressEvent(event)
 
     def keyReleaseEvent(self, event):
         """
         Key release event re-implemented to update the states for attributes:
         - ALT_state
```

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.5.9/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.5.8
+Version: 0.5.9
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.8 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.9 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.5.8/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.5.9/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/PKG-INFO` & `NodeGraphQt-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.5.8
+Version: 0.5.9
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.8 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.9 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.5.8/README.md` & `NodeGraphQt-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.5.9/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.5.9/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.5.9/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.5.9/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.8/setup.cfg` & `NodeGraphQt-0.5.9/setup.cfg`

 * *Files identical despite different names*

