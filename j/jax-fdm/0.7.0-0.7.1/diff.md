# Comparing `tmp/jax_fdm-0.7.0.tar.gz` & `tmp/jax_fdm-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_fdm-0.7.0.tar", last modified: Mon May  8 19:33:51 2023, max compression
+gzip compressed data, was "jax_fdm-0.7.1.tar", last modified: Mon May  8 20:50:50 2023, max compression
```

## Comparing `jax_fdm-0.7.0.tar` & `jax_fdm-0.7.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.725377 jax_fdm-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/edge/length.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/network/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/force.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/length.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/constraints/node/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/curvature.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/constraints/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/fdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/equilibrium/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/abstract_goal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/edge/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/network/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/network/loadpath.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/goals/node/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/line.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/goals/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/losses/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.733377 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/second_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/optimization/recorders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/artists/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/artists/network_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/loss_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.737377 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-08 19:33:38.000000 jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.729377 jax_fdm-0.7.0/src/jax_fdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 19:33:51.000000 jax_fdm-0.7.0/src/jax_fdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.568112 jax_fdm-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-05-08 20:50:50.568112 jax_fdm-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 20:50:50.568112 jax_fdm-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.556112 jax_fdm-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm/constraints/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/edge/length.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm/constraints/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/network/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/network/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm/constraints/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/node/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/constraints/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/datastructures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/equilibrium/fdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/equilibrium/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/equilibrium/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/equilibrium/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/equilibrium/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/goals/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/abstract_goal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/goals/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/edge/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/edge/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/goals/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/network/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/goals/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/goals/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/losses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/losses/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/second_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/optimization/recorders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/parameters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/parameters/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/parameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.564113 jax_fdm-0.7.1/src/jax_fdm/visualization/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/artists/network_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.568112 jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.568112 jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/loss_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.568112 jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-08 20:50:38.000000 jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:50:50.560113 jax_fdm-0.7.1/src/jax_fdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-05-08 20:50:50.000000 jax_fdm-0.7.1/src/jax_fdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 20:50:50.000000 jax_fdm-0.7.1/src/jax_fdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:50:50.000000 jax_fdm-0.7.1/src/jax_fdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:50:50.000000 jax_fdm-0.7.1/src/jax_fdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 20:50:50.000000 jax_fdm-0.7.1/src/jax_fdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 20:50:50.000000 jax_fdm-0.7.1/src/jax_fdm.egg-info/top_level.txt
```

### Comparing `jax_fdm-0.7.0/CHANGELOG.md` & `jax_fdm-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.1] 2023-05-08
+
+### Added
+
+### Changed
+
+- Fixed signature bug in constraint initialization in `ConstrainedOptimizer.constraints` 
+
+### Removed
+
+- Removed implicit `partial(jit)` decorator on `ConstrainedOptimizer.constraint`. Jitting now takes place explicitly in `ConstrainedOptimizer.constraints`.
+
+
 ## [0.7.0] 2023-05-08
 
 ### Added
  
 - Added `EquilibriumStructure.init` as a quick fix to warm start properties.
 
 ### Changed
```

### Comparing `jax_fdm-0.7.0/LICENSE` & `jax_fdm-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/PKG-INFO` & `jax_fdm-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_fdm
-Version: 0.7.0
+Version: 0.7.1
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
@@ -186,16 +186,16 @@
 
 ## Citation
 
 If you found this library to be useful in academic or industry work, please consider 1) starring the project on Github, and 2) citing it:
 
 ```bibtex
 @software{pastrana_jaxfdm,
-          title={{JAX~FDM}: Auto-differentiable and hardware-accelerated force density method},
-          author={Rafael Pastrana and Deniz Oktay and Ryan Adams and Sigrid Adriaenssens},
+          title={{JAX~FDM}: {A}uto-differentiable and hardware-accelerated force density method},
+          author={Rafael Pastrana and Deniz Oktay and Ryan P. Adams and Sigrid Adriaenssens},
           year={2023},
           doi={10.5281/zenodo.7258292},
           url={https://github.com/arpastrana/jax\_fdm}}
 ```
 
 ## Acknowledgements
```

### Comparing `jax_fdm-0.7.0/README.md` & `jax_fdm-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
 
 ## Citation
 
 If you found this library to be useful in academic or industry work, please consider 1) starring the project on Github, and 2) citing it:
 
 ```bibtex
 @software{pastrana_jaxfdm,
-          title={{JAX~FDM}: Auto-differentiable and hardware-accelerated force density method},
-          author={Rafael Pastrana and Deniz Oktay and Ryan Adams and Sigrid Adriaenssens},
+          title={{JAX~FDM}: {A}uto-differentiable and hardware-accelerated force density method},
+          author={Rafael Pastrana and Deniz Oktay and Ryan P. Adams and Sigrid Adriaenssens},
           year={2023},
           doi={10.5281/zenodo.7258292},
           url={https://github.com/arpastrana/jax\_fdm}}
 ```
 
 ## Acknowledgements
```

### Comparing `jax_fdm-0.7.0/setup.cfg` & `jax_fdm-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/setup.py` & `jax_fdm-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="jax_fdm",
-    version="0.7.0",
+    version="0.7.1",
     description="Auto-differentiable and hardware-accelerated force density method",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arpastrana/jax_fdm",
     author="Rafael Pastrana",
     author_email="arpastrana@princeton.edu",
     license="MIT license",
```

### Comparing `jax_fdm-0.7.0/src/jax_fdm/__init__.py` & `jax_fdm-0.7.1/src/jax_fdm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import jax.numpy as jnp
 
 
 __author__ = ["Rafael Pastrana"]
 __copyright__ = "Rafael Pastrana"
 __license__ = "MIT License"
 __email__ = "arpastrana@princeton.edu"
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `jax_fdm-0.7.0/src/jax_fdm/constraints/constraint.py` & `jax_fdm-0.7.1/src/jax_fdm/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/constraints/edge/angle.py` & `jax_fdm-0.7.1/src/jax_fdm/constraints/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/constraints/node/coordinates.py` & `jax_fdm-0.7.1/src/jax_fdm/constraints/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/constraints/node/curvature.py` & `jax_fdm-0.7.1/src/jax_fdm/constraints/node/curvature.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/constraints/node/normal.py` & `jax_fdm-0.7.1/src/jax_fdm/constraints/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/constraints/node/tangent.py` & `jax_fdm-0.7.1/src/jax_fdm/constraints/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/datastructures.py` & `jax_fdm-0.7.1/src/jax_fdm/datastructures.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/equilibrium/fdm.py` & `jax_fdm-0.7.1/src/jax_fdm/equilibrium/fdm.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/equilibrium/model.py` & `jax_fdm-0.7.1/src/jax_fdm/equilibrium/model.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/equilibrium/sparse.py` & `jax_fdm-0.7.1/src/jax_fdm/equilibrium/sparse.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/equilibrium/structure.py` & `jax_fdm-0.7.1/src/jax_fdm/equilibrium/structure.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/geometry.py` & `jax_fdm-0.7.1/src/jax_fdm/geometry.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/abstract_goal.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/abstract_goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/edge/angle.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/edge/direction.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/edge/direction.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/edge/edge.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/edge/edge.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/edge/force.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/edge/force.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/edge/length.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/edge/length.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/goal.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/helpers.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/network/loadpath.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/network/loadpath.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/coordinates.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/line.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/line.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/node.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/node.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/normal.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/plane.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/plane.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/residual.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/residual.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/goals/node/tangent.py` & `jax_fdm-0.7.1/src/jax_fdm/goals/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/losses/errors.py` & `jax_fdm-0.7.1/src/jax_fdm/losses/errors.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/losses/loss.py` & `jax_fdm-0.7.1/src/jax_fdm/losses/loss.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/collections.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/collections.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/constrained.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/constrained.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,55 +18,55 @@
 # Constrained optimizer
 # ========== ===============================================================
 
 class ConstrainedOptimizer(Optimizer):
     """
     A gradient-based optimizer that handles constraints.
     """
-    def constraints(self, constraints, model, params_opt):
+    def constraints(self, constraints, model, structure, params_opt):
         """
         Returns the defined constraints in a format amenable to `scipy.minimize`.
         """
         if not constraints:
             return
 
         print(f"Constraints: {len(constraints)}")
         constraints = self.collect_constraints(constraints)
         print(f"\tConstraint colections: {len(constraints)}")
 
         clist = []
         for constraint in constraints:
 
             # initialize constraint
-            constraint.init(model)
+            constraint.init(model, structure)
 
             # gather information for scipy constraint
-            fun = partial(self.constraint, constraint=constraint, model=model)
+            fun = partial(self.constraint, constraint=constraint, model=model, structure=structure)
+            fun = jit(fun)
             jac = jit(jacfwd(fun))
 
             lb = constraint.bound_low
             ub = constraint.bound_up
 
             # warm start
             fun(params_opt)
             jac(params_opt)
 
             # store non linear constraint
             clist.append(NonlinearConstraint(fun=fun, jac=jac, lb=lb, ub=ub))
 
         return clist
 
-    @partial(jit, static_argnums=(0, 2, 3))
-    def constraint(self, params_opt, constraint, model):
+    def constraint(self, params_opt, constraint, model, structure):
         """
         A wrapper around a constraint callable object.
         """
-        q, xyz_fixed, loads = self.parameters_fdm(params_opt)
+        params = self.parameters_fdm(params_opt)
 
-        return constraint(q, xyz_fixed, loads, model)
+        return constraint(params, model, structure)
 
     @staticmethod
     def collect_constraints(constraints):
         """
         Convert a list of constraints into a list of constraint collections.
         """
         constraints = sorted(constraints, key=lambda g: type(g).__name__)
```

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/ipopt.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/ipopt.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/optimizer.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/scipy.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/optimizers/second_order.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/optimizers/second_order.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/optimization/recorders.py` & `jax_fdm-0.7.1/src/jax_fdm/optimization/recorders.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/parameters/helpers.py` & `jax_fdm-0.7.1/src/jax_fdm/parameters/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/parameters/manager.py` & `jax_fdm-0.7.1/src/jax_fdm/parameters/manager.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/parameters/parameters.py` & `jax_fdm-0.7.1/src/jax_fdm/parameters/parameters.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/artists/network_artist.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/artists/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/network_artist.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/shapes.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/shapes.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/notebooks/viewer.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/notebooks/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/loss_plotter.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/loss_plotter.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/plotters/network_artist.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/plotters/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/network_artist.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm/visualization/viewers/viewer.py` & `jax_fdm-0.7.1/src/jax_fdm/visualization/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.7.0/src/jax_fdm.egg-info/PKG-INFO` & `jax_fdm-0.7.1/src/jax_fdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-fdm
-Version: 0.7.0
+Version: 0.7.1
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
@@ -186,16 +186,16 @@
 
 ## Citation
 
 If you found this library to be useful in academic or industry work, please consider 1) starring the project on Github, and 2) citing it:
 
 ```bibtex
 @software{pastrana_jaxfdm,
-          title={{JAX~FDM}: Auto-differentiable and hardware-accelerated force density method},
-          author={Rafael Pastrana and Deniz Oktay and Ryan Adams and Sigrid Adriaenssens},
+          title={{JAX~FDM}: {A}uto-differentiable and hardware-accelerated force density method},
+          author={Rafael Pastrana and Deniz Oktay and Ryan P. Adams and Sigrid Adriaenssens},
           year={2023},
           doi={10.5281/zenodo.7258292},
           url={https://github.com/arpastrana/jax\_fdm}}
 ```
 
 ## Acknowledgements
```

### Comparing `jax_fdm-0.7.0/src/jax_fdm.egg-info/SOURCES.txt` & `jax_fdm-0.7.1/src/jax_fdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

