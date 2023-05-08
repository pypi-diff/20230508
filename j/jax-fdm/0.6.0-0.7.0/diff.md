# Comparing `tmp/jax_fdm-0.6.0.tar.gz` & `tmp/jax_fdm-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_fdm-0.6.0.tar", last modified: Mon May  1 02:02:22 2023, max compression
+gzip compressed data, was "jax_fdm-0.7.0.tar", last modified: Mon May  8 19:33:51 2023, max compression
```

## Comparing `jax_fdm-0.6.0.tar` & `jax_fdm-0.7.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.562691 jax_fdm-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/length.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/network/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/force.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/length.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/node/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/curvature.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/fdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/abstract_goal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/network/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/network/loadpath.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/node/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/line.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/second_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/recorders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/visualization/artists/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/artists/network_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/loss_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.725377 jax_fdm-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/length.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/datastructures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/fdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/abstract_goal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/network/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/second_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/recorders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/artists/network_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/loss_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/top_level.txt
```

### Comparing `jax_fdm-0.6.0/CHANGELOG.md` & `jax_fdm-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] 2023-05-08
+
+### Added
+ 
+- Added `EquilibriumStructure.init` as a quick fix to warm start properties.
+
+### Changed
+
+- Changed signature of equilibrium model to be `EquilibriumModel(params, structure)`.
+- The `init` function in goals, constraints and parameter takes `(model, structure)` as arguments.
+- Removed `connectivity` related operations from `EquilibriumModel` and inserted them into `EquilibriumStructure`.
+- Fixed bug in `EquilibriumStructure.nodes` that led to a recursive timeout error.
+- Renamed example file `butt.py` to `vault.py`/
+- Renamed file `optimizers.py` to `scipy.py` in `jax_fdm.optimization`.
+
+### Removed
+
+- Removed `structure` attribute from `EquilibriumModel` en route to equinox modules. 
+
 ## [0.6.0] 2023-04-30
 
 ### Added
 
 Support for differentiable CPU sparse solver
 - Added support for differentiable CPU and GPU sparse solvers to compute the XYZ coordinates of the free nodes with FDM. The solver is custom made and registered via a `jax.custom_vjp`. The forward and backward passes of the sparse solver were made possible thanks to the contributions of @denizokt. This solver lives in `equilibrium.sparse.py`.
 - Added `spsolve_gpu` and `spsolve_cpu`. The sparse solver backend is different (the former uses CUDA and the latter scipy) and it gets selected automatically based on what the value of `jax.default_device` is at runtime with function `register_sparse_solver`.
```

### Comparing `jax_fdm-0.6.0/LICENSE` & `jax_fdm-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/PKG-INFO` & `jax_fdm-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_fdm
-Version: 0.6.0
+Version: 0.7.0
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax_fdm-0.6.0/README.md` & `jax_fdm-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/setup.cfg` & `jax_fdm-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/setup.py` & `jax_fdm-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="jax_fdm",
-    version="0.6.0",
+    version="0.7.0",
     description="Auto-differentiable and hardware-accelerated force density method",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arpastrana/jax_fdm",
     author="Rafael Pastrana",
     author_email="arpastrana@princeton.edu",
     license="MIT license",
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/__init__.py` & `jax_fdm-0.7.0/src/jax_fdm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import jax.numpy as jnp
 
 
 __author__ = ["Rafael Pastrana"]
 __copyright__ = "Rafael Pastrana"
 __license__ = "MIT License"
 __email__ = "arpastrana@princeton.edu"
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/constraints/constraint.py` & `jax_fdm-0.7.0/src/jax_fdm/constraints/constraint.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,27 +86,26 @@
     @staticmethod
     def index_from_model(model):
         """
         Get the index in the model of the constraint key.
         """
         raise NotImplementedError
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the constraint with information from an equilibrium model.
         """
-        self.index = self.index_from_model(model)
+        self.index = self.index_from_model(model, structure)
 
-    def __call__(self, q, xyz_fixed, loads, model):
+    def __call__(self, params, model, structure):
         """
         The called constraint function.
         """
-        eqstate = model(q, xyz_fixed, loads)
+        eqstate = model(params, structure)
         constraint = vmap(self.constraint, in_axes=(None, 0))(eqstate, self.index)
-
         # assert jnp.ravel(constraint).shape == jnp.ravel(self.index).shape, f"Constraint shape: {constraint.shape} vs. index shape: {self.index.shape}"
 
         return jnp.ravel(constraint)
 
     def constraint(self, eqstate, index):
         """
         The constraint function.
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/constraints/edge/angle.py` & `jax_fdm-0.7.0/src/jax_fdm/constraints/edge/angle.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,19 +32,19 @@
         Create a matrix of vectors.
         """
         matrix = np.zeros((max(self.index) + 1, 3))
         for vec, idx in zip(self.vector, self.index):
             matrix[idx, :] = vec
         return matrix
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the constraint with information from an equilibrium model.
         """
-        super().init(model)
+        super().init(model, structure)
         self.vector = self.vectors()
 
     def constraint(self, eqstate, index):
         """
         Returns the angle between an edge in an equilibrium state and a vector.
         """
         vector = eqstate.vectors[index, :]
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/constraints/node/coordinates.py` & `jax_fdm-0.7.0/src/jax_fdm/constraints/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/constraints/node/curvature.py` & `jax_fdm-0.7.0/src/jax_fdm/constraints/node/curvature.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     Constraints the (discrete) curvature of a node based on its surrounding polygon of neighboring nodes.
     """
     def __init__(self, key, polygon, bound_low, bound_up):
         super().__init__(key, bound_low, bound_up)
         self.polygon = polygon
         self.index_polygon = None
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the constraint with information from an equilibrium model.
         """
-        super().init(model)
-        self.index_polygon = self.polygon_indices(model)
+        super().init(model, structure)
+        self.index_polygon = self.polygon_indices(model, structure)
 
-    def polygon_indices(self, model):
+    def polygon_indices(self, model, structure):
         """
         Obtains the indices of the polygon from a model.
         """
         index_max = max(self.index) + 1
         polygon = np.atleast_2d(self.polygon)
         index_polygon = np.zeros((index_max, polygon.shape[1]))
         for p, idx in zip(polygon, self.index):
-            index_polygon[idx, :] = tuple([model.structure.node_index[nbr] for nbr in p])
+            index_polygon[idx, :] = tuple([structure.node_index[nbr] for nbr in p])
 
         return jnp.array(index_polygon, dtype=jnp.int64)
 
     def constraint(self, eqstate, index):
         """
         Returns the curvature at a node based on the xyz coordinates of its one-hop neighborhood.
         """
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/constraints/node/normal.py` & `jax_fdm-0.7.0/src/jax_fdm/constraints/node/normal.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,72 +38,72 @@
         Create a matrix of vectors.
         """
         matrix = np.zeros((max(self.index) + 1, 3))
         for vec, idx in zip(self.vector, self.index):
             matrix[idx, :] = vec
         return matrix
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the constraint with information from an equilibrium model.
         """
-        super().init(model)
+        super().init(model, structure)
         self.vector = self.vectors()
-        self.index_faces, self.mask_faces = self.faces_indices(model)
+        self.index_faces, self.mask_faces = self.faces_indices(model, structure)
 
-    def faces_indices(self, model):
+    def faces_indices(self, model, structure):
         """
         Get the node indices of the faces connected to a node.
 
         TODO: Please refactor me! I am illegible :(
         """
         index_max = max(self.index) + 1
 
         num_nodes_max = -1
         num_faces_max = -1
         for idx in self.index:
-            num_faces = len(self.node_faces(model, idx))
+            num_faces = len(self.node_faces(model, structure, idx))
             if num_faces > num_faces_max:
                 num_faces_max = num_faces
-            num_nodes = len(max(self.node_faces_indices(model, idx), key=lambda x: len(x)))
+            num_nodes = len(max(self.node_faces_indices(model, structure, idx), key=lambda x: len(x)))
             if num_nodes > num_nodes_max:
                 num_nodes_max = num_nodes
 
         index_faces = np.zeros((index_max, num_faces_max, num_nodes_max + 1))
         mask_faces = np.zeros((index_max, num_faces_max, num_nodes_max + 1))
 
         for idx in self.index:
-            nfn = self.node_faces_indices(model, idx)
+            nfn = self.node_faces_indices(model, structure, idx)
             for i, face_nodes in enumerate(nfn):
                 index_faces[idx, i, :len(face_nodes)] = face_nodes
                 mask_faces[idx, i, :len(face_nodes)] = [1] * len(face_nodes)
 
                 index_faces[idx, i, -1] = face_nodes[-1]
                 mask_faces[idx, i, -1] = 1
 
         index_faces = jnp.asarray(index_faces, dtype=jnp.int64)
         mask_faces[mask_faces == 0] = jnp.nan
         mask_faces = jnp.asarray(mask_faces, dtype=jnp.float64)
 
         return index_faces, mask_faces
 
     @staticmethod
-    def node_faces(model, index):
+    def node_faces(model, structure, index):
         """
         Return an iterable with the indices of the faces connected to a node.
         """
-        connectivity = model.structure.connectivity_faces
+        connectivity = structure.connectivity_faces
         return np.flatnonzero(connectivity[:, index])
 
-    def node_faces_indices(self, model, index):
+    def node_faces_indices(self, model, structure, index):
         """
         Return an iterable with the indices of the nodes of the faces connected to a node.
         """
-        fidx = self.node_faces(model, index)
-        return [model.structure.face_node_index[idx] for idx in fidx]
+        fidx = self.node_faces(model, structure, index)
+        return [structure.face_node_index[idx] for idx in fidx]
 
     @staticmethod
     def nan_normal_polygon(polygon):
         """
         Compute the normal of a polygon that contains nan entries.
         """
         centroid = jnp.nanmean(polygon, axis=0)
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/constraints/node/tangent.py` & `jax_fdm-0.7.0/src/jax_fdm/constraints/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/datastructures.py` & `jax_fdm-0.7.0/src/jax_fdm/datastructures.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/equilibrium/fdm.py` & `jax_fdm-0.7.0/src/jax_fdm/equilibrium/fdm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import numpy as np
 
 from jax_fdm import DTYPE_NP
 
 from jax_fdm.equilibrium import EquilibriumModel
 from jax_fdm.equilibrium import EquilibriumModelSparse
 
+from jax_fdm.equilibrium import EquilibriumStructure
+from jax_fdm.equilibrium import EquilibriumStructureSparse
+
 
 # ==========================================================================
 # Form-finding
 # ==========================================================================
 
-def _fdm(q, xyz_fixed, loads, model, network):
+def _fdm(model, params, structure, network):
     """
     Compute a network in a state of static equilibrium using the force density method.
     """
     # compute static equilibrium
-    eq_state = model(q, xyz_fixed, loads)
+    eq_state = model(params, structure)
 
     # update equilibrium state in a copy of the network
     return network_updated(network, eq_state)
 
 
 def fdm(network, sparse=True):
     """
     Compute a network in a state of static equilibrium using the force density method.
     """
     network_validate(network)
 
     model = model_from_network(network, sparse)
-    q, xyz_fixed, loads = (np.array(p, dtype=DTYPE_NP) for p in network.parameters())
+    structure = structure_from_network(network, sparse)
+
+    params = [np.array(p, dtype=DTYPE_NP) for p in network.parameters()]
 
-    return _fdm(q, xyz_fixed, loads, model, network)
+    return _fdm(model, params, structure, network)
 
 
 # ==========================================================================
 # Constrained form-finding
 # ==========================================================================
 
 def constrained_fdm(network,
@@ -52,20 +57,21 @@
     network_validate(network)
 
     if constraints and sparse:
         print("Constraints are not supported yet for sparse inputs. Switching to dense.")
         sparse = False
 
     model = model_from_network(network, sparse)
+    structure = structure_from_network(network, sparse)
 
-    opt_problem = optimizer.problem(model, loss, parameters, constraints, maxiter, tol, callback)
+    opt_problem = optimizer.problem(model, structure, loss, parameters, constraints, maxiter, tol, callback)
     opt_params = optimizer.solve(opt_problem)
-    q, xyz_fixed, loads = optimizer.parameters_fdm(opt_params)
+    params = optimizer.parameters_fdm(opt_params)
 
-    return _fdm(q, xyz_fixed, loads, model, network)
+    return _fdm(model, params, structure, network)
 
 
 # ==========================================================================
 # Helpers
 # ==========================================================================
 
 def model_from_network(network, sparse):
@@ -75,14 +81,25 @@
     model = EquilibriumModel
     if sparse:
         model = EquilibriumModelSparse
 
     return model.from_network(network)
 
 
+def structure_from_network(network, sparse):
+    """
+    Create a structure from a network.
+    """
+    structure = EquilibriumStructure
+    if sparse:
+        structure = EquilibriumStructureSparse
+
+    return structure.from_network(network)
+
+
 def network_validate(network):
     """
     Check that the network is healthy.
     """
     assert network.number_of_supports() > 0, "The network has no supports"
     assert network.number_of_edges() > 0, "The network has no edges"
     assert network.number_of_nodes() > 0, "The network has no nodes"
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/equilibrium/model.py` & `jax_fdm-0.7.0/src/jax_fdm/equilibrium/sparse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,171 @@
+"""
+NOTE: Sparse solver does not support forward mode auto-differentiation yet.
+"""
 from functools import partial
 
-import numpy as np
+import jax
 import jax.numpy as jnp
 
-from jax import jit
+from scipy.sparse import csc_matrix
+from scipy.sparse.linalg import spsolve as spsolve_scipy
 
 from jax.experimental.sparse import CSC
+from jax.experimental.sparse.linalg import spsolve as spsolve_jax
 
-from jax_fdm.equilibrium.state import EquilibriumState
-from jax_fdm.equilibrium.structure import EquilibriumStructure
-from jax_fdm.equilibrium.structure import EquilibriumStructureSparse
-
-from jax_fdm.equilibrium.sparse import sparse_solve
-
-
-# ==========================================================================
-# Equilibrium model
-# ==========================================================================
-
-class EquilibriumModel:
-    """
-    The equilibrium solver.
-    """
-    def __init__(self, network):
-        self.structure = EquilibriumStructure(network)
-
-    @classmethod
-    def from_network(cls, network):
-        """
-        Create an equilibrium model from a force density network.
-        """
-        return cls(network)
-
-    @staticmethod
-    def edges_vectors(xyz, connectivity):
-        """
-        Calculate the unnormalized edge directions.
-        """
-        return connectivity @ xyz
-
-    @staticmethod
-    def edges_lengths(vectors):
-        """
-        Compute the length of the edges.
-        """
-        return jnp.linalg.norm(vectors, axis=1, keepdims=True)
-
-    @staticmethod
-    def edges_forces(q, lengths):
-        """
-        Calculate the force in the edges.
-        """
-        return jnp.reshape(q, (-1, 1)) * lengths
-
-    @staticmethod
-    def nodes_residuals(q, loads, vectors, connectivity):
-        """
-        Compute the force at the anchor supports of the structure.
-        """
-        return loads - connectivity.T @ (q[:, None] * vectors)
-
-    @staticmethod
-    def nodes_positions(xyz_free, xyz_fixed, indices):
-        """
-        Concatenate in order the position of the free and the fixed nodes.
-        """
-        return jnp.concatenate((xyz_free, xyz_fixed))[indices, :]
-
-    def nodes_free_positions(self, q, xyz_fixed, loads):
-        """
-        Calculate the XYZ coordinates of the free nodes.
-        """
-        # shorthand
-        free = self.structure.free_nodes
-        c_fixed = self.structure.connectivity_fixed
-        c_free = self.structure.connectivity_free
-
-        A = c_free.T @ (q[:, None] * c_free)
-        b = loads[free, :] - c_free.T @ (q[:, None] * (c_fixed @ xyz_fixed))
-
-        return jnp.linalg.solve(A, b)
-
-    @partial(jit, static_argnums=0)
-    def __call__(self, q, xyz_fixed, loads):
-        """
-        Compute an equilibrium state using the force density method.
-        """
-        connectivity = self.structure.connectivity  # dense jax matrix now. BCOO, better?
-        indices = self.structure.freefixed_nodes  # tuple
-
-        xyz_free = self.nodes_free_positions(q, xyz_fixed, loads)
-        xyz_all = self.nodes_positions(xyz_free, xyz_fixed, indices)
-        vectors = self.edges_vectors(xyz_all, connectivity)
-        residuals = self.nodes_residuals(q, loads, vectors, connectivity)
-        lengths = self.edges_lengths(vectors)
-        forces = self.edges_forces(q, lengths)
-
-        return EquilibriumState(xyz=xyz_all,
-                                residuals=residuals,
-                                lengths=lengths,
-                                forces=forces,
-                                vectors=vectors,
-                                loads=loads,
-                                force_densities=q)
-
-
-# ==========================================================================
-# Sparse equilibrium model
-# ==========================================================================
-
-class EquilibriumModelSparse(EquilibriumModel):
-    """
-    The equilibrium solver. Sparse.
-    """
-    def __init__(self, network):
-        self.structure = EquilibriumStructureSparse(network)
-
-        # Do some precomputation to be able to construct the lhs matrix through indexing
-        c_free_csc = self.structure.connectivity_scipy[:, self.structure.free_nodes]
-        index_array = self._get_sparse_index_array(c_free_csc)
-        self.index_array = index_array
-
-        # Indices of data corresponding to diagonal.
-        # With this array we can just index directly into the CSC.data array to refer to the diagonal entries.
-        self.diag_indices = self._get_sparse_diag_indices(index_array)
-
-        # Prepare the array D st when D.T @ q we get the diagonal elements of matrix.
-        self.diags = self._get_sparse_diag_data(c_free_csc)
-
-    def nodes_free_positions(self, q, xyz_fixed, loads):
-        """
-        Calculate the XYZ coordinates of the free nodes.
-        """
-        return sparse_solve(q,  # differentiable parameters
-                            xyz_fixed,
-                            loads,
-                            self.structure.free_nodes,  # connectivity (non-differentiable)
-                            self.structure.connectivity_free,
-                            self.structure.connectivity_fixed,
-                            self.index_array,  # precomputed data (non-differentiable)
-                            self.diag_indices,
-                            self.diags)
-
-    def _get_sparse_index_array(self, c_free_csc):
-        """
-        Create an index array such that the off-diagonals can index into the force density vector.
-
-        This array is used to create the off-diagonal entries of the lhs matrix.
-        """
-        force_density_modified_c_free_csc = c_free_csc.copy()
-        force_density_modified_c_free_csc.data *= np.take(np.arange(c_free_csc.shape[0]) + 1, c_free_csc.indices)
-        index_array = -(c_free_csc.T @ force_density_modified_c_free_csc)
-
-        # The diagonal entries should be set to 0 so that it indexes
-        # into a valid entry, but will later be overwritten.
-        index_array.setdiag(0)
-
-        return index_array.astype(int)
-
-    @staticmethod
-    def _get_sparse_diag_data(c_free_csc):
-        """
-        The diagonal of the lhs matrix is the sum of force densities for
-        each outgoing/incoming edge on the node.
-
-        We create the `diags` matrix such that when we multiply it with the
-        force density vector we get the diagonal.
-        """
-        diags_data = jnp.ones_like(c_free_csc.data)
-
-        return CSC((diags_data, c_free_csc.indices, c_free_csc.indptr), shape=c_free_csc.shape)
-
-    @staticmethod
-    def _get_sparse_diag_indices(csc):
-        """
-        Given a CSC matrix, get indices into `data` that access diagonal elements in order.
-        """
-        all_indices = []
-        for i in range(csc.shape[0]):
-            index_range = csc.indices[csc.indptr[i]:csc.indptr[i + 1]]
-            ind_loc = jnp.where(index_range == i)[0]
-            all_indices.append(ind_loc + csc.indptr[i])
 
-        return jnp.concatenate(all_indices)
+# ==========================================================================
+# Register sparse linear solvers
+# ==========================================================================
+
+def spsolve_gpu(A, b):
+    """
+    A wrapper around cuda sparse linear solver that is GPU friendly.
+
+    Notes
+    -----
+    We must split b into three vectors (one per spatial coordinate),
+    and then solve a sparse system 3 times because the CUDA sparse solver
+    in the backend cannot take b as a matrix.
+
+    The sparse solve in a GPU is thus 3x more expensive than if it could
+    solve for the b matrix all at once.
+
+    This limitation with CUDA might make a GPU sparse solve more expensive
+    than a CPU sparse solve. So use this method with a pinch of salt.
+    """
+    # NOTE: we can pass csc indices directly because we can!
+    # Just kidding. This is because the matrix A is symmetric :)
+
+    # TODO: Ravel and unravel this!
+    x = spsolve_jax(A.data, A.indices, A.indptr, b[:, 0])
+    y = spsolve_jax(A.data, A.indices, A.indptr, b[:, 1])
+    z = spsolve_jax(A.data, A.indices, A.indptr, b[:, 2])
+
+    return jnp.stack((x, y, z), axis=1)
+
+
+def spsolve_cpu(A, b):
+    """
+    A wrapper around scipy sparse linear solver that acts as a JAX pure callback.
+    """
+    def callback(data, indices, indptr, _b):
+        _A = csc_matrix((data, indices, indptr))
+        return spsolve_scipy(_A, _b)
+
+    xk = jax.pure_callback(callback,  # callback function
+                           b,  # return type is b
+                           A.data,  # callback function arguments from here on
+                           A.indices,
+                           A.indptr,
+                           b)
+    return xk
+
+
+def register_sparse_solver(solvers):
+    """
+    Register the sparse solver used by the FDM model based on JAX default backend.
+    """
+    backend = jax.default_backend()
+    sparse_solver = solvers.get(backend)
+
+    if not sparse_solver:
+        raise ValueError(f"Default backend {backend} does not support a sparse solver")
+
+    return sparse_solver
+
+
+solvers = {"cpu": spsolve_cpu,
+           "gpu": spsolve_gpu}
+
+spsolve = register_sparse_solver(solvers)
+
+
+# ==========================================================================
+# Define sparse linear solver
+# ==========================================================================
+
+@partial(jax.custom_vjp, nondiff_argnums=(3, 4, 5, 6, 7, 8))
+def sparse_solve(q, xyz_fixed, loads, free, c_free, c_fixed, index_array, diag_indices, diags):
+    """
+    The sparse linear solver.
+    """
+    A = force_densities_to_A(q, index_array, diag_indices, diags)
+    b = force_densities_to_b(q, loads, xyz_fixed, c_free, c_fixed, free)
+
+    return spsolve(A, b)
+
+
+# ==========================================================================
+# Forward and backward passes
+# ==========================================================================
+
+def sparse_solve_fwd(q, xyz_fixed, loads, free, c_free, c_fixed, index_array, diag_indices, diags):
+    """
+    Forward pass of the sparse linear solver.
+
+    Call the linear solve and save parameters and solution for the backward pass.
+    """
+    xk = sparse_solve(q, xyz_fixed, loads, free, c_free, c_fixed, index_array, diag_indices, diags)
+
+    return xk, (xk, q, xyz_fixed, loads)
+
+
+def sparse_solve_bwd(free, c_free, c_fixed, index_array, diag_indices, diags, res, g):
+    """
+    Backward pass of the sparse linear solver.
+    """
+    xk, q, xyz_fixed, loads = res
+
+    # function that translates parameters into LHS matrix in CSC format
+    A = force_densities_to_A(q, index_array, diag_indices, diags)
+
+    # Solve adjoint system
+    # A.T @ xk_bar = -g
+    lam = spsolve(A, g)
+
+    # the implicit constraint function for implicit differentiation
+    def residual_fn(params):
+        q, xyz_fixed, loads = params
+        A = force_densities_to_A(q, index_array, diag_indices, diags)
+        b = force_densities_to_b(q, loads, xyz_fixed, c_free, c_fixed, free)
+        return b - A @ xk
+
+    params = (q, xyz_fixed, loads)
+
+    # Call vjp of residual_fn to compute gradient wrt params
+    params_bar = jax.vjp(residual_fn, params)[1](lam)[0]
+
+    return params_bar
+
+
+# ==========================================================================
+# Helpers
+# ==========================================================================
+
+def force_densities_to_A(q, index_array, diag_indices, diags):
+    """
+    Computes the LHS matrix in CSC format from a vector of force densities.
+    """
+    nondiags_data = -q[index_array.data - 1]
+    nondiags = CSC((nondiags_data, index_array.indices, index_array.indptr), shape=index_array.shape)
+    diag_fd = diags.T @ q  # sum of force densities for each node
+
+    nondiags.data = nondiags.data.at[diag_indices].set(diag_fd)
+
+    return nondiags
+
+
+def force_densities_to_b(q, loads, xyz_fixed, c_free, c_fixed, free):
+    """
+    Computes the RHS matrix in dense format from a vector of force densities.
+    """
+    b = loads[free, :] - c_free.T @ (q[:, None] * (c_fixed @ xyz_fixed))
+
+    return b
+
+
+# ==========================================================================
+# Register forward and backward passes to JAX
+# ==========================================================================
+
+sparse_solve.defvjp(sparse_solve_fwd, sparse_solve_bwd)
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/geometry.py` & `jax_fdm-0.7.0/src/jax_fdm/geometry.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/abstract_goal.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/abstract_goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/edge/angle.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/edge/angle.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
         """
         return self._vector
 
     @vector.setter
     def vector(self, vector):
         self._vector = jnp.reshape(jnp.asarray(vector), (-1, 3))
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the goal with information from an equilibrium model.
         """
-        super().init(model)
+        super().init(model, structure)
 
         # create matrix of vectors
         vector = self.vector
         vm = np.zeros((max(self.index) + 1, 3))
         for v, idx in zip(vector, self.index):
             vm[idx, :] = v
         self.vector = vm
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/edge/direction.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/edge/direction.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/edge/edge.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/edge/edge.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class EdgeGoal(Goal):
     """
     Base class for all goals that pertain to an edge of a network.
     """
     def __init__(self, key, target, weight=1.0):
         super().__init__(key=key, target=target, weight=weight)
 
-    def index_from_model(self, model):
+    def index_from_model(self, model, structure):
         """
         The index of the edge key in an equilibrium structure.
         """
         try:
-            return model.structure.edge_index[self.key]
+            return structure.edge_index[self.key]
         except TypeError:
-            return tuple([model.structure.edge_index[k] for k in self.key])
+            return tuple([structure.edge_index[k] for k in self.key])
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/edge/force.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/edge/force.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     Equalize the internal force in a selection of edges by minimizing
     the normalized variance of their internal forces.
     """
     def __init__(self, key, weight=1.0):
         super().__init__(key=key, target=0.0, weight=weight)
         self.is_collectible = False
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the goal with information from an equilibrium model.
         """
-        self.index = [super().index_from_model(model)]
+        self.index = [super().index_from_model(model, structure)]
 
     @staticmethod
     def prediction(eq_state, index):
         """
         The normalized variance of the forces of the edges.
         """
         forces = eq_state.forces[index]
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/edge/length.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/edge/length.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     Equalize the length of a selection of edges by minimizing
     the normalized variance of their lengths.
     """
     def __init__(self, key, weight=1.0):
         super().__init__(key=key, target=0.0, weight=weight)
         self.is_collectible = False
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the goal with information from an equilibrium model.
         """
-        self.index = [super().index_from_model(model)]
+        self.index = [super().index_from_model(model, structure)]
 
     @staticmethod
     def prediction(eq_state, index):
         """
         The normalized variance of the lengths of the edges.
         """
         lengths = eq_state.lengths[index]
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/goal.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/goal.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,19 @@
     @staticmethod
     def goal(target, prediction):
         """
         The target to achieve.
         """
         return target
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the goal with information from an equilibrium model.
         """
-        self.index = self.index_from_model(model)
+        self.index = self.index_from_model(model, structure)
 
     def __call__(self, eqstate):
         """
         Return the current goal state.
         """
         prediction = vmap(self.prediction, in_axes=(None, 0))(eqstate, self.index)
         goal = vmap(self.goal)(self.target, prediction)
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/helpers.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/network/loadpath.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/network/loadpath.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/coordinates.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/line.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/line.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/node.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/node.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class NodeGoal(Goal):
     """
     Base class for all goals that pertain to the node of a network.
     """
     def __init__(self, key, target, weight=1.0):
         super().__init__(key=key, target=target, weight=weight)
 
-    def index_from_model(self, model):
+    def index_from_model(self, model, structure):
         """
         The index of the edge in a structure.
         """
         try:
-            return model.structure.node_index[self.key]
+            return structure.node_index[self.key]
         except TypeError:
-            return tuple([model.structure.node_index[k] for k in self.key])
+            return tuple([structure.node_index[k] for k in self.key])
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/normal.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/normal.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,72 +39,72 @@
         Create a matrix of vectors.
         """
         matrix = np.zeros((max(self.index) + 1, 3))
         for vec, idx in zip(self.vector, self.index):
             matrix[idx, :] = vec
         return matrix
 
-    def init(self, model):
+    def init(self, model, structure):
         """
         Initialize the constraint with information from an equilibrium model.
         """
-        super().init(model)
+        super().init(model, structure)
         self.vector = self.vectors()
-        self.index_faces, self.mask_faces = self.faces_indices(model)
+        self.index_faces, self.mask_faces = self.faces_indices(model, structure)
 
-    def faces_indices(self, model):
+    def faces_indices(self, model, structure):
         """
         Get the node indices of the faces connected to a node.
 
         TODO: Please refactor me! I am illegible :(
         """
         index_max = max(self.index) + 1
 
         num_nodes_max = -1
         num_faces_max = -1
         for idx in self.index:
-            num_faces = len(self.node_faces(model, idx))
+            num_faces = len(self.node_faces(model, structure, idx))
             if num_faces > num_faces_max:
                 num_faces_max = num_faces
-            num_nodes = len(max(self.node_faces_indices(model, idx), key=lambda x: len(x)))
+            num_nodes = len(max(self.node_faces_indices(model, structure, idx), key=lambda x: len(x)))
             if num_nodes > num_nodes_max:
                 num_nodes_max = num_nodes
 
         index_faces = np.zeros((index_max, num_faces_max, num_nodes_max + 1))
         mask_faces = np.zeros((index_max, num_faces_max, num_nodes_max + 1))
 
         for idx in self.index:
-            nfn = self.node_faces_indices(model, idx)
+            nfn = self.node_faces_indices(model, structure, idx)
             for i, face_nodes in enumerate(nfn):
                 index_faces[idx, i, :len(face_nodes)] = face_nodes
                 mask_faces[idx, i, :len(face_nodes)] = [1] * len(face_nodes)
 
                 index_faces[idx, i, -1] = face_nodes[-1]
                 mask_faces[idx, i, -1] = 1
 
         index_faces = jnp.asarray(index_faces, dtype=jnp.int64)
         mask_faces[mask_faces == 0] = jnp.nan
         mask_faces = jnp.asarray(mask_faces, dtype=jnp.float64)
 
         return index_faces, mask_faces
 
     @staticmethod
-    def node_faces(model, index):
+    def node_faces(model, structure, index):
         """
         Return an iterable with the indices of the faces connected to a node.
         """
-        connectivity = model.structure.connectivity_faces
+        connectivity = structure.connectivity_faces
         return np.flatnonzero(connectivity[:, index])
 
-    def node_faces_indices(self, model, index):
+    def node_faces_indices(self, model, structure, index):
         """
         Return an iterable with the indices of the nodes of the faces connected to a node.
         """
-        fidx = self.node_faces(model, index)
-        return [model.structure.face_node_index[idx] for idx in fidx]
+        fidx = self.node_faces(model, structure, index)
+        return [structure.face_node_index[idx] for idx in fidx]
 
     @staticmethod
     def nan_normal_polygon(polygon):
         """
         Compute the normal of a polygon that contains nan entries.
         """
         centroid = jnp.nanmean(polygon, axis=0)
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/plane.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/plane.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/residual.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/residual.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/goals/node/tangent.py` & `jax_fdm-0.7.0/src/jax_fdm/goals/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/losses/errors.py` & `jax_fdm-0.7.0/src/jax_fdm/losses/errors.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/losses/loss.py` & `jax_fdm-0.7.0/src/jax_fdm/losses/loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,24 @@
         self._terms_error = None
         self._terms_regularization = None
 
         self.terms_error = args
         self.terms_regularization = args
         self.name = name or self.__class__.__name__
 
-    @partial(jit, static_argnums=(0, 4))
-    def __call__(self, q, xyz_fixed, loads, model):
+    @partial(jit, static_argnums=(0, 2, 3))
+    def __call__(self, params, model, structure):
         """
         Compute the scalar output of the loss function.
         """
-        eqstate = model(q, xyz_fixed, loads)
+        eq_state = model(params, structure)
 
         loss = 0.0
         for error_term in self.terms:
-            loss = loss + error_term(eqstate)
+            loss = loss + error_term(eq_state)
 
         return loss
 
     @property
     def terms_error(self):
         """
         The error terms in the loss function.
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/collections.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/collections.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/constrained.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/constrained.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/ipopt.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/ipopt.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizer.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/optimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,78 +49,81 @@
         """
         pass
 
 # ==========================================================================
 # Loss
 # ==========================================================================
 
-    @partial(jit, static_argnums=(0, 2, 3))
-    def loss(self, params_opt, loss, model):
+    # @partial(jit, static_argnums=(0, 2, 3))
+    def loss(self, params_opt, loss, model, structure):
         """
         The wrapper loss.
         """
-        q, xyz_fixed, loads = self.parameters_fdm(params_opt)
+        params = self.parameters_fdm(params_opt)
 
-        return loss(q, xyz_fixed, loads, model)
+        return loss(params, model, structure)
 
 # ==========================================================================
 # Goals
 # ==========================================================================
 
-    def goals(self, loss, model):
+    def goals(self, loss, model, structure):
         """
         Pre-process the goals in the loss function to accelerate computations.
         """
         for term in loss.terms_error:
             goal_collections = self.collect_goals(term.goals)
             for goal_collection in goal_collections:
-                goal_collection.init(model)
+                goal_collection.init(model, structure)
             term.collections = goal_collections
 
 # ==========================================================================
 # Minimization
 # ==========================================================================
 
     def problem(self,
                 model,
+                structure,
                 loss,
                 parameters=None,
                 constraints=None,
                 maxiter=100,
                 tol=1e-6,
                 callback=None):
         """
         Set up an optimization problem.
         """
         # optimization parameters
         if not parameters:
-            parameters = [EdgeForceDensityParameter(edge) for edge in model.structure.edges]
+            parameters = [EdgeForceDensityParameter(edge) for edge in structure.edges]
 
-        self.pm = ParameterManager(model, parameters)
+        self.pm = ParameterManager(model, structure, parameters)
         x = self.parameters_value()
 
         # message
         print(f"\n***Constrained form finding***\nParameters: {len(x)} \tGoals: {loss.number_of_goals()}")
 
         # parameter bounds
         bounds = self.parameters_bounds()
 
         assert x.size == self.pm.bounds_low.size
         assert x.size == self.pm.bounds_up.size
 
         # build goal collections
-        self.goals(loss, model)
+        self.goals(loss, model, structure)
         print(f"\tGoal collections: {loss.number_of_collections()}")
 
         # loss matters
-        loss = partial(self.loss, loss=loss, model=model)
+        loss = partial(self.loss, loss=loss, model=model, structure=structure)
+        loss = jit(loss)
 
         print("Warming up the pressure cooker...")
         start_time = time()
-        _ = loss(x)
+        loss_val = loss(x)
+        print(f"\tInitial loss value: {loss_val:.4}")
         print(f"\tLoss warmup time: {(time() - start_time):.4} seconds")
 
         # gradient of the loss function
         grad_loss = self.gradient(loss)  # w.r.t. first function argument
         start_time = time()
         _ = grad_loss(x)
         print(f"\tGradient warmup time: {(time() - start_time):.4} seconds")
@@ -132,16 +135,16 @@
             _ = hessian_loss(x)
             print(f"\tHessian warmup time: {(time() - start_time):.4} seconds")
 
         # constraints
         constraints = constraints or []
         if constraints:
             start_time = time()
-            constraints = self.constraints(constraints, model, x)
-            print(f"\tConstraints warmup time: {round(time() - start_time, 4)} seconds")
+            constraints = self.constraints(constraints, model, structure, x)
+            print(f"\tConstraints warmup time: {(time() - start_time):.4} seconds")
 
         opt_kwargs = {"fun": loss,
                       "jac": grad_loss,
                       "hess": hessian_loss,
                       "method": self.name,
                       "x0": x,
                       "tol": tol,
@@ -159,15 +162,15 @@
         print(f"Optimization with {self.name} started...")
         start_time = time()
 
         # minimize
         res_q = self._minimize(opt_problem)
 
         print(res_q.message)
-        print(f"Final loss in {res_q.nit} iterations: {res_q.fun}")
+        print(f"Final loss in {res_q.nit} iterations: {res_q.fun:.4}")
         print(f"Optimization elapsed time: {time() - start_time} seconds")
 
         return res_q.x
 
     @staticmethod
     def _minimize(opt_problem):
         """
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizers.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/second_order.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/second_order.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/optimization/recorders.py` & `jax_fdm-0.7.0/src/jax_fdm/optimization/recorders.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/parameters/helpers.py` & `jax_fdm-0.7.0/src/jax_fdm/parameters/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/parameters/manager.py` & `jax_fdm-0.7.0/src/jax_fdm/parameters/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,21 @@
                        NodeSupportXParameter,
                        NodeSupportYParameter,
                        NodeSupportZParameter,
                        NodeLoadXParameter,
                        NodeLoadYParameter,
                        NodeLoadZParameter]
 
-    def __init__(self, model, parameters):
+    def __init__(self, model, structure, parameters):
         """
         Initialize the manager.
         """
         self.model = model  # model.structure.network holds an FD network object.
-        self.structure = model.structure
-        self.network = model.structure.network
+        self.structure = structure
+        self.network = structure.network
         self.parameters = parameters
 
         self._indices_opt = None
         self._indices_frozen = None
         self._indices_optfrozen = None
         self._indices_groups = None
 
@@ -249,17 +249,17 @@
         """
         Compute the parameter index if a parameter is an instance of a given type.
         """
         indices = []
         for parameter in self.parameters:
             if isinstance(parameter, cls):
                 if isinstance(parameter, ParameterGroup):
-                    indices.extend(parameter.index(self.model))
+                    indices.extend(parameter.index(self.model, self.structure))
                 else:
-                    indices.append(parameter.index(self.model))
+                    indices.append(parameter.index(self.model, self.structure))
 
         # return np.array(indices, dtype=np.int64)
         return indices
 
     def _indices_shift(self, indices, shift):
         """
         Shift a collection of parameter indices by a given integer.
@@ -315,15 +315,15 @@
     def parameters_value(self):
         """
         Return an array with the intial value of the optimization parameters.
         """
         if self._parameters_value is None:
             values = []
             for parameter in self.parameters_ordered:
-                values.append(parameter.value(self.model))
+                values.append(parameter.value(self.model, self.structure))
             self._parameters_value = jnp.array(values, dtype=DTYPE_JAX)
 
         return self._parameters_value
 
 # ==========================================================================
 # Parameters
 # ==========================================================================
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/parameters/parameters.py` & `jax_fdm-0.7.0/src/jax_fdm/parameters/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,42 +76,42 @@
 # Individual parameters
 # ==========================================================================
 
 class NodeParameter(Parameter):
     """
     A node parameter.
     """
-    def index(self, model):
+    def index(self, model, structure):
         """
         Get the index of the key of the node parameter in the structure of a model.
         """
-        return model.structure.node_index[self.key]
+        return structure.node_index[self.key]
 
-    def value(self, model):
+    def value(self, model, structure):
         """
         Get the current value of the node parameter.
         """
-        return model.structure.network.node_attribute(self.key, name=self.attr_name)
+        return structure.network.node_attribute(self.key, name=self.attr_name)
 
 
 class EdgeParameter(Parameter):
     """
     An edge parameter.
     """
-    def index(self, model):
+    def index(self, model, structure):
         """
         Get the index of the key of the edge parameter in the structure of a model.
         """
-        return model.structure.edge_index[self.key]
+        return structure.edge_index[self.key]
 
-    def value(self, model):
+    def value(self, model, structure):
         """
         Get the current value of the edge parameter.
         """
-        return model.structure.network.edge_attribute(self.key, name=self.attr_name)
+        return structure.network.edge_attribute(self.key, name=self.attr_name)
 
 
 # ==========================================================================
 # ParameterGroups
 # ==========================================================================
 
 class ParameterGroup(Parameter):
@@ -123,43 +123,43 @@
         assert len(self.key) > 0
 
 
 class NodesParameter(ParameterGroup):
     """
     A single parameter applied to a group of nodes.
     """
-    def index(self, model):
+    def index(self, model, structure):
         """
         Get the indices of the keys of the parametrized nodes from the structure of a model.
         """
-        return [model.structure.node_index[key] for key in self.key]
+        return [structure.node_index[key] for key in self.key]
 
-    def value(self, model):
+    def value(self, model, structure):
         """
         Get the current average value of the parameter of the grouped nodes.
         """
-        values = [model.structure.network.node_attribute(key, name=self.attr_name) for key in self.key]
+        values = [structure.network.node_attribute(key, name=self.attr_name) for key in self.key]
         return sum(values) / len(values)
 
 
 class EdgesParameter(ParameterGroup):
     """
     A single parameter applied to a group of edges.
     """
-    def index(self, model):
+    def index(self, model, structure):
         """
         Get the indices of the keys of the parametrized edges from the structure of a model.
         """
-        return [model.structure.edge_index[key] for key in self.key]
+        return [structure.edge_index[key] for key in self.key]
 
-    def value(self, model):
+    def value(self, model, structure):
         """
         Get the current average value of the parameter of the grouped edges.
         """
-        values = [model.structure.network.edge_attribute(key, name=self.attr_name) for key in self.key]
+        values = [structure.network.edge_attribute(key, name=self.attr_name) for key in self.key]
         return sum(values) / len(values)
 
 
 # ==========================================================================
 # Edge force densities
 # ==========================================================================
 
@@ -184,19 +184,19 @@
 # Node supports
 # ==========================================================================
 
 class NodeSupportParameter(NodeParameter):
     """
     A node support parameter.
     """
-    def index(self, model):
+    def index(self, model, structure):
         """
         Get the index of the key of the node support in the structure of a model.
         """
-        return model.structure.anchor_index[self.key]
+        return structure.anchor_index[self.key]
 
 
 class NodeSupportXParameter(NodeSupportParameter):
     """
     Parametrize the X coordinate of a support node.
     """
     def __init__(self, *args, **kwargs):
@@ -227,19 +227,19 @@
 # ==========================================================================
 
 
 class NodesSupportParameter(NodesParameter):
     """
     Parametrize a group of support nodes.
     """
-    def index(self, model):
+    def index(self, model, structure):
         """
         Get the indices of the keys of the parametrized nodes from the structure of a model.
         """
-        return [model.structure.anchor_index[key] for key in self.key]
+        return [structure.anchor_index[key] for key in self.key]
 
 
 class NodesSupportXParameter(NodesSupportParameter, NodeSupportXParameter):
     """
     Parametrize wiht a single value the X coordinate of a group of support nodes.
     """
     def __init__(self, *args, **kwargs):
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/artists/network_artist.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/artists/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/network_artist.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/shapes.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/shapes.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/viewer.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/loss_plotter.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/loss_plotter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from time import time
-from functools import partial
 
 import matplotlib.pyplot as plt
 
 from jax import vmap
 import jax.numpy as jnp
 
 from jax_fdm import DTYPE_JAX
 from jax_fdm.equilibrium import EquilibriumModel
+from jax_fdm.equilibrium import EquilibriumStructure
 
 
 __all__ = ["LossPlotter"]
 
 
 class LossPlotter:
     """
     Plot a loss function.
     """
     def __init__(self, loss, network, *args, **kwargs):
         self.loss = loss
-        self.model = EquilibriumModel(network)
+        self.structure = EquilibriumStructure.from_network(network)
         self.fig = plt.figure(**kwargs)
 
     def plot(self, history):
         """
         Plot the loss function and its error components on a list of fdm parameter arrays.
         """
         print("\nPlotting loss function...")
         start_time = time()
 
         q = jnp.asarray(history["q"], dtype=DTYPE_JAX)
         xyz_fixed = jnp.asarray(history["xyz_fixed"], dtype=DTYPE_JAX)
         loads = jnp.asarray(history["loads"], dtype=DTYPE_JAX)
-        model_dense = partial(self.model)
-        eq_states = vmap(model_dense)(q, xyz_fixed, loads)
+
+        model = EquilibriumModel()
+        equilibrium_vmap = vmap(model, in_axes=(0, None))
+        eq_states = equilibrium_vmap((q, xyz_fixed, loads), self.structure)
 
         errors_all = []
         for error_term in self.loss.terms:
             errors = vmap(error_term)(eq_states)
             errors_all.append(errors)
             plt.plot(errors, label=error_term.name)
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/network_artist.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/network_artist.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/viewer.py` & `jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.6.0/src/jax_fdm.egg-info/PKG-INFO` & `jax_fdm-0.7.0/src/jax_fdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-fdm
-Version: 0.6.0
+Version: 0.7.0
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax_fdm-0.6.0/src/jax_fdm.egg-info/SOURCES.txt` & `jax_fdm-0.7.0/src/jax_fdm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 src/jax_fdm/optimization/__init__.py
 src/jax_fdm/optimization/collections.py
 src/jax_fdm/optimization/recorders.py
 src/jax_fdm/optimization/optimizers/__init__.py
 src/jax_fdm/optimization/optimizers/constrained.py
 src/jax_fdm/optimization/optimizers/ipopt.py
 src/jax_fdm/optimization/optimizers/optimizer.py
-src/jax_fdm/optimization/optimizers/optimizers.py
+src/jax_fdm/optimization/optimizers/scipy.py
 src/jax_fdm/optimization/optimizers/second_order.py
 src/jax_fdm/parameters/__init__.py
 src/jax_fdm/parameters/helpers.py
 src/jax_fdm/parameters/manager.py
 src/jax_fdm/parameters/parameters.py
 src/jax_fdm/visualization/__init__.py
 src/jax_fdm/visualization/artists/__init__.py
```

