# Comparing `tmp/cim_graph-0.1.20230420002327a0.tar.gz` & `tmp/cim_graph-0.1.20230508191837a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_graph-0.1.20230420002327a0.tar", max compression
+gzip compressed data, was "cim_graph-0.1.20230508191837a0.tar", max compression
```

## Comparing `cim_graph-0.1.20230420002327a0.tar` & `cim_graph-0.1.20230508191837a0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     4900 2023-04-20 00:22:35.436281 cim_graph-0.1.20230420002327a0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 00:22:35.436281 cim_graph-0.1.20230420002327a0/cimgraph/__init__.py
--rw-r--r--   0        0        0      105 2023-04-20 00:22:35.436281 cim_graph-0.1.20230420002327a0/cimgraph/data_profile/__init__.py
--rw-r--r--   0        0        0     9401 2023-04-20 00:22:35.436281 cim_graph-0.1.20230420002327a0/cimgraph/data_profile/cimext_2022/__init__.py
--rw-r--r--   0        0        0   370766 2023-04-20 00:22:35.436281 cim_graph-0.1.20230420002327a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
--rw-r--r--   0        0        0    24601 2023-04-20 00:22:35.436281 cim_graph-0.1.20230420002327a0/cimgraph/data_profile/rc4_2021/__init__.py
--rw-r--r--   0        0        0   835023 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
--rw-r--r--   0        0        0     1063 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/__init__.py
--rw-r--r--   0        0        0      353 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/blazegraph/__init__.py
--rw-r--r--   0        0        0     9114 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/blazegraph/blazegraph.py
--rw-r--r--   0        0        0     2797 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/blazegraph/query_parsers.py
--rw-r--r--   0        0        0    10318 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/gridappsd/__init__.py
--rw-r--r--   0        0        0     4226 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/__init__.py
--rw-r--r--   0        0        0     1492 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
--rw-r--r--   0        0        0     3711 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
--rw-r--r--   0        0        0     3156 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
--rw-r--r--   0        0        0     2646 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/analog.py
--rw-r--r--   0        0        0     1483 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/asset.py
--rw-r--r--   0        0        0      885 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py
--rw-r--r--   0        0        0     1491 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
--rw-r--r--   0        0        0     3141 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
--rw-r--r--   0        0        0     3046 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/breaker.py
--rw-r--r--   0        0        0     2795 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py
--rw-r--r--   0        0        0     5482 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
--rw-r--r--   0        0        0     2350 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py
--rw-r--r--   0        0        0     2672 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py
--rw-r--r--   0        0        0     2650 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/discrete.py
--rw-r--r--   0        0        0     3155 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
--rw-r--r--   0        0        0     2176 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
--rw-r--r--   0        0        0     2799 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/fuse.py
--rw-r--r--   0        0        0      995 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
--rw-r--r--   0        0        0     3961 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
--rw-r--r--   0        0        0     2973 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
--rw-r--r--   0        0        0     2881 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
--rw-r--r--   0        0        0     3615 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
--rw-r--r--   0        0        0     2446 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
--rw-r--r--   0        0        0     2585 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
--rw-r--r--   0        0        0     2444 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
--rw-r--r--   0        0        0     2831 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
--rw-r--r--   0        0        0     3956 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
--rw-r--r--   0        0        0     2101 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
--rw-r--r--   0        0        0     3294 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
--rw-r--r--   0        0        0     4090 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
--rw-r--r--   0        0        0     2366 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
--rw-r--r--   0        0        0     4137 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
--rw-r--r--   0        0        0     2813 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/recloser.py
--rw-r--r--   0        0        0     2668 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
--rw-r--r--   0        0        0     3314 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
--rw-r--r--   0        0        0     2801 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
--rw-r--r--   0        0        0     3015 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
--rw-r--r--   0        0        0     3688 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
--rw-r--r--   0        0        0     4996 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
--rw-r--r--   0        0        0     3020 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/terminal.py
--rw-r--r--   0        0        0     2415 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
--rw-r--r--   0        0        0     4452 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
--rw-r--r--   0        0        0     2648 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
--rw-r--r--   0        0        0     3122 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
--rw-r--r--   0        0        0     3765 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
--rw-r--r--   0        0        0     2604 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
--rw-r--r--   0        0        0     2280 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py
--rw-r--r--   0        0        0     2687 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
--rw-r--r--   0        0        0      386 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/models/__init__.py
--rw-r--r--   0        0        0     4116 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/models/distributed_model.py
--rw-r--r--   0        0        0     1715 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/models/model_parsers.py
--rw-r--r--   0        0        0     3167 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/models/secondary_area.py
--rw-r--r--   0        0        0     3734 2023-04-20 00:22:35.444281 cim_graph-0.1.20230420002327a0/cimgraph/models/switch_area.py
--rw-r--r--   0        0        0      757 2023-04-20 00:23:27.481356 cim_graph-0.1.20230420002327a0/pyproject.toml
--rw-r--r--   0        0        0     5569 1970-01-01 00:00:00.000000 cim_graph-0.1.20230420002327a0/PKG-INFO
+-rw-r--r--   0        0        0     4900 2023-05-08 19:17:43.657490 cim_graph-0.1.20230508191837a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 19:17:43.657490 cim_graph-0.1.20230508191837a0/cimgraph/__init__.py
+-rw-r--r--   0        0        0      105 2023-05-08 19:17:43.657490 cim_graph-0.1.20230508191837a0/cimgraph/data_profile/__init__.py
+-rw-r--r--   0        0        0     9401 2023-05-08 19:17:43.657490 cim_graph-0.1.20230508191837a0/cimgraph/data_profile/cimext_2022/__init__.py
+-rw-r--r--   0        0        0   370766 2023-05-08 19:17:43.657490 cim_graph-0.1.20230508191837a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
+-rw-r--r--   0        0        0    24601 2023-05-08 19:17:43.657490 cim_graph-0.1.20230508191837a0/cimgraph/data_profile/rc4_2021/__init__.py
+-rw-r--r--   0        0        0   835023 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
+-rw-r--r--   0        0        0     1063 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/__init__.py
+-rw-r--r--   0        0        0      353 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/blazegraph/__init__.py
+-rw-r--r--   0        0        0     9114 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/blazegraph/blazegraph.py
+-rw-r--r--   0        0        0     2797 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/blazegraph/query_parsers.py
+-rw-r--r--   0        0        0    10318 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4226 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/__init__.py
+-rw-r--r--   0        0        0     1492 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
+-rw-r--r--   0        0        0     3711 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
+-rw-r--r--   0        0        0     3156 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
+-rw-r--r--   0        0        0     2646 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/analog.py
+-rw-r--r--   0        0        0     1483 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/asset.py
+-rw-r--r--   0        0        0      885 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py
+-rw-r--r--   0        0        0     1491 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
+-rw-r--r--   0        0        0     3141 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
+-rw-r--r--   0        0        0     3046 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/breaker.py
+-rw-r--r--   0        0        0     2795 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py
+-rw-r--r--   0        0        0     5482 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
+-rw-r--r--   0        0        0     2350 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py
+-rw-r--r--   0        0        0     2672 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py
+-rw-r--r--   0        0        0     2650 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/discrete.py
+-rw-r--r--   0        0        0     3155 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
+-rw-r--r--   0        0        0     2176 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
+-rw-r--r--   0        0        0     2799 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/fuse.py
+-rw-r--r--   0        0        0      995 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
+-rw-r--r--   0        0        0     3961 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
+-rw-r--r--   0        0        0     2973 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
+-rw-r--r--   0        0        0     2881 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
+-rw-r--r--   0        0        0     3615 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
+-rw-r--r--   0        0        0     2446 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
+-rw-r--r--   0        0        0     2585 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
+-rw-r--r--   0        0        0     2444 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
+-rw-r--r--   0        0        0     2831 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
+-rw-r--r--   0        0        0     3956 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
+-rw-r--r--   0        0        0     2101 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
+-rw-r--r--   0        0        0     3294 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
+-rw-r--r--   0        0        0     4090 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
+-rw-r--r--   0        0        0     2366 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
+-rw-r--r--   0        0        0     4137 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
+-rw-r--r--   0        0        0     2813 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/recloser.py
+-rw-r--r--   0        0        0     2668 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
+-rw-r--r--   0        0        0     3314 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
+-rw-r--r--   0        0        0     2801 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
+-rw-r--r--   0        0        0     3015 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
+-rw-r--r--   0        0        0     3688 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
+-rw-r--r--   0        0        0     4996 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
+-rw-r--r--   0        0        0     3020 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/terminal.py
+-rw-r--r--   0        0        0     2415 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
+-rw-r--r--   0        0        0     4453 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
+-rw-r--r--   0        0        0     2648 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
+-rw-r--r--   0        0        0     3122 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
+-rw-r--r--   0        0        0     3765 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
+-rw-r--r--   0        0        0     2604 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
+-rw-r--r--   0        0        0     2280 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py
+-rw-r--r--   0        0        0     2687 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
+-rw-r--r--   0        0        0      386 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/models/__init__.py
+-rw-r--r--   0        0        0     4115 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/models/distributed_model.py
+-rw-r--r--   0        0        0     1715 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/models/model_parsers.py
+-rw-r--r--   0        0        0     3171 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/models/secondary_area.py
+-rw-r--r--   0        0        0     3737 2023-05-08 19:17:43.665490 cim_graph-0.1.20230508191837a0/cimgraph/models/switch_area.py
+-rw-r--r--   0        0        0      757 2023-05-08 19:18:37.809430 cim_graph-0.1.20230508191837a0/pyproject.toml
+-rw-r--r--   0        0        0     5569 1970-01-01 00:00:00.000000 cim_graph-0.1.20230508191837a0/PKG-INFO
```

### Comparing `cim_graph-0.1.20230420002327a0/README.md` & `cim_graph-0.1.20230508191837a0/README.md`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/data_profile/cimext_2022/__init__.py` & `cim_graph-0.1.20230508191837a0/cimgraph/data_profile/cimext_2022/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py` & `cim_graph-0.1.20230508191837a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/data_profile/rc4_2021/__init__.py` & `cim_graph-0.1.20230508191837a0/cimgraph/data_profile/rc4_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py` & `cim_graph-0.1.20230508191837a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/__init__.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/blazegraph/blazegraph.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/blazegraph/blazegraph.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/blazegraph/query_parsers.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/blazegraph/query_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/gridappsd/__init__.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/__init__.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/analog.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/analog.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/asset.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/asset.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/breaker.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/breaker.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/discrete.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/discrete.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/fuse.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/fuse.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/recloser.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/recloser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                   ?meas a ?meas_cls.
                   bind(concat(str(?meas_id),",",strafter(str(?meas_cls),"CIM100#")) as ?Measurement).}
 
         OPTIONAL {?eq cim:SwitchPhase.closed ?closed.}
         OPTIONAL {?eq cim:SwitchPhase.normalOpen ?normalOpen.}
         OPTIONAL {?eq cim:SwitchPhase.phaseSide1 ?phs1.
                  bind(strafter(str(?phs1),"SinglePhaseKind.") as ?phaseSide1)}
-        OPTIONAL {?eq cim:SwitchPhase.phaseSide1 ?phs2.
+        OPTIONAL {?eq cim:SwitchPhase.phaseSide2 ?phs2.
                  bind(strafter(str(?phs2),"SinglePhaseKind.") as ?phaseSide2)}
 
 		FILTER (regex(STR(?measphase), ?phaseSide1)  || regex(STR(?measphase), ?phaseSide2))
         
         }
         GROUP by ?mRID ?name ?Location ?Switch ?closed ?normalOpen ?phaseSide1 ?phaseSide2
```

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/terminal.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                   
         OPTIONAL {?esct cim:ShortCircuitTest.EnergisedEnd ?eq.
                   ?esct cim:IdentifiedObject.mRID ?EnergisedEndShortCircuitTests.}
                   
         OPTIONAL {?enol cim:NoLoadTest.EnergisedEnd ?eq.
                   ?enol cim:IdentifiedObject.mRID ?EnergisedEndNoLoadTests.}
                   
-        OPTIONAL {?tac cim:TransformerCoreAdmittace.TransformerEnd ?eq.
+        OPTIONAL {?tac cim:TransformerCoreAdmittance.TransformerEnd ?eq.
                   ?tac cim:IdentifiedObject.mRID ?CoreAdmittance.}
           
         OPTIONAL {?frmesh cim:TransformerMeshImpedance.FromTransformerEnd ?eq.
                   ?frmesh cim:IdentifiedObject.mRID ?FromMeshImpedance.}
           
         OPTIONAL {?frmesh cim:TransformerMeshImpedance.ToTransformerEnd ?eq.
                   ?frmesh cim:IdentifiedObject.mRID ?ToMeshImpedance.}
```

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py` & `cim_graph-0.1.20230508191837a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/models/distributed_model.py` & `cim_graph-0.1.20230508191837a0/cimgraph/models/distributed_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                                                               self.topology['connectivity_node'])
         for obj in conn_nodes:
             add_to_catalog(obj, self.connectivity_nodes)
             add_to_typed_catalog(obj, self.typed_catalog)
 
         # Initialize all CIM objects in a single switch area
         # def initialize_switch_areas(feeder_mrid) -> dict(str,object):
-        sa_index = -1
+        sa_index = 0
         for switch_msg in self.topology['switch_areas']:
             # Add switch area
             switch_area = SwitchArea(self.feeder.mRID + '.' + str(sa_index), self.connection)
             switch_area.initialize_switch_area(switch_msg)
             self.switch_areas.append(switch_area)
             # Add switch area unaddressable equipment to feeder unaddressable equipment
             self.unaddressable_equipment.update(switch_area.unaddressable_equipment)
```

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/models/model_parsers.py` & `cim_graph-0.1.20230508191837a0/cimgraph/models/model_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/models/secondary_area.py` & `cim_graph-0.1.20230508191837a0/cimgraph/models/secondary_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         for obj in unaddr_equip:
             add_to_catalog(obj, self.unaddressable_equipment)
             add_to_typed_catalog(obj, self.typed_catalog)
         conn_nodes = self.connection.create_default_instances(self.feeder_mrid, switch_msg['connectivity_node'])
         for obj in conn_nodes:
             add_to_catalog(obj, self.connectivity_nodes)
             add_to_typed_catalog(obj, self.typed_catalog)
-        xfmr = self.connection.create_default_instances(self.feeder_mrid, switch_msg['distribution_transformer'])
-        for obj in xfmr:
-            add_to_catalog(obj, self.distribution_transformer)
-            add_to_typed_catalog(obj, self.typed_catalog)
+#        xfmr = self.connection.create_default_instances(self.feeder_mrid, switch_msg['distribution_transformer'])
+#        for obj in xfmr:
+#            add_to_catalog(obj, self.distribution_transformer)
+#            add_to_typed_catalog(obj, self.typed_catalog)
             
     def get_all_attributes(self, cim_class):
         if cim_class in self.typed_catalog:
             self.connection.get_all_attributes(self.feeder_mrid, self.typed_catalog, cim_class)
         else:
             _log.info('no instances of '+str(cim_class.__name__)+' found in catalog.')
```

### Comparing `cim_graph-0.1.20230420002327a0/cimgraph/models/switch_area.py` & `cim_graph-0.1.20230508191837a0/cimgraph/models/switch_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,20 @@
         for obj in unaddr_equip:
             add_to_catalog(obj, self.unaddressable_equipment)
             add_to_typed_catalog(obj, self.typed_catalog)
         conn_nodes = self.connection.create_default_instances(self.feeder_mrid, switch_msg['connectivity_node'])
         for obj in conn_nodes:
             add_to_catalog(obj, self.connectivity_nodes)
             add_to_typed_catalog(obj, self.typed_catalog)
-        bound_sw = self.connection.create_default_instances(self.feeder_mrid, switch_msg['boundary_switches'])
-        for obj in bound_sw:
-            add_to_catalog(obj, self.boundary_switches)
-            add_to_typed_catalog(obj, self.typed_catalog)
+#        bound_sw = self.connection.create_default_instances(self.feeder_mrid, switch_msg['boundary_switches'])
+#        for obj in bound_sw:
+#            add_to_catalog(obj, self.boundary_switches)
+#            add_to_typed_catalog(obj, self.typed_catalog)
 
-        sa_index = -1
+        sa_index = 0
         for sec_area_msg in switch_msg['secondary_areas']:
             # Add switch area
             sec_area = SecondaryArea(self.area_id + '.' + str(sa_index), self.connection)
             sec_area.initialize_secondary_area(sec_area_msg)
             self.secondary_areas.append(sec_area)
             # Add switch area unaddressable equipment to feeder unaddressable equipment
             self.unaddressable_equipment.update(sec_area.unaddressable_equipment)
```

### Comparing `cim_graph-0.1.20230420002327a0/pyproject.toml` & `cim_graph-0.1.20230508191837a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cim-graph"
-version = "0.1.20230420002327a0"
+version = "0.1.20230508191837a0"
 description = "CIM Graph"
 authors = ["C. Allwardt <3979063+craig8@users.noreply.github.com>"]
 packages = [
     { include = "cimgraph" }
 ]
 readme = "README.md"
```

### Comparing `cim_graph-0.1.20230420002327a0/PKG-INFO` & `cim_graph-0.1.20230508191837a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-graph
-Version: 0.1.20230420002327a0
+Version: 0.1.20230508191837a0
 Summary: CIM Graph
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

