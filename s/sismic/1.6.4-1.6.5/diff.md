# Comparing `tmp/sismic-1.6.4.tar.gz` & `tmp/sismic-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sismic-1.6.4.tar", last modified: Fri Mar  3 15:51:47 2023, max compression
+gzip compressed data, was "sismic-1.6.5.tar", last modified: Mon May  8 13:19:21 2023, max compression
```

## Comparing `sismic-1.6.4.tar` & `sismic-1.6.5.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.821471 sismic-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-03-03 15:51:39.000000 sismic-1.6.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)    33083 2023-03-03 15:51:39.000000 sismic-1.6.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7558 2023-03-03 15:51:39.000000 sismic-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-03 15:51:39.000000 sismic-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6899 2023-03-03 15:51:47.821471 sismic-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5666 2023-03-03 15:51:39.000000 sismic-1.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.809471 sismic-1.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7401 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.809471 sismic-1.6.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/bdd.rst
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/clock.rst
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/code.rst
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/interpreter.rst
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/io.rst
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/model.rst
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/runner.rst
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/behavior.rst
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8432 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/code.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11763 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/concurrent.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9507 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/contract.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.809471 sismic-1.6.4/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.809471 sismic-1.6.4/docs/examples/elevator/
--rw-r--r--   0 runner    (1001) docker     (122)    40408 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/Elevator.graffle
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/elevator.feature
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/elevator.plantuml
--rw-r--r--   0 runner    (1001) docker     (122)    37204 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/elevator.png
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/elevator.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/elevator_buttons.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/elevator_contract.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/tester_elevator_7th_floor_never_reached.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/elevator/tester_elevator_moves_after_10s.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.813471 sismic-1.6.4/docs/examples/microwave/
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/cooking_human.feature
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/heating.feature
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/heating_off_property.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/heating_on_property.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/heating_property.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/lighting_human.feature
--rw-r--r--   0 runner    (1001) docker     (122)     9031 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/microwave.py
--rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/microwave.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/microwave_with_contracts.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      485 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/safety_human.feature
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/microwave/test_microwave.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.813471 sismic-1.6.4/docs/examples/stopwatch/
--rw-r--r--   0 runner    (1001) docker     (122)   135709 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch.graffle
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1279 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_external.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_gui.png
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_gui_external.py
--rw-r--r--   0 runner    (1001) docker     (122)   171745 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_overview.png
--rw-r--r--   0 runner    (1001) docker     (122)   188103 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_with_logic.png
--rw-r--r--   0 runner    (1001) docker     (122)   143243 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/stopwatch/stopwatch_with_object.png
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/examples/writer_options.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    18618 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/execution.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9548 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/format.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5873 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6891 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/integration.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/properties.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/time.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/unittests.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-03-03 15:51:39.000000 sismic-1.6.4/docs/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-03-03 15:51:39.000000 sismic-1.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-03-03 15:51:47.821471 sismic-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-03-03 15:51:39.000000 sismic-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.813471 sismic-1.6.4/sismic/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.813471 sismic-1.6.4/sismic/bdd/
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/bdd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/bdd/environment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6563 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/bdd/steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5228 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/bdd/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/sismic/clock/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/clock/clock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/sismic/code/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5932 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/code/context.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/code/dummy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6738 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/code/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (122)    12867 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/code/python.py
--rw-r--r--   0 runner    (1001) docker     (122)     3503 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/sismic/interpreter/
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34479 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/interpreter/default.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/interpreter/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/sismic/io/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10641 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/io/datadict.py
--rw-r--r--   0 runner    (1001) docker     (122)    15085 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/io/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/sismic/model/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11707 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/model/elements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/model/events.py
--rw-r--r--   0 runner    (1001) docker     (122)    24349 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/model/statechart.py
--rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/model/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/sismic/runner/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-03-03 15:51:39.000000 sismic-1.6.4/sismic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.813471 sismic-1.6.4/sismic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6899 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-03 15:51:47.000000 sismic-1.6.4/sismic.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.817471 sismic-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    10271 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_bdd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4372 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (122)     2173 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)    26016 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    24839 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     4166 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 15:51:47.821471 sismic-1.6.4/tests/yaml/
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/actions.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/composite.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/deep_history.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/final.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/history.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/infinite.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/internal.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/nested_parallel.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/nondeterministic.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/parallel.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/priority.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/simple.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-03-03 15:51:39.000000 sismic-1.6.4/tests/yaml/timer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.138748 sismic-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-08 13:19:09.000000 sismic-1.6.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    33245 2023-05-08 13:19:09.000000 sismic-1.6.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7558 2023-05-08 13:19:09.000000 sismic-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-08 13:19:09.000000 sismic-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6850 2023-05-08 13:19:21.138748 sismic-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5666 2023-05-08 13:19:09.000000 sismic-1.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.122748 sismic-1.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7401 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.122748 sismic-1.6.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/bdd.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/clock.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/code.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/interpreter.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/io.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/model.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/runner.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/behavior.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8432 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/code.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11763 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/concurrent.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9507 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/contract.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.122748 sismic-1.6.5/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.126748 sismic-1.6.5/docs/examples/elevator/
+-rw-r--r--   0 runner    (1001) docker     (122)    40408 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/Elevator.graffle
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/elevator.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/elevator.plantuml
+-rw-r--r--   0 runner    (1001) docker     (122)    37204 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/elevator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/elevator.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/elevator_buttons.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/elevator_contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/tester_elevator_7th_floor_never_reached.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/elevator/tester_elevator_moves_after_10s.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.126748 sismic-1.6.5/docs/examples/microwave/
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/cooking_human.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/heating.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/heating_off_property.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/heating_on_property.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/heating_property.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/lighting_human.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     9031 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/microwave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/microwave.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/microwave_with_contracts.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/safety_human.feature
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/microwave/test_microwave.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/docs/examples/stopwatch/
+-rw-r--r--   0 runner    (1001) docker     (122)   135709 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch.graffle
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1279 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_external.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_gui.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_gui_external.py
+-rw-r--r--   0 runner    (1001) docker     (122)   171745 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_overview.png
+-rw-r--r--   0 runner    (1001) docker     (122)   188103 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_with_logic.png
+-rw-r--r--   0 runner    (1001) docker     (122)   143243 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/stopwatch/stopwatch_with_object.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/examples/writer_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    18618 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/execution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9548 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/format.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5873 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6891 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/time.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/unittests.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-05-08 13:19:09.000000 sismic-1.6.5/docs/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-08 13:19:09.000000 sismic-1.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-08 13:19:21.138748 sismic-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-05-08 13:19:09.000000 sismic-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/sismic/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/sismic/bdd/
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/bdd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/bdd/environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6563 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/bdd/steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5228 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/bdd/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/sismic/clock/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/clock/clock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/sismic/code/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5932 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/code/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/code/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6738 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/code/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12867 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/code/python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3503 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/sismic/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34479 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/interpreter/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/interpreter/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.134748 sismic-1.6.5/sismic/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10641 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/io/datadict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15085 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/io/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.134748 sismic-1.6.5/sismic/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11707 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/model/elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24349 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/model/statechart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/model/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.134748 sismic-1.6.5/sismic/runner/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-05-08 13:19:09.000000 sismic-1.6.5/sismic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.130748 sismic-1.6.5/sismic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6850 2023-05-08 13:19:21.000000 sismic-1.6.5/sismic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-05-08 13:19:21.000000 sismic-1.6.5/sismic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 13:19:21.000000 sismic-1.6.5/sismic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-08 13:19:21.000000 sismic-1.6.5/sismic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-08 13:19:21.000000 sismic-1.6.5/sismic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-08 13:19:21.000000 sismic-1.6.5/sismic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 13:19:20.000000 sismic-1.6.5/sismic.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.134748 sismic-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10271 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4372 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2173 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26016 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24839 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4166 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:19:21.138748 sismic-1.6.5/tests/yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/composite.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/deep_history.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/final.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/history.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/infinite.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/internal.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/nested_parallel.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/nondeterministic.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/parallel.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/priority.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-08 13:19:09.000000 sismic-1.6.5/tests/yaml/timer.yaml
```

### Comparing `sismic-1.6.4/CHANGELOG.rst` & `sismic-1.6.5/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.6.5 (2023-05-08)
+------------------
+
+ - (Fixed) Dropped support for Python 3.5 and 3.6 since they are no longer supported by ``ruamel.yaml`` used internally.
+
+
 1.6.4 (2023-03-03)
 ------------------
 
  - (Fixed) Invalid output of ``export_to_plantuml`` if ``statechart_preamble`` is enabled, with plantuml-1.2022.12 (`#119 <https://github.com/AlexandreDecan/sismic/issues/119>`__).
 
 
 1.6.3 (2021-08-05)
```

### Comparing `sismic-1.6.4/LICENSE` & `sismic-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/PKG-INFO` & `sismic-1.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sismic
-Version: 1.6.4
+Version: 1.6.5
 Summary: Sismic Interactive Statechart Model Interpreter and Checker
 Home-page: https://github.com/AlexandreDecan/sismic/
 Author: Alexandre Decan
 License: LGPL3
 Keywords: statechart state machine interpreter model uml scxml harel
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -13,20 +13,19 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Sismic for Python
 =================
 
@@ -41,15 +40,15 @@
 
 Sismic Interactive Statechart Model Interpreter and Checker
 -----------------------------------------------------------
 
 *Sismic* is a recursive acronym that stands for *Sismic Interactive Statechart Model Interpreter and Checker*.
 
 Statecharts are a well-known visual modeling language for representing the executable behavior
-of complex reactive event-based systems. Sismic library for Python (version 3.5 or higher) provides a set of
+of complex reactive event-based systems. Sismic library for Python (version 3.6 or higher) provides a set of
 tools to define, validate, simulate, execute and test statecharts.
 More specifically, Sismic provides:
 
 - An easy way to define and to import statecharts, based on the human-friendly YAML markup language
 - A statechart interpreter offering a discrete, step-by-step, and fully observable simulation engine
 - Fully controllable simulation clock, with support for real and simulated time
 - Built-in support for expressing actions and guards using regular Python code, can be easily extended to other programming languages
@@ -60,15 +59,15 @@
 - Synchronous and asynchronous executions
 - Statechart visualization using `PlantUML <http://www.plantuml.com/plantuml>`__
 
 
 Installation
 ------------
 
-Sismic requires Python >=3.5.
+Sismic requires Python >=3.7.
 Sismic can be installed using ``pip`` as usual: ``pip install sismic``.
 This will install the latest stable version.
 
 You can also install Sismic from this repository by cloning it.
 
 Starting from release 1.0.0, Sismic adheres to a `semantic versioning <https://semver.org>`__ scheme.
```

### Comparing `sismic-1.6.4/README.rst` & `sismic-1.6.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Sismic Interactive Statechart Model Interpreter and Checker
 -----------------------------------------------------------
 
 *Sismic* is a recursive acronym that stands for *Sismic Interactive Statechart Model Interpreter and Checker*.
 
 Statecharts are a well-known visual modeling language for representing the executable behavior
-of complex reactive event-based systems. Sismic library for Python (version 3.5 or higher) provides a set of
+of complex reactive event-based systems. Sismic library for Python (version 3.6 or higher) provides a set of
 tools to define, validate, simulate, execute and test statecharts.
 More specifically, Sismic provides:
 
 - An easy way to define and to import statecharts, based on the human-friendly YAML markup language
 - A statechart interpreter offering a discrete, step-by-step, and fully observable simulation engine
 - Fully controllable simulation clock, with support for real and simulated time
 - Built-in support for expressing actions and guards using regular Python code, can be easily extended to other programming languages
@@ -31,15 +31,15 @@
 - Synchronous and asynchronous executions
 - Statechart visualization using `PlantUML <http://www.plantuml.com/plantuml>`__
 
 
 Installation
 ------------
 
-Sismic requires Python >=3.5.
+Sismic requires Python >=3.7.
 Sismic can be installed using ``pip`` as usual: ``pip install sismic``.
 This will install the latest stable version.
 
 You can also install Sismic from this repository by cloning it.
 
 Starting from release 1.0.0, Sismic adheres to a `semantic versioning <https://semver.org>`__ scheme.
```

### Comparing `sismic-1.6.4/docs/Makefile` & `sismic-1.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/behavior.rst` & `sismic-1.6.5/docs/behavior.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/code.rst` & `sismic-1.6.5/docs/code.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/concurrent.rst` & `sismic-1.6.5/docs/concurrent.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/conf.py` & `sismic-1.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/contract.rst` & `sismic-1.6.5/docs/contract.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/Elevator.graffle` & `sismic-1.6.5/docs/examples/elevator/Elevator.graffle`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/elevator.feature` & `sismic-1.6.5/docs/examples/elevator/elevator.feature`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/elevator.plantuml` & `sismic-1.6.5/docs/examples/elevator/elevator.plantuml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/elevator.png` & `sismic-1.6.5/docs/examples/elevator/elevator.png`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/elevator.yaml` & `sismic-1.6.5/docs/examples/elevator/elevator.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/elevator_buttons.yaml` & `sismic-1.6.5/docs/examples/elevator/elevator_buttons.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/elevator_contract.yaml` & `sismic-1.6.5/docs/examples/elevator/elevator_contract.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/tester_elevator_7th_floor_never_reached.yaml` & `sismic-1.6.5/docs/examples/elevator/tester_elevator_7th_floor_never_reached.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/elevator/tester_elevator_moves_after_10s.yaml` & `sismic-1.6.5/docs/examples/elevator/tester_elevator_moves_after_10s.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/cooking_human.feature` & `sismic-1.6.5/docs/examples/microwave/cooking_human.feature`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/heating.feature` & `sismic-1.6.5/docs/examples/microwave/heating.feature`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/heating_off_property.yaml` & `sismic-1.6.5/docs/examples/microwave/heating_off_property.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/heating_on_property.yaml` & `sismic-1.6.5/docs/examples/microwave/heating_on_property.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/heating_property.yaml` & `sismic-1.6.5/docs/examples/microwave/heating_property.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/lighting_human.feature` & `sismic-1.6.5/docs/examples/microwave/lighting_human.feature`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/microwave.py` & `sismic-1.6.5/docs/examples/microwave/microwave.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/microwave.yaml` & `sismic-1.6.5/docs/examples/microwave/microwave.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/microwave_with_contracts.yaml` & `sismic-1.6.5/docs/examples/microwave/microwave_with_contracts.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/steps.py` & `sismic-1.6.5/docs/examples/microwave/steps.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/microwave/test_microwave.py` & `sismic-1.6.5/docs/examples/microwave/test_microwave.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch.graffle` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch.graffle`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch.py` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch.yaml` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_external.yaml` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_external.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_gui.png` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_gui.png`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_gui.py` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_gui.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_gui_external.py` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_gui_external.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_overview.png` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_overview.png`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_with_logic.png` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_with_logic.png`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/stopwatch/stopwatch_with_object.png` & `sismic-1.6.5/docs/examples/stopwatch/stopwatch_with_object.png`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/examples/writer_options.yaml` & `sismic-1.6.5/docs/examples/writer_options.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/execution.rst` & `sismic-1.6.5/docs/execution.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/extensions.rst` & `sismic-1.6.5/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/format.rst` & `sismic-1.6.5/docs/format.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/index.rst` & `sismic-1.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/installation.rst` & `sismic-1.6.5/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Installation
 ============
 
 Using pip
 ---------
 
-Sismic requires Python >=3.5, and can be installed using ``pip`` as usual: ``pip install sismic``.
+Sismic requires Python >=3.7, and can be installed using ``pip`` as usual: ``pip install sismic``.
 This will install the latest stable version.
 Starting from release 1.0.0, Sismic adheres to a `semantic versioning <https://semver.org>`__ scheme.
 
 You can isolate Sismic installation by using virtual environments:
 
 1. Get the tool to create virtual environments: ``pip install virtualenv``
 2. Create the environment: ``virtualenv -p python3.5 env``
```

### Comparing `sismic-1.6.4/docs/integration.rst` & `sismic-1.6.5/docs/integration.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/properties.rst` & `sismic-1.6.5/docs/properties.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/time.rst` & `sismic-1.6.5/docs/time.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/unittests.rst` & `sismic-1.6.5/docs/unittests.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/docs/visualization.rst` & `sismic-1.6.5/docs/visualization.rst`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/setup.py` & `sismic-1.6.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,20 +33,19 @@
         'Topic :: Software Development :: Interpreters',
         'Topic :: Software Development :: Testing',
         'Topic :: Scientific/Engineering',
 
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
 
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='statechart state machine interpreter model uml scxml harel',
 
     packages=find_packages(exclude=['docs', 'tests']),
     python_requires='>=3.5',
     install_requires=[
         'ruamel.yaml>=0.12.10',
```

### Comparing `sismic-1.6.4/sismic/bdd/__main__.py` & `sismic-1.6.5/sismic/bdd/__main__.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/bdd/environment.py` & `sismic-1.6.5/sismic/bdd/environment.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/bdd/steps.py` & `sismic-1.6.5/sismic/bdd/steps.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/bdd/wrappers.py` & `sismic-1.6.5/sismic/bdd/wrappers.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/clock/clock.py` & `sismic-1.6.5/sismic/clock/clock.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/code/context.py` & `sismic-1.6.5/sismic/code/context.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/code/dummy.py` & `sismic-1.6.5/sismic/code/dummy.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/code/evaluator.py` & `sismic-1.6.5/sismic/code/evaluator.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/code/python.py` & `sismic-1.6.5/sismic/code/python.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/exceptions.py` & `sismic-1.6.5/sismic/exceptions.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/helpers.py` & `sismic-1.6.5/sismic/helpers.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/interpreter/default.py` & `sismic-1.6.5/sismic/interpreter/default.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/interpreter/listener.py` & `sismic-1.6.5/sismic/interpreter/listener.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/io/datadict.py` & `sismic-1.6.5/sismic/io/datadict.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/io/plantuml.py` & `sismic-1.6.5/sismic/io/plantuml.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/io/yaml.py` & `sismic-1.6.5/sismic/io/yaml.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/model/elements.py` & `sismic-1.6.5/sismic/model/elements.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/model/events.py` & `sismic-1.6.5/sismic/model/events.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/model/statechart.py` & `sismic-1.6.5/sismic/model/statechart.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/model/steps.py` & `sismic-1.6.5/sismic/model/steps.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/runner/runner.py` & `sismic-1.6.5/sismic/runner/runner.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic/testing.py` & `sismic-1.6.5/sismic/testing.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/sismic.egg-info/PKG-INFO` & `sismic-1.6.5/sismic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sismic
-Version: 1.6.4
+Version: 1.6.5
 Summary: Sismic Interactive Statechart Model Interpreter and Checker
 Home-page: https://github.com/AlexandreDecan/sismic/
 Author: Alexandre Decan
 License: LGPL3
 Keywords: statechart state machine interpreter model uml scxml harel
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -13,20 +13,19 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Sismic for Python
 =================
 
@@ -41,15 +40,15 @@
 
 Sismic Interactive Statechart Model Interpreter and Checker
 -----------------------------------------------------------
 
 *Sismic* is a recursive acronym that stands for *Sismic Interactive Statechart Model Interpreter and Checker*.
 
 Statecharts are a well-known visual modeling language for representing the executable behavior
-of complex reactive event-based systems. Sismic library for Python (version 3.5 or higher) provides a set of
+of complex reactive event-based systems. Sismic library for Python (version 3.6 or higher) provides a set of
 tools to define, validate, simulate, execute and test statecharts.
 More specifically, Sismic provides:
 
 - An easy way to define and to import statecharts, based on the human-friendly YAML markup language
 - A statechart interpreter offering a discrete, step-by-step, and fully observable simulation engine
 - Fully controllable simulation clock, with support for real and simulated time
 - Built-in support for expressing actions and guards using regular Python code, can be easily extended to other programming languages
@@ -60,15 +59,15 @@
 - Synchronous and asynchronous executions
 - Statechart visualization using `PlantUML <http://www.plantuml.com/plantuml>`__
 
 
 Installation
 ------------
 
-Sismic requires Python >=3.5.
+Sismic requires Python >=3.7.
 Sismic can be installed using ``pip`` as usual: ``pip install sismic``.
 This will install the latest stable version.
 
 You can also install Sismic from this repository by cloning it.
 
 Starting from release 1.0.0, Sismic adheres to a `semantic versioning <https://semver.org>`__ scheme.
```

### Comparing `sismic-1.6.4/sismic.egg-info/SOURCES.txt` & `sismic-1.6.5/sismic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/conftest.py` & `sismic-1.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_bdd.py` & `sismic-1.6.5/tests/test_bdd.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_clock.py` & `sismic-1.6.5/tests/test_clock.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_code.py` & `sismic-1.6.5/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_contract.py` & `sismic-1.6.5/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_examples.py` & `sismic-1.6.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_interpreter.py` & `sismic-1.6.5/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_io.py` & `sismic-1.6.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_model.py` & `sismic-1.6.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_property.py` & `sismic-1.6.5/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/test_runner.py` & `sismic-1.6.5/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/composite.yaml` & `sismic-1.6.5/tests/yaml/composite.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/deep_history.yaml` & `sismic-1.6.5/tests/yaml/deep_history.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/final.yaml` & `sismic-1.6.5/tests/yaml/final.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/history.yaml` & `sismic-1.6.5/tests/yaml/history.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/nested_parallel.yaml` & `sismic-1.6.5/tests/yaml/nested_parallel.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/parallel.yaml` & `sismic-1.6.5/tests/yaml/parallel.yaml`

 * *Files identical despite different names*

### Comparing `sismic-1.6.4/tests/yaml/timer.yaml` & `sismic-1.6.5/tests/yaml/timer.yaml`

 * *Files identical despite different names*

