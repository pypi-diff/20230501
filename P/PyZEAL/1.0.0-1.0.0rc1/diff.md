# Comparing `tmp/PyZEAL-1.0.0.tar.gz` & `tmp/PyZEAL-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyZEAL-1.0.0.tar", last modified: Mon May  1 20:51:20 2023, max compression
+gzip compressed data, was "PyZEAL-1.0.0rc1.tar", last modified: Thu Apr 27 16:02:44 2023, max compression
```

## Comparing `PyZEAL-1.0.0.tar` & `PyZEAL-1.0.0rc1.tar`

### file list

```diff
@@ -1,146 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.534153 PyZEAL-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    48728 2023-05-01 20:51:20.534153 PyZEAL-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.518153 PyZEAL-1.0.0/PyZEAL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48728 2023-05-01 20:51:20.000000 PyZEAL-1.0.0/PyZEAL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-01 20:51:20.000000 PyZEAL-1.0.0/PyZEAL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:51:20.000000 PyZEAL-1.0.0/PyZEAL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 20:51:20.000000 PyZEAL-1.0.0/PyZEAL.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 20:51:20.000000 PyZEAL-1.0.0/PyZEAL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 20:51:20.000000 PyZEAL-1.0.0/PyZEAL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.510153 PyZEAL-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.518153 PyZEAL-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/docs/_static/docstr_coverage_badge.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.518153 PyZEAL-1.0.0/pyzeal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.518153 PyZEAL-1.0.0/pyzeal/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.518153 PyZEAL-1.0.0/pyzeal/algorithms/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/estimators/argument_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/estimators/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/estimators/estimator_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/estimators/quad_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/estimators/sum_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/finder_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/newton_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/polynomial_holo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/simple_holo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/simple_holo_newton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.518153 PyZEAL-1.0.0/pyzeal/algorithms/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/wrappers/classical_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/algorithms/wrappers/polynomial_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.522153 PyZEAL-1.0.0/pyzeal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/cli_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/controller_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/parse_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/cli/parser_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.522153 PyZEAL-1.0.0/pyzeal/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.522153 PyZEAL-1.0.0/pyzeal/plugins/custom_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/plugins/custom_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/plugins/installation_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/plugins/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/plugins/pyzeal_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.522153 PyZEAL-1.0.0/pyzeal/pyzeal_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_logging/log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_logging/log_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_logging/loggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_logging/logger_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.522153 PyZEAL-1.0.0/pyzeal/pyzeal_types/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/algorithm_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/container_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/estimator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/filter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/init_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/parallel_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/root_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/pyzeal_types/settings_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.526153 PyZEAL-1.0.0/pyzeal/rootfinders/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/rootfinders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/rootfinders/finder_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/rootfinders/parallel_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/rootfinders/rootfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.526153 PyZEAL-1.0.0/pyzeal/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/core_settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/default_settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/invalid_setting_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/json_core_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/json_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/json_settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/ram_settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/settings_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/settings/settings_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.526153 PyZEAL-1.0.0/pyzeal/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.526153 PyZEAL-1.0.0/pyzeal/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/algorithms/test_associated_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/algorithms/test_newton_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/algorithms/test_simple_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/algorithms/test_simple_argument_newton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.526153 PyZEAL-1.0.0/pyzeal/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/benchmarks/newton_grid_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/benchmarks/simple_argument_newton_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/benchmarks/simple_argument_timings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.526153 PyZEAL-1.0.0/pyzeal/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/cli/test_json_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.530153 PyZEAL-1.0.0/pyzeal/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/containers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/containers/test_plain_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/containers/test_rounding_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.530153 PyZEAL-1.0.0/pyzeal/tests/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/estimators/test_quadrature_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/estimators/test_summation_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.530153 PyZEAL-1.0.0/pyzeal/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/resources/estimator_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/resources/finder_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/resources/finder_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/resources/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.530153 PyZEAL-1.0.0/pyzeal/tests/rootfinders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/rootfinders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_simple_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/tests/test_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.530153 PyZEAL-1.0.0/pyzeal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/configuration_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.534153 PyZEAL-1.0.0/pyzeal/utils/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/containers/plain_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/containers/root_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/containers/rounding_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:51:20.534153 PyZEAL-1.0.0/pyzeal/utils/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/factories/algorithm_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/factories/container_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/factories/estimator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/factories/settings_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/filter_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/finder_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/initialization_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/install_test_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/install_test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/lambda_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/root_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-01 20:51:08.000000 PyZEAL-1.0.0/pyzeal/utils/service_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:51:20.534153 PyZEAL-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    48722 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/PyZEAL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48722 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/pyzeal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/pyzeal/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/argument_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/estimator_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/quad_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/sum_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/finder_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/newton_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/polynomial_holo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/simple_holo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/simple_holo_newton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/cli_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/controller_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/parse_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/parser_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/plugins/custom_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/custom_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/installation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/pyzeal_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/log_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/loggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/logger_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/algorithm_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/container_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/estimator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/filter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/init_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/parallel_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/settings_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/rootfinders/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/finder_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/parallel_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/rootfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/core_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/default_settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/invalid_setting_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/json_core_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/json_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/json_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/ram_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/settings_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_associated_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_newton_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_simple_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_simple_argument_newton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/newton_grid_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/simple_argument_newton_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/simple_argument_timings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/cli/test_json_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/test_plain_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/test_rounding_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/test_quadrature_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/test_summation_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/estimator_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/finder_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/finder_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_simple_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/test_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/pyzeal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/configuration_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/pyzeal/utils/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/plain_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/root_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/rounding_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/pyzeal/utils/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/algorithm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/container_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/estimator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/settings_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/filter_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/finder_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/initialization_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/install_test_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/install_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/lambda_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/root_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/service_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/setup.cfg
```

### Comparing `PyZEAL-1.0.0/LICENSE` & `PyZEAL-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/PKG-INFO` & `PyZEAL-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyZEAL
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Python successor to the ZEAL package calculating zeros of holomorphic functions.
 Author-email: Philipp Schuette <pschuet2@mail.uni-paderborn.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,15 +695,15 @@
 The PyZEAL numerical project
 ============================
 
 .. |badge0| image:: ./docs/_static/docstr_coverage_badge.svg
    :target: https://pypi.org/project/docstr-coverage/
 
 .. |badge1| image:: https://img.shields.io/badge/Language-Python-blue.svg
-   :target: https://pypi.org/project/PyZEAL/
+   :target: https://www.python.org/
 
 .. |badge2| image:: http://img.shields.io/badge/benchmarked%20by-asv-blue.svg?style=flat
    :target: https://github.com/Spectral-Analysis-UPB/PyZEAL
 
 .. |badge3| image:: https://img.shields.io/github/v/release/Spectral-Analysis-UPB/PyZEAL
    :target: https://github.com/Spectral-Analysis-UPB/PyZEAL
```

### Comparing `PyZEAL-1.0.0/PyZEAL.egg-info/PKG-INFO` & `PyZEAL-1.0.0rc1/PyZEAL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyZEAL
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Python successor to the ZEAL package calculating zeros of holomorphic functions.
 Author-email: Philipp Schuette <pschuet2@mail.uni-paderborn.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,15 +695,15 @@
 The PyZEAL numerical project
 ============================
 
 .. |badge0| image:: ./docs/_static/docstr_coverage_badge.svg
    :target: https://pypi.org/project/docstr-coverage/
 
 .. |badge1| image:: https://img.shields.io/badge/Language-Python-blue.svg
-   :target: https://pypi.org/project/PyZEAL/
+   :target: https://www.python.org/
 
 .. |badge2| image:: http://img.shields.io/badge/benchmarked%20by-asv-blue.svg?style=flat
    :target: https://github.com/Spectral-Analysis-UPB/PyZEAL
 
 .. |badge3| image:: https://img.shields.io/github/v/release/Spectral-Analysis-UPB/PyZEAL
    :target: https://github.com/Spectral-Analysis-UPB/PyZEAL
```

### Comparing `PyZEAL-1.0.0/PyZEAL.egg-info/SOURCES.txt` & `PyZEAL-1.0.0rc1/PyZEAL.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,28 @@
 pyproject.toml
 PyZEAL.egg-info/PKG-INFO
 PyZEAL.egg-info/SOURCES.txt
 PyZEAL.egg-info/dependency_links.txt
 PyZEAL.egg-info/entry_points.txt
 PyZEAL.egg-info/requires.txt
 PyZEAL.egg-info/top_level.txt
-docs/_static/docstr_coverage_badge.svg
 pyzeal/py.typed
 pyzeal/algorithms/__init__.py
 pyzeal/algorithms/constants.py
 pyzeal/algorithms/finder_algorithm.py
 pyzeal/algorithms/newton_grid.py
 pyzeal/algorithms/polynomial_holo.py
 pyzeal/algorithms/simple_holo.py
 pyzeal/algorithms/simple_holo_newton.py
 pyzeal/algorithms/estimators/__init__.py
 pyzeal/algorithms/estimators/argument_estimator.py
 pyzeal/algorithms/estimators/constants.py
 pyzeal/algorithms/estimators/estimator_cache.py
 pyzeal/algorithms/estimators/quad_estimator.py
 pyzeal/algorithms/estimators/sum_estimator.py
-pyzeal/algorithms/wrappers/__init__.py
-pyzeal/algorithms/wrappers/classical_polynomial.py
-pyzeal/algorithms/wrappers/polynomial_wrapper.py
 pyzeal/cli/__init__.py
 pyzeal/cli/__main__.py
 pyzeal/cli/cli_controller.py
 pyzeal/cli/cli_parser.py
 pyzeal/cli/controller_facade.py
 pyzeal/cli/parse_results.py
 pyzeal/cli/parser_facade.py
@@ -60,15 +56,14 @@
 pyzeal/settings/core_settings_service.py
 pyzeal/settings/default_settings.json
 pyzeal/settings/invalid_setting_exception.py
 pyzeal/settings/json_core_settings.py
 pyzeal/settings/json_helper.py
 pyzeal/settings/json_settings_service.py
 pyzeal/settings/ram_settings_service.py
-pyzeal/settings/settings_schema.json
 pyzeal/settings/settings_service.py
 pyzeal/tests/__init__.py
 pyzeal/tests/test_locator.py
 pyzeal/tests/algorithms/__init__.py
 pyzeal/tests/algorithms/test_associated_polynomial.py
 pyzeal/tests/algorithms/test_newton_grid.py
 pyzeal/tests/algorithms/test_simple_argument.py
```

### Comparing `PyZEAL-1.0.0/README.rst` & `PyZEAL-1.0.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The PyZEAL numerical project
 ============================
 
 .. |badge0| image:: ./docs/_static/docstr_coverage_badge.svg
    :target: https://pypi.org/project/docstr-coverage/
 
 .. |badge1| image:: https://img.shields.io/badge/Language-Python-blue.svg
-   :target: https://pypi.org/project/PyZEAL/
+   :target: https://www.python.org/
 
 .. |badge2| image:: http://img.shields.io/badge/benchmarked%20by-asv-blue.svg?style=flat
    :target: https://github.com/Spectral-Analysis-UPB/PyZEAL
 
 .. |badge3| image:: https://img.shields.io/github/v/release/Spectral-Analysis-UPB/PyZEAL
    :target: https://github.com/Spectral-Analysis-UPB/PyZEAL
```

### Comparing `PyZEAL-1.0.0/pyproject.toml` & `PyZEAL-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyZEAL"
-version = "1.0.0"
+version = "1.0.0-rc1"
 authors = [
     {name = "Philipp Schuette", email = "pschuet2@mail.uni-paderborn.de"}
 ]
 description = "Python successor to the ZEAL package calculating zeros of holomorphic functions."
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/constants.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
 # numerical approximation of the discrete boundary between 0 and 2*pi
 TWO_PI: Final[float] = 0.8 * (2 * pi)
 # numerical approximation of the discrete boundary between 2*pi and 4*pi
 FOUR_PI: Final[float] = 0.65 * (4 * pi)
 
 # default values for argument estimation via phase summation
-DEFAULT_NUM_PTS: Final[int] = 6500
-DEFAULT_DELTA_PHI: Final[float] = 1e-2
-DEFAULT_MAX_PRECISION: Final[float] = 1e-10
+DEFAULT_NUM_PTS = 6500
+DEFAULT_DELTA_PHI = 0.01
+DEFAULT_MAX_PRECISION = 1e-10
 
-# cutoff for polynomial construction (at most 6*pi)
-MAX_PHASE: Final[float] = 0.85 * (8 * pi)
+# cutoff for polynomial construction
+MAXIMUM_PHASE_MULTIPLIER: Final[int] = 2
```

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/estimators/argument_estimator.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/argument_estimator.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/estimators/constants.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/constants.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/estimators/estimator_cache.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/estimator_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,17 @@
         :param argument: Total argument change
         """
         if (orderCache := self._cache.get(order, None)) is None:
             self._cache[order] = {(zStart, zEnd): argument}
         else:
             orderCache[(zStart, zEnd)] = argument
         self.logger.debug(
-            "stored value %s under key (%s, %d) in estimator cache!",
+            "stored value %s under key %s in estimator cache!",
             str(argument),
             str((order, (zStart, zEnd))),
-            order,
         )
 
     def retrieve(
         self,
         order: int,
         zStart: complex,
         zEnd: complex,
```

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/estimators/quad_estimator.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/quad_estimator.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/estimators/sum_estimator.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/sum_estimator.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/finder_algorithm.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/finder_algorithm.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/newton_grid.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/newton_grid.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/polynomial_holo.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/polynomial_holo.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 derivative using Newton's identities. Our implementation follows the original
 ideas of [Delves, Lyness].
 
 Authors:\n
 - Philipp Schuette\n
 """
 
-from typing import List, Tuple
+from typing import Tuple
 
 import numpy as np
 
-from pyzeal.algorithms.constants import MAX_PHASE, TWO_PI
+from pyzeal.algorithms.constants import FOUR_PI, TWO_PI
 from pyzeal.algorithms.simple_holo import SimpleArgumentAlgorithm
-from pyzeal.algorithms.wrappers.classical_polynomial import ClassicalPolynomial
 from pyzeal.utils.root_context import RootContext
 
 
 class AssociatedPolynomialAlgorithm(SimpleArgumentAlgorithm):
     """
     Class representation of a root finding algorithm which uses numerical
     quadrature to calculate higher moments. Then Newton's identities can be
@@ -65,67 +64,28 @@
             SimpleArgumentAlgorithm.getRootFromRectangle(
                 x2, x1, y2, y1, phi, context
             )
             return
 
         # check if the current box contains sufficiently few roots to construct
         # an associated polynomial with stable coefficients/roots
-        if TWO_PI < phi < MAX_PHASE:
-            degree = int(round(phi / (2 * np.pi), 0))
+        if TWO_PI < phi < FOUR_PI:
             self.logger.debug(
-                "constructing associated poly of degree %d from moments!",
-                degree,
+                "constructing Newton polynomials from higher moments!"
             )
 
-            # store higher moments for associated polynomial construction
-            moments: List[complex] = []
-            for order in range(1, degree + 1):
-                moment = self.estimator.calcMoment(
-                    order=order,
-                    reRan=(x1, x2),
-                    imRan=(y1, y2),
-                    context=context,
-                )
-                moments.append(moment / (2 * np.pi))
-
-            roots, orders = ClassicalPolynomial(
-                coefficients=self.coefficientsFromMoments(moments)
-            ).getRootsWithOrders(precision=context.precision)
-
-            for newRoot, newOrder in zip(roots, orders):
-                context.container.addRoot(
-                    (newRoot, newOrder), context.toFilterContext()
-                )
+            firstMoment = self.estimator.calcMoment(
+                order=1, reRan=(x1, x2), imRan=(y1, y2), context=context
+            )
+            newRoot = firstMoment / (2 * np.pi)
+            context.container.addRoot(
+                (newRoot, int(np.round(phi / (2 * np.pi)))),
+                context.toFilterContext(),
+            )
 
             if context.progress is not None and context.task is not None:
                 context.progress.update(
                     context.task, advance=deltaRe * deltaIm
                 )
             return
 
         super().decideRefinement((x1, x2), (y1, y2), phi, context)
-
-    def coefficientsFromMoments(self, moments: List[complex]) -> List[complex]:
-        """
-        Calculate the coefficients of the associated polynomial from the higher
-        moments (=power sums of roots) using Newton's identities.
-
-        :param moments: moments/power sums of roots
-        :returns: coefficients of the associated polynomial
-        """
-        coefficients: List[complex] = [1]
-        for k in range(1, len(moments) + 1):
-            temp: complex = 0
-            tempSign = 1
-
-            for i in range(1, k + 1):
-                temp += tempSign * coefficients[-i] * moments[i - 1]
-                tempSign *= -1
-            coefficients.append(temp / k)
-        # correct signs in the coefficients just calculated
-        sign = 1
-        for i, _ in enumerate(coefficients):
-            coefficients[i] *= sign
-            sign *= -1
-        coefficients.reverse()
-
-        return coefficients
```

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/simple_holo.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/simple_holo.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/algorithms/simple_holo_newton.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/simple_holo_newton.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             SimpleArgumentAlgorithm.getRootFromRectangle(
                 x2, x1, y2, y1, phi, context
             )
             return
 
         # check if the current box contains a simple root - Newton's algorithm
         # does not perform well enough to start within large rectangles
+        # TODO: keep on refining if Newton's algorithm finds no (valid) root!
         if TWO_PI < phi < FOUR_PI and deltaRe < 0.1 and deltaIm < 0.1:
             try:
                 self.logger.debug(
                     "starting Newton algorithm from %f+%fj", x1, (y1 + y2) / 2
                 )
                 newRoot = newton(
                     func=context.f,
```

### Comparing `PyZEAL-1.0.0/pyzeal/cli/__main__.py` & `PyZEAL-1.0.0rc1/pyzeal/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/cli/cli_controller.py` & `PyZEAL-1.0.0rc1/pyzeal/cli/cli_controller.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/cli/cli_parser.py` & `PyZEAL-1.0.0rc1/pyzeal/cli/cli_parser.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/cli/controller_facade.py` & `PyZEAL-1.0.0rc1/pyzeal/cli/controller_facade.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/cli/parse_results.py` & `PyZEAL-1.0.0rc1/pyzeal/cli/parse_results.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/cli/parser_facade.py` & `PyZEAL-1.0.0rc1/pyzeal/cli/parser_facade.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/plugins/installation_helper.py` & `PyZEAL-1.0.0rc1/pyzeal/plugins/installation_helper.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/plugins/plugin_loader.py` & `PyZEAL-1.0.0rc1/pyzeal/plugins/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/plugins/pyzeal_plugin.py` & `PyZEAL-1.0.0rc1/pyzeal/plugins/pyzeal_plugin.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_logging/log_levels.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/log_levels.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_logging/log_manager.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/log_manager.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_logging/loggable.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/loggable.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_logging/logger_facade.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/logger_facade.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_types/algorithm_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/algorithm_types.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_types/filter_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/filter_types.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_types/parallel_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/parallel_types.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/pyzeal_types/root_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/root_types.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/rootfinders/__init__.py` & `PyZEAL-1.0.0rc1/pyzeal/rootfinders/__init__.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/rootfinders/finder_interface.py` & `PyZEAL-1.0.0rc1/pyzeal/rootfinders/finder_interface.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/rootfinders/parallel_finder.py` & `PyZEAL-1.0.0rc1/pyzeal/rootfinders/parallel_finder.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/rootfinders/rootfinder.py` & `PyZEAL-1.0.0rc1/pyzeal/rootfinders/rootfinder.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/settings/core_settings_service.py` & `PyZEAL-1.0.0rc1/pyzeal/settings/core_settings_service.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/settings/json_core_settings.py` & `PyZEAL-1.0.0rc1/pyzeal/settings/json_core_settings.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/settings/json_helper.py` & `PyZEAL-1.0.0rc1/pyzeal/settings/json_helper.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/settings/json_settings_service.py` & `PyZEAL-1.0.0rc1/pyzeal/settings/json_settings_service.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/settings/ram_settings_service.py` & `PyZEAL-1.0.0rc1/pyzeal/settings/ram_settings_service.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/settings/settings_service.py` & `PyZEAL-1.0.0rc1/pyzeal/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/algorithms/test_associated_polynomial.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_associated_polynomial.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,31 +31,29 @@
 )
 
 # some test functions do not work due to z-refinement limitations
 KNOWN_FAILURES = ["x^100", "1e6 * x^100"]
 
 
 @pytest.mark.parametrize("testName", sorted(testFunctions.keys()))
-def testAssociatedPolynomial(testName: str) -> None:
+def testSimpleArgument(testName: str) -> None:
     """
-    Test the ASSOCIATED_POLYNOMIAL algorithm with the test case given by
-    `testName`.
+    Test the SIMPLE_ARGUMENT algorithm with the test case given by `testName`.
 
     :param testName: Name of the test case
     """
     if testName in KNOWN_FAILURES:
         pytest.skip()
 
     # initialize the algorithm under test
-    associatedPolynomialAlgo = AssociatedPolynomialAlgorithm(
+    simpleArgumentAlgo = AssociatedPolynomialAlgorithm(
         estimatorType=EstimatorTypes.QUADRATURE_ESTIMATOR
     )
-    precision = testFunctions[testName].precision
-    if testName in {"x^3-0.01x", "x^4-6.25x+9", "sin x cos"}:
-        precision = (2, 2)
 
     context = buildContextFromData(testFunctions[testName])
-    associatedPolynomialAlgo.calcRoots(context)
+    simpleArgumentAlgo.calcRoots(context)
     foundRoots = context.container.getRoots()  # pylint: disable=E1111
     expectedRoots = np.array(testFunctions[testName].expectedRoots)
 
-    assert rootsMatchClosely(foundRoots, expectedRoots, precision=precision)
+    assert rootsMatchClosely(
+        foundRoots, expectedRoots, precision=testFunctions[testName].precision
+    )
```

### Comparing `PyZEAL-1.0.0/pyzeal/tests/algorithms/test_newton_grid.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_newton_grid.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/algorithms/test_simple_argument.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_simple_argument.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/algorithms/test_simple_argument_newton.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_simple_argument_newton.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/benchmarks/newton_grid_timings.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/newton_grid_timings.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/benchmarks/simple_argument_newton_timings.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/simple_argument_newton_timings.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/benchmarks/simple_argument_timings.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/simple_argument_timings.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/cli/test_cli.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/cli/test_json_helper.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/cli/test_json_helper.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/containers/conftest.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/containers/conftest.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/containers/test_plain_container.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/containers/test_plain_container.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/containers/test_rounding_container.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/containers/test_rounding_container.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/estimators/test_quadrature_estimator.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/estimators/test_quadrature_estimator.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/estimators/test_summation_estimator.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/estimators/test_summation_estimator.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/resources/estimator_resources.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/resources/estimator_resources.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/resources/finder_helpers.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/resources/finder_helpers.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/resources/finder_test_cases.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/resources/finder_test_cases.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     """
     Convenience function building a root finding context from given test data.
 
     :param data: the data used for context building
     """
     # build a simple container for the context
     container = RoundingContainer(precision=data.precision)
-    # ContainerFactory.registerPreDefinedFilter(
-    #     container, filterType=FilterTypes.FUNCTION_VALUE_ZERO
-    # )
+    ContainerFactory.registerPreDefinedFilter(
+        container, filterType=FilterTypes.FUNCTION_VALUE_ZERO
+    )
     ContainerFactory.registerPreDefinedFilter(
         container, filterType=FilterTypes.ZERO_IN_BOUNDS
     )
 
     # assemble the context from the data
     deltaRe, deltaIm = data.precision
     reRan, imRan = data.reRan, data.imRan
@@ -269,17 +269,17 @@
             np.pi,
             -np.pi,
             0.5 * np.pi,
             1.5 * np.pi,
             -0.5 * np.pi,
             -1.5 * np.pi,
         ),
-        (-5.0001, 5.0102),
-        (-5.0003, 5.0204),
-        precision=(4, 4),
+        (-5, 5.01),
+        (-5, 5.02),
+        precision=(3, 3),
     ),
     "log and sinh composition": TestData(
         lambda x: cast(tVec, np.log(np.sinh(0.2 * x) ** 2 + 1)),
         lambda x: cast(
             tVec,
             0.4
             * np.sinh(0.2 * x)
@@ -287,30 +287,24 @@
             / (1 + np.sinh(0.2 * x) ** 2),
         ),
         (0,),
         (-5, 5),
         (-5, 5),
         precision=(3, 3),
     ),
-    "scaled exp": TestData(
-        lambda x: cast(tVec, np.exp(np.pi * x) - 1),
-        lambda x: cast(tVec, np.pi * np.exp(np.pi * x)),
-        (-2j, 0, 2j),
-        (-3, 3),
-        (-3, 3),
+    "square root of exp": TestData(
+        lambda x: cast(tVec, np.emath.sqrt(np.exp(2 * np.pi * x / 4)) - 1),
+        lambda x: cast(
+            tVec, 0.25 * np.pi / np.emath.sqrt(np.exp(2 * np.pi * x / 4))
+        ),
+        (0, -4j, 4j),
+        (-5, 5),
+        (-5, 5),
         precision=(3, 3),
     ),
-    "moved root": TestData(
-        lambda x: cast(tVec, np.emath.sqrt(x - 10)),
-        lambda x: cast(tVec, 0.5 / np.emath.sqrt(x - 10)),
-        (),
-        (-6, 6),
-        (-3, 7),
-        precision=(5, 5),
-    ),
     "log(x^2+26)": TestData(
         lambda x: cast(tVec, np.log(x**2 + 26)),
         lambda x: cast(tVec, 2 * x / (x**2 + 26)),
         (-5j, 5j),
         (-5.01, 5.02),
         (-5.03, 5.04),
         precision=(3, 3),
```

### Comparing `PyZEAL-1.0.0/pyzeal/tests/resources/utils.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/resources/utils.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_grid.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     if testName in KNOWN_FAILURES:
         pytest.skip()
 
     gridRF = newtonGridFinder(testName, numSamplePoints=30, parallel=parallel)
     reRan = testFunctions[testName].reRan
     imRan = testFunctions[testName].imRan
     precision = testFunctions[testName].precision
-
     if testName == "exp(x)-1":
         precision = (2, 2)
-
     gridRF.calculateRoots(reRan, imRan, precision=precision)
     foundRoots = np.sort_complex(gridRF.roots)
     expectedRoots = np.array(testFunctions[testName].expectedRoots)
 
     assert rootsMatchClosely(foundRoots, expectedRoots, precision=precision)
```

### Comparing `PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_hypothesis.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_hypothesis.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_simple.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_simple.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/rootfinders/test_finder_simple_newton.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_simple_newton.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/tests/test_locator.py` & `PyZEAL-1.0.0rc1/pyzeal/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/configuration_exception.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/configuration_exception.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/containers/plain_container.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/containers/plain_container.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/containers/root_container.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/containers/root_container.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/containers/rounding_container.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/containers/rounding_container.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/factories/algorithm_factory.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/factories/algorithm_factory.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/factories/container_factory.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/factories/container_factory.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/factories/estimator_factory.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/factories/estimator_factory.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/factories/settings_factory.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/factories/settings_factory.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/filter_context.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/filter_context.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/finder_progress.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/finder_progress.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/initialization_handler.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/initialization_handler.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/install_test_facade.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/install_test_facade.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/install_test_handler.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/install_test_handler.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/lambda_wrapper.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/lambda_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/root_context.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/root_context.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-1.0.0/pyzeal/utils/service_locator.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/service_locator.py`

 * *Files identical despite different names*

