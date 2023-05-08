# Comparing `tmp/control-lab-ly-1.0.1a2.tar.gz` & `tmp/control-lab-ly-1.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.0.1a2.tar", last modified: Tue Apr 25 13:24:14 2023, max compression
+gzip compressed data, was "control-lab-ly-1.0.1a3.tar", last modified: Tue May  2 09:32:31 2023, max compression
```

## Comparing `control-lab-ly-1.0.1a2.tar` & `control-lab-ly-1.0.1a3.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.644784 control-lab-ly-1.0.1a2/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a2/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/MANIFEST.in
--rw-rw-rw-   0        0        0    17492 2023-04-25 13:24:14.652926 control-lab-ly-1.0.1a2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.753396 control-lab-ly-1.0.1a2/docs/
--rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.1a2/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a2/docs/LICENSE.md
--rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.0.1a2/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/pyproject.toml
--rw-rw-rw-   0        0        0     1560 2023-04-25 13:24:14.668124 control-lab-ly-1.0.1a2/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.1a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.466196 control-lab-ly-1.0.1a2/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.818597 control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    17492 2023-04-25 13:24:12.000000 control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7306 2023-04-25 13:24:12.000000 control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:24:12.000000 control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-04-25 13:24:12.000000 control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 13:24:12.000000 control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.832858 control-lab-ly-1.0.1a2/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.841312 control-lab-ly-1.0.1a2/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.844302 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.850282 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.905427 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.929300 control-lab-ly-1.0.1a2/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.952845 control-lab-ly-1.0.1a2/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:12.977862 control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.009514 control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    16662 2023-04-25 13:21:57.000000 control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a2/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.020471 control-lab-ly-1.0.1a2/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.119482 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15405 2023-04-25 13:07:43.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3767 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a2/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.174801 control-lab-ly-1.0.1a2/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.1a2/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.223352 control-lab-ly-1.0.1a2/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.234486 control-lab-ly-1.0.1a2/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10517 2023-04-21 14:30:09.000000 control-lab-ly-1.0.1a2/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.298788 control-lab-ly-1.0.1a2/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.325083 control-lab-ly-1.0.1a2/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.382258 control-lab-ly-1.0.1a2/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.458351 control-lab-ly-1.0.1a2/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.478287 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.524094 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.569360 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.593477 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.658791 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10329 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.711250 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.717229 control-lab-ly-1.0.1a2/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8427 2023-04-25 13:14:54.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.721507 control-lab-ly-1.0.1a2/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.748149 control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.773080 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.793071 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.817077 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15851 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.837863 control-lab-ly-1.0.1a2/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.856414 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.884966 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.911466 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29831 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.926321 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    30605 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.938302 control-lab-ly-1.0.1a2/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.947756 control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.956732 control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.979505 control-lab-ly-1.0.1a2/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:13.990696 control-lab-ly-1.0.1a2/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.008396 control-lab-ly-1.0.1a2/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.016353 control-lab-ly-1.0.1a2/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a2/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.056000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.056000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.183173 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.197551 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      310 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a2/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15591 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a2/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    15865 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a2/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.282251 control-lab-ly-1.0.1a2/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6551 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a2/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.296884 control-lab-ly-1.0.1a2/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.316904 control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.363401 control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.381529 control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-04-25 13:24:14.638421 control-lab-ly-1.0.1a2/tests/
--rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a2/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      585 2023-04-21 08:33:59.000000 control-lab-ly-1.0.1a2/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.1a2/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a2/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a2/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.522635 control-lab-ly-1.0.1a3/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a3/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/MANIFEST.in
+-rw-rw-rw-   0        0        0    17492 2023-05-02 09:32:31.530653 control-lab-ly-1.0.1a3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.006379 control-lab-ly-1.0.1a3/docs/
+-rw-rw-rw-   0        0        0     4263 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.1a3/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.1a3/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.0.1a3/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/pyproject.toml
+-rw-rw-rw-   0        0        0     1560 2023-05-02 09:32:31.530653 control-lab-ly-1.0.1a3/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.1a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:29.635697 control-lab-ly-1.0.1a3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.040899 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    17492 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7306 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 09:32:29.000000 control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.050378 control-lab-ly-1.0.1a3/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.050874 control-lab-ly-1.0.1a3/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.061383 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.079349 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.114659 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.131858 control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.142625 control-lab-ly-1.0.1a3/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.150637 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.174831 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17622 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a3/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.174831 control-lab-ly-1.0.1a3/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.248341 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      516 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0    17704 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     8608 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15405 2023-04-27 03:04:50.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3767 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.264326 control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.288326 control-lab-ly-1.0.1a3/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.304818 control-lab-ly-1.0.1a3/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10533 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.327661 control-lab-ly-1.0.1a3/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9118 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.347192 control-lab-ly-1.0.1a3/src/controllably/Make/Mixture/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.363650 control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9684 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.403965 control-lab-ly-1.0.1a3/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.435867 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.471799 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18015 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.516873 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.534963 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.570797 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10345 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.597459 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.650685 control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8427 2023-04-27 03:04:50.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.662413 control-lab-ly-1.0.1a3/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.700109 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3402 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.716482 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.747133 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.769957 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15883 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.779587 control-lab-ly-1.0.1a3/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.850288 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.909703 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.942686 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29855 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.969417 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    31524 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13186 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.979991 control-lab-ly-1.0.1a3/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:30.995994 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.017387 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.033391 control-lab-ly-1.0.1a3/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.049382 control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.080412 control-lab-ly-1.0.1a3/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.096990 control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.113028 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.122188 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.168105 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.184151 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      310 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15591 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    15865 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.232436 control-lab-ly-1.0.1a3/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6559 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.0.1a3/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.240816 control-lab-ly-1.0.1a3/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.257346 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.285558 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.337557 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-05-02 09:32:31.522635 control-lab-ly-1.0.1a3/tests/
+-rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.0.1a3/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      629 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.1a3/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      390 2023-05-02 09:30:40.000000 control-lab-ly-1.0.1a3/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-04-12 15:51:49.000000 control-lab-ly-1.0.1a3/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.1a3/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.0.1a2/LICENSE.md` & `control-lab-ly-1.0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/PKG-INFO` & `control-lab-ly-1.0.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
```

### Comparing `control-lab-ly-1.0.1a2/docs/CHANGELOG.md` & `control-lab-ly-1.0.1a3/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.0.1a3/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/docs/LICENSE.md` & `control-lab-ly-1.0.1a3/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/docs/README.md` & `control-lab-ly-1.0.1a3/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/setup.cfg` & `control-lab-ly-1.0.1a3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e31 2d61 320d 0a64 6573 6372 6970 7469  .1-a2..descripti
+00000030: 2e31 2d61 330d 0a64 6573 6372 6970 7469  .1-a3..descripti
 00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
 00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
 00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
 00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
 00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

### Comparing `control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
```

### Comparing `control-lab-ly-1.0.1a2/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.0.1a3/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.0.1a3/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         Align the tool tip to the target coordinates, while also considering any additional offset
 
         Args:
             coordinates (tuple[float]): target coordinates
             offset (tuple[float], optional): additional x,y,z offset from tool tip. Defaults to (0,0,0).
         """
         coordinates = np.array(coordinates) - np.array(offset)
-        if not self.mover.isFeasible(coordinates, transform=True, tool_offset=True):
+        if not self.mover.isFeasible(coordinates, transform_in=True, tool_offset=True):
             raise ValueError(f"Infeasible tool position! {coordinates}")
         self.mover.safeMoveTo(coordinates, ascent_speed=0.2*self.mover._speed_max, descent_speed=0.2*self.mover._speed_max)
         self.setFlag(at_rest=False)
         return
     
     def aspirateAt(self, 
         coordinates: tuple[float], 
@@ -184,16 +184,23 @@
             start_tip (Optional[str], optional): channel to use. Defaults to None.
             tip_length (float, optional): length of pipette tip. Defaults to 80.
             channel (Optional[int], optional): channel to use. Defaults to None.
         
         Returns:
             tuple[float]: coordinates of top of tip rack well
         """
+        if 'eject' not in dir(self.liquid):
+            raise AttributeError("`attachTip` and `attachTipAt` methods not available.")
+        if self.liquid.isTipOn():
+            raise RuntimeError("Please eject current tip before attaching new tip.")
+        
         if start_tip is not None:
             self.updateStartTip(start_tip=start_tip, slot=slot)
+        well = self.deck.at(slot).wells_list[-len(self.positions[slot])]
+        print(well.name)
         next_tip_location, tip_length = self.positions[slot].pop(0)
         return self.attachTipAt(next_tip_location, tip_length=tip_length, channel=channel)
     
     def attachTipAt(self, 
         coordinates: tuple[float], 
         tip_length: float = 80, 
         channel: Optional[int] = None
@@ -275,14 +282,24 @@
         Args:
             slot (str, optional): name of slot with bin. Defaults to 'bin'.
             channel (Optional[int], optional): channel to use. Defaults to None.
         
         Returns:
             tuple[float]: coordinates of top of bin well
         """
+        if 'eject' not in dir(self.liquid):
+            raise AttributeError("`ejectTip` and `ejectTipAt` methods not available.")
+        if not self.liquid.isTipOn():
+            tip_length = self.liquid.tip_length
+            tip_offset = np.array((0,0,-tip_length + self.liquid.tip_inset_mm))
+            self.mover.implement_offset = self.mover.implement_offset - tip_offset
+            self.liquid.tip_length = 0
+            self.liquid.setFlag(tip_on=False)
+            raise RuntimeError("There is currently no tip to eject.")
+        
         bin_location,_ = self.positions[slot][0]
         return self.ejectTipAt(bin_location, channel=channel)
     
     def ejectTipAt(self, coordinates:tuple[float], channel:Optional[int] = None) -> tuple[float]:
         """
         Eject the pipette tip at the specified location
 
@@ -393,14 +410,14 @@
         """
         wells_list = self.deck.at(slot).wells_list.copy()
         well_names = [well.name for well in wells_list]
         if start_tip not in well_names:
             print(f"Received: start_tip={start_tip}; slot={slot}")
             print("Please enter a compatible set of inputs.")
             return
-        self.positions[slot] = wells_list
+        self.positions[slot] = [(well.top, well.depth) for well in wells_list]
         for name in well_names:
             if name == start_tip:
                 break
             self.positions[slot].pop(0)
         return
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/GUI/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,19 +129,19 @@
         except ValueError:
             pass
         else:
             ready = (abs(self.set_point - self.temperature)<=self.tolerance)
             if not ready:
                 pass
             elif not self._stabilize_time:
-                self._stabilize_time = time.time()
+                self._stabilize_time = time.perf_counter()
                 print(response)
             elif self.flags['temperature_reached']:
                 pass
-            elif (self._power <= self.power_threshold) or (time.time()-self._stabilize_time >= self.stabilize_buffer_time):
+            elif (self._power <= self.power_threshold) or (time.perf_counter()-self._stabilize_time >= self.stabilize_buffer_time):
                 print(response)
                 self.setFlag(temperature_reached=True)
                 print(f"Temperature of {self.set_point}°C reached!")
             if self.flags['record']:
                 values = [now] + values
                 row = {k:v for k,v in zip(self._columns, values)}
                 # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Make/Light/led_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ### Methods
     - `setPower`: set power and duration for illumination
     """
     
     channel: int
     update_power: bool = field(default=False, init=False)
     _duration: int = field(default=0, init=False)
-    _end_time: float = field(default=time.time(), init=False)
+    _end_time: float = field(default=time.perf_counter(), init=False)
     _power: int = field(default=0, init=False)
     
     # Properties
     @property
     def power(self) -> int:
         return self._power
     @power.setter
@@ -138,15 +138,15 @@
     def getTimedChannels(self) -> list[int]:
         """
         Get channels that are still timed
 
         Returns:
             list[int]: list of channels that are still timed
         """
-        now = time.time()
+        now = time.perf_counter()
         self._timed_channels = [chn.channel for chn in self.channels.values() if (chn._end_time>now and chn._duration)]
         return self._timed_channels
     
     def isBusy(self) -> bool:
         """
         Checks and returns whether the LED array is still busy
 
@@ -271,15 +271,15 @@
         if not any([chn.update_power for chn in self.channels.values()]):
             return ''
         command = f"{';'.join([str(v) for v in self.getPower()])}\n"
         try:
             self.device.write(command.encode('utf-8'))
         except AttributeError:
             pass
-        now = time.time()
+        now = time.perf_counter()
         for chn in self.channels.values():
             if chn.update_power:
                 chn._end_time = now + chn._duration
                 chn.update_power = False
         if self.verbose:
             print(command)
         return command
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,20 +120,20 @@
             speed (int): spin speed in rpm
             time_s (int): spin time in seconds
         """
         self._write(speed)
         self.speed = speed
         print(f"Duration   (channel {self.channel}): {time_s}s")
         interval = 1
-        start_time = time.time()
+        start_time = time.perf_counter()
         while(True):
             time.sleep(0.1)
-            if (interval <= time.time() - start_time):
+            if (interval <= time.perf_counter() - start_time):
                 interval += 1
-            if (time_s <= time.time() - start_time):
+            if (time_s <= time.perf_counter() - start_time):
                 break
         self._write(0)
         self.speed = 0
         return
 
     # Protected method(s)
     def _connect(self, port:str, baudrate:int = 9600, timeout:int = 1):
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Make/make_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,20 +216,20 @@
         Returns:
             Union[str, tuple[str]]: response string, or list of response strings
         """
         command_code = command.split(',')[0].strip().upper()
         if command_code not in CommandCode._member_names_:
             raise Exception(f"Please select a valid command code from: {', '.join(CommandCode._member_names_)}")
         
-        start_time = time.time()
+        start_time = time.perf_counter()
         self._write(command)
         cache = []
         response = ''
         while response != 'OKC':
-            if timeout_s is not None and (time.time()-start_time) > timeout_s:
+            if timeout_s is not None and (time.perf_counter()-start_time) > timeout_s:
                 print('Timeout! Aborting run...')
                 break
             response = self._read()
             if command_code == 'GET' and len(response):
                 cache.append(response)
         self.setFlag(busy=False)
         time.sleep(0.1)
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/__init__.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -390,22 +390,22 @@
         """
         self.connection_details = {
             'ip_address': ip_address,
             'timeout': timeout
         }
         self.device = Device(None,None)
         try:
-            start_time = time.time()
+            start_time = time.perf_counter()
             dashboard = dobot_api_dashboard(ip_address, 29999)
-            if time.time() - start_time > timeout:
+            if time.perf_counter() - start_time > timeout:
                 raise Exception(f"Unable to connect to arm at {ip_address}")
             
-            start_time = time.time()
+            start_time = time.perf_counter()
             feedback = dobot_api_feedback(ip_address, 30003)
-            if time.time() - start_time > timeout:
+            if time.perf_counter() - start_time > timeout:
                 raise Exception(f"Unable to connect to arm at {ip_address}")
         except Exception as e:
             print(e)
         else:
             self.device = Device(dashboard, feedback)
             self.reset()
             self.dashboard.User(0)
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Move/move_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -793,27 +793,27 @@
             command (str): command string
             timeout_s (int, optional): duration to wait before timeout. Defaults to 2.
 
         Returns:
             str: response string
         """
         # self.connect()
-        start_time = time.time()
+        start_time = time.perf_counter()
         self._write(command)
         response = ''
         while not self._is_expected_reply(response):
             if not self.isConnected():
                 break
-            if time.time() - start_time > timeout_s:
+            if time.perf_counter() - start_time > timeout_s:
                 break
             response = self._read()
             if response == '__break__':
                 response = ''
                 break
-        # print(time.time() - start_time)
+        # print(time.perf_counter() - start_time)
         # self.disconnect()
         return response
 
     def _read(self) -> str:
         """
         Read response from device
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -541,1373 +541,1431 @@
 000021c0: 766f 6c75 6d65 203d 3d20 303a 0d0a 2020  volume == 0:..  
 000021d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
 000021e0: 2027 270d 0a20 2020 2020 2020 2070 7269   ''..        pri
 000021f0: 6e74 2866 2741 7370 6972 6174 696e 6720  nt(f'Aspirating 
 00002200: 7b76 6f6c 756d 657d 2075 4c2e 2e2e 2729  {volume} uL...')
 00002210: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
 00002220: 6173 7069 7261 7465 203d 2074 696d 652e  aspirate = time.
-00002230: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
-00002240: 7370 6565 6420 3d20 7365 6c66 2e73 7065  speed = self.spe
-00002250: 6564 2e75 7020 6966 2073 7065 6564 2069  ed.up if speed i
-00002260: 7320 4e6f 6e65 2065 6c73 6520 7370 6565  s None else spee
-00002270: 640d 0a20 2020 2020 2020 200d 0a20 2020  d..        ..   
-00002280: 2020 2020 2069 6620 7370 6565 6420 696e       if speed in
-00002290: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
-000022a0: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
-000022b0: 2020 6966 2073 7065 6564 2021 3d20 7365    if speed != se
-000022c0: 6c66 2e73 7065 6564 2e75 703a 0d0a 2020  lf.speed.up:..  
-000022d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000022e0: 6c66 2e73 6574 5370 6565 6428 7370 6565  lf.setSpeed(spee
-000022f0: 643d 7370 6565 642c 2075 703d 5472 7565  d=speed, up=True
-00002300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002310: 2020 2073 656c 662e 7370 6565 642e 7570     self.speed.up
-00002320: 203d 2073 7065 6564 0d0a 2020 2020 2020   = speed..      
-00002330: 2020 2020 2020 7374 6172 745f 6173 7069        start_aspi
-00002340: 7261 7465 203d 2074 696d 652e 7469 6d65  rate = time.time
-00002350: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00002360: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00002370: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
-00002380: 737d 2729 0d0a 2020 2020 2020 2020 2020  s}')..          
-00002390: 2020 6d6f 7665 5f74 696d 6520 3d20 7374    move_time = st
-000023a0: 6570 732a 7365 6c66 2e72 6573 6f6c 7574  eps*self.resolut
-000023b0: 696f 6e20 2f20 7370 6565 640d 0a20 2020  ion / speed..   
-000023c0: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
-000023d0: 6565 7028 6d6f 7665 5f74 696d 6529 0d0a  eep(move_time)..
-000023e0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-000023f0: 2072 6573 706f 6e73 6520 213d 2027 6f6b   response != 'ok
-00002400: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-00002410: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
-00002420: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
-00002430: 2020 200d 0a20 2020 2020 2020 2065 6c69     ..        eli
-00002440: 6620 7370 6565 6420 6e6f 7420 696e 2073  f speed not in s
-00002450: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
-00002460: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00002470: 7072 696e 7428 6622 5461 7267 6574 3a20  print(f"Target: 
-00002480: 7b76 6f6c 756d 657d 2075 4c20 6174 207b  {volume} uL at {
-00002490: 7370 6565 647d 2075 4c2f 732e 2e2e 2229  speed} uL/s...")
-000024a0: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-000024b0: 6565 645f 7061 7261 6d65 7465 7273 203d  eed_parameters =
-000024c0: 2073 656c 662e 5f63 616c 6375 6c61 7465   self._calculate
-000024d0: 5f73 7065 6564 5f70 6172 616d 6574 6572  _speed_parameter
-000024e0: 7328 766f 6c75 6d65 3d76 6f6c 756d 652c  s(volume=volume,
-000024f0: 2073 7065 6564 3d73 7065 6564 290d 0a20   speed=speed).. 
-00002500: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00002510: 2873 7065 6564 5f70 6172 616d 6574 6572  (speed_parameter
-00002520: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00002530: 7072 6573 6574 203d 2073 7065 6564 5f70  preset = speed_p
-00002540: 6172 616d 6574 6572 732e 7072 6573 6574  arameters.preset
-00002550: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00002560: 2070 7265 7365 7420 6973 204e 6f6e 653a   preset is None:
-00002570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002580: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
-00002590: 7272 6f72 2827 5461 7267 6574 2073 7065  rror('Target spe
-000025a0: 6564 206e 6f74 2070 6f73 7369 626c 652e  ed not possible.
-000025b0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-000025c0: 7365 6c66 2e73 6574 5370 6565 6428 7370  self.setSpeed(sp
-000025d0: 6565 643d 7072 6573 6574 2c20 7570 3d54  eed=preset, up=T
-000025e0: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-000025f0: 2020 7365 6c66 2e73 7065 6564 2e75 7020    self.speed.up 
-00002600: 3d20 7370 6565 640d 0a20 2020 2020 2020  = speed..       
-00002610: 2020 2020 2073 7461 7274 5f61 7370 6972       start_aspir
-00002620: 6174 6520 3d20 7469 6d65 2e74 696d 6528  ate = time.time(
-00002630: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-00002640: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
-00002650: 7073 5f6c 6566 7420 3d20 7374 6570 730d  ps_left = steps.
-00002660: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-00002670: 6179 203d 2073 7065 6564 5f70 6172 616d  ay = speed_param
-00002680: 6574 6572 732e 6465 6c61 790d 0a20 2020  eters.delay..   
-00002690: 2020 2020 2020 2020 2073 7465 705f 7369           step_si
-000026a0: 7a65 203d 2073 7065 6564 5f70 6172 616d  ze = speed_param
-000026b0: 6574 6572 732e 7374 6570 5f73 697a 650d  eters.step_size.
-000026c0: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-000026d0: 6572 7661 6c73 203d 2073 7065 6564 5f70  ervals = speed_p
-000026e0: 6172 616d 6574 6572 732e 696e 7465 7276  arameters.interv
-000026f0: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
-00002700: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00002710: 696e 7465 7276 616c 7329 3a0d 0a20 2020  intervals):..   
-00002720: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00002730: 7274 5f74 696d 6520 3d20 7469 6d65 2e74  rt_time = time.t
-00002740: 696d 6528 290d 0a20 2020 2020 2020 2020  ime()..         
-00002750: 2020 2020 2020 2073 7465 7020 3d20 7374         step = st
-00002760: 6570 5f73 697a 6520 6966 2028 692b 3120  ep_size if (i+1 
-00002770: 213d 2069 6e74 6572 7661 6c73 2920 656c  != intervals) el
-00002780: 7365 2073 7465 7073 5f6c 6566 740d 0a20  se steps_left.. 
-00002790: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000027a0: 6f76 655f 7469 6d65 203d 2073 7465 702a  ove_time = step*
-000027b0: 7365 6c66 2e72 6573 6f6c 7574 696f 6e20  self.resolution 
-000027c0: 2f20 7072 6573 6574 0d0a 2020 2020 2020  / preset..      
-000027d0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-000027e0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-000027f0: 2866 2752 497b 7374 6570 7d27 2c20 7265  (f'RI{step}', re
-00002800: 7375 6d65 5f66 6565 6462 6163 6b3d 4661  sume_feedback=Fa
-00002810: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
-00002820: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
-00002830: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
-00002840: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002850: 2020 2020 7072 696e 7428 2241 7370 6972      print("Aspir
-00002860: 6174 696f 6e20 6661 696c 6564 2229 0d0a  ation failed")..
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
-00002890: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
-000028a0: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
-000028b0: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
-000028c0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-000028d0: 696f 6e20 3d20 7469 6d65 2e74 696d 6528  ion = time.time(
-000028e0: 2920 2d20 7374 6172 745f 7469 6d65 0d0a  ) - start_time..
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 6966 2064 7572 6174 696f 6e20 3c20 2864  if duration < (d
-00002910: 656c 6179 2b6d 6f76 655f 7469 6d65 293a  elay+move_time):
-00002920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002930: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00002940: 2864 656c 6179 2b6d 6f76 655f 7469 6d65  (delay+move_time
-00002950: 2d64 7572 6174 696f 6e29 0d0a 2020 2020  -duration)..    
-00002960: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
-00002970: 5570 6461 7465 2076 616c 7565 730d 0a20  Update values.. 
-00002980: 2020 2020 2020 2070 7269 6e74 2866 2741         print(f'A
-00002990: 7370 6972 6174 696f 6e20 7469 6d65 3a20  spiration time: 
-000029a0: 7b74 696d 652e 7469 6d65 2829 2d73 7461  {time.time()-sta
-000029b0: 7274 5f61 7370 6972 6174 657d 7327 290d  rt_aspirate}s').
-000029c0: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
-000029d0: 6565 7028 7761 6974 290d 0a20 2020 2020  eep(wait)..     
-000029e0: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
-000029f0: 6f63 6375 7069 6564 3d46 616c 7365 2c20  occupied=False, 
-00002a00: 7061 7573 655f 6665 6564 6261 636b 3d46  pause_feedback=F
-00002a10: 616c 7365 290d 0a20 2020 2020 2020 2073  alse)..        s
-00002a20: 656c 662e 766f 6c75 6d65 202b 3d20 766f  elf.volume += vo
-00002a30: 6c75 6d65 0d0a 2020 2020 2020 2020 7365  lume..        se
-00002a40: 6c66 2e70 6f73 6974 696f 6e20 2b3d 2073  lf.position += s
-00002a50: 7465 7073 0d0a 2020 2020 2020 2020 6966  teps..        if
-00002a60: 2072 6561 6765 6e74 2069 7320 6e6f 7420   reagent is not 
-00002a70: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00002a80: 2020 2073 656c 662e 7265 6167 656e 7420     self.reagent 
-00002a90: 3d20 7265 6167 656e 740d 0a20 2020 2020  = reagent..     
-00002aa0: 2020 2069 6620 7061 7573 653a 0d0a 2020     if pause:..  
-00002ab0: 2020 2020 2020 2020 2020 696e 7075 7428            input(
-00002ac0: 2250 7265 7373 2027 456e 7465 7227 2074  "Press 'Enter' t
-00002ad0: 6f20 7072 6f63 6565 642e 2229 0d0a 2020  o proceed.")..  
-00002ae0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00002af0: 706f 6e73 650d 0a20 2020 200d 0a20 2020  ponse..    ..   
-00002b00: 2064 6566 2062 6c6f 776f 7574 2873 656c   def blowout(sel
-00002b10: 662c 2068 6f6d 653a 626f 6f6c 203d 2054  f, home:bool = T
-00002b20: 7275 652c 202a 2a6b 7761 7267 7329 202d  rue, **kwargs) -
-00002b30: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
-00002b40: 2222 220d 0a20 2020 2020 2020 2042 6c6f  """..        Blo
-00002b50: 776f 7574 206c 6971 7569 6420 6672 6f6d  wout liquid from
-00002b60: 2074 6970 0d0a 0d0a 2020 2020 2020 2020   tip....        
-00002b70: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00002b80: 2020 2068 6f6d 6520 2862 6f6f 6c2c 206f     home (bool, o
-00002b90: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
-00002ba0: 7220 746f 2072 6574 7572 6e20 706c 756e  r to return plun
-00002bb0: 6765 7220 746f 2068 6f6d 6520 706f 7369  ger to home posi
-00002bc0: 7469 6f6e 2e20 4465 6661 756c 7473 2074  tion. Defaults t
-00002bd0: 6f20 5472 7565 2e0d 0a0d 0a20 2020 2020  o True.....     
-00002be0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00002bf0: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
-00002c00: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
-00002c10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00002c20: 2020 2020 636f 6d6d 616e 6420 3d20 6627      command = f'
-00002c30: 5242 7b73 656c 662e 686f 6d65 5f70 6f73  RB{self.home_pos
-00002c40: 6974 696f 6e7d 2720 6966 2068 6f6d 6520  ition}' if home 
-00002c50: 656c 7365 2027 5242 270d 0a20 2020 2020  else 'RB'..     
-00002c60: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00002c70: 6c66 2e5f 7175 6572 7928 636f 6d6d 616e  lf._query(comman
-00002c80: 6429 0d0a 2020 2020 2020 2020 7365 6c66  d)..        self
-00002c90: 2e70 6f73 6974 696f 6e20 3d20 7365 6c66  .position = self
-00002ca0: 2e68 6f6d 655f 706f 7369 7469 6f6e 0d0a  .home_position..
-00002cb0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-00002cc0: 6570 2831 290d 0a20 2020 2020 2020 2072  ep(1)..        r
-00002cd0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002ce0: 2020 2020 0d0a 2020 2020 6465 6620 6469      ..    def di
-00002cf0: 7370 656e 7365 2873 656c 662c 200d 0a20  spense(self, .. 
-00002d00: 2020 2020 2020 2076 6f6c 756d 653a 2066         volume: f
-00002d10: 6c6f 6174 2c20 0d0a 2020 2020 2020 2020  loat, ..        
-00002d20: 7370 6565 643a 204f 7074 696f 6e61 6c5b  speed: Optional[
-00002d30: 666c 6f61 745d 203d 204e 6f6e 652c 200d  float] = None, .
-00002d40: 0a20 2020 2020 2020 2077 6169 743a 2069  .        wait: i
-00002d50: 6e74 203d 2030 2c20 0d0a 2020 2020 2020  nt = 0, ..      
-00002d60: 2020 7061 7573 653a 2062 6f6f 6c20 3d20    pause: bool = 
-00002d70: 4661 6c73 652c 200d 0a20 2020 2020 2020  False, ..       
-00002d80: 2062 6c6f 776f 7574 3a20 626f 6f6c 203d   blowout: bool =
-00002d90: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00002da0: 2062 6c6f 776f 7574 5f68 6f6d 653a 2062   blowout_home: b
-00002db0: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
-00002dc0: 2020 2020 2066 6f72 6365 5f64 6973 7065       force_dispe
-00002dd0: 6e73 653a 2062 6f6f 6c20 3d20 4661 6c73  nse: bool = Fals
-00002de0: 652c 200d 0a20 2020 2020 2020 202a 2a6b  e, ..        **k
-00002df0: 7761 7267 730d 0a20 2020 2029 202d 3e20  wargs..    ) -> 
-00002e00: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
-00002e10: 220d 0a20 2020 2020 2020 2044 6973 7065  "..        Dispe
-00002e20: 6e73 6520 6465 7369 7265 6420 766f 6c75  nse desired volu
-00002e30: 6d65 206f 6620 7265 6167 656e 740d 0a0d  me of reagent...
-00002e40: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00002e50: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
-00002e60: 6d65 2028 666c 6f61 7429 3a20 7461 7267  me (float): targ
-00002e70: 6574 2076 6f6c 756d 650d 0a20 2020 2020  et volume..     
-00002e80: 2020 2020 2020 2073 7065 6564 2028 4f70         speed (Op
-00002e90: 7469 6f6e 616c 5b66 6c6f 6174 5d2c 206f  tional[float], o
-00002ea0: 7074 696f 6e61 6c29 3a20 7370 6565 6420  ptional): speed 
-00002eb0: 746f 2064 6973 7065 6e73 6520 6174 2e20  to dispense at. 
-00002ec0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00002ed0: 2e0d 0a20 2020 2020 2020 2020 2020 2077  ...            w
-00002ee0: 6169 7420 2869 6e74 2c20 6f70 7469 6f6e  ait (int, option
-00002ef0: 616c 293a 2074 696d 6520 6465 6c61 7920  al): time delay 
-00002f00: 6166 7465 7220 6469 7370 656e 7365 2e20  after dispense. 
-00002f10: 4465 6661 756c 7473 2074 6f20 302e 0d0a  Defaults to 0...
-00002f20: 2020 2020 2020 2020 2020 2020 7061 7573              paus
-00002f30: 6520 2862 6f6f 6c2c 206f 7074 696f 6e61  e (bool, optiona
-00002f40: 6c29 3a20 7768 6574 6865 7220 746f 2070  l): whether to p
-00002f50: 6175 7365 2066 6f72 2075 7365 7220 696e  ause for user in
-00002f60: 7465 7276 656e 7469 6f6e 2e20 4465 6661  tervention. Defa
-00002f70: 756c 7473 2074 6f20 4661 6c73 652e 0d0a  ults to False...
-00002f80: 2020 2020 2020 2020 2020 2020 626c 6f77              blow
-00002f90: 6f75 7420 2862 6f6f 6c2c 206f 7074 696f  out (bool, optio
-00002fa0: 6e61 6c29 3a20 7768 6574 6865 7220 7065  nal): whether pe
-00002fb0: 7266 6f72 6d20 626c 6f77 6f75 742e 2044  rform blowout. D
-00002fc0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00002fd0: 2e0d 0a20 2020 2020 2020 2020 2020 2062  ...            b
-00002fe0: 6c6f 776f 7574 5f68 6f6d 6520 2862 6f6f  lowout_home (boo
-00002ff0: 6c2c 206f 7074 696f 6e61 6c29 3a20 7768  l, optional): wh
-00003000: 6574 6865 7220 746f 2072 6574 7572 6e20  ether to return 
-00003010: 7468 6520 706c 756e 6765 7220 686f 6d65  the plunger home
-00003020: 2061 6674 6572 2062 6c6f 776f 7574 2e20   after blowout. 
-00003030: 4465 6661 756c 7473 2074 6f20 5472 7565  Defaults to True
-00003040: 2e0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-00003050: 6f72 6365 5f64 6973 7065 6e73 6520 2862  orce_dispense (b
-00003060: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-00003070: 7768 6574 6865 7220 746f 2064 6973 7065  whether to dispe
-00003080: 6e73 6520 7265 6167 656e 7420 7265 6761  nse reagent rega
-00003090: 7264 6c65 7373 2e20 4465 6661 756c 7473  rdless. Defaults
-000030a0: 2074 6f20 4661 6c73 652e 0d0a 0d0a 2020   to False.....  
-000030b0: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
-000030c0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-000030d0: 4572 726f 723a 2052 6571 7569 7265 6420  Error: Required 
-000030e0: 6469 7370 656e 7365 2076 6f6c 756d 6520  dispense volume 
-000030f0: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
-00003100: 766f 6c75 6d65 2069 6e20 7469 700d 0a0d  volume in tip...
-00003110: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00003120: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00003130: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
-00003140: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
-00003150: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00003160: 6574 466c 6167 2870 6175 7365 5f66 6565  etFlag(pause_fee
-00003170: 6462 6163 6b3d 5472 7565 2c20 6f63 6375  dback=True, occu
-00003180: 7069 6564 3d54 7275 6529 0d0a 2020 2020  pied=True)..    
-00003190: 2020 2020 6966 2066 6f72 6365 5f64 6973      if force_dis
-000031a0: 7065 6e73 653a 0d0a 2020 2020 2020 2020  pense:..        
-000031b0: 2020 2020 766f 6c75 6d65 203d 206d 696e      volume = min
-000031c0: 2876 6f6c 756d 652c 2073 656c 662e 766f  (volume, self.vo
-000031d0: 6c75 6d65 290d 0a20 2020 2020 2020 2065  lume)..        e
-000031e0: 6c69 6620 766f 6c75 6d65 203e 2073 656c  lif volume > sel
-000031f0: 662e 766f 6c75 6d65 3a0d 0a20 2020 2020  f.volume:..     
-00003200: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00003210: 7565 4572 726f 7228 2752 6571 7569 7265  ueError('Require
-00003220: 6420 6469 7370 656e 7365 2076 6f6c 756d  d dispense volum
-00003230: 6520 6973 2067 7265 6174 6572 2074 6861  e is greater tha
-00003240: 6e20 766f 6c75 6d65 2069 6e20 7469 702e  n volume in tip.
-00003250: 2729 0d0a 2020 2020 2020 2020 7374 6570  ')..        step
-00003260: 7320 3d20 696e 7428 766f 6c75 6d65 202f  s = int(volume /
-00003270: 2073 656c 662e 7265 736f 6c75 7469 6f6e   self.resolution
-00003280: 290d 0a20 2020 2020 2020 2076 6f6c 756d  )..        volum
-00003290: 6520 3d20 7374 6570 7320 2a20 7365 6c66  e = steps * self
-000032a0: 2e72 6573 6f6c 7574 696f 6e0d 0a20 2020  .resolution..   
-000032b0: 2020 2020 2069 6620 766f 6c75 6d65 203d       if volume =
-000032c0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-000032d0: 2020 7265 7475 726e 2027 270d 0a20 2020    return ''..   
-000032e0: 2020 2020 2070 7269 6e74 2866 2744 6973       print(f'Dis
-000032f0: 7065 6e73 696e 6720 7b76 6f6c 756d 657d  pensing {volume}
-00003300: 2075 4c2e 2e2e 2729 0d0a 2020 2020 2020   uL...')..      
-00003310: 2020 7374 6172 745f 6469 7370 656e 7365    start_dispense
-00003320: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
-00003330: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
-00003340: 7365 6c66 2e73 7065 6564 2e64 6f77 6e20  self.speed.down 
-00003350: 6966 2073 7065 6564 2069 7320 4e6f 6e65  if speed is None
-00003360: 2065 6c73 6520 7370 6565 640d 0a0d 0a20   else speed.... 
-00003370: 2020 2020 2020 2069 6620 7370 6565 6420         if speed 
-00003380: 696e 2073 656c 662e 7370 6565 645f 7072  in self.speed_pr
-00003390: 6573 6574 733a 0d0a 2020 2020 2020 2020  esets:..        
-000033a0: 2020 2020 6966 2073 7065 6564 2021 3d20      if speed != 
-000033b0: 7365 6c66 2e73 7065 6564 2e64 6f77 6e3a  self.speed.down:
-000033c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000033d0: 2020 7365 6c66 2e73 6574 5370 6565 6428    self.setSpeed(
-000033e0: 7370 6565 643d 7370 6565 642c 2075 703d  speed=speed, up=
-000033f0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-00003400: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-00003410: 6564 2e64 6f77 6e20 3d20 7370 6565 640d  ed.down = speed.
-00003420: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-00003430: 7274 5f64 6973 7065 6e73 6520 3d20 7469  rt_dispense = ti
-00003440: 6d65 2e74 696d 6528 290d 0a20 2020 2020  me.time()..     
-00003450: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00003460: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
-00003470: 524f 7b73 7465 7073 7d27 290d 0a20 2020  RO{steps}')..   
-00003480: 2020 2020 2020 2020 206d 6f76 655f 7469           move_ti
-00003490: 6d65 203d 2073 7465 7073 2a73 656c 662e  me = steps*self.
-000034a0: 7265 736f 6c75 7469 6f6e 202f 2073 7065  resolution / spe
-000034b0: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
-000034c0: 7469 6d65 2e73 6c65 6570 286d 6f76 655f  time.sleep(move_
-000034d0: 7469 6d65 290d 0a20 2020 2020 2020 2020  time)..         
-000034e0: 2020 2023 2069 6620 7265 7370 6f6e 7365     # if response
-000034f0: 2021 3d20 276f 6b27 3a0d 0a20 2020 2020   != 'ok':..     
-00003500: 2020 2020 2020 2023 2020 2020 2072 6574         #     ret
-00003510: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
-00003520: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003530: 2020 2020 656c 6966 2073 7065 6564 206e      elif speed n
-00003540: 6f74 2069 6e20 7365 6c66 2e73 7065 6564  ot in self.speed
-00003550: 5f70 7265 7365 7473 3a0d 0a20 2020 2020  _presets:..     
-00003560: 2020 2020 2020 2070 7269 6e74 2866 2254         print(f"T
-00003570: 6172 6765 743a 207b 766f 6c75 6d65 7d20  arget: {volume} 
-00003580: 754c 2061 7420 7b73 7065 6564 7d20 754c  uL at {speed} uL
-00003590: 2f73 2e2e 2e22 290d 0a20 2020 2020 2020  /s...")..       
-000035a0: 2020 2020 2073 7065 6564 5f70 6172 616d       speed_param
-000035b0: 6574 6572 7320 3d20 7365 6c66 2e5f 6361  eters = self._ca
-000035c0: 6c63 756c 6174 655f 7370 6565 645f 7061  lculate_speed_pa
-000035d0: 7261 6d65 7465 7273 2876 6f6c 756d 653d  rameters(volume=
-000035e0: 766f 6c75 6d65 2c20 7370 6565 643d 7370  volume, speed=sp
-000035f0: 6565 6429 0d0a 2020 2020 2020 2020 2020  eed)..          
-00003600: 2020 7072 696e 7428 7370 6565 645f 7061    print(speed_pa
-00003610: 7261 6d65 7465 7273 290d 0a20 2020 2020  rameters)..     
-00003620: 2020 2020 2020 2070 7265 7365 7420 3d20         preset = 
-00003630: 7370 6565 645f 7061 7261 6d65 7465 7273  speed_parameters
-00003640: 2e70 7265 7365 740d 0a20 2020 2020 2020  .preset..       
-00003650: 2020 2020 2069 6620 7072 6573 6574 2069       if preset i
-00003660: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00003670: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-00003680: 756e 7469 6d65 4572 726f 7228 2754 6172  untimeError('Tar
-00003690: 6765 7420 7370 6565 6420 6e6f 7420 706f  get speed not po
-000036a0: 7373 6962 6c65 2e27 290d 0a20 2020 2020  ssible.')..     
-000036b0: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
-000036c0: 7065 6564 2873 7065 6564 3d70 7265 7365  peed(speed=prese
-000036d0: 742c 2075 703d 4661 6c73 6529 0d0a 2020  t, up=False)..  
-000036e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000036f0: 7065 6564 2e64 6f77 6e20 3d20 7370 6565  peed.down = spee
-00003700: 640d 0a20 2020 2020 2020 2020 2020 2073  d..            s
-00003710: 7461 7274 5f64 6973 7065 6e73 6520 3d20  tart_dispense = 
-00003720: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00003730: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00003740: 2020 2073 7465 7073 5f6c 6566 7420 3d20     steps_left = 
-00003750: 7374 6570 730d 0a20 2020 2020 2020 2020  steps..         
-00003760: 2020 2064 656c 6179 203d 2073 7065 6564     delay = speed
-00003770: 5f70 6172 616d 6574 6572 732e 6465 6c61  _parameters.dela
-00003780: 790d 0a20 2020 2020 2020 2020 2020 2073  y..            s
-00003790: 7465 705f 7369 7a65 203d 2073 7065 6564  tep_size = speed
-000037a0: 5f70 6172 616d 6574 6572 732e 7374 6570  _parameters.step
-000037b0: 5f73 697a 650d 0a20 2020 2020 2020 2020  _size..         
-000037c0: 2020 2069 6e74 6572 7661 6c73 203d 2073     intervals = s
-000037d0: 7065 6564 5f70 6172 616d 6574 6572 732e  peed_parameters.
-000037e0: 696e 7465 7276 616c 730d 0a20 2020 2020  intervals..     
-000037f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00003800: 7261 6e67 6528 696e 7465 7276 616c 7329  range(intervals)
-00003810: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003820: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
-00003830: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00003840: 2020 2020 2020 2020 2020 2020 2073 7465               ste
-00003850: 7020 3d20 7374 6570 5f73 697a 6520 6966  p = step_size if
-00003860: 2028 692b 3120 213d 2069 6e74 6572 7661   (i+1 != interva
-00003870: 6c73 2920 656c 7365 2073 7465 7073 5f6c  ls) else steps_l
-00003880: 6566 740d 0a20 2020 2020 2020 2020 2020  eft..           
-00003890: 2020 2020 206d 6f76 655f 7469 6d65 203d       move_time =
-000038a0: 2073 7465 702a 7365 6c66 2e72 6573 6f6c   step*self.resol
-000038b0: 7574 696f 6e20 2f20 7072 6573 6574 0d0a  ution / preset..
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-000038e0: 5f71 7565 7279 2866 2752 4f7b 7374 6570  _query(f'RO{step
-000038f0: 7d27 2c20 7265 7375 6d65 5f66 6565 6462  }', resume_feedb
-00003900: 6163 6b3d 4661 6c73 6529 0d0a 2020 2020  ack=False)..    
-00003910: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00003920: 2072 6573 706f 6e73 6520 213d 2027 6f6b   response != 'ok
-00003930: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-00003940: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
-00003950: 2244 6973 7065 6e73 6520 6661 696c 6564  "Dispense failed
-00003960: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00003970: 2020 2020 2320 2020 2020 7265 7475 726e      #     return
-00003980: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00003990: 2020 2020 2020 2020 2020 2073 7465 7073             steps
-000039a0: 5f6c 6566 7420 2d3d 2073 7465 700d 0a20  _left -= step.. 
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000039c0: 7572 6174 696f 6e20 3d20 7469 6d65 2e74  uration = time.t
-000039d0: 696d 6528 2920 2d20 7374 6172 745f 7469  ime() - start_ti
-000039e0: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-000039f0: 2020 2020 6966 2064 7572 6174 696f 6e20      if duration 
-00003a00: 3c20 2864 656c 6179 2b6d 6f76 655f 7469  < (delay+move_ti
-00003a10: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
-00003a20: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00003a30: 6c65 6570 2864 656c 6179 2b6d 6f76 655f  leep(delay+move_
-00003a40: 7469 6d65 2d64 7572 6174 696f 6e29 0d0a  time-duration)..
-00003a50: 0d0a 2020 2020 2020 2020 2320 5570 6461  ..        # Upda
-00003a60: 7465 2076 616c 7565 730d 0a20 2020 2020  te values..     
-00003a70: 2020 2070 7269 6e74 2866 2744 6973 7065     print(f'Dispe
-00003a80: 6e73 6520 7469 6d65 3a20 7b74 696d 652e  nse time: {time.
-00003a90: 7469 6d65 2829 2d73 7461 7274 5f64 6973  time()-start_dis
-00003aa0: 7065 6e73 657d 7327 290d 0a20 2020 2020  pense}s')..     
-00003ab0: 2020 2074 696d 652e 736c 6565 7028 7761     time.sleep(wa
-00003ac0: 6974 290d 0a20 2020 2020 2020 2073 656c  it)..        sel
-00003ad0: 662e 7365 7446 6c61 6728 6f63 6375 7069  f.setFlag(occupi
-00003ae0: 6564 3d46 616c 7365 2c20 7061 7573 655f  ed=False, pause_
-00003af0: 6665 6564 6261 636b 3d46 616c 7365 290d  feedback=False).
-00003b00: 0a20 2020 2020 2020 2073 656c 662e 766f  .        self.vo
-00003b10: 6c75 6d65 203d 206d 6178 2873 656c 662e  lume = max(self.
-00003b20: 766f 6c75 6d65 202d 2076 6f6c 756d 652c  volume - volume,
-00003b30: 2030 290d 0a20 2020 2020 2020 2073 656c   0)..        sel
-00003b40: 662e 706f 7369 7469 6f6e 202d 3d20 7374  f.position -= st
-00003b50: 6570 730d 0a20 2020 2020 2020 2069 6620  eps..        if 
-00003b60: 7365 6c66 2e76 6f6c 756d 6520 3d3d 2030  self.volume == 0
-00003b70: 2061 6e64 2062 6c6f 776f 7574 3a0d 0a20   and blowout:.. 
-00003b80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003b90: 626c 6f77 6f75 7428 686f 6d65 3d62 6c6f  blowout(home=blo
-00003ba0: 776f 7574 5f68 6f6d 6529 0d0a 2020 2020  wout_home)..    
-00003bb0: 2020 2020 6966 2070 6175 7365 3a0d 0a20      if pause:.. 
-00003bc0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-00003bd0: 2822 5072 6573 7320 2745 6e74 6572 2720  ("Press 'Enter' 
-00003be0: 746f 2070 726f 6365 6564 2e22 290d 0a20  to proceed.").. 
-00003bf0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00003c00: 7370 6f6e 7365 0d0a 2020 2020 0d0a 2020  sponse..    ..  
-00003c10: 2020 6465 6620 656a 6563 7428 7365 6c66    def eject(self
-00003c20: 2c20 686f 6d65 3a62 6f6f 6c20 3d20 5472  , home:bool = Tr
-00003c30: 7565 2920 2d3e 2073 7472 3a0d 0a20 2020  ue) -> str:..   
-00003c40: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00003c50: 2020 456a 6563 7420 7468 6520 7069 7065    Eject the pipe
-00003c60: 7474 6520 7469 700d 0a0d 0a20 2020 2020  tte tip....     
-00003c70: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-00003c80: 2020 2020 2020 686f 6d65 2028 626f 6f6c        home (bool
-00003c90: 2c20 6f70 7469 6f6e 616c 293a 2077 6865  , optional): whe
-00003ca0: 7468 6572 2074 6f20 7265 7475 726e 2070  ther to return p
-00003cb0: 6c75 6e67 6572 2074 6f20 686f 6d65 2070  lunger to home p
-00003cc0: 6f73 6974 696f 6e2e 2044 6566 6175 6c74  osition. Default
-00003cd0: 7320 746f 2054 7275 652e 0d0a 0d0a 2020  s to True.....  
-00003ce0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00003cf0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00003d00: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00003d10: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00003d20: 2020 2020 2020 2073 656c 662e 7265 6167         self.reag
-00003d30: 656e 7420 3d20 2727 0d0a 2020 2020 2020  ent = ''..      
-00003d40: 2020 636f 6d6d 616e 6420 3d20 6627 5245    command = f'RE
-00003d50: 7b73 656c 662e 686f 6d65 5f70 6f73 6974  {self.home_posit
-00003d60: 696f 6e7d 2720 6966 2068 6f6d 6520 656c  ion}' if home el
-00003d70: 7365 2027 5245 270d 0a20 2020 2020 2020  se 'RE'..       
-00003d80: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
-00003d90: 2e5f 7175 6572 7928 636f 6d6d 616e 6429  ._query(command)
-00003da0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00003db0: 6f73 6974 696f 6e20 3d20 7365 6c66 2e68  osition = self.h
-00003dc0: 6f6d 655f 706f 7369 7469 6f6e 2069 6620  ome_position if 
-00003dd0: 686f 6d65 2065 6c73 6520 300d 0a20 2020  home else 0..   
-00003de0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00003df0: 3129 0d0a 2020 2020 2020 2020 7265 7475  1)..        retu
-00003e00: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-00003e10: 200d 0a20 2020 2064 6566 2065 6d70 7479   ..    def empty
-00003e20: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-00003e30: 3a0d 0a20 2020 2020 2020 2022 2222 456d  :..        """Em
-00003e40: 7074 7920 7468 6520 7069 7065 7474 6522  pty the pipette"
-00003e50: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00003e60: 726e 2073 656c 662e 686f 6d65 2829 0d0a  rn self.home()..
-00003e70: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
-00003e80: 7443 6170 6163 6974 616e 6365 2873 656c  tCapacitance(sel
-00003e90: 6629 202d 3e20 556e 696f 6e5b 696e 742c  f) -> Union[int,
-00003ea0: 2073 7472 5d3a 0d0a 2020 2020 2020 2020   str]:..        
-00003eb0: 2222 220d 0a20 2020 2020 2020 2047 6574  """..        Get
-00003ec0: 2074 6865 2063 6170 6163 6974 616e 6365   the capacitance
-00003ed0: 2061 7320 6d65 6173 7572 6564 2061 7420   as measured at 
-00003ee0: 7468 6520 656e 6420 6f66 2074 6865 2070  the end of the p
-00003ef0: 6970 6574 7465 0d0a 2020 2020 2020 2020  ipette..        
-00003f00: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00003f10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00003f20: 556e 696f 6e5b 696e 742c 2073 7472 5d3a  Union[int, str]:
-00003f30: 2063 6170 6163 6974 616e 6365 2076 616c   capacitance val
-00003f40: 7565 2c20 6f72 2064 6576 6963 6520 7265  ue, or device re
-00003f50: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00003f60: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
-00003f70: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
-00003f80: 6572 7928 2744 4e27 290d 0a20 2020 2020  ery('DN')..     
-00003f90: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00003fa0: 2020 2020 2063 6170 6163 6974 616e 6365       capacitance
-00003fb0: 203d 2069 6e74 2872 6573 706f 6e73 6529   = int(response)
-00003fc0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00003fd0: 2056 616c 7565 4572 726f 723a 0d0a 2020   ValueError:..  
-00003fe0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003ff0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00004000: 2020 2073 656c 662e 5f63 6170 6163 6974     self._capacit
-00004010: 616e 6365 203d 2063 6170 6163 6974 616e  ance = capacitan
-00004020: 6365 0d0a 2020 2020 2020 2020 7265 7475  ce..        retu
-00004030: 726e 2063 6170 6163 6974 616e 6365 0d0a  rn capacitance..
-00004040: 200d 0a20 2020 2064 6566 2067 6574 4572   ..    def getEr
-00004050: 726f 7273 2873 656c 6629 202d 3e20 7374  rors(self) -> st
-00004060: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-00004070: 0a20 2020 2020 2020 2047 6574 2065 7272  .        Get err
-00004080: 6f72 7320 6672 6f6d 2074 6865 2064 6576  ors from the dev
-00004090: 6963 650d 0a0d 0a20 2020 2020 2020 2052  ice....        R
-000040a0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000040b0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-000040c0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000040d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000040e0: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
-000040f0: 7279 2827 4445 2729 0d0a 2020 2020 0d0a  ry('DE')..    ..
-00004100: 2020 2020 6465 6620 6765 7449 6e66 6f28      def getInfo(
-00004110: 7365 6c66 2c20 6d6f 6465 6c3a 204f 7074  self, model: Opt
-00004120: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00004130: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00004140: 4765 7420 6465 7461 696c 7320 6f66 2074  Get details of t
-00004150: 6865 2053 6172 746f 7269 7573 2070 6970  he Sartorius pip
-00004160: 6574 7465 206d 6f64 656c 2222 220d 0a20  ette model""".. 
-00004170: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
-00004180: 656c 662e 5f5f 6d6f 6465 6c5f 5f28 292e  elf.__model__().
-00004190: 7370 6c69 7428 272d 2729 5b30 5d20 6966  split('-')[0] if
-000041a0: 206d 6f64 656c 2069 7320 4e6f 6e65 2065   model is None e
-000041b0: 6c73 6520 6d6f 6465 6c0d 0a20 2020 2020  lse model..     
-000041c0: 2020 2069 6620 6d6f 6465 6c20 6e6f 7420     if model not 
-000041d0: 696e 204d 6f64 656c 496e 666f 2e5f 6d65  in ModelInfo._me
-000041e0: 6d62 6572 5f6e 616d 6573 5f3a 0d0a 2020  mber_names_:..  
-000041f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00004200: 6627 5265 6365 6976 6564 3a20 7b6d 6f64  f'Received: {mod
-00004210: 656c 7d27 290d 0a20 2020 2020 2020 2020  el}')..         
-00004220: 2020 206d 6f64 656c 203d 2027 4252 4c30     model = 'BRL0
-00004230: 270d 0a20 2020 2020 2020 2020 2020 2070  '..            p
-00004240: 7269 6e74 2866 2244 6566 6175 6c74 696e  rint(f"Defaultin
-00004250: 6720 746f 3a20 7b27 4252 4c30 277d 2229  g to: {'BRL0'}")
-00004260: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00004270: 696e 7428 6622 5661 6c69 6420 6d6f 6465  int(f"Valid mode
-00004280: 6c73 2061 7265 3a20 7b27 2c20 272e 6a6f  ls are: {', '.jo
-00004290: 696e 284d 6f64 656c 496e 666f 2e5f 6d65  in(ModelInfo._me
-000042a0: 6d62 6572 5f6e 616d 6573 5f29 7d22 290d  mber_names_)}").
-000042b0: 0a20 2020 2020 2020 2069 6e66 6f3a 204d  .        info: M
-000042c0: 6f64 656c 203d 204d 6f64 656c 496e 666f  odel = ModelInfo
-000042d0: 5b6d 6f64 656c 5d2e 7661 6c75 650d 0a20  [model].value.. 
-000042e0: 2020 2020 2020 2070 7269 6e74 2869 6e66         print(inf
-000042f0: 6f29 0d0a 2020 2020 2020 2020 7365 6c66  o)..        self
-00004300: 2e6d 6f64 656c 5f69 6e66 6f20 3d20 696e  .model_info = in
-00004310: 666f 0d0a 2020 2020 2020 2020 7365 6c66  fo..        self
-00004320: 2e63 6170 6163 6974 7920 3d20 696e 666f  .capacity = info
-00004330: 2e63 6170 6163 6974 790d 0a20 2020 2020  .capacity..     
-00004340: 2020 2073 656c 662e 6c69 6d69 7473 203d     self.limits =
-00004350: 2028 696e 666f 2e74 6970 5f65 6a65 6374   (info.tip_eject
-00004360: 5f70 6f73 6974 696f 6e2c 2069 6e66 6f2e  _position, info.
-00004370: 6d61 785f 706f 7369 7469 6f6e 290d 0a20  max_position).. 
-00004380: 2020 2020 2020 2073 656c 662e 7370 6565         self.spee
-00004390: 645f 7072 6573 6574 7320 3d20 696e 666f  d_presets = info
-000043a0: 2e70 7265 7365 745f 7370 6565 6473 0d0a  .preset_speeds..
-000043b0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-000043c0: 6564 2e75 7020 3d20 7365 6c66 2e73 7065  ed.up = self.spe
-000043d0: 6564 5f70 7265 7365 7473 5b73 656c 662e  ed_presets[self.
-000043e0: 7370 6565 645f 636f 6465 2e75 705d 0d0a  speed_code.up]..
-000043f0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-00004400: 6564 2e64 6f77 6e20 3d20 7365 6c66 2e73  ed.down = self.s
-00004410: 7065 6564 5f70 7265 7365 7473 5b73 656c  peed_presets[sel
-00004420: 662e 7370 6565 645f 636f 6465 2e64 6f77  f.speed_code.dow
-00004430: 6e5d 0d0a 2020 2020 2020 2020 7265 7475  n]..        retu
-00004440: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
-00004450: 6620 6765 7450 6f73 6974 696f 6e28 7365  f getPosition(se
-00004460: 6c66 2c20 2a2a 6b77 6172 6773 2920 2d3e  lf, **kwargs) ->
-00004470: 2069 6e74 3a0d 0a20 2020 2020 2020 2022   int:..        "
-00004480: 2222 4765 7420 7468 6520 6375 7272 656e  ""Get the curren
-00004490: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
-000044a0: 6520 7069 7065 7474 6522 2222 0d0a 2020  e pipette"""..  
-000044b0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-000044c0: 2073 656c 662e 5f71 7565 7279 2827 4450   self._query('DP
-000044d0: 2729 0d0a 2020 2020 2020 2020 7472 793a  ')..        try:
-000044e0: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-000044f0: 7369 7469 6f6e 203d 2069 6e74 2872 6573  sition = int(res
-00004500: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
-00004510: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00004520: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00004530: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
-00004540: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-00004550: 7369 7469 6f6e 203d 2070 6f73 6974 696f  sition = positio
-00004560: 6e0d 0a20 2020 2020 2020 2072 6574 7572  n..        retur
-00004570: 6e20 7365 6c66 2e70 6f73 6974 696f 6e0d  n self.position.
-00004580: 0a20 2020 2020 200d 0a20 2020 2064 6566  .      ..    def
-00004590: 2067 6574 5374 6174 7573 2873 656c 662c   getStatus(self,
-000045a0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
-000045b0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-000045c0: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
-000045d0: 2073 7461 7475 7320 6f66 2074 6865 2070   status of the p
-000045e0: 6970 6574 7465 0d0a 0d0a 2020 2020 2020  ipette....      
-000045f0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00004600: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
-00004610: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
-00004620: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004630: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00004640: 6c66 2e5f 7175 6572 7928 2744 5327 290d  lf._query('DS').
-00004650: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00004660: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-00004670: 7320 3d20 696e 7428 7265 7370 6f6e 7365  s = int(response
-00004680: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
-00004690: 7420 5661 6c75 6545 7272 6f72 3a0d 0a20  t ValueError:.. 
-000046a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000046b0: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
-000046c0: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
-000046d0: 6e6f 7420 696e 205b 5f73 7461 7475 732e  not in [_status.
-000046e0: 7661 6c75 6520 666f 7220 5f73 7461 7475  value for _statu
-000046f0: 7320 696e 2053 7461 7475 7343 6f64 655d  s in StatusCode]
-00004700: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00004710: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00004720: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004730: 2020 7365 6c66 2e5f 7374 6174 7573 5f63    self._status_c
-00004740: 6f64 6520 3d20 7374 6174 7573 0d0a 2020  ode = status..  
-00004750: 2020 2020 2020 6966 2073 7461 7475 7320        if status 
-00004760: 696e 205b 342c 362c 385d 3a0d 0a20 2020  in [4,6,8]:..   
-00004770: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00004780: 7446 6c61 6728 6275 7379 3d54 7275 6529  tFlag(busy=True)
-00004790: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000047a0: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 7072 696e 7428 5374 6174 7573 436f 6465  print(StatusCode
-000047d0: 2873 7461 7475 7329 2e6e 616d 6529 0d0a  (status).name)..
-000047e0: 2020 2020 2020 2020 656c 6966 2073 7461          elif sta
-000047f0: 7475 7320 3d3d 2030 3a0d 0a20 2020 2020  tus == 0:..     
-00004800: 2020 2020 2020 2073 656c 662e 7365 7446         self.setF
-00004810: 6c61 6728 6275 7379 3d46 616c 7365 290d  lag(busy=False).
-00004820: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004830: 5374 6174 7573 436f 6465 2873 656c 662e  StatusCode(self.
-00004840: 5f73 7461 7475 735f 636f 6465 292e 6e61  _status_code).na
-00004850: 6d65 0d0a 2020 2020 0d0a 2020 2020 6465  me..    ..    de
-00004860: 6620 686f 6d65 2873 656c 6629 202d 3e20  f home(self) -> 
-00004870: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
-00004880: 220d 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
-00004890: 6e20 706c 756e 6765 7220 746f 2068 6f6d  n plunger to hom
-000048a0: 6520 706f 7369 7469 6f6e 0d0a 2020 2020  e position..    
-000048b0: 2020 2020 0d0a 2020 2020 2020 2020 5265      ..        Re
-000048c0: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-000048d0: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
-000048e0: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-000048f0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00004900: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00004910: 7175 6572 7928 6627 5250 7b73 656c 662e  query(f'RP{self.
-00004920: 686f 6d65 5f70 6f73 6974 696f 6e7d 2729  home_position}')
-00004930: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
-00004940: 6f6c 756d 6520 3d20 300d 0a20 2020 2020  olume = 0..     
-00004950: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00004960: 203d 2073 656c 662e 686f 6d65 5f70 6f73   = self.home_pos
-00004970: 6974 696f 6e0d 0a20 2020 2020 2020 2074  ition..        t
-00004980: 696d 652e 736c 6565 7028 3129 0d0a 2020  ime.sleep(1)..  
-00004990: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000049a0: 706f 6e73 650d 0a20 2020 200d 0a20 2020  ponse..    ..   
-000049b0: 2064 6566 2069 7346 6561 7369 626c 6528   def isFeasible(
-000049c0: 7365 6c66 2c20 706f 7369 7469 6f6e 3a69  self, position:i
-000049d0: 6e74 2920 2d3e 2062 6f6f 6c3a 0d0a 2020  nt) -> bool:..  
-000049e0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000049f0: 2020 2043 6865 636b 7320 616e 6420 7265     Checks and re
-00004a00: 7475 726e 7320 7768 6574 6865 7220 7468  turns whether th
-00004a10: 6520 706c 756e 6765 7220 706f 7369 7469  e plunger positi
-00004a20: 6f6e 2069 7320 6665 6173 6962 6c65 0d0a  on is feasible..
-00004a30: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-00004a40: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
-00004a50: 6974 696f 6e20 2869 6e74 293a 2070 6c75  ition (int): plu
-00004a60: 6e67 6572 2070 6f73 6974 696f 6e0d 0a0d  nger position...
-00004a70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004a80: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
-00004a90: 6f6f 6c3a 2077 6865 7468 6572 2070 6c75  ool: whether plu
-00004aa0: 6e67 6572 2070 6f73 6974 696f 6e20 6973  nger position is
-00004ab0: 2066 6561 7369 626c 650d 0a20 2020 2020   feasible..     
-00004ac0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004ad0: 6966 2028 7365 6c66 2e6c 696d 6974 735b  if (self.limits[
-00004ae0: 305d 203c 3d20 706f 7369 7469 6f6e 203c  0] <= position <
-00004af0: 3d20 7365 6c66 2e6c 696d 6974 735b 315d  = self.limits[1]
-00004b00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004b10: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00004b20: 2020 2020 2070 7269 6e74 2866 2252 616e       print(f"Ran
-00004b30: 6765 206c 696d 6974 7320 7265 6163 6865  ge limits reache
-00004b40: 6421 207b 7365 6c66 2e6c 696d 6974 737d  d! {self.limits}
-00004b50: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00004b60: 726e 2046 616c 7365 0d0a 2020 2020 0d0a  rn False..    ..
-00004b70: 2020 2020 6465 6620 6973 5469 704f 6e28      def isTipOn(
-00004b80: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0d0a  self) -> bool:..
-00004b90: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004ba0: 2020 2020 2043 6865 636b 7320 616e 6420       Checks and 
-00004bb0: 7265 7475 726e 7320 7768 6574 6865 7220  returns whether 
-00004bc0: 6120 7069 7065 7474 6520 7469 7020 6973  a pipette tip is
-00004bd0: 2061 7474 6163 6865 640d 0a20 2020 2020   attached..     
-00004be0: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
-00004bf0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00004c00: 2020 2062 6f6f 6c3a 2077 6865 7468 6572     bool: whether
-00004c10: 2061 2070 6970 6574 7465 2074 6970 2069   a pipette tip i
-00004c20: 6e20 6174 7461 6368 6564 0d0a 2020 2020  n attached..    
-00004c30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00004c40: 2073 656c 662e 6765 7443 6170 6163 6974   self.getCapacit
-00004c50: 616e 6365 2829 0d0a 2020 2020 2020 2020  ance()..        
-00004c60: 7072 696e 7428 6627 5469 7020 6361 7061  print(f'Tip capa
-00004c70: 6369 7461 6e63 653a 207b 7365 6c66 2e63  citance: {self.c
-00004c80: 6170 6163 6974 616e 6365 7d27 290d 0a20  apacitance}').. 
-00004c90: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
-00004ca0: 6c61 6773 5b27 636f 6e64 7563 7469 7665  lags['conductive
-00004cb0: 5f74 6970 7327 5d3a 0d0a 2020 2020 2020  _tips']:..      
-00004cc0: 2020 2020 2020 7469 705f 6f6e 203d 2028        tip_on = (
-00004cd0: 7365 6c66 2e63 6170 6163 6974 616e 6365  self.capacitance
-00004ce0: 203e 2073 656c 662e 7469 705f 7468 7265   > self.tip_thre
-00004cf0: 7368 6f6c 6429 0d0a 2020 2020 2020 2020  shold)..        
-00004d00: 2020 2020 7365 6c66 2e73 6574 466c 6167      self.setFlag
-00004d10: 2874 6970 5f6f 6e3d 7469 705f 6f6e 290d  (tip_on=tip_on).
-00004d20: 0a20 2020 2020 2020 2074 6970 5f6f 6e20  .        tip_on 
-00004d30: 3d20 7365 6c66 2e66 6c61 6773 5b27 7469  = self.flags['ti
-00004d40: 705f 6f6e 275d 0d0a 2020 2020 2020 2020  p_on']..        
-00004d50: 7265 7475 726e 2074 6970 5f6f 6e0d 0a20  return tip_on.. 
-00004d60: 2020 200d 0a20 2020 2064 6566 206d 6f76     ..    def mov
-00004d70: 6528 7365 6c66 2c20 7374 6570 733a 696e  e(self, steps:in
-00004d80: 742c 2075 703a 626f 6f6c 2c20 2a2a 6b77  t, up:bool, **kw
-00004d90: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
-00004da0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00004db0: 2020 2020 4d6f 7665 2074 6865 2070 6c75      Move the plu
-00004dc0: 6e67 6572 2065 6974 6865 7220 7570 206f  nger either up o
-00004dd0: 7220 646f 776e 2062 7920 6120 7370 6563  r down by a spec
-00004de0: 6966 6965 6420 6e75 6d62 6572 206f 6620  ified number of 
-00004df0: 7374 6570 730d 0a0d 0a20 2020 2020 2020  steps....       
-00004e00: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00004e10: 2020 2020 7374 6570 7320 2869 6e74 293a      steps (int):
-00004e20: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
-00004e30: 2074 6f20 6d6f 7665 2070 6c75 6e67 6572   to move plunger
-00004e40: 2062 790d 0a20 2020 2020 2020 2020 2020   by..           
-00004e50: 2075 7020 2862 6f6f 6c29 3a20 7768 6574   up (bool): whet
-00004e60: 6865 7220 746f 206d 6f76 6520 7468 6520  her to move the 
-00004e70: 706c 756e 6765 7220 7570 0d0a 0d0a 2020  plunger up....  
-00004e80: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00004e90: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00004ea0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00004eb0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00004ec0: 2020 2020 2020 2073 7465 7073 203d 2061         steps = a
-00004ed0: 6273 2873 7465 7073 2920 6966 2075 7020  bs(steps) if up 
-00004ee0: 656c 7365 202d 6162 7328 7374 6570 7329  else -abs(steps)
-00004ef0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00004f00: 2073 656c 662e 6d6f 7665 4279 2873 7465   self.moveBy(ste
-00004f10: 7073 290d 0a20 2020 200d 0a20 2020 2064  ps)..    ..    d
-00004f20: 6566 206d 6f76 6542 7928 7365 6c66 2c20  ef moveBy(self, 
-00004f30: 7374 6570 733a 696e 742c 202a 2a6b 7761  steps:int, **kwa
-00004f40: 7267 7329 202d 3e20 7374 723a 0d0a 2020  rgs) -> str:..  
-00004f50: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004f60: 2020 204d 6f76 6520 7468 6520 706c 756e     Move the plun
-00004f70: 6765 7220 6279 2073 7065 6369 6669 6564  ger by specified
-00004f80: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
-00004f90: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
-00004fa0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00004fb0: 7465 7073 2028 696e 7429 3a20 6e75 6d62  teps (int): numb
-00004fc0: 6572 206f 6620 7374 6570 7320 746f 206d  er of steps to m
-00004fd0: 6f76 6520 706c 756e 6765 7220 6279 2028  ove plunger by (
-00004fe0: 3c30 3a20 6d6f 7665 2064 6f77 6e2f 6469  <0: move down/di
-00004ff0: 7370 656e 7365 3b20 3e30 206d 6f76 6520  spense; >0 move 
-00005000: 7570 2f61 7370 6972 6174 6529 0d0a 0d0a  up/aspirate)....
-00005010: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00005020: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00005030: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
-00005040: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
-00005050: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00005060: 203d 2066 2752 497b 7374 6570 737d 2720   = f'RI{steps}' 
-00005070: 6966 2073 7465 7073 203e 2030 2065 6c73  if steps > 0 els
-00005080: 6520 6627 524f 7b2d 7374 6570 737d 270d  e f'RO{-steps}'.
-00005090: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-000050a0: 7369 7469 6f6e 202b 3d20 7374 6570 730d  sition += steps.
-000050b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000050c0: 7365 6c66 2e5f 7175 6572 7928 636f 6d6d  self._query(comm
-000050d0: 616e 6429 0d0a 2020 2020 0d0a 2020 2020  and)..    ..    
-000050e0: 6465 6620 6d6f 7665 546f 2873 656c 662c  def moveTo(self,
-000050f0: 2070 6f73 6974 696f 6e3a 696e 742c 202a   position:int, *
-00005100: 2a6b 7761 7267 7329 202d 3e20 7374 723a  *kwargs) -> str:
-00005110: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005120: 2020 2020 2020 204d 6f76 6520 7468 6520         Move the 
-00005130: 706c 756e 6765 7220 746f 2061 2073 7065  plunger to a spe
-00005140: 6369 6669 6564 2070 6f73 6974 696f 6e0d  cified position.
-00005150: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00005160: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-00005170: 7369 7469 6f6e 2028 696e 7429 3a20 7461  sition (int): ta
-00005180: 7267 6574 2070 6c75 6e67 6572 2070 6f73  rget plunger pos
-00005190: 6974 696f 6e0d 0a0d 0a20 2020 2020 2020  ition....       
-000051a0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-000051b0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
-000051c0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
-000051d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000051e0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-000051f0: 3d20 706f 7369 7469 6f6e 0d0a 2020 2020  = position..    
-00005200: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00005210: 5f71 7565 7279 2866 2752 507b 706f 7369  _query(f'RP{posi
-00005220: 7469 6f6e 7d27 290d 0a20 2020 200d 0a20  tion}')..    .. 
-00005230: 2020 2064 6566 2070 756c 6c62 6163 6b28     def pullback(
-00005240: 7365 6c66 2c20 7374 6570 733a 696e 7420  self, steps:int 
-00005250: 3d20 352c 202a 2a6b 7761 7267 7329 202d  = 5, **kwargs) -
-00005260: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
-00005270: 2222 220d 0a20 2020 2020 2020 2050 756c  """..        Pul
-00005280: 6c62 6163 6b20 6c69 7175 6964 2066 726f  lback liquid fro
-00005290: 6d20 7469 700d 0a20 2020 2020 2020 200d  m tip..        .
-000052a0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-000052b0: 2020 2020 2020 2020 2020 2020 7374 6570              step
-000052c0: 7320 2869 6e74 2c20 6f70 7469 6f6e 616c  s (int, optional
-000052d0: 293a 206e 756d 6265 7220 6f66 2073 7465  ): number of ste
-000052e0: 7073 2074 6f20 7075 6c6c 6261 636b 2e20  ps to pullback. 
-000052f0: 4465 6661 756c 7473 2074 6f20 352e 0d0a  Defaults to 5...
-00005300: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00005310: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005320: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
-00005330: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
-00005340: 220d 0a20 2020 2020 2020 2072 6573 706f  "..        respo
-00005350: 6e73 6520 3d20 7365 6c66 2e5f 7175 6572  nse = self._quer
-00005360: 7928 6627 5249 7b73 7465 7073 7d27 290d  y(f'RI{steps}').
-00005370: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-00005380: 7369 7469 6f6e 202b 3d20 7374 6570 730d  sition += steps.
-00005390: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
-000053a0: 6565 7028 3129 0d0a 2020 2020 2020 2020  eep(1)..        
-000053b0: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
-000053c0: 0a20 2020 200d 0a20 2020 2064 6566 2072  .    ..    def r
-000053d0: 6573 6574 2873 656c 6629 202d 3e20 7374  eset(self) -> st
-000053e0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-000053f0: 0a20 2020 2020 2020 2052 6573 6574 2074  .        Reset t
-00005400: 6865 2070 6970 6574 7465 0d0a 0d0a 2020  he pipette....  
-00005410: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005420: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00005430: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00005440: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005450: 2020 2020 2020 2073 656c 662e 7a65 726f         self.zero
-00005460: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
-00005470: 726e 2073 656c 662e 686f 6d65 2829 0d0a  rn self.home()..
-00005480: 2020 2020 0d0a 2020 2020 6465 6620 7365      ..    def se
-00005490: 7453 7065 6564 2873 656c 662c 2073 7065  tSpeed(self, spe
-000054a0: 6564 3a69 6e74 2c20 7570 3a62 6f6f 6c2c  ed:int, up:bool,
-000054b0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
-000054c0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-000054d0: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
-000054e0: 2073 7065 6564 206f 6620 7468 6520 706c   speed of the pl
-000054f0: 756e 6765 720d 0a0d 0a20 2020 2020 2020  unger....       
-00005500: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00005510: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
-00005520: 2073 7065 6564 206f 6620 706c 756e 6765   speed of plunge
-00005530: 720d 0a20 2020 2020 2020 2020 2020 2075  r..            u
-00005540: 7020 2862 6f6f 6c29 3a20 6469 7265 6374  p (bool): direct
-00005550: 696f 6e20 6f66 2074 7261 7665 6c0d 0a0d  ion of travel...
-00005560: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00005570: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00005580: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
-00005590: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
-000055a0: 0d0a 2020 2020 2020 2020 7370 6565 645f  ..        speed_
-000055b0: 636f 6465 203d 2031 202b 205b 7820 666f  code = 1 + [x fo
-000055c0: 7220 782c 7661 6c20 696e 2065 6e75 6d65  r x,val in enume
-000055d0: 7261 7465 286e 702e 6172 7261 7928 7365  rate(np.array(se
-000055e0: 6c66 2e73 7065 6564 5f70 7265 7365 7473  lf.speed_presets
-000055f0: 292d 7370 6565 6429 2069 6620 7661 6c20  )-speed) if val 
-00005600: 3e3d 2030 5d5b 305d 0d0a 2020 2020 2020  >= 0][0]..      
-00005610: 2020 7072 696e 7428 6627 5370 6565 6420    print(f'Speed 
-00005620: 7b73 7065 6564 5f63 6f64 657d 3a20 7b73  {speed_code}: {s
-00005630: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
-00005640: 735b 7370 6565 645f 636f 6465 2d31 5d7d  s[speed_code-1]}
-00005650: 2075 4c2f 7327 290d 0a20 2020 2020 2020   uL/s')..       
-00005660: 2064 6972 6563 7469 6f6e 203d 2027 4927   direction = 'I'
-00005670: 2069 6620 7570 2065 6c73 6520 274f 270d   if up else 'O'.
-00005680: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
-00005690: 7565 7279 2866 2753 7b64 6972 6563 7469  uery(f'S{directi
-000056a0: 6f6e 7d7b 7370 6565 645f 636f 6465 7d27  on}{speed_code}'
-000056b0: 290d 0a20 2020 2020 2020 2069 6620 7570  )..        if up
-000056c0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000056d0: 656c 662e 7370 6565 645f 636f 6465 2e75  elf.speed_code.u
-000056e0: 7020 3d20 7370 6565 645f 636f 6465 0d0a  p = speed_code..
-000056f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00005700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005710: 7370 6565 645f 636f 6465 2e64 6f77 6e20  speed_code.down 
-00005720: 3d20 7370 6565 645f 636f 6465 0d0a 2020  = speed_code..  
-00005730: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005740: 662e 5f71 7565 7279 2866 2744 7b64 6972  f._query(f'D{dir
-00005750: 6563 7469 6f6e 7d27 290d 0a20 2020 200d  ection}')..    .
-00005760: 0a20 2020 2064 6566 2073 6875 7464 6f77  .    def shutdow
-00005770: 6e28 7365 6c66 293a 0d0a 2020 2020 2020  n(self):..      
-00005780: 2020 2222 2253 6875 7464 6f77 6e20 7072    """Shutdown pr
-00005790: 6f63 6564 7572 6520 666f 7220 746f 6f6c  ocedure for tool
-000057a0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-000057b0: 662e 746f 6767 6c65 4665 6564 6261 636b  f.toggleFeedback
-000057c0: 4c6f 6f70 286f 6e3d 4661 6c73 6529 0d0a  Loop(on=False)..
-000057d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000057e0: 7570 6572 2829 2e73 6875 7464 6f77 6e28  uper().shutdown(
-000057f0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
-00005800: 2074 6f67 676c 6546 6565 6462 6163 6b4c   toggleFeedbackL
-00005810: 6f6f 7028 7365 6c66 2c20 6f6e 3a62 6f6f  oop(self, on:boo
-00005820: 6c29 3a0d 0a20 2020 2020 2020 2022 2222  l):..        """
-00005830: 0d0a 2020 2020 2020 2020 5374 6172 7420  ..        Start 
-00005840: 6f72 2073 746f 7020 6665 6564 6261 636b  or stop feedback
-00005850: 206c 6f6f 700d 0a20 2020 2020 2020 200d   loop..        .
-00005860: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00005870: 2020 2020 2020 2020 2020 2020 6f6e 2028              on (
-00005880: 626f 6f6c 293a 2077 6865 7468 6572 2074  bool): whether t
-00005890: 6f20 7374 6172 7420 6665 6564 6261 636b  o start feedback
-000058a0: 206c 6f6f 700d 0a20 2020 2020 2020 2022   loop..        "
-000058b0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-000058c0: 2e73 6574 466c 6167 2867 6574 5f66 6565  .setFlag(get_fee
-000058d0: 6462 6163 6b3d 6f6e 290d 0a20 2020 2020  dback=on)..     
-000058e0: 2020 2069 6620 6f6e 3a0d 0a20 2020 2020     if on:..     
-000058f0: 2020 2020 2020 2069 6620 2766 6565 6462         if 'feedb
-00005900: 6163 6b5f 6c6f 6f70 2720 696e 2073 656c  ack_loop' in sel
-00005910: 662e 5f74 6872 6561 6473 3a0d 0a20 2020  f._threads:..   
-00005920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005930: 662e 5f74 6872 6561 6473 5b27 6665 6564  f._threads['feed
-00005940: 6261 636b 5f6c 6f6f 7027 5d2e 6a6f 696e  back_loop'].join
-00005950: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00005960: 7468 7265 6164 203d 2054 6872 6561 6428  thread = Thread(
-00005970: 7461 7267 6574 3d73 656c 662e 5f6c 6f6f  target=self._loo
-00005980: 705f 6665 6564 6261 636b 290d 0a20 2020  p_feedback)..   
-00005990: 2020 2020 2020 2020 2074 6872 6561 642e           thread.
-000059a0: 7374 6172 7428 290d 0a20 2020 2020 2020  start()..       
-000059b0: 2020 2020 2073 656c 662e 5f74 6872 6561       self._threa
-000059c0: 6473 5b27 6665 6564 6261 636b 5f6c 6f6f  ds['feedback_loo
-000059d0: 7027 5d20 3d20 7468 7265 6164 0d0a 2020  p'] = thread..  
-000059e0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000059f0: 2020 2020 2020 2020 2069 6620 2766 6565           if 'fee
-00005a00: 6462 6163 6b5f 6c6f 6f70 2720 696e 2073  dback_loop' in s
-00005a10: 656c 662e 5f74 6872 6561 6473 3a0d 0a20  elf._threads:.. 
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005a30: 656c 662e 5f74 6872 6561 6473 5b27 6665  elf._threads['fe
-00005a40: 6564 6261 636b 5f6c 6f6f 7027 5d2e 6a6f  edback_loop'].jo
-00005a50: 696e 2829 0d0a 2020 2020 2020 2020 7265  in()..        re
-00005a60: 7475 726e 0d0a 0d0a 2020 2020 6465 6620  turn....    def 
-00005a70: 7a65 726f 2873 656c 6629 202d 3e20 7374  zero(self) -> st
-00005a80: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-00005a90: 0a20 2020 2020 2020 205a 6572 6f20 7468  .        Zero th
-00005aa0: 6520 706c 756e 6765 7220 706f 7369 7469  e plunger positi
-00005ab0: 6f6e 0d0a 2020 2020 2020 2020 0d0a 2020  on..        ..  
-00005ac0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005ad0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00005ae0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00005af0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005b00: 2020 2020 2020 2073 656c 662e 656a 6563         self.ejec
-00005b10: 7428 290d 0a20 2020 2020 2020 2072 6573  t()..        res
-00005b20: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
-00005b30: 6572 7928 2752 5a27 290d 0a20 2020 2020  ery('RZ')..     
-00005b40: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00005b50: 203d 2030 0d0a 2020 2020 2020 2020 7469   = 0..        ti
-00005b60: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
-00005b70: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00005b80: 6f6e 7365 0d0a 0d0a 2020 2020 2320 5072  onse....    # Pr
-00005b90: 6f74 6563 7465 6420 6d65 7468 6f64 2873  otected method(s
-00005ba0: 290d 0a20 2020 2064 6566 205f 6361 6c63  )..    def _calc
-00005bb0: 756c 6174 655f 7370 6565 645f 7061 7261  ulate_speed_para
-00005bc0: 6d65 7465 7273 2873 656c 662c 2076 6f6c  meters(self, vol
-00005bd0: 756d 653a 696e 742c 2073 7065 6564 3a69  ume:int, speed:i
-00005be0: 6e74 2920 2d3e 2053 7065 6564 5061 7261  nt) -> SpeedPara
-00005bf0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
-00005c00: 2022 2222 0d0a 2020 2020 2020 2020 4361   """..        Ca
-00005c10: 6c63 756c 6174 6573 2074 6865 2062 6573  lculates the bes
-00005c20: 7420 7061 7261 6d65 7465 7273 2066 6f72  t parameters for
-00005c30: 2076 6f6c 756d 6520 616e 6420 7370 6565   volume and spee
-00005c40: 640d 0a0d 0a20 2020 2020 2020 2041 7267  d....        Arg
-00005c50: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005c60: 766f 6c75 6d65 2028 696e 7429 3a20 766f  volume (int): vo
-00005c70: 6c75 6d65 2074 6f20 6265 2074 7261 6e73  lume to be trans
-00005c80: 6665 7272 6564 0d0a 2020 2020 2020 2020  ferred..        
-00005c90: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
-00005ca0: 2073 7065 6564 2061 7420 7768 6963 6820   speed at which 
-00005cb0: 6c69 7175 6964 2069 7320 7472 616e 7366  liquid is transf
-00005cc0: 6572 7265 640d 0a0d 0a20 2020 2020 2020  erred....       
-00005cd0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00005ce0: 2020 2020 2020 2064 6963 743a 2064 6963         dict: dic
-00005cf0: 7469 6f6e 6172 7920 6f66 2062 6573 7420  tionary of best 
-00005d00: 7061 7261 6d65 7465 7273 0d0a 2020 2020  parameters..    
-00005d10: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00005d20: 206f 7574 636f 6d65 7320 3d20 7b7d 0d0a   outcomes = {}..
-00005d30: 2020 2020 2020 2020 7374 6570 5f69 6e74          step_int
-00005d40: 6572 7661 6c5f 6c69 6d69 7420 3d20 696e  erval_limit = in
-00005d50: 7428 766f 6c75 6d65 2f73 656c 662e 7265  t(volume/self.re
-00005d60: 736f 6c75 7469 6f6e 2f53 5445 505f 5245  solution/STEP_RE
-00005d70: 534f 4c55 5449 4f4e 290d 0a20 2020 2020  SOLUTION)..     
-00005d80: 2020 2066 6f72 2070 7265 7365 7420 696e     for preset in
-00005d90: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
-00005da0: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
-00005db0: 2020 6966 2070 7265 7365 7420 3c20 7370    if preset < sp
-00005dc0: 6565 643a 0d0a 2020 2020 2020 2020 2020  eed:..          
-00005dd0: 2020 2020 2020 2320 7072 6573 6574 2069        # preset i
-00005de0: 7320 736c 6f77 6572 2074 6861 6e20 7461  s slower than ta
-00005df0: 7267 6574 2073 7065 6564 2c20 6974 2077  rget speed, it w
-00005e00: 696c 6c20 6e65 7665 7220 6869 7420 7461  ill never hit ta
-00005e10: 7267 6574 2073 7065 6564 0d0a 2020 2020  rget speed..    
-00005e20: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00005e30: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-00005e40: 2020 7469 6d65 5f69 6e74 6572 7661 6c5f    time_interval_
-00005e50: 6c69 6d69 7420 3d20 696e 7428 766f 6c75  limit = int(volu
-00005e60: 6d65 2a28 312f 7370 6565 6420 2d20 312f  me*(1/speed - 1/
-00005e70: 7072 6573 6574 292f 7365 6c66 2e72 6573  preset)/self.res
-00005e80: 706f 6e73 655f 7469 6d65 290d 0a20 2020  ponse_time)..   
-00005e90: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00005ea0: 7374 6570 5f69 6e74 6572 7661 6c5f 6c69  step_interval_li
-00005eb0: 6d69 7420 6f72 206e 6f74 2074 696d 655f  mit or not time_
-00005ec0: 696e 7465 7276 616c 5f6c 696d 6974 3a0d  interval_limit:.
-00005ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ee0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-00005ef0: 2020 2020 2020 2069 6e74 6572 7661 6c73         intervals
-00005f00: 203d 206d 6178 286d 696e 2873 7465 705f   = max(min(step_
-00005f10: 696e 7465 7276 616c 5f6c 696d 6974 2c20  interval_limit, 
-00005f20: 7469 6d65 5f69 6e74 6572 7661 6c5f 6c69  time_interval_li
-00005f30: 6d69 7429 2c20 3129 0d0a 2020 2020 2020  mit), 1)..      
-00005f40: 2020 2020 2020 6561 6368 5f73 7465 7073        each_steps
-00005f50: 203d 2076 6f6c 756d 652f 7365 6c66 2e72   = volume/self.r
-00005f60: 6573 6f6c 7574 696f 6e2f 696e 7465 7276  esolution/interv
-00005f70: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
-00005f80: 2065 6163 685f 6465 6c61 7920 3d20 766f   each_delay = vo
-00005f90: 6c75 6d65 2a28 312f 7370 6565 6420 2d20  lume*(1/speed - 
-00005fa0: 312f 7072 6573 6574 292f 696e 7465 7276  1/preset)/interv
-00005fb0: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
-00005fc0: 2061 7265 6120 3d20 302e 3520 2a20 2876   area = 0.5 * (v
-00005fd0: 6f6c 756d 652a 2a32 2920 2a20 2831 2f73  olume**2) * (1/s
-00005fe0: 656c 662e 7265 736f 6c75 7469 6f6e 2920  elf.resolution) 
-00005ff0: 2a20 2831 2f69 6e74 6572 7661 6c73 2920  * (1/intervals) 
-00006000: 2a20 2831 2f73 7065 6564 202d 2031 2f70  * (1/speed - 1/p
-00006010: 7265 7365 7429 0d0a 2020 2020 2020 2020  reset)..        
-00006020: 2020 2020 6f75 7463 6f6d 6573 5b61 7265      outcomes[are
-00006030: 615d 203d 2053 7065 6564 5061 7261 6d65  a] = SpeedParame
-00006040: 7465 7273 2870 7265 7365 742c 2069 6e74  ters(preset, int
-00006050: 6572 7661 6c73 2c20 696e 7428 6561 6368  ervals, int(each
-00006060: 5f73 7465 7073 292c 2065 6163 685f 6465  _steps), each_de
-00006070: 6c61 7929 0d0a 2020 2020 2020 2020 6966  lay)..        if
-00006080: 206c 656e 286f 7574 636f 6d65 7329 203d   len(outcomes) =
-00006090: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-000060a0: 2020 7072 696e 7428 224e 6f20 6665 6173    print("No feas
-000060b0: 6962 6c65 2073 7065 6564 2070 6172 616d  ible speed param
-000060c0: 6574 6572 732e 2229 0d0a 2020 2020 2020  eters.")..      
-000060d0: 2020 2020 2020 7265 7475 726e 2053 7065        return Spe
-000060e0: 6564 5061 7261 6d65 7465 7273 284e 6f6e  edParameters(Non
-000060f0: 652c 2053 5445 505f 5245 534f 4c55 5449  e, STEP_RESOLUTI
-00006100: 4f4e 2c20 5354 4550 5f52 4553 4f4c 5554  ON, STEP_RESOLUT
-00006110: 494f 4e2c 2073 656c 662e 7265 7370 6f6e  ION, self.respon
-00006120: 7365 5f74 696d 6529 0d0a 2020 2020 2020  se_time)..      
-00006130: 2020 7072 696e 7428 6627 4265 7374 2070    print(f'Best p
-00006140: 6172 616d 6574 6572 733a 207b 6f75 7463  arameters: {outc
-00006150: 6f6d 6573 5b6d 696e 286f 7574 636f 6d65  omes[min(outcome
-00006160: 7329 5d7d 2729 0d0a 2020 2020 2020 2020  s)]}')..        
-00006170: 7265 7475 726e 206f 7574 636f 6d65 735b  return outcomes[
-00006180: 6d69 6e28 6f75 7463 6f6d 6573 295d 0d0a  min(outcomes)]..
-00006190: 2020 2020 0d0a 2020 2020 6465 6620 5f63      ..    def _c
-000061a0: 6f6e 6e65 6374 2873 656c 662c 2070 6f72  onnect(self, por
-000061b0: 743a 7374 722c 2062 6175 6472 6174 653a  t:str, baudrate:
-000061c0: 696e 7420 3d20 3936 3030 2c20 7469 6d65  int = 9600, time
-000061d0: 6f75 743a 696e 7420 3d20 3129 3a0d 0a20  out:int = 1):.. 
-000061e0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000061f0: 2020 2020 436f 6e6e 6563 7469 6f6e 2070      Connection p
-00006200: 726f 6365 6475 7265 2066 6f72 2074 6f6f  rocedure for too
-00006210: 6c0d 0a0d 0a20 2020 2020 2020 2041 7267  l....        Arg
-00006220: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00006230: 706f 7274 2028 7374 7229 3a20 434f 4d20  port (str): COM 
-00006240: 706f 7274 2061 6464 7265 7373 0d0a 2020  port address..  
-00006250: 2020 2020 2020 2020 2020 6261 7564 7261            baudra
-00006260: 7465 2028 696e 742c 206f 7074 696f 6e61  te (int, optiona
-00006270: 6c29 3a20 6261 7564 7261 7465 2e20 4465  l): baudrate. De
-00006280: 6661 756c 7473 2074 6f20 3936 3030 2e0d  faults to 9600..
-00006290: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-000062a0: 656f 7574 2028 696e 742c 206f 7074 696f  eout (int, optio
-000062b0: 6e61 6c29 3a20 7469 6d65 6f75 7420 696e  nal): timeout in
-000062c0: 2073 6563 6f6e 6473 2e20 4465 6661 756c   seconds. Defaul
-000062d0: 7473 2074 6f20 312e 0d0a 2020 2020 2020  ts to 1...      
-000062e0: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-000062f0: 656c 662e 636f 6e6e 6563 7469 6f6e 5f64  elf.connection_d
-00006300: 6574 6169 6c73 203d 207b 0d0a 2020 2020  etails = {..    
-00006310: 2020 2020 2020 2020 2770 6f72 7427 3a20          'port': 
-00006320: 706f 7274 2c0d 0a20 2020 2020 2020 2020  port,..         
-00006330: 2020 2027 6261 7564 7261 7465 273a 2062     'baudrate': b
-00006340: 6175 6472 6174 652c 0d0a 2020 2020 2020  audrate,..      
-00006350: 2020 2020 2020 2774 696d 656f 7574 273a        'timeout':
-00006360: 2074 696d 656f 7574 0d0a 2020 2020 2020   timeout..      
-00006370: 2020 7d0d 0a20 2020 2020 2020 2064 6576    }..        dev
-00006380: 6963 6520 3d20 4e6f 6e65 0d0a 2020 2020  ice = None..    
-00006390: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-000063a0: 2020 2020 2020 6465 7669 6365 203d 2073        device = s
-000063b0: 6572 6961 6c2e 5365 7269 616c 2870 6f72  erial.Serial(por
-000063c0: 742c 2062 6175 6472 6174 652c 2074 696d  t, baudrate, tim
-000063d0: 656f 7574 3d74 696d 656f 7574 290d 0a20  eout=timeout).. 
-000063e0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000063f0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-00006400: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00006410: 2866 2243 6f75 6c64 206e 6f74 2063 6f6e  (f"Could not con
-00006420: 6e65 6374 2074 6f20 7b70 6f72 747d 2229  nect to {port}")
-00006430: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00006440: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
-00006470: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00006480: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00006490: 3229 2020 2023 2057 6169 7420 666f 7220  2)   # Wait for 
-000064a0: 6772 626c 2074 6f20 696e 6974 6961 6c69  grbl to initiali
-000064b0: 7a65 0d0a 2020 2020 2020 2020 2020 2020  ze..            
-000064c0: 6465 7669 6365 2e66 6c75 7368 496e 7075  device.flushInpu
-000064d0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-000064e0: 2070 7269 6e74 2866 2243 6f6e 6e65 6374   print(f"Connect
-000064f0: 696f 6e20 6f70 656e 6564 2074 6f20 7b70  ion opened to {p
-00006500: 6f72 747d 2229 0d0a 2020 2020 2020 2020  ort}")..        
-00006510: 2020 2020 7365 6c66 2e73 6574 466c 6167      self.setFlag
-00006520: 2863 6f6e 6e65 6374 6564 3d54 7275 6529  (connected=True)
-00006530: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-00006540: 6576 6963 6520 3d20 6465 7669 6365 0d0a  evice = device..
-00006550: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-00006560: 496e 666f 2829 0d0a 2020 2020 2020 2020  Info()..        
-00006570: 7365 6c66 2e72 6573 6574 2829 0d0a 2020  self.reset()..  
-00006580: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00006590: 2020 0d0a 2020 2020 6465 6620 5f69 735f    ..    def _is_
-000065a0: 6578 7065 6374 6564 5f72 6570 6c79 2873  expected_reply(s
-000065b0: 656c 662c 2072 6573 706f 6e73 653a 7374  elf, response:st
-000065c0: 722c 2063 6f6d 6d61 6e64 5f63 6f64 653a  r, command_code:
-000065d0: 7374 722c 202a 2a6b 7761 7267 7329 202d  str, **kwargs) -
-000065e0: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
-000065f0: 2022 2222 0d0a 2020 2020 2020 2020 4368   """..        Ch
-00006600: 6563 6b73 2061 6e64 2072 6574 7572 6e73  ecks and returns
-00006610: 2077 6865 7468 6572 2074 6865 2072 6573   whether the res
-00006620: 706f 6e73 6520 6973 2061 6e20 6578 7065  ponse is an expe
-00006630: 6374 6564 2072 6570 6c79 0d0a 0d0a 2020  cted reply....  
-00006640: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00006650: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00006660: 6520 2873 7472 293a 2072 6573 706f 6e73  e (str): respons
-00006670: 6520 7374 7269 6e67 2066 726f 6d20 6465  e string from de
-00006680: 7669 6365 0d0a 2020 2020 2020 2020 2020  vice..          
-00006690: 2020 636f 6d6d 616e 645f 636f 6465 2028    command_code (
-000066a0: 7374 7229 3a20 7477 6f2d 6368 6172 6163  str): two-charac
-000066b0: 7465 7220 636f 6d6d 616e 6420 636f 6465  ter command code
-000066c0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-000066d0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-000066e0: 2020 626f 6f6c 3a20 7768 6574 6865 7220    bool: whether 
-000066f0: 7468 6520 7265 7370 6f6e 7365 2069 7320  the response is 
-00006700: 616e 2065 7870 6563 7465 6420 7265 706c  an expected repl
-00006710: 790d 0a20 2020 2020 2020 2022 2222 0d0a  y..        """..
-00006720: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
-00006730: 6e73 6520 696e 2045 7272 6f72 436f 6465  nse in ErrorCode
-00006740: 2e5f 6d65 6d62 6572 5f6e 616d 6573 5f3a  ._member_names_:
-00006750: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006760: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00006770: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
-00006780: 6465 206e 6f74 2069 6e20 5155 4552 4945  de not in QUERIE
-00006790: 5320 616e 6420 7265 7370 6f6e 7365 203d  S and response =
-000067a0: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
-000067b0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-000067c0: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
-000067d0: 6d61 6e64 5f63 6f64 6520 696e 2051 5545  mand_code in QUE
-000067e0: 5249 4553 2061 6e64 2072 6573 706f 6e73  RIES and respons
-000067f0: 655b 3a32 5d20 3d3d 2063 6f6d 6d61 6e64  e[:2] == command
-00006800: 5f63 6f64 652e 6c6f 7765 7228 293a 0d0a  _code.lower():..
-00006810: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00006820: 795f 636f 6465 2c20 6461 7461 203d 2072  y_code, data = r
-00006830: 6573 706f 6e73 655b 3a32 5d2c 2072 6573  esponse[:2], res
-00006840: 706f 6e73 655b 323a 5d0d 0a20 2020 2020  ponse[2:]..     
-00006850: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-00006860: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00006870: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00006880: 275b 7b72 6570 6c79 5f63 6f64 657d 5d20  '[{reply_code}] 
-00006890: 7b64 6174 617d 2729 0d0a 2020 2020 2020  {data}')..      
-000068a0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000068b0: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-000068c0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
-000068d0: 6566 205f 6c6f 6f70 5f66 6565 6462 6163  ef _loop_feedbac
-000068e0: 6b28 7365 6c66 293a 0d0a 2020 2020 2020  k(self):..      
-000068f0: 2020 2222 224c 6f6f 7020 746f 2063 6f6e    """Loop to con
-00006900: 7374 616e 746c 7920 7265 6164 2066 726f  stantly read fro
-00006910: 6d20 6465 7669 6365 2222 220d 0a20 2020  m device"""..   
-00006920: 2020 2020 2070 7269 6e74 2827 4c69 7374       print('List
-00006930: 656e 696e 672e 2e2e 2729 0d0a 2020 2020  ening...')..    
-00006940: 2020 2020 7768 696c 6520 7365 6c66 2e66      while self.f
-00006950: 6c61 6773 5b27 6765 745f 6665 6564 6261  lags['get_feedba
-00006960: 636b 275d 3a0d 0a20 2020 2020 2020 2020  ck']:..         
-00006970: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
-00006980: 5b27 7061 7573 655f 6665 6564 6261 636b  ['pause_feedback
-00006990: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
-000069a0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-000069b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000069c0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
-000069d0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-000069e0: 7443 6170 6163 6974 616e 6365 2829 0d0a  tCapacitance()..
-000069f0: 2020 2020 2020 2020 7072 696e 7428 2753          print('S
-00006a00: 746f 7020 6c69 7374 656e 696e 672e 2e2e  top listening...
-00006a10: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
-00006a20: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
-00006a30: 6620 5f71 7565 7279 2873 656c 662c 200d  f _query(self, .
-00006a40: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00006a50: 3a20 7374 722c 200d 0a20 2020 2020 2020  : str, ..       
-00006a60: 2074 696d 656f 7574 5f73 3a20 666c 6f61   timeout_s: floa
-00006a70: 7420 3d20 302e 332c 200d 0a20 2020 2020  t = 0.3, ..     
-00006a80: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
-00006a90: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
-00006aa0: 0d0a 2020 2020 2920 2d3e 2073 7472 3a0d  ..    ) -> str:.
-00006ab0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00006ac0: 2020 2020 2020 5772 6974 6520 636f 6d6d        Write comm
-00006ad0: 616e 6420 746f 2061 6e64 2072 6561 6420  and to and read 
-00006ae0: 7265 7370 6f6e 7365 2066 726f 6d20 6465  response from de
-00006af0: 7669 6365 0d0a 0d0a 2020 2020 2020 2020  vice....        
-00006b00: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00006b10: 2020 2063 6f6d 6d61 6e64 2028 7374 7229     command (str)
-00006b20: 3a20 636f 6d6d 616e 6420 7374 7269 6e67  : command string
-00006b30: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-00006b40: 6d65 6f75 745f 7320 2866 6c6f 6174 2c20  meout_s (float, 
-00006b50: 6f70 7469 6f6e 616c 293a 2064 7572 6174  optional): durat
-00006b60: 696f 6e20 746f 2077 6169 7420 6265 666f  ion to wait befo
-00006b70: 7265 2074 696d 656f 7574 2e20 4465 6661  re timeout. Defa
-00006b80: 756c 7473 2074 6f20 302e 332e 0d0a 2020  ults to 0.3...  
-00006b90: 2020 2020 2020 2020 2020 7265 7375 6d65            resume
-00006ba0: 5f66 6565 6462 6163 6b20 2862 6f6f 6c2c  _feedback (bool,
-00006bb0: 206f 7074 696f 6e61 6c29 3a20 7768 6574   optional): whet
-00006bc0: 6865 7220 746f 2072 6573 756d 6520 7265  her to resume re
-00006bd0: 6164 696e 6720 6672 6f6d 2064 6576 6963  ading from devic
-00006be0: 652e 2044 6566 6175 6c74 7320 746f 2046  e. Defaults to F
-00006bf0: 616c 7365 2e0d 0a0d 0a20 2020 2020 2020  alse.....       
-00006c00: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00006c10: 2020 2020 2020 2073 7472 3a20 7265 7370         str: resp
-00006c20: 6f6e 7365 2073 7472 696e 670d 0a20 2020  onse string..   
-00006c30: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00006c40: 2020 636f 6d6d 616e 645f 636f 6465 203d    command_code =
-00006c50: 2063 6f6d 6d61 6e64 5b3a 325d 0d0a 2020   command[:2]..  
-00006c60: 2020 2020 2020 6966 2063 6f6d 6d61 6e64        if command
-00006c70: 5f63 6f64 6520 6e6f 7420 696e 2053 5441  _code not in STA
-00006c80: 5455 535f 5155 4552 4945 533a 0d0a 2020  TUS_QUERIES:..  
-00006c90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00006ca0: 662e 666c 6167 735b 2767 6574 5f66 6565  f.flags['get_fee
-00006cb0: 6462 6163 6b27 5d20 616e 6420 6e6f 7420  dback'] and not 
-00006cc0: 7365 6c66 2e66 6c61 6773 5b27 7061 7573  self.flags['paus
-00006cd0: 655f 6665 6564 6261 636b 275d 3a0d 0a20  e_feedback']:.. 
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006cf0: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
-00006d00: 655f 6665 6564 6261 636b 3d54 7275 6529  e_feedback=True)
-00006d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006d20: 2020 7469 6d65 2e73 6c65 6570 2874 696d    time.sleep(tim
-00006d30: 656f 7574 5f73 290d 0a20 2020 2020 2020  eout_s)..       
-00006d40: 2020 2020 2073 656c 662e 6765 7453 7461       self.getSta
-00006d50: 7475 7328 290d 0a20 2020 2020 2020 2020  tus()..         
-00006d60: 2020 2077 6869 6c65 2073 656c 662e 6973     while self.is
-00006d70: 4275 7379 2829 3a0d 0a20 2020 2020 2020  Busy():..       
-00006d80: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00006d90: 7453 7461 7475 7328 290d 0a20 2020 2020  tStatus()..     
-00006da0: 2020 200d 0a20 2020 2020 2020 2073 7461     ..        sta
-00006db0: 7274 5f74 696d 6520 3d20 7469 6d65 2e74  rt_time = time.t
-00006dc0: 696d 6528 290d 0a20 2020 2020 2020 2073  ime()..        s
-00006dd0: 656c 662e 5f77 7269 7465 2863 6f6d 6d61  elf._write(comma
-00006de0: 6e64 290d 0a20 2020 2020 2020 2072 6573  nd)..        res
-00006df0: 706f 6e73 6520 3d20 2727 0d0a 2020 2020  ponse = ''..    
-00006e00: 2020 2020 7768 696c 6520 6e6f 7420 7365      while not se
-00006e10: 6c66 2e5f 6973 5f65 7870 6563 7465 645f  lf._is_expected_
-00006e20: 7265 706c 7928 7265 7370 6f6e 7365 2c20  reply(response, 
-00006e30: 636f 6d6d 616e 645f 636f 6465 293a 0d0a  command_code):..
-00006e40: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00006e50: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
-00006e60: 7274 5f74 696d 6520 3e20 7469 6d65 6f75  rt_time > timeou
-00006e70: 745f 733a 0d0a 2020 2020 2020 2020 2020  t_s:..          
-00006e80: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
-00006e90: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00006ea0: 6520 3d20 7365 6c66 2e5f 7265 6164 2829  e = self._read()
-00006eb0: 0d0a 2020 2020 2020 2020 2320 7072 696e  ..        # prin
-00006ec0: 7428 7469 6d65 2e74 696d 6528 2920 2d20  t(time.time() - 
-00006ed0: 7374 6172 745f 7469 6d65 290d 0a20 2020  start_time)..   
-00006ee0: 2020 2020 2069 6620 636f 6d6d 616e 645f       if command_
-00006ef0: 636f 6465 2069 6e20 5155 4552 4945 533a  code in QUERIES:
-00006f00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006f10: 7370 6f6e 7365 203d 2072 6573 706f 6e73  sponse = respons
-00006f20: 655b 323a 5d0d 0a20 2020 2020 2020 2069  e[2:]..        i
-00006f30: 6620 636f 6d6d 616e 645f 636f 6465 206e  f command_code n
-00006f40: 6f74 2069 6e20 5354 4154 5553 5f51 5545  ot in STATUS_QUE
-00006f50: 5249 4553 3a0d 0a20 2020 2020 2020 2020  RIES:..         
-00006f60: 2020 2073 656c 662e 6765 7450 6f73 6974     self.getPosit
-00006f70: 696f 6e28 290d 0a20 2020 2020 2020 2020  ion()..         
-00006f80: 2020 2069 6620 7265 7375 6d65 5f66 6565     if resume_fee
-00006f90: 6462 6163 6b3a 0d0a 2020 2020 2020 2020  dback:..        
-00006fa0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00006fb0: 466c 6167 2870 6175 7365 5f66 6565 6462  Flag(pause_feedb
-00006fc0: 6163 6b3d 4661 6c73 6529 0d0a 2020 2020  ack=False)..    
-00006fd0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00006fe0: 6e73 650d 0a0d 0a20 2020 2064 6566 205f  nse....    def _
-00006ff0: 7265 6164 2873 656c 6629 202d 3e20 7374  read(self) -> st
-00007000: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-00007010: 0a20 2020 2020 2020 2052 6561 6420 7265  .        Read re
-00007020: 7370 6f6e 7365 2066 726f 6d20 6465 7669  sponse from devi
-00007030: 6365 0d0a 0d0a 2020 2020 2020 2020 5265  ce....        Re
-00007040: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00007050: 2020 2020 7374 723a 2072 6573 706f 6e73      str: respons
-00007060: 6520 7374 7269 6e67 0d0a 2020 2020 2020  e string..      
-00007070: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00007080: 6573 706f 6e73 6520 3d20 2727 0d0a 2020  esponse = ''..  
-00007090: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000070a0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000070b0: 203d 2073 656c 662e 6465 7669 6365 2e72   = self.device.r
-000070c0: 6561 646c 696e 6528 290d 0a20 2020 2020  eadline()..     
-000070d0: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-000070e0: 7370 6f6e 7365 2920 3d3d 2030 3a0d 0a20  sponse) == 0:.. 
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007100: 6573 706f 6e73 6520 3d20 7365 6c66 2e64  esponse = self.d
-00007110: 6576 6963 652e 7265 6164 6c69 6e65 2829  evice.readline()
-00007120: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00007130: 7370 6f6e 7365 203d 2072 6573 706f 6e73  sponse = respons
-00007140: 655b 323a 2d32 5d2e 6465 636f 6465 2827  e[2:-2].decode('
-00007150: 7574 662d 3827 290d 0a20 2020 2020 2020  utf-8')..       
-00007160: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
-00007170: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
-00007180: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-00007190: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000071a0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-000071b0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-000071c0: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-000071d0: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-000071e0: 290d 0a20 2020 2020 2020 2069 6620 7265  )..        if re
-000071f0: 7370 6f6e 7365 2069 6e20 4572 726f 7243  sponse in ErrorC
-00007200: 6f64 652e 5f6d 656d 6265 725f 6e61 6d65  ode._member_name
-00007210: 735f 3a0d 0a20 2020 2020 2020 2020 2020  s_:..           
-00007220: 2070 7269 6e74 2845 7272 6f72 436f 6465   print(ErrorCode
-00007230: 5b72 6573 706f 6e73 655d 2e76 616c 7565  [response].value
-00007240: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00007250: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
-00007260: 0d0a 2020 2020 6465 6620 5f73 6574 5f63  ..    def _set_c
-00007270: 6861 6e6e 656c 5f69 6428 7365 6c66 2c20  hannel_id(self, 
-00007280: 6e65 775f 6368 616e 6e65 6c5f 6964 3a69  new_channel_id:i
-00007290: 6e74 293a 0d0a 2020 2020 2020 2020 2222  nt):..        ""
-000072a0: 220d 0a20 2020 2020 2020 2053 6574 2063  "..        Set c
-000072b0: 6861 6e6e 656c 2069 6420 6f66 2064 6576  hannel id of dev
-000072c0: 6963 650d 0a0d 0a20 2020 2020 2020 2041  ice....        A
-000072d0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-000072e0: 2020 6e65 775f 6368 616e 6e65 6c20 2869    new_channel (i
-000072f0: 6e74 293a 206e 6577 2063 6861 6e6e 656c  nt): new channel
-00007300: 2069 640d 0a0d 0a20 2020 2020 2020 2052   id....        R
-00007310: 6169 7365 733a 0d0a 2020 2020 2020 2020  aises:..        
-00007320: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00007330: 506c 6561 7365 2073 656c 6563 7420 6120  Please select a 
-00007340: 7661 6c69 6420 724c 696e 6520 6164 6472  valid rLine addr
-00007350: 6573 7320 6672 6f6d 2031 2074 6f20 390d  ess from 1 to 9.
-00007360: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00007370: 2020 2020 2020 6966 206e 6f74 2028 3020        if not (0 
-00007380: 3c20 6e65 775f 6368 616e 6e65 6c5f 6964  < new_channel_id
-00007390: 203c 2031 3029 3a0d 0a20 2020 2020 2020   < 10):..       
-000073a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000073b0: 4572 726f 7228 2750 6c65 6173 6520 7365  Error('Please se
-000073c0: 6c65 6374 2061 2076 616c 6964 2072 4c69  lect a valid rLi
-000073d0: 6e65 2061 6464 7265 7373 2066 726f 6d20  ne address from 
-000073e0: 3120 746f 2039 2e27 290d 0a20 2020 2020  1 to 9.')..     
-000073f0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00007400: 6c66 2e5f 7175 6572 7928 6627 2a41 7b6e  lf._query(f'*A{n
-00007410: 6577 5f63 6861 6e6e 656c 5f69 647d 2729  ew_channel_id}')
-00007420: 0d0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
-00007430: 706f 6e73 6520 3d3d 2027 6f6b 273a 0d0a  ponse == 'ok':..
-00007440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007450: 2e63 6861 6e6e 656c 203d 206e 6577 5f63  .channel = new_c
-00007460: 6861 6e6e 656c 5f69 640d 0a20 2020 2020  hannel_id..     
-00007470: 2020 2072 6574 7572 6e0d 0a20 2020 200d     return..    .
-00007480: 0a20 2020 2064 6566 205f 7772 6974 6528  .    def _write(
-00007490: 7365 6c66 2c20 636f 6d6d 616e 643a 7374  self, command:st
-000074a0: 7229 202d 3e20 626f 6f6c 3a0d 0a20 2020  r) -> bool:..   
-000074b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000074c0: 2020 5772 6974 6520 636f 6d6d 616e 6420    Write command 
-000074d0: 746f 2064 6576 6963 650d 0a0d 0a20 2020  to device....   
-000074e0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
-000074f0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
-00007500: 2873 7472 293a 203c 636f 6d6d 616e 6420  (str): <command 
-00007510: 636f 6465 3e3c 7661 6c75 653e 0d0a 0d0a  code><value>....
-00007520: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00007530: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-00007540: 6f6c 3a20 7768 6574 6865 7220 636f 6d6d  ol: whether comm
-00007550: 616e 6420 7761 7320 7365 6e74 2073 7563  and was sent suc
-00007560: 6365 7373 6675 6c6c 790d 0a20 2020 2020  cessfully..     
-00007570: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00007580: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
-00007590: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-000075a0: 696e 7428 636f 6d6d 616e 6429 0d0a 2020  int(command)..  
-000075b0: 2020 2020 2020 6673 7472 696e 6720 3d20        fstring = 
-000075c0: 6627 017b 7365 6c66 2e63 6861 6e6e 656c  f'.{self.channel
-000075d0: 7d7b 636f 6d6d 616e 647d c2ba 5c72 2720  }{command}..\r' 
-000075e0: 2320 636f 6d6d 616e 6420 7465 6d70 6c61  # command templa
-000075f0: 7465 3a20 3c50 5245 3e3c 4144 523e 3c43  te: <PRE><ADR><C
-00007600: 4f44 453e 3c44 4154 413e 3c4c 5243 3e3c  ODE><DATA><LRC><
-00007610: 504f 5354 3e0d 0a20 2020 2020 2020 2023  POST>..        #
-00007620: 2062 7374 7269 6e67 203d 2062 7974 6561   bstring = bytea
-00007630: 7272 6179 2e66 726f 6d68 6578 2866 7374  rray.fromhex(fst
-00007640: 7269 6e67 2e65 6e63 6f64 6528 2775 7466  ring.encode('utf
-00007650: 2d38 2729 2e68 6578 2829 290d 0a20 2020  -8').hex())..   
-00007660: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00007670: 2020 2020 2020 2023 2054 7970 6963 616c         # Typical
-00007680: 2074 696d 656f 7574 2077 6169 7420 6973   timeout wait is
-00007690: 2034 3030 6d73 0d0a 2020 2020 2020 2020   400ms..        
-000076a0: 2020 2020 7365 6c66 2e64 6576 6963 652e      self.device.
-000076b0: 7772 6974 6528 6673 7472 696e 672e 656e  write(fstring.en
-000076c0: 636f 6465 2827 7574 662d 3827 2929 0d0a  code('utf-8'))..
-000076d0: 2020 2020 2020 2020 6578 6365 7074 2041          except A
-000076e0: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
-000076f0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00007700: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00007710: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00007720: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00007730: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
-00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007750: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
-00007760: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00007770: 7365 0d0a 2020 2020 2020 2020 7265 7475  se..        retu
-00007780: 726e 2054 7275 650d 0a20 2020 20         rn True..    
+00002230: 7065 7266 5f63 6f75 6e74 6572 2829 0d0a  perf_counter()..
+00002240: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
+00002250: 7365 6c66 2e73 7065 6564 2e75 7020 6966  self.speed.up if
+00002260: 2073 7065 6564 2069 7320 4e6f 6e65 2065   speed is None e
+00002270: 6c73 6520 7370 6565 640d 0a20 2020 2020  lse speed..     
+00002280: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+00002290: 7370 6565 6420 696e 2073 656c 662e 7370  speed in self.sp
+000022a0: 6565 645f 7072 6573 6574 733a 0d0a 2020  eed_presets:..  
+000022b0: 2020 2020 2020 2020 2020 6966 2073 7065            if spe
+000022c0: 6564 2021 3d20 7365 6c66 2e73 7065 6564  ed != self.speed
+000022d0: 2e75 703a 0d0a 2020 2020 2020 2020 2020  .up:..          
+000022e0: 2020 2020 2020 7365 6c66 2e73 6574 5370        self.setSp
+000022f0: 6565 6428 7370 6565 643d 7370 6565 642c  eed(speed=speed,
+00002300: 2075 703d 5472 7565 2c20 6465 6661 756c   up=True, defaul
+00002310: 743d 4661 6c73 6529 0d0a 2020 2020 2020  t=False)..      
+00002320: 2020 2020 2020 7374 6172 745f 6173 7069        start_aspi
+00002330: 7261 7465 203d 2074 696d 652e 7065 7266  rate = time.perf
+00002340: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
+00002350: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00002360: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
+00002370: 2752 497b 7374 6570 737d 2729 0d0a 2020  'RI{steps}')..  
+00002380: 2020 2020 2020 2020 2020 6d6f 7665 5f74            move_t
+00002390: 696d 6520 3d20 7374 6570 732a 7365 6c66  ime = steps*self
+000023a0: 2e72 6573 6f6c 7574 696f 6e20 2f20 7370  .resolution / sp
+000023b0: 6565 640d 0a20 2020 2020 2020 2020 2020  eed..           
+000023c0: 2064 7572 6174 696f 6e20 3d20 7469 6d65   duration = time
+000023d0: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
+000023e0: 2d20 7374 6172 745f 6173 7069 7261 7465  - start_aspirate
+000023f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00002400: 2064 7572 6174 696f 6e20 3c20 286d 6f76   duration < (mov
+00002410: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
+00002420: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00002430: 6c65 6570 286d 6f76 655f 7469 6d65 2d64  leep(move_time-d
+00002440: 7572 6174 696f 6e29 0d0a 2020 2020 2020  uration)..      
+00002450: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
+00002460: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
+00002470: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00002480: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+00002490: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+000024a0: 2020 2020 2020 2065 6c69 6620 7370 6565         elif spee
+000024b0: 6420 6e6f 7420 696e 2073 656c 662e 7370  d not in self.sp
+000024c0: 6565 645f 7072 6573 6574 733a 0d0a 2020  eed_presets:..  
+000024d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000024e0: 6622 5461 7267 6574 3a20 7b76 6f6c 756d  f"Target: {volum
+000024f0: 657d 2075 4c20 6174 207b 7370 6565 647d  e} uL at {speed}
+00002500: 2075 4c2f 732e 2e2e 2229 0d0a 2020 2020   uL/s...")..    
+00002510: 2020 2020 2020 2020 7370 6565 645f 7061          speed_pa
+00002520: 7261 6d65 7465 7273 203d 2073 656c 662e  rameters = self.
+00002530: 5f63 616c 6375 6c61 7465 5f73 7065 6564  _calculate_speed
+00002540: 5f70 6172 616d 6574 6572 7328 766f 6c75  _parameters(volu
+00002550: 6d65 3d76 6f6c 756d 652c 2073 7065 6564  me=volume, speed
+00002560: 3d73 7065 6564 290d 0a20 2020 2020 2020  =speed)..       
+00002570: 2020 2020 2070 7269 6e74 2873 7065 6564       print(speed
+00002580: 5f70 6172 616d 6574 6572 7329 0d0a 2020  _parameters)..  
+00002590: 2020 2020 2020 2020 2020 7072 6573 6574            preset
+000025a0: 203d 2073 7065 6564 5f70 6172 616d 6574   = speed_paramet
+000025b0: 6572 732e 7072 6573 6574 0d0a 2020 2020  ers.preset..    
+000025c0: 2020 2020 2020 2020 6966 2070 7265 7365          if prese
+000025d0: 7420 6973 204e 6f6e 653a 0d0a 2020 2020  t is None:..    
+000025e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000025f0: 6520 5275 6e74 696d 6545 7272 6f72 2827  e RuntimeError('
+00002600: 5461 7267 6574 2073 7065 6564 206e 6f74  Target speed not
+00002610: 2070 6f73 7369 626c 652e 2729 0d0a 2020   possible.')..  
+00002620: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00002630: 6574 5370 6565 6428 7370 6565 643d 7072  etSpeed(speed=pr
+00002640: 6573 6574 2c20 7570 3d54 7275 652c 2064  eset, up=True, d
+00002650: 6566 6175 6c74 3d46 616c 7365 290d 0a20  efault=False).. 
+00002660: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00002670: 2020 2020 2020 2020 2073 7465 7073 5f6c           steps_l
+00002680: 6566 7420 3d20 7374 6570 730d 0a20 2020  eft = steps..   
+00002690: 2020 2020 2020 2020 2064 656c 6179 203d           delay =
+000026a0: 2073 7065 6564 5f70 6172 616d 6574 6572   speed_parameter
+000026b0: 732e 6465 6c61 790d 0a20 2020 2020 2020  s.delay..       
+000026c0: 2020 2020 2073 7465 705f 7369 7a65 203d       step_size =
+000026d0: 2073 7065 6564 5f70 6172 616d 6574 6572   speed_parameter
+000026e0: 732e 7374 6570 5f73 697a 650d 0a20 2020  s.step_size..   
+000026f0: 2020 2020 2020 2020 2069 6e74 6572 7661           interva
+00002700: 6c73 203d 2073 7065 6564 5f70 6172 616d  ls = speed_param
+00002710: 6574 6572 732e 696e 7465 7276 616c 730d  eters.intervals.
+00002720: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00002730: 7274 5f61 7370 6972 6174 6520 3d20 7469  rt_aspirate = ti
+00002740: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+00002750: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00002760: 6f72 2069 2069 6e20 7261 6e67 6528 696e  or i in range(in
+00002770: 7465 7276 616c 7329 3a0d 0a20 2020 2020  tervals):..     
+00002780: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00002790: 5f74 696d 6520 3d20 7469 6d65 2e70 6572  _time = time.per
+000027a0: 665f 636f 756e 7465 7228 290d 0a20 2020  f_counter()..   
+000027b0: 2020 2020 2020 2020 2020 2020 2073 7465               ste
+000027c0: 7020 3d20 7374 6570 5f73 697a 6520 6966  p = step_size if
+000027d0: 2028 692b 3120 213d 2069 6e74 6572 7661   (i+1 != interva
+000027e0: 6c73 2920 656c 7365 2073 7465 7073 5f6c  ls) else steps_l
+000027f0: 6566 740d 0a20 2020 2020 2020 2020 2020  eft..           
+00002800: 2020 2020 206d 6f76 655f 7469 6d65 203d       move_time =
+00002810: 2073 7465 702a 7365 6c66 2e72 6573 6f6c   step*self.resol
+00002820: 7574 696f 6e20 2f20 7072 6573 6574 0d0a  ution / preset..
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00002850: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
+00002860: 7d27 2c20 7265 7375 6d65 5f66 6565 6462  }', resume_feedb
+00002870: 6163 6b3d 4661 6c73 652c 2067 6574 5f70  ack=False, get_p
+00002880: 6f73 6974 696f 6e3d 4661 6c73 6529 0d0a  osition=False)..
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2320 6966 2072 6573 706f 6e73 6520 213d  # if response !=
+000028b0: 2027 6f6b 273a 0d0a 2020 2020 2020 2020   'ok':..        
+000028c0: 2020 2020 2020 2020 2320 2020 2020 7072          #     pr
+000028d0: 696e 7428 2241 7370 6972 6174 696f 6e20  int("Aspiration 
+000028e0: 6661 696c 6564 2229 0d0a 2020 2020 2020  failed")..      
+000028f0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00002900: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+00002910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002920: 2073 7465 7073 5f6c 6566 7420 2d3d 2073   steps_left -= s
+00002930: 7465 700d 0a20 2020 2020 2020 2020 2020  tep..           
+00002940: 2020 2020 2064 7572 6174 696f 6e20 3d20       duration = 
+00002950: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
+00002960: 7228 2920 2d20 7374 6172 745f 7469 6d65  r() - start_time
+00002970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002980: 2020 6966 2064 7572 6174 696f 6e20 3c20    if duration < 
+00002990: 2864 656c 6179 2b6d 6f76 655f 7469 6d65  (delay+move_time
+000029a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000029b0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
+000029c0: 6570 2864 656c 6179 2b6d 6f76 655f 7469  ep(delay+move_ti
+000029d0: 6d65 2d64 7572 6174 696f 6e29 0d0a 2020  me-duration)..  
+000029e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000029f0: 2320 5570 6461 7465 2076 616c 7565 730d  # Update values.
+00002a00: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00002a10: 2741 7370 6972 6174 696f 6e20 7469 6d65  'Aspiration time
+00002a20: 3a20 7b74 696d 652e 7065 7266 5f63 6f75  : {time.perf_cou
+00002a30: 6e74 6572 2829 2d73 7461 7274 5f61 7370  nter()-start_asp
+00002a40: 6972 6174 657d 7327 290d 0a20 2020 2020  irate}s')..     
+00002a50: 2020 2074 696d 652e 736c 6565 7028 7761     time.sleep(wa
+00002a60: 6974 290d 0a20 2020 2020 2020 2073 656c  it)..        sel
+00002a70: 662e 7365 7446 6c61 6728 6f63 6375 7069  f.setFlag(occupi
+00002a80: 6564 3d46 616c 7365 2c20 7061 7573 655f  ed=False, pause_
+00002a90: 6665 6564 6261 636b 3d46 616c 7365 290d  feedback=False).
+00002aa0: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
+00002ab0: 7450 6f73 6974 696f 6e28 290d 0a20 2020  tPosition()..   
+00002ac0: 2020 2020 2073 656c 662e 766f 6c75 6d65       self.volume
+00002ad0: 202b 3d20 766f 6c75 6d65 0d0a 2020 2020   += volume..    
+00002ae0: 2020 2020 7365 6c66 2e70 6f73 6974 696f      self.positio
+00002af0: 6e20 2b3d 2073 7465 7073 0d0a 2020 2020  n += steps..    
+00002b00: 2020 2020 6966 2072 6561 6765 6e74 2069      if reagent i
+00002b10: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00002b20: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00002b30: 6167 656e 7420 3d20 7265 6167 656e 740d  agent = reagent.
+00002b40: 0a20 2020 2020 2020 2069 6620 7061 7573  .        if paus
+00002b50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002b60: 696e 7075 7428 2250 7265 7373 2027 456e  input("Press 'En
+00002b70: 7465 7227 2074 6f20 7072 6f63 6565 642e  ter' to proceed.
+00002b80: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00002b90: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
+00002ba0: 200d 0a20 2020 2064 6566 2062 6c6f 776f   ..    def blowo
+00002bb0: 7574 2873 656c 662c 2068 6f6d 653a 626f  ut(self, home:bo
+00002bc0: 6f6c 203d 2054 7275 652c 202a 2a6b 7761  ol = True, **kwa
+00002bd0: 7267 7329 202d 3e20 7374 723a 0d0a 2020  rgs) -> str:..  
+00002be0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00002bf0: 2020 2042 6c6f 776f 7574 206c 6971 7569     Blowout liqui
+00002c00: 6420 6672 6f6d 2074 6970 0d0a 0d0a 2020  d from tip....  
+00002c10: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00002c20: 2020 2020 2020 2020 2068 6f6d 6520 2862           home (b
+00002c30: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+00002c40: 7768 6574 6865 7220 746f 2072 6574 7572  whether to retur
+00002c50: 6e20 706c 756e 6765 7220 746f 2068 6f6d  n plunger to hom
+00002c60: 6520 706f 7369 7469 6f6e 2e20 4465 6661  e position. Defa
+00002c70: 756c 7473 2074 6f20 5472 7565 2e0d 0a0d  ults to True....
+00002c80: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00002c90: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00002ca0: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
+00002cb0: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
+00002cc0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+00002cd0: 6420 3d20 6627 5242 7b73 656c 662e 686f  d = f'RB{self.ho
+00002ce0: 6d65 5f70 6f73 6974 696f 6e7d 2720 6966  me_position}' if
+00002cf0: 2068 6f6d 6520 656c 7365 2027 5242 270d   home else 'RB'.
+00002d00: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00002d10: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
+00002d20: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
+00002d30: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
+00002d40: 3d20 7365 6c66 2e68 6f6d 655f 706f 7369  = self.home_posi
+00002d50: 7469 6f6e 0d0a 2020 2020 2020 2020 7469  tion..        ti
+00002d60: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
+00002d70: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00002d80: 6f6e 7365 0d0a 2020 2020 0d0a 2020 2020  onse..    ..    
+00002d90: 6465 6620 6469 7370 656e 7365 2873 656c  def dispense(sel
+00002da0: 662c 200d 0a20 2020 2020 2020 2076 6f6c  f, ..        vol
+00002db0: 756d 653a 2066 6c6f 6174 2c20 0d0a 2020  ume: float, ..  
+00002dc0: 2020 2020 2020 7370 6565 643a 204f 7074        speed: Opt
+00002dd0: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
+00002de0: 6f6e 652c 200d 0a20 2020 2020 2020 2077  one, ..        w
+00002df0: 6169 743a 2069 6e74 203d 2030 2c20 0d0a  ait: int = 0, ..
+00002e00: 2020 2020 2020 2020 7061 7573 653a 2062          pause: b
+00002e10: 6f6f 6c20 3d20 4661 6c73 652c 200d 0a20  ool = False, .. 
+00002e20: 2020 2020 2020 2062 6c6f 776f 7574 3a20         blowout: 
+00002e30: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
+00002e40: 2020 2020 2020 2062 6c6f 776f 7574 5f68         blowout_h
+00002e50: 6f6d 653a 2062 6f6f 6c20 3d20 5472 7565  ome: bool = True
+00002e60: 2c0d 0a20 2020 2020 2020 2066 6f72 6365  ,..        force
+00002e70: 5f64 6973 7065 6e73 653a 2062 6f6f 6c20  _dispense: bool 
+00002e80: 3d20 4661 6c73 652c 200d 0a20 2020 2020  = False, ..     
+00002e90: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
+00002ea0: 2029 202d 3e20 7374 723a 0d0a 2020 2020   ) -> str:..    
+00002eb0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002ec0: 2044 6973 7065 6e73 6520 6465 7369 7265   Dispense desire
+00002ed0: 6420 766f 6c75 6d65 206f 6620 7265 6167  d volume of reag
+00002ee0: 656e 740d 0a0d 0a20 2020 2020 2020 2041  ent....        A
+00002ef0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00002f00: 2020 766f 6c75 6d65 2028 666c 6f61 7429    volume (float)
+00002f10: 3a20 7461 7267 6574 2076 6f6c 756d 650d  : target volume.
+00002f20: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
+00002f30: 6564 2028 4f70 7469 6f6e 616c 5b66 6c6f  ed (Optional[flo
+00002f40: 6174 5d2c 206f 7074 696f 6e61 6c29 3a20  at], optional): 
+00002f50: 7370 6565 6420 746f 2064 6973 7065 6e73  speed to dispens
+00002f60: 6520 6174 2e20 4465 6661 756c 7473 2074  e at. Defaults t
+00002f70: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
+00002f80: 2020 2020 2077 6169 7420 2869 6e74 2c20       wait (int, 
+00002f90: 6f70 7469 6f6e 616c 293a 2074 696d 6520  optional): time 
+00002fa0: 6465 6c61 7920 6166 7465 7220 6469 7370  delay after disp
+00002fb0: 656e 7365 2e20 4465 6661 756c 7473 2074  ense. Defaults t
+00002fc0: 6f20 302e 0d0a 2020 2020 2020 2020 2020  o 0...          
+00002fd0: 2020 7061 7573 6520 2862 6f6f 6c2c 206f    pause (bool, o
+00002fe0: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
+00002ff0: 7220 746f 2070 6175 7365 2066 6f72 2075  r to pause for u
+00003000: 7365 7220 696e 7465 7276 656e 7469 6f6e  ser intervention
+00003010: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
+00003020: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
+00003030: 2020 626c 6f77 6f75 7420 2862 6f6f 6c2c    blowout (bool,
+00003040: 206f 7074 696f 6e61 6c29 3a20 7768 6574   optional): whet
+00003050: 6865 7220 7065 7266 6f72 6d20 626c 6f77  her perform blow
+00003060: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
+00003070: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+00003080: 2020 2020 2062 6c6f 776f 7574 5f68 6f6d       blowout_hom
+00003090: 6520 2862 6f6f 6c2c 206f 7074 696f 6e61  e (bool, optiona
+000030a0: 6c29 3a20 7768 6574 6865 7220 746f 2072  l): whether to r
+000030b0: 6574 7572 6e20 7468 6520 706c 756e 6765  eturn the plunge
+000030c0: 7220 686f 6d65 2061 6674 6572 2062 6c6f  r home after blo
+000030d0: 776f 7574 2e20 4465 6661 756c 7473 2074  wout. Defaults t
+000030e0: 6f20 5472 7565 2e0d 0a20 2020 2020 2020  o True...       
+000030f0: 2020 2020 2066 6f72 6365 5f64 6973 7065       force_dispe
+00003100: 6e73 6520 2862 6f6f 6c2c 206f 7074 696f  nse (bool, optio
+00003110: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
+00003120: 2064 6973 7065 6e73 6520 7265 6167 656e   dispense reagen
+00003130: 7420 7265 6761 7264 6c65 7373 2e20 4465  t regardless. De
+00003140: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
+00003150: 0d0a 0d0a 2020 2020 2020 2020 5261 6973  ....        Rais
+00003160: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00003170: 2056 616c 7565 4572 726f 723a 2052 6571   ValueError: Req
+00003180: 7569 7265 6420 6469 7370 656e 7365 2076  uired dispense v
+00003190: 6f6c 756d 6520 6973 2067 7265 6174 6572  olume is greater
+000031a0: 2074 6861 6e20 766f 6c75 6d65 2069 6e20   than volume in 
+000031b0: 7469 700d 0a0d 0a20 2020 2020 2020 2052  tip....        R
+000031c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000031d0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+000031e0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+000031f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00003200: 7365 6c66 2e73 6574 466c 6167 2870 6175  self.setFlag(pau
+00003210: 7365 5f66 6565 6462 6163 6b3d 5472 7565  se_feedback=True
+00003220: 2c20 6f63 6375 7069 6564 3d54 7275 6529  , occupied=True)
+00003230: 0d0a 2020 2020 2020 2020 6966 2066 6f72  ..        if for
+00003240: 6365 5f64 6973 7065 6e73 653a 0d0a 2020  ce_dispense:..  
+00003250: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+00003260: 203d 206d 696e 2876 6f6c 756d 652c 2073   = min(volume, s
+00003270: 656c 662e 766f 6c75 6d65 290d 0a20 2020  elf.volume)..   
+00003280: 2020 2020 2065 6c69 6620 766f 6c75 6d65       elif volume
+00003290: 203e 2073 656c 662e 766f 6c75 6d65 3a0d   > self.volume:.
+000032a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000032b0: 7365 2056 616c 7565 4572 726f 7228 2752  se ValueError('R
+000032c0: 6571 7569 7265 6420 6469 7370 656e 7365  equired dispense
+000032d0: 2076 6f6c 756d 6520 6973 2067 7265 6174   volume is great
+000032e0: 6572 2074 6861 6e20 766f 6c75 6d65 2069  er than volume i
+000032f0: 6e20 7469 702e 2729 0d0a 2020 2020 2020  n tip.')..      
+00003300: 2020 7374 6570 7320 3d20 696e 7428 766f    steps = int(vo
+00003310: 6c75 6d65 202f 2073 656c 662e 7265 736f  lume / self.reso
+00003320: 6c75 7469 6f6e 290d 0a20 2020 2020 2020  lution)..       
+00003330: 2076 6f6c 756d 6520 3d20 7374 6570 7320   volume = steps 
+00003340: 2a20 7365 6c66 2e72 6573 6f6c 7574 696f  * self.resolutio
+00003350: 6e0d 0a20 2020 2020 2020 2069 6620 766f  n..        if vo
+00003360: 6c75 6d65 203d 3d20 303a 0d0a 2020 2020  lume == 0:..    
+00003370: 2020 2020 2020 2020 7265 7475 726e 2027          return '
+00003380: 270d 0a20 2020 2020 2020 2070 7269 6e74  '..        print
+00003390: 2866 2744 6973 7065 6e73 696e 6720 7b76  (f'Dispensing {v
+000033a0: 6f6c 756d 657d 2075 4c2e 2e2e 2729 0d0a  olume} uL...')..
+000033b0: 2020 2020 2020 2020 7374 6172 745f 6469          start_di
+000033c0: 7370 656e 7365 203d 2074 696d 652e 7065  spense = time.pe
+000033d0: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
+000033e0: 2020 2020 2020 7370 6565 6420 3d20 7365        speed = se
+000033f0: 6c66 2e73 7065 6564 2e64 6f77 6e20 6966  lf.speed.down if
+00003400: 2073 7065 6564 2069 7320 4e6f 6e65 2065   speed is None e
+00003410: 6c73 6520 7370 6565 640d 0a0d 0a20 2020  lse speed....   
+00003420: 2020 2020 2069 6620 7370 6565 6420 696e       if speed in
+00003430: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
+00003440: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
+00003450: 2020 6966 2073 7065 6564 2021 3d20 7365    if speed != se
+00003460: 6c66 2e73 7065 6564 2e64 6f77 6e3a 0d0a  lf.speed.down:..
+00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003480: 7365 6c66 2e73 6574 5370 6565 6428 7370  self.setSpeed(sp
+00003490: 6565 643d 7370 6565 642c 2075 703d 4661  eed=speed, up=Fa
+000034a0: 6c73 652c 2064 6566 6175 6c74 3d46 616c  lse, default=Fal
+000034b0: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
+000034c0: 2073 7461 7274 5f64 6973 7065 6e73 6520   start_dispense 
+000034d0: 3d20 7469 6d65 2e70 6572 665f 636f 756e  = time.perf_coun
+000034e0: 7465 7228 290d 0a20 2020 2020 2020 2020  ter()..         
+000034f0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00003500: 6c66 2e5f 7175 6572 7928 6627 524f 7b73  lf._query(f'RO{s
+00003510: 7465 7073 7d27 290d 0a20 2020 2020 2020  teps}')..       
+00003520: 2020 2020 206d 6f76 655f 7469 6d65 203d       move_time =
+00003530: 2073 7465 7073 2a73 656c 662e 7265 736f   steps*self.reso
+00003540: 6c75 7469 6f6e 202f 2073 7065 6564 0d0a  lution / speed..
+00003550: 2020 2020 2020 2020 2020 2020 6475 7261              dura
+00003560: 7469 6f6e 203d 2074 696d 652e 7065 7266  tion = time.perf
+00003570: 5f63 6f75 6e74 6572 2829 202d 2073 7461  _counter() - sta
+00003580: 7274 5f64 6973 7065 6e73 650d 0a20 2020  rt_dispense..   
+00003590: 2020 2020 2020 2020 2069 6620 6475 7261           if dura
+000035a0: 7469 6f6e 203c 2028 6d6f 7665 5f74 696d  tion < (move_tim
+000035b0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+000035c0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+000035d0: 6d6f 7665 5f74 696d 652d 6475 7261 7469  move_time-durati
+000035e0: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
+000035f0: 2023 2069 6620 7265 7370 6f6e 7365 2021   # if response !
+00003600: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
+00003610: 2020 2020 2023 2020 2020 2072 6574 7572       #     retur
+00003620: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00003630: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003640: 2020 656c 6966 2073 7065 6564 206e 6f74    elif speed not
+00003650: 2069 6e20 7365 6c66 2e73 7065 6564 5f70   in self.speed_p
+00003660: 7265 7365 7473 3a0d 0a20 2020 2020 2020  resets:..       
+00003670: 2020 2020 2070 7269 6e74 2866 2254 6172       print(f"Tar
+00003680: 6765 743a 207b 766f 6c75 6d65 7d20 754c  get: {volume} uL
+00003690: 2061 7420 7b73 7065 6564 7d20 754c 2f73   at {speed} uL/s
+000036a0: 2e2e 2e22 290d 0a20 2020 2020 2020 2020  ...")..         
+000036b0: 2020 2073 7065 6564 5f70 6172 616d 6574     speed_paramet
+000036c0: 6572 7320 3d20 7365 6c66 2e5f 6361 6c63  ers = self._calc
+000036d0: 756c 6174 655f 7370 6565 645f 7061 7261  ulate_speed_para
+000036e0: 6d65 7465 7273 2876 6f6c 756d 653d 766f  meters(volume=vo
+000036f0: 6c75 6d65 2c20 7370 6565 643d 7370 6565  lume, speed=spee
+00003700: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00003710: 7072 696e 7428 7370 6565 645f 7061 7261  print(speed_para
+00003720: 6d65 7465 7273 290d 0a20 2020 2020 2020  meters)..       
+00003730: 2020 2020 2070 7265 7365 7420 3d20 7370       preset = sp
+00003740: 6565 645f 7061 7261 6d65 7465 7273 2e70  eed_parameters.p
+00003750: 7265 7365 740d 0a20 2020 2020 2020 2020  reset..         
+00003760: 2020 2069 6620 7072 6573 6574 2069 7320     if preset is 
+00003770: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00003780: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00003790: 7469 6d65 4572 726f 7228 2754 6172 6765  timeError('Targe
+000037a0: 7420 7370 6565 6420 6e6f 7420 706f 7373  t speed not poss
+000037b0: 6962 6c65 2e27 290d 0a20 2020 2020 2020  ible.')..       
+000037c0: 2020 2020 2073 656c 662e 7365 7453 7065       self.setSpe
+000037d0: 6564 2873 7065 6564 3d70 7265 7365 742c  ed(speed=preset,
+000037e0: 2075 703d 4661 6c73 652c 2064 6566 6175   up=False, defau
+000037f0: 6c74 3d46 616c 7365 290d 0a20 2020 2020  lt=False)..     
+00003800: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00003810: 2073 7465 7073 5f6c 6566 7420 3d20 7374   steps_left = st
+00003820: 6570 730d 0a20 2020 2020 2020 2020 2020  eps..           
+00003830: 2064 656c 6179 203d 2073 7065 6564 5f70   delay = speed_p
+00003840: 6172 616d 6574 6572 732e 6465 6c61 790d  arameters.delay.
+00003850: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
+00003860: 705f 7369 7a65 203d 2073 7065 6564 5f70  p_size = speed_p
+00003870: 6172 616d 6574 6572 732e 7374 6570 5f73  arameters.step_s
+00003880: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
+00003890: 2069 6e74 6572 7661 6c73 203d 2073 7065   intervals = spe
+000038a0: 6564 5f70 6172 616d 6574 6572 732e 696e  ed_parameters.in
+000038b0: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
+000038c0: 2020 2020 2073 7461 7274 5f64 6973 7065       start_dispe
+000038d0: 6e73 6520 3d20 7469 6d65 2e70 6572 665f  nse = time.perf_
+000038e0: 636f 756e 7465 7228 290d 0a20 2020 2020  counter()..     
+000038f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00003900: 7261 6e67 6528 696e 7465 7276 616c 7329  range(intervals)
+00003910: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003920: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
+00003930: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
+00003940: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
+00003950: 2020 2020 2073 7465 7020 3d20 7374 6570       step = step
+00003960: 5f73 697a 6520 6966 2028 692b 3120 213d  _size if (i+1 !=
+00003970: 2069 6e74 6572 7661 6c73 2920 656c 7365   intervals) else
+00003980: 2073 7465 7073 5f6c 6566 740d 0a20 2020   steps_left..   
+00003990: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
+000039a0: 655f 7469 6d65 203d 2073 7465 702a 7365  e_time = step*se
+000039b0: 6c66 2e72 6573 6f6c 7574 696f 6e20 2f20  lf.resolution / 
+000039c0: 7072 6573 6574 0d0a 2020 2020 2020 2020  preset..        
+000039d0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000039e0: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
+000039f0: 2752 4f7b 7374 6570 7d27 2c20 7265 7375  'RO{step}', resu
+00003a00: 6d65 5f66 6565 6462 6163 6b3d 4661 6c73  me_feedback=Fals
+00003a10: 652c 2067 6574 5f70 6f73 6974 696f 6e3d  e, get_position=
+00003a20: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00003a30: 2020 2020 2020 2020 2320 6966 2072 6573          # if res
+00003a40: 706f 6e73 6520 213d 2027 6f6b 273a 0d0a  ponse != 'ok':..
+00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a60: 2320 2020 2020 7072 696e 7428 2244 6973  #     print("Dis
+00003a70: 7065 6e73 6520 6661 696c 6564 2229 0d0a  pense failed")..
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
+00003aa0: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
+00003ab0: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
+00003ac0: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
+00003ad0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+00003ae0: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
+00003af0: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
+00003b00: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
+00003b10: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
+00003b20: 696f 6e20 3c20 2864 656c 6179 2b6d 6f76  ion < (delay+mov
+00003b30: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
+00003b40: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00003b50: 6d65 2e73 6c65 6570 2864 656c 6179 2b6d  me.sleep(delay+m
+00003b60: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
+00003b70: 6e29 0d0a 0d0a 2020 2020 2020 2020 2320  n)....        # 
+00003b80: 5570 6461 7465 2076 616c 7565 730d 0a20  Update values.. 
+00003b90: 2020 2020 2020 2070 7269 6e74 2866 2744         print(f'D
+00003ba0: 6973 7065 6e73 6520 7469 6d65 3a20 7b74  ispense time: {t
+00003bb0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+00003bc0: 2829 2d73 7461 7274 5f64 6973 7065 6e73  ()-start_dispens
+00003bd0: 657d 7327 290d 0a20 2020 2020 2020 2074  e}s')..        t
+00003be0: 696d 652e 736c 6565 7028 7761 6974 290d  ime.sleep(wait).
+00003bf0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00003c00: 7446 6c61 6728 6f63 6375 7069 6564 3d46  tFlag(occupied=F
+00003c10: 616c 7365 2c20 7061 7573 655f 6665 6564  alse, pause_feed
+00003c20: 6261 636b 3d46 616c 7365 290d 0a20 2020  back=False)..   
+00003c30: 2020 2020 2073 656c 662e 6765 7450 6f73       self.getPos
+00003c40: 6974 696f 6e28 290d 0a20 2020 2020 2020  ition()..       
+00003c50: 2073 656c 662e 766f 6c75 6d65 203d 206d   self.volume = m
+00003c60: 6178 2873 656c 662e 766f 6c75 6d65 202d  ax(self.volume -
+00003c70: 2076 6f6c 756d 652c 2030 290d 0a20 2020   volume, 0)..   
+00003c80: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+00003c90: 6f6e 202d 3d20 7374 6570 730d 0a20 2020  on -= steps..   
+00003ca0: 2020 2020 2069 6620 7365 6c66 2e76 6f6c       if self.vol
+00003cb0: 756d 6520 3d3d 2030 2061 6e64 2062 6c6f  ume == 0 and blo
+00003cc0: 776f 7574 3a0d 0a20 2020 2020 2020 2020  wout:..         
+00003cd0: 2020 2073 656c 662e 626c 6f77 6f75 7428     self.blowout(
+00003ce0: 686f 6d65 3d62 6c6f 776f 7574 5f68 6f6d  home=blowout_hom
+00003cf0: 6529 0d0a 2020 2020 2020 2020 6966 2070  e)..        if p
+00003d00: 6175 7365 3a0d 0a20 2020 2020 2020 2020  ause:..         
+00003d10: 2020 2069 6e70 7574 2822 5072 6573 7320     input("Press 
+00003d20: 2745 6e74 6572 2720 746f 2070 726f 6365  'Enter' to proce
+00003d30: 6564 2e22 290d 0a20 2020 2020 2020 2072  ed.")..        r
+00003d40: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00003d50: 2020 2020 0d0a 2020 2020 6465 6620 656a      ..    def ej
+00003d60: 6563 7428 7365 6c66 2c20 686f 6d65 3a62  ect(self, home:b
+00003d70: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2073  ool = True) -> s
+00003d80: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+00003d90: 0d0a 2020 2020 2020 2020 456a 6563 7420  ..        Eject 
+00003da0: 7468 6520 7069 7065 7474 6520 7469 700d  the pipette tip.
+00003db0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00003dc0: 0d0a 2020 2020 2020 2020 2020 2020 686f  ..            ho
+00003dd0: 6d65 2028 626f 6f6c 2c20 6f70 7469 6f6e  me (bool, option
+00003de0: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
+00003df0: 7265 7475 726e 2070 6c75 6e67 6572 2074  return plunger t
+00003e00: 6f20 686f 6d65 2070 6f73 6974 696f 6e2e  o home position.
+00003e10: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
+00003e20: 652e 0d0a 0d0a 2020 2020 2020 2020 5265  e.....        Re
+00003e30: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00003e40: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
+00003e50: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00003e60: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
+00003e70: 656c 662e 7265 6167 656e 7420 3d20 2727  elf.reagent = ''
+00003e80: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+00003e90: 6420 3d20 6627 5245 7b73 656c 662e 686f  d = f'RE{self.ho
+00003ea0: 6d65 5f70 6f73 6974 696f 6e7d 2720 6966  me_position}' if
+00003eb0: 2068 6f6d 6520 656c 7365 2027 5245 270d   home else 'RE'.
+00003ec0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00003ed0: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
+00003ee0: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
+00003ef0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
+00003f00: 3d20 7365 6c66 2e68 6f6d 655f 706f 7369  = self.home_posi
+00003f10: 7469 6f6e 2069 6620 686f 6d65 2065 6c73  tion if home els
+00003f20: 6520 300d 0a20 2020 2020 2020 2074 696d  e 0..        tim
+00003f30: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
+00003f40: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00003f50: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
+00003f60: 6566 2065 6d70 7479 2873 656c 662c 202a  ef empty(self, *
+00003f70: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00003f80: 2020 2022 2222 456d 7074 7920 7468 6520     """Empty the 
+00003f90: 7069 7065 7474 6522 2222 0d0a 2020 2020  pipette"""..    
+00003fa0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00003fb0: 686f 6d65 2829 0d0a 2020 2020 0d0a 2020  home()..    ..  
+00003fc0: 2020 6465 6620 6765 7443 6170 6163 6974    def getCapacit
+00003fd0: 616e 6365 2873 656c 6629 202d 3e20 556e  ance(self) -> Un
+00003fe0: 696f 6e5b 696e 742c 2073 7472 5d3a 0d0a  ion[int, str]:..
+00003ff0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004000: 2020 2020 2047 6574 2074 6865 2063 6170       Get the cap
+00004010: 6163 6974 616e 6365 2061 7320 6d65 6173  acitance as meas
+00004020: 7572 6564 2061 7420 7468 6520 656e 6420  ured at the end 
+00004030: 6f66 2074 6865 2070 6970 6574 7465 0d0a  of the pipette..
+00004040: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00004050: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00004060: 2020 2020 2020 2020 556e 696f 6e5b 696e          Union[in
+00004070: 742c 2073 7472 5d3a 2063 6170 6163 6974  t, str]: capacit
+00004080: 616e 6365 2076 616c 7565 2c20 6f72 2064  ance value, or d
+00004090: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
+000040a0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000040b0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+000040c0: 7365 6c66 2e5f 7175 6572 7928 2744 4e27  self._query('DN'
+000040d0: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
+000040e0: 0a20 2020 2020 2020 2020 2020 2063 6170  .            cap
+000040f0: 6163 6974 616e 6365 203d 2069 6e74 2872  acitance = int(r
+00004100: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
+00004110: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00004120: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00004130: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00004140: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00004150: 5f63 6170 6163 6974 616e 6365 203d 2063  _capacitance = c
+00004160: 6170 6163 6974 616e 6365 0d0a 2020 2020  apacitance..    
+00004170: 2020 2020 7265 7475 726e 2063 6170 6163      return capac
+00004180: 6974 616e 6365 0d0a 200d 0a20 2020 2064  itance.. ..    d
+00004190: 6566 2067 6574 4572 726f 7273 2873 656c  ef getErrors(sel
+000041a0: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
+000041b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000041c0: 2047 6574 2065 7272 6f72 7320 6672 6f6d   Get errors from
+000041d0: 2074 6865 2064 6576 6963 650d 0a0d 0a20   the device.... 
+000041e0: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+000041f0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00004200: 3a20 6465 7669 6365 2072 6573 706f 6e73  : device respons
+00004210: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+00004220: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00004230: 656c 662e 5f71 7565 7279 2827 4445 2729  elf._query('DE')
+00004240: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00004250: 6765 7449 6e66 6f28 7365 6c66 2c20 6d6f  getInfo(self, mo
+00004260: 6465 6c3a 204f 7074 696f 6e61 6c5b 7374  del: Optional[st
+00004270: 725d 203d 204e 6f6e 6529 3a0d 0a20 2020  r] = None):..   
+00004280: 2020 2020 2022 2222 4765 7420 6465 7461       """Get deta
+00004290: 696c 7320 6f66 2074 6865 2053 6172 746f  ils of the Sarto
+000042a0: 7269 7573 2070 6970 6574 7465 206d 6f64  rius pipette mod
+000042b0: 656c 2222 220d 0a20 2020 2020 2020 206d  el"""..        m
+000042c0: 6f64 656c 203d 2073 656c 662e 5f5f 6d6f  odel = self.__mo
+000042d0: 6465 6c5f 5f28 292e 7370 6c69 7428 272d  del__().split('-
+000042e0: 2729 5b30 5d20 6966 206d 6f64 656c 2069  ')[0] if model i
+000042f0: 7320 4e6f 6e65 2065 6c73 6520 6d6f 6465  s None else mode
+00004300: 6c0d 0a20 2020 2020 2020 2069 6620 6d6f  l..        if mo
+00004310: 6465 6c20 6e6f 7420 696e 204d 6f64 656c  del not in Model
+00004320: 496e 666f 2e5f 6d65 6d62 6572 5f6e 616d  Info._member_nam
+00004330: 6573 5f3a 0d0a 2020 2020 2020 2020 2020  es_:..          
+00004340: 2020 7072 696e 7428 6627 5265 6365 6976    print(f'Receiv
+00004350: 6564 3a20 7b6d 6f64 656c 7d27 290d 0a20  ed: {model}').. 
+00004360: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+00004370: 203d 2027 4252 4c30 270d 0a20 2020 2020   = 'BRL0'..     
+00004380: 2020 2020 2020 2070 7269 6e74 2866 2244         print(f"D
+00004390: 6566 6175 6c74 696e 6720 746f 3a20 7b27  efaulting to: {'
+000043a0: 4252 4c30 277d 2229 0d0a 2020 2020 2020  BRL0'}")..      
+000043b0: 2020 2020 2020 7072 696e 7428 6622 5661        print(f"Va
+000043c0: 6c69 6420 6d6f 6465 6c73 2061 7265 3a20  lid models are: 
+000043d0: 7b27 2c20 272e 6a6f 696e 284d 6f64 656c  {', '.join(Model
+000043e0: 496e 666f 2e5f 6d65 6d62 6572 5f6e 616d  Info._member_nam
+000043f0: 6573 5f29 7d22 290d 0a20 2020 2020 2020  es_)}")..       
+00004400: 2069 6e66 6f3a 204d 6f64 656c 203d 204d   info: Model = M
+00004410: 6f64 656c 496e 666f 5b6d 6f64 656c 5d2e  odelInfo[model].
+00004420: 7661 6c75 650d 0a20 2020 2020 2020 2070  value..        p
+00004430: 7269 6e74 2869 6e66 6f29 0d0a 2020 2020  rint(info)..    
+00004440: 2020 2020 7365 6c66 2e6d 6f64 656c 5f69      self.model_i
+00004450: 6e66 6f20 3d20 696e 666f 0d0a 2020 2020  nfo = info..    
+00004460: 2020 2020 7365 6c66 2e63 6170 6163 6974      self.capacit
+00004470: 7920 3d20 696e 666f 2e63 6170 6163 6974  y = info.capacit
+00004480: 790d 0a20 2020 2020 2020 2073 656c 662e  y..        self.
+00004490: 6c69 6d69 7473 203d 2028 696e 666f 2e74  limits = (info.t
+000044a0: 6970 5f65 6a65 6374 5f70 6f73 6974 696f  ip_eject_positio
+000044b0: 6e2c 2069 6e66 6f2e 6d61 785f 706f 7369  n, info.max_posi
+000044c0: 7469 6f6e 290d 0a20 2020 2020 2020 2073  tion)..        s
+000044d0: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
+000044e0: 7320 3d20 696e 666f 2e70 7265 7365 745f  s = info.preset_
+000044f0: 7370 6565 6473 0d0a 2020 2020 2020 2020  speeds..        
+00004500: 7365 6c66 2e73 7065 6564 2e75 7020 3d20  self.speed.up = 
+00004510: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
+00004520: 7473 5b73 656c 662e 7370 6565 645f 636f  ts[self.speed_co
+00004530: 6465 2e75 702d 315d 0d0a 2020 2020 2020  de.up-1]..      
+00004540: 2020 7365 6c66 2e73 7065 6564 2e64 6f77    self.speed.dow
+00004550: 6e20 3d20 7365 6c66 2e73 7065 6564 5f70  n = self.speed_p
+00004560: 7265 7365 7473 5b73 656c 662e 7370 6565  resets[self.spee
+00004570: 645f 636f 6465 2e64 6f77 6e2d 315d 0d0a  d_code.down-1]..
+00004580: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00004590: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
+000045a0: 7450 6f73 6974 696f 6e28 7365 6c66 2c20  tPosition(self, 
+000045b0: 2a2a 6b77 6172 6773 2920 2d3e 2069 6e74  **kwargs) -> int
+000045c0: 3a0d 0a20 2020 2020 2020 2022 2222 4765  :..        """Ge
+000045d0: 7420 7468 6520 6375 7272 656e 7420 706f  t the current po
+000045e0: 7369 7469 6f6e 206f 6620 7468 6520 7069  sition of the pi
+000045f0: 7065 7474 6522 2222 0d0a 2020 2020 2020  pette"""..      
+00004600: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00004610: 662e 5f71 7565 7279 2827 4450 2729 0d0a  f._query('DP')..
+00004620: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00004630: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+00004640: 6f6e 203d 2069 6e74 2872 6573 706f 6e73  on = int(respons
+00004650: 6529 0d0a 2020 2020 2020 2020 6578 6365  e)..        exce
+00004660: 7074 2056 616c 7565 4572 726f 723a 0d0a  pt ValueError:..
+00004670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004680: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
+00004690: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+000046a0: 6f6e 203d 2070 6f73 6974 696f 6e0d 0a20  on = position.. 
+000046b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000046c0: 6c66 2e70 6f73 6974 696f 6e0d 0a20 2020  lf.position..   
+000046d0: 2020 200d 0a20 2020 2064 6566 2067 6574     ..    def get
+000046e0: 5374 6174 7573 2873 656c 662c 202a 2a6b  Status(self, **k
+000046f0: 7761 7267 7329 202d 3e20 7374 723a 0d0a  wargs) -> str:..
+00004700: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004710: 2020 2020 2047 6574 2074 6865 2073 7461       Get the sta
+00004720: 7475 7320 6f66 2074 6865 2070 6970 6574  tus of the pipet
+00004730: 7465 0d0a 0d0a 2020 2020 2020 2020 5265  te....        Re
+00004740: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00004750: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
+00004760: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00004770: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00004780: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00004790: 7175 6572 7928 2744 5327 290d 0a20 2020  query('DS')..   
+000047a0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+000047b0: 2020 2020 2020 2073 7461 7475 7320 3d20         status = 
+000047c0: 696e 7428 7265 7370 6f6e 7365 290d 0a20  int(response).. 
+000047d0: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+000047e0: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
+000047f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00004800: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+00004810: 6966 2072 6573 706f 6e73 6520 6e6f 7420  if response not 
+00004820: 696e 205b 5f73 7461 7475 732e 7661 6c75  in [_status.valu
+00004830: 6520 666f 7220 5f73 7461 7475 7320 696e  e for _status in
+00004840: 2053 7461 7475 7343 6f64 655d 3a0d 0a20   StatusCode]:.. 
+00004850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00004860: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00004870: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+00004880: 6c66 2e5f 7374 6174 7573 5f63 6f64 6520  lf._status_code 
+00004890: 3d20 7374 6174 7573 0d0a 2020 2020 2020  = status..      
+000048a0: 2020 6966 2073 7461 7475 7320 696e 205b    if status in [
+000048b0: 342c 362c 385d 3a0d 0a20 2020 2020 2020  4,6,8]:..       
+000048c0: 2020 2020 2073 656c 662e 7365 7446 6c61       self.setFla
+000048d0: 6728 6275 7379 3d54 7275 6529 0d0a 2020  g(busy=True)..  
+000048e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000048f0: 662e 7665 7262 6f73 653a 0d0a 2020 2020  f.verbose:..    
+00004900: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00004910: 7428 5374 6174 7573 436f 6465 2873 7461  t(StatusCode(sta
+00004920: 7475 7329 2e6e 616d 6529 0d0a 2020 2020  tus).name)..    
+00004930: 2020 2020 656c 6966 2073 7461 7475 7320      elif status 
+00004940: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+00004950: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
+00004960: 6275 7379 3d46 616c 7365 290d 0a20 2020  busy=False)..   
+00004970: 2020 2020 2072 6574 7572 6e20 5374 6174       return Stat
+00004980: 7573 436f 6465 2873 656c 662e 5f73 7461  usCode(self._sta
+00004990: 7475 735f 636f 6465 292e 6e61 6d65 0d0a  tus_code).name..
+000049a0: 2020 2020 0d0a 2020 2020 6465 6620 686f      ..    def ho
+000049b0: 6d65 2873 656c 6629 202d 3e20 7374 723a  me(self) -> str:
+000049c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000049d0: 2020 2020 2020 2052 6574 7572 6e20 706c         Return pl
+000049e0: 756e 6765 7220 746f 2068 6f6d 6520 706f  unger to home po
+000049f0: 7369 7469 6f6e 0d0a 2020 2020 2020 2020  sition..        
+00004a00: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00004a10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004a20: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
+00004a30: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
+00004a40: 220d 0a20 2020 2020 2020 2072 6573 706f  "..        respo
+00004a50: 6e73 6520 3d20 7365 6c66 2e5f 7175 6572  nse = self._quer
+00004a60: 7928 6627 5250 7b73 656c 662e 686f 6d65  y(f'RP{self.home
+00004a70: 5f70 6f73 6974 696f 6e7d 2729 0d0a 2020  _position}')..  
+00004a80: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
+00004a90: 6520 3d20 300d 0a20 2020 2020 2020 2073  e = 0..        s
+00004aa0: 656c 662e 706f 7369 7469 6f6e 203d 2073  elf.position = s
+00004ab0: 656c 662e 686f 6d65 5f70 6f73 6974 696f  elf.home_positio
+00004ac0: 6e0d 0a20 2020 2020 2020 2074 696d 652e  n..        time.
+00004ad0: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
+00004ae0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00004af0: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
+00004b00: 2069 7346 6561 7369 626c 6528 7365 6c66   isFeasible(self
+00004b10: 2c20 706f 7369 7469 6f6e 3a69 6e74 2920  , position:int) 
+00004b20: 2d3e 2062 6f6f 6c3a 0d0a 2020 2020 2020  -> bool:..      
+00004b30: 2020 2222 220d 0a20 2020 2020 2020 2043    """..        C
+00004b40: 6865 636b 7320 616e 6420 7265 7475 726e  hecks and return
+00004b50: 7320 7768 6574 6865 7220 7468 6520 706c  s whether the pl
+00004b60: 756e 6765 7220 706f 7369 7469 6f6e 2069  unger position i
+00004b70: 7320 6665 6173 6962 6c65 0d0a 0d0a 2020  s feasible....  
+00004b80: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00004b90: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
+00004ba0: 6e20 2869 6e74 293a 2070 6c75 6e67 6572  n (int): plunger
+00004bb0: 2070 6f73 6974 696f 6e0d 0a0d 0a20 2020   position....   
+00004bc0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+00004bd0: 2020 2020 2020 2020 2020 2062 6f6f 6c3a             bool:
+00004be0: 2077 6865 7468 6572 2070 6c75 6e67 6572   whether plunger
+00004bf0: 2070 6f73 6974 696f 6e20 6973 2066 6561   position is fea
+00004c00: 7369 626c 650d 0a20 2020 2020 2020 2022  sible..        "
+00004c10: 2222 0d0a 2020 2020 2020 2020 6966 2028  ""..        if (
+00004c20: 7365 6c66 2e6c 696d 6974 735b 305d 203c  self.limits[0] <
+00004c30: 3d20 706f 7369 7469 6f6e 203c 3d20 7365  = position <= se
+00004c40: 6c66 2e6c 696d 6974 735b 315d 293a 0d0a  lf.limits[1]):..
+00004c50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004c60: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
+00004c70: 2070 7269 6e74 2866 2252 616e 6765 206c   print(f"Range l
+00004c80: 696d 6974 7320 7265 6163 6865 6421 207b  imits reached! {
+00004c90: 7365 6c66 2e6c 696d 6974 737d 2229 0d0a  self.limits}")..
+00004ca0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00004cb0: 616c 7365 0d0a 2020 2020 0d0a 2020 2020  alse..    ..    
+00004cc0: 6465 6620 6973 5469 704f 6e28 7365 6c66  def isTipOn(self
+00004cd0: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
+00004ce0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00004cf0: 2043 6865 636b 7320 616e 6420 7265 7475   Checks and retu
+00004d00: 726e 7320 7768 6574 6865 7220 6120 7069  rns whether a pi
+00004d10: 7065 7474 6520 7469 7020 6973 2061 7474  pette tip is att
+00004d20: 6163 6865 640d 0a20 2020 2020 2020 200d  ached..        .
+00004d30: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00004d40: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
+00004d50: 6f6f 6c3a 2077 6865 7468 6572 2061 2070  ool: whether a p
+00004d60: 6970 6574 7465 2074 6970 2069 6e20 6174  ipette tip in at
+00004d70: 7461 6368 6564 0d0a 2020 2020 2020 2020  tached..        
+00004d80: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00004d90: 662e 6765 7443 6170 6163 6974 616e 6365  f.getCapacitance
+00004da0: 2829 0d0a 2020 2020 2020 2020 7072 696e  ()..        prin
+00004db0: 7428 6627 5469 7020 6361 7061 6369 7461  t(f'Tip capacita
+00004dc0: 6e63 653a 207b 7365 6c66 2e63 6170 6163  nce: {self.capac
+00004dd0: 6974 616e 6365 7d27 290d 0a20 2020 2020  itance}')..     
+00004de0: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
+00004df0: 5b27 636f 6e64 7563 7469 7665 5f74 6970  ['conductive_tip
+00004e00: 7327 5d3a 0d0a 2020 2020 2020 2020 2020  s']:..          
+00004e10: 2020 7469 705f 6f6e 203d 2028 7365 6c66    tip_on = (self
+00004e20: 2e63 6170 6163 6974 616e 6365 203e 2073  .capacitance > s
+00004e30: 656c 662e 7469 705f 7468 7265 7368 6f6c  elf.tip_threshol
+00004e40: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00004e50: 7365 6c66 2e73 6574 466c 6167 2874 6970  self.setFlag(tip
+00004e60: 5f6f 6e3d 7469 705f 6f6e 290d 0a20 2020  _on=tip_on)..   
+00004e70: 2020 2020 2074 6970 5f6f 6e20 3d20 7365       tip_on = se
+00004e80: 6c66 2e66 6c61 6773 5b27 7469 705f 6f6e  lf.flags['tip_on
+00004e90: 275d 0d0a 2020 2020 2020 2020 7265 7475  ']..        retu
+00004ea0: 726e 2074 6970 5f6f 6e0d 0a20 2020 200d  rn tip_on..    .
+00004eb0: 0a20 2020 2064 6566 206d 6f76 6528 7365  .    def move(se
+00004ec0: 6c66 2c20 7374 6570 733a 696e 742c 2075  lf, steps:int, u
+00004ed0: 703a 626f 6f6c 2c20 2a2a 6b77 6172 6773  p:bool, **kwargs
+00004ee0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00004ef0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004f00: 4d6f 7665 2074 6865 2070 6c75 6e67 6572  Move the plunger
+00004f10: 2065 6974 6865 7220 7570 206f 7220 646f   either up or do
+00004f20: 776e 2062 7920 6120 7370 6563 6966 6965  wn by a specifie
+00004f30: 6420 6e75 6d62 6572 206f 6620 7374 6570  d number of step
+00004f40: 730d 0a0d 0a20 2020 2020 2020 2041 7267  s....        Arg
+00004f50: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004f60: 7374 6570 7320 2869 6e74 293a 206e 756d  steps (int): num
+00004f70: 6265 7220 6f66 2073 7465 7073 2074 6f20  ber of steps to 
+00004f80: 6d6f 7665 2070 6c75 6e67 6572 2062 790d  move plunger by.
+00004f90: 0a20 2020 2020 2020 2020 2020 2075 7020  .            up 
+00004fa0: 2862 6f6f 6c29 3a20 7768 6574 6865 7220  (bool): whether 
+00004fb0: 746f 206d 6f76 6520 7468 6520 706c 756e  to move the plun
+00004fc0: 6765 7220 7570 0d0a 0d0a 2020 2020 2020  ger up....      
+00004fd0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00004fe0: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
+00004ff0: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
+00005000: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00005010: 2020 2073 7465 7073 203d 2061 6273 2873     steps = abs(s
+00005020: 7465 7073 2920 6966 2075 7020 656c 7365  teps) if up else
+00005030: 202d 6162 7328 7374 6570 7329 0d0a 2020   -abs(steps)..  
+00005040: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00005050: 662e 6d6f 7665 4279 2873 7465 7073 290d  f.moveBy(steps).
+00005060: 0a20 2020 200d 0a20 2020 2064 6566 206d  .    ..    def m
+00005070: 6f76 6542 7928 7365 6c66 2c20 7374 6570  oveBy(self, step
+00005080: 733a 696e 742c 202a 2a6b 7761 7267 7329  s:int, **kwargs)
+00005090: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
+000050a0: 2020 2222 220d 0a20 2020 2020 2020 204d    """..        M
+000050b0: 6f76 6520 7468 6520 706c 756e 6765 7220  ove the plunger 
+000050c0: 6279 2073 7065 6369 6669 6564 206e 756d  by specified num
+000050d0: 6265 7220 6f66 2073 7465 7073 0d0a 0d0a  ber of steps....
+000050e0: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+000050f0: 2020 2020 2020 2020 2020 2073 7465 7073             steps
+00005100: 2028 696e 7429 3a20 6e75 6d62 6572 206f   (int): number o
+00005110: 6620 7374 6570 7320 746f 206d 6f76 6520  f steps to move 
+00005120: 706c 756e 6765 7220 6279 2028 3c30 3a20  plunger by (<0: 
+00005130: 6d6f 7665 2064 6f77 6e2f 6469 7370 656e  move down/dispen
+00005140: 7365 3b20 3e30 206d 6f76 6520 7570 2f61  se; >0 move up/a
+00005150: 7370 6972 6174 6529 0d0a 0d0a 2020 2020  spirate)....    
+00005160: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00005170: 2020 2020 2020 2020 2020 7374 723a 2064            str: d
+00005180: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
+00005190: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000051a0: 2020 2020 2063 6f6d 6d61 6e64 203d 2066       command = f
+000051b0: 2752 497b 7374 6570 737d 2720 6966 2073  'RI{steps}' if s
+000051c0: 7465 7073 203e 2030 2065 6c73 6520 6627  teps > 0 else f'
+000051d0: 524f 7b2d 7374 6570 737d 270d 0a20 2020  RO{-steps}'..   
+000051e0: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+000051f0: 6f6e 202b 3d20 7374 6570 730d 0a20 2020  on += steps..   
+00005200: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00005210: 2e5f 7175 6572 7928 636f 6d6d 616e 6429  ._query(command)
+00005220: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00005230: 6d6f 7665 546f 2873 656c 662c 2070 6f73  moveTo(self, pos
+00005240: 6974 696f 6e3a 696e 742c 202a 2a6b 7761  ition:int, **kwa
+00005250: 7267 7329 202d 3e20 7374 723a 0d0a 2020  rgs) -> str:..  
+00005260: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00005270: 2020 204d 6f76 6520 7468 6520 706c 756e     Move the plun
+00005280: 6765 7220 746f 2061 2073 7065 6369 6669  ger to a specifi
+00005290: 6564 2070 6f73 6974 696f 6e0d 0a0d 0a20  ed position.... 
+000052a0: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+000052b0: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+000052c0: 6f6e 2028 696e 7429 3a20 7461 7267 6574  on (int): target
+000052d0: 2070 6c75 6e67 6572 2070 6f73 6974 696f   plunger positio
+000052e0: 6e0d 0a0d 0a20 2020 2020 2020 2052 6574  n....        Ret
+000052f0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00005300: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+00005310: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00005320: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+00005330: 6c66 2e70 6f73 6974 696f 6e20 3d20 706f  lf.position = po
+00005340: 7369 7469 6f6e 0d0a 2020 2020 2020 2020  sition..        
+00005350: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
+00005360: 7279 2866 2752 507b 706f 7369 7469 6f6e  ry(f'RP{position
+00005370: 7d27 290d 0a20 2020 200d 0a20 2020 2064  }')..    ..    d
+00005380: 6566 2070 756c 6c62 6163 6b28 7365 6c66  ef pullback(self
+00005390: 2c20 7374 6570 733a 696e 7420 3d20 352c  , steps:int = 5,
+000053a0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
+000053b0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+000053c0: 0a20 2020 2020 2020 2050 756c 6c62 6163  .        Pullbac
+000053d0: 6b20 6c69 7175 6964 2066 726f 6d20 7469  k liquid from ti
+000053e0: 700d 0a20 2020 2020 2020 200d 0a20 2020  p..        ..   
+000053f0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+00005400: 2020 2020 2020 2020 7374 6570 7320 2869          steps (i
+00005410: 6e74 2c20 6f70 7469 6f6e 616c 293a 206e  nt, optional): n
+00005420: 756d 6265 7220 6f66 2073 7465 7073 2074  umber of steps t
+00005430: 6f20 7075 6c6c 6261 636b 2e20 4465 6661  o pullback. Defa
+00005440: 756c 7473 2074 6f20 352e 0d0a 0d0a 2020  ults to 5.....  
+00005450: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005460: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00005470: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00005480: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005490: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000054a0: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
+000054b0: 5249 7b73 7465 7073 7d27 290d 0a20 2020  RI{steps}')..   
+000054c0: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+000054d0: 6f6e 202b 3d20 7374 6570 730d 0a20 2020  on += steps..   
+000054e0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+000054f0: 3129 0d0a 2020 2020 2020 2020 7265 7475  1)..        retu
+00005500: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
+00005510: 200d 0a20 2020 2064 6566 2072 6573 6574   ..    def reset
+00005520: 2873 656c 6629 202d 3e20 7374 723a 0d0a  (self) -> str:..
+00005530: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00005540: 2020 2020 2052 6573 6574 2074 6865 2070       Reset the p
+00005550: 6970 6574 7465 0d0a 0d0a 2020 2020 2020  ipette....      
+00005560: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00005570: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
+00005580: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
+00005590: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000055a0: 2020 2073 656c 662e 7a65 726f 2829 0d0a     self.zero()..
+000055b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000055c0: 656c 662e 686f 6d65 2829 0d0a 2020 2020  elf.home()..    
+000055d0: 0d0a 2020 2020 6465 6620 7365 7453 7065  ..    def setSpe
+000055e0: 6564 2873 656c 662c 2073 7065 6564 3a69  ed(self, speed:i
+000055f0: 6e74 2c20 7570 3a62 6f6f 6c2c 2064 6566  nt, up:bool, def
+00005600: 6175 6c74 3a62 6f6f 6c20 3d20 5472 7565  ault:bool = True
+00005610: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2073  , **kwargs) -> s
+00005620: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+00005630: 0d0a 2020 2020 2020 2020 5365 7420 7468  ..        Set th
+00005640: 6520 7370 6565 6420 6f66 2074 6865 2070  e speed of the p
+00005650: 6c75 6e67 6572 0d0a 0d0a 2020 2020 2020  lunger....      
+00005660: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+00005670: 2020 2020 2073 7065 6564 2028 696e 7429       speed (int)
+00005680: 3a20 7370 6565 6420 6f66 2070 6c75 6e67  : speed of plung
+00005690: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+000056a0: 7570 2028 626f 6f6c 293a 2064 6972 6563  up (bool): direc
+000056b0: 7469 6f6e 206f 6620 7472 6176 656c 0d0a  tion of travel..
+000056c0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+000056d0: 756c 7420 2862 6f6f 6c2c 206f 7074 696f  ult (bool, optio
+000056e0: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
+000056f0: 2073 6574 2073 7065 6564 2061 7320 6120   set speed as a 
+00005700: 6465 6661 756c 742e 2044 6566 6175 6c74  default. Default
+00005710: 7320 746f 2054 7275 652e 0d0a 0d0a 2020  s to True.....  
+00005720: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005730: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00005740: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00005750: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005760: 2020 2020 2020 2073 7065 6564 5f63 6f64         speed_cod
+00005770: 6520 3d20 3120 2b20 5b78 2066 6f72 2078  e = 1 + [x for x
+00005780: 2c76 616c 2069 6e20 656e 756d 6572 6174  ,val in enumerat
+00005790: 6528 6e70 2e61 7272 6179 2873 656c 662e  e(np.array(self.
+000057a0: 7370 6565 645f 7072 6573 6574 7329 2d73  speed_presets)-s
+000057b0: 7065 6564 2920 6966 2076 616c 203e 3d20  peed) if val >= 
+000057c0: 305d 5b30 5d0d 0a20 2020 2020 2020 2070  0][0]..        p
+000057d0: 7269 6e74 2866 2753 7065 6564 207b 7370  rint(f'Speed {sp
+000057e0: 6565 645f 636f 6465 7d3a 207b 7365 6c66  eed_code}: {self
+000057f0: 2e73 7065 6564 5f70 7265 7365 7473 5b73  .speed_presets[s
+00005800: 7065 6564 5f63 6f64 652d 315d 7d20 754c  peed_code-1]} uL
+00005810: 2f73 2729 0d0a 2020 2020 2020 2020 6469  /s')..        di
+00005820: 7265 6374 696f 6e20 3d20 2749 2720 6966  rection = 'I' if
+00005830: 2075 7020 656c 7365 2027 4f27 0d0a 2020   up else 'O'..  
+00005840: 2020 2020 2020 7365 6c66 2e5f 7175 6572        self._quer
+00005850: 7928 6627 537b 6469 7265 6374 696f 6e7d  y(f'S{direction}
+00005860: 7b73 7065 6564 5f63 6f64 657d 2729 0d0a  {speed_code}')..
+00005870: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+00005880: 6566 6175 6c74 3a0d 0a20 2020 2020 2020  efault:..       
+00005890: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000058a0: 2e5f 7175 6572 7928 6627 447b 6469 7265  ._query(f'D{dire
+000058b0: 6374 696f 6e7d 2729 0d0a 2020 2020 2020  ction}')..      
+000058c0: 2020 6966 2075 703a 0d0a 2020 2020 2020    if up:..      
+000058d0: 2020 2020 2020 7365 6c66 2e73 7065 6564        self.speed
+000058e0: 5f63 6f64 652e 7570 203d 2073 7065 6564  _code.up = speed
+000058f0: 5f63 6f64 650d 0a20 2020 2020 2020 2020  _code..         
+00005900: 2020 2073 656c 662e 7370 6565 642e 7570     self.speed.up
+00005910: 203d 2073 656c 662e 7370 6565 645f 7072   = self.speed_pr
+00005920: 6573 6574 735b 7370 6565 645f 636f 6465  esets[speed_code
+00005930: 2d31 5d0d 0a20 2020 2020 2020 2065 6c73  -1]..        els
+00005940: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00005950: 7365 6c66 2e73 7065 6564 5f63 6f64 652e  self.speed_code.
+00005960: 646f 776e 203d 2073 7065 6564 5f63 6f64  down = speed_cod
+00005970: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
+00005980: 656c 662e 7370 6565 642e 646f 776e 203d  elf.speed.down =
+00005990: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
+000059a0: 6574 735b 7370 6565 645f 636f 6465 2d31  ets[speed_code-1
+000059b0: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+000059c0: 6e20 7365 6c66 2e5f 7175 6572 7928 6627  n self._query(f'
+000059d0: 447b 6469 7265 6374 696f 6e7d 2729 0d0a  D{direction}')..
+000059e0: 2020 2020 0d0a 2020 2020 6465 6620 7368      ..    def sh
+000059f0: 7574 646f 776e 2873 656c 6629 3a0d 0a20  utdown(self):.. 
+00005a00: 2020 2020 2020 2022 2222 5368 7574 646f         """Shutdo
+00005a10: 776e 2070 726f 6365 6475 7265 2066 6f72  wn procedure for
+00005a20: 2074 6f6f 6c22 2222 0d0a 2020 2020 2020   tool"""..      
+00005a30: 2020 7365 6c66 2e74 6f67 676c 6546 6565    self.toggleFee
+00005a40: 6462 6163 6b4c 6f6f 7028 6f6e 3d46 616c  dbackLoop(on=Fal
+00005a50: 7365 290d 0a20 2020 2020 2020 2072 6574  se)..        ret
+00005a60: 7572 6e20 7375 7065 7228 292e 7368 7574  urn super().shut
+00005a70: 646f 776e 2829 0d0a 2020 2020 0d0a 2020  down()..    ..  
+00005a80: 2020 6465 6620 746f 6767 6c65 4665 6564    def toggleFeed
+00005a90: 6261 636b 4c6f 6f70 2873 656c 662c 206f  backLoop(self, o
+00005aa0: 6e3a 626f 6f6c 293a 0d0a 2020 2020 2020  n:bool):..      
+00005ab0: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
+00005ac0: 7461 7274 206f 7220 7374 6f70 2066 6565  tart or stop fee
+00005ad0: 6462 6163 6b20 6c6f 6f70 0d0a 2020 2020  dback loop..    
+00005ae0: 2020 2020 0d0a 2020 2020 2020 2020 4172      ..        Ar
+00005af0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+00005b00: 206f 6e20 2862 6f6f 6c29 3a20 7768 6574   on (bool): whet
+00005b10: 6865 7220 746f 2073 7461 7274 2066 6565  her to start fee
+00005b20: 6462 6163 6b20 6c6f 6f70 0d0a 2020 2020  dback loop..    
+00005b30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00005b40: 2073 656c 662e 7365 7446 6c61 6728 6765   self.setFlag(ge
+00005b50: 745f 6665 6564 6261 636b 3d6f 6e29 0d0a  t_feedback=on)..
+00005b60: 2020 2020 2020 2020 6966 206f 6e3a 0d0a          if on:..
+00005b70: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+00005b80: 6665 6564 6261 636b 5f6c 6f6f 7027 2069  feedback_loop' i
+00005b90: 6e20 7365 6c66 2e5f 7468 7265 6164 733a  n self._threads:
+00005ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005bb0: 2020 7365 6c66 2e5f 7468 7265 6164 735b    self._threads[
+00005bc0: 2766 6565 6462 6163 6b5f 6c6f 6f70 275d  'feedback_loop']
+00005bd0: 2e6a 6f69 6e28 290d 0a20 2020 2020 2020  .join()..       
+00005be0: 2020 2020 2074 6872 6561 6420 3d20 5468       thread = Th
+00005bf0: 7265 6164 2874 6172 6765 743d 7365 6c66  read(target=self
+00005c00: 2e5f 6c6f 6f70 5f66 6565 6462 6163 6b29  ._loop_feedback)
+00005c10: 0d0a 2020 2020 2020 2020 2020 2020 7468  ..            th
+00005c20: 7265 6164 2e73 7461 7274 2829 0d0a 2020  read.start()..  
+00005c30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00005c40: 7468 7265 6164 735b 2766 6565 6462 6163  threads['feedbac
+00005c50: 6b5f 6c6f 6f70 275d 203d 2074 6872 6561  k_loop'] = threa
+00005c60: 640d 0a20 2020 2020 2020 2065 6c73 653a  d..        else:
+00005c70: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00005c80: 2027 6665 6564 6261 636b 5f6c 6f6f 7027   'feedback_loop'
+00005c90: 2069 6e20 7365 6c66 2e5f 7468 7265 6164   in self._thread
+00005ca0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00005cb0: 2020 2020 7365 6c66 2e5f 7468 7265 6164      self._thread
+00005cc0: 735b 2766 6565 6462 6163 6b5f 6c6f 6f70  s['feedback_loop
+00005cd0: 275d 2e6a 6f69 6e28 290d 0a20 2020 2020  '].join()..     
+00005ce0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+00005cf0: 2064 6566 207a 6572 6f28 7365 6c66 2920   def zero(self) 
+00005d00: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+00005d10: 2022 2222 0d0a 2020 2020 2020 2020 5a65   """..        Ze
+00005d20: 726f 2074 6865 2070 6c75 6e67 6572 2070  ro the plunger p
+00005d30: 6f73 6974 696f 6e0d 0a20 2020 2020 2020  osition..       
+00005d40: 200d 0a20 2020 2020 2020 2052 6574 7572   ..        Retur
+00005d50: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+00005d60: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
+00005d70: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
+00005d80: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00005d90: 2e65 6a65 6374 2829 0d0a 2020 2020 2020  .eject()..      
+00005da0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00005db0: 662e 5f71 7565 7279 2827 525a 2729 0d0a  f._query('RZ')..
+00005dc0: 2020 2020 2020 2020 7365 6c66 2e70 6f73          self.pos
+00005dd0: 6974 696f 6e20 3d20 300d 0a20 2020 2020  ition = 0..     
+00005de0: 2020 2074 696d 652e 736c 6565 7028 3229     time.sleep(2)
+00005df0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005e00: 2072 6573 706f 6e73 650d 0a0d 0a20 2020   response....   
+00005e10: 2023 2050 726f 7465 6374 6564 206d 6574   # Protected met
+00005e20: 686f 6428 7329 0d0a 2020 2020 6465 6620  hod(s)..    def 
+00005e30: 5f63 616c 6375 6c61 7465 5f73 7065 6564  _calculate_speed
+00005e40: 5f70 6172 616d 6574 6572 7328 7365 6c66  _parameters(self
+00005e50: 2c20 766f 6c75 6d65 3a69 6e74 2c20 7370  , volume:int, sp
+00005e60: 6565 643a 696e 7429 202d 3e20 5370 6565  eed:int) -> Spee
+00005e70: 6450 6172 616d 6574 6572 733a 0d0a 2020  dParameters:..  
+00005e80: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00005e90: 2020 2043 616c 6375 6c61 7465 7320 7468     Calculates th
+00005ea0: 6520 6265 7374 2070 6172 616d 6574 6572  e best parameter
+00005eb0: 7320 666f 7220 766f 6c75 6d65 2061 6e64  s for volume and
+00005ec0: 2073 7065 6564 0d0a 0d0a 2020 2020 2020   speed....      
+00005ed0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+00005ee0: 2020 2020 2076 6f6c 756d 6520 2869 6e74       volume (int
+00005ef0: 293a 2076 6f6c 756d 6520 746f 2062 6520  ): volume to be 
+00005f00: 7472 616e 7366 6572 7265 640d 0a20 2020  transferred..   
+00005f10: 2020 2020 2020 2020 2073 7065 6564 2028           speed (
+00005f20: 696e 7429 3a20 7370 6565 6420 6174 2077  int): speed at w
+00005f30: 6869 6368 206c 6971 7569 6420 6973 2074  hich liquid is t
+00005f40: 7261 6e73 6665 7272 6564 0d0a 0d0a 2020  ransferred....  
+00005f50: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005f60: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+00005f70: 3a20 6469 6374 696f 6e61 7279 206f 6620  : dictionary of 
+00005f80: 6265 7374 2070 6172 616d 6574 6572 730d  best parameters.
+00005f90: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00005fa0: 2020 2020 2020 6f75 7463 6f6d 6573 203d        outcomes =
+00005fb0: 207b 7d0d 0a20 2020 2020 2020 2073 7465   {}..        ste
+00005fc0: 705f 696e 7465 7276 616c 5f6c 696d 6974  p_interval_limit
+00005fd0: 203d 2069 6e74 2876 6f6c 756d 652f 7365   = int(volume/se
+00005fe0: 6c66 2e72 6573 6f6c 7574 696f 6e2f 5354  lf.resolution/ST
+00005ff0: 4550 5f52 4553 4f4c 5554 494f 4e29 0d0a  EP_RESOLUTION)..
+00006000: 2020 2020 2020 2020 666f 7220 7072 6573          for pres
+00006010: 6574 2069 6e20 7365 6c66 2e73 7065 6564  et in self.speed
+00006020: 5f70 7265 7365 7473 3a0d 0a20 2020 2020  _presets:..     
+00006030: 2020 2020 2020 2069 6620 7072 6573 6574         if preset
+00006040: 203c 2073 7065 6564 3a0d 0a20 2020 2020   < speed:..     
+00006050: 2020 2020 2020 2020 2020 2023 2070 7265             # pre
+00006060: 7365 7420 6973 2073 6c6f 7765 7220 7468  set is slower th
+00006070: 616e 2074 6172 6765 7420 7370 6565 642c  an target speed,
+00006080: 2069 7420 7769 6c6c 206e 6576 6572 2068   it will never h
+00006090: 6974 2074 6172 6765 7420 7370 6565 640d  it target speed.
+000060a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060b0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+000060c0: 2020 2020 2020 2074 696d 655f 696e 7465         time_inte
+000060d0: 7276 616c 5f6c 696d 6974 203d 2069 6e74  rval_limit = int
+000060e0: 2876 6f6c 756d 652a 2831 2f73 7065 6564  (volume*(1/speed
+000060f0: 202d 2031 2f70 7265 7365 7429 2f73 656c   - 1/preset)/sel
+00006100: 662e 7265 7370 6f6e 7365 5f74 696d 6529  f.response_time)
+00006110: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00006120: 206e 6f74 2073 7465 705f 696e 7465 7276   not step_interv
+00006130: 616c 5f6c 696d 6974 206f 7220 6e6f 7420  al_limit or not 
+00006140: 7469 6d65 5f69 6e74 6572 7661 6c5f 6c69  time_interval_li
+00006150: 6d69 743a 0d0a 2020 2020 2020 2020 2020  mit:..          
+00006160: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00006170: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+00006180: 7276 616c 7320 3d20 6d61 7828 6d69 6e28  rvals = max(min(
+00006190: 7374 6570 5f69 6e74 6572 7661 6c5f 6c69  step_interval_li
+000061a0: 6d69 742c 2074 696d 655f 696e 7465 7276  mit, time_interv
+000061b0: 616c 5f6c 696d 6974 292c 2031 290d 0a20  al_limit), 1).. 
+000061c0: 2020 2020 2020 2020 2020 2065 6163 685f             each_
+000061d0: 7374 6570 7320 3d20 766f 6c75 6d65 2f73  steps = volume/s
+000061e0: 656c 662e 7265 736f 6c75 7469 6f6e 2f69  elf.resolution/i
+000061f0: 6e74 6572 7661 6c73 0d0a 2020 2020 2020  ntervals..      
+00006200: 2020 2020 2020 6561 6368 5f64 656c 6179        each_delay
+00006210: 203d 2076 6f6c 756d 652a 2831 2f73 7065   = volume*(1/spe
+00006220: 6564 202d 2031 2f70 7265 7365 7429 2f69  ed - 1/preset)/i
+00006230: 6e74 6572 7661 6c73 0d0a 2020 2020 2020  ntervals..      
+00006240: 2020 2020 2020 6172 6561 203d 2030 2e35        area = 0.5
+00006250: 202a 2028 766f 6c75 6d65 2a2a 3229 202a   * (volume**2) *
+00006260: 2028 312f 7365 6c66 2e72 6573 6f6c 7574   (1/self.resolut
+00006270: 696f 6e29 202a 2028 312f 696e 7465 7276  ion) * (1/interv
+00006280: 616c 7329 202a 2028 312f 7370 6565 6420  als) * (1/speed 
+00006290: 2d20 312f 7072 6573 6574 290d 0a20 2020  - 1/preset)..   
+000062a0: 2020 2020 2020 2020 206f 7574 636f 6d65           outcome
+000062b0: 735b 6172 6561 5d20 3d20 5370 6565 6450  s[area] = SpeedP
+000062c0: 6172 616d 6574 6572 7328 7072 6573 6574  arameters(preset
+000062d0: 2c20 696e 7465 7276 616c 732c 2069 6e74  , intervals, int
+000062e0: 2865 6163 685f 7374 6570 7329 2c20 6561  (each_steps), ea
+000062f0: 6368 5f64 656c 6179 290d 0a20 2020 2020  ch_delay)..     
+00006300: 2020 2069 6620 6c65 6e28 6f75 7463 6f6d     if len(outcom
+00006310: 6573 2920 3d3d 2030 3a0d 0a20 2020 2020  es) == 0:..     
+00006320: 2020 2020 2020 2070 7269 6e74 2822 4e6f         print("No
+00006330: 2066 6561 7369 626c 6520 7370 6565 6420   feasible speed 
+00006340: 7061 7261 6d65 7465 7273 2e22 290d 0a20  parameters.").. 
+00006350: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006360: 6e20 5370 6565 6450 6172 616d 6574 6572  n SpeedParameter
+00006370: 7328 4e6f 6e65 2c20 5354 4550 5f52 4553  s(None, STEP_RES
+00006380: 4f4c 5554 494f 4e2c 2053 5445 505f 5245  OLUTION, STEP_RE
+00006390: 534f 4c55 5449 4f4e 2c20 7365 6c66 2e72  SOLUTION, self.r
+000063a0: 6573 706f 6e73 655f 7469 6d65 290d 0a20  esponse_time).. 
+000063b0: 2020 2020 2020 2070 7269 6e74 2866 2742         print(f'B
+000063c0: 6573 7420 7061 7261 6d65 7465 7273 3a20  est parameters: 
+000063d0: 7b6f 7574 636f 6d65 735b 6d69 6e28 6f75  {outcomes[min(ou
+000063e0: 7463 6f6d 6573 295d 7d27 290d 0a20 2020  tcomes)]}')..   
+000063f0: 2020 2020 2072 6574 7572 6e20 6f75 7463       return outc
+00006400: 6f6d 6573 5b6d 696e 286f 7574 636f 6d65  omes[min(outcome
+00006410: 7329 5d0d 0a20 2020 200d 0a20 2020 2064  s)]..    ..    d
+00006420: 6566 205f 636f 6e6e 6563 7428 7365 6c66  ef _connect(self
+00006430: 2c20 706f 7274 3a73 7472 2c20 6261 7564  , port:str, baud
+00006440: 7261 7465 3a69 6e74 203d 2039 3630 302c  rate:int = 9600,
+00006450: 2074 696d 656f 7574 3a69 6e74 203d 2031   timeout:int = 1
+00006460: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00006470: 0a20 2020 2020 2020 2043 6f6e 6e65 6374  .        Connect
+00006480: 696f 6e20 7072 6f63 6564 7572 6520 666f  ion procedure fo
+00006490: 7220 746f 6f6c 0d0a 0d0a 2020 2020 2020  r tool....      
+000064a0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+000064b0: 2020 2020 2070 6f72 7420 2873 7472 293a       port (str):
+000064c0: 2043 4f4d 2070 6f72 7420 6164 6472 6573   COM port addres
+000064d0: 730d 0a20 2020 2020 2020 2020 2020 2062  s..            b
+000064e0: 6175 6472 6174 6520 2869 6e74 2c20 6f70  audrate (int, op
+000064f0: 7469 6f6e 616c 293a 2062 6175 6472 6174  tional): baudrat
+00006500: 652e 2044 6566 6175 6c74 7320 746f 2039  e. Defaults to 9
+00006510: 3630 302e 0d0a 2020 2020 2020 2020 2020  600...          
+00006520: 2020 7469 6d65 6f75 7420 2869 6e74 2c20    timeout (int, 
+00006530: 6f70 7469 6f6e 616c 293a 2074 696d 656f  optional): timeo
+00006540: 7574 2069 6e20 7365 636f 6e64 732e 2044  ut in seconds. D
+00006550: 6566 6175 6c74 7320 746f 2031 2e0d 0a20  efaults to 1... 
+00006560: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00006570: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
+00006580: 696f 6e5f 6465 7461 696c 7320 3d20 7b0d  ion_details = {.
+00006590: 0a20 2020 2020 2020 2020 2020 2027 706f  .            'po
+000065a0: 7274 273a 2070 6f72 742c 0d0a 2020 2020  rt': port,..    
+000065b0: 2020 2020 2020 2020 2762 6175 6472 6174          'baudrat
+000065c0: 6527 3a20 6261 7564 7261 7465 2c0d 0a20  e': baudrate,.. 
+000065d0: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
+000065e0: 6f75 7427 3a20 7469 6d65 6f75 740d 0a20  out': timeout.. 
+000065f0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00006600: 2020 6465 7669 6365 203d 204e 6f6e 650d    device = None.
+00006610: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00006620: 2020 2020 2020 2020 2020 2064 6576 6963             devic
+00006630: 6520 3d20 7365 7269 616c 2e53 6572 6961  e = serial.Seria
+00006640: 6c28 706f 7274 2c20 6261 7564 7261 7465  l(port, baudrate
+00006650: 2c20 7469 6d65 6f75 743d 7469 6d65 6f75  , timeout=timeou
+00006660: 7429 0d0a 2020 2020 2020 2020 6578 6365  t)..        exce
+00006670: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00006680: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00006690: 7072 696e 7428 6622 436f 756c 6420 6e6f  print(f"Could no
+000066a0: 7420 636f 6e6e 6563 7420 746f 207b 706f  t connect to {po
+000066b0: 7274 7d22 290d 0a20 2020 2020 2020 2020  rt}")..         
+000066c0: 2020 2069 6620 7365 6c66 2e76 6572 626f     if self.verbo
+000066d0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000066e0: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+000066f0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00006700: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00006710: 6c65 6570 2832 2920 2020 2320 5761 6974  leep(2)   # Wait
+00006720: 2066 6f72 2067 7262 6c20 746f 2069 6e69   for grbl to ini
+00006730: 7469 616c 697a 650d 0a20 2020 2020 2020  tialize..       
+00006740: 2020 2020 2064 6576 6963 652e 666c 7573       device.flus
+00006750: 6849 6e70 7574 2829 0d0a 2020 2020 2020  hInput()..      
+00006760: 2020 2020 2020 7072 696e 7428 6622 436f        print(f"Co
+00006770: 6e6e 6563 7469 6f6e 206f 7065 6e65 6420  nnection opened 
+00006780: 746f 207b 706f 7274 7d22 290d 0a20 2020  to {port}")..   
+00006790: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000067a0: 7446 6c61 6728 636f 6e6e 6563 7465 643d  tFlag(connected=
+000067b0: 5472 7565 290d 0a20 2020 2020 2020 2073  True)..        s
+000067c0: 656c 662e 6465 7669 6365 203d 2064 6576  elf.device = dev
+000067d0: 6963 650d 0a20 2020 2020 2020 2073 656c  ice..        sel
+000067e0: 662e 6765 7449 6e66 6f28 290d 0a20 2020  f.getInfo()..   
+000067f0: 2020 2020 2073 656c 662e 7265 7365 7428       self.reset(
+00006800: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00006810: 6e0d 0a20 2020 200d 0a20 2020 2064 6566  n..    ..    def
+00006820: 205f 6973 5f65 7870 6563 7465 645f 7265   _is_expected_re
+00006830: 706c 7928 7365 6c66 2c20 7265 7370 6f6e  ply(self, respon
+00006840: 7365 3a73 7472 2c20 636f 6d6d 616e 645f  se:str, command_
+00006850: 636f 6465 3a73 7472 2c20 2a2a 6b77 6172  code:str, **kwar
+00006860: 6773 2920 2d3e 2062 6f6f 6c3a 0d0a 2020  gs) -> bool:..  
+00006870: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00006880: 2020 2043 6865 636b 7320 616e 6420 7265     Checks and re
+00006890: 7475 726e 7320 7768 6574 6865 7220 7468  turns whether th
+000068a0: 6520 7265 7370 6f6e 7365 2069 7320 616e  e response is an
+000068b0: 2065 7870 6563 7465 6420 7265 706c 790d   expected reply.
+000068c0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+000068d0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000068e0: 7370 6f6e 7365 2028 7374 7229 3a20 7265  sponse (str): re
+000068f0: 7370 6f6e 7365 2073 7472 696e 6720 6672  sponse string fr
+00006900: 6f6d 2064 6576 6963 650d 0a20 2020 2020  om device..     
+00006910: 2020 2020 2020 2063 6f6d 6d61 6e64 5f63         command_c
+00006920: 6f64 6520 2873 7472 293a 2074 776f 2d63  ode (str): two-c
+00006930: 6861 7261 6374 6572 2063 6f6d 6d61 6e64  haracter command
+00006940: 2063 6f64 650d 0a0d 0a20 2020 2020 2020   code....       
+00006950: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00006960: 2020 2020 2020 2062 6f6f 6c3a 2077 6865         bool: whe
+00006970: 7468 6572 2074 6865 2072 6573 706f 6e73  ther the respons
+00006980: 6520 6973 2061 6e20 6578 7065 6374 6564  e is an expected
+00006990: 2072 6570 6c79 0d0a 2020 2020 2020 2020   reply..        
+000069a0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+000069b0: 7265 7370 6f6e 7365 2069 6e20 4572 726f  response in Erro
+000069c0: 7243 6f64 652e 5f6d 656d 6265 725f 6e61  rCode._member_na
+000069d0: 6d65 735f 3a0d 0a20 2020 2020 2020 2020  mes_:..         
+000069e0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+000069f0: 2020 2020 2020 2020 6966 2063 6f6d 6d61          if comma
+00006a00: 6e64 5f63 6f64 6520 6e6f 7420 696e 2051  nd_code not in Q
+00006a10: 5545 5249 4553 2061 6e64 2072 6573 706f  UERIES and respo
+00006a20: 6e73 6520 3d3d 2027 6f6b 273a 0d0a 2020  nse == 'ok':..  
+00006a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006a40: 2054 7275 650d 0a20 2020 2020 2020 2069   True..        i
+00006a50: 6620 636f 6d6d 616e 645f 636f 6465 2069  f command_code i
+00006a60: 6e20 5155 4552 4945 5320 616e 6420 7265  n QUERIES and re
+00006a70: 7370 6f6e 7365 5b3a 325d 203d 3d20 636f  sponse[:2] == co
+00006a80: 6d6d 616e 645f 636f 6465 2e6c 6f77 6572  mmand_code.lower
+00006a90: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00006aa0: 2072 6570 6c79 5f63 6f64 652c 2064 6174   reply_code, dat
+00006ab0: 6120 3d20 7265 7370 6f6e 7365 5b3a 325d  a = response[:2]
+00006ac0: 2c20 7265 7370 6f6e 7365 5b32 3a5d 0d0a  , response[2:]..
+00006ad0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00006ae0: 656c 662e 7665 7262 6f73 653a 0d0a 2020  elf.verbose:..  
+00006af0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00006b00: 696e 7428 6627 5b7b 7265 706c 795f 636f  int(f'[{reply_co
+00006b10: 6465 7d5d 207b 6461 7461 7d27 290d 0a20  de}] {data}').. 
+00006b20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006b30: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
+00006b40: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
+00006b50: 2020 2020 6465 6620 5f6c 6f6f 705f 6665      def _loop_fe
+00006b60: 6564 6261 636b 2873 656c 6629 3a0d 0a20  edback(self):.. 
+00006b70: 2020 2020 2020 2022 2222 4c6f 6f70 2074         """Loop t
+00006b80: 6f20 636f 6e73 7461 6e74 6c79 2072 6561  o constantly rea
+00006b90: 6420 6672 6f6d 2064 6576 6963 6522 2222  d from device"""
+00006ba0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00006bb0: 274c 6973 7465 6e69 6e67 2e2e 2e27 290d  'Listening...').
+00006bc0: 0a20 2020 2020 2020 2077 6869 6c65 2073  .        while s
+00006bd0: 656c 662e 666c 6167 735b 2767 6574 5f66  elf.flags['get_f
+00006be0: 6565 6462 6163 6b27 5d3a 0d0a 2020 2020  eedback']:..    
+00006bf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006c00: 666c 6167 735b 2770 6175 7365 5f66 6565  flags['pause_fee
+00006c10: 6462 6163 6b27 5d3a 0d0a 2020 2020 2020  dback']:..      
+00006c20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00006c30: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00006c40: 7365 6c66 2e67 6574 5374 6174 7573 2829  self.getStatus()
+00006c50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00006c60: 6c66 2e67 6574 4361 7061 6369 7461 6e63  lf.getCapacitanc
+00006c70: 6528 290d 0a20 2020 2020 2020 2070 7269  e()..        pri
+00006c80: 6e74 2827 5374 6f70 206c 6973 7465 6e69  nt('Stop listeni
+00006c90: 6e67 2e2e 2e27 290d 0a20 2020 2020 2020  ng...')..       
+00006ca0: 2072 6574 7572 6e0d 0a20 2020 200d 0a20   return..    .. 
+00006cb0: 2020 2064 6566 205f 7175 6572 7928 7365     def _query(se
+00006cc0: 6c66 2c20 0d0a 2020 2020 2020 2020 636f  lf, ..        co
+00006cd0: 6d6d 616e 643a 2073 7472 2c20 0d0a 2020  mmand: str, ..  
+00006ce0: 2020 2020 2020 7469 6d65 6f75 745f 733a        timeout_s:
+00006cf0: 2066 6c6f 6174 203d 2030 2e33 2c20 0d0a   float = 0.3, ..
+00006d00: 2020 2020 2020 2020 7265 7375 6d65 5f66          resume_f
+00006d10: 6565 6462 6163 6b3a 2062 6f6f 6c20 3d20  eedback: bool = 
+00006d20: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00006d30: 6765 745f 706f 7369 7469 6f6e 3a20 626f  get_position: bo
+00006d40: 6f6c 203d 2054 7275 650d 0a20 2020 2029  ol = True..    )
+00006d50: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
+00006d60: 2020 2222 220d 0a20 2020 2020 2020 2057    """..        W
+00006d70: 7269 7465 2063 6f6d 6d61 6e64 2074 6f20  rite command to 
+00006d80: 616e 6420 7265 6164 2072 6573 706f 6e73  and read respons
+00006d90: 6520 6672 6f6d 2064 6576 6963 650d 0a0d  e from device...
+00006da0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00006db0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+00006dc0: 616e 6420 2873 7472 293a 2063 6f6d 6d61  and (str): comma
+00006dd0: 6e64 2073 7472 696e 670d 0a20 2020 2020  nd string..     
+00006de0: 2020 2020 2020 2074 696d 656f 7574 5f73         timeout_s
+00006df0: 2028 666c 6f61 742c 206f 7074 696f 6e61   (float, optiona
+00006e00: 6c29 3a20 6475 7261 7469 6f6e 2074 6f20  l): duration to 
+00006e10: 7761 6974 2062 6566 6f72 6520 7469 6d65  wait before time
+00006e20: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
+00006e30: 2030 2e33 2e0d 0a20 2020 2020 2020 2020   0.3...         
+00006e40: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
+00006e50: 636b 2028 626f 6f6c 2c20 6f70 7469 6f6e  ck (bool, option
+00006e60: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
+00006e70: 7265 7375 6d65 2072 6561 6469 6e67 2066  resume reading f
+00006e80: 726f 6d20 6465 7669 6365 2e20 4465 6661  rom device. Defa
+00006e90: 756c 7473 2074 6f20 4661 6c73 652e 0d0a  ults to False...
+00006ea0: 2020 2020 2020 2020 2020 2020 6765 745f              get_
+00006eb0: 706f 7369 7469 6f6e 2028 626f 6f6c 2c20  position (bool, 
+00006ec0: 6f70 7469 6f6e 616c 293a 2077 6865 7468  optional): wheth
+00006ed0: 6572 2074 6f20 6765 7420 7468 6520 706f  er to get the po
+00006ee0: 7369 7469 6f6e 206f 6620 7468 6520 706c  sition of the pl
+00006ef0: 756e 6765 722e 2044 6566 6175 6c74 7320  unger. Defaults 
+00006f00: 746f 2054 7275 652e 0d0a 2020 2020 2020  to True...      
+00006f10: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00006f20: 2020 2020 2020 2020 7374 723a 2072 6573          str: res
+00006f30: 706f 6e73 6520 7374 7269 6e67 0d0a 2020  ponse string..  
+00006f40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00006f50: 2020 2063 6f6d 6d61 6e64 5f63 6f64 6520     command_code 
+00006f60: 3d20 636f 6d6d 616e 645b 3a32 5d0d 0a20  = command[:2].. 
+00006f70: 2020 2020 2020 2069 6620 636f 6d6d 616e         if comman
+00006f80: 645f 636f 6465 206e 6f74 2069 6e20 5354  d_code not in ST
+00006f90: 4154 5553 5f51 5545 5249 4553 3a0d 0a20  ATUS_QUERIES:.. 
+00006fa0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00006fb0: 6c66 2e66 6c61 6773 5b27 6765 745f 6665  lf.flags['get_fe
+00006fc0: 6564 6261 636b 275d 2061 6e64 206e 6f74  edback'] and not
+00006fd0: 2073 656c 662e 666c 6167 735b 2770 6175   self.flags['pau
+00006fe0: 7365 5f66 6565 6462 6163 6b27 5d3a 0d0a  se_feedback']:..
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007000: 7365 6c66 2e73 6574 466c 6167 2870 6175  self.setFlag(pau
+00007010: 7365 5f66 6565 6462 6163 6b3d 5472 7565  se_feedback=True
+00007020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007030: 2020 2074 696d 652e 736c 6565 7028 7469     time.sleep(ti
+00007040: 6d65 6f75 745f 7329 0d0a 2020 2020 2020  meout_s)..      
+00007050: 2020 2020 2020 2320 7365 6c66 2e67 6574        # self.get
+00007060: 5374 6174 7573 2829 0d0a 2020 2020 2020  Status()..      
+00007070: 2020 2020 2020 2320 7768 696c 6520 7365        # while se
+00007080: 6c66 2e69 7342 7573 7928 293a 0d0a 2020  lf.isBusy():..  
+00007090: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+000070a0: 7365 6c66 2e67 6574 5374 6174 7573 2829  self.getStatus()
+000070b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000070c0: 2073 656c 662e 6973 4275 7379 2829 3a0d   self.isBusy():.
+000070d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000070e0: 2074 696d 652e 736c 6565 7028 7469 6d65   time.sleep(time
+000070f0: 6f75 745f 7329 0d0a 2020 2020 2020 2020  out_s)..        
+00007100: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
+00007110: 7469 6d65 203d 2074 696d 652e 7065 7266  time = time.perf
+00007120: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
+00007130: 2020 2020 7365 6c66 2e5f 7772 6974 6528      self._write(
+00007140: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
+00007150: 2020 7265 7370 6f6e 7365 203d 2027 270d    response = ''.
+00007160: 0a20 2020 2020 2020 2077 6869 6c65 206e  .        while n
+00007170: 6f74 2073 656c 662e 5f69 735f 6578 7065  ot self._is_expe
+00007180: 6374 6564 5f72 6570 6c79 2872 6573 706f  cted_reply(respo
+00007190: 6e73 652c 2063 6f6d 6d61 6e64 5f63 6f64  nse, command_cod
+000071a0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+000071b0: 2069 6620 7469 6d65 2e70 6572 665f 636f   if time.perf_co
+000071c0: 756e 7465 7228 2920 2d20 7374 6172 745f  unter() - start_
+000071d0: 7469 6d65 203e 2074 696d 656f 7574 5f73  time > timeout_s
+000071e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000071f0: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
+00007200: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00007210: 2073 656c 662e 5f72 6561 6428 290d 0a20   self._read().. 
+00007220: 2020 2020 2020 2023 2070 7269 6e74 2874         # print(t
+00007230: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+00007240: 2829 202d 2073 7461 7274 5f74 696d 6529  () - start_time)
+00007250: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
+00007260: 6d61 6e64 5f63 6f64 6520 696e 2051 5545  mand_code in QUE
+00007270: 5249 4553 3a0d 0a20 2020 2020 2020 2020  RIES:..         
+00007280: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
+00007290: 7370 6f6e 7365 5b32 3a5d 0d0a 2020 2020  sponse[2:]..    
+000072a0: 2020 2020 6966 2063 6f6d 6d61 6e64 5f63      if command_c
+000072b0: 6f64 6520 6e6f 7420 696e 2053 5441 5455  ode not in STATU
+000072c0: 535f 5155 4552 4945 533a 0d0a 2020 2020  S_QUERIES:..    
+000072d0: 2020 2020 2020 2020 6966 2067 6574 5f70          if get_p
+000072e0: 6f73 6974 696f 6e3a 0d0a 2020 2020 2020  osition:..      
+000072f0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00007300: 6574 506f 7369 7469 6f6e 2829 0d0a 2020  etPosition()..  
+00007310: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+00007320: 756d 655f 6665 6564 6261 636b 3a0d 0a20  ume_feedback:.. 
+00007330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007340: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
+00007350: 655f 6665 6564 6261 636b 3d46 616c 7365  e_feedback=False
+00007360: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00007370: 6e20 7265 7370 6f6e 7365 0d0a 0d0a 2020  n response....  
+00007380: 2020 6465 6620 5f72 6561 6428 7365 6c66    def _read(self
+00007390: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000073a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000073b0: 5265 6164 2072 6573 706f 6e73 6520 6672  Read response fr
+000073c0: 6f6d 2064 6576 6963 650d 0a0d 0a20 2020  om device....   
+000073d0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+000073e0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
+000073f0: 7265 7370 6f6e 7365 2073 7472 696e 670d  response string.
+00007400: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00007410: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00007420: 2027 270d 0a20 2020 2020 2020 2074 7279   ''..        try
+00007430: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00007440: 6573 706f 6e73 6520 3d20 7365 6c66 2e64  esponse = self.d
+00007450: 6576 6963 652e 7265 6164 6c69 6e65 2829  evice.readline()
+00007460: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00007470: 206c 656e 2872 6573 706f 6e73 6529 203d   len(response) =
+00007480: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00007490: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+000074a0: 2073 656c 662e 6465 7669 6365 2e72 6561   self.device.rea
+000074b0: 646c 696e 6528 290d 0a20 2020 2020 2020  dline()..       
+000074c0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+000074d0: 7265 7370 6f6e 7365 5b32 3a2d 325d 2e64  response[2:-2].d
+000074e0: 6563 6f64 6528 2775 7466 2d38 2729 0d0a  ecode('utf-8')..
+000074f0: 2020 2020 2020 2020 6578 6365 7074 2041          except A
+00007500: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
+00007510: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00007520: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00007530: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00007540: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00007550: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
+00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007570: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
+00007580: 2020 6966 2072 6573 706f 6e73 6520 696e    if response in
+00007590: 2045 7272 6f72 436f 6465 2e5f 6d65 6d62   ErrorCode._memb
+000075a0: 6572 5f6e 616d 6573 5f3a 0d0a 2020 2020  er_names_:..    
+000075b0: 2020 2020 2020 2020 7072 696e 7428 4572          print(Er
+000075c0: 726f 7243 6f64 655b 7265 7370 6f6e 7365  rorCode[response
+000075d0: 5d2e 7661 6c75 6529 0d0a 2020 2020 2020  ].value)..      
+000075e0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+000075f0: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
+00007600: 205f 7365 745f 6368 616e 6e65 6c5f 6964   _set_channel_id
+00007610: 2873 656c 662c 206e 6577 5f63 6861 6e6e  (self, new_chann
+00007620: 656c 5f69 643a 696e 7429 3a0d 0a20 2020  el_id:int):..   
+00007630: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00007640: 2020 5365 7420 6368 616e 6e65 6c20 6964    Set channel id
+00007650: 206f 6620 6465 7669 6365 0d0a 0d0a 2020   of device....  
+00007660: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00007670: 2020 2020 2020 2020 206e 6577 5f63 6861           new_cha
+00007680: 6e6e 656c 2028 696e 7429 3a20 6e65 7720  nnel (int): new 
+00007690: 6368 616e 6e65 6c20 6964 0d0a 0d0a 2020  channel id....  
+000076a0: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
+000076b0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
+000076c0: 4572 726f 723a 2050 6c65 6173 6520 7365  Error: Please se
+000076d0: 6c65 6374 2061 2076 616c 6964 2072 4c69  lect a valid rLi
+000076e0: 6e65 2061 6464 7265 7373 2066 726f 6d20  ne address from 
+000076f0: 3120 746f 2039 0d0a 2020 2020 2020 2020  1 to 9..        
+00007700: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+00007710: 6e6f 7420 2830 203c 206e 6577 5f63 6861  not (0 < new_cha
+00007720: 6e6e 656c 5f69 6420 3c20 3130 293a 0d0a  nnel_id < 10):..
+00007730: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00007740: 6520 5661 6c75 6545 7272 6f72 2827 506c  e ValueError('Pl
+00007750: 6561 7365 2073 656c 6563 7420 6120 7661  ease select a va
+00007760: 6c69 6420 724c 696e 6520 6164 6472 6573  lid rLine addres
+00007770: 7320 6672 6f6d 2031 2074 6f20 392e 2729  s from 1 to 9.')
+00007780: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+00007790: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+000077a0: 2866 272a 417b 6e65 775f 6368 616e 6e65  (f'*A{new_channe
+000077b0: 6c5f 6964 7d27 290d 0a20 2020 2020 2020  l_id}')..       
+000077c0: 2069 6620 7265 7370 6f6e 7365 203d 3d20   if response == 
+000077d0: 276f 6b27 3a0d 0a20 2020 2020 2020 2020  'ok':..         
+000077e0: 2020 2073 656c 662e 6368 616e 6e65 6c20     self.channel 
+000077f0: 3d20 6e65 775f 6368 616e 6e65 6c5f 6964  = new_channel_id
+00007800: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00007810: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00007820: 5f77 7269 7465 2873 656c 662c 2063 6f6d  _write(self, com
+00007830: 6d61 6e64 3a73 7472 2920 2d3e 2062 6f6f  mand:str) -> boo
+00007840: 6c3a 0d0a 2020 2020 2020 2020 2222 220d  l:..        """.
+00007850: 0a20 2020 2020 2020 2057 7269 7465 2063  .        Write c
+00007860: 6f6d 6d61 6e64 2074 6f20 6465 7669 6365  ommand to device
+00007870: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
+00007880: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00007890: 6f6d 6d61 6e64 2028 7374 7229 3a20 3c63  ommand (str): <c
+000078a0: 6f6d 6d61 6e64 2063 6f64 653e 3c76 616c  ommand code><val
+000078b0: 7565 3e0d 0a0d 0a20 2020 2020 2020 2052  ue>....        R
+000078c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000078d0: 2020 2020 2062 6f6f 6c3a 2077 6865 7468       bool: wheth
+000078e0: 6572 2063 6f6d 6d61 6e64 2077 6173 2073  er command was s
+000078f0: 656e 7420 7375 6363 6573 7366 756c 6c79  ent successfully
+00007900: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00007910: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00007920: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+00007930: 2020 2020 2070 7269 6e74 2863 6f6d 6d61       print(comma
+00007940: 6e64 290d 0a20 2020 2020 2020 2066 7374  nd)..        fst
+00007950: 7269 6e67 203d 2066 2701 7b73 656c 662e  ring = f'.{self.
+00007960: 6368 616e 6e65 6c7d 7b63 6f6d 6d61 6e64  channel}{command
+00007970: 7dc2 ba5c 7227 2023 2063 6f6d 6d61 6e64  }..\r' # command
+00007980: 2074 656d 706c 6174 653a 203c 5052 453e   template: <PRE>
+00007990: 3c41 4452 3e3c 434f 4445 3e3c 4441 5441  <ADR><CODE><DATA
+000079a0: 3e3c 4c52 433e 3c50 4f53 543e 0d0a 2020  ><LRC><POST>..  
+000079b0: 2020 2020 2020 2320 6273 7472 696e 6720        # bstring 
+000079c0: 3d20 6279 7465 6172 7261 792e 6672 6f6d  = bytearray.from
+000079d0: 6865 7828 6673 7472 696e 672e 656e 636f  hex(fstring.enco
+000079e0: 6465 2827 7574 662d 3827 292e 6865 7828  de('utf-8').hex(
+000079f0: 2929 0d0a 2020 2020 2020 2020 7472 793a  ))..        try:
+00007a00: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00007a10: 5479 7069 6361 6c20 7469 6d65 6f75 7420  Typical timeout 
+00007a20: 7761 6974 2069 7320 3430 306d 730d 0a20  wait is 400ms.. 
+00007a30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007a40: 6465 7669 6365 2e77 7269 7465 2866 7374  device.write(fst
+00007a50: 7269 6e67 2e65 6e63 6f64 6528 2775 7466  ring.encode('utf
+00007a60: 2d38 2729 290d 0a20 2020 2020 2020 2065  -8'))..        e
+00007a70: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
+00007a80: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+00007a90: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00007aa0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00007ab0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+00007ac0: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
+00007ad0: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+00007ae0: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
+00007af0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007b00: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+00007b10: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00007b20: 2020 2020
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,34 +269,36 @@
         ret2 = self.blowout(channel=channel)
         return all([ret1,ret2])
     
     def fill(self, 
         speed: Optional[float] = None, 
         wait: int = 0, 
         pause: bool = False, 
-        cycles: int = 1,
+        cycles: int = 0,
         reagent: Optional[str] = None, 
         channel: Optional[Union[int, tuple[int]]] = None,
         **kwargs
     ) -> bool:
         """
         Fill the channel
 
         Args:
             speed (Optional[float], optional): speed to aspirate and dispense at. Defaults to None.
             wait (int, optional): time delay after each action. Defaults to 0.
             pause (bool, optional): whether to pause for user intervention. Defaults to False.
-            cycles (int, optional): number of cycles. Defaults to 1.
+            cycles (int, optional): number of cycles before filling. Defaults to 0.
             reagent (Optional[str], optional): name of reagent. Defaults to None.
             channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
         
         Returns:
             bool: whether the action is successful
         """
-        ret1 = self.cycle(volume=self.capacity, speed=speed, wait=wait, cycles=cycles, reagent=reagent, channel=channel)
+        ret1 = True
+        if cycles:
+            ret1 = self.cycle(volume=self.capacity, speed=speed, wait=wait, cycles=cycles, reagent=reagent, channel=channel)
         ret2 = self.aspirate(volume=self.capacity, speed=speed, wait=wait, pause=pause, reagent=reagent, channel=channel)
         ret3 = self.pullback(channel=channel)
         return all([ret1,ret2,ret3])
     
     def isBusy(self) -> bool:
         """
         Checks and returns whether the device is busy
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.0.1a3/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/image_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/View/image_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/View/view_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/__init__.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/decorators.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/factory.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/helper.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     Args:
         start_time (float): start time in seconds since epoch
         timeout (float): timeout duration
 
     Returns:
         bool: whether the process has overrun
     """
-    if timeout!=None and time.time() - start_time > timeout:
+    if timeout!=None and time.perf_counter() - start_time > timeout:
         return True
     return False
 
 def pretty_print_duration(total_time:float) -> str:
     """
     Display time duration (s) as HH:MM:SS text
```

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/layout.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/logger.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.0.1a3/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/tests/test_compound_liquidmover.py` & `control-lab-ly-1.0.1a3/tests/test_compound_liquidmover.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import init
 import numpy as np
 from controllably.Compound.LiquidMover import LiquidMoverSetup
 from controllably import Helper, Factory
 
 details = Factory.get_details(Helper.read_yaml('configs/skwr.yaml'))['setup']
 me = LiquidMoverSetup(**details['settings'])
+me.liquid.getInfo('BRL1000')
 me.__dict__
 # %%
 me.loadDeck(r"C:\Users\leongcj\Desktop\Astar_git\control-lab-le\library\deck\layoutB1.json")
 # %%
-me.attachTip()
+me.attachTip(start_tip='D4')
 # %%
 me.mover.home()
 # %%
 me.aspirateAt(me.mover.tool_position[0], 200)
 # %%
 me.dispenseAt(me.mover.tool_position[0]+np.array((10,10,10)), 200)
 # %%
```

### Comparing `control-lab-ly-1.0.1a2/tests/test_compound_spin_printer.py` & `control-lab-ly-1.0.1a3/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/tests/test_dobot_m1pro.py` & `control-lab-ly-1.0.1a3/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/tests/test_dobot_mg400.py` & `control-lab-ly-1.0.1a3/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/tests/test_heat_peltier.py` & `control-lab-ly-1.0.1a3/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.0.1a2/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.0.1a3/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

