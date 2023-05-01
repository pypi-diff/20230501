# Comparing `tmp/hivemind-1.1.7.tar.gz` & `tmp/hivemind-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivemind-1.1.7.tar", last modified: Fri Mar 31 13:56:35 2023, max compression
+gzip compressed data, was "hivemind-1.1.8.tar", last modified: Mon May  1 16:11:19 2023, max compression
```

## Comparing `hivemind-1.1.7.tar` & `hivemind-1.1.8.tar`

### file list

```diff
@@ -1,154 +1,126 @@
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.622149 hivemind-1.1.7/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1096 2021-02-19 07:15:37.000000 hivemind-1.1.7/LICENSE
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1295 2023-03-31 13:56:35.621209 hivemind-1.1.7/PKG-INFO
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10865 2023-03-31 13:55:15.000000 hivemind-1.1.7/README.md
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.294290 hivemind-1.1.7/hivemind/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      479 2023-03-31 13:55:37.000000 hivemind-1.1.7/hivemind/__init__.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.323966 hivemind-1.1.7/hivemind/averaging/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)       62 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    18412 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/allreduce.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    39698 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/averager.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6511 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/control.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      671 2021-08-11 06:04:46.000000 hivemind-1.1.7/hivemind/averaging/group_info.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5436 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/key_manager.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5450 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/load_balancing.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    28174 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/matchmaking.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    14877 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/averaging/partition.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.348024 hivemind-1.1.7/hivemind/compression/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      658 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/compression/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2823 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/compression/adaptive.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5345 2023-03-31 13:55:15.000000 hivemind-1.1.7/hivemind/compression/base.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4067 2022-06-08 15:22:00.000000 hivemind-1.1.7/hivemind/compression/floating.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8300 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/compression/quantization.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2846 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/compression/serialization.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.379327 hivemind-1.1.7/hivemind/dht/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1057 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/dht/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3595 2021-08-11 06:04:46.000000 hivemind-1.1.7/hivemind/dht/crypto.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    14912 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/dht/dht.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    52055 2023-03-31 13:55:14.000000 hivemind-1.1.7/hivemind/dht/node.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    22566 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/dht/protocol.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15550 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/dht/routing.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7304 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/dht/schema.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3757 2021-08-11 06:04:46.000000 hivemind-1.1.7/hivemind/dht/storage.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15234 2021-08-11 06:04:46.000000 hivemind-1.1.7/hivemind/dht/traverse.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4555 2021-07-12 19:08:17.000000 hivemind-1.1.7/hivemind/dht/validation.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.415632 hivemind-1.1.7/hivemind/hivemind_cli/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2021-04-02 18:12:53.000000 hivemind-1.1.7/hivemind/hivemind_cli/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      181 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/hivemind_cli/config.yml
--rwxrwxrwx   0 mryab    (1786541415) LD\Domain Users (593637566)  9172340 2023-01-03 13:33:41.000000 hivemind-1.1.7/hivemind/hivemind_cli/p2pd
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3325 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/hivemind_cli/run_dht.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6370 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/hivemind_cli/run_server.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.418914 hivemind-1.1.7/hivemind/moe/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      254 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/__init__.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.430638 hivemind-1.1.7/hivemind/moe/client/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      183 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/client/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    20911 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/client/beam_search.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     9758 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/client/expert.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    20442 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/client/moe.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1120 2023-03-31 13:55:15.000000 hivemind-1.1.7/hivemind/moe/client/remote_expert_worker.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10484 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/client/switch_moe.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1644 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/expert_uid.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.447421 hivemind-1.1.7/hivemind/moe/server/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      260 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2731 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/checkpoints.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7267 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/connection_handler.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4945 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/dht_handler.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.463757 hivemind-1.1.7/hivemind/moe/server/layers/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      398 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/layers/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3283 2021-07-12 19:08:17.000000 hivemind-1.1.7/hivemind/moe/server/layers/common.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1182 2021-08-11 06:04:46.000000 hivemind-1.1.7/hivemind/moe/server/layers/custom_experts.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1732 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/layers/dropout.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1209 2021-07-03 15:49:22.000000 hivemind-1.1.7/hivemind/moe/server/layers/lr_schedule.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1775 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/layers/optim.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     9743 2023-03-31 13:55:14.000000 hivemind-1.1.7/hivemind/moe/server/module_backend.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8835 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/runtime.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    17792 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/server.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10951 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/moe/server/task_pool.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.500989 hivemind-1.1.7/hivemind/optim/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      179 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/optim/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    12669 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/optim/grad_averager.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6239 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/optim/grad_scaler.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    45413 2023-03-31 13:55:14.000000 hivemind-1.1.7/hivemind/optim/optimizer.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10944 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/optim/power_sgd_averager.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    17452 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/optim/progress_tracker.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    40626 2023-03-31 13:55:14.000000 hivemind-1.1.7/hivemind/optim/state_averager.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    12900 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/optim/training_averager.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.507257 hivemind-1.1.7/hivemind/p2p/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      204 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    30416 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/p2p_daemon.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.515163 hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      160 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    16666 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/control.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5992 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/datastructures.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4373 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/p2pclient.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2271 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/utils.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6393 2023-03-31 13:55:15.000000 hivemind-1.1.7/hivemind/p2p/servicer.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.539132 hivemind-1.1.7/hivemind/proto/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      441 2022-06-16 10:08:09.000000 hivemind-1.1.7/hivemind/proto/auth.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2572 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/auth_pb2.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3672 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/proto/averaging.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5102 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/averaging_pb2.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      407 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/proto/crypto.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2148 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/crypto_pb2.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3364 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/proto/dht.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5846 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/dht_pb2.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4607 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/proto/p2pd.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    19245 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/p2pd_pb2.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      599 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/proto/runtime.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3878 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/runtime_pb2.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      114 2022-06-16 10:08:09.000000 hivemind-1.1.7/hivemind/proto/test.proto
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1609 2023-03-11 13:51:45.000000 hivemind-1.1.7/hivemind/proto/test_pb2.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.571040 hivemind-1.1.7/hivemind/utils/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      628 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/__init__.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7162 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/asyncio.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7781 2022-06-08 15:22:00.000000 hivemind-1.1.7/hivemind/utils/auth.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3293 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/crypto.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      740 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/limits.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6748 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/logging.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      849 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/math.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15185 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/mpfuture.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2622 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/nested.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2712 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/networking.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3225 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/performance_ema.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2637 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/serializer.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1611 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/streaming.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4657 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/tensor_descr.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5533 2023-03-31 13:53:53.000000 hivemind-1.1.7/hivemind/utils/timed_storage.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.301203 hivemind-1.1.7/hivemind.egg-info/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1295 2023-03-31 13:56:35.000000 hivemind-1.1.7/hivemind.egg-info/PKG-INFO
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3979 2023-03-31 13:56:35.000000 hivemind-1.1.7/hivemind.egg-info/SOURCES.txt
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)        1 2023-03-31 13:56:35.000000 hivemind-1.1.7/hivemind.egg-info/dependency_links.txt
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      124 2023-03-31 13:56:35.000000 hivemind-1.1.7/hivemind.egg-info/entry_points.txt
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      779 2023-03-31 13:56:35.000000 hivemind-1.1.7/hivemind.egg-info/requires.txt
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)        9 2023-03-31 13:56:35.000000 hivemind-1.1.7/hivemind.egg-info/top_level.txt
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      222 2023-03-31 13:53:53.000000 hivemind-1.1.7/pyproject.toml
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)       38 2023-03-31 13:56:35.622302 hivemind-1.1.7/setup.cfg
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6803 2023-03-31 13:53:53.000000 hivemind-1.1.7/setup.py
-drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-03-31 13:56:35.618774 hivemind-1.1.7/tests/
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     9981 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_allreduce.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8978 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_allreduce_fault_tolerance.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6048 2022-06-08 15:22:00.000000 hivemind-1.1.7/tests/test_auth.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    18064 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_averaging.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2118 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_cli_scripts.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     9410 2023-03-31 13:55:15.000000 hivemind-1.1.7/tests/test_compression.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7574 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_connection_handler.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2292 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_custom_experts.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3929 2023-03-31 13:53:53.000000 hivemind-1.1.7/tests/test_dht.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5419 2022-05-31 15:27:03.000000 hivemind-1.1.7/tests/test_dht_crypto.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8918 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_dht_experts.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    12652 2022-06-03 08:59:12.000000 hivemind-1.1.7/tests/test_dht_node.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6855 2021-08-26 07:54:05.000000 hivemind-1.1.7/tests/test_dht_protocol.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8151 2021-07-12 19:08:17.000000 hivemind-1.1.7/tests/test_dht_schema.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5972 2021-08-11 06:04:46.000000 hivemind-1.1.7/tests/test_dht_storage.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3766 2021-08-11 06:04:46.000000 hivemind-1.1.7/tests/test_dht_validation.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3531 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_expert_backend.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    13210 2023-03-31 13:55:15.000000 hivemind-1.1.7/tests/test_moe.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    17305 2023-03-31 13:55:14.000000 hivemind-1.1.7/tests/test_optimizer.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15355 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_p2p_daemon.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    20371 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_p2p_daemon_bindings.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6953 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_p2p_servicer.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1715 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_relays.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6251 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_routing.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2973 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_start_server.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4987 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_training.py
--rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    19217 2023-03-31 13:53:54.000000 hivemind-1.1.7/tests/test_util_modules.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.793133 hivemind-1.1.8/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1096 2021-02-19 07:15:37.000000 hivemind-1.1.8/LICENSE
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1314 2023-05-01 16:11:19.792395 hivemind-1.1.8/PKG-INFO
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10865 2023-03-31 13:55:15.000000 hivemind-1.1.8/README.md
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.498956 hivemind-1.1.8/hivemind/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      479 2023-05-01 16:10:38.000000 hivemind-1.1.8/hivemind/__init__.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.514307 hivemind-1.1.8/hivemind/averaging/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)       62 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    18412 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/allreduce.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    39698 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/averager.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6511 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/control.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      671 2021-08-11 06:04:46.000000 hivemind-1.1.8/hivemind/averaging/group_info.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5436 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/key_manager.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5450 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/load_balancing.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    28174 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/matchmaking.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    14877 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/averaging/partition.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.538033 hivemind-1.1.8/hivemind/compression/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      658 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/compression/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2823 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/compression/adaptive.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5178 2023-05-01 16:02:30.000000 hivemind-1.1.8/hivemind/compression/base.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4067 2022-06-08 15:22:00.000000 hivemind-1.1.8/hivemind/compression/floating.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8300 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/compression/quantization.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2846 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/compression/serialization.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.550740 hivemind-1.1.8/hivemind/dht/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1057 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/dht/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3595 2021-08-11 06:04:46.000000 hivemind-1.1.8/hivemind/dht/crypto.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    14912 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/dht/dht.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    52055 2023-03-31 13:55:14.000000 hivemind-1.1.8/hivemind/dht/node.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    22566 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/dht/protocol.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15550 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/dht/routing.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7304 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/dht/schema.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3757 2021-08-11 06:04:46.000000 hivemind-1.1.8/hivemind/dht/storage.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15234 2021-08-11 06:04:46.000000 hivemind-1.1.8/hivemind/dht/traverse.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4555 2021-07-12 19:08:17.000000 hivemind-1.1.8/hivemind/dht/validation.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.587394 hivemind-1.1.8/hivemind/hivemind_cli/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2021-04-02 18:12:53.000000 hivemind-1.1.8/hivemind/hivemind_cli/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      181 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/hivemind_cli/config.yml
+-rwxrwxrwx   0 mryab    (1786541415) LD\Domain Users (593637566)  9172340 2023-01-03 13:33:41.000000 hivemind-1.1.8/hivemind/hivemind_cli/p2pd
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3325 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/hivemind_cli/run_dht.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6370 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/hivemind_cli/run_server.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.589454 hivemind-1.1.8/hivemind/moe/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      254 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/__init__.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.596790 hivemind-1.1.8/hivemind/moe/client/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      183 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/client/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    20911 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/client/beam_search.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     9758 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/client/expert.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    20442 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/client/moe.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1120 2023-03-31 13:55:15.000000 hivemind-1.1.8/hivemind/moe/client/remote_expert_worker.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10484 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/client/switch_moe.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1644 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/expert_uid.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.605356 hivemind-1.1.8/hivemind/moe/server/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      260 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2731 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/checkpoints.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7267 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/connection_handler.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4945 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/dht_handler.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.612025 hivemind-1.1.8/hivemind/moe/server/layers/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      398 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/layers/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3283 2021-07-12 19:08:17.000000 hivemind-1.1.8/hivemind/moe/server/layers/common.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1182 2021-08-11 06:04:46.000000 hivemind-1.1.8/hivemind/moe/server/layers/custom_experts.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1732 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/layers/dropout.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1209 2021-07-03 15:49:22.000000 hivemind-1.1.8/hivemind/moe/server/layers/lr_schedule.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1775 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/layers/optim.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     9743 2023-03-31 13:55:14.000000 hivemind-1.1.8/hivemind/moe/server/module_backend.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     8835 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/runtime.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    17792 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/server.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10951 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/moe/server/task_pool.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.637466 hivemind-1.1.8/hivemind/optim/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      179 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/optim/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    12669 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/optim/grad_averager.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6239 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/optim/grad_scaler.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    45413 2023-03-31 13:55:14.000000 hivemind-1.1.8/hivemind/optim/optimizer.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    10944 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/optim/power_sgd_averager.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    17452 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/optim/progress_tracker.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    40626 2023-03-31 13:55:14.000000 hivemind-1.1.8/hivemind/optim/state_averager.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    12900 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/optim/training_averager.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.640612 hivemind-1.1.8/hivemind/p2p/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      204 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/p2p/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    30471 2023-05-01 16:02:30.000000 hivemind-1.1.8/hivemind/p2p/p2p_daemon.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.645624 hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      160 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    16666 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/control.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5992 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/datastructures.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4414 2023-05-01 16:02:30.000000 hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/p2pclient.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2271 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/utils.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6393 2023-03-31 13:55:15.000000 hivemind-1.1.8/hivemind/p2p/servicer.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.702378 hivemind-1.1.8/hivemind/proto/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      441 2022-06-16 10:08:09.000000 hivemind-1.1.8/hivemind/proto/auth.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2572 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/auth_pb2.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3672 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/proto/averaging.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5102 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/averaging_pb2.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      407 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/proto/crypto.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2148 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/crypto_pb2.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3364 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/proto/dht.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5846 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/dht_pb2.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4607 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/proto/p2pd.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    19245 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/p2pd_pb2.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      599 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/proto/runtime.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3878 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/runtime_pb2.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      114 2022-06-16 10:08:09.000000 hivemind-1.1.8/hivemind/proto/test.proto
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1609 2023-03-11 13:51:45.000000 hivemind-1.1.8/hivemind/proto/test_pb2.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.790797 hivemind-1.1.8/hivemind/utils/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      628 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/__init__.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7162 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/asyncio.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     7781 2022-06-08 15:22:00.000000 hivemind-1.1.8/hivemind/utils/auth.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3293 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/crypto.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      740 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/limits.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6748 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/logging.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      849 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/math.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)    15185 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/mpfuture.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2622 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/nested.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2712 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/networking.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3225 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/performance_ema.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     2637 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/serializer.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1611 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/streaming.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     4657 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/tensor_descr.py
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     5533 2023-03-31 13:53:53.000000 hivemind-1.1.8/hivemind/utils/timed_storage.py
+drwxr-xr-x   0 mryab    (1786541415) LD\Domain Users (593637566)        0 2023-05-01 16:11:19.504021 hivemind-1.1.8/hivemind.egg-info/
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     1314 2023-05-01 16:11:19.000000 hivemind-1.1.8/hivemind.egg-info/PKG-INFO
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     3282 2023-05-01 16:11:19.000000 hivemind-1.1.8/hivemind.egg-info/SOURCES.txt
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)        1 2023-05-01 16:11:19.000000 hivemind-1.1.8/hivemind.egg-info/dependency_links.txt
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      125 2023-05-01 16:11:19.000000 hivemind-1.1.8/hivemind.egg-info/entry_points.txt
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      779 2023-05-01 16:11:19.000000 hivemind-1.1.8/hivemind.egg-info/requires.txt
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)        9 2023-05-01 16:11:19.000000 hivemind-1.1.8/hivemind.egg-info/top_level.txt
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)      222 2023-03-31 13:53:53.000000 hivemind-1.1.8/pyproject.toml
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)       38 2023-05-01 16:11:19.793339 hivemind-1.1.8/setup.cfg
+-rw-r--r--   0 mryab    (1786541415) LD\Domain Users (593637566)     6803 2023-03-31 13:53:53.000000 hivemind-1.1.8/setup.py
```

### Comparing `hivemind-1.1.7/LICENSE` & `hivemind-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/PKG-INFO` & `hivemind-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: hivemind
-Version: 1.1.7
+Version: 1.1.8
 Summary: Decentralized deep learning in PyTorch
 Home-page: https://github.com/learning-at-home/hivemind
 Author: Learning@home & contributors
 Author-email: hivemind-team@hotmail.com
 License: MIT
 Keywords: pytorch,deep learning,machine learning,gpu,distributed computing,volunteer computing,dht
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,7 +25,8 @@
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: bitsandbytes
 Provides-Extra: all
 License-File: LICENSE
 
 Decentralized deep learning in PyTorch. Built to train models on thousands of volunteers across the world.
+
```

### Comparing `hivemind-1.1.7/README.md` & `hivemind-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/allreduce.py` & `hivemind-1.1.8/hivemind/averaging/allreduce.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/averager.py` & `hivemind-1.1.8/hivemind/averaging/averager.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/control.py` & `hivemind-1.1.8/hivemind/averaging/control.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/group_info.py` & `hivemind-1.1.8/hivemind/averaging/group_info.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/key_manager.py` & `hivemind-1.1.8/hivemind/averaging/key_manager.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/load_balancing.py` & `hivemind-1.1.8/hivemind/averaging/load_balancing.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/matchmaking.py` & `hivemind-1.1.8/hivemind/averaging/matchmaking.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/averaging/partition.py` & `hivemind-1.1.8/hivemind/averaging/partition.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/compression/__init__.py` & `hivemind-1.1.8/hivemind/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/compression/adaptive.py` & `hivemind-1.1.8/hivemind/compression/adaptive.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/compression/base.py` & `hivemind-1.1.8/hivemind/compression/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,40 +83,39 @@
 
     def compress(self, tensor: torch.Tensor, info: CompressionInfo, allow_inplace: bool = False) -> runtime_pb2.Tensor:
         tensor = tensor.detach()
         shape = tensor.shape
         dtype_name = str(tensor.dtype).lstrip("torch.")
         raw_data = tensor
         if tensor.dtype == torch.bfloat16:
-            if USE_LEGACY_BFLOAT16:
+            if USE_LEGACY_BFLOAT16:  # legacy mode: convert to fp32
                 raw_data = tensor.to(torch.float32)
-            else:
-                typed_storage = tensor.storage()
-                storage = typed_storage.untyped() if hasattr(typed_storage, "untyped") else typed_storage._untyped()
-                raw_data = torch.tensor(storage, dtype=torch.int8)
+            else:  # efficient mode: send bfloat16 data directly
+                # reinterpret_cast to an arbitrary 2-byte type supported by numpy
+                raw_data = tensor.view(torch.int16)
 
         return runtime_pb2.Tensor(
             compression=self.compression_type,
             buffer=raw_data.numpy().tobytes(),
             size=shape,
             dtype=dtype_name,
             requires_grad=tensor.requires_grad,
         )
 
     def extract(self, serialized_tensor: runtime_pb2.Tensor) -> torch.Tensor:
         shape = torch.Size(serialized_tensor.size)
         if serialized_tensor.dtype == "bfloat16":
             numel = shape.numel()
-            if numel > 0 and len(serialized_tensor.buffer) // numel == 4:  # legacy mode: convert to fp32
+            if numel > 0 and len(serialized_tensor.buffer) // numel == 4:
                 array = np.frombuffer(serialized_tensor.buffer, dtype=np.float32)
                 tensor = torch.as_tensor(array, dtype=torch.bfloat16)
-            else:  # efficient mode: send bfloat16 data directly
-                storage_type = torch.TypedStorage if hasattr(torch, "TypedStorage") else torch._TypedStorage
-                storage = storage_type.from_buffer(serialized_tensor.buffer, byte_order="little", dtype=torch.bfloat16)
-                tensor = torch.as_tensor(storage, dtype=torch.bfloat16)
+            else:
+                array = np.frombuffer(serialized_tensor.buffer, dtype=np.int16)
+                # reinterpret_cast from an arbitrary 2-byte type supported by numpy
+                tensor = torch.as_tensor(array).view(torch.bfloat16)
         else:
             array = np.frombuffer(serialized_tensor.buffer, dtype=np.dtype(serialized_tensor.dtype))
             tensor = torch.as_tensor(array)
         return tensor.reshape(shape)
 
     def estimate_compression_ratio(self, info: CompressionInfo) -> float:
         return 1.0
```

### Comparing `hivemind-1.1.7/hivemind/compression/floating.py` & `hivemind-1.1.8/hivemind/compression/floating.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/compression/quantization.py` & `hivemind-1.1.8/hivemind/compression/quantization.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/compression/serialization.py` & `hivemind-1.1.8/hivemind/compression/serialization.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/__init__.py` & `hivemind-1.1.8/hivemind/dht/__init__.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/crypto.py` & `hivemind-1.1.8/hivemind/dht/crypto.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/dht.py` & `hivemind-1.1.8/hivemind/dht/dht.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/node.py` & `hivemind-1.1.8/hivemind/dht/node.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/protocol.py` & `hivemind-1.1.8/hivemind/dht/protocol.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/routing.py` & `hivemind-1.1.8/hivemind/dht/routing.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/schema.py` & `hivemind-1.1.8/hivemind/dht/schema.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/storage.py` & `hivemind-1.1.8/hivemind/dht/storage.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/traverse.py` & `hivemind-1.1.8/hivemind/dht/traverse.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/dht/validation.py` & `hivemind-1.1.8/hivemind/dht/validation.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/hivemind_cli/p2pd` & `hivemind-1.1.8/hivemind/hivemind_cli/p2pd`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/hivemind_cli/run_dht.py` & `hivemind-1.1.8/hivemind/hivemind_cli/run_dht.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/hivemind_cli/run_server.py` & `hivemind-1.1.8/hivemind/hivemind_cli/run_server.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/client/beam_search.py` & `hivemind-1.1.8/hivemind/moe/client/beam_search.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/client/expert.py` & `hivemind-1.1.8/hivemind/moe/client/expert.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/client/moe.py` & `hivemind-1.1.8/hivemind/moe/client/moe.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/client/remote_expert_worker.py` & `hivemind-1.1.8/hivemind/moe/client/remote_expert_worker.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/client/switch_moe.py` & `hivemind-1.1.8/hivemind/moe/client/switch_moe.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/expert_uid.py` & `hivemind-1.1.8/hivemind/moe/expert_uid.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/checkpoints.py` & `hivemind-1.1.8/hivemind/moe/server/checkpoints.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/connection_handler.py` & `hivemind-1.1.8/hivemind/moe/server/connection_handler.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/dht_handler.py` & `hivemind-1.1.8/hivemind/moe/server/dht_handler.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/layers/common.py` & `hivemind-1.1.8/hivemind/moe/server/layers/common.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/layers/custom_experts.py` & `hivemind-1.1.8/hivemind/moe/server/layers/custom_experts.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/layers/dropout.py` & `hivemind-1.1.8/hivemind/moe/server/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/layers/lr_schedule.py` & `hivemind-1.1.8/hivemind/moe/server/layers/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/layers/optim.py` & `hivemind-1.1.8/hivemind/moe/server/layers/optim.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/module_backend.py` & `hivemind-1.1.8/hivemind/moe/server/module_backend.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/runtime.py` & `hivemind-1.1.8/hivemind/moe/server/runtime.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/server.py` & `hivemind-1.1.8/hivemind/moe/server/server.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/moe/server/task_pool.py` & `hivemind-1.1.8/hivemind/moe/server/task_pool.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/grad_averager.py` & `hivemind-1.1.8/hivemind/optim/grad_averager.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/grad_scaler.py` & `hivemind-1.1.8/hivemind/optim/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/optimizer.py` & `hivemind-1.1.8/hivemind/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/power_sgd_averager.py` & `hivemind-1.1.8/hivemind/optim/power_sgd_averager.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/progress_tracker.py` & `hivemind-1.1.8/hivemind/optim/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/state_averager.py` & `hivemind-1.1.8/hivemind/optim/state_averager.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/optim/training_averager.py` & `hivemind-1.1.8/hivemind/optim/training_averager.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/p2p/p2p_daemon.py` & `hivemind-1.1.8/hivemind/p2p/p2p_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,16 +650,17 @@
         if self._listen_task is not None:
             self._listen_task.cancel()
         if self._reader_task is not None:
             self._reader_task.cancel()
 
         self._alive = False
         if self._child is not None and self._child.returncode is None:
-            self._child.terminate()
-            logger.debug(f"Terminated p2pd with id = {self.peer_id}")
+            with suppress(ProcessLookupError):
+                self._child.terminate()
+                logger.debug(f"Terminated p2pd with id = {self.peer_id}")
 
             with suppress(FileNotFoundError):
                 os.remove(self._daemon_listen_maddr["unix"])
         with suppress(FileNotFoundError):
             os.remove(self._client_listen_maddr["unix"])
 
     @staticmethod
```

### Comparing `hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/control.py` & `hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/control.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/datastructures.py` & `hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/datastructures.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/p2pclient.py` & `hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/p2pclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             listen_maddr=listen_maddr,
             persistent_conn_max_msg_size=persistent_conn_max_msg_size,
         )
 
         return client
 
     def close(self) -> None:
-        self.control.close()
+        if self.control is not None:
+            self.control.close()
 
     def __del__(self):
         self.close()
 
     @asynccontextmanager
     async def listen(self) -> AsyncIterator["Client"]:
         """
```

### Comparing `hivemind-1.1.7/hivemind/p2p/p2p_daemon_bindings/utils.py` & `hivemind-1.1.8/hivemind/p2p/p2p_daemon_bindings/utils.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/p2p/servicer.py` & `hivemind-1.1.8/hivemind/p2p/servicer.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/auth_pb2.py` & `hivemind-1.1.8/hivemind/proto/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/averaging.proto` & `hivemind-1.1.8/hivemind/proto/averaging.proto`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/averaging_pb2.py` & `hivemind-1.1.8/hivemind/proto/averaging_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/crypto_pb2.py` & `hivemind-1.1.8/hivemind/proto/crypto_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/dht.proto` & `hivemind-1.1.8/hivemind/proto/dht.proto`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/dht_pb2.py` & `hivemind-1.1.8/hivemind/proto/dht_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/p2pd.proto` & `hivemind-1.1.8/hivemind/proto/p2pd.proto`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/p2pd_pb2.py` & `hivemind-1.1.8/hivemind/proto/p2pd_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/runtime.proto` & `hivemind-1.1.8/hivemind/proto/runtime.proto`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/runtime_pb2.py` & `hivemind-1.1.8/hivemind/proto/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/proto/test_pb2.py` & `hivemind-1.1.8/hivemind/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/__init__.py` & `hivemind-1.1.8/hivemind/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/asyncio.py` & `hivemind-1.1.8/hivemind/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/auth.py` & `hivemind-1.1.8/hivemind/utils/auth.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/crypto.py` & `hivemind-1.1.8/hivemind/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/limits.py` & `hivemind-1.1.8/hivemind/utils/limits.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/logging.py` & `hivemind-1.1.8/hivemind/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/math.py` & `hivemind-1.1.8/hivemind/utils/math.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/mpfuture.py` & `hivemind-1.1.8/hivemind/utils/mpfuture.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/nested.py` & `hivemind-1.1.8/hivemind/utils/nested.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/networking.py` & `hivemind-1.1.8/hivemind/utils/networking.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/performance_ema.py` & `hivemind-1.1.8/hivemind/utils/performance_ema.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/serializer.py` & `hivemind-1.1.8/hivemind/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/streaming.py` & `hivemind-1.1.8/hivemind/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/tensor_descr.py` & `hivemind-1.1.8/hivemind/utils/tensor_descr.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind/utils/timed_storage.py` & `hivemind-1.1.8/hivemind/utils/timed_storage.py`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/hivemind.egg-info/PKG-INFO` & `hivemind-1.1.8/hivemind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: hivemind
-Version: 1.1.7
+Version: 1.1.8
 Summary: Decentralized deep learning in PyTorch
 Home-page: https://github.com/learning-at-home/hivemind
 Author: Learning@home & contributors
 Author-email: hivemind-team@hotmail.com
 License: MIT
 Keywords: pytorch,deep learning,machine learning,gpu,distributed computing,volunteer computing,dht
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,7 +25,8 @@
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: bitsandbytes
 Provides-Extra: all
 License-File: LICENSE
 
 Decentralized deep learning in PyTorch. Built to train models on thousands of volunteers across the world.
+
```

### Comparing `hivemind-1.1.7/hivemind.egg-info/SOURCES.txt` & `hivemind-1.1.8/hivemind.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -101,35 +101,8 @@
 hivemind/utils/mpfuture.py
 hivemind/utils/nested.py
 hivemind/utils/networking.py
 hivemind/utils/performance_ema.py
 hivemind/utils/serializer.py
 hivemind/utils/streaming.py
 hivemind/utils/tensor_descr.py
-hivemind/utils/timed_storage.py
-tests/test_allreduce.py
-tests/test_allreduce_fault_tolerance.py
-tests/test_auth.py
-tests/test_averaging.py
-tests/test_cli_scripts.py
-tests/test_compression.py
-tests/test_connection_handler.py
-tests/test_custom_experts.py
-tests/test_dht.py
-tests/test_dht_crypto.py
-tests/test_dht_experts.py
-tests/test_dht_node.py
-tests/test_dht_protocol.py
-tests/test_dht_schema.py
-tests/test_dht_storage.py
-tests/test_dht_validation.py
-tests/test_expert_backend.py
-tests/test_moe.py
-tests/test_optimizer.py
-tests/test_p2p_daemon.py
-tests/test_p2p_daemon_bindings.py
-tests/test_p2p_servicer.py
-tests/test_relays.py
-tests/test_routing.py
-tests/test_start_server.py
-tests/test_training.py
-tests/test_util_modules.py
+hivemind/utils/timed_storage.py
```

### Comparing `hivemind-1.1.7/hivemind.egg-info/requires.txt` & `hivemind-1.1.8/hivemind.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hivemind-1.1.7/setup.py` & `hivemind-1.1.8/setup.py`

 * *Files identical despite different names*

