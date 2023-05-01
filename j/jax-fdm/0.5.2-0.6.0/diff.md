# Comparing `tmp/jax_fdm-0.5.2.tar.gz` & `tmp/jax_fdm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_fdm-0.5.2.tar", last modified: Wed Mar 15 21:57:43 2023, max compression
+gzip compressed data, was "jax_fdm-0.6.0.tar", last modified: Mon May  1 02:02:22 2023, max compression
```

## Comparing `jax_fdm-0.5.2.tar` & `jax_fdm-0.6.0.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10150 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-15 21:57:43.098422 jax_fdm-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.086422 jax_fdm-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/constraints/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/edge/length.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/constraints/network/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/network/force.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/network/length.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/constraints/node/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/node/curvature.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/constraints/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/equilibrium/fdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/equilibrium/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/equilibrium/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/equilibrium/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/goals/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/abstract_goal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/goals/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/edge/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/edge/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm/goals/network/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/network/loadpath.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/goals/node/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/line.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/goals/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/losses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/losses/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/constrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/second_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/optimization/recorders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/parameters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/parameters/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/visualization/artists/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/artists/network_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/loss_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.094422 jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-15 21:57:32.000000 jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:57:43.090422 jax_fdm-0.5.2/src/jax_fdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-03-15 21:57:43.000000 jax_fdm-0.5.2/src/jax_fdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-15 21:57:43.000000 jax_fdm-0.5.2/src/jax_fdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:57:43.000000 jax_fdm-0.5.2/src/jax_fdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:57:43.000000 jax_fdm-0.5.2/src/jax_fdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-15 21:57:43.000000 jax_fdm-0.5.2/src/jax_fdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 21:57:43.000000 jax_fdm-0.5.2/src/jax_fdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.562691 jax_fdm-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/edge/length.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm/constraints/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/constraints/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/datastructures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/fdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/equilibrium/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/abstract_goal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/edge/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/network/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/goals/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/goals/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/losses/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/second_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/optimization/recorders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/parameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.570685 jax_fdm-0.6.0/src/jax_fdm/visualization/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/artists/network_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/loss_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.574683 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-01 02:02:10.000000 jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:02:22.566688 jax_fdm-0.6.0/src/jax_fdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 02:02:22.000000 jax_fdm-0.6.0/src/jax_fdm.egg-info/top_level.txt
```

### Comparing `jax_fdm-0.5.2/CHANGELOG.md` & `jax_fdm-0.6.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.6.0] 2023-04-30
+
+### Added
+
+Support for differentiable CPU sparse solver
+- Added support for differentiable CPU and GPU sparse solvers to compute the XYZ coordinates of the free nodes with FDM. The solver is custom made and registered via a `jax.custom_vjp`. The forward and backward passes of the sparse solver were made possible thanks to the contributions of @denizokt. This solver lives in `equilibrium.sparse.py`.
+- Added `spsolve_gpu` and `spsolve_cpu`. The sparse solver backend is different (the former uses CUDA and the latter scipy) and it gets selected automatically based on what the value of `jax.default_device` is at runtime with function `register_sparse_solver`.
+- Implemented `EquilibriumStructureSparse`.
+- Division of responsabilities: created a `EquilibriumModelSparse` that solves for static equilibrium using an `EquilibriumStructureSparse` and the sparse solver. `EquilibriumModel` implements the dense linear solver.
+
+### Changed
+
+- `LossPlotter` instantiates a dense `EquilibriumModel`.
+
+### Removed
+
+
 ## [0.5.2] 2023-03-15
 
 ### Added
 
 ### Changed
 
 ### Removed
```

### Comparing `jax_fdm-0.5.2/LICENSE` & `jax_fdm-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/PKG-INFO` & `jax_fdm-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_fdm
-Version: 0.5.2
+Version: 0.6.0
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
@@ -187,16 +187,16 @@
 ## Citation
 
 If you found this library to be useful in academic or industry work, please consider 1) starring the project on Github, and 2) citing it:
 
 ```bibtex
 @software{pastrana_jaxfdm,
           title={{JAX~FDM}: Auto-differentiable and hardware-accelerated force density method},
-          author={Rafael Pastrana and Sigrid Adriaenssens},
-          year={2022},
+          author={Rafael Pastrana and Deniz Oktay and Ryan Adams and Sigrid Adriaenssens},
+          year={2023},
           doi={10.5281/zenodo.7258292},
           url={https://github.com/arpastrana/jax\_fdm}}
 ```
 
 ## Acknowledgements
 
 This work has been supported by the **U.S. National Science Foundation** under grant **OAC-2118201** and the [Institute for Data Driven Dynamical Design](https://www.mines.edu/id4/).
```

### Comparing `jax_fdm-0.5.2/README.md` & `jax_fdm-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,16 @@
 ## Citation
 
 If you found this library to be useful in academic or industry work, please consider 1) starring the project on Github, and 2) citing it:
 
 ```bibtex
 @software{pastrana_jaxfdm,
           title={{JAX~FDM}: Auto-differentiable and hardware-accelerated force density method},
-          author={Rafael Pastrana and Sigrid Adriaenssens},
-          year={2022},
+          author={Rafael Pastrana and Deniz Oktay and Ryan Adams and Sigrid Adriaenssens},
+          year={2023},
           doi={10.5281/zenodo.7258292},
           url={https://github.com/arpastrana/jax\_fdm}}
 ```
 
 ## Acknowledgements
 
 This work has been supported by the **U.S. National Science Foundation** under grant **OAC-2118201** and the [Institute for Data Driven Dynamical Design](https://www.mines.edu/id4/).
```

### Comparing `jax_fdm-0.5.2/setup.cfg` & `jax_fdm-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/setup.py` & `jax_fdm-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="jax_fdm",
-    version="0.5.2",
+    version="0.6.0",
     description="Auto-differentiable and hardware-accelerated force density method",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arpastrana/jax_fdm",
     author="Rafael Pastrana",
     author_email="arpastrana@princeton.edu",
     license="MIT license",
```

### Comparing `jax_fdm-0.5.2/src/jax_fdm/__init__.py` & `jax_fdm-0.6.0/src/jax_fdm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import jax.numpy as jnp
 
 
 __author__ = ["Rafael Pastrana"]
 __copyright__ = "Rafael Pastrana"
 __license__ = "MIT License"
 __email__ = "arpastrana@princeton.edu"
-__version__ = "0.5.2"
+__version__ = "0.6.0"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `jax_fdm-0.5.2/src/jax_fdm/constraints/constraint.py` & `jax_fdm-0.6.0/src/jax_fdm/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/constraints/edge/angle.py` & `jax_fdm-0.6.0/src/jax_fdm/constraints/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/constraints/node/coordinates.py` & `jax_fdm-0.6.0/src/jax_fdm/constraints/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/constraints/node/curvature.py` & `jax_fdm-0.6.0/src/jax_fdm/constraints/node/curvature.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/constraints/node/normal.py` & `jax_fdm-0.6.0/src/jax_fdm/constraints/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/constraints/node/tangent.py` & `jax_fdm-0.6.0/src/jax_fdm/constraints/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/datastructures.py` & `jax_fdm-0.6.0/src/jax_fdm/datastructures.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/equilibrium/fdm.py` & `jax_fdm-0.6.0/src/jax_fdm/equilibrium/fdm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,88 @@
 import numpy as np
 
 from jax_fdm import DTYPE_NP
 
 from jax_fdm.equilibrium import EquilibriumModel
+from jax_fdm.equilibrium import EquilibriumModelSparse
 
 
 # ==========================================================================
 # Form-finding
 # ==========================================================================
 
-def _fdm(network, q, xyz_fixed, loads):
+def _fdm(q, xyz_fixed, loads, model, network):
     """
     Compute a network in a state of static equilibrium using the force density method.
     """
-    model = EquilibriumModel(network)
-
     # compute static equilibrium
     eq_state = model(q, xyz_fixed, loads)
 
     # update equilibrium state in a copy of the network
     return network_updated(network, eq_state)
 
 
-def fdm(network):
+def fdm(network, sparse=True):
     """
     Compute a network in a state of static equilibrium using the force density method.
     """
     network_validate(network)
 
+    model = model_from_network(network, sparse)
     q, xyz_fixed, loads = (np.array(p, dtype=DTYPE_NP) for p in network.parameters())
 
-    return _fdm(network, q, xyz_fixed, loads)
+    return _fdm(q, xyz_fixed, loads, model, network)
 
 
 # ==========================================================================
 # Constrained form-finding
 # ==========================================================================
 
 def constrained_fdm(network,
                     optimizer,
                     loss,
                     parameters=None,
                     constraints=None,
                     maxiter=100,
                     tol=1e-6,
-                    callback=None):
+                    callback=None,
+                    sparse=True):
     """
     Generate a network in a constrained state of static equilibrium using the force density method.
     """
     network_validate(network)
 
-    model = EquilibriumModel(network)
+    if constraints and sparse:
+        print("Constraints are not supported yet for sparse inputs. Switching to dense.")
+        sparse = False
+
+    model = model_from_network(network, sparse)
 
     opt_problem = optimizer.problem(model, loss, parameters, constraints, maxiter, tol, callback)
     opt_params = optimizer.solve(opt_problem)
     q, xyz_fixed, loads = optimizer.parameters_fdm(opt_params)
 
-    return _fdm(network, q, xyz_fixed, loads)
+    return _fdm(q, xyz_fixed, loads, model, network)
 
 
 # ==========================================================================
 # Helpers
 # ==========================================================================
 
+def model_from_network(network, sparse):
+    """
+    Create an equilibrium model from a network.
+    """
+    model = EquilibriumModel
+    if sparse:
+        model = EquilibriumModelSparse
+
+    return model.from_network(network)
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

### Comparing `jax_fdm-0.5.2/src/jax_fdm/equilibrium/structure.py` & `jax_fdm-0.6.0/src/jax_fdm/equilibrium/structure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import numpy as np
+import jax.numpy as jnp
 
 from compas.datastructures import network_find_cycles
 
 from compas.numerical import connectivity_matrix
 from compas.numerical import face_matrix
 
+from jax.experimental.sparse import BCOO
+
 
 # ==========================================================================
 # Structure
 # ==========================================================================
 
 class EquilibriumStructure:
     """
@@ -18,14 +20,16 @@
         self._network = network
 
         self._connectivity = None
         self._connectivity_free = None
         self._connectivity_fixed = None
         self._connectivity_faces = None
 
+        self._connectivity_scipy = None
+
         self._edges = None
         self._nodes = None
         self._faces = None
 
         self._free_nodes = None
         self._fixed_nodes = None
         self._freefixed_nodes = None
@@ -106,52 +110,73 @@
         if not self._edge_index:
             self._edge_index = self.network.uv_index()
         return self._edge_index
 
     @property
     def connectivity(self):
         """
-        The connectivity of the network encoded as an incidence matrix.
+        The connectivity of the network encoded as an ncidence matrix.
         """
         if self._connectivity is None:
             node_idx = self.node_index
             edges = [(node_idx[u], node_idx[v]) for u, v in self.network.edges()]
-            self._connectivity = np.array(connectivity_matrix(edges, "list"), dtype=np.float64)
+
+            # NOTE: Dense array
+            # Currently there is a JAX bug that prevents us from using the sparse format with the connectivity matrix.
+            # When `todense()` is removed from the next line, we get the following error:
+            # TypeError: Value Zero(ShapedArray(float64[193,3])) with type <class 'jax._src.ad_util.Zero'> is not a valid JAX type
+
+            con = connectivity_matrix(edges, "array")
+            self._connectivity = jnp.asarray(con)
+
         return self._connectivity
 
     @property
-    def connectivity_faces(self):
+    def connectivity_scipy(self):
         """
-        The connectivity of the face cycles of a network encoded as as matrix.
+        The connectivity of the network encoded as an incidence matrix in CSC format.
         """
-        if self._connectivity_faces is None:
-            self._connectivity_faces = face_matrix(self.face_node_index, rtype="array")
-        return self._connectivity_faces
+        if self._connectivity_scipy is None:
+            node_idx = self.node_index
+            edges = [(node_idx[u], node_idx[v]) for u, v in self.network.edges()]
+            # We should get a CSC representation since we are interested in slicing columns
+            self._connectivity_scipy = connectivity_matrix(edges, "csc")
+
+        return self._connectivity_scipy
 
     @property
     def connectivity_fixed(self):
         """
         The connectivity of the fixed nodes of the network.
         """
         if self._connectivity_fixed is None:
-            fixed_nodes = self.fixed_nodes
-            self._connectivity_fixed = self.connectivity[:, fixed_nodes]
+            self._connectivity_fixed = self.connectivity[:, self.fixed_nodes]
+
         return self._connectivity_fixed
 
     @property
     def connectivity_free(self):
         """
         The connectivity of the free nodes of the network.
         """
         if self._connectivity_free is None:
-            free_nodes = self.free_nodes
-            self._connectivity_free = self.connectivity[:, free_nodes]
+            self._connectivity_free = self.connectivity[:, self.free_nodes]
+
         return self._connectivity_free
 
     @property
+    def connectivity_faces(self):
+        """
+        The connectivity of the face cycles of a network encoded as as matrix.
+        """
+        if self._connectivity_faces is None:
+            self._connectivity_faces = face_matrix(self.face_node_index, rtype="array")
+        return self._connectivity_faces
+
+    @property
     def free_nodes(self):
         """
         Returns a list with the indices of the anchored nodes.
         """
         if not self._free_nodes:
             self._free_nodes = [self.node_index[node] for node in self.network.nodes_free()]
         return self._free_nodes
@@ -165,18 +190,67 @@
             self._fixed_nodes = [self.node_index[node] for node in self.network.nodes_fixed()]
         return self._fixed_nodes
 
     @property
     def freefixed_nodes(self):
         """
         A list with the node keys of all the nodes sorted by their node index.
-        TODO: this method must be refactored to be more transparent.
         """
+        # TODO: this method must be refactored to be more transparent.
         if not self._freefixed_nodes:
-            freefixed_nodes = self.free_nodes + self._fixed_nodes
+            freefixed_nodes = self.free_nodes + self.fixed_nodes
             indices = {node: index for index, node in enumerate(freefixed_nodes)}
             sorted_indices = []
             for _, index in sorted(indices.items(), key=lambda item: item[0]):
                 sorted_indices.append(index)
             self._freefixed_nodes = tuple(sorted_indices)
 
         return self._freefixed_nodes
+
+
+# ==========================================================================
+# Structure
+# ==========================================================================
+
+class EquilibriumStructureSparse(EquilibriumStructure):
+    """
+    An equilibrium structure.
+    """
+    def __init__(self, network):
+        super().__init__(network)
+        self.init()
+
+    def init(self):
+        """
+        Warm start properties.
+
+        Otherwise we get a leakage error:
+
+        jax._src.errors.UnexpectedTracerError: Encountered an unexpected tracer.
+        A function transformed by JAX had a side effect, allowing for a reference to an
+        intermediate value with type float64[611] wrapped in a DynamicJaxprTracer
+        to escape the scope of the transformation.
+        """
+        self.connectivity_free
+        self.connectivity_fixed
+
+    @property
+    def connectivity_fixed(self):
+        """
+        The connectivity of the fixed nodes of the network.
+        """
+        if self._connectivity_fixed is None:
+            con_fixed = BCOO.from_scipy_sparse(self.connectivity_scipy[:, self.fixed_nodes])
+            self._connectivity_fixed = con_fixed
+
+        return self._connectivity_fixed
+
+    @property
+    def connectivity_free(self):
+        """
+        The connectivity of the free nodes of the network.
+        """
+        if self._connectivity_free is None:
+            con_free = BCOO.from_scipy_sparse(self.connectivity_scipy[:, self.free_nodes])
+            self._connectivity_free = con_free
+
+        return self._connectivity_free
```

### Comparing `jax_fdm-0.5.2/src/jax_fdm/geometry.py` & `jax_fdm-0.6.0/src/jax_fdm/geometry.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/abstract_goal.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/abstract_goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/edge/angle.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/edge/direction.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/edge/direction.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/edge/edge.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/edge/edge.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/edge/force.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/edge/force.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/edge/length.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/edge/length.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/goal.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/helpers.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/network/loadpath.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/network/loadpath.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/coordinates.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/line.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/line.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/node.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/node.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/normal.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/plane.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/plane.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/residual.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/residual.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/goals/node/tangent.py` & `jax_fdm-0.6.0/src/jax_fdm/goals/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/losses/errors.py` & `jax_fdm-0.6.0/src/jax_fdm/losses/errors.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/losses/loss.py` & `jax_fdm-0.6.0/src/jax_fdm/losses/loss.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/collections.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/collections.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/constrained.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/constrained.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/ipopt.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/ipopt.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/optimizer.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/optimizers.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/optimizers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/optimizers/second_order.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/optimizers/second_order.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/optimization/recorders.py` & `jax_fdm-0.6.0/src/jax_fdm/optimization/recorders.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/parameters/helpers.py` & `jax_fdm-0.6.0/src/jax_fdm/parameters/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/parameters/manager.py` & `jax_fdm-0.6.0/src/jax_fdm/parameters/manager.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/parameters/parameters.py` & `jax_fdm-0.6.0/src/jax_fdm/parameters/parameters.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/artists/network_artist.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/artists/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/network_artist.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/shapes.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/shapes.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/notebooks/viewer.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/notebooks/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/loss_plotter.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/loss_plotter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from time import time
+from functools import partial
 
 import matplotlib.pyplot as plt
 
 from jax import vmap
 import jax.numpy as jnp
 
 from jax_fdm import DTYPE_JAX
@@ -27,15 +28,16 @@
         """
         print("\nPlotting loss function...")
         start_time = time()
 
         q = jnp.asarray(history["q"], dtype=DTYPE_JAX)
         xyz_fixed = jnp.asarray(history["xyz_fixed"], dtype=DTYPE_JAX)
         loads = jnp.asarray(history["loads"], dtype=DTYPE_JAX)
-        eq_states = vmap(self.model)(q, xyz_fixed, loads)
+        model_dense = partial(self.model)
+        eq_states = vmap(model_dense)(q, xyz_fixed, loads)
 
         errors_all = []
         for error_term in self.loss.terms:
             errors = vmap(error_term)(eq_states)
             errors_all.append(errors)
             plt.plot(errors, label=error_term.name)
 
@@ -43,14 +45,15 @@
         plt.plot(losses, label=self.loss.name)
 
         plt.xlabel("Optimization iterations")
         plt.ylabel("Loss")
         plt.yscale("log")
         plt.grid()
         plt.legend()
+
         print(f"Plotting time: {(time() - start_time):.4} seconds")
 
     def show(self):
         """
         Display the plot.
         """
         plt.show()
```

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/plotters/network_artist.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/plotters/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/network_artist.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm/visualization/viewers/viewer.py` & `jax_fdm-0.6.0/src/jax_fdm/visualization/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.5.2/src/jax_fdm.egg-info/PKG-INFO` & `jax_fdm-0.6.0/src/jax_fdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-fdm
-Version: 0.5.2
+Version: 0.6.0
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
@@ -187,16 +187,16 @@
 ## Citation
 
 If you found this library to be useful in academic or industry work, please consider 1) starring the project on Github, and 2) citing it:
 
 ```bibtex
 @software{pastrana_jaxfdm,
           title={{JAX~FDM}: Auto-differentiable and hardware-accelerated force density method},
-          author={Rafael Pastrana and Sigrid Adriaenssens},
-          year={2022},
+          author={Rafael Pastrana and Deniz Oktay and Ryan Adams and Sigrid Adriaenssens},
+          year={2023},
           doi={10.5281/zenodo.7258292},
           url={https://github.com/arpastrana/jax\_fdm}}
 ```
 
 ## Acknowledgements
 
 This work has been supported by the **U.S. National Science Foundation** under grant **OAC-2118201** and the [Institute for Data Driven Dynamical Design](https://www.mines.edu/id4/).
```

### Comparing `jax_fdm-0.5.2/src/jax_fdm.egg-info/SOURCES.txt` & `jax_fdm-0.6.0/src/jax_fdm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/jax_fdm/constraints/node/curvature.py
 src/jax_fdm/constraints/node/node.py
 src/jax_fdm/constraints/node/normal.py
 src/jax_fdm/constraints/node/tangent.py
 src/jax_fdm/equilibrium/__init__.py
 src/jax_fdm/equilibrium/fdm.py
 src/jax_fdm/equilibrium/model.py
+src/jax_fdm/equilibrium/sparse.py
 src/jax_fdm/equilibrium/state.py
 src/jax_fdm/equilibrium/structure.py
 src/jax_fdm/goals/__init__.py
 src/jax_fdm/goals/abstract_goal.py
 src/jax_fdm/goals/goal.py
 src/jax_fdm/goals/helpers.py
 src/jax_fdm/goals/state.py
```

