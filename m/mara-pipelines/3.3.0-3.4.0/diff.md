# Comparing `tmp/mara-pipelines-3.3.0.tar.gz` & `tmp/mara-pipelines-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mara-pipelines-3.3.0.tar", last modified: Thu Sep 22 07:16:11 2022, max compression
+gzip compressed data, was "mara-pipelines-3.4.0.tar", last modified: Mon May  1 19:53:02 2023, max compression
```

## Comparing `mara-pipelines-3.3.0.tar` & `mara-pipelines-3.4.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.942332 mara-pipelines-3.3.0/
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1061 2022-05-19 12:28:30.000000 mara-pipelines-3.3.0/LICENSE
--rw-r--r--   0 lschick   (1000) lschick   (1000)     7371 2022-09-22 07:16:11.942332 mara-pipelines-3.3.0/PKG-INFO
--rw-r--r--   0 lschick   (1000) lschick   (1000)     7061 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/README.md
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.922332 mara-pipelines-3.3.0/mara_pipelines/
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)     1015 2022-09-22 07:11:59.000000 mara-pipelines-3.3.0/mara_pipelines/__init__.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.932332 mara-pipelines-3.3.0/mara_pipelines/commands/
--rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/commands/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)      739 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/commands/bash.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     8331 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/mara_pipelines/commands/files.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     4527 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/commands/python.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)    22686 2022-09-22 07:06:50.000000 mara-pipelines-3.3.0/mara_pipelines/commands/sql.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3329 2022-09-19 06:33:26.000000 mara-pipelines-3.3.0/mara_pipelines/config.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1008 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/events.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)    25103 2022-09-19 06:33:26.000000 mara-pipelines-3.3.0/mara_pipelines/execution.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.932332 mara-pipelines-3.3.0/mara_pipelines/incremental_processing/
--rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/incremental_processing/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3794 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/incremental_processing/file_dependencies.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2908 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/incremental_processing/incremental_copy_status.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2044 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/incremental_processing/processed_files.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1280 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/incremental_processing/reset.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.932332 mara-pipelines-3.3.0/mara_pipelines/logging/
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)       71 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/logging/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3069 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/logging/logger.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3408 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/logging/node_cost.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     5142 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/logging/pipeline_events.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     9525 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/mara_pipelines/logging/run_log.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     4130 2022-09-19 06:33:26.000000 mara-pipelines-3.3.0/mara_pipelines/logging/system_statistics.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.932332 mara-pipelines-3.3.0/mara_pipelines/notification/
--rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/notification/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2348 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/notification/notifier.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3153 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/notification/slack.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3460 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/notification/teams.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.942332 mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/
--rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)    15107 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/files.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3664 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/python.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3315 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/sql.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)    12007 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/pipelines.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2783 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/shell.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.942332 mara-pipelines-3.3.0/mara_pipelines/ui/
--rw-r--r--   0 lschick   (1000) lschick   (1000)      167 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     5953 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/cli.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     5638 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/mara_pipelines/ui/dependency_graph.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     8763 2022-09-19 06:33:26.000000 mara-pipelines-3.3.0/mara_pipelines/ui/last_runs.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     8825 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/node_page.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     5888 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/run_page.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1726 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/run_time_chart.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3702 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/run_time_chart.sql
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.942332 mara-pipelines-3.3.0/mara_pipelines/ui/static/
--rw-r--r--   0 lschick   (1000) lschick   (1000)      597 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/common.css
--rw-r--r--   0 lschick   (1000) lschick   (1000)     8934 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/kolorwheel.js
--rw-r--r--   0 lschick   (1000) lschick   (1000)      183 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/node-page.css
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3443 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/node-page.js
--rw-r--r--   0 lschick   (1000) lschick   (1000)      462 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/run-page.css
--rw-r--r--   0 lschick   (1000) lschick   (1000)     6246 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/run-page.js
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3933 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/run-time-chart.js
--rw-r--r--   0 lschick   (1000) lschick   (1000)     4294 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/system-stats-chart.js
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1394 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/timeline-chart.css
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3867 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/timeline-chart.js
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3621 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/static/utils.js
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)     1996 2022-07-13 18:46:56.000000 mara-pipelines-3.3.0/mara_pipelines/ui/views.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-22 07:16:11.922332 mara-pipelines-3.3.0/mara_pipelines.egg-info/
--rw-r--r--   0 lschick   (1000) lschick   (1000)     7371 2022-09-22 07:16:11.000000 mara-pipelines-3.3.0/mara_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2100 2022-09-22 07:16:11.000000 mara-pipelines-3.3.0/mara_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)        1 2022-09-22 07:16:11.000000 mara-pipelines-3.3.0/mara_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)      173 2022-09-22 07:16:11.000000 mara-pipelines-3.3.0/mara_pipelines.egg-info/requires.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)       15 2022-09-22 07:16:11.000000 mara-pipelines-3.3.0/mara_pipelines.egg-info/top_level.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)      108 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/pyproject.toml
--rw-r--r--   0 lschick   (1000) lschick   (1000)      706 2022-09-22 07:16:11.942332 mara-pipelines-3.3.0/setup.cfg
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)       37 2022-07-13 18:48:14.000000 mara-pipelines-3.3.0/setup.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1066 2023-02-26 10:28:04.000000 mara-pipelines-3.4.0/LICENSE
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     7728 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/PKG-INFO
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     7418 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/README.md
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.263240 mara-pipelines-3.4.0/mara_pipelines/
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)     1015 2023-05-01 19:51:18.000000 mara-pipelines-3.4.0/mara_pipelines/__init__.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/commands/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/commands/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      755 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/commands/bash.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)    12908 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/commands/files.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1293 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/commands/http.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     4551 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/commands/python.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)    22820 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/commands/sql.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3347 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/config.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      996 2023-02-26 10:28:04.000000 mara-pipelines-3.4.0/mara_pipelines/events.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)    25190 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/execution.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/incremental_processing/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/incremental_processing/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3775 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/incremental_processing/file_dependencies.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2859 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/incremental_processing/incremental_copy_status.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2014 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/incremental_processing/processed_files.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1286 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/incremental_processing/reset.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/logging/
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)       71 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/logging/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3097 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/logging/logger.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3455 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/logging/node_cost.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     5260 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/logging/pipeline_events.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     9160 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/logging/run_log.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     4130 2023-02-26 10:28:04.000000 mara-pipelines-3.4.0/mara_pipelines/logging/system_statistics.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/notification/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/notification/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2390 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/notification/notifier.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3181 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/notification/slack.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3488 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/notification/teams.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        0 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)    15370 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/files.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3774 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/python.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3456 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/sql.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)    12192 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/pipelines.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3947 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/shell.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/ui/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      167 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/ui/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     5979 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/ui/cli.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     5666 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/ui/dependency_graph.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     8497 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/ui/last_runs.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     8825 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/ui/node_page.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     5888 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/ui/run_page.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1640 2023-05-01 18:56:07.000000 mara-pipelines-3.4.0/mara_pipelines/ui/run_time_chart.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3701 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/run_time_chart.sql
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/mara_pipelines/ui/static/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      598 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/common.css
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     8935 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/kolorwheel.js
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      183 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/node-page.css
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3439 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/node-page.js
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      460 2023-05-01 19:51:50.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/run-page.css
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     6247 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/run-page.js
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3931 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/run-time-chart.js
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     4293 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/system-stats-chart.js
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1395 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/timeline-chart.css
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3865 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/timeline-chart.js
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3620 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/mara_pipelines/ui/static/utils.js
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)     1996 2022-07-13 18:46:56.000000 mara-pipelines-3.4.0/mara_pipelines/ui/views.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.263240 mara-pipelines-3.4.0/mara_pipelines.egg-info/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     7728 2023-05-01 19:53:02.000000 mara-pipelines-3.4.0/mara_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2163 2023-05-01 19:53:02.000000 mara-pipelines-3.4.0/mara_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        1 2023-05-01 19:53:02.000000 mara-pipelines-3.4.0/mara_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      245 2023-05-01 19:53:02.000000 mara-pipelines-3.4.0/mara_pipelines.egg-info/requires.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       15 2023-05-01 19:53:02.000000 mara-pipelines-3.4.0/mara_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      184 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/pyproject.toml
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      782 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/setup.cfg
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)       38 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/setup.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:53:02.273240 mara-pipelines-3.4.0/tests/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1818 2023-05-01 18:56:10.000000 mara-pipelines-3.4.0/tests/test_execute_pipeline.py
```

### Comparing `mara-pipelines-3.3.0/LICENSE` & `mara-pipelines-3.4.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017 Mara contributors
+Copyright (c) 2017-2022 Mara contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mara-pipelines-3.3.0/PKG-INFO` & `mara-pipelines-3.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mara-pipelines
-Version: 3.3.0
+Version: 3.4.0
 Summary: Opinionated lightweight ELT pipeline framework
 Home-page: https://github.com/mara/mara-pipelines
 Author: Mara contributors
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Mara Pipelines
 
 [![Build & Test](https://github.com/mara/mara-pipelines/actions/workflows/build.yaml/badge.svg)](https://github.com/mara/mara-pipelines/actions/workflows/build.yaml)
-[![PyPI - License](https://img.shields.io/pypi/l/mara-pipelines.svg)](https://github.com/mara/mara-pipelines/blob/master/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/mara-pipelines.svg)](https://github.com/mara/mara-pipelines/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/mara-pipelines.svg)](https://badge.fury.io/py/mara-pipelines)
 [![Slack Status](https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social)](https://communityinviter.com/apps/mara-users/public-invite)
 
 
 
 This package contains a lightweight data transformation framework with a focus on transparency and complexity reduction. It has a number of baked-in assumptions/ principles:
 
@@ -42,22 +42,22 @@
 To use the library directly, use pip:
 
 ```
 pip install mara-pipelines
 ```
 
 or
- 
+
 ```
 pip install git+https://github.com/mara/mara-pipelines.git
 ```
 
 For an example of an integration into a flask application, have a look at the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2).
 
-Due to the heavy use of forking, Mara Pipelines does not run natively on Windows. If you want to run it on Windows, then please use Docker or the [Windows Subsystem for Linux](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux). 
+Due to the heavy use of forking, Mara Pipelines does not run natively on Windows. If you want to run it on Windows, then please use Docker or the [Windows Subsystem for Linux](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux).
 
 &nbsp;
 
 ## Example
 
 Here is a pipeline "demo" consisting of three nodes that depend on each other: the task `ping_localhost`, the pipeline `sub_pipeline` and the task `sleep`:
 
@@ -85,19 +85,19 @@
 
 pipeline.add(sub_pipeline, ['ping_localhost'])
 
 pipeline.add(Task(id='sleep', description='Sleeps for 2 seconds',
                   commands=[RunBash('sleep 2')]), ['sub_pipeline'])
 ```
 
-Tasks contain lists of commands, which do the actual work (in this case running bash commands that ping various hosts). 
+Tasks contain lists of commands, which do the actual work (in this case running bash commands that ping various hosts).
 
 &nbsp;
 
-In order to run the pipeline, a PostgreSQL database needs to be configured for storing run-time information, run output and status of incremental processing: 
+In order to run the pipeline, a PostgreSQL database is recommended to be configured for storing run-time information, run output and status of incremental processing:
 
 ```python
 import mara_db.auto_migration
 import mara_db.config
 import mara_db.dbs
 
 mara_db.config.databases \
@@ -108,18 +108,18 @@
 
 Given that PostgresSQL is running and the credentials work, the output looks like this (a database with a number of tables is created):
 
 ```
 Created database "postgresql+psycopg2://root@localhost/example_etl_mara"
 
 CREATE TABLE data_integration_file_dependency (
-    node_path TEXT[] NOT NULL, 
-    dependency_type VARCHAR NOT NULL, 
-    hash VARCHAR, 
-    timestamp TIMESTAMP WITHOUT TIME ZONE, 
+    node_path TEXT[] NOT NULL,
+    dependency_type VARCHAR NOT NULL,
+    hash VARCHAR,
+    timestamp TIMESTAMP WITHOUT TIME ZONE,
     PRIMARY KEY (node_path, dependency_type)
 );
 
 .. more tables
 ```
 
 ### CLI UI
@@ -128,38 +128,38 @@
 
 ```python
 from mara_pipelines.ui.cli import run_pipeline
 
 run_pipeline(pipeline)
 ```
 
-![Example run cli 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-1.gif)
+![Example run cli 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-1.gif)
 
 &nbsp;
 
 And this runs a single node of pipeline `sub_pipeline` together with all the nodes that it depends on:
 
 ```python
 run_pipeline(sub_pipeline, nodes=[sub_pipeline.nodes['ping_amazon']], with_upstreams=True)
 ```
 
-![Example run cli 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-2.gif)
+![Example run cli 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-2.gif)
 
 &nbsp;
 
 
 And finally, there is some sort of menu based on [pythondialog](http://pythondialog.sourceforge.net/) that allows to navigate and run pipelines like this:
 
 ```python
 from mara_pipelines.ui.cli import run_interactively
 
 run_interactively()
 ```
 
-![Example run cli 3](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-3.gif)
+![Example run cli 3](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-3.gif)
 
 
 
 ### Web UI
 
 More importantly, this package provides an extensive web interface. It can be easily integrated into any [Flask](https://flask.palletsprojects.com/) based app and the [mara example project](https://github.com/mara/mara-example-project) demonstrates how to do this using [mara-app](https://github.com/mara/mara-app).
 
@@ -167,30 +167,36 @@
 
 - a graph of all child nodes and the dependencies between them
 - a chart of the overal run time of the pipeline and it's most expensive nodes over the last 30 days (configurable)
 - a table of all the pipeline's nodes with their average run times and the resulting queuing priority
 - output and timeline for the last runs of the pipeline
 
 
-![Mara pipelines web ui 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/mara-pipelines-web-ui-1.png)
+![Mara pipelines web ui 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/mara-pipelines-web-ui-1.png)
 
-For each task, there is a page showing 
+For each task, there is a page showing
 
 - the upstreams and downstreams of the task in the pipeline
 - the run times of the task in the last 30 days
 - all commands of the task
 - output of the last runs of the task
 
-![Mara pipelines web ui 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/mara-pipelines-web-ui-2.png)
+![Mara pipelines web ui 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/mara-pipelines-web-ui-2.png)
 
 
-Pipelines and tasks can be run from the web ui directly, which is probably one of the main features of this package: 
+Pipelines and tasks can be run from the web ui directly, which is probably one of the main features of this package:
 
-![Example run web ui](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-web-ui.gif)
+![Example run web ui](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-web-ui.gif)
 
 &nbsp;
 
-# Getting started
+## Getting started
 
-Documentation is currently work in progress. Please use the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2) as a reference for getting started. 
+Documentation is currently work in progress. Please use the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2) as a reference for getting started.
 
+## Links
 
+* Documentation: https://mara-pipelines.readthedocs.io/
+* Changes: https://mara-pipelines.readthedocs.io/en/latest/changes.html
+* PyPI Releases: https://pypi.org/project/mara-pipelines/
+* Source Code: https://github.com/mara/mara-pipelines
+* Issue Tracker: https://github.com/mara/mara-pipelines/issues
```

### Comparing `mara-pipelines-3.3.0/README.md` & `mara-pipelines-3.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Mara Pipelines
 
 [![Build & Test](https://github.com/mara/mara-pipelines/actions/workflows/build.yaml/badge.svg)](https://github.com/mara/mara-pipelines/actions/workflows/build.yaml)
-[![PyPI - License](https://img.shields.io/pypi/l/mara-pipelines.svg)](https://github.com/mara/mara-pipelines/blob/master/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/mara-pipelines.svg)](https://github.com/mara/mara-pipelines/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/mara-pipelines.svg)](https://badge.fury.io/py/mara-pipelines)
 [![Slack Status](https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social)](https://communityinviter.com/apps/mara-users/public-invite)
 
 
 
 This package contains a lightweight data transformation framework with a focus on transparency and complexity reduction. It has a number of baked-in assumptions/ principles:
 
@@ -30,22 +30,22 @@
 To use the library directly, use pip:
 
 ```
 pip install mara-pipelines
 ```
 
 or
- 
+
 ```
 pip install git+https://github.com/mara/mara-pipelines.git
 ```
 
 For an example of an integration into a flask application, have a look at the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2).
 
-Due to the heavy use of forking, Mara Pipelines does not run natively on Windows. If you want to run it on Windows, then please use Docker or the [Windows Subsystem for Linux](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux). 
+Due to the heavy use of forking, Mara Pipelines does not run natively on Windows. If you want to run it on Windows, then please use Docker or the [Windows Subsystem for Linux](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux).
 
 &nbsp;
 
 ## Example
 
 Here is a pipeline "demo" consisting of three nodes that depend on each other: the task `ping_localhost`, the pipeline `sub_pipeline` and the task `sleep`:
 
@@ -73,19 +73,19 @@
 
 pipeline.add(sub_pipeline, ['ping_localhost'])
 
 pipeline.add(Task(id='sleep', description='Sleeps for 2 seconds',
                   commands=[RunBash('sleep 2')]), ['sub_pipeline'])
 ```
 
-Tasks contain lists of commands, which do the actual work (in this case running bash commands that ping various hosts). 
+Tasks contain lists of commands, which do the actual work (in this case running bash commands that ping various hosts).
 
 &nbsp;
 
-In order to run the pipeline, a PostgreSQL database needs to be configured for storing run-time information, run output and status of incremental processing: 
+In order to run the pipeline, a PostgreSQL database is recommended to be configured for storing run-time information, run output and status of incremental processing:
 
 ```python
 import mara_db.auto_migration
 import mara_db.config
 import mara_db.dbs
 
 mara_db.config.databases \
@@ -96,18 +96,18 @@
 
 Given that PostgresSQL is running and the credentials work, the output looks like this (a database with a number of tables is created):
 
 ```
 Created database "postgresql+psycopg2://root@localhost/example_etl_mara"
 
 CREATE TABLE data_integration_file_dependency (
-    node_path TEXT[] NOT NULL, 
-    dependency_type VARCHAR NOT NULL, 
-    hash VARCHAR, 
-    timestamp TIMESTAMP WITHOUT TIME ZONE, 
+    node_path TEXT[] NOT NULL,
+    dependency_type VARCHAR NOT NULL,
+    hash VARCHAR,
+    timestamp TIMESTAMP WITHOUT TIME ZONE,
     PRIMARY KEY (node_path, dependency_type)
 );
 
 .. more tables
 ```
 
 ### CLI UI
@@ -116,38 +116,38 @@
 
 ```python
 from mara_pipelines.ui.cli import run_pipeline
 
 run_pipeline(pipeline)
 ```
 
-![Example run cli 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-1.gif)
+![Example run cli 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-1.gif)
 
 &nbsp;
 
 And this runs a single node of pipeline `sub_pipeline` together with all the nodes that it depends on:
 
 ```python
 run_pipeline(sub_pipeline, nodes=[sub_pipeline.nodes['ping_amazon']], with_upstreams=True)
 ```
 
-![Example run cli 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-2.gif)
+![Example run cli 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-2.gif)
 
 &nbsp;
 
 
 And finally, there is some sort of menu based on [pythondialog](http://pythondialog.sourceforge.net/) that allows to navigate and run pipelines like this:
 
 ```python
 from mara_pipelines.ui.cli import run_interactively
 
 run_interactively()
 ```
 
-![Example run cli 3](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-3.gif)
+![Example run cli 3](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-3.gif)
 
 
 
 ### Web UI
 
 More importantly, this package provides an extensive web interface. It can be easily integrated into any [Flask](https://flask.palletsprojects.com/) based app and the [mara example project](https://github.com/mara/mara-example-project) demonstrates how to do this using [mara-app](https://github.com/mara/mara-app).
 
@@ -155,30 +155,36 @@
 
 - a graph of all child nodes and the dependencies between them
 - a chart of the overal run time of the pipeline and it's most expensive nodes over the last 30 days (configurable)
 - a table of all the pipeline's nodes with their average run times and the resulting queuing priority
 - output and timeline for the last runs of the pipeline
 
 
-![Mara pipelines web ui 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/mara-pipelines-web-ui-1.png)
+![Mara pipelines web ui 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/mara-pipelines-web-ui-1.png)
 
-For each task, there is a page showing 
+For each task, there is a page showing
 
 - the upstreams and downstreams of the task in the pipeline
 - the run times of the task in the last 30 days
 - all commands of the task
 - output of the last runs of the task
 
-![Mara pipelines web ui 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/mara-pipelines-web-ui-2.png)
+![Mara pipelines web ui 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/mara-pipelines-web-ui-2.png)
 
 
-Pipelines and tasks can be run from the web ui directly, which is probably one of the main features of this package: 
+Pipelines and tasks can be run from the web ui directly, which is probably one of the main features of this package:
 
-![Example run web ui](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-web-ui.gif)
+![Example run web ui](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-web-ui.gif)
 
 &nbsp;
 
-# Getting started
+## Getting started
 
-Documentation is currently work in progress. Please use the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2) as a reference for getting started. 
+Documentation is currently work in progress. Please use the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2) as a reference for getting started.
 
+## Links
 
+* Documentation: https://mara-pipelines.readthedocs.io/
+* Changes: https://mara-pipelines.readthedocs.io/en/latest/changes.html
+* PyPI Releases: https://pypi.org/project/mara-pipelines/
+* Source Code: https://github.com/mara/mara-pipelines
+* Issue Tracker: https://github.com/mara/mara-pipelines/issues
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/__init__.py` & `mara-pipelines-3.4.0/mara_pipelines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Make the functionalities of this package auto-discoverable by mara-app"""
-__version__ = '3.3.0'
+__version__ = '3.4.0'
 
 
 def MARA_CONFIG_MODULES():
     from . import config
     return [config]
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/commands/files.py` & `mara-pipelines-3.4.0/mara_pipelines/commands/files.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Commands for reading files"""
 
 import json
 import pathlib
 import shlex
 import sys
+from typing import List, Tuple, Dict, Union, Callable, Optional
 
 import enum
 
 import mara_db.dbs
+from mara_db import formats
 import mara_db.shell
 from . import sql
 from mara_page import _, html
 from .. import config, pipelines
 
 
-class Compression(enum.EnumMeta):
+class Compression(enum.Enum):
     """Different compression formats that are understood by file readers"""
     NONE = 'none'
     GZIP = 'gzip'
     TAR_GZIP = 'tar.gzip'
     ZIP = 'zip'
 
 
@@ -31,148 +33,237 @@
 
 
 class ReadFile(pipelines.Command):
     """Reads data from a local file"""
 
     def __init__(self, file_name: str, compression: Compression, target_table: str,
                  mapper_script_file_name: str = None, make_unique: bool = False,
-                 db_alias: str = None, csv_format: bool = False, skip_header: bool = False,
+                 db_alias: str = None, csv_format: bool = None, skip_header: bool = None,
                  delimiter_char: str = None, quote_char: str = None,
-                 null_value_string: str = None, timezone: str = None) -> None:
+                 null_value_string: str = None, timezone: str = None,
+                 file_format: formats.Format = None) -> None:
+        """
+        Reads data from a local file
+
+        Args:
+            file_name: local file name under mara_pipelines.config.data_dir()
+            compression: the compression of the file. If none, use Compression.NONE
+            target_table: the target database table the data should be imported to
+            mapper_script_file_name: a mapper shell script receiving the file content
+                                     from stdin, sends new data to stdout for further
+                                     processing
+            make_unique: drop duplicated lines
+            db_alias: the db alias of the target table
+            csv_format: Treat the input as a CSV file
+            skip_header: When true, skip the first line
+            delimiter_char: The character that separates columns
+            quote_char: The character for quoting strings
+            null_value_string: The string that denotes NULL values
+            file_format: The format of the file.
+        """
         super().__init__()
+        formats._check_format_with_args_used(
+            pipe_format=file_format,
+            header=skip_header,
+            delimiter_char=delimiter_char,
+            csv_format=csv_format,
+            quote_char=quote_char,
+            null_value_string=null_value_string)
         self.file_name = file_name
         self.compression = compression
         self.mapper_script_file_name = mapper_script_file_name
         self.make_unique = make_unique
 
         self.target_table = target_table
         self.csv_format = csv_format
         self.skip_header = skip_header
         self._db_alias = db_alias
         self.delimiter_char = delimiter_char
         self.quote_char = quote_char
         self.null_value_string = null_value_string
         self.timezone = timezone
+        self.file_format = file_format
 
-    def db_alias(self):
+    def db_alias(self) -> str:
         return self._db_alias or config.default_db_alias()
 
-    def shell_command(self):
+    def shell_command(self) -> str:
         copy_from_stdin_command = mara_db.shell.copy_from_stdin_command(
             self.db_alias(), csv_format=self.csv_format, target_table=self.target_table,
             skip_header=self.skip_header,
             delimiter_char=self.delimiter_char, quote_char=self.quote_char,
-            null_value_string=self.null_value_string, timezone=self.timezone)
+            null_value_string=self.null_value_string, timezone=self.timezone,
+            pipe_format=self.file_format)
         if not isinstance(mara_db.dbs.db(self.db_alias()), mara_db.dbs.BigQueryDB):
             return \
                 f'{uncompressor(self.compression)} "{pathlib.Path(config.data_dir()) / self.file_name}" \\\n' \
                 + (f'  | {shlex.quote(sys.executable)} "{self.mapper_file_path()}" \\\n'
                    if self.mapper_script_file_name else '') \
                 + ('  | sort -u \\\n' if self.make_unique else '') \
                 + '  | ' + copy_from_stdin_command
         else:
             # Bigquery loading does not support streaming data through pipes
             return copy_from_stdin_command + f" {pathlib.Path(config.data_dir()) / self.file_name}"
 
-    def mapper_file_path(self):
+    def mapper_file_path(self) -> pathlib.Path:
         return self.parent.parent.base_path() / self.mapper_script_file_name
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('file name', _.i[self.file_name]),
                 ('compression', _.tt[self.compression]),
                 ('mapper script file name', _.i[self.mapper_script_file_name]),
                 (_.i['content'], html.highlight_syntax(self.mapper_file_path().read_text().strip('\n')
                                                        if self.mapper_script_file_name and self.mapper_file_path().exists()
                                                        else '', 'python')),
                 ('make unique', _.tt[self.make_unique]),
                 ('target_table', _.tt[self.target_table]),
                 ('db alias', _.tt[self.db_alias()]),
+                ('file format', _.tt[self.file_format]),
                 ('csv format', _.tt[self.csv_format]),
                 ('skip header', _.tt[self.skip_header]),
                 ('delimiter char',
-                 _.tt[json.dumps(self.delimiter_char) if self.delimiter_char != None else None]),
-                ('quote char', _.tt[json.dumps(self.quote_char) if self.quote_char != None else None]),
+                 _.tt[json.dumps(self.delimiter_char) if self.delimiter_char is not None else None]),
+                ('quote char', _.tt[json.dumps(self.quote_char) if self.quote_char is not None else None]),
                 ('null value string',
-                 _.tt[json.dumps(self.null_value_string) if self.null_value_string != None else None]),
+                 _.tt[json.dumps(self.null_value_string) if self.null_value_string is not None else None]),
                 ('time zone', _.tt[self.timezone]),
                 (_.i['shell command'], html.highlight_syntax(self.shell_command(), 'bash'))]
 
 
 class ReadSQLite(sql._SQLCommand):
     def __init__(self, sqlite_file_name: str, target_table: str,
-                 sql_statement: str = None, sql_file_name: str = None, replace: {str: str} = None,
+                 sql_statement: str = None, sql_file_name: str = None, replace: Dict[str, str] = None,
                  db_alias: str = None, timezone: str = None) -> None:
         sql._SQLCommand.__init__(self, sql_statement, sql_file_name, replace)
         self.sqlite_file_name = sqlite_file_name
 
         self.target_table = target_table
         self._db_alias = db_alias
         self.timezone = timezone
 
     @property
-    def db_alias(self):
+    def db_alias(self) -> str:
         return self._db_alias or config.default_db_alias()
 
-    def shell_command(self):
+    def shell_command(self) -> str:
         return (sql._SQLCommand.shell_command(self)
                 + '  | ' + mara_db.shell.copy_command(
-                    mara_db.dbs.SQLiteDB(file_name=config.data_dir().absolute() / self.sqlite_file_name),
+                    mara_db.dbs.SQLiteDB(file_name=pathlib.Path(config.data_dir()).absolute() / self.sqlite_file_name),
                     self.db_alias, self.target_table, timezone=self.timezone))
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('sqlite file name', _.i[self.sqlite_file_name])] \
                + sql._SQLCommand.html_doc_items(self, None) \
                + [('target_table', _.tt[self.target_table]),
                   ('db alias', _.tt[self.db_alias]),
                   ('time zone', _.tt[self.timezone]),
                   (_.i['shell command'], html.highlight_syntax(self.shell_command(), 'bash'))]
 
 
 class ReadScriptOutput(pipelines.Command):
     """Reads the output from a python script into a database table"""
 
     def __init__(self, file_name: str, target_table: str, make_unique: bool = False,
-                 db_alias: str = None, csv_format: bool = False, skip_header: bool = False,
+                 db_alias: str = None, csv_format: bool = None, skip_header: bool = None,
                  delimiter_char: str = None, quote_char: str = None,
-                 null_value_string: str = None, timezone: str = None) -> None:
+                 null_value_string: str = None, timezone: str = None,
+                 pipe_format: formats.Format = None) -> None:
         super().__init__()
+        formats._check_format_with_args_used(
+            pipe_format=pipe_format,
+            header=skip_header,
+            delimiter_char=delimiter_char,
+            csv_format=csv_format,
+            quote_char=quote_char,
+            null_value_string=null_value_string)
         self.file_name = file_name
         self.make_unique = make_unique
 
         self.target_table = target_table
         self.csv_format = csv_format
         self.skip_header = skip_header
         self._db_alias = db_alias
         self.delimiter_char = delimiter_char
         self.quote_char = quote_char
         self.null_value_string = null_value_string
         self.timezone = timezone
+        self.pipe_format = pipe_format
 
-    def db_alias(self):
+    def db_alias(self) -> str:
         return self._db_alias or config.default_db_alias()
 
-    def shell_command(self):
+    def shell_command(self) -> str:
         return f'{shlex.quote(sys.executable)} "{self.file_path()}" \\\n' \
                + ('  | sort -u \\\n' if self.make_unique else '') \
                + '  | ' + mara_db.shell.copy_from_stdin_command(
             self.db_alias(), csv_format=self.csv_format, target_table=self.target_table, skip_header=self.skip_header,
             delimiter_char=self.delimiter_char, quote_char=self.quote_char,
-            null_value_string=self.null_value_string, timezone=self.timezone)
+            null_value_string=self.null_value_string, timezone=self.timezone,
+            pipe_format=self.pipe_format)
 
-    def file_path(self):
+    def file_path(self) -> pathlib.Path:
         return self.parent.parent.base_path() / self.file_name
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('file name', _.i[self.file_name]),
                 (_.i['content'], html.highlight_syntax(self.file_path().read_text().strip('\n')
                                                        if self.file_name and self.file_path().exists()
                                                        else '', 'python')),
                 ('make unique', _.tt[self.make_unique]),
                 ('target_table', _.tt[self.target_table]),
                 ('db alias', _.tt[self.db_alias()]),
+                ('pipe format', _.tt[self.pipe_format])
                 ('delimiter char',
-                 _.tt[json.dumps(self.delimiter_char) if self.delimiter_char != None else None]),
-                ('quote char', _.tt[json.dumps(self.quote_char) if self.quote_char != None else None]),
+                 _.tt[json.dumps(self.delimiter_char) if self.delimiter_char is not None else None]),
+                ('quote char', _.tt[json.dumps(self.quote_char) if self.quote_char is not None else None]),
                 ('null value string',
-                 _.tt[json.dumps(self.null_value_string) if self.null_value_string != None else None]),
+                 _.tt[json.dumps(self.null_value_string) if self.null_value_string is not None else None]),
                 ('time zone', _.tt[self.timezone]),
                 (_.i['shell command'], html.highlight_syntax(self.shell_command(), 'bash'))]
+
+
+class WriteFile(sql._SQLCommand):
+    """Writes data to a local file. The command is executed on the shell."""
+
+    def __init__(self, dest_file_name: str, sql_statement: Optional[Union[Callable, str]] = None, sql_file_name: Optional[str] = None,
+                 replace: Optional[Dict[str, str]] = None, db_alias: Optional[str] = None,
+                 compression: Compression = Compression.NONE,
+                 format: formats.Format = formats.CsvFormat()) -> None:
+        """
+        Writes the output of a sql query to a file in a specific format. The command is executed on the shell.
+
+        Args:
+            dest_file_name: destination file name
+            sql_statement: The statement to run as a string
+            sql_file_name: The name of the file to run (relative to the directory of the parent pipeline)
+            replace: A set of replacements to perform against the sql query `{'replace`: 'with', ..}`
+            db_alias: db on which the SQL statement shall run
+            storage_alias: storage on which the CSV file shall be saved
+            format: the format in which the file shall be written. Default: CSV according to RFC 4180
+        """
+        if compression != Compression.NONE:
+            raise ValueError('Currently WriteFile only supports compression NONE')
+        super().__init__(sql_statement, sql_file_name, replace)
+        self.dest_file_name = dest_file_name
+        self._db_alias = db_alias
+        self.compression = compression
+        self.format = format
+
+    @property
+    def db_alias(self) -> str:
+        return self._db_alias or config.default_db_alias()
+
+    def shell_command(self) -> str:
+        command = super().shell_command() \
+            + '  | ' + mara_db.shell.copy_to_stdout_command( \
+                self.db_alias, header=None, footer=None, delimiter_char=None, \
+                csv_format=None, pipe_format=self.format) +' \\\n'
+        return command \
+            + f'  > "{pathlib.Path(config.data_dir()) / self.dest_file_name}"'
+
+    def html_doc_items(self) -> List[Tuple[str, str]]:
+        return [('db', _.tt[self.db_alias])
+                ] \
+               + sql._SQLCommand.html_doc_items(self, self.db_alias) \
+               + [('format', _.tt[self.format]),
+                  ('destination file name', _.tt[self.dest_file_name]),
+                  (_.i['shell command'], html.highlight_syntax(self.shell_command(), 'bash'))]
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/commands/python.py` & `mara-pipelines-3.4.0/mara_pipelines/commands/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Commands for running python functions and scripts"""
 
 import inspect
 import shlex
 import sys
 import json
 from html import escape
-from typing import Union, Callable, List
+from typing import Union, Callable, List, Optional, Tuple
 from ..incremental_processing import file_dependencies
 from ..logging import logger
 
 from mara_page import html, _
 from .. import pipelines
 
 
 class RunFunction(pipelines.Command):
-    def __init__(self, function: Callable = None, args: [str] = None, file_dependencies: [str] = None) -> None:
-        """
-        Runs an arbitrary python function
-
-        Args:
-            function: The parameterless function to run
-            args: A list of arguments to be passed to the script
-            file_dependencies: Run triggered based on whether a list of files changed since the last pipeline run
-        Note:
-            if you want to pass arguments, then use a lambda function
-        """
+    """
+    Runs an arbitrary python function
+
+    Args:
+        function: The parameterless function to run
+        args: A list of arguments to be passed to the script
+        file_dependencies: Run triggered based on whether a list of files changed since the last pipeline run
+    Note:
+        if you want to pass arguments, then use a lambda function
+    """
+    def __init__(self, function: Optional[Callable] = None, args: Optional[List[str]] = None, file_dependencies: Optional[List[str]] = None) -> None:
         self.function = function
         self.args = args or []
         self.file_dependencies = file_dependencies or []
 
     def run(self) -> bool:
         dependency_type = 'RunFunction ' + self.function.__name__
         if self.file_dependencies:
@@ -44,32 +44,32 @@
             return False
 
         if self.file_dependencies:
             file_dependencies.update(self.node_path(), dependency_type, pipeline_base_path, self.file_dependencies)
 
         return True
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('function', _.pre[escape(str(self.function))]),
                 ('args', _.tt[repr(self.args)]),
                 (_.i['implementation'], html.highlight_syntax(inspect.getsource(self.function), 'python')),
                 ('file dependencies', [_.i[dependency, _.br] for dependency in self.file_dependencies])]
 
 
 class ExecutePython(pipelines.Command):
+    """
+    Runs a python script in a separate interpreter process
+
+    Args:
+        file_name: the path of the file to run, relative to the pipeline directory
+        args: A list of arguments to be passed to the script
+        file_dependencies: Run triggered based on whether a list of files changed since the last pipeline run
+    """
     def __init__(self, file_name: Union[Callable, str],
-                 args: Union[Callable, List[str]] = None, file_dependencies: [str] = None) -> None:
-        """
-        Runs a python script in a separate interpreter process
-
-        Args:
-            file_name: the path of the file to run, relative to the pipeline directory
-            args: A list of arguments to be passed to the script
-            file_dependencies: Run triggered based on whether a list of files changed since the last pipeline run
-        """
+                 args: Optional[Union[Callable, List[str]]] = None, file_dependencies: Optional[List[str]] = None) -> None:
         self._file_name = file_name
         self._args = args or []
         self.file_dependencies = file_dependencies or []
 
     @property
     def file_name(self):
         return self._file_name() if callable(self._file_name) else self._file_name
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/commands/sql.py` & `mara-pipelines-3.4.0/mara_pipelines/commands/sql.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """Commands for working with sql databases"""
 
 import functools
 import json
 import pathlib
 import shlex
-from typing import Callable, Union
+from typing import Callable, Union, Dict, Optional, List, Tuple
 
 import mara_db.dbs
 import mara_db.shell
-import mara_db.postgresql
 from mara_page import _, html
 from .. import config, shell, pipelines
 from ..incremental_processing import file_dependencies
 from ..incremental_processing import incremental_copy_status
 from ..logging import logger
 
 
 class _SQLCommand(pipelines.Command):
-    def __init__(self, sql_statement: Union[Callable, str] = None, sql_file_name: str = None,
-                 replace: {str: str} = None) -> None:
-        """
-        Something that runs a sql query (either a query string or a query file).
-
-        Args:
-            sql_statement: The statement to run as a string
-            sql_file_name: The name of the file to run (relative to the directory of the parent pipeline)
-            replace: A set of replacements to perform against the sql query `{'replace`: 'with', ..}`
-        """
+    """
+    Something that runs a sql query (either a query string or a query file).
+
+    Args:
+        sql_statement: The statement to run as a string
+        sql_file_name: The name of the file to run (relative to the directory of the parent pipeline)
+        replace: A set of replacements to perform against the sql query `{'replace`: 'with', ..}`
+    """
+    def __init__(self, sql_statement: Optional[Union[Callable, str]] = None, sql_file_name: Optional[str] = None,
+                 replace: Optional[Dict[str, str]] = None) -> None:
         if (not (sql_statement or sql_file_name)) or (sql_statement and sql_file_name):
             raise ValueError('Please provide either sql_statement or sql_file_name (but not both)')
 
         super().__init__()
         self.sql_file_name = sql_file_name
         self._sql_statement = sql_statement
         self.replace = replace or {}
@@ -76,25 +75,25 @@
                 sql = sql.replace(k, v)
             doc.append((_.i['substituted sql'], html.highlight_syntax(sql, _sql_syntax_higlighting_lexter(db_alias))))
 
         return doc
 
 
 class ExecuteSQL(_SQLCommand):
-    def __init__(self, sql_statement: str = None, sql_file_name: Union[str, Callable] = None,
-                 replace: {str: str} = None, file_dependencies=None, db_alias: str = None,
-                 echo_queries: bool = None, timezone: str = None) -> None:
-        """
-        Runs an sql file or statement in a database
-
-        Args:
-            sql_statement: The statement to run as a string
-            sql_file_name: The name of the file to run (relative to the directory of the parent pipeline)
-            replace: A set of replacements to perform against the sql query `{'replace`: 'with', ..}`
-        """
+    """
+    Runs an sql file or statement in a database
+
+    Args:
+        sql_statement: The statement to run as a string
+        sql_file_name: The name of the file to run (relative to the directory of the parent pipeline)
+        replace: A set of replacements to perform against the sql query `{'replace`: 'with', ..}`
+    """
+    def __init__(self, sql_statement: Optional[Union[str, Callable]] = None, sql_file_name: Optional[str] = None,
+                 replace: Optional[Dict[str, str]] = None, file_dependencies: Optional[List[str]] = None, db_alias: Optional[str] = None,
+                 echo_queries: Optional[bool] = None, timezone: Optional[str] = None) -> None:
         _SQLCommand.__init__(self, sql_statement, sql_file_name, replace)
 
         self._db_alias = db_alias
         self.timezone = timezone
         self.file_dependencies = file_dependencies or []
         self.echo_queries = echo_queries
 
@@ -143,29 +142,29 @@
                   ('timezone', _.tt[self.timezone or '']),
                   (_.i['shell command'], html.highlight_syntax(self.shell_command(), 'bash'))]
 
 
 class Copy(_SQLCommand):
     """Loads data from an external database"""
 
-    def __init__(self, source_db_alias: str, target_table: str, target_db_alias: str = None,
-                 sql_statement: str = None, sql_file_name: Union[Callable, str] = None, replace: {str: str} = None,
-                 timezone: str = None, csv_format: bool = None, delimiter_char: str = None,
-                 file_dependencies=None) -> None:
+    def __init__(self, source_db_alias: str, target_table: str, target_db_alias: Optional[str] = None,
+                 sql_statement: Optional[Union[Callable, str]] = None, sql_file_name: Optional[str] = None, replace: Dict[str, str] = None,
+                 timezone: Optional[str] = None, csv_format: Optional[bool] = None, delimiter_char: Optional[str] = None,
+                 file_dependencies: Optional[List[str]]=None) -> None:
         _SQLCommand.__init__(self, sql_statement, sql_file_name, replace)
         self.source_db_alias = source_db_alias
         self.target_table = target_table
         self._target_db_alias = target_db_alias
         self.timezone = timezone
         self.csv_format = csv_format
         self.delimiter_char = delimiter_char
         self.file_dependencies = file_dependencies or []
 
     @property
-    def target_db_alias(self):
+    def target_db_alias(self) -> str:
         return self._target_db_alias or config.default_db_alias()
 
     def file_path(self) -> pathlib.Path:
         return self.parent.parent.base_path() / self.sql_file_name
 
     def run(self) -> bool:
         if self.sql_file_name:
@@ -190,64 +189,64 @@
         if not super().run():
             return False
 
         if self.file_dependencies:
             file_dependencies.update(self.node_path(), dependency_type, pipeline_base_path, self.file_dependencies)
         return True
 
-    def shell_command(self):
+    def shell_command(self) -> str:
         return _SQLCommand.shell_command(self) \
                + '  | ' + mara_db.shell.copy_command(self.source_db_alias, self.target_db_alias, self.target_table,
                                                      self.timezone, self.csv_format, self.delimiter_char)
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('source db', _.tt[self.source_db_alias])] \
                + _SQLCommand.html_doc_items(self, self.source_db_alias) \
                + [('target db', _.tt[self.target_db_alias]),
                   ('target table', _.tt[self.target_table]),
                   ('timezone', _.tt[self.timezone or '']),
                   ('csv format', _.tt[self.csv_format or '']),
                   ('delimiter char', _.tt[self.delimiter_char or '']),
                   (_.i['shell command'], html.highlight_syntax(self.shell_command(), 'bash'))]
 
 
 class CopyIncrementally(_SQLCommand):
+    """
+    Incrementally loads data from one database into another.
+
+    Requires the source table to have an monotonously increasing column or combination of columns that
+    allow to identify "newer" columns (the modification comparison).
+
+    After an initial full load, only those rows with a with a a higher modification comparison than the last
+    comparison value are read.
+
+    Args:
+        source_db_alias: The database to load from
+        source_table: The table to read from
+        sql_statement: A query that is run to query the source database
+        sql_file_name: The path of a file name that is run to query the source database
+        replace: A set of replacements to perform against the sql query
+        modification_comparison: SQL expression that evaluates to a comparable value
+        modification_comparison_type: type of the saved (as string) modification_comparison value
+        comparison_value_placeholder: A placeholder in the sql code that gets replaced with the
+                                        actual incremental load comparison or `1=1`.
+        target_db_alias: The database to write to
+        target_table: The table for loading data into
+        primary_keys: A combination of primary key columns that are used for upserting into the target table
+        timezone: How to interpret timestamps in the target db
+        use_explicit_upsert: When True, uses an Update + Insert query combination. Otherwise ON CONFLICT DO UPDATE.
+    """
     def __init__(self, source_db_alias: str, source_table: str,
                  modification_comparison: str, comparison_value_placeholder: str,
-                 target_table: str, primary_keys: [str],
-                 sql_file_name: Union[str, Callable] = None, sql_statement: Union[str, Callable] = None,
-                 target_db_alias: str = None, timezone: str = None, replace: {str: str} = None,
+                 target_table: str, primary_keys: List[str],
+                 sql_file_name: Optional[str] = None, sql_statement: Optional[Union[str, Callable]] = None,
+                 target_db_alias: Optional[str] = None, timezone: Optional[str] = None, replace: Dict[str, str] = None,
                  use_explicit_upsert: bool = False,
-                 csv_format: bool = None, delimiter_char: str = None,
-                 modification_comparison_type: str = None) -> None:
-        """
-        Incrementally loads data from one database into another.
-
-        Requires the source table to have an monotonously increasing column or combination of columns that
-        allow to identify "newer" columns (the modification comparison).
-
-        After an initial full load, only those rows with a with a a higher modification comparison than the last
-        comparison value are read.
-
-        Args:
-            source_db_alias: The database to load from
-            source_table: The table to read from
-            sql_statement: A query that is run to query the source database
-            sql_file_name: The path of a file name that is run to query the source database
-            replace: A set of replacements to perform against the sql query
-            modification_comparison: SQL expression that evaluates to a comparable value
-            modification_comparison_type: type of the saved (as string) modification_comparison value
-            comparison_value_placeholder: A placeholder in the sql code that gets replaced with the
-                                          actual incremental load comparison or `1=1`.
-            target_db_alias: The database to write to
-            target_table: The table for loading data into
-            primary_keys: A combination of primary key columns that are used for upserting into the target table
-            timezone: How to interpret timestamps in the target db
-            use_explicit_upsert: When True, uses an Update + Insert query combination. Otherwise ON CONFLICT DO UPDATE.
-        """
+                 csv_format: Optional[bool] = None, delimiter_char: Optional[str] = None,
+                 modification_comparison_type: Optional[str] = None) -> None:
         _SQLCommand.__init__(self, sql_statement, sql_file_name, replace)
         self.source_db_alias = source_db_alias
         self.source_table = source_table
         self.modification_comparison = modification_comparison
         self.modification_comparison_type = modification_comparison_type
         self.comparison_value_placeholder = comparison_value_placeholder
 
@@ -256,15 +255,15 @@
         self.primary_keys = primary_keys
         self.timezone = timezone
         self.use_explicit_upsert = use_explicit_upsert
         self.csv_format = csv_format
         self.delimiter_char = delimiter_char
 
     @property
-    def target_db_alias(self):
+    def target_db_alias(self) -> str:
         return self._target_db_alias or config.default_db_alias()
 
     def run(self) -> bool:
         # retrieve the highest current value for the modification comparison (e.g.: the highest timestamp)
         # We intentionally use the command line here (rather than sqlalchemy) to avoid forcing people python drivers,
         # which can be hard for example in the case of SQL Server
         logger.log(f'Get new max modification comparison value...', format=logger.Format.ITALICS)
@@ -289,15 +288,15 @@
 
         # check whether target table is empty
         target_table_is_empty = True
 
         target_table_empty_query = f'SELECT TRUE FROM {self.target_table} LIMIT 1'
         logger.log(f'Check if target table is empty', format=logger.Format.ITALICS)
         logger.log(target_table_empty_query, format=logger.Format.VERBATIM)
-        with mara_db.postgresql.postgres_cursor_context(self.target_db_alias) as cursor:
+        with mara_db.dbs.cursor_context(self.target_db_alias) as cursor:
             cursor.execute(f'SELECT TRUE FROM {self.target_table} LIMIT 1')
             target_table_is_empty = not cursor.fetchone()
             logger.log(f"target table{'' if target_table_is_empty else ' not'} empty", format=logger.Format.ITALICS)
 
         # get last comparison value
         logger.log('Get last comparison value...', format=logger.Format.ITALICS)
         last_comparison_value = incremental_copy_status.get_last_comparison_value(
@@ -306,15 +305,15 @@
 
         if target_table_is_empty or not last_comparison_value:
             # full load
             logger.log('Using full (non incremental) Copy', logger.Format.ITALICS)
             if not target_table_is_empty:
                 truncate_query = f'TRUNCATE TABLE {self.target_table}'
                 logger.log(truncate_query, format=logger.Format.VERBATIM)
-                with mara_db.postgresql.postgres_cursor_context(self.target_db_alias) as cursor:
+                with mara_db.dbs.cursor_context(self.target_db_alias) as cursor:
                     cursor.execute(truncate_query)
             elif last_comparison_value:
                 # table is empty but we have a last comparison value from earlier runs
                 # If we would crash during load (with some data already in the table), the next run would
                 # not trigger a full load and we would miss data. To prevent that, delete the old
                 # comparison value (we will then set it only on success)
                 logger.log('Deleting old comparison value', logger.Format.ITALICS)
@@ -343,15 +342,15 @@
                            f'({self.modification_comparison} >= {modification_comparison_type} \'{last_comparison_value}\')'}
             if not shell.run_shell_command(self._copy_command(self.target_table + '_upsert', replace)):
                 return False
 
             # now the upsert table has to be merged with the target one
 
             # retrieve the target table columns to build the SET clause of the upsert query
-            with mara_db.postgresql.postgres_cursor_context(self.target_db_alias) as cursor:
+            with mara_db.dbs.cursor_context(self.target_db_alias) as cursor:
                 retrieve_column_query = f"SELECT attname FROM pg_attribute WHERE attrelid = '{self.target_table}'::REGCLASS AND attnum > 0;"
                 logger.log(retrieve_column_query, format=logger.Format.VERBATIM)
                 cursor.execute(retrieve_column_query)
                 if self.use_explicit_upsert:
                     set_clause = ', '.join([f'"{col[0]}" = src."{col[0]}"' for col in cursor.fetchall()])
                     key_definition = ' AND '.join([f'dst."{k}" = src."{k}"' for k in self.primary_keys])
                 else:
@@ -396,15 +395,15 @@
         """Helper function for creating the actual copy command"""
         return (_SQLCommand.shell_command(self)
                 + '  | ' + shell.sed_command(replace)
                 + '  | ' + mara_db.shell.copy_command(self.source_db_alias, self.target_db_alias,
                                                       target_table, timezone=self.timezone,
                                                       csv_format=self.csv_format, delimiter_char=self.delimiter_char))
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('source db', _.tt[self.source_db_alias]),
                 ('source table', _.tt[self.source_table]),
                 ('modification comparison', _.tt[self.modification_comparison])] \
                + _SQLCommand.html_doc_items(self, self.source_db_alias) \
                + [('comparison value placeholder', _.tt[self.comparison_value_placeholder]),
                   ('modification comparison type', _.tt[self.modification_comparison_type if self.modification_comparison_type else '(no cast)']),
                   ('target db', _.tt[self.target_db_alias]),
@@ -412,21 +411,21 @@
                   ('primary_keys', _.tt[repr(self.primary_keys)]),
                   ('timezone', _.tt[self.timezone or '']),
                   ('csv format', _.tt[self.csv_format or '']),
                   ('delimiter char', _.tt[self.delimiter_char or '']),
                   ('use explicit upsert', _.tt[repr(self.use_explicit_upsert)])]
 
 
-def _expand_pattern_substitution(replace: {str: str}) -> {str: str}:
+def _expand_pattern_substitution(replace: Dict[str, str]) -> Dict[str, str]:
     """Helper function for replacing callables with their value in a dictionary"""
     return {k: (str(v()) if callable(v) else str(v)) for k, v in replace.items()}
 
 
 @functools.singledispatch
-def _sql_syntax_higlighting_lexter(db):
+def _sql_syntax_higlighting_lexter(db) -> str:
     """Returns the best lexer from http://pygments.org/docs/lexers/ for a database dialect"""
     return 'sql'
 
 
 _sql_syntax_higlighting_lexter.register(str, lambda alias: _sql_syntax_higlighting_lexter(mara_db.dbs.db(alias)))
 _sql_syntax_higlighting_lexter.register(mara_db.dbs.PostgreSQLDB, lambda _: 'postgresql')
 _sql_syntax_higlighting_lexter.register(mara_db.dbs.MysqlDB, lambda _: 'mysql')
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/config.py` & `mara-pipelines-3.4.0/mara_pipelines/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def last_date() -> datetime.date:
     """Ignore data after this date"""
     return datetime.date(3000, 1, 1)
 
 
-def max_number_of_parallel_tasks():
+def max_number_of_parallel_tasks() -> int:
     """How many tasks can run in parallel at maximum"""
     return multiprocessing.cpu_count()
 
 
 def bash_command_string() -> str:
     """The command used for running a bash, should somehow include the `pipefail` option"""
     return '/usr/bin/env bash -o pipefail'
@@ -86,15 +86,15 @@
     Slack channel's token (i.e. THISIS/ASLACK/TOCKEN) can be retrieved from the
     channel's app "Incoming WebHooks" configuration as part part of the Webhook URL
     """
     return None
 
 
 @functools.lru_cache(maxsize=None)
-def event_handlers() -> [events.EventHandler]:
+def event_handlers() -> typing.List[events.EventHandler]:
     """
     Configure additional event handlers that listen to pipeline events, e.g. chat bots that announce failed runs
 
     Example:
         mara_pipelines.config.event_handlers = lambda: [mara_pipelines.notification.slack.Slack('123/ABC/cdef')]
     """
     # the default implementation ensures backward compatibility, don't use otherwise
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/events.py` & `mara-pipelines-3.4.0/mara_pipelines/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import abc
 import datetime
 import sys
 
 
 class Event():
+    """
+    Base class for events that are emitted from mara.
+    """
     def __init__(self) -> None:
-        """
-        Base class for events that are emitted from mara.
-        """
         pass
 
     def to_json(self):
         return json.dumps({field: value.isoformat() if isinstance(value, datetime.datetime) else value
                            for field, value in self.__dict__.items()})
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/execution.py` & `mara-pipelines-3.4.0/mara_pipelines/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 import signal
 import atexit
 import time
 import traceback
 from multiprocessing import queues
 from multiprocessing.context import BaseContext
 from queue import Empty
+from typing import Set, List, Dict, Optional
 
 from . import pipelines, config
 from .logging import logger, pipeline_events, system_statistics, run_log, node_cost
 from . import events
 
 
-def run_pipeline(pipeline: pipelines.Pipeline, nodes: {pipelines.Node} = None,
+def run_pipeline(pipeline: pipelines.Pipeline, nodes: Optional[Set[pipelines.Node]] = None,
                  with_upstreams: bool = False,
                  interactively_started: bool = False
-                 ) -> [events.Event]:
+                 ) -> List[events.Event]:
     """
     Runs a pipeline in a forked sub process. Acts as a generator that yields events from the sub process.
 
     Using forking has two advantages:
     1. The pipeline is also forked and thus can be modified without affecting the original pipeline.
     2. It's possible to hand over control to the parent process while the pipeline is running, for example
        for sending output to a browser.
@@ -68,28 +69,28 @@
         statistics_process: multiprocessing.Process = None
 
         try:
             # capture output of print statements and other unplanned output
             logger.redirect_output(event_queue, pipeline.path())
 
             # all nodes that have not run yet, ordered by priority
-            node_queue: [pipelines.Node] = []
+            node_queue: List[pipelines.Node] = []
 
             # data needed for computing cost
             node_durations_and_run_times = node_cost.node_durations_and_run_times(pipeline) if use_historical_node_cost else {}
 
             # Putting nodes into the node queue
-            def queue(nodes: [pipelines.Node]):
+            def queue(nodes: List[pipelines.Node]):
                 for node in nodes:
                     node_cost.compute_cost(node, node_durations_and_run_times)
                     node_queue.append(node)
                 node_queue.sort(key=lambda node: node.cost, reverse=True)
 
             if nodes:  # only run a set of child nodes
-                def with_all_upstreams(nodes: {pipelines.Node}):
+                def with_all_upstreams(nodes: Set[pipelines.Node]):
                     """recursively find all upstreams of a list of nodes"""
                     return functools.reduce(set.union, [with_all_upstreams(node.upstreams) for node in nodes], nodes)
 
                 # when requested, include all upstreams of nodes, otherwise just use provided nodes
                 nodes_to_run = with_all_upstreams(set(nodes)) if with_upstreams else set(nodes)
 
                 # remove everything from pipeline that should not be run
@@ -106,19 +107,19 @@
                 pipeline.downstreams = set()
                 # queue whole pipeline
                 queue([pipeline])
 
             # book keeping
             run_start_time = datetime.datetime.now(tz.utc)
             # all nodes that already ran or that won't be run anymore
-            processed_nodes: {pipelines.Node} = set()
+            processed_nodes: Set[pipelines.Node] = set()
             # running pipelines with start times and number of running children
-            running_pipelines: {pipelines.Pipeline: [datetime.datetime, int]} = {}
-            failed_pipelines: {pipelines.Pipeline} = set()  # pipelines with failed tasks
-            running_task_processes: {pipelines.Task: TaskProcess} = {}
+            running_pipelines: Dict[pipelines.Pipeline, [datetime.datetime, int]] = {}
+            failed_pipelines: Set[pipelines.Pipeline] = set()  # pipelines with failed tasks
+            running_task_processes: Dict[pipelines.Task, TaskProcess] = {}
 
             # make sure any running tasks are killed when this executor process is shutdown
             executor_pid = os.getpid()
 
             def ensure_task_processes_killed():
                 # as we fork, the TaskProcess also runs this function -> ignore it there
                 if os.getpid() != executor_pid: return
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/incremental_processing/file_dependencies.py` & `mara-pipelines-3.4.0/mara_pipelines/incremental_processing/file_dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Functions for keeping track of whether a list of files changed since the last pipeline run"""
 import datetime
 import hashlib
 import pathlib
+from typing import List
 
 import sqlalchemy
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
-import mara_db.postgresql
+import mara_db.dbs
 from .. import config
 
 Base = declarative_base()
 
 
 class FileDependency(Base):
     """A combined hash of the content of a list of files"""
@@ -18,70 +19,70 @@
 
     node_path = sqlalchemy.Column(sqlalchemy.ARRAY(sqlalchemy.TEXT), primary_key=True)
     dependency_type = sqlalchemy.Column(sqlalchemy.String, primary_key=True)
     hash = sqlalchemy.Column(sqlalchemy.String)
     timestamp = sqlalchemy.Column(sqlalchemy.TIMESTAMP(timezone=True))
 
 
-def update(node_path: [str], dependency_type: str, pipeline_base_path: str, file_dependencies: [str]):
+def update(node_path: List[str], dependency_type: str, pipeline_base_path: str, file_dependencies: List[str]):
     """
     Stores the combined hash of a list of files
 
     Args:
         node_path: The path of the node that depends on the files
         dependency_type: An arbitrary string that allows to distinguish between multiple dependencies of a node
         pipeline_base_path: The base directory of the pipeline
         file_dependencies: A list of file names relative to pipeline_base_path
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f"""
 INSERT INTO data_integration_file_dependency (node_path, dependency_type, hash, timestamp)
 VALUES ({'%s,%s,%s,%s'})
 ON CONFLICT (node_path, dependency_type)
 DO UPDATE SET timestamp = EXCLUDED.timestamp, hash = EXCLUDED.hash
     """, (node_path, dependency_type, hash(pipeline_base_path, file_dependencies), datetime.datetime.utcnow()))
 
-def delete(node_path: [str], dependency_type: str):
+def delete(node_path: List[str], dependency_type: str):
     """
     Delets the combined hash of a list of files for that node and dependency type
 
     Args:
         node_path: The path of the node that depends on the files
         dependency_type: An arbitrary string that allows to distinguish between multiple dependencies of a node
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f"""
 DELETE FROM data_integration_file_dependency
 WHERE node_path = {'%s'} AND dependency_type = {'%s'}
     """, (node_path, dependency_type))
 
 
-def is_modified(node_path: [str], dependency_type: str, pipeline_base_path: str, file_dependencies: [str]):
+def is_modified(node_path: List[str], dependency_type: str, pipeline_base_path: str, file_dependencies: List[str]):
     """
     Checks whether a list of files have been modified since the last pipeline run
 
     Args:
         node_path: The path of the node that depends on the files
         dependency_type: An arbitrary string that allows to distinguish between multiple dependencies of a node
         pipeline_base_path: The base directory of the pipeline
         file_dependencies: A list of file names relative to pipeline_base_path
 
     Returns: True when at least one of the files was modified
 
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute("""
 SELECT TRUE
 FROM data_integration_file_dependency
 WHERE node_path=%s AND dependency_type=%s AND hash=%s """,
                        (node_path, dependency_type, hash(pipeline_base_path, file_dependencies)))
         return False if cursor.fetchone() else True
 
 
-def hash(pipeline_base_path: pathlib.Path, file_dependencies: [str]) -> str:
+def hash(pipeline_base_path: pathlib.Path, file_dependencies: List[str]) -> str:
     """
     Creates a combined hash of the content of a list of files
 
     Args:
         pipeline_base_path: The base directory of the pipeline
         file_dependencies: A list of file names relative to pipeline_base_path
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/incremental_processing/incremental_copy_status.py` & `mara-pipelines-3.4.0/mara_pipelines/incremental_processing/incremental_copy_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 """Tracks the last comparison value of an incremental copy"""
 
+from typing import List
+
 import sqlalchemy
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
 import mara_db.config
 import mara_db.dbs
-import mara_db.postgresql
 
 Base = declarative_base()
 
 
 class IncrementalCopyStatus(Base):
     """The last `modification_value` for a table that is incrementally loaded"""
     __tablename__ = 'data_integration_incremental_copy_status'
 
     node_path = sqlalchemy.Column(sqlalchemy.ARRAY(sqlalchemy.Text), primary_key=True, index=True)
     source_table = sqlalchemy.Column(sqlalchemy.Text, primary_key=True)
     last_comparison_value = sqlalchemy.Column(sqlalchemy.Text)
 
 
-def update(node_path: [str], source_db_alias: str, source_table: str, last_comparison_value):
+def update(node_path: List[str], source_db_alias: str, source_table: str, last_comparison_value):
     """
     Updates the last_comparison_value for a pipeline node and table
     Args:
         node_path: The path of the parent pipeline node
         source_db_alias: The alias of the the db from which data is copied
         source_table: The table from which is copied
         max_modification_value: The last retrieved modification value
 
     Returns:
 
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 INSERT INTO data_integration_incremental_copy_status (node_path, source_table, last_comparison_value)
 VALUES ({'%s,%s,%s'})
 ON CONFLICT (node_path, source_table)
 DO UPDATE SET last_comparison_value = EXCLUDED.last_comparison_value
 ''', (node_path, f'{source_db_alias}.{source_table}', last_comparison_value))
 
 
-def delete(node_path: [str], source_db_alias: str, source_table: str):
+def delete(node_path: List[str], source_db_alias: str, source_table: str):
     """
     Deletes the last_comparison_value for a pipeline node and table
     Args:
         node_path: The path of the parent pipeline node
         source_db_alias: The alias of the the db from which data is copied
         source_table: The table from which is copied
     Returns:
 
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 DELETE FROM data_integration_incremental_copy_status
 WHERE node_path = {'%s'} AND source_table = {'%s'}
 ''', (node_path, f'{source_db_alias}.{source_table}'))
 
 
 
-def get_last_comparison_value(node_path: [str], source_db_alias: str, source_table: str):
+def get_last_comparison_value(node_path: List[str], source_db_alias: str, source_table: str):
     """
     Returns the last comparison value for a pipeline node and table
     Args:
         node_path: The path of the parent pipeline node
         source_db_alias: The alias of the the db from which data is copied
         source_table: The table from which is copied
 
     Returns:
         The value or None
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f"""
 SELECT last_comparison_value
 FROM data_integration_incremental_copy_status
 WHERE node_path = {'%s'} AND source_table = {'%s'}""", (node_path, f'{source_db_alias}.{source_table}'))
         result = cursor.fetchone()
         return result[0] if result else None
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/incremental_processing/processed_files.py` & `mara-pipelines-3.4.0/mara_pipelines/incremental_processing/processed_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Functions for keeping track whether an input file has already been 'processed' """
 
-import datetime
+from datetime import datetime
+from typing import Dict
 
 import sqlalchemy
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
 import mara_db.config
 import mara_db.dbs
-import mara_db.postgresql
 
 Base = declarative_base()
 
 
 class ProcessedFile(Base):
     """A local file that has been 'processed' (e.g. has been read)"""
     __tablename__ = 'data_integration_processed_file'
@@ -28,32 +28,32 @@
     Args:
         node_path: The path of the node that processed the file
         file_name: The name of the file that has been processed
         last_modified_timestamp: The time when the file was modified last
 
     Returns: True
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
-INSERT INTO data_integration_processed_file (node_path, file_name, last_modified_timestamp) 
+INSERT INTO data_integration_processed_file (node_path, file_name, last_modified_timestamp)
 VALUES ({'%s,%s,%s'})
-ON CONFLICT (node_path, file_name) 
+ON CONFLICT (node_path, file_name)
 DO UPDATE SET last_modified_timestamp = EXCLUDED.last_modified_timestamp
 ''', (node_path, file_name, last_modified_timestamp))
     return True
 
 
-def already_processed_files(node_path: str) -> {str: datetime}:
+def already_processed_files(node_path: str) -> Dict[str, datetime]:
     """
     Returns all files that already have been processed by a node
     Args:
         node_path: The path of the node that processed the file
 
     Returns:
         A mapping of file names to timestamps of last modification
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f"""
 SELECT file_name, last_modified_timestamp
 FROM data_integration_processed_file WHERE node_path = {'%s'}
 """, (node_path,))
         return {row[0]: row[1] for row in cursor.fetchall()}
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/incremental_processing/reset.py` & `mara-pipelines-3.4.0/mara_pipelines/incremental_processing/reset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Resetting incremental copy status"""
 
+from typing import List
+
 import mara_db.config
-import mara_db.postgresql
+import mara_db.dbs
 
 
-def reset_incremental_processing(node_path: [str]):
+def reset_incremental_processing(node_path: List[str]):
     """
     Recursively resets all incremental processing status information that is stored in the mara db
     Args:
         node_path: The path of the node to reset
 
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 SELECT *
 FROM
   (SELECT node_path, 'processed files', count(*)
    FROM data_integration_processed_file
    GROUP BY node_path
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/logging/logger.py` & `mara-pipelines-3.4.0/mara_pipelines/logging/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Text output logging with redirection to queues"""
 
+from datetime import datetime
 import multiprocessing
 import sys
-from datetime import datetime
+from typing import List
 
 from ..logging import pipeline_events
 import mara_pipelines.config
 
 Format = pipeline_events.Output.Format
 
 
@@ -42,15 +43,15 @@
 _event_queue: multiprocessing.Queue = None
 """When running in a forked process, this will be bound to a queue for sending events to the parent process."""
 
 _current_node_path = None
 """When running in a forked task process, this will be bound to the path of the currently running pipeline node"""
 
 
-def redirect_output(event_queue: multiprocessing.Queue, node_path: [str]):
+def redirect_output(event_queue: multiprocessing.Queue, node_path: List[str]):
     """
     Redirects the output of the `log` function as well as `sys.stdout` and `sys.stderr` to `event_queue`
     Args:
         queue: The queue where to redirect messages to
         node_path: The id and parent ids of the currently running tasks
     """
     global _event_queue
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/logging/node_cost.py` & `mara-pipelines-3.4.0/mara_pipelines/logging/node_cost.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Computation of node duration, run time and cost"""
 
 import functools
 import math
+from typing import Dict
 
 import mara_db.config
-import mara_db.postgresql
+import mara_db.dbs
 from .. import pipelines
 
 
-def node_durations_and_run_times(node: pipelines.Node) -> {tuple: [float, float]}:
+def node_durations_and_run_times(node: pipelines.Node) -> Dict[tuple, object]:  # object = [float, float]
     """
     Returns for children of `node` the average duration and run time (sum of average duration of all leaf nodes)
 
     Args:
         node: The parent node
 
     Returns:
         A dictionary of {(node_path,): [avg_duration, avg_run_time]} entries for all children of `node`
 
     """
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f"""
 WITH child_nodes AS
        (SELECT node.node_path [ 0 : {'%(level)s'} + 1]                     AS node_path,
                avg(CASE -- direct children
                      WHEN array_length(node.node_path, 1) = {'%(level)s'} + 1
                        THEN extract(EPOCH FROM end_time - start_time) END) AS avg_duration,
                avg(CASE -- all children except pipelines
@@ -39,15 +40,15 @@
        round(sum(avg_run_time)::NUMERIC, 1) AS avg_run_time
 FROM child_nodes
 GROUP BY node_path;""", {'path': node.path(), 'level': len(node.path())})
 
         return {tuple(row[0]): row[1:] for row in cursor.fetchall()}
 
 
-def compute_cost(node: pipelines.Node, node_durations_and_run_times: {tuple: [float, float]}) -> float:
+def compute_cost(node: pipelines.Node, node_durations_and_run_times: Dict[tuple, object]) -> float:  # object = [float, float]
     """
     Computes the cost of a node as maximum cumulative run time of a node and all its downstreams.
     Stores the result in `node` and also returns it
 
     Args:
         node: The node for which to compute the cost
         node_durations_and_run_times: Duration and run time information as computed by
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/logging/pipeline_events.py` & `mara-pipelines-3.4.0/mara_pipelines/logging/pipeline_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Events that are emitted during pipeline execution"""
 
 import datetime
-import json
+import os
+import getpass
 
 import enum
 import typing as t
 
 from ..events import Event
 
 
 class PipelineEvent(Event):
-    def __init__(self, node_path: [str]) -> None:
+    def __init__(self, node_path: t.List[str]) -> None:
         """
         Base class for events that are emitted during a pipeline run.
 
         Args:
             node_path: The path of the current node in the data pipeline that is run
 
         """
         super().__init__()
         self.node_path = node_path
 
 
 class RunStarted(PipelineEvent):
-    def __init__(self, node_path: [str],
+    def __init__(self, node_path: t.List[str],
                  start_time: datetime.datetime,
                  pid: int,
                  is_root_pipeline: bool = False,
                  node_ids: t.Optional[t.List[str]] = None,
                  interactively_started: bool = False) -> None:
         """
         A pipeline run started
@@ -47,15 +48,15 @@
         self.is_root_pipeline = is_root_pipeline
         self.node_ids = node_ids or []
 
         self.user: str = get_user_display_name(interactively_started)
 
 
 class RunFinished(PipelineEvent):
-    def __init__(self, node_path: [str],
+    def __init__(self, node_path: t.List[str],
                  end_time: datetime.datetime,
                  succeeded: bool,
                  interactively_started: bool = False) -> None:
         """
         A pipeline run finished
         Args:
             node_path: The path of the pipeline that was run
@@ -67,29 +68,29 @@
         self.node_path = node_path
         self.end_time = end_time
         self.succeeded = succeeded
         self.interactively_started = interactively_started
 
 
 class NodeStarted(PipelineEvent):
-    def __init__(self, node_path: [str], start_time: datetime.datetime, is_pipeline: bool) -> None:
+    def __init__(self, node_path: t.List[str], start_time: datetime.datetime, is_pipeline: bool) -> None:
         """
         A task run started.
         Args:
             node_path: The path of the current node in the data pipeline that is run
             start_time: The time when the task started
             is_pipeline: Whether the node is a pipeline
         """
         super().__init__(node_path)
         self.start_time = start_time
         self.is_pipeline = is_pipeline
 
 
 class NodeFinished(PipelineEvent):
-    def __init__(self, node_path: [str], start_time: datetime.datetime, end_time: datetime.datetime,
+    def __init__(self, node_path: t.List[str], start_time: datetime.datetime, end_time: datetime.datetime,
                  is_pipeline: bool, succeeded: bool) -> None:
         """
         A run of a task or pipeline finished.
         Args:
             node_path: The path of the current node in the data pipeline that is run
             start_time: The time when the task started
             end_time: The time when the task finished
@@ -106,15 +107,15 @@
 class Output(PipelineEvent):
     class Format(enum.EnumMeta):
         """Formats for displaying log messages"""
         STANDARD = 'standard'
         VERBATIM = 'verbatim'
         ITALICS = 'italics'
 
-    def __init__(self, node_path: [str], message: str,
+    def __init__(self, node_path: t.List[str], message: str,
                  format: Format = Format.STANDARD, is_error: bool = False) -> None:
         """
         Some text output occurred.
         Args:
             node_path: The path of the current node in the data pipeline that is run
             message: The message to display
             format: How to format the message
@@ -133,13 +134,15 @@
     Defaults to MARA_RUN_USER_DISPLAY_NAME and falls back to the current OS-level name
     if the run was started interactively, else None.
 
     :param interactively_started: True if the run was triggered interactively
 
     Patch if you have more sophisticated needs.
     """
-    import os
     if 'MARA_RUN_USER_DISPLAY_NAME' in os.environ:
         return os.environ.get('MARA_RUN_USER_DISPLAY_NAME')
     if not interactively_started:
         return None
-    return os.environ.get('SUDO_USER') or os.environ.get('USER') or os.getlogin()
+    try:
+        return os.environ.get('SUDO_USER') or os.environ.get('USER') or getpass.getuser()
+    except Exception: # pylint: disable=W0703
+        return None
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/logging/run_log.py` & `mara-pipelines-3.4.0/mara_pipelines/logging/run_log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Logging pipeline runs, node output and status information in mara database"""
 
+from typing import List, Dict
+
 import sqlalchemy.orm
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
 from .. import config
 from ..logging import pipeline_events, system_statistics
 from .. import events
 
 Base = declarative_base()
 
@@ -73,30 +75,29 @@
         return
 
     import mara_db.config
 
     if 'mara' not in mara_db.config.databases():
         return
 
-    import psycopg2.extensions
-    import mara_db.postgresql
+    import mara_db.dbs
 
     _close_run = f'''
 UPDATE  data_integration_run
 SET end_time = now(), succeeded = FALSE
 WHERE run_id = {"%s"} and end_time IS NULL
 RETURNING run_id
     '''
     _close_node_run = f'''
 UPDATE  data_integration_node_run
 SET end_time = now(), succeeded = FALSE
 WHERE run_id = {"%s"} and end_time IS NULL
 RETURNING run_id
         '''
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+    with mara_db.dbs.cursor_context('mara') as cursor:
         _closed_any=False
         for code in [_close_node_run, _close_run]:
             try:
                 cursor.execute(code, (run_id,))
                 if cursor.fetchall():
                     _closed_any = True
             except:
@@ -112,22 +113,21 @@
     def handle_event(self, event: events.Event):
         pass
 
 
 class RunLogger(events.EventHandler):
     """A run logger saving the pipeline events to the 'mara' database alias"""
     run_id: int = None
-    node_output: {tuple: [pipeline_events.Output]} = None
+    node_output: Dict[tuple, List[pipeline_events.Output]] = None
 
     def handle_event(self, event: events.Event):
-        import psycopg2.extensions
-        import mara_db.postgresql
+        import mara_db.dbs
 
         if isinstance(event, pipeline_events.RunStarted):
-            with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+            with mara_db.dbs.cursor_context('mara') as cursor:
                 cursor.execute(f'''
 INSERT INTO data_integration_run (node_path, pid, start_time)
 VALUES ({"%s, %s, %s"})
 RETURNING run_id;''', (event.node_path, event.pid, event.start_time))
                 self.run_id = cursor.fetchone()[0]
 
         elif isinstance(event, pipeline_events.Output):
@@ -138,23 +138,23 @@
 
             if key in self.node_output:
                 self.node_output[key].append(event)
             else:
                 self.node_output[key] = [event]
 
         elif isinstance(event, pipeline_events.NodeStarted):
-            with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+            with mara_db.dbs.cursor_context('mara') as cursor:
                 cursor.execute(f'''
 INSERT INTO data_integration_node_run (run_id, node_path, start_time, is_pipeline)
 VALUES  ({"%s, %s, %s, %s"})
 RETURNING node_run_id''', (self.run_id, event.node_path, event.start_time, event.is_pipeline))
 
         elif isinstance(event, system_statistics.SystemStatistics):
             try:
-                with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+                with mara_db.dbs.cursor_context('mara') as cursor:
                     cursor.execute(f'''
     INSERT INTO data_integration_system_statistics (timestamp, run_id, disc_read, disc_write, net_recv, net_sent,
                                       cpu_usage, mem_usage, swap_usage, iowait)
     VALUES ({"%s, %s, %s, %s, %s, %s, %s, %s, %s, %s"})''',
                                    (event.timestamp, self.run_id, event.disc_read, event.disc_write, event.net_recv,
                                     event.net_sent, event.cpu_usage, event.mem_usage, event.swap_usage, event.iowait))
             except Exception as e:
@@ -162,15 +162,15 @@
                 # ETLs at the same time it could happened that two of them get inserted with same TS and it fails.
                 # Nowadays we have a compound PK but the migration scripts didn't pick this up so we could still
                 # have a single PK on upgraded tables.
                 # As we do not really care about every single stat we simply throw away that single stat, the next
                 # will come in 1 sec (default, if not changed...)
                 print(f'Ignored problem on inserting system statistic events into the table: {e!r}', flush=True)
         elif isinstance(event, pipeline_events.NodeFinished):
-            with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+            with mara_db.dbs.cursor_context('mara') as cursor:
                 cursor.execute(f'''
 UPDATE data_integration_node_run
 SET end_time={"%s"}, succeeded={"%s"}
 WHERE run_id={"%s"} AND node_path={"%s"}
 RETURNING node_run_id''', (event.end_time, event.succeeded, self.run_id, event.node_path))
                 node_run_id = cursor.fetchone()[0]
 
@@ -178,15 +178,15 @@
 INSERT INTO data_integration_node_output (node_run_id, timestamp, message, format, is_error)
 VALUES ''' + ','.join([cursor.mogrify('(%s,%s,%s,%s,%s)', (node_run_id, output_event.timestamp, output_event.message,
                                                            output_event.format, output_event.is_error))
                       .decode('utf-8')
                        for output_event in self.node_output.get(tuple(event.node_path))]))
 
         elif isinstance(event, pipeline_events.RunFinished):
-            with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+            with mara_db.dbs.cursor_context('mara') as cursor:
                 cursor.execute(f'''
 UPDATE data_integration_run
 SET end_time={"%s"}, succeeded={"%s"}
 WHERE run_id={"%s"}''', (event.end_time, event.succeeded, self.run_id))
 
                 cursor.execute(f'''
 DELETE FROM data_integration_node_output WHERE node_run_id IN (
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/logging/system_statistics.py` & `mara-pipelines-3.4.0/mara_pipelines/logging/system_statistics.py`

 * *Files identical despite different names*

### Comparing `mara-pipelines-3.3.0/mara_pipelines/notification/notifier.py` & `mara-pipelines-3.4.0/mara_pipelines/notification/notifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import abc
+from typing import Dict, List
 
 from .. import events
 from ..logging import pipeline_events
 
 
 class ChatNotifier(events.EventHandler, abc.ABC):
 
     def __init__(self):
         """ Abstract class for sending notifications to chat bots when pipeline errors occur"""
 
         # keep a list of log messages and error log messages for each node
-        self.node_output: {tuple: {bool: [events.Event]}} = None
+        self.node_output: Dict[tuple, Dict[bool, List[events.Event]]] = None
 
 
     def handle_event(self, event: events.Event):
         """
         Send notifications for failed tasks and interactively started pipelines
 
         Args:
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/notification/slack.py` & `mara-pipelines-3.4.0/mara_pipelines/notification/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from typing import List
 from .. import config
 from ..logging import pipeline_events
 from ..notification.notifier import ChatNotifier
 
 
 class Slack(ChatNotifier):
 
@@ -56,15 +57,15 @@
         self._send_message({'text': text, 'attachments': attachments})
 
     def _send_message(self, message):
         response = requests.post(url='https://hooks.slack.com/services/' + self.token, json=message)
         if response.status_code != 200:
             raise ValueError(f'Could not send message. Status {response.status_code}, response "{response.text}"')
 
-    def _format_output(self, output_events: [pipeline_events.Output]):
+    def _format_output(self, output_events: List[pipeline_events.Output]):
         output, last_format = '', ''
         for event in output_events:
             if event.format == pipeline_events.Output.Format.VERBATIM:
                 if last_format == event.format:
                     # append new verbatim line to the already initialized verbatim output
                     output = output[0:-3] + f'\n{event.message}```'
                 else:
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/notification/teams.py` & `mara-pipelines-3.4.0/mara_pipelines/notification/teams.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from typing import List
 from .. import config
 from ..logging import pipeline_events
 from .notifier import ChatNotifier
 
 
 class Teams(ChatNotifier):
     def __init__(self, token):
@@ -52,15 +53,15 @@
 
     def _send_message(self, message):
         response = requests.post(url='https://outlook.office.com/webhook/' + self.token, json=message)
 
         if response.status_code != 200:
             raise ValueError(f'Could not send message. Status {response.status_code}, response "{response.text}"')
 
-    def _format_output(self, output_events: [pipeline_events.Output]):
+    def _format_output(self, output_events: List[pipeline_events.Output]):
         output, last_format = '', ''
         for event in output_events:
             if event.format == pipeline_events.Output.Format.VERBATIM:
                 if last_format == event.format:
                     # append new verbatim line to the already initialized verbatim output
                     output = output[0:-len('</pre>')] + f'\n{event.message}</pre>'
                 else:
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/files.py` & `mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import glob
 import json
 import math
 import os.path
 import pathlib
 import re
 from html import escape
+from typing import List, Tuple, Optional
 
 import mara_db.config
 import mara_db.dbs
-import mara_db.postgresql
 from mara_page import _, html
 
 from .. import config, pipelines
 from ..commands import python, sql, files
 from ..incremental_processing import file_dependencies as _file_dependencies
 from ..incremental_processing import processed_files as _processed_files
 from ..logging import logger
@@ -27,18 +27,18 @@
     ONLY_NEW = 'only_new'  # load only files that have not been loaded yet
     ONLY_CHANGED = 'only_changed'  # load all files that were modified since the last run (or that are new)
     ONLY_NEW_EXCEPT_LATEST = 'only_new_except_latest'  # load only files that have not been loaded yet and not the last one
 
 
 class _ParallelRead(pipelines.ParallelTask):
     def __init__(self, id: str, description: str, file_pattern: str, read_mode: ReadMode, target_table: str,
-                 max_number_of_parallel_tasks: int = None, file_dependencies: [str] = None, date_regex: str = None,
+                 max_number_of_parallel_tasks: Optional[int] = None, file_dependencies: Optional[List[str]] = None, date_regex: Optional[str] = None,
                  partition_target_table_by_day_id: bool = False, truncate_partitions: bool = False,
-                 commands_before: [pipelines.Command] = None, commands_after: [pipelines.Command] = None,
-                 db_alias: str = None, timezone: str = None) -> None:
+                 commands_before: Optional[List[pipelines.Command]] = None, commands_after: Optional[List[pipelines.Command]] = None,
+                 db_alias: Optional[str] = None, timezone: Optional[str] = None) -> None:
         pipelines.ParallelTask.__init__(self, id=id, description=description,
                                         max_number_of_parallel_tasks=max_number_of_parallel_tasks,
                                         commands_before=commands_before, commands_after=commands_after)
         self.file_pattern = file_pattern
         self.read_mode = read_mode
         self.date_regex = date_regex
         self.file_dependencies = file_dependencies or []
@@ -115,15 +115,15 @@
 
         chunk_size = math.ceil(len(files) / (2 * config.max_number_of_parallel_tasks()))
 
         if self.partition_target_table_by_day_id:
             if not isinstance(mara_db.dbs.db(self.db_alias), mara_db.dbs.PostgreSQLDB):
                 raise NotImplementedError(
                     f'Partitioning by day_id has only been implemented for postgresql so far, \n'
-                    f'not for {mara_db.postgresql.engine(self.db_alias).name}')
+                    f'not for {mara_db.dbs.db(self.db_alias)}')
             files_per_day = {}
             for (file, date) in files:
                 if date in files_per_day:
                     files_per_day[date].append(file)
                 else:
                     files_per_day[date] = [file]
 
@@ -153,15 +153,15 @@
                 sub_pipeline.add(task, ['create_partitions'])
         else:
             for n, chunk in enumerate(more_itertools.chunked(files, chunk_size)):
                 sub_pipeline.add(
                     pipelines.Task(id=str(n), description=f'Reads {len(chunk)} files',
                                    commands=sum([self.parallel_commands(x[0]) for x in chunk], [])))
 
-    def parallel_commands(self, file_name: str) -> [pipelines.Command]:
+    def parallel_commands(self, file_name: str) -> List[pipelines.Command]:
         return [self.read_command(file_name)] + (
             [python.RunFunction(function=lambda: _processed_files.track_processed_file(
                 self.path(), file_name, self._last_modification_timestamp(file_name)))]
             if self.read_mode != ReadMode.ALL else [])
 
     def read_command(self) -> pipelines.Command:
         raise NotImplementedError
@@ -169,22 +169,22 @@
     def _last_modification_timestamp(self, file_name):
         return datetime.datetime.fromtimestamp(
             os.path.getmtime(pathlib.Path(config.data_dir()) / file_name)).astimezone()
 
 
 class ParallelReadFile(_ParallelRead):
     def __init__(self, id: str, description: str, file_pattern: str, read_mode: ReadMode,
-                 compression: files.Compression, target_table: str, file_dependencies: [str] = None,
-                 date_regex: str = None, partition_target_table_by_day_id: bool = False,
+                 compression: files.Compression, target_table: str, file_dependencies: Optional[List[str]] = None,
+                 date_regex: Optional[str] = None, partition_target_table_by_day_id: bool = False,
                  truncate_partitions: bool = False,
-                 commands_before: [pipelines.Command] = None, commands_after: [pipelines.Command] = None,
-                 mapper_script_file_name: str = None, make_unique: bool = False, db_alias: str = None,
-                 delimiter_char: str = None, quote_char: str = None, null_value_string: str = None,
-                 skip_header: bool = None, csv_format: bool = False,
-                 timezone: str = None, max_number_of_parallel_tasks: int = None) -> None:
+                 commands_before: Optional[List[pipelines.Command]] = None, commands_after: Optional[List[pipelines.Command]] = None,
+                 mapper_script_file_name: Optional[str] = None, make_unique: bool = False, db_alias: Optional[str] = None,
+                 delimiter_char: Optional[str] = None, quote_char: Optional[str] = None, null_value_string: Optional[str] = None,
+                 skip_header: Optional[bool] = None, csv_format: bool = False,
+                 timezone: Optional[str] = None, max_number_of_parallel_tasks: Optional[int] = None) -> None:
         _ParallelRead.__init__(self, id=id, description=description, file_pattern=file_pattern,
                                read_mode=read_mode, target_table=target_table, file_dependencies=file_dependencies,
                                date_regex=date_regex, partition_target_table_by_day_id=partition_target_table_by_day_id,
                                truncate_partitions=truncate_partitions,
                                commands_before=commands_before, commands_after=commands_after,
                                db_alias=db_alias, timezone=timezone,
                                max_number_of_parallel_tasks=max_number_of_parallel_tasks)
@@ -200,16 +200,16 @@
     def read_command(self, file_name: str) -> pipelines.Command:
         return files.ReadFile(file_name=file_name, compression=self.compression, target_table=self.target_table,
                               mapper_script_file_name=self.mapper_script_file_name, make_unique=self.make_unique,
                               db_alias=self.db_alias, delimiter_char=self.delimiter_char, skip_header=self.skip_header,
                               quote_char=self.quote_char, null_value_string=self.null_value_string,
                               csv_format=self.csv_format, timezone=self.timezone)
 
-    def html_doc_items(self) -> [(str, str)]:
-        path = self.parent.base_path() / self.mapper_script_file_name if self.mapper_script_file_name else ''
+    def html_doc_items(self) -> List[Tuple[str, str]]:
+        path = self.parent.base_path() / self.mapper_script_file_name if self.mapper_script_file_name else pathlib.Path()
         return [('file pattern', _.i[self.file_pattern]),
                 ('compression', _.tt[self.compression]),
                 ('read mode', _.tt[self.read_mode]),
                 ('date regex', _.tt[escape(self.date_regex)] if self.date_regex else None),
                 ('file dependencies', [_.i[dependency, _.br] for dependency in self.file_dependencies]),
                 ('mapper script file name', _.i[self.mapper_script_file_name]),
                 (_.i['mapper script'], html.highlight_syntax(path.read_text().strip('\n')
@@ -227,34 +227,34 @@
                 ('null value string',
                  _.tt[json.dumps(self.null_value_string) if self.null_value_string != None else None]),
                 ('time zone', _.tt[self.timezone])]
 
 
 class ParallelReadSqlite(_ParallelRead):
     def __init__(self, id: str, description: str, file_pattern: str, read_mode: ReadMode, sql_file_name: str,
-                 target_table: str, file_dependencies: [str] = None, date_regex: str = None,
+                 target_table: str, file_dependencies: List[str] = None, date_regex: str = None,
                  partition_target_table_by_day_id: bool = False, truncate_partitions: bool = False,
-                 commands_before: [pipelines.Command] = None, commands_after: [pipelines.Command] = None,
+                 commands_before: List[pipelines.Command] = None, commands_after: List[pipelines.Command] = None,
                  db_alias: str = None, timezone=None, max_number_of_parallel_tasks: int = None) -> None:
         _ParallelRead.__init__(self, id=id, description=description, file_pattern=file_pattern,
                                read_mode=read_mode, target_table=target_table, file_dependencies=file_dependencies,
                                date_regex=date_regex, partition_target_table_by_day_id=partition_target_table_by_day_id,
                                truncate_partitions=truncate_partitions,
                                commands_before=commands_before, commands_after=commands_after, db_alias=db_alias,
                                timezone=timezone, max_number_of_parallel_tasks=max_number_of_parallel_tasks)
         self.sql_file_name = sql_file_name
 
-    def read_command(self, file_name: str) -> [pipelines.Command]:
+    def read_command(self, file_name: str) -> List[pipelines.Command]:
         return files.ReadSQLite(sqlite_file_name=file_name, sql_file_name=self.sql_file_name,
                                 target_table=self.target_table, db_alias=self.db_alias, timezone=self.timezone)
 
     def sql_file_path(self):
         return self.parent.base_path() / self.sql_file_name
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         path = self.sql_file_path()
         return [('file pattern', _.i[self.file_pattern]),
                 ('read mode', _.tt[self.read_mode]),
                 ('date regex', _.tt[escape(self.date_regex)] if self.date_regex else None),
                 ('file dependencies', [_.i[dependency, _.br] for dependency in self.file_dependencies]),
                 ('query file name', _.i[self.sql_file_name]),
                 (_.i['query'], html.highlight_syntax(path.read_text().strip('\n')
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/python.py` & `mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import inspect
 import re
-import typing
+from typing import List, Optional, Tuple, Callable
 from html import escape
 
 from mara_page import _, html
 from .. import pipelines
 from ..commands import python
 
 
 class ParallelExecutePython(pipelines.ParallelTask):
-    def __init__(self, id: str, description: str, file_name: str, parameter_function: typing.Callable,
-                 max_number_of_parallel_tasks: int = None, commands_before: [pipelines.Command] = None,
-                 commands_after: [pipelines.Command] = None) -> None:
+    def __init__(self, id: str, description: str, file_name: str, parameter_function: Callable,
+                 max_number_of_parallel_tasks: Optional[int] = None, commands_before: Optional[List[pipelines.Command]] = None,
+                 commands_after: Optional[List[pipelines.Command]] = None) -> None:
         super().__init__(id=id, description=description, max_number_of_parallel_tasks=max_number_of_parallel_tasks,
                          commands_before=commands_before, commands_after=commands_after)
         self.file_name = file_name
         self.parameter_function = parameter_function
 
     def add_parallel_tasks(self, sub_pipeline: 'pipelines.Pipeline') -> None:
         parameters = self.parameter_function()
@@ -25,28 +25,28 @@
 
         for parameter_tuple in parameters:
             sub_pipeline.add(pipelines.Task(
                 id='_'.join([re.sub('[^0-9a-z\-_]+', '', str(x).lower().replace('-', '_')) for x in parameter_tuple]),
                 description=f'Runs the script with parameters {repr(parameter_tuple)}',
                 commands=[python.ExecutePython(file_name=self.file_name, args=list(parameter_tuple))]))
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         path = self.parent.base_path() / self.file_name
         return [('parameter function',
                  html.highlight_syntax(inspect.getsource(self.parameter_function), 'python')),
                 ('file name', _.i[self.file_name]),
                 (_.i['file content'], html.highlight_syntax(path.read_text().strip('\n')
                                                             if self.file_name and path.exists()
                                                             else '', 'python'))]
 
 
 class ParallelRunFunction(pipelines.ParallelTask):
-    def __init__(self, id: str, description: str, function: typing.Callable, parameter_function: typing.Callable,
-                 max_number_of_parallel_tasks: int = None, commands_before: [pipelines.Command] = None,
-                 commands_after: [pipelines.Command] = None) -> None:
+    def __init__(self, id: str, description: str, function: Callable, parameter_function: Callable,
+                 max_number_of_parallel_tasks: Optional[int] = None, commands_before: Optional[List[pipelines.Command]] = None,
+                 commands_after: Optional[List[pipelines.Command]] = None) -> None:
         super().__init__(id=id, description=description, max_number_of_parallel_tasks=max_number_of_parallel_tasks,
                          commands_before=commands_before, commands_after=commands_after)
         self.function = function
         self.parameter_function = parameter_function
 
     def add_parallel_tasks(self, sub_pipeline: 'pipelines.Pipeline') -> None:
         parameters = self.parameter_function()
@@ -56,12 +56,12 @@
 
         for parameter in parameters:
             sub_pipeline.add(pipelines.Task(
                 id=str(parameter).lower().replace(' ', '_').replace('-', '_'),
                 description=f'Runs the function with parameters {repr(parameter)}',
                 commands=[python.RunFunction(lambda args=parameter: self.function(args))]))
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('function', _.pre[escape(str(self.function))]),
                 ('parameter function',
                  html.highlight_syntax(inspect.getsource(self.parameter_function), 'python')),
                 (_.i['implementation'], html.highlight_syntax(inspect.getsource(self.function), 'python'))]
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/parallel_tasks/sql.py` & `mara-pipelines-3.4.0/mara_pipelines/parallel_tasks/sql.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import inspect
 import re
-import typing
+from typing import Callable, List, Optional, Dict, Tuple
 
 from mara_page import _, html
 from .. import config, pipelines
 from ..commands import sql
 
 
 class ParallelExecuteSQL(pipelines.ParallelTask, sql._SQLCommand):
-    def __init__(self, id: str, description: str, parameter_function: typing.Callable, parameter_placeholders: [str],
-                 max_number_of_parallel_tasks: int = None, sql_statement: str = None, file_name: str = None,
-                 commands_before: [pipelines.Command] = None, commands_after: [pipelines.Command] = None,
-                 db_alias: str = None, echo_queries: bool = None, timezone: str = None,
-                 replace: {str: str} = None) -> None:
+    def __init__(self, id: str, description: str, parameter_function: Callable, parameter_placeholders: List[str],
+                 max_number_of_parallel_tasks: Optional[int] = None, sql_statement: Optional[str] = None, file_name: Optional[str] = None,
+                 commands_before: Optional[List[pipelines.Command]] = None, commands_after: Optional[List[pipelines.Command]] = None,
+                 db_alias: Optional[str] = None, echo_queries: Optional[bool] = None, timezone: Optional[str] = None,
+                 replace: Dict[str, str] = None) -> None:
 
         if (not (sql_statement or file_name)) or (sql_statement and file_name):
             raise ValueError('Please provide either sql_statement or file_name (but not both)')
 
         pipelines.ParallelTask.__init__(self, id=id, description=description,
                                         max_number_of_parallel_tasks=max_number_of_parallel_tasks,
                                         commands_before=commands_before, commands_after=commands_after)
@@ -49,14 +49,14 @@
                 commands=[
                     sql.ExecuteSQL(sql_file_name=self.sql_file_name, db_alias=self.db_alias,
                                    echo_queries=self.echo_queries, timezone=self.timezone, replace=replace)
                     if self.sql_file_name else
                     sql.ExecuteSQL(sql_statement=self.sql_statement, db_alias=self.db_alias,
                                    echo_queries=self.echo_queries, timezone=self.timezone, replace=replace)]))
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         return [('db', _.tt[self.db_alias])] \
                + sql._SQLCommand.html_doc_items(self, self.db_alias) \
                + [('parameter function', html.highlight_syntax(inspect.getsource(self.parameter_function), 'python')),
                   ('parameter placeholders', _.tt[repr(self.parameter_placeholders)]),
                   ('echo queries', _.tt[str(self.echo_queries)]),
                   ('timezone', _.tt[self.timezone or ''])]
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/pipelines.py` & `mara-pipelines-3.4.0/mara_pipelines/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import copy
 import pathlib
 import re
-import typing
+from typing import Optional, Dict, Set, List, Tuple, Union
 
 from . import config
 
 
 class Node():
     """Base class for pipeline elements"""
 
-    def __init__(self, id: str, description: str, labels: {str: str} = None) -> None:
+    def __init__(self, id: str, description: str, labels: Optional[Dict[str, str]] = None) -> None:
         if not re.match('^[a-z0-9_]+$', id):
             raise ValueError(f'Invalid id "{id}". Should only contain lowercase letters, numbers and "_".')
         self.id: str = id
         self.description: str = description
-        self.labels: {str: str} = labels or {}
+        self.labels: Dict[str, str] = labels or {}
 
-        self.upstreams: {'Node'} = set()
-        self.downstreams: {'Node'} = set()
+        self.upstreams: Set[Node] = set()
+        self.downstreams: Set[Node] = set()
 
-        self.parent: typing.Optional['Pipeline'] = None
-        self.cost: typing.Optional[float] = None
+        self.parent: Optional['Pipeline'] = None
+        self.cost: Optional[float] = None
 
 
     def parents(self):
         """Returns all parents of a node from top to bottom"""
         if self.parent:
             return self.parent.parents() + [self]
         else:
             return [self]
 
-    def path(self) -> [str]:
+    def path(self) -> List[str]:
         """Returns a list of ids that identify the node across all pipelines, from top to bottom"""
         return [node.id for node in self.parents()[1:]]
 
     def url_path(self) -> str:
         """Returns a uri fragment for referring to nodes"""
         return '/'.join(self.path()) or None
 
@@ -60,60 +60,60 @@
         """
         from . import shell
         shell_command = self.shell_command()
 
         # logger.log(f'{config.bash_command_string()} -c {shlex.quote(shell_command)}', format=logger.Format.ITALICS)
         return shell.run_shell_command(shell_command)
 
-    def shell_command(self):
+    def shell_command(self) -> str:
         """A bash command string that that runs the command"""
         raise NotImplementedError()
 
     def node_path(self):
         """The path of the parent node"""
         return self.parent.path() if self.parent else ''
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         """
         Things to display in the documentation of a command. Can contain html
         Example: `[('filename','/tmp/foo.txt'), ('max-retries', 15)]`
         """
         raise NotImplementedError()
 
 
 class Task(Node):
-    def __init__(self, id: str, description: str, commands: [Command] = None, max_retries: int = None) -> None:
+    def __init__(self, id: str, description: str, commands: Optional[List[Command]] = None, max_retries: Optional[int] = None) -> None:
         super().__init__(id, description)
         self.commands = []
         self.max_retries = max_retries
 
         for command in commands or []:
             self.add_command(command)
 
     def add_command(self, command: Command, prepend=False):
         if prepend:
             self.commands.insert(0, command)
         else:
             self.commands.append(command)
         command.parent = self
 
-    def add_commands(self, commands: [Command]):
+    def add_commands(self, commands: List[Command]):
         for command in commands:
             self.add_command(command)
 
     def run(self):
         for command in self.commands:
             if not command.run():
                 return False
         return True
 
 
 class ParallelTask(Node):
-    def __init__(self, id: str, description: str, max_number_of_parallel_tasks: int = None,
-                 commands_before: [Command] = None, commands_after: [Command] = None) -> None:
+    def __init__(self, id: str, description: str, max_number_of_parallel_tasks: Optional[int] = None,
+                 commands_before: Optional[List[Command]] = None, commands_after: Optional[List[Command]] = None) -> None:
         super().__init__(id, description)
         self.commands_before = []
         for command in commands_before or []:
             self.add_command_before(command)
         self.commands_after = []
         for command in commands_after or []:
             self.add_command_after(command)
@@ -129,61 +129,63 @@
 
     def add_parallel_tasks(self, sub_pipeline: 'Pipeline') -> None:
         pass
 
     def launch(self) -> 'Pipeline':
         sub_pipeline = Pipeline(self.id, description=f'Runs f{self.id} in parallel',
                                 max_number_of_parallel_tasks=self.max_number_of_parallel_tasks)
-        sub_pipeline.add_initial(Task(id='before', description='Runs commands-before', commands=self.commands_before))
-        sub_pipeline.add_final(Task(id='after', description='Runs commands-after', commands=self.commands_after))
+        if self.commands_before:
+            sub_pipeline.add_initial(Task(id='before', description='Runs commands-before', commands=self.commands_before))
+        if self.commands_after:
+            sub_pipeline.add_final(Task(id='after', description='Runs commands-after', commands=self.commands_after))
 
         self.add_parallel_tasks(sub_pipeline)
 
         return sub_pipeline
 
-    def html_doc_items(self) -> [(str, str)]:
+    def html_doc_items(self) -> List[Tuple[str, str]]:
         """
         Things to display in the documentation of the parallel task. Can contain html.
         Example: `[('filename','/tmp/foo.txt'), ('max-retries', 15)]`
         """
         raise NotImplementedError
 
 
 class Pipeline(Node):
-    nodes: {str: Node} = None
+    """
+    A directed acyclic graph (DAG) of nodes with dependencies between them.
+
+    Args:
+        id: The id of the pipeline
+        description: A short summary of what the pipeline is doing
+        max_number_of_parallel_tasks: Only that many nodes of the pipeline will run in parallel
+        base_path: The absolute path of the pipeline root, file names are relative to that
+        labels: An arbitrary dictionary application specific tags, schemas and so on.
+        ignore_errors: When true, then the pipeline execution will not fail when a child node fails
+        force_run_all_children: When true, child nodes will run even when their upstreams failed
+    """
+    nodes: Dict[str, Node] = None
     initial_node: Node = None
     final_node: Node = None
 
     def __init__(self, id: str,
                  description: str,
                  max_number_of_parallel_tasks: int = None,
                  base_path: pathlib.Path = None,
-                 labels: {str: str} = None,
+                 labels: Dict[str, str] = None,
                  ignore_errors: bool = False,
                  force_run_all_children: bool = False) -> None:
-        """
-        A directed acyclic graph (DAG) of nodes with dependencies between them.
-
-        Args:
-            id: The id of the pipeline
-            description: A short summary of what the pipeline is doing
-            max_number_of_parallel_tasks: Only that many nodes of the pipeline will run in parallel
-            base_path: The absolute path of the pipeline root, file names are relative to that
-            labels: An arbitrary dictionary application specific tags, schemas and so on.
-            ignore_errors: When true, then the pipeline execution will not fail when a child node fails
-            force_run_all_children: When true, child nodes will run even when their upstreams failed
-        """
         super().__init__(id, description, labels)
         self.nodes = {}
         self._base_path = base_path
         self.max_number_of_parallel_tasks = max_number_of_parallel_tasks
         self.force_run_all_children = force_run_all_children
         self.ignore_errors = ignore_errors
 
-    def add(self, node: Node, upstreams: [typing.Union[str, Node]] = None) -> 'Pipeline':
+    def add(self, node: Node, upstreams: Optional[List[Union[str, Node]]] = None) -> 'Pipeline':
         if node.id in self.nodes:
             raise ValueError(f'A node with id "{node.id}" already exists in pipeline "{self.id}"')
 
         self.nodes[node.id] = node
         node.parent = self
 
         for upstream in upstreams or []:
@@ -236,15 +238,15 @@
 
         for downstream in copy.copy(node.downstreams):
             self.add_dependency(new_node, downstream)
 
         self.remove(node)
         self.add(new_node)
 
-    def add_dependency(self, upstream: typing.Union[Node, str], downstream: typing.Union[Node, str]):
+    def add_dependency(self, upstream: Union[Node, str], downstream: Union[Node, str]):
         if isinstance(upstream, str):
             if not upstream in self.nodes:
                 raise KeyError(f'Node "{upstream}" not found in pipeline "{self.id}"')
             upstream = self.nodes[upstream]
 
         if isinstance(downstream, str):
             if not downstream in self.nodes:
@@ -278,15 +280,15 @@
                 self.add_dependency(upstream, node)
         self.add(node)
 
     def base_path(self):
         return self._base_path or (self.parent.base_path() if self.parent else pathlib.Path('.'))
 
 
-def find_node(path: [str]) -> (Node, bool):
+def find_node(path: List[str]) -> Tuple[Node, bool]:
     """
     Retrieves a node by the the path from its parents
     Args:
         path: The ids of the node and of all its parent, from top to bottom
 
     Returns:
         A tuple of the node and True if the node was found, or a the closest known parent node if and False otherwise
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/cli.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Command line interface for running data pipelines"""
 
 import sys
+from typing import Set
 
 import click
 
 from .. import config, pipelines
 
 
-def run_pipeline(pipeline: pipelines.Pipeline, nodes: {pipelines.Node} = None,
+def run_pipeline(pipeline: pipelines.Pipeline, nodes: Set[pipelines.Node] = None,
                  with_upstreams: bool = False,
                  interactively_started: bool = False,
                  disable_colors: bool = False) -> bool:
     """
     Runs a pipeline or parts of it with output printed to stdout
     Args:
         pipeline: The pipeline to run
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/dependency_graph.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/dependency_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Visualization of pipelines using graphviz"""
 
 import functools
+from typing import Dict
 
 import flask
 
 from mara_page import acl, html, bootstrap, _
 from . import views
 from .. import pipelines
 
@@ -26,15 +27,15 @@
     if not found:
         flask.abort(404, f'Node "{path}" not found')
 
     return dependency_graph(node)
 
 
 @functools.singledispatch
-def dependency_graph(nodes: {str: pipelines.Node},
+def dependency_graph(nodes: Dict[str, pipelines.Node],
                      current_node: pipelines.Node = None) -> str:
     """
     Draws a list of pipeline nodes and the dependencies between them using graphviz
 
     Args:
         nodes: The nodes to render
         current_node: If not null, then this node is highlighted
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/last_runs.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/last_runs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Functions for visualizing the last runs of a pipeline node"""
 
 import datetime
 import json
+from typing import List
 
 import flask
-import psycopg2.extensions
 
-import mara_db.postgresql
+import mara_db.dbs
 from mara_page import bootstrap, html, acl, _
 from . import views
 from .. import config, pipelines
 
 
 def card(node: pipelines.Node) -> str:
     """A card that shows the system stats, the time line and output for the last runs or a node"""
@@ -49,15 +49,15 @@
     Returns:
         A `<select..><option ../><option ../></select>` element
     """
     from ..logging import node_cost
 
     node, __ = pipelines.find_node(path.split('/'))
 
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 SELECT
   run_id,
   to_char(start_time, 'Mon DD HH24:MI') AS start_time,
   extract(EPOCH FROM (end_time - start_time)) AS duration,
   succeeded
 FROM data_integration_node_run
@@ -99,15 +99,15 @@
 
     run_id = run_id or _latest_run_id(node.path())
 
     if not run_id:
         return ''
 
     line_limit = 1000
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 SELECT node_path, message, format, is_error
 FROM data_integration_node_run
   JOIN data_integration_node_output USING (node_run_id)
 WHERE node_path [1:{"%s"}] = %s
       AND run_id = %s
 ORDER BY timestamp
@@ -133,15 +133,15 @@
     node, __ = pipelines.find_node(path.split('/'))
 
     run_id = run_id or _latest_run_id(node.path())
 
     if not run_id:
         return ''
 
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 SELECT
   -- needs to be spelled out to be able to rely on the order in the postprocessing of the row
   -- run_id is not needed in the frontend...
   stats.timestamp,
   stats.disc_read,
   stats.disc_write,
@@ -174,15 +174,15 @@
     node, __ = pipelines.find_node(path.split('/'))
 
     run_id = run_id or _latest_run_id(node.path())
 
     if not run_id:
         return ''
 
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(f'''
 SELECT node_path, start_time, end_time, max(end_time) over () AS max_end_time, succeeded, is_pipeline
 FROM data_integration_node_run
 WHERE node_path [1 :{'%(level)s'}] = {'%(node_path)s'}
       AND array_length(node_path, 1) > {'%(level)s'}
       AND run_id = {'%(run_id)s'};''', {'level': len(node.path()), 'node_path': node.path(), 'run_id': run_id})
 
@@ -197,11 +197,11 @@
 
         if nodes:
             return str(_.script[f"drawTimelineChart('timeline-chart', {json.dumps(nodes)})"])
         else:
             return ''
 
 
-def _latest_run_id(node_path: [str]):
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+def _latest_run_id(node_path: List[str]):
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute('SELECT max(run_id) FROM data_integration_node_run WHERE node_path=%s', (node_path,))
         return cursor.fetchone()[0]
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/node_page.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/node_page.py`

 * *Files identical despite different names*

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/run_page.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/run_page.py`

 * *Files identical despite different names*

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/run_time_chart.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/run_time_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import pathlib
 
 import flask
-import psycopg2.extensions
 
 import mara_db.config
-import mara_db.postgresql
+import mara_db.dbs
 from mara_page import acl, bootstrap, html, _
 from . import views
 from .. import pipelines
 
 
 def card(node: pipelines.Node):
     """A card that shows the duration of the node and its top children over time"""
@@ -25,15 +24,15 @@
 def run_time_chart(path: str):
     node, found = pipelines.find_node(path.split('/'))
     if not found:
         flask.abort(404, f'Node "{path}" not found')
 
     query = (pathlib.Path(__file__).parent / 'run_time_chart.sql').read_text()
 
-    with mara_db.postgresql.postgres_cursor_context('mara') as cursor:  # type: psycopg2.extensions.cursor
+    with mara_db.dbs.cursor_context('mara') as cursor:
         cursor.execute(query)
         cursor.execute(f'SELECT row_to_json(t) FROM pg_temp.node_run_times({"%s"}) t', (node.path(),))
         rows = [row[0] for row in cursor.fetchall()]
 
         if rows and len(rows) > 1:
             number_of_child_runs = len(rows[0]['child_runs']) if rows[0]['child_runs'] else 0
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/run_time_chart.sql` & `mara-pipelines-3.4.0/mara_pipelines/ui/run_time_chart.sql`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,7 @@
 ORDER BY all_runs.run_id;
 
 $$
   LANGUAGE SQL;
 
 -- SELECT *
 -- FROM pg_temp.node_run_times(ARRAY [] :: TEXT []);
-
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/common.css` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/common.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     font-style: italic;
     color: #888;
 }
 
 .run-output > div > span.verbatim {
     font-family: "Courier", monospace;
     color: #222;
-}
+}
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/kolorwheel.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/kolorwheel.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -552,8 +552,8 @@
 00002270: 7452 6762 2829 3b0a 2020 2020 7661 7220  tRgb();.    var 
 00002280: 6c75 6d20 3d20 2830 2e32 3939 202a 2072  lum = (0.299 * r
 00002290: 6762 5b30 5d29 202b 2028 302e 3538 3720  gb[0]) + (0.587 
 000022a0: 2a20 7267 625b 315d 2920 2b20 2830 2e31  * rgb[1]) + (0.1
 000022b0: 3134 202a 2072 6762 5b32 5d29 3b0a 0a20  14 * rgb[2]);.. 
 000022c0: 2020 2072 6574 7572 6e20 286c 756d 203e     return (lum >
 000022d0: 2031 3237 293b 0a7d 3b20 2f2f 2069 734c   127);.}; // isL
-000022e0: 6967 6874 2829                           ight()
+000022e0: 6967 6874 2829 0a                        ight().
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/node-page.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/node-page.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 2% similar despite different names*

```diff
@@ -208,9 +208,8 @@
 00000cf0: 6453 7973 7465 6d53 7461 7473 286e 6f64  dSystemStats(nod
 00000d00: 6555 726c 5061 7468 293b 0a20 2020 2020  eUrlPath);.     
 00000d10: 2020 2020 2020 206c 6f61 6454 696d 656c         loadTimel
 00000d20: 696e 6528 6e6f 6465 5572 6c50 6174 6829  ine(nodeUrlPath)
 00000d30: 3b0a 2020 2020 2020 2020 2020 2020 6c6f  ;.            lo
 00000d40: 6164 4f75 7470 7574 286e 6f64 6555 726c  adOutput(nodeUrl
 00000d50: 5061 7468 2c20 7472 7565 293b 0a20 2020  Path, true);.   
-00000d60: 2020 2020 207d 0a20 2020 207d 0a7d 0a0a       }.    }.}..
-00000d70: 0a0a 0a                                  ...
+00000d60: 2020 2020 207d 0a20 2020 207d 0a7d 0a         }.    }.}.
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/run-page.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/run-page.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -384,8 +384,8 @@
 000017f0: 6768 7427 2c20 6865 6967 6874 293b 0a20  ght', height);. 
 00001800: 2020 2020 2020 206d 6169 6e4f 7574 7075         mainOutpu
 00001810: 7441 7265 612e 6373 7328 276d 696e 2d68  tArea.css('min-h
 00001820: 6569 6768 7427 2c20 6865 6967 6874 293b  eight', height);
 00001830: 0a20 2020 207d 0a0a 2020 2020 2428 7769  .    }..    $(wi
 00001840: 6e64 6f77 292e 7265 7369 7a65 2872 6573  ndow).resize(res
 00001850: 697a 6529 3b0a 0a20 2020 2072 6573 697a  ize);..    resiz
-00001860: 6528 293b 0a7d                           e();.}
+00001860: 6528 293b 0a7d 0a                        e();.}.
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/run-time-chart.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/run-time-chart.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -239,8 +239,8 @@
 00000ee0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
 00000ef0: 2020 2020 7d29 3b0a 0a20 2020 2020 2020      });..       
 00000f00: 2024 2877 696e 646f 7729 2e72 6573 697a   $(window).resiz
 00000f10: 6528 6675 6e63 7469 6f6e 2028 2920 7b0a  e(function () {.
 00000f20: 2020 2020 2020 2020 2020 2020 6368 6172              char
 00000f30: 742e 6472 6177 2864 6174 612c 206f 7074  t.draw(data, opt
 00000f40: 696f 6e73 293b 0a20 2020 2020 2020 207d  ions);.        }
-00000f50: 293b 0a20 2020 207d 0a7d 0a0a 0a         );.    }.}...
+00000f50: 293b 0a20 2020 207d 0a7d 0a              );.    }.}.
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/system-stats-chart.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/system-stats-chart.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -262,8 +262,8 @@
 00001050: 6461 7461 2c20 6f70 7469 6f6e 7329 3b0a  data, options);.
 00001060: 2020 2020 2020 2020 2020 2020 7d20 656c              } el
 00001070: 7365 207b 0a20 2020 2020 2020 2020 2020  se {.           
 00001080: 2020 2020 2069 6e69 7469 616c 526f 7773       initialRows
 00001090: 203d 2070 726f 6365 7373 6564 5f72 6f77   = processed_row
 000010a0: 733b 0a20 2020 2020 2020 2020 2020 207d  s;.            }
 000010b0: 0a20 2020 2020 2020 207d 0a20 2020 207d  .        }.    }
-000010c0: 3b0a 7d3b 0a0a                           ;.};..
+000010c0: 3b0a 7d3b 0a                             ;.};.
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/timeline-chart.css` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/timeline-chart.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 div.timeline > div.timeline-grid-line {
     position: absolute;
     top: 0px;
     height: 100%;
     width: 1px;
     border-left: 1px dashed #888;
     z-index: 0;
-}
+}
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/timeline-chart.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/timeline-chart.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 1% similar despite different names*

```diff
@@ -235,8 +235,8 @@
 00000ea0: 2020 2020 7d0a 0a20 2020 2064 7261 7728      }..    draw(
 00000eb0: 293b 0a20 2020 2077 696e 646f 772e 7265  );.    window.re
 00000ec0: 7175 6573 7441 6e69 6d61 7469 6f6e 4672  questAnimationFr
 00000ed0: 616d 6528 6472 6177 293b 0a0a 2020 2020  ame(draw);..    
 00000ee0: 2428 7769 6e64 6f77 292e 7265 7369 7a65  $(window).resize
 00000ef0: 2866 756e 6374 696f 6e20 2829 207b 0a20  (function () {. 
 00000f00: 2020 2020 2020 2064 7261 7728 293b 0a20         draw();. 
-00000f10: 2020 207d 293b 0a7d 0a0a 0a                 });.}...
+00000f10: 2020 207d 293b 0a7d 0a                      });.}.
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/static/utils.js` & `mara-pipelines-3.4.0/mara_pipelines/ui/static/utils.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -220,8 +220,8 @@
 00000db0: 7375 6666 6978 293b 0a20 2020 2020 2020  suffix);.       
 00000dc0: 207d 0a20 2020 207d 0a20 2020 202f 2f20   }.    }.    // 
 00000dd0: 6279 2064 6566 6175 6c74 2c20 6469 7370  by default, disp
 00000de0: 6c61 7920 6461 7973 0a20 2020 2072 6574  lay days.    ret
 00000df0: 7572 6e20 6765 6e65 7261 7465 5f74 6963  urn generate_tic
 00000e00: 6b73 2831 2c20 3234 202a 2036 3020 2a20  ks(1, 24 * 60 * 
 00000e10: 3630 202a 2031 3030 302c 2027 6427 293b  60 * 1000, 'd');
-00000e20: 0a0a 7d0a 0a                             ..}..
+00000e20: 0a0a 7d0a                                ..}.
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines/ui/views.py` & `mara-pipelines-3.4.0/mara_pipelines/ui/views.py`

 * *Files identical despite different names*

### Comparing `mara-pipelines-3.3.0/mara_pipelines.egg-info/PKG-INFO` & `mara-pipelines-3.4.0/mara_pipelines.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mara-pipelines
-Version: 3.3.0
+Version: 3.4.0
 Summary: Opinionated lightweight ELT pipeline framework
 Home-page: https://github.com/mara/mara-pipelines
 Author: Mara contributors
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Mara Pipelines
 
 [![Build & Test](https://github.com/mara/mara-pipelines/actions/workflows/build.yaml/badge.svg)](https://github.com/mara/mara-pipelines/actions/workflows/build.yaml)
-[![PyPI - License](https://img.shields.io/pypi/l/mara-pipelines.svg)](https://github.com/mara/mara-pipelines/blob/master/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/mara-pipelines.svg)](https://github.com/mara/mara-pipelines/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/mara-pipelines.svg)](https://badge.fury.io/py/mara-pipelines)
 [![Slack Status](https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social)](https://communityinviter.com/apps/mara-users/public-invite)
 
 
 
 This package contains a lightweight data transformation framework with a focus on transparency and complexity reduction. It has a number of baked-in assumptions/ principles:
 
@@ -42,22 +42,22 @@
 To use the library directly, use pip:
 
 ```
 pip install mara-pipelines
 ```
 
 or
- 
+
 ```
 pip install git+https://github.com/mara/mara-pipelines.git
 ```
 
 For an example of an integration into a flask application, have a look at the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2).
 
-Due to the heavy use of forking, Mara Pipelines does not run natively on Windows. If you want to run it on Windows, then please use Docker or the [Windows Subsystem for Linux](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux). 
+Due to the heavy use of forking, Mara Pipelines does not run natively on Windows. If you want to run it on Windows, then please use Docker or the [Windows Subsystem for Linux](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux).
 
 &nbsp;
 
 ## Example
 
 Here is a pipeline "demo" consisting of three nodes that depend on each other: the task `ping_localhost`, the pipeline `sub_pipeline` and the task `sleep`:
 
@@ -85,19 +85,19 @@
 
 pipeline.add(sub_pipeline, ['ping_localhost'])
 
 pipeline.add(Task(id='sleep', description='Sleeps for 2 seconds',
                   commands=[RunBash('sleep 2')]), ['sub_pipeline'])
 ```
 
-Tasks contain lists of commands, which do the actual work (in this case running bash commands that ping various hosts). 
+Tasks contain lists of commands, which do the actual work (in this case running bash commands that ping various hosts).
 
 &nbsp;
 
-In order to run the pipeline, a PostgreSQL database needs to be configured for storing run-time information, run output and status of incremental processing: 
+In order to run the pipeline, a PostgreSQL database is recommended to be configured for storing run-time information, run output and status of incremental processing:
 
 ```python
 import mara_db.auto_migration
 import mara_db.config
 import mara_db.dbs
 
 mara_db.config.databases \
@@ -108,18 +108,18 @@
 
 Given that PostgresSQL is running and the credentials work, the output looks like this (a database with a number of tables is created):
 
 ```
 Created database "postgresql+psycopg2://root@localhost/example_etl_mara"
 
 CREATE TABLE data_integration_file_dependency (
-    node_path TEXT[] NOT NULL, 
-    dependency_type VARCHAR NOT NULL, 
-    hash VARCHAR, 
-    timestamp TIMESTAMP WITHOUT TIME ZONE, 
+    node_path TEXT[] NOT NULL,
+    dependency_type VARCHAR NOT NULL,
+    hash VARCHAR,
+    timestamp TIMESTAMP WITHOUT TIME ZONE,
     PRIMARY KEY (node_path, dependency_type)
 );
 
 .. more tables
 ```
 
 ### CLI UI
@@ -128,38 +128,38 @@
 
 ```python
 from mara_pipelines.ui.cli import run_pipeline
 
 run_pipeline(pipeline)
 ```
 
-![Example run cli 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-1.gif)
+![Example run cli 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-1.gif)
 
 &nbsp;
 
 And this runs a single node of pipeline `sub_pipeline` together with all the nodes that it depends on:
 
 ```python
 run_pipeline(sub_pipeline, nodes=[sub_pipeline.nodes['ping_amazon']], with_upstreams=True)
 ```
 
-![Example run cli 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-2.gif)
+![Example run cli 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-2.gif)
 
 &nbsp;
 
 
 And finally, there is some sort of menu based on [pythondialog](http://pythondialog.sourceforge.net/) that allows to navigate and run pipelines like this:
 
 ```python
 from mara_pipelines.ui.cli import run_interactively
 
 run_interactively()
 ```
 
-![Example run cli 3](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-cli-3.gif)
+![Example run cli 3](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-cli-3.gif)
 
 
 
 ### Web UI
 
 More importantly, this package provides an extensive web interface. It can be easily integrated into any [Flask](https://flask.palletsprojects.com/) based app and the [mara example project](https://github.com/mara/mara-example-project) demonstrates how to do this using [mara-app](https://github.com/mara/mara-app).
 
@@ -167,30 +167,36 @@
 
 - a graph of all child nodes and the dependencies between them
 - a chart of the overal run time of the pipeline and it's most expensive nodes over the last 30 days (configurable)
 - a table of all the pipeline's nodes with their average run times and the resulting queuing priority
 - output and timeline for the last runs of the pipeline
 
 
-![Mara pipelines web ui 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/mara-pipelines-web-ui-1.png)
+![Mara pipelines web ui 1](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/mara-pipelines-web-ui-1.png)
 
-For each task, there is a page showing 
+For each task, there is a page showing
 
 - the upstreams and downstreams of the task in the pipeline
 - the run times of the task in the last 30 days
 - all commands of the task
 - output of the last runs of the task
 
-![Mara pipelines web ui 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/mara-pipelines-web-ui-2.png)
+![Mara pipelines web ui 2](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/mara-pipelines-web-ui-2.png)
 
 
-Pipelines and tasks can be run from the web ui directly, which is probably one of the main features of this package: 
+Pipelines and tasks can be run from the web ui directly, which is probably one of the main features of this package:
 
-![Example run web ui](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/example-run-web-ui.gif)
+![Example run web ui](https://github.com/mara/mara-pipelines/raw/3.2.x/docs/_static/example-run-web-ui.gif)
 
 &nbsp;
 
-# Getting started
+## Getting started
 
-Documentation is currently work in progress. Please use the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2) as a reference for getting started. 
+Documentation is currently work in progress. Please use the [mara example project 1](https://github.com/mara/mara-example-project-1) and [mara example project 2](https://github.com/mara/mara-example-project-2) as a reference for getting started.
 
+## Links
 
+* Documentation: https://mara-pipelines.readthedocs.io/
+* Changes: https://mara-pipelines.readthedocs.io/en/latest/changes.html
+* PyPI Releases: https://pypi.org/project/mara-pipelines/
+* Source Code: https://github.com/mara/mara-pipelines
+* Issue Tracker: https://github.com/mara/mara-pipelines/issues
```

### Comparing `mara-pipelines-3.3.0/mara_pipelines.egg-info/SOURCES.txt` & `mara-pipelines-3.4.0/mara_pipelines.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 mara_pipelines.egg-info/SOURCES.txt
 mara_pipelines.egg-info/dependency_links.txt
 mara_pipelines.egg-info/requires.txt
 mara_pipelines.egg-info/top_level.txt
 mara_pipelines/commands/__init__.py
 mara_pipelines/commands/bash.py
 mara_pipelines/commands/files.py
+mara_pipelines/commands/http.py
 mara_pipelines/commands/python.py
 mara_pipelines/commands/sql.py
 mara_pipelines/incremental_processing/__init__.py
 mara_pipelines/incremental_processing/file_dependencies.py
 mara_pipelines/incremental_processing/incremental_copy_status.py
 mara_pipelines/incremental_processing/processed_files.py
 mara_pipelines/incremental_processing/reset.py
@@ -53,8 +54,9 @@
 mara_pipelines/ui/static/node-page.js
 mara_pipelines/ui/static/run-page.css
 mara_pipelines/ui/static/run-page.js
 mara_pipelines/ui/static/run-time-chart.js
 mara_pipelines/ui/static/system-stats-chart.js
 mara_pipelines/ui/static/timeline-chart.css
 mara_pipelines/ui/static/timeline-chart.js
-mara_pipelines/ui/static/utils.js
+mara_pipelines/ui/static/utils.js
+tests/test_execute_pipeline.py
```

### Comparing `mara-pipelines-3.3.0/setup.cfg` & `mara-pipelines-3.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 author = Mara contributors
 license = MIT
 
 [options]
 packages = mara_pipelines
 python_requires = >= 3.6
 install_requires = 
-	mara-db>=4.7.1
-	mara-page>=1.3.0
+	mara-db>=4.9.1
+	mara-page>=1.7.0
 	graphviz>=0.8
 	python-dateutil>=2.6.1
 	pythondialog>=3.4.0
 	more-itertools>=3.1.0
 	psutil>=5.4.0
 	requests>=2.19.1
+	SQLAlchemy>=1.4
 
 [options.package_data]
 mara_pipelines = **/*.py, **/*.sql, ui/static/*
 
 [options.extras_require]
 test = 
 	pytest
+	pytest-docker
+	pytest-dependency
 	mara_app>=1.5.2
+	mara-db[postgres,mssql]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

