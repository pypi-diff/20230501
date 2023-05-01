# Comparing `tmp/globus-compute-endpoint-2.0.1a4.tar.gz` & `tmp/globus-compute-endpoint-2.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.1a4.tar", last modified: Thu Apr 20 15:07:51 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.2a0.tar", last modified: Mon May  1 15:14:39 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.1a4.tar` & `globus-compute-endpoint-2.0.2a0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.234129 globus-compute-endpoint-2.0.1a4/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.1a4/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-20 15:07:51.234213 globus-compute-endpoint-2.0.1a4/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.1a4/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.226309 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    19298 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.228979 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    24838 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.229728 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.230025 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.230172 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.232028 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.232268 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.232649 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.233367 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-20 15:03:56.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.227092 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2657 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      308 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-20 15:07:51.234479 globus-compute-endpoint-2.0.1a4/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3635 2023-04-20 15:03:52.000000 globus-compute-endpoint-2.0.1a4/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.233987 globus-compute-endpoint-2.0.1a4/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a4/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.999767 globus-compute-endpoint-2.0.2a0/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.2a0/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-05-01 15:14:38.999832 globus-compute-endpoint-2.0.2a0/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.2a0/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.993466 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    19300 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.995486 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24838 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.996174 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.996431 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.996564 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.998079 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    49946 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    36234 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.998216 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.998604 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.999264 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5470 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-05-01 15:05:29.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.994151 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2657 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      308 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-05-01 15:14:39.000067 globus-compute-endpoint-2.0.2a0/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3635 2023-05-01 15:05:24.000000 globus-compute-endpoint-2.0.2a0/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.999624 globus-compute-endpoint-2.0.2a0/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.0.2a0/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.1a4/LICENSE` & `globus-compute-endpoint-2.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/PKG-INFO` & `globus-compute-endpoint-2.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a4
+Version: 2.0.2a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.0.1a4/PyPI.md` & `globus-compute-endpoint-2.0.2a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,17 +362,17 @@
         raise ClickException(msg) from err
 
 
 def read_config(endpoint_dir: pathlib.Path) -> Config:
     endpoint_name = endpoint_dir.name
 
     try:
-        import funcx_endpoint
+        from funcx_endpoint.version import VERSION
 
-        if Version(funcx_endpoint.__version__) < Version("2.0.0"):
+        if Version(VERSION) < Version("2.0.0"):
             msg = (
                 "To avoid compatibility issues with Globus Compute, please uninstall "
                 "funcx-endpoint or upgrade funcx-endpoint to >=2.0.0. Note that the "
                 "funcx-endpoint package is now deprecated."
             )
             raise ClickException(msg)
     except ModuleNotFoundError:
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,14 @@
         # Set proportions of workers equal to the proportion of queue size.
         for q_type in q_sizes:
             ratio = q_sizes[q_type] / sum_q_size
             new_worker_map[q_type] = min(
                 int(math.floor(ratio * max_workers)), q_sizes[q_type]
             )
 
-        # CLEANUP: Assign the difference here to any random worker. Should be small.
-        # log.debug("Temporary new worker map: {}".format(new_worker_map))
-
         # Check the difference
         tmp_sum_q_size = sum(new_worker_map.values())
         difference = 0
         if sum_q_size > tmp_sum_q_size:
             difference = min(max_workers - tmp_sum_q_size, sum_q_size - tmp_sum_q_size)
         log.debug(f"Offset difference: {difference}")
         log.debug(f"Queue Types: {q_types}")
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import argparse
 import collections
+import copy
 import json
 import logging
 import os
 import platform
 import queue
 import signal
 import sys
 import threading
 import time
 import typing as t
+from collections import defaultdict
 
 import daemon
 import dill
 import zmq
 from globus_compute_common.messagepack.message_types import TaskTransition
 from globus_compute_common.tasks import ActorName, TaskState
 from globus_compute_endpoint.exception_handling import (
@@ -29,14 +31,15 @@
     BadCommand,
     EPStatusReport,
     Heartbeat,
     Message,
     MessageType,
 )
 from globus_compute_endpoint.logging_config import ComputeLogger
+from globus_compute_sdk.sdk.utils import chunk_by
 from globus_compute_sdk.serialize import ComputeSerializer
 from parsl.version import VERSION as PARSL_VERSION
 
 if t.TYPE_CHECKING:
     import multiprocessing as mp
 
 log: ComputeLogger = logging.getLogger(__name__)  # type: ignore
@@ -332,15 +335,16 @@
             self.load_config()
         except Exception:
             log.exception("Caught exception")
             raise
 
         self.task_cancel_running_queue: queue.Queue = queue.Queue()
         self.task_cancel_pending_trap: dict[str, str] = {}
-        self.task_status_deltas: dict[str, list[TaskTransition]] = {}
+        self.task_status_deltas: dict[str, list[TaskTransition]] = defaultdict(list)
+        self._task_status_delta_lock = threading.Lock()
         self.container_switch_count: dict[bytes, int] = {}
 
     def load_config(self):
         """Load the config"""
         log.info("Loading endpoint local config")
         working_dir = self.working_dir
         if self.working_dir is None:
@@ -456,18 +460,16 @@
                 self.total_pending_task_count += 1
                 tt = TaskTransition(
                     timestamp=time.time_ns(),
                     state=TaskState.WAITING_FOR_NODES,
                     actor=ActorName.INTERCHANGE,
                 )
 
-                self.task_status_deltas[msg.task_id] = self.task_status_deltas.get(
-                    msg.task_id, []
-                )
-                self.task_status_deltas[msg.task_id].append(tt)
+                with self._task_status_delta_lock:
+                    self.task_status_deltas[msg.task_id].append(tt)
 
                 log.debug(
                     f"[TASK_PULL_THREAD] task {msg.task_id} is now WAITING_FOR_NODES"
                 )
                 log.debug(
                     "[TASK_PULL_THREAD] pending task count: {}".format(
                         self.total_pending_task_count
@@ -547,27 +549,41 @@
         manager : str
           Manager id to be put on hold while being killed
         """
         if manager in self._ready_manager_queue:
             self._ready_manager_queue[manager]["active"] = False
 
     def _status_report_loop(self, kill_event, status_report_queue: queue.Queue):
-        log.debug("Status reporting loop starting")
         log.info(f"Endpoint id: {self.endpoint_id}")
 
         while True:
-            log.trace("Endpoint id : %s, %s", self.endpoint_id, type(self.endpoint_id))
-            msg = EPStatusReport(
-                self.endpoint_id,
-                self.get_global_state_for_status_report(),
-                self.task_status_deltas,
+            with self._task_status_delta_lock:
+                task_status_deltas = copy.deepcopy(self.task_status_deltas)
+                self.task_status_deltas.clear()
+
+            log.debug(
+                "Cleared task deltas (%s); sending status report to executor.",
+                len(task_status_deltas),
             )
-            log.debug("Sending status report to executor, and clearing task deltas.")
-            status_report_queue.put(msg.pack())
-            self.task_status_deltas.clear()
+
+            # The result processor will gracefully handle any size message, but
+            # courtesy says to chunk work; 4,096 is empirically chosen to be plenty
+            # "bulk enough," but not rude.
+            for tsd_chunk in chunk_by(task_status_deltas.items(), 4_096):
+                try:
+                    msg = EPStatusReport(
+                        self.endpoint_id,
+                        self.get_global_state_for_status_report(),
+                        dict(tsd_chunk),
+                    )
+                    status_report_queue.put(msg.pack())
+                except Exception:
+                    log.exception("Unable to create or send EP status report.")
+                    log.debug("Attempted to send chunk: %s", tsd_chunk)
+                    # ignoring so that the thread continues; "it's just a status"
 
             if kill_event.wait(self.heartbeat_period):
                 break
 
     def _command_server(self, kill_event):
         """Command server to run async command to the interchange
 
@@ -715,14 +731,16 @@
         # switch
         # Cold routing is to reduce the number idle workers of specific task types on
         # the managers when there are not enough tasks of those types in the task queues
         # on interchange
         last_cold_routing_time = time.time()
         prev_manager_stat = None
 
+        task_deltas_to_merge: dict[str, list[TaskTransition]] = defaultdict(list)
+
         while not self._kill_event.is_set():
             self.socks = dict(poller.poll(timeout=poll_period))
 
             # Listen for requests for work
             if (
                 self.task_outgoing in self.socks
                 and self.socks[self.task_outgoing] == zmq.POLLIN
@@ -754,17 +772,19 @@
                         "max_worker_count": 0,
                         "active": True,
                         "tasks": collections.defaultdict(set),
                         "total_tasks": 0,
                     }
                     if reg_flag is True:
                         interesting_managers.add(manager)
-                        log.info(f"Adding manager: {manager!r} to ready queue")
+                        log.info(
+                            f"Add manager to ready queue: {manager!r}"
+                            f"\n  Registration info: {msg})"
+                        )
                         mdata.update(msg)
-                        log.info(f"Registration info for manager {manager!r}: {msg}")
                         self._ready_manager_queue[manager] = mdata
 
                         if (
                             msg["python_v"].rsplit(".", 1)[0]
                             != self.current_platform["python_v"].rsplit(".", 1)[0]
                             or msg["parsl_v"] != self.current_platform["parsl_v"]
                         ):
@@ -876,16 +896,21 @@
                         else:
                             log.debug("Task:%s is now WAITING_FOR_LAUNCH", task_id)
                             tt = TaskTransition(
                                 timestamp=time.time_ns(),
                                 state=TaskState.WAITING_FOR_LAUNCH,
                                 actor=ActorName.INTERCHANGE,
                             )
-                            self.task_status_deltas.setdefault(task_id, [])
-                            self.task_status_deltas[task_id].append(tt)
+                            task_deltas_to_merge[task_id].append(tt)
+
+            if task_deltas_to_merge:
+                with self._task_status_delta_lock:
+                    for task_id, deltas in task_deltas_to_merge.items():
+                        self.task_status_deltas[task_id].extend(deltas)
+                task_deltas_to_merge.clear()
 
             # Receive any results and forward to client
             if (
                 self.results_incoming in self.socks
                 and self.socks[self.results_incoming] == zmq.POLLIN
             ):
                 log.debug("entering results_incoming section")
@@ -904,20 +929,16 @@
                         manager_report = Message.unpack(b_messages[0])
                         if manager_report.task_statuses:
                             log.info(
                                 "Got manager status report: %s",
                                 manager_report.task_statuses,
                             )
 
-                        # merge the two dicts of statuses
-                        for tid, statuses in manager_report.task_statuses.items():
-                            if tid in self.task_status_deltas.keys():
-                                self.task_status_deltas[tid] += statuses
-                            else:
-                                self.task_status_deltas[tid] = statuses
+                            for tid, statuses in manager_report.task_statuses.items():
+                                task_deltas_to_merge[tid].extend(statuses)
 
                         self.task_outgoing.send_multipart(
                             [manager, b"", PKL_HEARTBEAT_CODE]
                         )
                         b_messages = b_messages[1:]
                         mdata["last"] = time.time()
                         self.container_switch_count[
@@ -927,41 +948,44 @@
                             "Got container switch count: %s",
                             self.container_switch_count,
                         )
                     except Exception:
                         pass
                     if len(b_messages):
                         log.info(f"Got {len(b_messages)} result items in batch")
-                    for idx, b_message in enumerate(b_messages):
-                        r = dill.loads(b_message)
-
-                        log.debug(
-                            "Received task result %s (from %s)", r["task_id"], manager
-                        )
-                        task_container = self.containers[r["container_id"]]
-                        log.debug(
-                            "Removing for manager: %s from %s",
-                            manager,
-                            self._ready_manager_queue,
-                        )
-
-                        mdata["tasks"][task_container].remove(r["task_id"])
-
-                        # Transfer any outstanding task statuses to the result message
-                        if r["task_id"] in self.task_status_deltas:
-                            r["task_statuses"] += self.task_status_deltas[r["task_id"]]
-                            b_messages[idx] = dill.dumps(r)
-                            log.debug(
-                                "Transferring statuses for %s: %s",
-                                r["task_id"],
-                                r["task_statuses"],
-                            )
-                            del self.task_status_deltas[r["task_id"]]
+                        with self._task_status_delta_lock:
+                            for idx, b_message in enumerate(b_messages):
+                                r = dill.loads(b_message)
+                                tid = r["task_id"]
+
+                                log.debug(
+                                    "Received task result %s (from %s)", tid, manager
+                                )
+                                task_container = self.containers[r["container_id"]]
+                                log.debug(
+                                    "Removing for manager: %s from %s",
+                                    manager,
+                                    self._ready_manager_queue,
+                                )
+
+                                mdata["tasks"][task_container].remove(tid)
+
+                                # Transfer any outstanding task statuses to the
+                                # result message
+                                if tid in self.task_status_deltas:
+                                    r["task_statuses"] += self.task_status_deltas[tid]
+                                    del self.task_status_deltas[tid]
+                                    b_messages[idx] = dill.dumps(r)
+                                    log.debug(
+                                        "Transferring statuses for %s: %s",
+                                        tid,
+                                        r["task_statuses"],
+                                    )
 
-                    mdata["total_tasks"] -= len(b_messages)
+                        mdata["total_tasks"] -= len(b_messages)
 
                     # TODO: handle this with a Task message or something?
                     # previously used this; switched to mono-message,
                     # self.results_outgoing.send_multipart(b_messages)
                     self.results_outgoing.send(dill.dumps(b_messages))
                     interesting_managers.add(manager)
 
@@ -973,21 +997,20 @@
             try:
                 packed_status_report = status_report_queue.get(block=False)
                 log.trace("forwarding status report: %s", packed_status_report)
                 self.results_outgoing.send(packed_status_report)
             except queue.Empty:
                 pass
 
-            log.trace("entering bad_managers section")
             now = time.time()
             hbt_window_start = now - self.heartbeat_threshold
             bad_managers = [
                 manager
-                for manager in self._ready_manager_queue
-                if hbt_window_start > self._ready_manager_queue[manager]["last"]
+                for manager, mdata in self._ready_manager_queue.items()
+                if hbt_window_start > mdata["last"]
             ]
             bad_manager_msgs = []
             for manager in bad_managers:
                 log.debug(
                     "Last: %s Current: %s",
                     self._ready_manager_queue[manager]["last"],
                     now,
@@ -1008,15 +1031,14 @@
                 log.warning(f"Unregistering manager {manager!r}")
                 self._ready_manager_queue.pop(manager, None)
                 if manager in interesting_managers:
                     interesting_managers.remove(manager)
             if bad_manager_msgs:
                 log.warning(f"Sending task failure reports of manager {manager!r}")
                 self.results_outgoing.send(dill.dumps(bad_manager_msgs))
-            log.trace("ending one main loop iteration")
 
         delta = time.time() - start
         log.info(f"Processed {count} tasks in {delta} seconds")
         log.warning("Exiting")
 
     def get_global_state_for_status_report(self):
         outstanding_tasks = self.get_total_tasks_outstanding()
@@ -1030,14 +1052,15 @@
 
         return {
             "managers": num_managers,
             "total_workers": live_workers,
             "idle_workers": free_capacity,
             "pending_tasks": pending_tasks,
             "outstanding_tasks": outstanding_tasks,
+            "heartbeat_period": self.heartbeat_period,
         }
 
     def scale_out(self, blocks=1, task_type=None):
         """Scales out the number of blocks by "blocks"
 
         Raises:
              NotImplementedError
@@ -1127,16 +1150,17 @@
 
     def provider_status(self):
         """Get status of all blocks from the provider. The return type is
         defined by the particular provider in use.
         """
         status = []
         if self.provider:
-            log.trace("Getting the status of %s blocks.", list(self.blocks.values()))
-            status = self.provider.status(list(self.blocks.values()))
+            job_ids: list[str] = list(self.blocks.values())
+            log.trace("Getting the status of %s blocks.", job_ids)
+            status = self.provider.status(job_ids)
             log.trace("The status is %s", status)
 
         return status
 
 
 def starter(comm_q: mp.Queue, *args, **kwargs) -> None:
     """Start the interchange process
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,24 +312,31 @@
         self.task_incoming.send(msg)
         last_interchange_contact = time.time()
         task_recv_counter = 0
 
         poll_timer = self.poll_period
 
         new_worker_map = None
+        last_count_pending = -1
+        last_count_worker = -1
         while not kill_event.is_set():
             # Disabling the check on ready_worker_queue disables batching
-            log.trace("Loop start")
             pending_task_count = task_recv_counter - self.task_done_counter
             ready_worker_count = self.worker_map.ready_worker_count()
-            log.trace(
-                "pending_task_count: %s, Ready_worker_count: %s",
+            if (last_count_pending, last_count_worker) != (
                 pending_task_count,
                 ready_worker_count,
-            )
+            ):
+                log.trace(
+                    "pending_task_count: %s, Ready_worker_count: %s",
+                    pending_task_count,
+                    ready_worker_count,
+                )
+                last_count_pending = pending_task_count
+                last_count_worker = ready_worker_count
 
             if pending_task_count < self.max_queue_size and ready_worker_count > 0:
                 ads = self.worker_map.advertisement()
                 log.trace("Requesting tasks: %s", ads)
                 msg = dill.dumps(ads)
                 self.task_incoming.send(msg)
 
@@ -663,16 +670,17 @@
         while not kill_event.wait(timeout=self.heartbeat_period):
             msg = ManagerStatusReport(
                 self.task_status_deltas,
                 self.container_switch_count,
             )
             log.info(f"Sending status report to interchange: {msg.task_statuses}")
             self.pending_result_queue.put(msg)
-            log.info("Clearing task deltas")
-            self.task_status_deltas.clear()
+            if self.task_status_deltas:
+                log.info("Clearing task deltas")
+                self.task_status_deltas.clear()
 
     def push_results(self, kill_event, max_result_batch_size=1):
         """Listens on the pending_result_queue and sends out results via 0mq
 
         Parameters:
         -----------
         kill_event : threading.Event
@@ -856,30 +864,33 @@
 
     setup_logging(
         logfile=os.path.join(args.logdir, args.uid, "manager.log"), debug=args.debug
     )
 
     try:
         log.info(f"Python version: {sys.version}")
-        log.info(f"Debug logging: {args.debug}")
-        log.info(f"Log dir: {args.logdir}")
-        log.info(f"Manager ID: {args.uid}")
-        log.info(f"Block ID: {args.block_id}")
-        log.info(f"cores_per_worker: {args.cores_per_worker}")
-        log.info(f"available_accelerators: {args.available_accelerators}")
-        log.info(f"task_url: {args.task_url}")
-        log.info(f"result_url: {args.result_url}")
-        log.info(f"hb_period: {args.hb_period}")
-        log.info(f"hb_threshold: {args.hb_threshold}")
-        log.info(f"max_workers: {args.max_workers}")
-        log.info(f"poll_period: {args.poll}")
-        log.info(f"worker_mode: {args.worker_mode}")
-        log.info(f"container_cmd_options: {args.container_cmd_options}")
-        log.info(f"scheduler_mode: {args.scheduler_mode}")
-        log.info(f"worker_type: {args.worker_type}")
+        log.info(
+            "Arguments:"
+            f"\n  Debug logging: {args.debug}"
+            f"\n  Log dir: {args.logdir}"
+            f"\n  Manager ID: {args.uid}"
+            f"\n  Block ID: {args.block_id}"
+            f"\n  cores_per_worker: {args.cores_per_worker}"
+            f"\n  available_accelerators: {args.available_accelerators}"
+            f"\n  task_url: {args.task_url}"
+            f"\n  result_url: {args.result_url}"
+            f"\n  hb_period: {args.hb_period}"
+            f"\n  hb_threshold: {args.hb_threshold}"
+            f"\n  max_workers: {args.max_workers}"
+            f"\n  poll_period: {args.poll}"
+            f"\n  worker_mode: {args.worker_mode}"
+            f"\n  container_cmd_options: {args.container_cmd_options}"
+            f"\n  scheduler_mode: {args.scheduler_mode}"
+            f"\n  worker_type: {args.worker_type}"
+        )
 
         manager = Manager(
             task_q_url=args.task_url,
             result_q_url=args.result_url,
             uid=args.uid,
             block_id=args.block_id,
             cores_per_worker=float(args.cores_per_worker),
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
 import random
 import subprocess
 import time
+from collections import defaultdict
 from queue import Empty, Queue
 from typing import Any
 
 from globus_compute_endpoint.logging_config import ComputeLogger
 
 log: ComputeLogger = logging.getLogger(__name__)  # type: ignore
 
@@ -58,14 +59,16 @@
         self.available_accelerators: Queue | None = None
         if len(available_accelerators) != 0:
             self.available_accelerators = Queue()
             for device in available_accelerators:
                 self.available_accelerators.put(device)
         self.assigned_accelerators: dict[str, str] = {}  # Map worker ID -> accelerator
 
+        self._noisy_log: dict[str, Any] = defaultdict(dict)
+
     def register_worker(self, worker_id, worker_type):
         """Add a new worker"""
         log.debug(f"In register worker worker_id: {worker_id} type:{worker_type}")
         self.worker_types[worker_id] = worker_type
 
         if worker_type not in self.worker_queues:
             self.worker_queues[worker_type] = Queue()
@@ -414,40 +417,44 @@
            {worker_type: total_number_of_containers,...}
 
         Returns
         ---------
         Queue containing the next workers the system should spin-up.
         """
 
-        # next_worker_q = []
-        new_worker_list = []
-        log.debug(
-            "total_worker_type_counts: %s",
+        _log_data = self._noisy_log["get_next_worker_q"]
+        _l_total = _log_data.get("total_worker_type_counts")
+        _l_pending = _log_data.get("pending_worker_type_counts")
+        if (_l_total, _l_pending) != (
             self.total_worker_type_counts,
-        )
-        log.debug(
-            "pending_worker_type_counts: %s",
             self.pending_worker_type_counts,
-        )
+        ):
+            log.debug(
+                "total_worker_type_counts: %s; pending_worker_type_counts: %s",
+                self.total_worker_type_counts,
+                self.pending_worker_type_counts,
+            )
+            _log_data["total_worker_type_counts"] = self.total_worker_type_counts
+            _log_data["pending_worker_type_counts"] = self.pending_worker_type_counts
+
+        new_worker_list = []
         for worker_type in new_worker_map:
             cur_workers = self.total_worker_type_counts.get(
                 worker_type, 0
             ) + self.pending_worker_type_counts.get(worker_type, 0)
             if new_worker_map[worker_type] > cur_workers:
                 for _i in range(new_worker_map[worker_type] - cur_workers):
                     # Add worker
                     new_worker_list.append(worker_type)
 
         # need_more is to reflect if a manager needs more workers than the current
         # unused slots
         # If yes, that means the manager needs to turn off some warm workers to serve
         # the requests
-        need_more = False
-        if len(new_worker_list) > self.total_worker_type_counts["unused"]:
-            need_more = True
+        need_more = len(new_worker_list) > self.total_worker_type_counts["unused"]
         # Randomly assign order of newly needed containers... add to spin-up queue.
         if len(new_worker_list) > 0:
             random.shuffle(new_worker_list)
 
         return new_worker_list, need_more
 
     def update_worker_idle(self, worker_type):
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import queue
 import time
 from typing import Any, Dict, List, Optional, Tuple
 
 import typeguard
 from globus_compute_endpoint.providers.kubernetes.template import template_string
 from parsl.errors import OptionalModuleMissing
@@ -199,15 +200,14 @@
              - job_ids (list) : A list of job identifiers
         Returns:
              - A dictionary keyed by task_types, containing the count of
                known pods known with that task type.
                For example: {"RAW": 16}
         """
         # This is a hack
-        log.debug("Getting Kubernetes provider status")
         status = {}
         for jid in job_ids:
             if jid in self.resources_by_pod_name:
                 task_type = self.resources_by_pod_name[jid]["task_type"]
                 status[task_type] = status.get(task_type, 0) + 1
 
         return status
@@ -285,15 +285,18 @@
             security_context = client.V1SecurityContext(
                 run_as_group=self.group_id,
                 run_as_user=self.user_id,
                 run_as_non_root=self.run_as_non_root,
             )
 
         # Create the enviornment variables and command to initiate IPP
-        environment_vars = client.V1EnvVar(name="TEST", value="SOME DATA")
+        env = []
+        for var_name in ("GC_TASK_TIMEOUT",):
+            if var_name in os.environ:
+                env.append(client.V1EnvVar(name=var_name, value=os.getenv(var_name)))
 
         launch_args = ["-c", f"{cmd_string}"]
 
         volume_mounts = []
         # Create mount paths for the volumes
         for volume in volumes:
             volume_mounts.append(
@@ -308,15 +311,15 @@
             name=pod_name,
             image=image,
             resources=resources,
             ports=[client.V1ContainerPort(container_port=port)],
             volume_mounts=volume_mounts,
             command=["/bin/bash"],
             args=launch_args,
-            env=[environment_vars],
+            env=env,
             security_context=security_context,
         )
 
         # Create a secret to enable pulling images from secure repositories
         secret = None
         if self.secret:
             secret = client.V1LocalObjectReference(name=self.secret)
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import math
 import time
+from collections import defaultdict
 
 from globus_compute_endpoint.logging_config import ComputeLogger
 from globus_compute_endpoint.strategies.base import BaseStrategy
 
 log: ComputeLogger = logging.getLogger(__name__)  # type: ignore
 
 
@@ -26,18 +27,19 @@
 
         max_idletime: (int)
           maximum idle time(seconds) allowed for resources after which strategy will
           try to kill them.
           default: 60s
 
         """
-        log.info("KubeSimpleStrategy Initialized")
         super().__init__(*args, threshold=threshold, interval=interval)
         self.max_idletime = max_idletime
         self.executors_idle_since = {}
+        self._task_type_status_msg = defaultdict(str)
+        log.info(f"KubeSimpleStrategy Initialized; max idle time: {max_idletime}s")
 
     def strategize(self, *args, **kwargs):
         try:
             self._strategize(*args, **kwargs)
         except Exception as e:
             log.exception(f"Caught error in strategize : {e}")
 
@@ -56,28 +58,35 @@
 
         active_tasks = self.interchange.get_total_tasks_outstanding()
         log.trace("Pending tasks : %s", active_tasks)
 
         status = self.interchange.provider_status()
         log.trace("Provider status : %s", status)
 
+        task_dbg_msg = (
+            "Endpoint has %s active tasks of %s, %s active blocks, "
+            "%s connected workers for %s"
+        )
+
         for task_type in active_tasks.keys():
             active_pods = status.get(task_type, 0)
             active_slots = active_pods * workers_per_pod * managers_per_pod
             active_tasks_per_type = active_tasks[task_type]
 
-            log.debug(
-                "Endpoint has %s active tasks of %s, %s active blocks, "
-                "%s connected workers for %s",
+            _tmp = task_dbg_msg % (
                 active_tasks_per_type,
                 task_type,
                 active_pods,
                 self.interchange.get_total_live_workers(),
                 task_type,
             )
+            if _tmp != self._task_type_status_msg[task_type]:
+                # Quiet some not-helpful logs
+                self._task_type_status_msg[task_type] = _tmp
+                log.debug(_tmp)
 
             # Reset the idle time if we are currently running tasks
             if active_tasks_per_type > 0:
                 self.executors_idle_since[task_type] = None
 
             # Scale down only if there are no active tasks to avoid having to find which
             # workers are unoccupied
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a4"
+__version__ = "2.0.2a0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a4
+Version: 2.0.2a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a4/setup.py` & `globus-compute-endpoint-2.0.2a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk>=2.0.1a4",
+    "globus-compute-sdk>=2.0.2a0",
     "globus-compute-common==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.0.1a4/tests/conftest.py` & `globus-compute-endpoint-2.0.2a0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,24 +69,24 @@
         ...
 
     def get_auth_client(self) -> globus_sdk.AuthClient:
         return globus_sdk.AuthClient(authorizer=globus_sdk.NullAuthorizer())
 
     def get_web_client(self, *, base_url: str | None = None) -> WebClient:
         return WebClient(
-            base_url="https://api2.funcx.org/v2/",
+            base_url="https://compute.api.globus.org/v2/",
             authorizer=globus_sdk.NullAuthorizer(),
         )
 
 
 @pytest.fixture
 def get_standard_compute_client():
     responses.add(
         method=responses.GET,
-        url="https://api2.funcx.org/v2/version",
+        url="https://compute.api.globus.org/v2/version",
         headers={"Content-Type": "application/json"},
         json={"api": "0.4.0", "min_ep_version": "0.0.0", "min_sdk_version": "0.0.0"},
     )
 
     def func():
         return gc.Client(
             login_manager=FakeLoginManager(),
```

### Comparing `globus-compute-endpoint-2.0.1a4/tests/utils.py` & `globus-compute-endpoint-2.0.2a0/tests/utils.py`

 * *Files identical despite different names*

