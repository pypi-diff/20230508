# Comparing `tmp/modelbase-1.9.3.tar.gz` & `tmp/modelbase-1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbase-1.9.3.tar", max compression
+gzip compressed data, was "dist/modelbase-1rc2.tar", last modified: Tue Mar 31 12:46:29 2020, max compression
```

## Comparing `modelbase-1.9.3.tar` & `modelbase-1rc2.tar`

### file list

```diff
@@ -1,43 +1,93 @@
--rw-r--r--   0        0        0    35079 2022-06-07 06:51:20.868442 modelbase-1.9.3/LICENSE
--rw-r--r--   0        0        0     4152 2022-06-07 06:51:20.868442 modelbase-1.9.3/README.md
--rw-r--r--   0        0        0     3339 2022-06-07 06:51:20.877442 modelbase-1.9.3/pyproject.toml
--rw-r--r--   0        0        0      136 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/__init__.py
--rw-r--r--   0        0        0      423 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/__init__.py
--rw-r--r--   0        0        0    20702 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/algebraicmixin.py
--rw-r--r--   0        0        0     8806 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/basemodel.py
--rw-r--r--   0        0        0     6500 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/compoundmixin.py
--rw-r--r--   0        0        0    12855 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/parametermixin.py
--rw-r--r--   0        0        0    21775 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/ratemixin.py
--rw-r--r--   0        0        0     8535 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/stoichiometricmixin.py
--rw-r--r--   0        0        0     5529 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/core/utils.py
--rw-r--r--   0        0        0      471 2022-06-07 06:51:20.877442 modelbase-1.9.3/src/modelbase/ode/__init__.py
--rw-r--r--   0        0        0      304 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/integrators/__init__.py
--rw-r--r--   0        0        0     1274 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/integrators/abstract_integrator.py
--rw-r--r--   0        0        0     3334 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/integrators/int_assimulo.py
--rw-r--r--   0        0        0     3878 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/integrators/int_scipy.py
--rw-r--r--   0        0        0      520 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/models/__init__.py
--rw-r--r--   0        0        0     1930 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/models/abstract_model.py
--rw-r--r--   0        0        0    39722 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/models/labelmodel.py
--rw-r--r--   0        0        0    14744 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/models/linearlabelmodel.py
--rw-r--r--   0        0        0    27960 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/models/model.py
--rw-r--r--   0        0        0     2675 2022-06-07 06:51:20.878442 modelbase-1.9.3/src/modelbase/ode/simulators/__init__.py
--rw-r--r--   0        0        0    64512 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/simulators/abstract_simulator.py
--rw-r--r--   0        0        0    16060 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/simulators/labelsimulator.py
--rw-r--r--   0        0        0     9838 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/simulators/linearlabelsimulator.py
--rw-r--r--   0        0        0     5247 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/simulators/simulator.py
--rw-r--r--   0        0        0      188 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/utils/__init__.py
--rw-r--r--   0        0        0      261 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/utils/algebraicfunctions.py
--rw-r--r--   0        0        0    21387 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/utils/mca.py
--rw-r--r--   0        0        0    14205 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/utils/ratefunctions.py
--rw-r--r--   0        0        0     6035 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/ode/utils/ratelaws.py
--rw-r--r--   0        0        0        0 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/py.typed
--rw-r--r--   0        0        0       92 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/sbml/__init__.py
--rw-r--r--   0        0        0     2200 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/sbml/data.py
--rw-r--r--   0        0        0    21331 2022-06-07 06:51:20.879442 modelbase-1.9.3/src/modelbase/sbml/mathml.py
--rw-r--r--   0        0        0    40812 2022-06-07 06:51:20.880442 modelbase-1.9.3/src/modelbase/sbml/parser.py
--rw-r--r--   0        0        0     1969 2022-06-07 06:51:20.880442 modelbase-1.9.3/src/modelbase/sbml/unit_conversion.py
--rw-r--r--   0        0        0      483 2022-06-07 06:51:20.880442 modelbase-1.9.3/src/modelbase/typing.py
--rw-r--r--   0        0        0      357 2022-06-07 06:51:20.880442 modelbase-1.9.3/src/modelbase/utils/__init__.py
--rw-r--r--   0        0        0    12470 2022-06-07 06:51:20.880442 modelbase-1.9.3/src/modelbase/utils/plotting.py
--rw-r--r--   0        0        0     5471 1970-01-01 00:00:00.000000 modelbase-1.9.3/setup.py
--rw-r--r--   0        0        0     6146 1970-01-01 00:00:00.000000 modelbase-1.9.3/PKG-INFO
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     4395 2020-03-31 12:46:29.000000 modelbase-1rc2/PKG-INFO
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     3084 2020-03-31 12:27:32.000000 modelbase-1rc2/README.md
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)      164 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/core/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)      246 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    15946 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/algebraicmixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     6715 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/basemodel.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     6058 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/compoundmixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    13665 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/parametermixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    14857 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/ratemixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     9320 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/stoichiometricmixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     4880 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/core/utils.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/ode/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     1460 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/ode/models/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        1 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/models/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    37610 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/models/labelmodel.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    12771 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/models/linearlabelmodel.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    19647 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/models/model.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/ode/simulators/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/simulators/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     9888 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/simulators/basesimulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     4823 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/simulators/integrators.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    16083 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/simulators/labelsimulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     8852 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/simulators/linearlabelsimulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    41364 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/simulators/simulator.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/ode/utils/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/utils/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)      302 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/utils/algebraicfunctions.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    15038 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/utils/mca.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     7136 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/utils/ratefunctions.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     4798 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/ode/utils/ratelaws.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/pde/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)      325 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       94 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/basemodels.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       94 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/leafmodels.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/pde/utils/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       16 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/utils/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       84 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/utils/coordinates.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       82 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/utils/perffuncs.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       98 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/pde/utils/plotting.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase/utils/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       16 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/utils/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    12291 2020-03-31 12:27:32.000000 modelbase-1rc2/modelbase/utils/plotting.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase.egg-info/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     4395 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase.egg-info/PKG-INFO
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)     2341 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        1 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        1 2019-10-15 11:35:33.000000 modelbase-1rc2/modelbase.egg-info/not-zip-safe
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)       85 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase.egg-info/requires.txt
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)       16 2020-03-31 12:46:29.000000 modelbase-1rc2/modelbase.egg-info/top_level.txt
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)       38 2020-03-31 12:46:29.000000 modelbase-1rc2/setup.cfg
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     2442 2020-03-31 12:27:32.000000 modelbase-1rc2/setup.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/
+-rw-rw-rw-   0 marvin    (1047) marvin    (1047)        0 2019-09-16 10:52:26.000000 modelbase-1rc2/tests/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/core/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-02-23 15:14:10.000000 modelbase-1rc2/tests/core/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    24251 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_algebraic_mixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     5183 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_base_model.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    10199 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_compound_mixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    14160 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_parameter_mixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    22943 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_rate_mixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    10587 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_stoichiometric_mixin.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     5247 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/core/test_utils.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/ode/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-02-23 19:01:18.000000 modelbase-1rc2/tests/ode/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/ode/integrators/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/integrators/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    11154 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/integrators/test_integrator_assimulo.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     9782 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/integrators/test_integrator_scipy.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/ode/model/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/model/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    55861 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/model/test_label_model.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     9259 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/model/test_linear_label_model.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    45689 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/model/test_model.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/ode/simulator/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/simulator/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    12038 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/simulator/test_base_simulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     6901 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/simulator/test_label_simulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     5770 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/simulator/test_linear_label_simulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     7755 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/simulator/test_simulator.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     6816 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/simulator/test_simulator_plotting.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)      456 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/test_algebraicfunctions.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    17517 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/test_mca.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    12101 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/test_ratefunctions.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)    10755 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/ode/test_ratelaws.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/pde/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-19 08:13:33.000000 modelbase-1rc2/tests/pde/__init__.py
+drwxrwxr-x   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:46:29.000000 modelbase-1rc2/tests/utils/
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)        0 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/utils/__init__.py
+-rw-rw-r--   0 marvin    (1047) marvin    (1047)     4713 2020-03-31 12:27:32.000000 modelbase-1rc2/tests/utils/test_plotting.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `modelbase-1.9.3/src/modelbase/core/algebraicmixin.py` & `modelbase-1rc2/modelbase/core/algebraicmixin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,513 +1,408 @@
-from __future__ import annotations
+"""Mixin for algebraic modules. These are used to calculate e.g. QSSA assumptions."""
 
-__all__ = [
-    "Module",
-    "AlgebraicModule",
-]
-
-import copy
 import warnings
-from dataclasses import dataclass, field
-from queue import Empty, SimpleQueue
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generator,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    Union,
-)
 
-import libsbml
-import numpy as np
+from dataclasses import field
+from dataclasses import dataclass
 
-from ..typing import Array
-from .basemodel import BaseModel
-from .compoundmixin import CompoundMixin
-from .parametermixin import ParameterMixin
 from .utils import (
-    check_function_arity,
     get_formatted_function_source_code,
     patch_lambda_function_name,
     warning_on_one_line,
 )
 
-warnings.formatwarning = warning_on_one_line  # type: ignore
+warnings.formatwarning = warning_on_one_line
 
 
 @dataclass
 class Module:
     """Meta-info container for an algebraic module."""
 
-    common_name: Optional[str] = None
+    common_name: str = None
     notes: dict = field(default_factory=dict)
     database_links: dict = field(default_factory=dict)
 
 
-class AlgebraicModule:
-    """Container for algebraic modules"""
-
-    def __init__(
-        self,
-        name: str,
-        function: Union[Callable[..., float], Callable[..., Iterable[float]]],
-        derived_compounds: List[str],
-        compounds: List[str],
-        modifiers: List[str],
-        parameters: List[str],
-        dynamic_variables: List[str],
-        args: List[str],
-    ):
-        self.name = name
-        self.function = function
-        self.compounds = compounds
-        self.derived_compounds = derived_compounds
-        self.modifiers = modifiers
-        self.parameters = parameters
-        self.dynamic_variables = dynamic_variables
-        self.args = args
-
-    def check_consistency(self) -> None:
-        """Check whether all arguments exists and the arity matches"""
-        self._check_dynamic_variables()
-        self._check_module_args()
-
-        if not check_function_arity(function=self.function, arity=len(self.args)):
-            warnings.warn(f"Function arity does not match args of {self.name}")
-
-    def _check_dynamic_variables(self) -> None:
-        difference = set(self.dynamic_variables).difference(self.compounds + self.modifiers)
-        if difference:
-            warnings.warn(
-                f"Supplied args {difference} for module {self.name} that aren't in compounds or modifiers"
-            )
-
-    def _check_module_args(self) -> None:
-        difference = set(self.args).difference(self.dynamic_variables + self.parameters)
-        if difference:
-            warnings.warn(
-                f"Supplied args {difference} for module {self.name} that aren't in compounds, modifiers or parameters"
-            )
-
-    def __repr__(self) -> str:
-        return repr(self.__dict__)
-
-    def __str__(self) -> str:
-        return f"{self.function.__name__}({', '.join(self.args)}) -> {self.derived_compounds}"
-
-    def keys(self) -> List[str]:
-        """Get all valid keys of the algebraic module"""
-        return [
-            "function",
-            "compounds",
-            "derived_compounds",
-            "modifiers",
-            "parameters",
-            "dynamic_variables",
-            "args",
-        ]
-
-    def __getitem__(self, key: str) -> Any:
-        return self.__dict__[key]
-
-    def __iter__(self) -> Generator:
-        yield "function", self.function
-        yield "compounds", self.compounds
-        yield "derived_compounds", self.derived_compounds
-        yield "modifiers", self.modifiers
-        yield "parameters", self.parameters
-        yield "dynamic_variables", self.dynamic_variables
-        yield "args", self.args
-
-    def copy(self) -> AlgebraicModule:
-        """Create a copy of the module"""
-        return copy.deepcopy(self)
-
-
-class AlgebraicMixin(ParameterMixin, CompoundMixin, BaseModel):
+class AlgebraicMixin:
     """Mixin for algebraic modules.
 
     This adds the capability to calculate concentrations of derived
     compounds that are calculated before the rate functions are calculated.
     """
 
-    def __init__(self, algebraic_modules: Optional[Dict[str, Dict[str, Any]]] = None) -> None:
-        self.algebraic_modules: Dict[str, AlgebraicModule] = {}
-        self._algebraic_module_order: List[str] = []
+    def __init__(self, algebraic_modules=None):
+        self.derived_compounds = []
+        self.algebraic_modules = {}
         if algebraic_modules is not None:
             self.add_algebraic_modules(algebraic_modules=algebraic_modules)
 
     ##########################################################################
     # Derived compound functions
     ##########################################################################
 
-    def get_derived_compounds(self) -> List[str]:
-        """Return names of compounds derived from algebraic modules."""
-        derived_compounds = []
-        for module in self.algebraic_modules.values():
-            derived_compounds.extend(module.derived_compounds)
-        return derived_compounds
+    def _add_derived_compound(self, compound):
+        """Add a derived compound to the model.
 
-    @property
-    def derived_compounds(self) -> List[str]:
-        """Return names of compounds derived from algebraic modules
+        Derived compounds are dynamic quantities calculated by algebraic modules.
+        They are accessible by other rates but are not returned to any integrators.
 
-        Used to be an attribute of the model, so this is kept to ensure backwards compatability
+        Parameters
+        ----------
+        compound : str
+            Name / id of the compound
         """
-        return self.get_derived_compounds()
+        if not isinstance(compound, str):
+            raise TypeError("The compound name should be string")
+        if compound == "time":
+            raise KeyError("time is a protected variable for time")
+        if compound in self.derived_compounds:
+            warnings.warn(f"Overwriting derived compound {compound}")
+        self.derived_compounds.append(compound)
 
-    def _get_all_compounds(self) -> List[str]:
-        return list(self.get_compounds() + self.get_derived_compounds())
+    def _add_derived_compounds(self, compounds):
+        """Add multiple derived compounds to the model.
 
-    def get_all_compounds(self) -> List[str]:
-        """Return names of compounds and derived compounds (in that order)."""
-        return self._get_all_compounds()
+        Derived compounds are dynamic quantities calculated by algebraic modules.
+        They are accessible by other rates but are not returned to any integrators.
+
+        Parameters
+        ----------
+        compounds : Iterable(str)
+
+        See Also
+        --------
+        _add_derived_compound
+        """
+        for compound in compounds:
+            self._add_derived_compound(compound=compound)
+
+    def _remove_derived_compound(self, compound):
+        """Remove a derived compound from the model.
+
+        Parameters
+        ----------
+        compound : str
+            Name / id of the compound
+        """
+        self.derived_compounds.remove(compound)
+
+    def _remove_derived_compounds(self, compounds):
+        """Remove multiple derived compounds from the model.
+
+        Parameters
+        ----------
+        compounds : Iterable(str)
+        """
+        for compound in compounds:
+            self._remove_derived_compound(compound=compound)
+
+    def get_derived_compounds(self):
+        """Return names of compounds derived from algebraic modules.
+
+        Returns
+        -------
+        derived_compounds : list(str)
+        """
+        return list(self.derived_compounds)
+
+    def get_all_compounds(self):
+        """Return names of compounds and derived compounds in that order.
+
+        Returns
+        -------
+        all_compounds: list(str)
+        """
+        return list(self.get_compounds() + self.get_derived_compounds())
 
     ##########################################################################
     # Algebraic Modules
     ##########################################################################
 
-    def _sort_algebraic_modules(self, max_iterations: int = 10_000) -> None:
-        def submodule(v: AlgebraicModule) -> Dict[str, Set[str]]:
-            return {
-                "in": set(v.compounds),
-                "out": set(v.derived_compounds),
-            }
-
-        available_compounds = set(self.compounds)
-        module_order = []
-        modules_to_sort: SimpleQueue = SimpleQueue()
-        for k, v in self.algebraic_modules.items():
-            modules_to_sort.put((k, submodule(v)))
-
-        last_name = None
-        i = 0
-        while True:
-            try:
-                name, mod = modules_to_sort.get_nowait()
-            except Empty:
-                break
-            if mod["in"].issubset(available_compounds):
-                available_compounds.update(mod["out"])
-                module_order.append(name)
-            else:
-                if last_name == name:
-                    module_order.append(name)
-                    break
-                modules_to_sort.put((name, mod))
-                last_name = name
-            i += 1
-            if i > max_iterations:
-                raise ValueError(
-                    "Exceeded max iterations on algebraic module sorting. Check if there are circular references."
-                )
-        self._algebraic_module_order = module_order
-
-    def _check_module_consistency(self, module: AlgebraicModule, check_ids: bool = True) -> None:
-        self._check_for_existence(
-            name=module.name,
-            check_against=self.get_all_compounds(),
-            candidates=module.compounds + module.modifiers,
-            element_type="compound",
-            raise_on_missing=False,
-        )
-        self._check_for_existence(
-            name=module.name,
-            check_against=self.get_parameter_names(),
-            candidates=module.parameters,
-            element_type="parameter",
-        )
-        if check_ids:
-            self._check_and_insert_ids(module.derived_compounds, context=module.name)
-        module.check_consistency()
-
     def add_algebraic_module(
         self,
-        module_name: str,
-        function: Union[Callable[..., float], Callable[..., Iterable[float]]],
-        compounds: List[str] | None = None,
-        derived_compounds: List[str] | None = None,
-        modifiers: List[str] | None = None,
-        parameters: List[str] | None = None,
-        dynamic_variables: List[str] | None = None,
-        args: List[str] | None = None,
-        check_consistency: bool = True,
-        sort_modules: bool = True,
-        **meta_info: Dict[str, Any],
-    ) -> None:
+        module_name,
+        function,
+        compounds=None,
+        derived_compounds=None,
+        modifiers=None,
+        parameters=None,
+        **meta_info,
+    ):
         """Add an algebraic module to the model.
 
         CAUTION: The Python function of the module has to return an iterable.
         The Python function will get the function arguments in the following order:
         [**compounds, **modifiers, **parameters]
 
+        Parameters
+        ----------
+        module_name : str
+            Name of the module
+        function : callable
+            Python method of the algebraic module
+        compounds : iterable(str)
+            Names of compounds used for module
+        derived_compounds : iterable(str)
+            Names of compounds which are calculated by the module
+        modifiers : iterable(str)
+            Names of compounds which act as modifiers on the module
+        parameters : iterable(str)
+            Names of the parameters which are passed to the function
+        meta_info : dict, optional
+            Meta info of the algebraic module. Allowed keys are
+            {common_name, notes, database_links}
+
         Warns
         -----
         UserWarning
             If algebraic module is already in the model.
 
         Examples
         --------
-        def rapid_equilibrium(substrate, k_eq)-> None:
+        def rapid_equilibrium(substrate, k_eq):
             x = substrate / (1 + k_eq)
             y = substrate * k_eq / (1 + k_eq)
             return x, y
 
         add_algebraic_module(
             module_name="fast_eq",
             function=rapid_equilibrium,
             compounds=["A"],
             derived_compounds=["X", "Y"],
             parameters=["K"],
         )
         """
-        if module_name in self.algebraic_modules:
-            self.remove_algebraic_module(module_name=module_name)
-            warnings.warn(f"Overwriting algebraic module {module_name}")
-
-        patch_lambda_function_name(function=function, name=module_name)
-
         if compounds is None:
             compounds = []
         if derived_compounds is None:
             derived_compounds = []
         if modifiers is None:
             modifiers = []
         if parameters is None:
             parameters = []
-        if dynamic_variables is None:
-            dynamic_variables = compounds + modifiers
-        if args is None:
-            args = dynamic_variables + parameters
 
-        module = AlgebraicModule(
-            name=module_name,
-            function=function,
-            compounds=compounds,
-            derived_compounds=derived_compounds,
-            modifiers=modifiers,
-            parameters=parameters,
-            dynamic_variables=dynamic_variables,
-            args=args,
-        )
-        self.algebraic_modules[module_name] = module
+        patch_lambda_function_name(function=function, name=module_name)
+
+        if module_name in self.algebraic_modules:
+            self.remove_algebraic_module(module_name=module_name)
+            warnings.warn(f"Overwriting algebraic module {module_name}")
+
+        self.algebraic_modules[module_name] = {
+            "function": function,
+            "compounds": compounds,
+            "derived_compounds": derived_compounds,
+            "modifiers": modifiers,
+            "parameters": parameters,
+        }
+        for compound in derived_compounds:
+            self._add_derived_compound(compound=compound)
 
         self.meta_info.setdefault("modules", {}).setdefault(
-            module_name,
-            Module(**meta_info),  # type: ignore
+            module_name, Module(**meta_info)
         )
 
-        if check_consistency:
-            self._check_module_consistency(module)
-        if sort_modules:
-            self._sort_algebraic_modules()
-
-    def add_algebraic_modules(self, algebraic_modules: dict, meta_info: dict | None = None) -> None:
+    def add_algebraic_modules(self, algebraic_modules, meta_info=None):
         """Add multiple algebraic modules to the model.
 
+        CAUTION: The Python function of the module has to return an iterable.
+
+        Parameters
+        ----------
+        algebraic_modules : dict
+
         See Also
         --------
         add_algebraic_module
         """
         meta_info = {} if meta_info is None else meta_info
         for module_name, module in algebraic_modules.items():
-            info = meta_info.get(module_name, {})
+            try:
+                info = meta_info[module_name]
+            except KeyError:
+                info = {}
             self.add_algebraic_module(module_name=module_name, **module, **info)
 
     def update_algebraic_module(
         self,
-        module_name: str,
-        function: Union[Callable[..., float], Callable[..., Iterable[float]]] | None = None,
-        compounds: List[str] | None = None,
-        derived_compounds: List[str] | None = None,
-        modifiers: List[str] | None = None,
-        parameters: List[str] | None = None,
-        dynamic_variables: List[str] | None = None,
-        args: List[str] | None = None,
-        check_consistency: bool = True,
-        sort_modules: bool = True,
-    ) -> None:
-        """Update an existing reaction."""
-        module = self.algebraic_modules[module_name]
-        args_have_changed = False
-        derived_have_changed = False
-
-        if function is not None:
-            patch_lambda_function_name(function=function, name=module_name)
-            module.function = function
-
-        if compounds is not None:
-            module.compounds = compounds
-            args_have_changed = True
-        else:
-            compounds = module.compounds
-
-        if derived_compounds is not None:
-            self._remove_ids(module.derived_compounds)
-            module.derived_compounds = derived_compounds
-            derived_have_changed = True
-
-        if modifiers is not None:
-            module.modifiers = modifiers
-            args_have_changed = True
-        else:
-            modifiers = module.modifiers
-
-        if parameters is not None:
-            module.parameters = parameters
-            args_have_changed = True
-        else:
-            parameters = module.parameters
-
-        if dynamic_variables is not None:
-            args_have_changed = True
-            module.dynamic_variables = dynamic_variables
-        elif args_have_changed:
-            dynamic_variables = compounds + modifiers
-            module.dynamic_variables = dynamic_variables
-        else:
-            dynamic_variables = module.dynamic_variables
-
-        if args is not None:
-            dynamic_variables = [i for i in args if i in module.dynamic_variables]
-            module.dynamic_variables = dynamic_variables
-            module.args = args
-        elif args_have_changed:
-            args = dynamic_variables + parameters
-            module.args = args
-        else:
-            args = module.args
-
-        if check_consistency:
-            self._check_module_consistency(module, check_ids=derived_have_changed)
-        if sort_modules:
-            self._sort_algebraic_modules()
-
-    def update_algebraic_modules(self, modules: dict) -> None:
-        """Update multiple algebraic modules
+        module_name,
+        function=None,
+        compounds=None,
+        derived_compounds=None,
+        modifiers=None,
+        parameters=None,
+        **meta_info,
+    ):
+        """Update an existing reaction.
 
-        See Also
-        --------
-        update_algebraic_module
+        Parameters
+        ----------
+        module_name : str
+            Name of the module
+        function : callable
+            Python method of the algebraic module
+        compounds : iterable(str)
+            Names of compounds used for module
+        derived_compounds : iterable(str)
+            Names of compounds which are calculated by the module
+        modifiers : iterable(str)
+            Names of compounds which act as modifiers on the module
+        parameters : iterable(str)
+            Names of the parameters which are passed to the function
+        meta_info : dict(module_name, meta_info)
+            Meta info of the algebraic module. Allowed keys are
+            {common_name, notes, database_links}
         """
-        for name, module in modules.items():
-            self.update_algebraic_module(name, **module)
+        if function is None:
+            function = self.algebraic_modules[module_name]["function"]
+        if compounds is None:
+            compounds = self.algebraic_modules[module_name]["compounds"]
+        if derived_compounds is None:
+            derived_compounds = self.algebraic_modules[module_name]["derived_compounds"]
+        if modifiers is None:
+            modifiers = self.algebraic_modules[module_name]["modifiers"]
+        if parameters is None:
+            parameters = self.algebraic_modules[module_name]["parameters"]
+        meta = self.meta_info["modules"][module_name].__dict__
+        meta.update(meta_info)
+        self.remove_algebraic_module(module_name=module_name)
+        self.add_algebraic_module(
+            module_name=module_name,
+            function=function,
+            compounds=compounds,
+            derived_compounds=derived_compounds,
+            modifiers=modifiers,
+            parameters=parameters,
+            **meta,
+        )
 
-    def update_module_meta_info(self, module: str, meta_info: dict) -> None:
+    def update_module_meta_info(self, module, meta_info):
         """Update meta info of an algebraic module.
 
         Parameters
         ----------
         module : str
             Name of the algebraic module
         meta_info : dict
             Meta info of the algebraic module. Allowed keys are
             {common_name, notes, database_links}
         """
         self.update_meta_info(component="modules", meta_info={module: meta_info})
 
-    def remove_algebraic_module(self, module_name: str, sort_modules: bool = True) -> None:
+    def remove_algebraic_module(self, module_name):
         """Remove an algebraic module.
 
         Parameters
         ----------
         module_name : str
             Name of the algebraic module
         """
         module = self.algebraic_modules.pop(module_name)
-        self._remove_ids(module.derived_compounds)
-        if sort_modules:
-            self._sort_algebraic_modules()
+        for compound in module["derived_compounds"]:
+            self._remove_derived_compound(compound=compound)
 
-    def remove_algebraic_modules(self, module_names: List[str]) -> None:
+    def remove_algebraic_modules(self, module_names):
         """Remove multiple algebraic modules.
 
         Parameters
         ----------
         module_names : iterable(str)
             Names of the algebraic modules
         """
         for module_name in module_names:
             self.remove_algebraic_module(module_name=module_name)
 
-    def get_algebraic_module(self, module_name: str) -> AlgebraicModule:
-        """Return the algebraic module"""
-        return self.algebraic_modules[module_name]
-
-    def get_algebraic_module_function(
-        self, module_name: str
-    ) -> Union[Callable[..., float], Callable[..., Iterable[float]]]:
-        """Return the function of the algebraic module"""
-        return self.algebraic_modules[module_name].function
-
-    def get_algebraic_module_compounds(self, module_name: str) -> List[str]:
-        """Return the compounds of the algebraic module"""
-        return list(self.algebraic_modules[module_name].compounds)
-
-    def get_algebraic_module_derived_compounds(self, module_name: str) -> List[str]:
-        """Return the derived compounds of the algebraic module"""
-        return list(self.algebraic_modules[module_name].derived_compounds)
-
-    def get_algebraic_module_modifiers(self, module_name: str) -> List[str]:
-        """Return the modifiers of the algebraic module"""
-        return list(self.algebraic_modules[module_name].modifiers)
-
-    def get_algebraic_module_parameters(self, module_name: str) -> List[str]:
-        """Return the parameters of the algebraic module"""
-        return list(self.algebraic_modules[module_name].parameters)
-
-    def get_algebraic_module_args(self, module_name: str) -> List[str]:
-        """Return the arguments of the algebraic module function"""
-        return list(self.algebraic_modules[module_name].args)
+    def get_algebraic_module_compounds(self, module_name):
+        """Return the compounds of the algebraic module.
+
+        Parameters
+        ----------
+        module_name : str
+            Name of the algebraic module
+
+        Returns
+        -------
+        module_compounds : list(str)
+        """
+        return list(self.algebraic_modules[module_name]["compounds"])
+
+    def get_algebraic_module_derived_compounds(self, module_name):
+        """Return the derived compounds of the algebraic module.
+
+        Parameters
+        ----------
+        module_name : str
+            Name of the algebraic module
+
+        Returns
+        -------
+        module_compounds : list(str)
+            Derived compounds of the algebraic module
+        """
+        return list(self.algebraic_modules[module_name]["derived_compounds"])
+
+    def get_algebraic_module_modifiers(self, module_name):
+        """Return the derived compounds of the algebraic module.
+
+        Parameters
+        ----------
+        module_name : str
+            Name of the algebraic module
+
+        Returns
+        -------
+        module_compounds : list(str)
+            Derived compounds of the algebraic module
+        """
+        return list(self.algebraic_modules[module_name]["modifiers"])
+
+    def get_algebraic_module_parameters(self, module_name):
+        """Return the parameters of the algebraic module.
+
+        Parameters
+        ----------
+        module_name : str
+            Name of the algebraic module
+
+        Returns
+        -------
+        parameters : list(str)
+            Parameters of the algebraic module
+        """
+        return list(self.algebraic_modules[module_name]["parameters"])
 
     ##########################################################################
     # Simulation functions
     ##########################################################################
 
-    def _get_fcd(
-        self,
-        *,
-        t: Array,
-        y: Dict[str, Array],
-    ) -> Dict[str, Array]:
+    def _get_fcd(self, t, y):
         """Calculate the derived variables of all algebraic modules.
 
-        fdc = full_concentration_dict
-
-        The derived compounds are sorted by the algebraic modules and their internal
-        derived_modules attribute.
+        Parameters
+        ----------
+        t : num, array(num)
+            One are multiple time points
+        y : dict(str: num)
+            A dictionary of the concentrations of all non-derived compounds
         """
         y["time"] = t
-        # args = self.parameters | y # that is python 3.9+ syntax, wait for a bit
-        args: Dict[str, Union[float, Array]] = {**self.parameters, **y}
-        for name, module in self.algebraic_modules.items():
-            try:
-                derived_values = module.function(*(args[arg] for arg in module.args))
-            except KeyError as e:
-                raise KeyError(f"Could not find argument {e} for module {name}") from e
-            derived_compounds = dict(
-                zip(
-                    module.derived_compounds,
-                    np.array(derived_values).reshape((len(module.derived_compounds), -1)),
-                )
+        for module in self.algebraic_modules.values():
+            derived_values = module["function"](
+                *(y[var] for var in module["compounds"]),
+                *(y[var] for var in module["modifiers"]),
+                *(self.parameters[par] for par in module["parameters"]),
             )
-            y.update(derived_compounds)
-            args.update(derived_compounds)
+            y.update(zip(module["derived_compounds"], derived_values))
         return y
 
     ##########################################################################
     # Source code functions
     ##########################################################################
 
-    def _generate_algebraic_modules_source_code(self, *, include_meta_info: bool = True) -> Tuple[str, str]:
+    def _generate_algebraic_modules_source_code(self, include_meta_info=True):
         """Generate modelbase source code for algebraic modules.
 
         This is mainly used for the generate_model_source_code function.
 
         Parameters
         ----------
         include_meta_info : bool
@@ -520,54 +415,53 @@
         algebraic_module_modelbase_code : str
             Code generating the modelbase objects
 
         See Also
         --------
         generate_model_source_code
         """
+        if include_meta_info:
+            meta_info = self._get_nonzero_meta_info(component="modules")
         module_functions = set()
         modules = []
         for name, module in self.algebraic_modules.items():
-            function = module.function
-            compounds = module.compounds
-            derived_compounds = module.derived_compounds
-            modifiers = module.modifiers
-            parameters = module.parameters
-            args = module.args
+            function = module["function"]
+            compounds = module["compounds"]
+            derived_compounds = module["derived_compounds"]
+            modifiers = module["modifiers"]
+            parameters = module["parameters"]
 
             function_code = get_formatted_function_source_code(
                 function_name=name, function=function, function_type="module"
             )
             module_functions.add(function_code)
             module_definition = (
                 "m.add_algebraic_module(\n"
                 f"    module_name={repr(name)},\n"
                 f"    function={function.__name__},\n"
                 f"    compounds={compounds},\n"
                 f"    derived_compounds={derived_compounds},\n"
                 f"    modifiers={modifiers},\n"
                 f"    parameters={parameters},\n"
-                f"    args={args},\n"
             )
             if include_meta_info:
-                meta_info = self._get_nonzero_meta_info(component="modules")
                 try:
                     info = meta_info[name]
                     module_definition += f"**{info}"
                 except KeyError:
                     pass
             module_definition += ")"
             modules.append(module_definition)
         return "\n".join(sorted(module_functions)), "\n".join(modules)
 
     ##########################################################################
     # SBML functions
     ##########################################################################
 
-    def _create_sbml_algebraic_modules(self, *, _sbml_model: libsbml.Model) -> None:
+    def _create_sbml_algebraic_modules(self, sbml_model):
         """Convert the algebraic modules their sbml equivalent.
 
         Notes
         -----
         The closest we can get in SBML are assignment rules of the form x = f(V), see
         http://sbml.org/Software/libSBML/docs/python-api/classlibsbml_1_1_assignment_rule.html
```

### Comparing `modelbase-1.9.3/src/modelbase/core/basemodel.py` & `modelbase-1rc2/modelbase/core/basemodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,39 @@
-from __future__ import annotations
+"""Base model module."""
 
-__all__ = [
-    "Model",
-    "BaseModel",
-]
-
-import copy
-import warnings
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
+import copy as copy
+import libsbml as libsbml
 from datetime import datetime
-from types import TracebackType
-from typing import Any, Dict, List, Optional
-
-import libsbml
-from typing_extensions import Self, TypeAlias
-
-from .utils import convert_id_to_sbml, warning_on_one_line
+from abc import ABC, abstractmethod
+from dataclasses import field
+from dataclasses import dataclass
 
-warnings.formatwarning = warning_on_one_line  # type: ignore
+from .utils import convert_id_to_sbml
 
 
 @dataclass
 class Model:
     """Meta-info container for model."""
 
-    sbo: Optional[str] = None
-    id: Optional[str] = None
-    name: Optional[str] = None
+    sbo: str = None
+    id: str = None
+    name: str = None
     units: dict = field(default_factory=dict)
     compartments: dict = field(default_factory=dict)
     notes: dict = field(default_factory=dict)
 
 
 class BaseModel(ABC):
     """Abstract model class."""
 
-    def __init__(self, meta_info: Dict[str, Any] | None = None) -> None:
-        default_meta_info: Dict[str, Any] = {
+    def __init__(self, meta_info=None):
+        default_meta_info = {
             "sbo": "SBO:0000004",  # modelling framework
             "id": f"modelbase-model-{datetime.now().date().strftime('%Y-%m-%d')}",
-            "name": "modelbase-model",
+            "name": f"modelbase-model",
             "units": {
                 "per_second": {
                     "kind": libsbml.UNIT_KIND_SECOND,
                     "exponent": -1,
                     "scale": 0,
                     "multiplier": 1,
                 },
@@ -57,88 +46,44 @@
                     "spatial_dimensions": 3,
                     "units": "litre",
                 }
             },
         }
         if meta_info is not None:
             default_meta_info.update(meta_info)
-        self.meta_info: Dict[str, Any] = {"model": Model(**default_meta_info)}
-        self._ids: set[str] = set()
-        self._copy: BaseModel | None = None
+        self.meta_info = {"model": Model(**default_meta_info)}
 
-    def __enter__(self) -> Self:  # type: ignore
+    def __enter__(self):
         """Enter the context manager.
 
         Returns
         -------
             Deepcopy of the model object
         """
         self._copy = self.copy()
         return self.copy()
 
-    def __exit__(
-        self,
-        exception_type: Optional[BaseException],
-        exception_value: Optional[BaseException],
-        exception_traceback: Optional[TracebackType],
-    ) -> None:
+    def __exit__(self, exception_type, exception_value, exception_traceback):
         """Exit the context manager.
 
         Restores any changes made to the model structure.
         """
-        if self._copy is not None:
-            self.__dict__ = self._copy.__dict__
+        self.__dict__ = self._copy.__dict__
 
-    def copy(self) -> Self:  # type: ignore
+    def copy(self):
         """Create a deepcopy of the model.
 
         Returns
         -------
         model
             Deepcopy of the model object
         """
-        return copy.deepcopy(self)  # type: ignore
-
-    def _check_for_existence(
-        self,
-        *,
-        name: str,
-        check_against: List[str],
-        candidates: List[str],
-        element_type: str,
-        raise_on_missing: bool = False,
-    ) -> None:
-        to_check = set(check_against)
-        to_check.add("time")
-        for i in set(candidates).difference(to_check):
-            if raise_on_missing:
-                raise KeyError(f"Could not find {element_type} {i} for {name}")
-            warnings.warn(f"Could not find {element_type} {i} for {name}")
-
-    def _check_and_insert_ids(self, ids: List[str], context: str) -> None:
-        for id_ in ids:
-            if id_ in self._ids:
-                warnings.warn(
-                    f"{context}: Id {id_} already exists in the model. This might lead to variable shading!"
-                )
-            self._ids.add(id_)
-
-    def _update_ids(self, ids: Dict[str, str]) -> None:
-        for k, v in ids.items():
-            self._ids.remove(k)
-            self._ids.add(v)
-
-    def _remove_ids(self, ids: List[str]) -> None:
-        for id_ in ids:
-            try:
-                self._ids.remove(id_)
-            except KeyError:
-                warnings.warn("Could not find id. Do you have duplicate ids in the model?")
+        return copy.deepcopy(self)
 
-    def update_meta_info(self, component: str, meta_info: dict) -> None:
+    def update_meta_info(self, component, meta_info):
         """Add meta info for any given model component.
 
         Parameters
         ----------
         component : str
             Name of the component. Available components depend of the model type
         meta_info : dict
@@ -148,15 +93,15 @@
         for k1, d in meta_info.items():
             if isinstance(d, dict):
                 for k2, v in d.items():
                     setattr(self.meta_info[component][k1], k2, v)
             else:
                 setattr(self.meta_info[component], k1, d)
 
-    def _get_nonzero_meta_info(self, *, component: str) -> Dict[str, Any]:
+    def _get_nonzero_meta_info(self, component):
         """Get meta info of a component for all entries that are not None.
 
         Parameters
         ----------
         component : str
             Name of the component. Available components depend of the model type
         """
@@ -167,15 +112,15 @@
                 meta_info[k1] = info
         return meta_info
 
     ##########################################################################
     # SBML functions
     ##########################################################################
 
-    def _create_sbml_document(self) -> libsbml.SBMLDocument:
+    def _create_sbml_document(self):
         """Create an sbml document, into which sbml information can be written.
 
         Returns
         -------
         doc : libsbml.Document
         """
         # SBML namespaces
@@ -183,36 +128,40 @@
         sbml_ns.addPackageNamespace("fbc", 2)
         # SBML document
         doc = libsbml.SBMLDocument(sbml_ns)
         doc.setPackageRequired("fbc", False)
         doc.setSBOTerm(self.meta_info["model"].sbo)
         return doc
 
-    def _create_sbml_model(self, *, doc: libsbml.SBMLDocument) -> libsbml.Model:
+    def _create_sbml_model(self, doc):
         """Create an sbml model.
 
         Parameters
         ----------
         doc : libsbml.Document
 
         Returns
         -------
         sbml_model : libsbml.Model
         """
         sbml_model = doc.createModel()
-        sbml_model.setId(convert_id_to_sbml(id_=self.meta_info["model"].id, prefix="MODEL"))
-        sbml_model.setName(convert_id_to_sbml(id_=self.meta_info["model"].name, prefix="MODEL"))
+        sbml_model.setId(
+            convert_id_to_sbml(id_=self.meta_info["model"].id, prefix="MODEL")
+        )
+        sbml_model.setName(
+            convert_id_to_sbml(id_=self.meta_info["model"].name, prefix="MODEL")
+        )
         sbml_model.setTimeUnits("second")
         sbml_model.setExtentUnits("mole")
         sbml_model.setSubstanceUnits("mole")
         sbml_model_fbc = sbml_model.getPlugin("fbc")
         sbml_model_fbc.setStrict(True)
         return sbml_model
 
-    def _create_sbml_units(self, *, sbml_model: libsbml.Model) -> None:
+    def _create_sbml_units(self, sbml_model):
         """Create sbml units out of the meta_info.
 
         Parameters
         ----------
         sbml_model : libsbml.Model
         """
         for unit_id, unit in self.meta_info["model"].units.items():
@@ -220,15 +169,15 @@
             sbml_definition.setId(unit_id)
             sbml_unit = sbml_definition.createUnit()
             sbml_unit.setKind(unit["kind"])
             sbml_unit.setExponent(unit["exponent"])
             sbml_unit.setScale(unit["scale"])
             sbml_unit.setMultiplier(unit["multiplier"])
 
-    def _create_sbml_compartments(self, *, sbml_model: libsbml.Model) -> None:
+    def _create_sbml_compartments(self, sbml_model):
         """Create the compartments for the sbml model.
 
         Since modelbase does not enforce any compartments, so far
         only a cytosol placeholder is introduced.
 
         Parameters
         ----------
@@ -240,27 +189,26 @@
             sbml_compartment.setName(compartment["name"])
             sbml_compartment.setConstant(compartment["is_constant"])
             sbml_compartment.setSize(compartment["size"])
             sbml_compartment.setSpatialDimensions(compartment["spatial_dimensions"])
             sbml_compartment.setUnits(compartment["units"])
 
     @abstractmethod
-    def _model_to_sbml(self) -> None:
+    def _model_to_sbml(self):
         """Define which methods shall be used for sbml export."""
 
-    def write_sbml_model(self, filename: str | None = None) -> Optional[str]:
+    def write_sbml_model(self, filename=None):
         """Write the model to an sbml file.
 
         Parameters
         ----------
         filename : str
 
         Returns
         -------
         doc : libsbml.Document
         """
         doc = self._model_to_sbml()
         if filename is not None:
             libsbml.writeSBMLToFile(doc, filename)
-            return None
-        model_str: str = libsbml.writeSBMLToString(doc)
-        return model_str
+        else:
+            return libsbml.writeSBMLToString(doc)
```

### Comparing `modelbase-1.9.3/src/modelbase/core/ratemixin.py` & `modelbase-1rc2/modelbase/ode/models/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,636 +1,602 @@
-from __future__ import annotations
+"""Main ODE model module.
 
-__all__ = [
-    "Rate",
-    "RateMeta",
-    "RateMixin",
-]
+Description of the module
+"""
 
-import copy
-import warnings
-from collections import defaultdict
-from dataclasses import dataclass, field
-from typing import Any, Callable, Dict, Generator, List, Optional, Tuple
-
-import libsbml
+import subprocess
 import numpy as np
+import pandas as pd
+import libsbml
+import warnings
 
-from ..typing import Array
-from . import BaseModel, CompoundMixin, ParameterMixin
-from .utils import (
-    check_function_arity,
-    convert_id_to_sbml,
-    get_formatted_function_source_code,
-    patch_lambda_function_name,
-    warning_on_one_line,
+from ...core import (
+    BaseModel,
+    CompoundMixin,
+    ParameterMixin,
+    AlgebraicMixin,
+    StoichiometricMixin,
+    RateMixin,
 )
 
-warnings.formatwarning = warning_on_one_line  # type: ignore
+from ...core.utils import convert_id_to_sbml
 
 
-class Rate:
-    """A container for a rate"""
+class Model(
+    RateMixin,
+    StoichiometricMixin,
+    AlgebraicMixin,
+    ParameterMixin,
+    CompoundMixin,
+    BaseModel,
+):
+    """The main class for modeling. Provides model construction and inspection tools."""
 
     def __init__(
         self,
-        name: str,
-        function: Callable[..., float],
-        substrates: List[str],
-        products: List[str],
-        modifiers: List[str],
-        dynamic_variables: List[str],
-        parameters: List[str],
-        reversible: bool,
-        args: List[str],
+        parameters=None,
+        compounds=None,
+        algebraic_modules=None,
+        rate_stoichiometries=None,
+        rates=None,
+        meta_info=None,
     ):
-        self.name = name
-        self.function = function
-        self.substrates = substrates
-        self.products = products
-        self.modifiers = modifiers
-        self.parameters = parameters
-        self.dynamic_variables = dynamic_variables
-        self.args = args
-        self.reversible = reversible
-
-    def _check_rate_dynamic_variables(self) -> None:
-        if self.reversible:
-            difference = set(self.dynamic_variables).difference(
-                self.substrates + self.products + self.modifiers
-            )
-            targets = "substrates, products or modifiers"
-        else:
-            difference = set(self.dynamic_variables).difference(self.substrates + self.modifiers)
-            targets = "substrates or modifiers"
-        if difference:
-            warnings.warn(
-                f"Supplied dynamic variables {difference} for rate {self.name} that aren't in {targets}"
-            )
-
-    def _check_rate_args(self) -> None:
-        difference = set(self.args).difference(self.dynamic_variables + self.parameters)
-        if self.reversible:
-            targets = "substrates, products, modifiers or parameters"
-        else:
-            targets = "substrates, modifiers or parameters"
-        if difference:
-            warnings.warn(f"Supplied args {difference} for rate {self.name} that aren't in {targets}")
-
-    def check_consistency(self) -> None:
-        """Check if args and arity of the rate are ok."""
-        self._check_rate_dynamic_variables()
-        self._check_rate_args()
-        if not check_function_arity(function=self.function, arity=len(self.args)):
-            warnings.warn(f"Function arity does not match args of {self.name}")
-
-    def __repr__(self) -> str:
-        return repr(self.__dict__)
-
-    def __str__(self) -> str:
-        return f"{self.function.__name__}({', '.join(self.args)}) -> {', '.join(self.products)}"
-
-    def keys(self) -> List[str]:
-        """Get all valid keys of the rate"""
-        return [
-            "function",
-            "substrates",
-            "products",
-            "modifiers",
-            "dynamic_variables",
-            "parameters",
-            "reversible",
-            "args",
-        ]
-
-    def __getitem__(self, key: str) -> Any:
-        return self.__dict__[key]
-
-    def __iter__(self) -> Generator:
-        yield "function", self.function
-        yield "substrates", self.substrates
-        yield "products", self.products
-        yield "modifiers", self.modifiers
-        yield "parameters", self.parameters
-        yield "dynamic_variables", self.dynamic_variables
-        yield "args", self.args
-        yield "reversible", self.reversible
-
-    def copy(self) -> Rate:
-        """Create a copy of the rate"""
-        return copy.deepcopy(self)
-
-
-@dataclass
-class RateMeta:
-    """Meta-info container for rates."""
-
-    common_name: Optional[str] = None
-    unit: Optional[str] = None
-    gibbs0: Optional[float] = None
-    ec: Optional[str] = None
-    database_links: dict = field(default_factory=dict)
-    notes: dict = field(default_factory=dict)
-    sbml_function: Optional[str] = None
-    python_function: Optional[str] = None
-
-
-class RateMixin(ParameterMixin, CompoundMixin, BaseModel):
-    """Mixin adding rate functions."""
-
-    def __init__(
-        self, rates: dict[str, Rate] | None = None, functions: dict[str, Callable[..., float]] | None = None
-    ) -> None:
-        self.rates: Dict[str, Rate] = {}
-        self.functions: Dict[str, Callable[..., float]] = {}
-        if rates is not None:
-            self.add_rates(rates=rates)
-        if functions is not None:
-            self.add_functions(functions=functions)
+        BaseModel.__init__(self, meta_info=meta_info)
+        CompoundMixin.__init__(self, compounds=compounds)
+        ParameterMixin.__init__(self, parameters=parameters)
+        AlgebraicMixin.__init__(self, algebraic_modules=algebraic_modules)
+        StoichiometricMixin.__init__(self, rate_stoichiometries=rate_stoichiometries)
+        RateMixin.__init__(self, rates=rates)
+        self.meta_info["model"].sbo = "SBO:0000062"  # continuous framework
+
+    def __str__(self):
+        """Give a string representation.
+
+        Returns
+        -------
+        representation : str
+        """
+        return (
+            "Model:"
+            + f"\n    {len(self.get_compounds())} Compounds"
+            + f"\n    {len(self.get_stoichiometries())} Reactions"
+        )
 
     ##########################################################################
-    # Basic rate functions
+    # Reactions
     ##########################################################################
 
-    def add_function(self, function_name: str, function: Callable[..., float]) -> None:
-        """Add a function to the model"""
-        if function.__name__ == "<lambda>":
-            patch_lambda_function_name(function=function, name=function_name)
-
-        self.functions[function_name] = function
-
-    def add_functions(self, functions: Dict[str, Callable[..., float]]) -> None:
-        """Add multiple functions to the model"""
-        for function_name, function in functions.items():
-            self.add_function(function_name=function_name, function=function)
-
-    def update_function(self, function_name: str, function: Callable[..., float]) -> None:
-        """Update a function"""
-        if function.__name__ == "<lambda>":
-            patch_lambda_function_name(function=function, name=function_name)
-        self.functions[function_name] = function
-
-    def update_functions(self, functions: Dict[str, Callable[..., float]]) -> None:
-        """Update multiple functions"""
-        for function_name, function in functions.items():
-            self.update_function(function_name, function)
-
-    def remove_function(self, function_name: str) -> None:
-        """Remove a function from the model"""
-        del self.functions[function_name]
-
-    def remove_functions(self, function_names: List[str]) -> None:
-        """Remove multiple functions from the model"""
-        for function_name in function_names:
-            self.remove_function(function_name)
-
-    def _check_rate_consistency(self, rate: Rate) -> None:
-        self._check_for_existence(
-            name=rate.name,
-            check_against=self._get_all_compounds(),
-            candidates=rate.dynamic_variables,
-            element_type="compound",
-        )
-        self._check_for_existence(
-            name=rate.name,
-            check_against=self.get_parameter_names(),
-            candidates=rate.parameters,
-            element_type="parameter",
-        )
-        rate.check_consistency()
-
-    def add_rate(
+    def add_reaction(
         self,
-        rate_name: str,
-        function: Callable[..., float],
-        substrates: List[str] | None = None,
-        products: List[str] | None = None,
-        modifiers: List[str] | None = None,
-        dynamic_variables: List[str] | None = None,
-        parameters: List[str] | None = None,
-        reversible: bool = False,
-        args: List[str] | None = None,
-        check_consistency: bool = True,
-        **meta_info: Dict[str, Any],
-    ) -> None:
-        """Add a rate function to the model.
-
-        The Python function will get the function arguments in the following order:
-        [**substrates, **(products if reversible), **modifiers, **parameters.]
+        rate_name,
+        function,
+        stoichiometry,
+        modifiers=None,
+        parameters=None,
+        reversible=False,
+        **meta_info,
+    ):
+        """Add a reaction to the model.
+
+        Shortcut for add_rate and add stoichiometry functions.
+        Additional variable ["time"] can be passed for time-dependent functions.
 
         Parameters
         ----------
-        rate_name
-            Name of the rate function
-        function
-            Python method calculating the rate equation
-        substrates
-            Names of the substrates
-        products
-            Names of the products
-        modifiers
-            Names of the modifiers. E.g time.
-        parameters
-            Names of the parameters
-        reversible
-            Whether the reaction is reversible.
-        meta_info
-            Meta info of the rate. Allowed keys are
-            {common_name, gibbs0, ec, database_links, notes, sbml_function}
-
-        Warns
-        -----
-        UserWarning
-            If rate is already in the model
+        rate_name : str
+        function : callable
+        stoichiometry : dict
+        modifiers: iterable(str)
+        parameters: iterable(str)
+        reversible: bool
 
-        Examples
+        See Also
         --------
-        def mass_action(S, k1) -> None:
-            return k1 * S
-
-        m.add_reaction(
-            rate_name="v1",
-            function=mass_action,
-            stoichiometry={"X": -1},
-            parameters=["k1"],
-        )
-
-        def reversible_mass_action(S, P, k_fwd, k_bwd) -> None:
-            return k_fwd * S - k_bwd * P
+        add_rate
+        add_stoichiometry
 
-        m.add_reaction(
-            rate_name="v2",
-            function=reversible_mass_action,
-            stoichiometry={"X": -1, "Y": 1},
-            parameters=["k2_fwd", "k2_bwd"],
-            reversible=True,
-        )
+        Examples
+        --------
+        >>> add_reaction(
+                rate_name="v1",
+                function=mass_action,
+                stoichiometry={"X": -1, "Y": 1},
+                parameters=["k2"],
+            )
+        >>> add_reaction(
+                rate_name="v1",
+                function=reversible_mass_action,
+                stoichiometry={"X": -1, "Y": 1},
+                parameters=["k1_fwd", "k1_bwd"],
+                reversible=True,
+            )
         """
-        if rate_name in self.rates:
-            warnings.warn(f"Overwriting rate {rate_name}")
-            self.remove_rate(rate_name=rate_name)
-
-        patch_lambda_function_name(function=function, name=rate_name)
-
-        if substrates is None:
-            substrates = []
-        if products is None:
-            products = []
-        if parameters is None:
-            parameters = []
-        if modifiers is None:
-            modifiers = []
-        if dynamic_variables is None:
-            if reversible:
-                dynamic_variables = substrates + products + modifiers
-            else:
-                dynamic_variables = substrates + modifiers
-        if args is None:
-            args = dynamic_variables + parameters
+        substrates = [k for k, v in stoichiometry.items() if v < 0]
+        products = [k for k, v in stoichiometry.items() if v > 0]
 
-        rate = Rate(
-            name=rate_name,
+        self.add_rate(
+            rate_name=rate_name,
             function=function,
-            parameters=parameters,
             substrates=substrates,
             products=products,
             modifiers=modifiers,
+            parameters=parameters,
             reversible=reversible,
-            dynamic_variables=dynamic_variables,
-            args=args,
-        )
-        self.rates[rate_name] = rate
-
-        self.meta_info.setdefault("rates", {}).setdefault(
-            rate_name,
-            RateMeta(**meta_info),  # type: ignore
+            **meta_info,
         )
+        self.add_stoichiometry(rate_name=rate_name, stoichiometry=stoichiometry)
 
-        if check_consistency:
-            self._check_rate_consistency(rate)
+    def update_reaction(
+        self,
+        rate_name,
+        function=None,
+        stoichiometry=None,
+        modifiers=None,
+        parameters=None,
+        reversible=None,
+        **meta_info,
+    ):
+        """Update an existing reaction.
 
-    def add_rates(self, rates: Dict[str, Any], meta_info: Optional[Dict[str, Any]] = None) -> None:
-        """Add multiple rates to the model.
+        Parameters
+        ----------
+        rate_name : str
+        function : callable, optional
+        stoichiometry : dict, optional
+        modifiers: iterable(str), optional
+        parameters: iterable(str), optional
+        reversible: bool, optional
 
         See Also
         --------
-        add_rate
+        add_reaction
+        update_rate
+        update_stoichiometry
         """
-        meta_info = {} if meta_info is None else meta_info
-        for rate_name, rate in rates.items():
-            info = meta_info.get(rate_name, {})
-            self.add_rate(rate_name=rate_name, **rate, **info)
+        if function is None:
+            function = self.rates[rate_name]["function"]
+        if stoichiometry is None:
+            stoichiometry = self.stoichiometries[rate_name]
+        if modifiers is None:
+            modifiers = self.rates[rate_name]["modifiers"]
+        if parameters is None:
+            parameters = self.rates[rate_name]["parameters"]
+        if reversible is None:
+            reversible = self.rates[rate_name]["reversible"]
+        meta = self.meta_info["rates"][rate_name].__dict__
+        meta.update(meta_info)
+        self.remove_reaction(rate_name=rate_name)
+        self.add_reaction(
+            rate_name=rate_name,
+            function=function,
+            stoichiometry=stoichiometry,
+            modifiers=modifiers,
+            parameters=parameters,
+            reversible=reversible,
+            **meta,
+        )
 
-    def update_rate(
-        self,
-        rate_name: str,
-        function: Optional[Callable[..., float]] = None,
-        substrates: Optional[List[str]] = None,
-        products: Optional[List[str]] = None,
-        modifiers: Optional[List[str]] = None,
-        parameters: Optional[List[str]] = None,
-        reversible: Optional[bool] = None,
-        dynamic_variables: Optional[List[str]] = None,
-        args: Optional[List[str]] = None,
-        check_consistency: bool = True,
-    ) -> None:
-        """Update an existing rate.
+    def add_reaction_from_ratelaw(self, rate_name, ratelaw, **meta_info):
+        """Add a reaction from a ratelaw.
 
         Parameters
         ----------
-        rate_name
-            Name of the rate function
-        function
-            Python method calculating the rate equation
-        substrates
-            Names of the substrates
-        products
-            Names of the products
-        modifiers
-            Names of the modifiers. E.g time.
-        parameters
-            Names of the parameters
-        reversible
-            Whether the reaction is reversible.
-        meta_info
-            Meta info of the rate. Allowed keys are
-            {common_name, gibbs0, ec, database_links, notes, sbml_function}
+        rate_name : str
+        ratelaw : modelbase.ode.utils.ratelaw.BaseRateLaw
+            Ratelaw instance
+        meta_info : dict, optional
 
-        See Also
+        Examples
         --------
-        add_rate
+        >>> add_reaction_from_ratelaw(
+                rate_name="v1",
+                ratelaw=ReversibleMassAction(
+                    substrates=["X"],
+                    products=["Y"],
+                    k_fwd="k1p",
+                    k_bwd="k1m"
+                ),
+            )
         """
-        rate = self.rates[rate_name]
-        reversible_changed = False
-        args_have_changed = False
-
-        if function is not None:
-            patch_lambda_function_name(function=function, name=rate_name)
-            rate.function = function
-
-        if substrates is not None:
-            args_have_changed = True
-            rate.substrates = substrates
-        else:
-            substrates = rate.substrates
+        default_meta_info = {"sbml_function": ratelaw.get_sbml_function_string()}
+        default_meta_info.update(meta_info)
 
-        if products is not None:
-            args_have_changed = True
-            rate.products = products
-        else:
-            products = rate.products
+        self.add_rate(
+            rate_name=rate_name,
+            function=ratelaw.get_rate_function(),
+            substrates=ratelaw.substrates,
+            products=ratelaw.products,
+            modifiers=ratelaw.modifiers,
+            parameters=ratelaw.parameters,
+            reversible=ratelaw.reversible,
+            **default_meta_info,
+        )
+        self.add_stoichiometry(rate_name=rate_name, stoichiometry=ratelaw.stoichiometry)
 
-        if parameters is not None:
-            args_have_changed = True
-            rate.parameters = parameters
-        else:
-            parameters = rate.parameters
+    def remove_reaction(self, rate_name):
+        """Remove a reaction from the model.
 
-        if modifiers is not None:
-            args_have_changed = True
-            rate.modifiers = modifiers
-        else:
-            modifiers = rate.modifiers
+        Parameters
+        ----------
+        rate_name : str
+        """
+        self.remove_rate(rate_name=rate_name)
+        self.remove_rate_stoichiometry(rate_name=rate_name)
 
-        if reversible is not None:
-            reversible_changed = True
-            rate.reversible = reversible
-        else:
-            reversible = rate.reversible
+    def remove_reactions(self, rate_names):
+        """Remove multiple reactions from the model.
 
-        if dynamic_variables is not None:
-            args_have_changed = True
-            rate.dynamic_variables = dynamic_variables
-        elif reversible_changed or args_have_changed:
-            if rate.reversible:
-                dynamic_variables = substrates + products + modifiers
-            else:
-                dynamic_variables = substrates + modifiers
-            rate.dynamic_variables = dynamic_variables
-        else:
-            dynamic_variables = rate.dynamic_variables
+        Parameters
+        ----------
+        names : iterable(str)
+        """
+        for rate_name in rate_names:
+            self.remove_reaction(rate_name=rate_name)
+
+    ##########################################################################
+    # Simulation functions
+    ##########################################################################
 
-        if args is not None:
-            dynamic_variables = [i for i in args if i in rate.dynamic_variables]
-            rate.dynamic_variables = dynamic_variables
-            rate.args = args
-        elif reversible_changed or args_have_changed:
-            args = dynamic_variables + parameters
-            rate.args = args
+    def get_full_concentration_dict(self, y, t=0):
+        """Calculate the derived variables (at time(s) t).
+
+        Parameters
+        ----------
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num)), optional
+
+        Returns
+        -------
+        y_full : dict
+            Dictionary of the concentrations of all compounds and derived compounds
+
+        Example
+        -------
+        >>> get_full_concentration_dict(y=[0, 0])
+        >>> get_full_concentration_dict(y={"X": 0, "Y": 0})
+        """
+        self._update_derived_parameters()
+        if isinstance(t, (int, float)):
+            t = np.array([t])
+        if isinstance(y, dict):
+            # y = y.copy()
+            y = {k: np.ones(len(t)) * v for k, v in y.items()}
         else:
-            args = rate.args
+            y = dict(zip(self.get_compounds(), (np.ones((len(t), 1)) * y).T))
+        return self._get_fcd(t=t, y=y)
 
-        if check_consistency:
-            self._check_rate_consistency(rate)
+    def get_fluxes_dict(self, y, t=0):
+        """Calculate the fluxes at time point(s) t.
 
-    def update_rates(self, rates: dict) -> None:
-        """Update multiple rates."""
-        for rate_name, rate in rates.items():
-            self.update_rate(rate_name, **rate)
+        Parameters
+        ----------
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num))
 
-    def update_rate_meta_info(self, rate: str, meta_info: dict) -> None:
-        """Update meta info of a rate.
+        Returns
+        -------
+        fluxes : dict
+        """
+        self._update_derived_parameters()
+        y = self.get_full_concentration_dict(y=y, t=t)
+        return {
+            k: np.ones(len(y["time"])) * v for k, v in self._get_fluxes(y=y).items()
+        }
+
+    def get_fluxes_array(self, y, t=0):
+        """Calculate the fluxes at time point(s) t.
 
         Parameters
         ----------
-        rate : str
-            Name of the rate
-        meta_info : dict
-            Meta info of the rate. Allowed keys are
-            {common_name, gibbs0, ec, database_links, notes, sbml_function}
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num))
+
+        Returns
+        -------
+        fluxes : numpy.array
         """
-        self.update_meta_info(component="rates", meta_info={rate: meta_info})
+        return np.array([i for i in self.get_fluxes_dict(y=y, t=t).values()]).T
 
-    def remove_rate(self, rate_name: str) -> None:
-        """Remove a rate function from the model.
+    def get_fluxes_df(self, y, t=0):
+        """Calculate the fluxes at time point(s) t.
 
         Parameters
         ----------
-        rate_name : str
-            Name of the rate
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num))
+
+        Returns
+        -------
+        fluxes : pandas.DataFrame
         """
-        del self.rates[rate_name]
+        if isinstance(t, (int, float)):
+            t = [t]
+        return pd.DataFrame(
+            data=self.get_fluxes_dict(y=y, t=t), index=t, columns=self.get_rate_names()
+        )
+
+    def _get_rhs(self, t, y):
+        """Calculate the right hand side of the ODE system.
 
-    def remove_rates(self, rate_names: List[str]) -> None:
-        """Remove multiple rate functions from the model.
+        This is the more performant version of get_right_hand_side()
+        and thus returns only an array instead of a dictionary.
+
+        Watch out that this function swaps t and y!
 
         Parameters
         ----------
-        rate_names : iterable(str)
-            Names of the rates
+        t : num
+        y : iterable(num)
+
+        Returns
+        -------
+        rhs : list
+            List of the right hand side
         """
-        for rate_name in rate_names:
-            self.remove_rate(rate_name=rate_name)
+        y = dict(zip(self.get_compounds(), y))
+        fcd = self._get_fcd(t=t, y=y)
+        fluxes = self._get_fluxes(y=fcd)
+        compounds_local = self.get_compounds()
+        dxdt = dict(zip(compounds_local, np.zeros(len(compounds_local))))
+        for k, stoc in self.stoichiometries_by_compounds.items():
+            for flux, n in stoc.items():
+                dxdt[k] += n * fluxes[flux]
+        return [dxdt[i] for i in compounds_local]
 
-    def get_rate_names(self) -> List[str]:
-        """Return all rate names."""
-        return list(self.rates)
-
-    def get_rate_function(self, rate_name: str) -> Callable[..., float]:
-        """Get the function of a rate."""
-        return self.rates[rate_name].function
-
-    def get_rate_parameters(self, rate_name: str) -> List[str]:
-        """Get the parameters of a rate."""
-        return list(self.rates[rate_name].parameters)
-
-    def get_rate_substrates(self, rate_name: str) -> List[str]:
-        """Get the substrates of a rate."""
-        return list(self.rates[rate_name].substrates)
-
-    def get_rate_products(self, rate_name: str) -> List[str]:
-        """Get the products of a rate."""
-        return list(self.rates[rate_name].products)
-
-    def get_rate_modifiers(self, rate_name: str) -> List[str]:
-        """Get the modifiers of a rate."""
-        return list(self.rates[rate_name].modifiers)
-
-    def get_rate_dynamic_variables(self, rate_name: str) -> List[str]:
-        """Get the dynamic variables of a rate."""
-        return list(self.rates[rate_name].dynamic_variables)
-
-    def get_rate_args(self, rate_name: str) -> List[str]:
-        """Get the rate function arguments of a rate."""
-        return list(self.rates[rate_name].args)
+    def get_right_hand_side(self, y, t=0):
+        """Calculate the right hand side of the ODE system.
+
+        Parameters
+        ----------
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num))
+        """
+        self._update_derived_parameters()
+        if isinstance(y, dict):
+            y = [y[i] for i in self.get_compounds()]
+        rhs = self._get_rhs(t=t, y=y)
+        eqs = [f"d{cpd}dt" for cpd in self.get_compounds()]
+        return dict(zip(eqs, rhs))
 
     ##########################################################################
-    # Simulation functions
+    # Model conversion functions
     ##########################################################################
 
-    def _get_fluxes(
-        self,
-        *,
-        fcd: Dict[str, float],
-    ) -> Dict[str, float]:
-        # args = self.parameters | fcd # python 3.9+ syntax
-        args = {**self.parameters, **fcd}
-        fluxes = {}
-        for name, rate in self.rates.items():
-            try:
-                fluxes[name] = float(rate.function(*(args[arg] for arg in rate.args)))
-            except KeyError as e:
-                raise KeyError(f"Could not find argument {e} for rate {name}") from e
-        return fluxes
+    def to_labelmodel(self, labelcompounds, labelmaps):
+        """Create a LabelModel from this model.
 
-    def _get_fluxes_array(
-        self,
-        *,
-        fcd: Dict[str, float],
-    ) -> Dict[str, Array]:
-        # args = self.parameters | fcd # python 3.9+ syntax
-        args = {**self.parameters, **fcd}
-        fluxes = {}
-        for name, rate in self.rates.items():
-            try:
-                fluxes[name] = np.atleast_1d(rate.function(*(args[arg] for arg in rate.args)))
-            except KeyError as e:
-                raise KeyError(f"Could not find argument {e} for rate {name}") from e
-        return fluxes
+        Parameters
+        ----------
+        labelcompounds : dict
+            Mapping compound to the amount of labels they can carry
+        labelmaps : dict
+            Mapping reaction to labelmap
+
+        Returns
+        -------
+        LabelModel: modelbase.ode.LabelModel
 
-    ##########################################################################
-    # Source code functions
-    ##########################################################################
+        Examples
+        --------
+        >>> m = Model()
+        >>> m.add_reaction(
+                rate_name="TPI",
+                function=reversible_mass_action_1_1,
+                stoichiometry={"GAP": -1, "DHAP": 1},
+                parameters=["kf_TPI", "kr_TPI"],
+                reversible=True,
+            )
+        >>> labelcompounds = {"GAP": 3, "DHAP": 3}
+        >>> labelmaps = {"TPI": [2, 1, 0]}
+        >>> m.to_labelmodel(labelcompounds=labelcompounds, labelmaps=labelmaps)
+        """
+        from modelbase.ode import LabelModel
+
+        lm = LabelModel()
+        lm.add_parameters(self.parameters)
+        for compound in self.get_compounds():
+            if compound in labelcompounds:
+                lm.add_label_compound(
+                    compound=compound, num_labels=labelcompounds[compound]
+                )
+            else:
+                lm.add_compound(compound=compound)
 
-    def _generate_function_source_code(self) -> str:
-        function_strings = []
-        for name, function in self.functions.items():
-            function_code = get_formatted_function_source_code(
-                function_name=name, function=function, function_type="function"
+        for module_name, module in self.algebraic_modules.items():
+            lm.add_algebraic_module(
+                module_name=module_name,
+                function=module["function"],
+                compounds=module["compounds"],
+                derived_compounds=module["derived_compounds"],
+                modifiers=module["modifiers"],
+                parameters=module["parameters"],
             )
-            function_strings.append(function_code)
-        return "\n".join(sorted(function_strings))
 
-    def _generate_rates_source_code(self, *, include_meta_info: bool = True) -> Tuple[str, str]:
-        """Generate modelbase source code for rates.
+        for rate_name, rate_dict in self.rates.items():
+            if rate_name not in labelmaps:
+                lm.add_reaction(
+                    rate_name=rate_name,
+                    function=rate_dict["function"],
+                    stoichiometry=self.stoichiometries[rate_name],
+                    modifiers=rate_dict["modifiers"],
+                    parameters=rate_dict["parameters"],
+                    reversible=rate_dict["reversible"],
+                )
+            else:
+                lm.add_labelmap_reaction(
+                    rate_name=rate_name,
+                    function=rate_dict["function"],
+                    stoichiometry=self.stoichiometries[rate_name],
+                    labelmap=labelmaps[rate_name],
+                    modifiers=rate_dict["modifiers"],
+                    parameters=rate_dict["parameters"],
+                    reversible=rate_dict["reversible"],
+                )
+        return lm
 
-        See Also
+    def to_linear_labelmodel(self, labelcompounds, labelmaps):
+        """Create a LinearLabelModel from this model.
+
+        Watch out that for a linear label model reversible reactions have to be split
+        into a forward and backward part.
+
+        Parameters
+        ----------
+        labelcompounds : dict
+            Mapping compound to the amount of labels they can carry
+        labelmaps : dict
+            Mapping reaction to labelmap
+
+        Returns
+        -------
+        LabelModel: modelbase.ode.LabelModel
+
+        Examples
         --------
-        generate_model_source_code
+        >>> m = Model()
+        >>> m.add_reaction(
+                rate_name="TPI_fwd",
+                function=_mass_action_1_1,
+                stoichiometry={"GAP": -1, "DHAP": 1},
+                parameters=["kf_TPI"],
+            )
+        >>> m.add_reaction(
+                rate_name="TPI_bwd",
+                function=mass_action_1_1,
+                stoichiometry={"DHAP": -1, "GAP": 1},
+                parameters=["kr_TPI"],
+            )
+        >>> labelcompounds = {"GAP": 3, "DHAP": 3}
+        >>> labelmaps = {"TPI_fwd": [2, 1, 0], 'TPI_bwd': [2, 1, 0]}
+        >>> m.to_linear_labelmodel(labelcompounds=labelcompounds, labelmaps=labelmaps)
         """
-        rate_functions = set()
-        rates = []
+        from modelbase.ode import LinearLabelModel
+
+        lm = LinearLabelModel()
+        for compound in self.get_compounds():
+            if compound in labelcompounds:
+                lm.add_compound(compound=compound, num_labels=labelcompounds[compound])
+
+        for rate_name, rate_dict in self.rates.items():
+            if rate_name in labelmaps:
+                if rate_dict["reversible"]:
+                    warnings.warn(
+                        f"Reaction {rate_name} is annotated as reversible. "
+                        "Did you remember to split it into a forward and backward part?"
+                    )
+                lm.add_reaction(
+                    rate_name=rate_name,
+                    stoichiometry={
+                        k: v
+                        for k, v in self.stoichiometries[rate_name].items()
+                        if k in labelcompounds
+                    },
+                    labelmap=labelmaps[rate_name],
+                )
+            else:
+                warnings.warn(f"Skipping reaction {rate_name} as no labelmap is given")
+        return lm
+
+    ##########################################################################
+    # Source code functions
+    ##########################################################################
+
+    def generate_model_source_code(self, linted=True, include_meta_info=False):
+        """Generate source code of the model.
 
-        for name, rate in self.rates.items():
-            function = rate.function
-            substrates = rate.substrates
-            products = rate.products
-            modifiers = rate.modifiers
-            parameters = rate.parameters
-            reversible = rate.reversible
-            args = rate.args
+        Parameters
+        ----------
+        linted : bool
+            Whether the source code should be formatted via black.
+            Usually it only makes sense to turn this off if there is an error somewhere.
+        include_meta_info : bool
+            Whether to include meta info of the model components
+
+        Returns
+        -------
+        model_source_code : str
+        """
+        parameters = self._generate_parameters_source_code(
+            include_meta_info=include_meta_info
+        )
+        compounds = self._generate_compounds_source_code(
+            include_meta_info=include_meta_info
+        )
+        module_functions, modules = self._generate_algebraic_modules_source_code(
+            include_meta_info=include_meta_info
+        )
+        rate_functions, rates = self._generate_rates_source_code(
+            include_meta_info=include_meta_info
+        )
+        stoichiometries = self._generate_stoichiometries_source_code()
 
-            function_code = get_formatted_function_source_code(
-                function_name=name, function=function, function_type="rate"
+        model_string = "\n".join(
+            (
+                "from modelbase.ode import Model, Simulator",
+                module_functions,
+                rate_functions,
+                "m = Model()",
+                parameters,
+                compounds,
+                modules,
+                rates,
+                stoichiometries,
             )
-            rate_functions.add(function_code)
-            rate_definition = (
-                "m.add_rate(\n"
-                f"    rate_name={repr(name)},\n"
-                f"    function={function.__name__},\n"
-                f"    substrates={substrates},\n"
-                f"    products={products},\n"
-                f"    modifiers={modifiers},\n"
-                f"    parameters={parameters},\n"
-                f"    reversible={reversible},\n"
-                f"    args={args},\n"
+        )
+        if linted:
+            blacked_string = subprocess.run(
+                ["black", "-c", model_string], stdout=subprocess.PIPE
             )
-            if include_meta_info:
-                meta_info = self._get_nonzero_meta_info(component="rates")
-                try:
-                    info = meta_info[name]
-                    rate_definition += f"    **{info}\n"
-                except KeyError:
-                    pass
-            rate_definition += ")"
-            rates.append(rate_definition)
-        return "\n".join(sorted(rate_functions)), "\n".join(rates)
+            return blacked_string.stdout.decode("utf-8")
+        else:
+            return model_string
 
     ##########################################################################
     # SBML functions
     ##########################################################################
 
-    def _create_sbml_rates(self, *, sbml_model: libsbml.Model) -> None:
-        """Convert the rates into sbml reactions.
+    def _create_sbml_reactions(self, sbml_model):
+        """Create the reactions for the sbml model.
 
         Parameters
         ----------
         sbml_model : libsbml.Model
         """
-        for rate_id, rate in self.rates.items():
-            meta_info = self.meta_info["rates"][rate_id]
-
+        for rate_id, stoichiometry in self.stoichiometries.items():
+            rate = self.meta_info["rates"][rate_id]
             rxn = sbml_model.createReaction()
             rxn.setId(convert_id_to_sbml(id_=rate_id, prefix="RXN"))
-            name = meta_info.common_name
+            name = rate.common_name
             if name:
                 rxn.setName(name)
             rxn.setFast(False)
-            rxn.setReversible(rate.reversible)
+            rxn.setReversible(self.rates[rate_id]["reversible"])
 
-            substrates: defaultdict[str, int] = defaultdict(int)
-            products: defaultdict[str, int] = defaultdict(int)
-            for compound in rate.substrates:
-                substrates[compound] += 1
-            for compound in rate.products:
-                products[compound] += 1
-
-            for compound, stoichiometry in substrates.items():
-                sref = rxn.createReactant()
-                sref.setSpecies(convert_id_to_sbml(id_=compound, prefix="CPD"))
-                sref.setStoichiometry(stoichiometry)
+            for compound_id, factor in stoichiometry.items():
+                if factor < 0:
+                    sref = rxn.createReactant()
+                else:
+                    sref = rxn.createProduct()
+                sref.setSpecies(convert_id_to_sbml(id_=compound_id, prefix="CPD"))
+                sref.setStoichiometry(abs(factor))
                 sref.setConstant(False)
 
-            for compound, stoichiometry in products.items():
-                sref = rxn.createProduct()
-                sref.setSpecies(convert_id_to_sbml(id_=compound, prefix="CPD"))
-                sref.setStoichiometry(stoichiometry)
-                sref.setConstant(False)
-
-            for compound in rate.modifiers:
+            for compound in self.rates[rate_id]["modifiers"]:
                 sref = rxn.createModifier()
                 sref.setSpecies(convert_id_to_sbml(id_=compound, prefix="CPD"))
 
-            function = meta_info.sbml_function
+            function = rate.sbml_function
             if function is not None:
                 kinetic_law = rxn.createKineticLaw()
                 kinetic_law.setMath(libsbml.parseL3Formula(function))
+
+    def _model_to_sbml(self):
+        """Export model to sbml."""
+        doc = self._create_sbml_document()
+        sbml_model = self._create_sbml_model(doc=doc)
+        self._create_sbml_units(sbml_model=sbml_model)
+        self._create_sbml_compartments(sbml_model=sbml_model)
+        self._create_sbml_compounds(sbml_model=sbml_model)
+        if bool(self.algebraic_modules):
+            self._create_sbml_algebraic_modules(sbml_model=sbml_model)
+        self._create_sbml_reactions(sbml_model=sbml_model)
+        return doc
```

### Comparing `modelbase-1.9.3/src/modelbase/ode/models/labelmodel.py` & `modelbase-1rc2/modelbase/ode/models/labelmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,66 @@
-from __future__ import annotations
+"""LabelModel base class."""
 
-__all__ = ["LabelModel"]
-
-import copy
-import itertools as it
 import warnings
-from collections import defaultdict
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, cast
-
-import libsbml
+import itertools as it
 import numpy as np
 import pandas as pd
+import libsbml
+from collections import defaultdict as _defaultdict
 
-from ...core.compoundmixin import Compound
-from ...core.ratemixin import RateMeta
-from ...core.utils import convert_id_to_sbml, warning_on_one_line
-from ...typing import Array, ArrayLike
 from .model import Model
+from ...core.compoundmixin import Compound
+from ...core.ratemixin import Rate
+from ...core.utils import warning_on_one_line, convert_id_to_sbml
 
-warnings.formatwarning = warning_on_one_line  # type: ignore
+warnings.formatwarning = warning_on_one_line
 
 
-def total_concentration(*args: float) -> List[Array]:
+def total_concentration(*args):
     """Return concentration of all isotopomers.
 
     Algebraic module function to keep track of the total
     concentration of a compound (so sum of its isotopomers).
     """
-    return [np.sum(args, axis=0)]  # type: ignore
+    return [np.sum(args, axis=0)]
 
 
 class LabelModel(Model):
     """LabelModel."""
 
     def __init__(
         self,
-        parameters: dict[str, float] | None = None,
-        compounds: List[str] | None = None,
-        algebraic_modules: dict[str, dict[str, Any]] | None = None,
-        rate_stoichiometries: Dict[str, Dict[str, int]] | None = None,
-        rates: dict[str, dict[str, Any]] | None = None,
-        meta_info: dict | None = None,
+        parameters=None,
+        compounds=None,
+        algebraic_modules=None,
+        rate_stoichiometries=None,
+        rates=None,
+        meta_info=None,
     ):
-        self.label_compounds: Dict[str, Dict[str, Any]] = {}
-        self.nonlabel_compounds: List[str] = []
-        self.base_reactions: Dict[str, Dict[str, Any]] = {}
+        self.label_compounds = {}
+        self.nonlabel_compounds = []
+        self.base_reactions = {}
         super().__init__(
             parameters=parameters,
             compounds=compounds,
             algebraic_modules=algebraic_modules,
             rate_stoichiometries=rate_stoichiometries,
             rates=rates,
             meta_info=meta_info,
         )
 
-    def __enter__(self) -> LabelModel:
-        """Enter the context manager.
-
-        Returns
-        -------
-            Deepcopy of the model object
-        """
-        self._copy = self.copy()
-        return self.copy()
-
-    def copy(self) -> LabelModel:
-        """Create a deepcopy of the model.
-
-        Returns
-        -------
-        model
-            Deepcopy of the model object
-        """
-        return copy.deepcopy(self)  # type: ignore
-
     @staticmethod
-    def _generate_binary_labels(*, base_name: str, num_labels: int) -> List[str]:
+    def _generate_binary_labels(base_name, num_labels):
         """Create binary label string.
 
+        Parameters
+        ----------
+        base_name : str
+        num_labels : int
+
         Returns
         -------
         isotopomers : list(str)
             Returns a list of all label isotopomers of the compound
 
         Examples
         --------
@@ -91,60 +70,50 @@
         >>> _generate_binary_labels(base_name='cpd', num_labels=1)
         ['cpd__0', 'cpd__1']
 
         >>> _generate_binary_labels(base_name='cpd', num_labels=2)
         ['cpd__00', 'cpd__01', 'cpd__10', 'cpd__11']
         """
         if num_labels > 0:
-            return [base_name + "__" + "".join(i) for i in it.product(("0", "1"), repeat=num_labels)]
-        return [base_name]
+            return [
+                base_name + "__" + "".join(i)
+                for i in it.product(("0", "1"), repeat=num_labels)
+            ]
+        else:
+            return [base_name]
 
-    def add_compound(  # type: ignore
-        self,
-        compound: str,
-        is_isotopomer: bool = False,
-        **meta_info: Dict[str, Any],
-    ) -> None:
+    def add_compound(self, compound, is_isotopomer=False, **meta_info):
         """Add a single compound to the model.
 
         Parameters
         ----------
-        compound
+        compound : str
             Name / id of the compound
-        is_isotopomer
+        is_isotopomer : bool
             Whether the compound is an isotopomer of a base compound
             or a non-label compound
-        meta_info
+        meta_info : dict, optional
             Meta info of the compound. Available keys are
             {common_name, compartment, formula, charge, gibbs0, smiles, database_links, notes}
         """
         super().add_compound(compound=compound, **meta_info)
         if not is_isotopomer:
             self.nonlabel_compounds.append(compound)
 
-    def _add_base_compound(
-        self,
-        *,
-        base_compound: str,
-        num_labels: int,
-        label_names: List[str],
-        **meta_info: Dict[str, Any],
-    ) -> None:
+    def _add_base_compound(self, base_compound, num_labels, label_names, **meta_info):
         """Add a base compound of label isotopomer."""
         self.label_compounds[base_compound] = {
             "num_labels": num_labels,
             "isotopomers": label_names,
         }
-        self._check_and_insert_ids([base_compound], context="base_compound")
         self.meta_info.setdefault("compounds", {}).setdefault(
-            base_compound,
-            Compound(**meta_info),  # type: ignore
+            base_compound, Compound(**meta_info)
         )
 
-    def _add_isotopomers(self, *, base_compound: str, label_names: List[str]) -> None:
+    def _add_isotopomers(self, base_compound, label_names):
         # Add all labelled compounds
         for compound in label_names:
             self.add_compound(compound=compound, is_isotopomer=True)
             del self.meta_info["compounds"][compound]
 
         # Create moiety for total compound concentration
         self.add_algebraic_module(
@@ -152,129 +121,170 @@
             function=total_concentration,
             compounds=label_names,
             derived_compounds=[base_compound + "__total"],
             modifiers=None,
             parameters=None,
         )
 
-    def add_label_compound(self, compound: str, num_labels: int, **meta_info: Dict[str, Any]) -> None:
+    def add_label_compound(self, compound, num_labels, **meta_info):
         """Create all label isotopomers and add them as compounds.
 
         Also create an algebraic module that tracks the total
         concentration of that compound
 
         Parameters
         ----------
-        base_compound
+        base_compound : str
             Base name of the compound
-        num_labels
+        num_labels : int
             Number of labels in the compound
 
         Warns
         -----
         UserWarning
             If compound is already in the model
         """
         if compound in self.label_compounds:
             warnings.warn(f"Overwriting compound {compound}")
             self.remove_label_compound(compound=compound)
         if num_labels == 0:
-            self.add_compound(
-                compound=compound,
-                is_isotopomer=False,
-                **meta_info,  # type: ignore
-            )
+            self.add_compound(compound=compound, is_isotopomer=False, **meta_info)
         else:
-            label_names = self._generate_binary_labels(base_name=compound, num_labels=num_labels)
+            label_names = self._generate_binary_labels(
+                base_name=compound, num_labels=num_labels
+            )
             self._add_base_compound(
                 base_compound=compound,
                 num_labels=num_labels,
                 label_names=label_names,
-                **meta_info,  # type: ignore
+                **meta_info,
             )
             self._add_isotopomers(base_compound=compound, label_names=label_names)
 
-    def add_label_compounds(
-        self,
-        compounds: Dict[str, int],
-        meta_info: Optional[Dict[str, Any]] = None,
-    ) -> None:
+    def add_label_compounds(self, compounds, meta_info=None):
         """Add multiple label-containing compounds to the model.
 
         Parameters
         ----------
-        compounds
-            {compound: num_labels}
+        compounds : dict(str, int)
+            {compound: num_labels} dictionary
 
         Examples
         --------
         >>> add_label_compounds({"GAP": 3, "DHAP": 3, "FBP": 6})
-
-        See Also
-        --------
-        add_label_compound
         """
         meta_info = {} if meta_info is None else meta_info
 
         for compound, num_labels in compounds.items():
-            info = meta_info.get(compound, {})
+            try:
+                info = meta_info[compound]
+            except KeyError:
+                info = {}
             self.add_label_compound(compound=compound, num_labels=num_labels, **info)
 
-    def remove_compound(self, compound: str, is_isotopomer: bool = False) -> None:
+    def remove_compound(self, compound, is_isotopomer=False):
         """Remove a compound from the model.
 
         Parameters
         ----------
-        compound
-        is_isotopomer
+        compound : str
+        is_isotopomer : bool
             Whether the compound is an isotopomer of a base compound
             or a non-label compound
         """
         super().remove_compound(compound=compound)
         if not is_isotopomer:
             self.nonlabel_compounds.remove(compound)
 
-    def remove_label_compound(self, compound: str) -> None:
-        """Remove a label compound from the model."""
+    def remove_label_compound(self, compound):
+        """Remove a label compound from the model.
+
+        Parameters
+        ----------
+        compound : str
+            Name of the compound
+        """
         label_compound = self.label_compounds.pop(compound)
-        self._remove_ids([compound])
         for key in label_compound["isotopomers"]:
             self.remove_compound(compound=key, is_isotopomer=True)
 
-    def remove_label_compounds(self, compounds: List[str]) -> None:
-        """Remove label compounds."""
+    def remove_label_compounds(self, compounds):
+        """Remove label compounds.
+
+        Parameters
+        ----------
+        compounds : iterable(str)
+            Names of the compounds
+        """
         for compound in compounds:
             self.remove_label_compound(compound=compound)
 
-    def get_base_compounds(self) -> List[str]:
-        """Get all base compounds and non-label compounds."""
+    def get_base_compounds(self):
+        """Get all base compounds and non-label compounds.
+
+        Returns
+        -------
+        base_compounds : list(str)
+        """
         return sorted(list(self.label_compounds) + self.nonlabel_compounds)
 
-    def get_compound_number_of_label_positions(self, compound: str) -> int:
-        """Get the number of possible labels positions of a compound."""
+    def get_compound_number_of_label_positions(self, compound):
+        """Get the number of possible labels positions of a compound.
+
+        Parameters
+        ----------
+        compound : str
+
+        Returns
+        -------
+        num_labels : int
+        """
         return int(self.label_compounds[compound]["num_labels"])
 
-    def get_compound_isotopomers(self, compound: str) -> List[str]:
-        """Get all isotopomers of a compound."""
+    def get_compound_isotopomers(self, compound):
+        """Get all isotopomers of a compound.
+
+        Parameters
+        ----------
+        compound : str
+
+        Returns
+        -------
+        isotopomers : list(str)
+        """
         return list(self.label_compounds[compound]["isotopomers"])
 
-    def get_compound_isotopomers_with_n_labels(self, compound: str, n_labels: int) -> List[str]:
-        """Get all isotopomers of a compound, that have excactly n labels."""
+    def get_compound_isotopomers_with_n_labels(self, compound, n_labels):
+        """Get all isotopomers of a compound, that have excactly n labels.
+
+        Parameters
+        ----------
+        compound : str
+
+        Returns
+        -------
+        isotopomers : list(str)
+        """
         label_positions = self.label_compounds[compound]["num_labels"]
         label_patterns = [
             ["1" if i in positions else "0" for i in range(label_positions)]
             for positions in it.combinations(range(label_positions), n_labels)
         ]
         return [f"{compound}__{''.join(i)}" for i in label_patterns]
 
     def get_compound_isotopomer_with_label_position(
-        self, base_compound: str, label_position: Union[int, List[int]]
-    ) -> str:
+        self, base_compound, label_position
+    ):
         """Get compound isotopomer with a given label position.
 
+        Parameters
+        ----------
+        base_compound : str
+        label_position : Union(int, iterable(int))
+
         Examples
         --------
         >>> add_label_compounds({"x": 2})
         >>> get_compound_isotopomer_with_label_position(x, 0) -> x__10
         >>> get_compound_isotopomer_with_label_position(x, [0]) -> x__10
         >>> get_compound_isotopomer_with_label_position(x, [0, 1]) -> x__11
         """
@@ -282,54 +292,65 @@
             label_position = [label_position]
         return f"{base_compound}__" + "".join(
             "1" if idx in label_position else "0"
             for idx in range(self.label_compounds[base_compound]["num_labels"])
         )
 
     @staticmethod
-    def _split_label_string(label: str, *, labels_per_compound: List[int]) -> List[str]:
+    def _split_label_string(label, labels_per_compound):
         """Split label string according to labels given in label list.
 
         The labels in the label list correspond to the number of
         label positions in the compound.
 
+        Parameters
+        ----------
+        labels : str
+        labels_per_compound : list(int)
+
         Examples
         --------
-        >>> _split_label_string(label="01", labels_per_compound=[2])
+        >>>_split_label_string(label="01", labels_per_compound=[2])
         ["01"]
 
-        >>> _split_label_string(label="01", labels_per_compound=[1, 1])
+        >>>_split_label_string(label="01", labels_per_compound=[1, 1])
         ["0", "1"]
 
-        >>> _split_label_string(label="0011", labels_per_compound=[4])
+        >>>_split_label_string(label="0011", labels_per_compound=[4])
         ["0011"]
 
-        >>> _split_label_string(label="0011", labels_per_compound=[3, 1])
+        >>>_split_label_string(label="0011", labels_per_compound=[3, 1])
         ["001", "1"]
 
-        >>> _split_label_string(label="0011", labels_per_compound=[2, 2])
+        >>>_split_label_string(label="0011", labels_per_compound=[2, 2])
         ["00", "11"]
 
-        >>> _split_label_string(label="0011", labels_per_compound=[1, 3])
+        >>>_split_label_string(label="0011", labels_per_compound=[1, 3])
         ["0", "011"]
         """
         split_labels = []
         cnt = 0
         for i in range(len(labels_per_compound)):
             split_labels.append(label[cnt : cnt + labels_per_compound[i]])
             cnt += labels_per_compound[i]
         return split_labels
 
     @staticmethod
-    def _map_substrates_to_products(*, rate_suffix: str, labelmap: List[int]) -> str:
-        """Map the rate_suffix to products using the labelmap."""
+    def _map_substrates_to_products(rate_suffix, labelmap):
+        """Map the rate_suffix to products using the labelmap.
+
+        Parameters
+        ----------
+        rate_suffix : str
+        labelmap : iterable(int)
+        """
         return "".join([rate_suffix[i] for i in labelmap])
 
     @staticmethod
-    def _unpack_stoichiometries(*, stoichiometries: Dict[str, int]) -> Tuple[List[str], List[str]]:
+    def _unpack_stoichiometries(stoichiometries):
         """Split stoichiometries into substrates and products.
 
         Parameters
         ----------
         stoichiometries : dict(str: int)
 
         Returns
@@ -342,215 +363,220 @@
         for k, v in stoichiometries.items():
             if v < 0:
                 substrates.extend([k] * -v)
             else:
                 products.extend([k] * v)
         return substrates, products
 
-    def _get_labels_per_compound(self, *, compounds: List[str]) -> List[int]:
+    def _get_labels_per_compound(self, compounds):
         """Get labels per compound.
 
         This is used for _split_label string. Adds 0 for non-label compounds,
-        to show that they get no label."""
+        to show that they get no label.
+
+        Parameters
+        ----------
+        compounds : list(str)
+
+        Returns
+        -------
+        label_per_compound : list(int)
+        """
         labels_per_compound = []
         for compound in compounds:
             try:
                 labels_per_compound.append(self.label_compounds[compound]["num_labels"])
-            except KeyError as e:
+            except KeyError:
                 if compound not in self.get_compounds():
-                    raise KeyError(f"Compound {compound} neither a compound nor a label compound") from e
+                    raise KeyError(
+                        f"Compound {compound} neither a compound nor a label compound"
+                    )
                 labels_per_compound.append(0)
         return labels_per_compound
 
     @staticmethod
-    def _repack_stoichiometries(*, new_substrates: List[str], new_products: List[str]) -> Dict[str, float]:
-        """Pack substrates and products into stoichiometric dict."""
-        new_stoichiometries: defaultdict[str, int] = defaultdict(int)
+    def _repack_stoichiometries(new_substrates, new_products):
+        """Pack substrates and products into stoichiometric dict.
+
+        Parameters
+        ----------
+        new_substrates : iterable(str)
+        new_products : iterable(str)
+
+        Returns
+        -------
+        stoichiometries : dict(str: int)
+        """
+        new_stoichiometries = _defaultdict(int)
         for arg in new_substrates:
             new_stoichiometries[arg] -= 1
         for arg in new_products:
             new_stoichiometries[arg] += 1
         return dict(new_stoichiometries)
 
     @staticmethod
-    def _assign_compound_labels(*, base_compounds: List[str], label_suffixes: List[str]) -> List[str]:
-        """Assign the correct suffixes."""
+    def _assign_compound_labels(base_compounds, label_suffixes):
+        """Assign the correct suffixes.
+
+        Parameters
+        ----------
+        base_compounds : iterable(str)
+        label_suffixes : iterable(str)
+
+        Returns
+        -------
+        new_compounds : list(str)
+        """
         new_compounds = []
         for i, compound in enumerate(base_compounds):
             if label_suffixes[i] != "":
                 new_compounds.append(compound + "__" + label_suffixes[i])
             else:
                 new_compounds.append(compound)
         return new_compounds
 
-    def add_algebraic_module(  # type: ignore
+    def add_algebraic_module(
         self,
-        module_name: str,
-        function: Callable,
-        compounds: List[str] | None = None,
-        derived_compounds: List[str] | None = None,
-        modifiers: List[str] | None = None,
-        parameters: List[str] | None = None,
-        args: List[str] | None = None,
+        module_name,
+        function,
+        compounds=None,
+        derived_compounds=None,
+        modifiers=None,
+        parameters=None,
     ):
         """Add an algebraic module to the model.
 
         CAUTION: The Python function of the module has to return an iterable.
         The Python function will get the function arguments in the following order:
         [**compounds, **modifiers, **parameters]
 
         CAUTION: In a LabelModel context compounds and modifiers will be mapped to
         __total if a label_compound without the isotopomer suffix is supplied.
 
         Parameters
         ----------
-        module_name
+        module_name : str
             Name of the module
-        function
+        function : callable
             Python method of the algebraic module
-        compounds
+        compounds : iterable(str)
             Names of compounds used for module
-        derived_compounds
+        derived_compounds : iterable(str)
             Names of compounds which are calculated by the module
-        modifiers
+        modifiers : iterable(str)
             Names of compounds which act as modifiers on the module
-        parameters
+        parameters : iterable(str)
             Names of the parameters which are passed to the function
-        meta_info
+        meta_info : dict, optional
             Meta info of the algebraic module. Allowed keys are
             {common_name, notes, database_links}
 
         Warns
         -----
         UserWarning
             If algebraic module is already in the model.
 
         Examples
         --------
-        >>> def rapid_equilibrium(substrate, k_eq)-> None:
-        >>>    x = substrate / (1 + k_eq)
-        >>>    y = substrate * k_eq / (1 + k_eq)
-        >>>    return x, y
-
-        >>> add_algebraic_module(
-        >>>     module_name="fast_eq",
-        >>>     function=rapid_equilibrium,
-        >>>     compounds=["A"],
-        >>>     derived_compounds=["X", "Y"],
-        >>>     parameters=["K"],
-        >>> )
+        def rapid_equilibrium(substrate, k_eq):
+            x = substrate / (1 + k_eq)
+            y = substrate * k_eq / (1 + k_eq)
+            return x, y
+
+        add_algebraic_module(
+            module_name="fast_eq",
+            function=rapid_equilibrium,
+            compounds=["A"],
+            derived_compounds=["X", "Y"],
+            parameters=["K"],
+        )
         """
         if compounds is not None:
-            compounds = [i + "__total" if i in self.label_compounds else i for i in compounds]
+            compounds = [
+                i + "__total" if i in self.label_compounds else i for i in compounds
+            ]
         if modifiers is not None:
-            modifiers = [i + "__total" if i in self.label_compounds else i for i in modifiers]
+            modifiers = [
+                i + "__total" if i in self.label_compounds else i for i in modifiers
+            ]
         super().add_algebraic_module(
             module_name=module_name,
             function=function,
             compounds=compounds,
             derived_compounds=derived_compounds,
             modifiers=modifiers,
             parameters=parameters,
-            args=args,
         )
 
     def _get_external_labels(
-        self,
-        *,
-        rate_name: str,
-        total_product_labels: int,
-        total_substrate_labels: int,
-        external_labels: Optional[List[int]],
-    ) -> str:
+        self, rate_name, total_product_labels, total_substrate_labels, external_labels
+    ):
         n_external_labels = total_product_labels - total_substrate_labels
         if n_external_labels > 0:
-            if external_labels is None:
+            if not external_labels:
                 warnings.warn(f"Added external labels for reaction {rate_name}")
                 external_label_string = ["1"] * n_external_labels
             else:
                 external_label_string = ["0"] * n_external_labels
                 for label_pos in external_labels:
                     external_label_string[label_pos] = "1"
-            return "".join(external_label_string)
-        return ""
+            external_labels = "".join(external_label_string)
+        else:
+            external_labels = ""
+        return external_labels
 
     def _add_base_reaction(
         self,
-        *,
-        rate_name: str,
-        function: Callable,
-        stoichiometry: Dict[str, int],
-        # base_substrates: List[str],
-        # base_products: List[str],
-        labelmap: List[int],
-        external_labels: Optional[str],
-        modifiers: Optional[List[str]],
-        parameters: Optional[List[str]],
-        reversible: bool,
-        # dynamic_variables: List[str] = None,
-        # args: List[str] = None,
-        variants: List[str],
-        **meta_info: Dict[str, Any],
-    ) -> None:
-        # The check isn't as easy.
-        # Don't compare to the compounds, probably against base compounds, non-isotopomers and derived compounds?
-        # if parameters is None:
-        #     parameters = []
-        # if modifiers is None:
-        #     modifiers = []
-        # if reversible:
-        #     dynamic_variables = base_substrates + base_products + modifiers
-        # else:
-        #     dynamic_variables = base_substrates + modifiers
-        # self._check_for_existence(
-        #     name=rate_name, check_against=self.get_all_compounds(), candidates=dynamic_variables
-        # )
-        # self._check_for_existence(
-        #     name=rate_name, check_against=self.get_parameter_names(), candidates=parameters
-        # )
+        rate_name,
+        function,
+        stoichiometry,
+        labelmap,
+        external_labels,
+        modifiers,
+        parameters,
+        reversible,
+        variants,
+        **meta_info,
+    ):
         self.base_reactions[rate_name] = {
             "function": function,
             "stoichiometry": stoichiometry,
             "labelmap": labelmap,
             "external_labels": external_labels,
             "modifiers": modifiers,
             "parameters": parameters,
             "reversible": reversible,
             "variants": variants,
         }
-        self.meta_info.setdefault("rates", {}).setdefault(
-            rate_name,
-            RateMeta(
-                **meta_info,  # type: ignore
-            ),
-        )
+        self.meta_info.setdefault("rates", {}).setdefault(rate_name, Rate(**meta_info))
 
     def _create_isotopomer_reactions(
         self,
-        *,
-        rate_name: str,
-        function: Callable,
-        labelmap: List[int],
-        modifiers: Optional[List[str]],
-        parameters: Optional[List[str]],
-        reversible: bool,
-        # dynamic_variables: List[str],
-        # args: List[str],
-        external_labels: str,
-        total_substrate_labels: int,
-        base_substrates: List[str],
-        base_products: List[str],
-        labels_per_substrate: List[int],
-        labels_per_product: List[int],
-    ) -> List[str]:
+        rate_name,
+        function,
+        labelmap,
+        modifiers,
+        parameters,
+        reversible,
+        external_labels,
+        total_substrate_labels,
+        base_substrates,
+        base_products,
+        labels_per_substrate,
+        labels_per_product,
+    ):
         variants = []
-        for rate_suffix in ("".join(i) for i in it.product(("0", "1"), repeat=total_substrate_labels)):
+        for rate_suffix in (
+            "".join(i) for i in it.product(("0", "1"), repeat=total_substrate_labels)
+        ):
             rate_suffix += external_labels
             # This is the magic
-            product_suffix = self._map_substrates_to_products(rate_suffix=rate_suffix, labelmap=labelmap)
+            product_suffix = self._map_substrates_to_products(
+                rate_suffix=rate_suffix, labelmap=labelmap
+            )
             product_labels = self._split_label_string(
                 label=product_suffix, labels_per_compound=labels_per_product
             )
             substrate_labels = self._split_label_string(
                 label=rate_suffix, labels_per_compound=labels_per_substrate
             )
 
@@ -567,57 +593,52 @@
             self.add_reaction(
                 rate_name=new_rate_name,
                 function=function,
                 stoichiometry=new_stoichiometry,
                 modifiers=modifiers,
                 parameters=parameters,
                 reversible=reversible,
-                # dynamic_variables=dynamic_variables,
-                # args=args,
-                check_consistency=False,
             )
             del self.meta_info["rates"][new_rate_name]
             variants.append(new_rate_name)
         return variants
 
     def add_labelmap_reaction(
         self,
-        rate_name: str,
-        function: Callable,
-        stoichiometry: Dict[str, int],
-        labelmap: List[int],
-        external_labels: Optional[List[int]] = None,
-        modifiers: Optional[List[str]] = None,
-        parameters: Optional[List[str]] = None,
-        reversible: bool = False,
-        # dynamic_variables: List[str] = None,
-        # args: List[str] = None,
-        **meta_info: Dict[str, Any],
-    ) -> None:
+        rate_name,
+        function,
+        stoichiometry,
+        labelmap,
+        external_labels=None,
+        modifiers=None,
+        parameters=None,
+        reversible=False,
+        **meta_info,
+    ):
         """Add a labelmap reaction.
 
         Parameters
         ----------
-        rate_name
+        rate_name : str
             Name of the rate function
-        function
+        function : callable
             Python method calculating the rate equation
-        stoichiometry
+        stoichiometry : dict(str: int)
             stoichiometry of the reaction
-        labelmap
+        labelmap : iterable(int)
             Mapping of the product label positions to the substrates
-        external_labels
+        external_labels: iterable(int)
             Positions in which external labels are supposed to be inserted
-        modifiers
+        modifiers: iterable(str)
             Names of the modifiers. E.g time.
-        parameters
+        parameters: iterable(str)
             Names of the parameters
-        reversible
+        reversible: bool
             Whether the reaction is reversible.
-        meta_info
+        meta_info : dict, optional
             Meta info of the rate. Allowed keys are
             {common_name, gibbs0, ec, database_links, notes, sbml_function}
 
         Examples
         --------
         >>> add_labelmap_reaction(
                 rate_name="triose-phosphate-isomerase",
@@ -633,242 +654,246 @@
                 labelmap=[0, 1, 2, 3, 4, 5],
                 stoichiometry={"DHAP": -1, "GAP": -1, "FBP": 1},
                 parameters=["kf_Ald", "kr_Ald"],
                 reversible=True,
             )
         """
         if modifiers is not None:
-            modifiers = [i + "__total" if i in self.label_compounds else i for i in modifiers]
+            modifiers = [
+                i + "__total" if i in self.label_compounds else i for i in modifiers
+            ]
 
-        base_substrates, base_products = self._unpack_stoichiometries(stoichiometries=stoichiometry)
+        base_substrates, base_products = self._unpack_stoichiometries(stoichiometry)
         labels_per_substrate = self._get_labels_per_compound(compounds=base_substrates)
         labels_per_product = self._get_labels_per_compound(compounds=base_products)
         total_substrate_labels = sum(labels_per_substrate)
         total_product_labels = sum(labels_per_product)
 
         if len(labelmap) - total_substrate_labels < 0:
-            raise ValueError(f"Labelmap 'missing' {abs(len(labelmap) - total_substrate_labels)} label(s)")
+            raise ValueError(
+                f"Labelmap 'missing' {abs(len(labelmap) - total_substrate_labels)} label(s)"
+            )
 
-        external_label_str = self._get_external_labels(
+        external_labels = self._get_external_labels(
             rate_name=rate_name,
             total_product_labels=total_product_labels,
             total_substrate_labels=total_substrate_labels,
             external_labels=external_labels,
         )
 
         variants = self._create_isotopomer_reactions(
             rate_name=rate_name,
             function=function,
             labelmap=labelmap,
             modifiers=modifiers,
             parameters=parameters,
             reversible=reversible,
-            # dynamic_variables=dynamic_variables,
-            # args=args,
-            external_labels=external_label_str,
+            external_labels=external_labels,
             total_substrate_labels=total_substrate_labels,
             base_substrates=base_substrates,
             base_products=base_products,
             labels_per_substrate=labels_per_substrate,
             labels_per_product=labels_per_product,
         )
 
         self._add_base_reaction(
             rate_name=rate_name,
             function=function,
-            # base_substrates=base_substrates,
-            # base_products=base_products,
             stoichiometry=stoichiometry,
             labelmap=labelmap,
-            external_labels=external_label_str,
+            external_labels=external_labels,
             modifiers=modifiers,
             parameters=parameters,
             reversible=reversible,
-            # dynamic_variables=dynamic_variables,
-            # args=args,
             variants=variants,
             **meta_info,
         )
 
     def update_labelmap_reaction(
         self,
-        rate_name: str,
-        function: Optional[Callable] = None,
-        stoichiometry: Optional[Dict[str, int]] = None,
-        labelmap: Optional[List[int]] = None,
-        modifiers: Optional[List[str]] = None,
-        parameters: Optional[List[str]] = None,
-        reversible: Optional[bool] = None,
-        # dynamic_variables: List[str] = None,
-        # args: List[str] = None,
-    ) -> None:
+        rate_name,
+        function=None,
+        stoichiometry=None,
+        labelmap=None,
+        modifiers=None,
+        parameters=None,
+        reversible=None,
+        **meta_info,
+    ):
         """Update an existing labelmap reaction.
 
         Parameters
         ----------
-        rate_name
+        rate_name : str
             Name of the rate function
-        function
+        function : callable, optional
             Python method calculating the rate equation
-        stoichiometry
+        stoichiometry : dict(str: int), optional
             stoichiometry of the reaction
-        labelmap
+        labelmap : iterable(int), optional
             Mapping of the product label positions to the substrates
-        external_labels
+        external_labels: iterable(int), optional
             Positions in which external labels are supposed to be inserted
-        modifiers
+        modifiers: iterable(str), optional
             Names of the modifiers. E.g time.
-        parameters
+        parameters: iterable(str), optional
             Names of the parameters
-        reversible
+        reversible: bool, optional
             Whether the reaction is reversible.
+        meta_info : dict, optional
+            Meta info of the rate. Allowed keys are
+            {common_name, gibbs0, ec, database_links, notes, sbml_function}
         """
         if function is None:
             function = self.base_reactions[rate_name]["function"]
         if stoichiometry is None:
             stoichiometry = self.base_reactions[rate_name]["stoichiometry"]
         if labelmap is None:
             labelmap = self.base_reactions[rate_name]["labelmap"]
         if modifiers is None:
             modifiers = self.base_reactions[rate_name]["modifiers"]
         if parameters is None:
             parameters = self.base_reactions[rate_name]["parameters"]
         if reversible is None:
             reversible = self.base_reactions[rate_name]["reversible"]
+        meta = self.meta_info["rates"][rate_name].__dict__
+        meta.update(meta_info)
 
         self.remove_labelmap_reaction(rate_name=rate_name)
         self.add_labelmap_reaction(
             rate_name=rate_name,
-            function=function,  # type: ignore
-            stoichiometry=stoichiometry,  # type: ignore
-            labelmap=labelmap,  # type: ignore
+            function=function,
+            stoichiometry=stoichiometry,
+            labelmap=labelmap,
             modifiers=modifiers,
             parameters=parameters,
-            reversible=reversible,  # type: ignore
-            # dynamic_variables=dynamic_variables,
-            # args=args,
+            reversible=reversible,
         )
 
-    def remove_labelmap_reaction(self, rate_name: str) -> None:
+    def remove_labelmap_reaction(self, rate_name):
         """Remove all variants of a base reaction.
 
         Parameters
         ----------
         rate_name : str
             Name of the rate
         """
         self.meta_info["rates"].pop(rate_name)
         base_reaction = self.base_reactions.pop(rate_name)
         for rate in base_reaction["variants"]:
             if rate.startswith(rate_name):
                 self.remove_reaction(rate_name=rate)
 
-    def remove_labelmap_reactions(self, rate_names: List[str]) -> None:
+    def remove_labelmap_reactions(self, rate_names):
         """Remove all variants of a multiple labelmap reactions.
 
         Parameters
         ----------
         rate_names : iterable(str)
 
         See Also
         --------
         remove_labelmap_reaction
         """
         for rate_name in rate_names:
             self.remove_labelmap_reaction(rate_name=rate_name)
 
-    def generate_y0(
-        self,
-        base_y0: Union[ArrayLike, Dict[str, float]],
-        label_positions: Dict[str, Union[int, List[int]]] | None = None,
-    ) -> Dict[str, float]:
+    # Simulation functions
+    def generate_y0(self, base_y0, label_positions=None):
         """Generate y0 for all isotopomers given a base y0.
 
+        Parameters
+        ----------
+        base_y0 : dict(str: num)
+        label_positions: dict(str: num)
+
+        Returns
+        -------
+        y0 : dict(str: num)
+
         Examples
         --------
         >>> base_y0 = {"GAP": 1, "DHAP": 0, "FBP": 0}
         >>> generate_y0(base_y0=base_y0, label_positions={"GAP": 0})
-        >>> generate_y0(base_y0=base_y0, label_positions={"GAP": [0, 1, 2]})
         """
         if label_positions is None:
             label_positions = {}
         if not isinstance(base_y0, dict):
             base_y0 = dict(zip(self.label_compounds, base_y0))
 
         y0 = dict(zip(self.get_compounds(), np.zeros(len(self.get_compounds()))))
         for base_compound, concentration in base_y0.items():
             label_position = label_positions.get(base_compound, None)
             if label_position is None:
                 try:
-                    y0[self.label_compounds[base_compound]["isotopomers"][0]] = concentration
+                    y0[
+                        self.label_compounds[base_compound]["isotopomers"][0]
+                    ] = concentration
                 except KeyError:  # non label compound
                     y0[base_compound] = concentration
             else:
                 if isinstance(label_position, int):
                     label_position = [label_position]
                 suffix = "__" + "".join(
                     "1" if idx in label_position else "0"
                     for idx in range(self.label_compounds[base_compound]["num_labels"])
                 )
                 y0[base_compound + suffix] = concentration
         return y0
 
-    def get_total_fluxes(
-        self,
-        rate_base_name: str,
-        y: Union[Dict[str, float], Dict[str, ArrayLike]],
-        t: Union[float, ArrayLike] = 0,
-    ) -> Array:
+    def get_total_fluxes(self, rate_base_name, y, t=0):
         """Get total fluxes of a base rate.
 
         Parameters
         ----------
         rate_base_name : str
         y : Union(iterable(num), dict(str: num))
         t : Union(num, iterable(num))
 
         Returns
         -------
         fluxes : numpy.array
         """
         rates = [i for i in self.rates if i.startswith(rate_base_name + "__")]
-        return cast(
-            Array,
-            self.get_fluxes_df(y=y, t=t)[rates].sum(axis=1).values,  # type: ignore
-        )
+        return self.get_fluxes_df(y=y, t=t)[rates].sum(axis=1).values
+
+    def _create_label_scope_seed(self, initial_labels):
+        """Create initial label scope seed.
+
+        Parameters
+        ----------
+        initial_labels : iterable(str)
 
-    def _create_label_scope_seed(
-        self, *, initial_labels: Union[Dict[str, int], Dict[str, List[int]]]
-    ) -> Dict[str, int]:
-        """Create initial label scope seed."""
+        Returns
+        -------
+        labelled_compounds : set(str)
+        """
+        initial_labels = [
+            self.get_compound_isotopomer_with_label_position(
+                base_compound=base_compound, label_position=label_position
+            )
+            for base_compound, label_position in initial_labels.items()
+        ]
 
         # initialise all compounds with 0 (no label)
         labelled_compounds = {compound: 0 for compound in self.get_compounds()}
 
         # Set all unlabelled compounds to 1
-        for name, compound in self.label_compounds.items():
-            num_labels = compound["num_labels"]
-            labelled_compounds[f"{name}__{'0' * num_labels}"] = 1
+        for compound, cpd_dict in self.label_compounds.items():
+            num_labels = cpd_dict["num_labels"]
+            labelled_compounds[f"{compound}__{'0' * num_labels}"] = 1
         # Also set all non-label compounds to 1
-        for name in self.nonlabel_compounds:
-            labelled_compounds[name] = 1
+        for compound in self.nonlabel_compounds:
+            labelled_compounds[compound] = 1
         # Set initial label
-        for i in [
-            self.get_compound_isotopomer_with_label_position(
-                base_compound=base_compound, label_position=label_position
-            )
-            for base_compound, label_position in initial_labels.items()
-        ]:
+        for i in initial_labels:
             labelled_compounds[i] = 1
         return labelled_compounds
 
-    def get_label_scope(
-        self,
-        initial_labels: Union[Dict[str, int], Dict[str, List[int]]],
-    ) -> Dict[int, set[str]]:
+    def get_label_scope(self, initial_labels):
         """Return all label positions that can be reached step by step.
 
         Parameters
         ----------
         initial_labels : dict(str: num)
 
         Returns
@@ -876,15 +901,17 @@
         label_scope : dict{step : set of new positions}
 
         Examples
         --------
         >>> l.get_label_scope({"x": 0})
         >>> l.get_label_scope({"x": [0, 1], "y": 0})
         """
-        labelled_compounds = self._create_label_scope_seed(initial_labels=initial_labels)
+        labelled_compounds = self._create_label_scope_seed(
+            initial_labels=initial_labels
+        )
         new_labels = set("non empty entry to not fulfill while condition")
         # Loop until no new labels are inserted
         loop_count = 0
         result = {}
         while new_labels != set():
             new_cpds = labelled_compounds.copy()
             for rec, cpd_dict in self.get_stoichiometries().items():
@@ -907,87 +934,83 @@
                         i += labelled_compounds[j]
                     # If all substrates are 1, set all products to 1
                     if i == len(cpds):
                         for cpd in self.get_stoichiometries()[rec]:
                             new_cpds[cpd] = 1
             # Isolate "old" labels
             s1 = pd.Series(labelled_compounds)
-            s1 = cast(pd.Series, s1[s1 == 1])
+            s1 = s1[s1 == 1]
             # Isolate new labels
             s2 = pd.Series(new_cpds)
-            s2 = cast(pd.Series, s2[s2 == 1])
+            s2 = s2[s2 == 1]
             # Find new labels
-            new_labels = cast(Set[str], set(s2.index).difference(set(s1.index)))
+            new_labels = set(s2.index).difference(set(s1.index))
             # Break the loop once no new labels can be found
             if new_labels == set():
                 break
-            labelled_compounds = new_cpds
-            result[loop_count] = new_labels
-            loop_count += 1
+            else:
+                labelled_compounds = new_cpds
+                result[loop_count] = new_labels
+                loop_count += 1
         return result
 
     ##########################################################################
     # Model conversion functions
     ##########################################################################
 
-    def _map_label_compound_to_compound(self, *, compound: str) -> str:
+    def _map_label_compound_to_compound(self, compound):
         if compound in self.nonlabel_compounds:
             return compound
-        return compound.rsplit("__")[0]
+        else:
+            return compound.rsplit("__")[0]
 
-    def to_model(self) -> Model:
+    def to_model(self):
         """Convert LabelModel to Model."""
         m = Model()
         m.add_parameters(self.parameters)
         m.add_compounds(list(self.label_compounds.keys()))
         m.add_compounds(self.nonlabel_compounds)
 
         for module_name, module in self.algebraic_modules.items():
             if not module_name.endswith("__total"):
-                module_ = dict(module)
-                module_["compounds"] = [
-                    self._map_label_compound_to_compound(compound=i) for i in module["compounds"]
+                module = module.copy()
+                module["compounds"] = [
+                    self._map_label_compound_to_compound(i) for i in module["compounds"]
                 ]
-                module_["derived_compounds"] = [
-                    self._map_label_compound_to_compound(compound=i) for i in module["derived_compounds"]
+                module["derived_compounds"] = [
+                    self._map_label_compound_to_compound(i)
+                    for i in module["derived_compounds"]
                 ]
-                module_["modifiers"] = [
-                    self._map_label_compound_to_compound(compound=i) for i in module["modifiers"]
+                module["modifiers"] = [
+                    self._map_label_compound_to_compound(i) for i in module["modifiers"]
                 ]
-                m.add_algebraic_module(module_name=module_name, **module_)
+                m.add_algebraic_module(module_name=module_name, **module)
 
         for rate_name, reaction in self.base_reactions.items():
             reaction = reaction.copy()
             reaction["stoichiometry"] = {
-                self._map_label_compound_to_compound(compound=k): v
+                self._map_label_compound_to_compound(k): v
                 for k, v in reaction["stoichiometry"].items()
             }
             reaction["modifiers"] = [
-                self._map_label_compound_to_compound(compound=i) for i in reaction["modifiers"]
+                self._map_label_compound_to_compound(i) for i in reaction["modifiers"]
             ]
             del reaction["labelmap"]
             del reaction["external_labels"]
             del reaction["variants"]
             m.add_reaction(rate_name=rate_name, **reaction)
         return m
 
     ##########################################################################
     # SBML functions
     ##########################################################################
 
     def _add_sbml_compound(
-        self,
-        *,
-        sbml_model: libsbml.Model,
-        compound_id: str,
-        common_name: str,
-        compartment: str,
-        charge: int,
-        formula: str,
-    ) -> None:
+        self, sbml_model, compound_id, common_name, compartment, charge, formula
+    ):
         cpd = sbml_model.createSpecies()
         cpd.setId(convert_id_to_sbml(id_=compound_id, prefix="CPD"))
         if common_name is not None:
             cpd.setName(common_name)
         cpd.setConstant(False)
         cpd.setBoundaryCondition(False)
         cpd.setHasOnlySubstanceUnits(False)
@@ -995,15 +1018,15 @@
 
         cpd_fbc = cpd.getPlugin("fbc")
         if charge is not None:
             cpd_fbc.setCharge(int(charge))
         if formula is not None:
             cpd_fbc.setChemicalFormula(formula)
 
-    def _create_sbml_compounds(self, *, sbml_model: libsbml.Model) -> None:
+    def _create_sbml_compounds(self, sbml_model):
         """Create the compounds for the sbml model.
 
         Parameters
         ----------
         sbml_model : libsbml.Model
         """
         for base_compound_id, base_compound in self.label_compounds.items():
@@ -1034,15 +1057,15 @@
                 compound_id=compound_id,
                 common_name=common_name,
                 compartment=compartment,
                 charge=charge,
                 formula=formula,
             )
 
-    def _create_sbml_reactions(self, *, sbml_model: libsbml.Model) -> None:
+    def _create_sbml_reactions(self, sbml_model):
         """Create the reactions for the sbml model.
 
         Parameters
         ----------
         sbml_model : libsbml.Model
         """
         for base_rate_id, base_rate in self.base_reactions.items():
```

### Comparing `modelbase-1.9.3/src/modelbase/ode/models/linearlabelmodel.py` & `modelbase-1rc2/modelbase/ode/models/linearlabelmodel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,404 +1,359 @@
-from __future__ import annotations
+"""LinearLabelModel base class."""
 
-__all__ = [
-    "LinearRate",
-    "LinearLabelModel",
-]
-
-import copy
 import warnings
-from typing import Any, Dict, Iterable, List, Tuple, Union, cast
-
-import libsbml
 import numpy as np
 import pandas as pd
+import libsbml
 
-from ...core import BaseModel, CompoundMixin, StoichiometricMixin
-from ...core.ratemixin import RateMeta
+from ...core import BaseModel, CompoundMixin, RateMixin, StoichiometricMixin
+from ...core.ratemixin import Rate
 from ...core.utils import convert_id_to_sbml
-from ...typing import Array, ArrayLike
-from . import _AbstractStoichiometricModel
 
 
-def relative_label_flux(substrate: float, v_ss: float) -> float:
+def relative_label_flux(substrate, v_ss):
     """Calculate relative label flux."""
     return v_ss * substrate
 
 
-class LinearRate:
-    def __init__(
-        self,
-        base_name: str,
-        substrate: str,
-    ):
-        self.base_name = base_name
-        self.substrate = substrate
-        self._y_ss = None
-        self._v_ss = None
-        self._external_label = None
-
-    def __repr__(self) -> str:
-        return repr(self.__dict__)
-
-    def __str__(self) -> str:
-        return f"LinearRate(base_name={self.base_name}, substrate={self.substrate}"
-
-    def keys(self) -> List[str]:
-        return [
-            "base_name",
-            "substrate",
-        ]
-
-    def __getitem__(self, key: str) -> Any:
-        return self.__dict__[key]
-
-
-class LinearLabelModel(_AbstractStoichiometricModel):
+class LinearLabelModel(RateMixin, StoichiometricMixin, CompoundMixin, BaseModel):
     """LinearLabelModel."""
 
     def __init__(
-        self,
-        compounds: List[str] | None = None,
-        rate_stoichiometries: dict[str, dict[str, float]] | None = None,
-        rates: dict | None = None,
-        meta_info: dict | None = None,
+        self, compounds=None, rate_stoichiometries=None, rates=None, meta_info=None
     ):
-        self.isotopomers: Dict[str, List[str]] = {}
-        self.base_rates: Dict[str, set[str]] = {}
-        self.rates: Dict[str, LinearRate] = {}
+        self.isotopomers = {}
+        self.base_rates = {}
         BaseModel.__init__(self, meta_info=meta_info)
         CompoundMixin.__init__(self, compounds=compounds)
         StoichiometricMixin.__init__(self, rate_stoichiometries=rate_stoichiometries)
+        RateMixin.__init__(self, rates=rates)
         self.meta_info["model"].sbo = "SBO:0000062"  # continuous framework
 
-        if rates is not None:
-            for k, v in rates.items():
-                self.add_rate(rate_name=k, **v)
-
-    def __enter__(self) -> LinearLabelModel:
-        """Enter the context manager.
-
-        Returns
-        -------
-            Deepcopy of the model object
-        """
-        self._copy = self.copy()
-        return self.copy()
+    @staticmethod
+    def _generate_isotope_labels(base_name, num_labels):
+        """Create binary label string.
 
-    def copy(self) -> LinearLabelModel:
-        """Create a deepcopy of the model.
+        Parameters
+        ----------
+        base_name : str
+        num_labels : int
 
         Returns
         -------
-        model
-            Deepcopy of the model object
+        isotopomers : list(str)
+            Returns a list of all label isotopomers of the compound
         """
-        return copy.deepcopy(self)  # type: ignore
-
-    @staticmethod
-    def _generate_isotope_labels(*, base_name: str, num_labels: int) -> List[str]:
-        """Returns a list of all label isotopomers of the compound."""
         if num_labels > 0:
             return [f"{base_name}__{i}" for i in range(num_labels)]
-        raise ValueError(f"Compound {base_name} must have labels")
+        else:
+            raise ValueError(f"Compound {base_name} must have labels")
 
-    def add_compound(self, compound: str, num_labels: int) -> None:  # type: ignore
+    def add_compound(self, compound, num_labels):
         """Add a label-containing compound to the model."""
         if compound in self.isotopomers:
             self.remove_compound(compound=compound)
             warnings.warn(f"Overwriting compound {compound}")
 
-        label_names = self._generate_isotope_labels(base_name=compound, num_labels=num_labels)
+        label_names = self._generate_isotope_labels(
+            base_name=compound, num_labels=num_labels
+        )
         self.isotopomers[compound] = label_names
-        self._check_and_insert_ids([compound], context="add_compound")
 
         # Add all labelled compounds
         for isotopomer in label_names:
             super().add_compound(compound=isotopomer)
 
-    def add_compounds(self, compounds: Dict[str, int]) -> None:  # type: ignore
+    def add_compounds(self, compounds):
         """Add multiple label-containing compounds to the model.
 
         Parameters
         ----------
-        compounds
-            {compound_name: num_labels}
+        compounds : dict(str, int)
+            {compound: num_labels} dictionary
         """
         for compound, num_labels in compounds.items():
             self.add_compound(compound=compound, num_labels=num_labels)
 
-    def remove_compound(self, compound: str) -> None:
-        """Remove a compound from the model."""
+    def remove_compound(self, compound):
+        """Remove a compound from the model.
+
+        Parameters
+        ----------
+        compound : str
+        """
         isotopomers = self.isotopomers.pop(compound)
         for i in isotopomers:
-            super().remove_compound(i)
-        self._remove_ids([compound])
+            self.compounds.remove(i)
 
-    def add_rate(self, rate_name: str, base_name: str, substrate: str, **meta_info) -> None:  # type: ignore
+    def add_rate(self, rate_name, base_name, substrate, **meta_info):
         """Add a rate function to the model.
 
+        The Python function will get the function arguments in the following order:
+        [**substrates, **(products if reversible), **modifiers, **parameters.]
+
         Parameters
         ----------
-        rate_name
+        rate_name : str
             Name of the rate function plus suffixes
-        base_name
+        base_name : str
             Name of the rate function
-        substrate
+        substrate: str
             Name of the substrate
         meta_info : dict, optional
             Meta info of the rate. Allowed keys are
             {common_name, gibbs0, ec, database_links, notes, sbml_function}
 
         Warns
         -----
         UserWarning
             If rate is already in the model
         """
         if rate_name in self.rates:
             warnings.warn(f"Overwriting rate {rate_name}", UserWarning)
             self.remove_rate(rate_name=rate_name)
 
-        self.rates[rate_name] = LinearRate(
-            base_name=base_name,
-            substrate=substrate,
-        )
+        self.rates[rate_name] = {
+            "base_name": base_name,
+            "substrate": substrate,
+        }
         self.base_rates.setdefault(base_name, set()).add(rate_name)
-        self.meta_info.setdefault("rates", {}).setdefault(rate_name, RateMeta(**meta_info))
+        self.meta_info.setdefault("rates", {}).setdefault(rate_name, Rate(**meta_info))
 
-    def remove_rate(self, rate_name: str) -> None:
-        del self.rates[rate_name]
+    @staticmethod
+    def _unpack_stoichiometries(stoichiometries):
+        """Split stoichiometries into substrates and products.
 
-    def get_rate_names(self) -> List[str]:
-        return list(self.rates.keys())
+        Parameters
+        ----------
+        stoichiometries : dict(str: int)
 
-    @staticmethod
-    def _unpack_stoichiometries(*, stoichiometries: Dict[str, int]) -> Tuple[List[str], List[str]]:
-        """Split stoichiometries into substrates and products."""
+        Returns
+        -------
+        substrates : list(str)
+        products : list(str)
+        """
         substrates = []
         products = []
         for k, v in stoichiometries.items():
             if v < 0:
                 substrates.extend([k] * -v)
             else:
                 products.extend([k] * v)
         return substrates, products
 
     @staticmethod
-    def _add_label_influx_or_efflux(
-        *,
-        rate_name: str,
-        substrates: List[str],
-        products: List[str],
-        labelmap: List[int],
-    ) -> None:
+    def _add_label_influx_or_efflux(rate_name, substrates, products, labelmap):
         # Label outfluxes
         diff = len(substrates) - len(products)
         for _ in range(diff):
             products.append("EXT")
 
         # Label influxes
         diff = len(labelmap) - len(substrates)
         if diff < 0:
             raise ValueError(f"Labelmap 'missing' {abs(diff)} label(s)")
-        warnings.warn(f"Added external label influx for reaction {rate_name}")
-        for _ in range(diff):
-            substrates.append("EXT")
+        elif diff > 0:
+            warnings.warn(f"Added external label influx for reaction {rate_name}")
+            for _ in range(diff):
+                substrates.append("EXT")
 
     @staticmethod
-    def _map_substrates_to_labelmap(*, substrates: List[str], labelmap: List[int]) -> List[str]:
+    def _map_substrates_to_labelmap(substrates, labelmap):
         return [substrates[i] for i in labelmap]
 
-    def add_reaction(self, rate_name: str, stoichiometry: Dict[str, int], labelmap: List[int]) -> None:
+    def add_reaction(self, rate_name, stoichiometry, labelmap):
         """Add a reaction to the model.
 
-        Examples
-        --------
-        >>> add_reaction(rate_name="v1", stoichiometry={"x": -1, "y": 1}, labelmap=[0, 1])
+        Parameters
+        ----------
+        rate_name : str
+        stoichiometry : dict
+        labelmap : iterable(int)
         """
         if rate_name in self.base_rates:
             warnings.warn(f"Overwriting reaction {rate_name}")
             self.remove_reaction(rate_name=rate_name)
 
-        base_substrates, base_products = self._unpack_stoichiometries(stoichiometries=stoichiometry)
+        base_substrates, base_products = self._unpack_stoichiometries(stoichiometry)
         substrates = [j for i in base_substrates for j in self.isotopomers[i]]
         products = [j for i in base_products for j in self.isotopomers[i]]
 
         self._add_label_influx_or_efflux(
             rate_name=rate_name,
             substrates=substrates,
             products=products,
             labelmap=labelmap,
         )
-        substrates = self._map_substrates_to_labelmap(substrates=substrates, labelmap=labelmap)
+        substrates = self._map_substrates_to_labelmap(
+            substrates=substrates, labelmap=labelmap
+        )
 
         for i, (substrate, product) in enumerate(zip(substrates, products)):
-            self.add_stoichiometry(rate_name=f"{rate_name}__{i}", stoichiometry={substrate: -1, product: 1})
+            self.add_stoichiometry(
+                rate_name=f"{rate_name}__{i}", stoichiometry={substrate: -1, product: 1}
+            )
             self.add_rate(
                 rate_name=f"{rate_name}__{i}",
                 base_name=rate_name,
                 substrate=substrate,
                 **{"sbml_function": f"{rate_name} * {substrate}"},
             )
 
-    def remove_reaction(self, rate_name: str) -> None:
+    def remove_reaction(self, rate_name):
         """Remove a reaction from the model.
 
         Parameters
         ----------
         rate_name : str
         """
         for rate in self.base_rates[rate_name]:
             self.remove_rate(rate_name=rate)
             self.remove_rate_stoichiometry(rate_name=rate)
-        del self.base_rates[rate_name]
 
-    def generate_y0(
-        self, initial_labels: Union[Dict[str, int], Dict[str, List[int]]] | None = None
-    ) -> Dict[str, float]:
+    def generate_y0(self, initial_labels=None):
         """Generate y0 for all isotopomers.
 
+        Parameters
+        ----------
+        initial_labels : dict(str: num)
+
+        Returns
+        -------
+        y0 : dict(str: num)
+
         Examples
         --------
         >>> generate_y0()
         >>> generate_y0(initial_labels={"x": 0})
         >>> generate_y0(initial_labels={"x": [0, 1]})
         """
-        y0 = {k: 0.0 for k in self.get_compounds()}
+        y0 = {k: 0 for k in self.get_compounds()}
         if initial_labels is not None:
             for base_compound, label_positions in initial_labels.items():
                 if isinstance(label_positions, int):
                     label_positions = [label_positions]
                 for pos in label_positions:
                     y0[f"{base_compound}__{pos}"] = 1 / len(label_positions)
         return y0
 
-    def _get_fluxes(  # type: ignore
-        self,
-        *,
-        fcd: Dict[str, float],
-        v_ss: Dict[str, float],
-        external_label: float = 1.0,
-    ) -> Dict[str, float]:
-        fcd["EXT"] = external_label
+    def _get_fluxes(self, y, v_ss, external_label=1):
+        y["EXT"] = external_label
+
         fluxes = {}
         for name, rate in self.rates.items():
-            fluxes[name] = relative_label_flux(fcd[rate["substrate"]], v_ss[rate["base_name"]])
+            fluxes[name] = relative_label_flux(
+                y[rate["substrate"]], v_ss[rate["base_name"]]
+            )
         return fluxes
 
-    def get_fluxes_dict(
-        self,
-        y: Union[Iterable[float], Dict[str, float]],
-        v_ss: Dict[str, float],
-        external_label: float = 1.0,
-    ) -> Dict[str, float]:
-        """Calculate the fluxes at time point(s) t."""
+    def get_fluxes_dict(self, y, v_ss, external_label=1, t=0):
+        """Calculate the fluxes at time point(s) t.
+
+        Parameters
+        ----------
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num))
+
+        Returns
+        -------
+        fluxes : dict
+        """
         if not isinstance(y, dict):
             y = dict(zip(self.compounds, y))
-        return self._get_fluxes(
-            fcd=y,  # type: ignore
-            v_ss=v_ss,
-            external_label=external_label,
-        )
+        return self._get_fluxes(y=y, v_ss=v_ss, external_label=external_label)
+
+    def get_fluxes_array(self, y, v_ss, external_label=1, t=0):
+        """Calculate the fluxes at time point(s) t.
 
-    def get_fluxes_array(
-        self,
-        y: Dict[str, float],
-        v_ss: Dict[str, float],
-        external_label: float = 1.0,
-    ) -> Array:
-        """Calculate the fluxes at time point(s) t."""
+        Parameters
+        ----------
+        y : Union(dict(str: num), iterable(num))
+        t : Union(num, iterable(num))
+
+        Returns
+        -------
+        fluxes : numpy.array
+        """
         return np.array(
-            list(
-                self.get_fluxes_dict(
-                    y=y,
-                    v_ss=v_ss,
-                    external_label=external_label,
+            [
+                i
+                for i in self.get_fluxes_dict(
+                    y=y, v_ss=v_ss, external_label=external_label
                 ).values()
-            )
+            ]
         ).T
 
-    def get_fluxes_df(
-        self,
-        y: Dict[str, float],
-        v_ss: Dict[str, float],
-        external_label: float = 1.0,
-        t: float = 0.0,
-    ) -> pd.DataFrame:
+    def get_fluxes_df(self, y, v_ss, external_label=1, t=0):
         """Calculate the fluxest.
 
         Parameters
         ----------
         y : Union(dict(str: num), iterable(num))
         t : Union(num, iterable(num))
 
         Returns
         -------
         fluxes : pandas.DataFrame
         """
         if isinstance(t, (int, float)):
-            t_array = [t]
-        else:
-            t_array = t
+            t = [t]
         return pd.DataFrame(
-            data=self.get_fluxes_dict(y=y, v_ss=v_ss, external_label=external_label),
-            index=t_array,
+            data=self.get_fluxes_dict(
+                y=y, v_ss=v_ss, external_label=external_label, t=t
+            ),
+            index=t,
             columns=self.get_rate_names(),
         )
 
-    # This can't get keyword-only arguments, as the integrators are calling it with
-    # positional arguments
-    def _get_rhs(self, _t: float, y_labels: ArrayLike) -> ArrayLike:  # type: ignore[override]
-        fcd = dict(zip(self.compounds, y_labels))
-        dxdt: Dict[str, float] = {i: 0.0 for i in self.compounds}
+    def _get_rhs(self, t, y_labels):
+        y_labels = dict(zip(self.compounds, y_labels))
+        dxdt = {i: 0 for i in y_labels}
 
-        fluxes = self._get_fluxes(fcd=fcd, v_ss=self._v_ss, external_label=self._external_label)
+        fluxes = self._get_fluxes(
+            y=y_labels, v_ss=self._v_ss, external_label=self._external_label
+        )
         for compound, isotopomers in self.isotopomers.items():
             for isotomoper in isotopomers:
-                for rate, stoich in self.stoichiometries_by_compounds[isotomoper].items():
+                for rate, stoich in self.stoichiometries_by_compounds[
+                    isotomoper
+                ].items():
                     dxdt[isotomoper] += stoich * fluxes[rate] / self._y_ss[compound]
         return list(dxdt.values())
 
-    def get_right_hand_side(
-        self,
-        y_labels: Union[ArrayLike, Dict[str, float]],
-        y_ss: Dict[str, float],
-        v_ss: Dict[str, float],
-        external_label: float = 1.0,
-        t: float = 0.0,
-    ) -> Dict[str, float]:
+    def get_right_hand_side(self, y_labels, y_ss, v_ss, external_label=1, t=0):
         """Calculate the right hand side of the ODE system.
 
         Parameters
         ----------
-        y_labels
+        y_labels : dict
             Relative concentrations of the label positions
-        y_ss
+        y_ss : dict
             Steady-state concentrations of the base compounds
             obtained from the non-labelled model
-        v_ss
+        v_ss : dict
             Steady-state fluxes of the base reactions
             obtained from the non-labelled model
-        external_label
+        external_label : num
             Relative concentration of an external label pool
-        t
+        t : num
             Time
         """
         self._y_ss = y_ss
         self._v_ss = v_ss
         self._external_label = external_label
         if isinstance(y_labels, dict):
-            y_labels = cast(ArrayLike, [y_labels[i] for i in self.compounds])
-        return dict(zip(self.compounds, self._get_rhs(_t=t, y_labels=y_labels)))
+            y_labels = [y_labels[i] for i in self.compounds]
+        return dict(zip(self.compounds, self._get_rhs(t=0, y_labels=y_labels)))
 
     ##########################################################################
     # SBML functions
     ##########################################################################
 
-    def _create_sbml_reactions(self, *, sbml_model: libsbml.Model) -> None:
+    def _create_sbml_reactions(self, sbml_model):
         """Create the reactions for the sbml model.
 
         Parameters
         ----------
         sbml_model : libsbml.Model
         """
         for rate_id, stoichiometry in self.stoichiometries.items():
@@ -417,15 +372,15 @@
                 sref.setSpecies(convert_id_to_sbml(id_=compound_id, prefix="CPD"))
                 sref.setStoichiometry(abs(factor))
                 sref.setConstant(False)
 
             kinetic_law = rxn.createKineticLaw()
             kinetic_law.setMath(libsbml.parseL3Formula(rate.sbml_function))
 
-    def _model_to_sbml(self) -> libsbml.SBMLDocument:
+    def _model_to_sbml(self):
         """Export model to sbml."""
         doc = self._create_sbml_document()
         sbml_model = self._create_sbml_model(doc=doc)
         self._create_sbml_units(sbml_model=sbml_model)
         self._create_sbml_compartments(sbml_model=sbml_model)
         self._create_sbml_compounds(sbml_model=sbml_model)
         self._create_sbml_reactions(sbml_model=sbml_model)
```

### Comparing `modelbase-1.9.3/src/modelbase/ode/utils/ratelaws.py` & `modelbase-1rc2/modelbase/ode/utils/ratelaws.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,149 @@
-from __future__ import annotations
-
-__all__ = [
-    "BaseRateLaw",
-    "Constant",
-    "MassAction",
-    "ReversibleMassAction",
-    "MichaelisMenten",
-    "ReversibleMichaelisMenten",
-    "ReversibleMichaelisMentenKeq",
-]
-
 from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import Callable, Dict, List, Union
 
 from . import ratefunctions
 
 
-def _pack_stoichiometries(substrates: List[str], products: List[str]) -> Dict[str, int]:
-    new_stoichiometries: defaultdict[str, int] = defaultdict(int)
+def _pack_stoichiometries(substrates, products):
+    new_stoichiometries = defaultdict(int)
     for arg in substrates:
         new_stoichiometries[arg] -= 1
     for arg in products:
         new_stoichiometries[arg] += 1
     return dict(new_stoichiometries)
 
 
 class BaseRateLaw(ABC):
-    def __init__(self) -> None:
-        self.substrates: List[str] = []
-        self.products: List[str] = []
-        self.modifiers: List[str] = []
-        self.parameters: List[str] = []
-        self.stoichiometry: Dict[str, int] = {}
-        self.reversible: bool = False
+    def __init__(self):
+        self.substrates = []
+        self.products = []
+        self.modifiers = []
+        self.parameters = []
+        self.stoichiometry = {}
+        self.reversible = False
 
     @abstractmethod
-    def get_sbml_function_string(self) -> str:
-        ...
+    def get_sbml_function_string(self):
+        """Write me."""
 
     @abstractmethod
-    def get_rate_function(self) -> Callable:
-        ...
+    def get_rate_function(self):
+        """Write me."""
 
 
 class Constant(BaseRateLaw):
-    def __init__(self, product: str, k: str) -> None:
+    def __init__(self, product, k):
         super().__init__()
         self.products = [product]
         self.parameters = [k]
         self.stoichiometry = {product: 1}
+
         self.k = k
 
-    def get_sbml_function_string(self) -> str:
+    def get_sbml_function_string(self):
         return f"{self.k}"
 
-    def get_rate_function(self) -> Callable:
+    def get_rate_function(self):
         return ratefunctions.constant
 
 
 class MassAction(BaseRateLaw):
-    def __init__(
-        self,
-        substrates: Union[str, List[str]],
-        products: Union[str, List[str]],
-        k_fwd: str,
-    ):
+    def __init__(self, substrates, products, k_fwd):
+
         super().__init__()
-        self.substrates: List[str] = list(substrates) if not isinstance(substrates, str) else [substrates]
-        self.products: List[str] = list(products) if not isinstance(products, str) else [products]
+        self.substrates = (
+            list(substrates) if not isinstance(substrates, str) else [substrates]
+        )
+        self.products = list(products) if not isinstance(products, str) else [products]
         self.parameters = [k_fwd]
-        self.stoichiometry = _pack_stoichiometries(self.substrates, self.products)
+        self.stoichiometry = _pack_stoichiometries(substrates, products)
+
         self.k_fwd = k_fwd
 
-    def get_sbml_function_string(self) -> str:
+    def get_sbml_function_string(self):
         return f"{self.k_fwd} * {' * '.join(self.substrates)}"
 
-    def get_rate_function(self) -> Callable:
-        try:
-            function: Callable = getattr(ratefunctions, f"mass_action_{len(self.substrates)}")
-            return function
-        except AttributeError:
-            return ratefunctions.mass_action_variable
+    def get_rate_function(self):
+        return getattr(ratefunctions, f"mass_action_{len(self.substrates)}")
 
 
 class ReversibleMassAction(BaseRateLaw):
-    def __init__(
-        self,
-        substrates: Union[str, List[str]],
-        products: Union[str, List[str]],
-        k_fwd: str,
-        k_bwd: str,
-    ):
+    def __init__(self, substrates, products, k_fwd, k_bwd):
         super().__init__()
-        self.substrates: List[str] = list(substrates) if not isinstance(substrates, str) else [substrates]
-        self.products: List[str] = list(products) if not isinstance(products, str) else [products]
+        self.substrates = (
+            list(substrates) if not isinstance(substrates, str) else [substrates]
+        )
+        self.products = list(products) if not isinstance(products, str) else [products]
         self.parameters = [k_fwd, k_bwd]
-        self.stoichiometry = _pack_stoichiometries(self.substrates, self.products)
+        self.stoichiometry = _pack_stoichiometries(substrates, products)
         self.reversible = True
 
         self.k_fwd = k_fwd
         self.k_bwd = k_bwd
 
-    def get_sbml_function_string(self) -> str:
+    def get_sbml_function_string(self):
         return f"{self.k_fwd} * {' * '.join(self.substrates)} - {self.k_bwd} * {' * '.join(self.products)}"
 
-    def get_rate_function(self) -> Callable:
-        try:
-            function: Callable = getattr(
-                ratefunctions,
-                f"reversible_mass_action_{len(self.substrates)}_{len(self.products)}",
-            )
-        except AttributeError:
-            function = getattr(
-                ratefunctions,
-                f"reversible_mass_action_variable_{len(self.substrates)}",
-            )
-        return function
+    def get_rate_function(self):
+        return getattr(
+            ratefunctions,
+            f"reversible_mass_action_{len(self.substrates)}_{len(self.products)}",
+        )
 
 
 class MichaelisMenten(BaseRateLaw):
-    def __init__(self, S: str, P: str, vmax: str, km: str) -> None:
+    def __init__(self, S, P, vmax, km):
+
         super().__init__()
         self.substrates = [S]
         self.products = [P]
         self.parameters = [vmax, km]
         self.stoichiometry = {S: -1, P: 1}
 
         self.S = S
         self.vmax = vmax
         self.km = km
 
-    def get_sbml_function_string(self) -> str:
+    def get_sbml_function_string(self):
         return f"{self.S} * {self.vmax} / ({self.S} + {self.km})"
 
-    def get_rate_function(self) -> Callable:
+    def get_rate_function(self):
         return ratefunctions.michaelis_menten
 
 
 class ReversibleMichaelisMenten(BaseRateLaw):
-    def __init__(self, S: str, P: str, vmax_fwd: str, vmax_bwd: str, km_fwd: str, km_bwd: str) -> None:
+    def __init__(self, S, P, vmax_fwd, vmax_bwd, km_fwd, km_bwd):
         super().__init__()
         self.substrates = [S]
         self.products = [P]
         self.parameters = [vmax_fwd, vmax_bwd, km_fwd, km_bwd]
         self.stoichiometry = {S: -1, P: 1}
         self.reversible = True
 
         self.S = S
         self.P = P
         self.vmax_fwd = vmax_fwd
         self.vmax_bwd = vmax_bwd
         self.km_fwd = km_fwd
         self.km_bwd = km_bwd
 
-    def get_sbml_function_string(self) -> str:
+    def get_sbml_function_string(self):
         return (
             f"({self.vmax_fwd} * {self.S} / {self.km_fwd} - {self.vmax_bwd} * {self.P} / {self.km_bwd})"
             + f" / (1 + {self.S} / {self.km_fwd} + {self.P} / {self.km_bwd})"
         )
 
-    def get_rate_function(self) -> Callable:
+    def get_rate_function(self):
         return ratefunctions.reversible_michaelis_menten
 
 
 class ReversibleMichaelisMentenKeq(BaseRateLaw):
-    def __init__(self, S: str, P: str, vmax_fwd: str, km_fwd: str, km_bwd: str, k_eq: str) -> None:
+    def __init__(self, S, P, vmax_fwd, km_fwd, km_bwd, k_eq):
+
         super().__init__()
         self.substrates = [S]
         self.products = [P]
         self.parameters = [vmax_fwd, km_fwd, km_bwd, k_eq]
         self.stoichiometry = {S: -1, P: 1}
         self.reversible = True
 
@@ -177,15 +151,15 @@
         self.P = P
 
         self.vmax_fwd = vmax_fwd
         self.km_fwd = km_fwd
         self.km_bwd = km_bwd
         self.k_eq = k_eq
 
-    def get_sbml_function_string(self) -> str:
+    def get_sbml_function_string(self):
         return (
             f"{self.vmax_fwd} / {self.km_fwd} * ({self.S} - {self.P} / {self.k_eq})"
             + f"/ (1 + {self.S} / {self.km_fwd} + {self.P} / {self.km_bwd})"
         )
 
-    def get_rate_function(self) -> Callable:
+    def get_rate_function(self):
         return ratefunctions.reversible_michaelis_menten_keq
```

